# Comparing `tmp/agent_protocol-0.2.2.tar.gz` & `tmp/agent_protocol-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "agent_protocol-0.2.2.tar", max compression
+gzip compressed data, was "agent_protocol-0.2.3.tar", max compression
```

## Comparing `agent_protocol-0.2.2.tar` & `agent_protocol-0.2.3.tar`

### file list

```diff
@@ -1,14 +1,13 @@
--rw-r--r--   0        0        0     3009 2023-08-08 08:46:00.630377 agent_protocol-0.2.2/README.md
--rw-r--r--   0        0        0      353 2023-08-08 08:46:00.630377 agent_protocol-0.2.2/agent_protocol/__init__.py
--rw-r--r--   0        0        0     5057 2023-08-08 08:46:00.630377 agent_protocol-0.2.2/agent_protocol/agent.py
--rw-r--r--   0        0        0      600 2023-08-08 08:46:00.630377 agent_protocol-0.2.2/agent_protocol/cli.py
--rw-r--r--   0        0        0     3592 2023-08-08 08:46:00.630377 agent_protocol-0.2.2/agent_protocol/db.py
--rw-r--r--   0        0        0     2319 2023-08-08 08:46:00.630377 agent_protocol-0.2.2/agent_protocol/models.py
--rw-r--r--   0        0        0        0 2023-08-08 08:46:00.630377 agent_protocol-0.2.2/agent_protocol/router.py
--rw-r--r--   0        0        0      331 2023-08-08 08:46:00.630377 agent_protocol-0.2.2/agent_protocol/server.py
--rw-r--r--   0        0        0        0 2023-08-08 08:46:00.630377 agent_protocol-0.2.2/agent_protocol/utils/__init__.py
--rw-r--r--   0        0        0       35 2023-08-08 08:46:00.630377 agent_protocol-0.2.2/agent_protocol/utils/compliance/__init__.py
--rw-r--r--   0        0        0      449 2023-08-08 08:46:00.630377 agent_protocol-0.2.2/agent_protocol/utils/compliance/conftest.py
--rw-r--r--   0        0        0     3748 2023-08-08 08:46:00.630377 agent_protocol-0.2.2/agent_protocol/utils/compliance/main.py
--rw-r--r--   0        0        0      804 2023-08-08 08:46:00.630377 agent_protocol-0.2.2/pyproject.toml
--rw-r--r--   0        0        0     4015 1970-01-01 00:00:00.000000 agent_protocol-0.2.2/PKG-INFO
+-rw-r--r--   0        0        0     3009 2023-08-08 13:06:54.467973 agent_protocol-0.2.3/README.md
+-rw-r--r--   0        0        0      353 2023-08-08 13:06:54.467973 agent_protocol-0.2.3/agent_protocol/__init__.py
+-rw-r--r--   0        0        0     6021 2023-08-08 13:06:54.467973 agent_protocol-0.2.3/agent_protocol/agent.py
+-rw-r--r--   0        0        0      600 2023-08-08 13:06:54.467973 agent_protocol-0.2.3/agent_protocol/cli.py
+-rw-r--r--   0        0        0     4412 2023-08-08 13:06:54.467973 agent_protocol-0.2.3/agent_protocol/db.py
+-rw-r--r--   0        0        0     2546 2023-08-08 13:06:54.467973 agent_protocol-0.2.3/agent_protocol/models.py
+-rw-r--r--   0        0        0      331 2023-08-08 13:06:54.467973 agent_protocol-0.2.3/agent_protocol/server.py
+-rw-r--r--   0        0        0        0 2023-08-08 13:06:54.467973 agent_protocol-0.2.3/agent_protocol/utils/__init__.py
+-rw-r--r--   0        0        0       35 2023-08-08 13:06:54.467973 agent_protocol-0.2.3/agent_protocol/utils/compliance/__init__.py
+-rw-r--r--   0        0        0      449 2023-08-08 13:06:54.467973 agent_protocol-0.2.3/agent_protocol/utils/compliance/conftest.py
+-rw-r--r--   0        0        0     3748 2023-08-08 13:06:54.467973 agent_protocol-0.2.3/agent_protocol/utils/compliance/main.py
+-rw-r--r--   0        0        0      853 2023-08-08 13:06:54.467973 agent_protocol-0.2.3/pyproject.toml
+-rw-r--r--   0        0        0     4107 1970-01-01 00:00:00.000000 agent_protocol-0.2.3/PKG-INFO
```

### Comparing `agent_protocol-0.2.2/README.md` & `agent_protocol-0.2.3/README.md`

 * *Files identical despite different names*

### Comparing `agent_protocol-0.2.2/agent_protocol/agent.py` & `agent_protocol-0.2.3/agent_protocol/agent.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import asyncio
 import os
 
-from fastapi import APIRouter
+import aiofiles
+from fastapi import APIRouter, UploadFile
 from fastapi.responses import FileResponse
 from hypercorn.asyncio import serve
 from hypercorn.config import Config
 from typing import Awaitable, Callable, List, Optional
 
 from .db import InMemoryTaskDB, TaskDB
 from .server import app
@@ -96,18 +97,14 @@
 
     step.input = body.input if body else None
     step.additional_input = body.additional_input if body else None
 
     step = await _step_handler(step)
 
     step.status = Status.completed
-
-    if step.artifacts:
-        task.artifacts.extend(step.artifacts)
-
     return step
 
 
 @base_router.get(
     "/agent/tasks/{task_id}/steps/{step_id}",
     response_model=Step,
     tags=["agent"],
@@ -128,14 +125,39 @@
     """
     List all artifacts for the specified task.
     """
     task = await Agent.db.get_task(task_id)
     return task.artifacts
 
 
+@base_router.post(
+    "/agent/tasks/{task_id}/artifacts",
+    response_model=Artifact,
+    tags=["agent"],
+)
+async def upload_agent_task_artifacts(
+    task_id: str, file: UploadFile, relative_path: Optional[str] = None
+) -> Artifact:
+    """
+    Upload an artifact for the specified task.
+    """
+    await Agent.db.get_task(task_id)
+    artifact = await Agent.db.create_artifact(task_id, file.filename, relative_path)
+
+    path = Agent.get_artifact_folder(task_id, artifact)
+    if not os.path.exists(path):
+        os.makedirs(path)
+
+    async with aiofiles.open(os.path.join(path, file.filename), "wb") as f:
+        while content := await file.read(1024 * 1024):  # async read chunk ~1MiB
+            await f.write(content)
+
+    return artifact
+
+
 @base_router.get(
     "/agent/tasks/{task_id}/artifacts/{artifact_id}",
     tags=["agent"],
 )
 async def download_agent_task_artifacts(task_id: str, artifact_id: str) -> FileResponse:
     """
     Download the specified artifact.
@@ -168,21 +190,28 @@
     def get_workspace(task_id: str) -> str:
         """
         Get the workspace path for the specified task.
         """
         return os.path.join(os.getcwd(), Agent.workspace, task_id)
 
     @staticmethod
-    def get_artifact_path(task_id: str, artifact: Artifact) -> str:
+    def get_artifact_folder(task_id: str, artifact: Artifact) -> str:
         """
         Get the artifact path for the specified task and artifact.
         """
         workspace_path = Agent.get_workspace(task_id)
         relative_path = artifact.relative_path or ""
-        return os.path.join(workspace_path, relative_path, artifact.file_name)
+        return os.path.join(workspace_path, relative_path)
+
+    @staticmethod
+    def get_artifact_path(task_id: str, artifact: Artifact) -> str:
+        """
+        Get the artifact path for the specified task and artifact.
+        """
+        return os.path.join(Agent.get_artifact_folder(task_id, artifact), artifact.file_name)
 
     @staticmethod
     def start(port: int = 8000, router: APIRouter = base_router):
         """
         Start the agent server.
         """
         config = Config()
```

### Comparing `agent_protocol-0.2.2/agent_protocol/cli.py` & `agent_protocol-0.2.3/agent_protocol/cli.py`

 * *Files identical despite different names*

### Comparing `agent_protocol-0.2.2/agent_protocol/db.py` & `agent_protocol-0.2.3/agent_protocol/db.py`

 * *Files 12% similar despite different names*

```diff
@@ -27,14 +27,23 @@
         task_id: str,
         name: Optional[str] = None,
         is_last: bool = False,
         additional_properties: Optional[Dict[str, str]] = None,
     ) -> Step:
         raise NotImplementedError
 
+    async def create_artifact(
+        self,
+        task_id: str,
+        file_name: str,
+        relative_path: Optional[str] = None,
+        step_id: Optional[str] = None,
+    ) -> Artifact:
+        raise NotImplementedError
+
     async def get_task(self, task_id: str) -> Task:
         raise NotImplementedError
 
     async def get_step(self, task_id: str, step_id: str) -> Step:
         raise NotImplementedError
 
     async def get_artifact(self, task_id: str, artifact_id: str) -> Artifact:
@@ -110,13 +119,33 @@
         artifact = next(
             filter(lambda a: a.artifact_id == artifact_id, task.artifacts), None
         )
         if not artifact:
             raise Exception(f"Artifact with id {artifact_id} not found")
         return artifact
 
+    async def create_artifact(
+        self,
+        task_id: str,
+        file_name: str,
+        relative_path: Optional[str] = None,
+        step_id: Optional[str] = None,
+    ) -> Artifact:
+        artifact_id = str(uuid.uuid4())
+        artifact = Artifact(
+            artifact_id=artifact_id, file_name=file_name, relative_path=relative_path
+        )
+        task = await self.get_task(task_id)
+        task.artifacts.append(artifact)
+
+        if step_id:
+            step = await self.get_step(task_id, step_id)
+            step.artifacts.append(artifact)
+
+        return artifact
+
     async def list_tasks(self) -> List[Task]:
         return [task for task in self._tasks.values()]
 
     async def list_steps(self, task_id: str) -> List[Step]:
         task = await self.get_task(task_id)
         return [step for step in task.steps]
```

### Comparing `agent_protocol-0.2.2/agent_protocol/models.py` & `agent_protocol-0.2.3/agent_protocol/models.py`

 * *Files 3% similar despite different names*

```diff
@@ -20,14 +20,21 @@
     artifact_id: str = Field(..., description="ID of the artifact.")
     file_name: str = Field(..., description="Filename of the artifact.")
     relative_path: Optional[str] = Field(
         None, description="Relative path of the artifact in the agent's workspace."
     )
 
 
+class ArtifactUpload(BaseModel):
+    file: bytes = Field(..., description="File to upload.")
+    relative_path: Optional[str] = Field(
+        None, description="Relative path of the artifact in the agent's workspace."
+    )
+
+
 class StepInput(BaseModel):
     __root__: Any = Field(
         ..., description="Input parameters for the task step. Any value is allowed."
     )
 
 
 class StepOutput(BaseModel):
```

### Comparing `agent_protocol-0.2.2/agent_protocol/utils/compliance/main.py` & `agent_protocol-0.2.3/agent_protocol/utils/compliance/main.py`

 * *Files identical despite different names*

### Comparing `agent_protocol-0.2.2/pyproject.toml` & `agent_protocol-0.2.3/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "agent-protocol"
-version = "0.2.2"
+version = "0.2.3"
 description = "API for interacting with Agent"
 authors = ["e2b <hello@e2b.dev>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://e2b.dev/"
 repository = "https://github.com/e2b-dev/sdk/tree/main/agent/python/"
 packages = [{ include = "agent_protocol" }]
@@ -13,14 +13,16 @@
 python = ">=3.7, <4.0.0"
 fastapi = "^0.100.0"
 hypercorn = "^0.14.4"
 pytest = "^7.0.0"
 pydantic = "^1.10.5, <2"
 click = "^8.1.6"
 requests = "^2.31.0"
+python-multipart = "^0.0.6"
+aiofiles = "^23.1.0"
 
 [tool.poetry.group.dev.dependencies]
 fastapi-code-generator = "^0.4.2"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `agent_protocol-0.2.2/PKG-INFO` & `agent_protocol-0.2.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,30 @@
 Metadata-Version: 2.1
 Name: agent-protocol
-Version: 0.2.2
+Version: 0.2.3
 Summary: API for interacting with Agent
 Home-page: https://e2b.dev/
 License: MIT
 Author: e2b
 Author-email: hello@e2b.dev
 Requires-Python: >=3.7,<4.0.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: aiofiles (>=23.1.0,<24.0.0)
 Requires-Dist: click (>=8.1.6,<9.0.0)
 Requires-Dist: fastapi (>=0.100.0,<0.101.0)
 Requires-Dist: hypercorn (>=0.14.4,<0.15.0)
 Requires-Dist: pydantic (>=1.10.5,<2.0.0)
 Requires-Dist: pytest (>=7.0.0,<8.0.0)
+Requires-Dist: python-multipart (>=0.0.6,<0.0.7)
 Requires-Dist: requests (>=2.31.0,<3.0.0)
 Project-URL: Bug Tracker, https://github.com/e2b-dev/agent-protocol/issues
 Project-URL: Repository, https://github.com/e2b-dev/sdk/tree/main/agent/python/
 Description-Content-Type: text/markdown
 
 # Agent Communication Protocol - Python SDK
```


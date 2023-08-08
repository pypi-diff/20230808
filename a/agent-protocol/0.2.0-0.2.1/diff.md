# Comparing `tmp/agent_protocol-0.2.0.tar.gz` & `tmp/agent_protocol-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "agent_protocol-0.2.0.tar", max compression
+gzip compressed data, was "agent_protocol-0.2.1.tar", max compression
```

## Comparing `agent_protocol-0.2.0.tar` & `agent_protocol-0.2.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     3009 2023-08-07 15:23:03.772802 agent_protocol-0.2.0/README.md
--rw-r--r--   0        0        0      353 2023-08-07 15:23:03.772802 agent_protocol-0.2.0/agent_protocol/__init__.py
--rw-r--r--   0        0        0     5052 2023-08-07 15:23:03.772802 agent_protocol-0.2.0/agent_protocol/agent.py
--rw-r--r--   0        0        0      600 2023-08-07 15:23:03.772802 agent_protocol-0.2.0/agent_protocol/cli.py
--rw-r--r--   0        0        0     3592 2023-08-07 15:23:03.772802 agent_protocol-0.2.0/agent_protocol/db.py
--rw-r--r--   0        0        0     2319 2023-08-07 15:23:03.772802 agent_protocol-0.2.0/agent_protocol/models.py
--rw-r--r--   0        0        0        0 2023-08-07 15:23:03.772802 agent_protocol-0.2.0/agent_protocol/router.py
--rw-r--r--   0        0        0      331 2023-08-07 15:23:03.772802 agent_protocol-0.2.0/agent_protocol/server.py
--rw-r--r--   0        0        0        0 2023-08-07 15:23:03.772802 agent_protocol-0.2.0/agent_protocol/utils/__init__.py
--rw-r--r--   0        0        0       35 2023-08-07 15:23:03.772802 agent_protocol-0.2.0/agent_protocol/utils/compliance/__init__.py
--rw-r--r--   0        0        0      449 2023-08-07 15:23:03.772802 agent_protocol-0.2.0/agent_protocol/utils/compliance/conftest.py
--rw-r--r--   0        0        0     3754 2023-08-07 15:23:03.772802 agent_protocol-0.2.0/agent_protocol/utils/compliance/main.py
--rw-r--r--   0        0        0      804 2023-08-07 15:23:03.772802 agent_protocol-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     4015 1970-01-01 00:00:00.000000 agent_protocol-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     3009 2023-08-08 08:04:14.654728 agent_protocol-0.2.1/README.md
+-rw-r--r--   0        0        0      353 2023-08-08 08:04:14.654728 agent_protocol-0.2.1/agent_protocol/__init__.py
+-rw-r--r--   0        0        0     5052 2023-08-08 08:04:14.654728 agent_protocol-0.2.1/agent_protocol/agent.py
+-rw-r--r--   0        0        0      600 2023-08-08 08:04:14.654728 agent_protocol-0.2.1/agent_protocol/cli.py
+-rw-r--r--   0        0        0     3592 2023-08-08 08:04:14.654728 agent_protocol-0.2.1/agent_protocol/db.py
+-rw-r--r--   0        0        0     2319 2023-08-08 08:04:14.654728 agent_protocol-0.2.1/agent_protocol/models.py
+-rw-r--r--   0        0        0        0 2023-08-08 08:04:14.654728 agent_protocol-0.2.1/agent_protocol/router.py
+-rw-r--r--   0        0        0      331 2023-08-08 08:04:14.654728 agent_protocol-0.2.1/agent_protocol/server.py
+-rw-r--r--   0        0        0        0 2023-08-08 08:04:14.654728 agent_protocol-0.2.1/agent_protocol/utils/__init__.py
+-rw-r--r--   0        0        0       35 2023-08-08 08:04:14.654728 agent_protocol-0.2.1/agent_protocol/utils/compliance/__init__.py
+-rw-r--r--   0        0        0      449 2023-08-08 08:04:14.654728 agent_protocol-0.2.1/agent_protocol/utils/compliance/conftest.py
+-rw-r--r--   0        0        0     3748 2023-08-08 08:04:14.654728 agent_protocol-0.2.1/agent_protocol/utils/compliance/main.py
+-rw-r--r--   0        0        0      804 2023-08-08 08:04:14.654728 agent_protocol-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0     4015 1970-01-01 00:00:00.000000 agent_protocol-0.2.1/PKG-INFO
```

### Comparing `agent_protocol-0.2.0/README.md` & `agent_protocol-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `agent_protocol-0.2.0/agent_protocol/agent.py` & `agent_protocol-0.2.1/agent_protocol/agent.py`

 * *Files identical despite different names*

### Comparing `agent_protocol-0.2.0/agent_protocol/cli.py` & `agent_protocol-0.2.1/agent_protocol/cli.py`

 * *Files identical despite different names*

### Comparing `agent_protocol-0.2.0/agent_protocol/db.py` & `agent_protocol-0.2.1/agent_protocol/db.py`

 * *Files identical despite different names*

### Comparing `agent_protocol-0.2.0/agent_protocol/models.py` & `agent_protocol-0.2.1/agent_protocol/models.py`

 * *Files identical despite different names*

### Comparing `agent_protocol-0.2.0/agent_protocol/utils/compliance/main.py` & `agent_protocol-0.2.1/agent_protocol/utils/compliance/main.py`

 * *Files 3% similar despite different names*

```diff
@@ -48,26 +48,24 @@
     def test_list_artifacts(self, url):
         response = requests.post(f"{url}/agent/tasks", json=self.task_data)
         task_id = response.json()["task_id"]
         response = requests.get(f"{url}/agent/tasks/{task_id}/artifacts")
         assert response.status_code == 200
         assert isinstance(response.json(), list)
 
-    @pytest.mark.skip("There is no way to be sure any step exists")
     def test_get_agent_task_step(self, url):
         # Create task
-        response = requests.post(f"{url}agent/tasks", json=self.task_data)
+        response = requests.post(f"{url}/agent/tasks", json=self.task_data)
         task_id = response.json()["task_id"]
         # Get steps
         response = requests.get(f"{url}/agent/tasks/{task_id}/steps")
-        step_id = response.json()["step_id"]
+        step_id = response.json()[0]
         response = requests.get(f"{url}/agent/tasks/{task_id}/steps/{step_id}")
         assert response.status_code == 200
-        assert response.json()["step_id"] == step_id
-        Step(**response.json())
+        assert Step(**response.json()).step_id == step_id
 
 
 def provide_url_scheme(url: str, default_scheme: str = "https") -> str:
     """Make sure we have valid url scheme.
     Params:
         url : string : the URL
         default_scheme : string : default scheme to use, e.g. 'https'
@@ -88,18 +86,19 @@
     if is_universal_scheme:
         return default_scheme + ":" + url
     return default_scheme + "://" + url
 
 
 def check_compliance(url, additional_pytest_args):
     url = provide_url_scheme(url)
-    pytest.main(
+    exit_code = pytest.main(
         [
             "-v",
             __file__,
             "--url",
             url,
             "-W",
             "ignore:Module already imported:pytest.PytestWarning",
         ]
         + list(additional_pytest_args)
     )
+    assert exit_code == 0, "Your Agent API isn't compliant with the agent protocol"
```

### Comparing `agent_protocol-0.2.0/pyproject.toml` & `agent_protocol-0.2.1/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 [tool.poetry]
 name = "agent-protocol"
-version = "0.2.0"
+version = "0.2.1"
 description = "API for interacting with Agent"
 authors = ["e2b <hello@e2b.dev>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://e2b.dev/"
 repository = "https://github.com/e2b-dev/sdk/tree/main/agent/python/"
 packages = [{ include = "agent_protocol" }]
 
 [tool.poetry.dependencies]
 python = ">=3.7, <4.0.0"
 fastapi = "^0.100.0"
 hypercorn = "^0.14.4"
-pytest = "^7.4.0"
+pytest = "^7.0.0"
 pydantic = "^1.10.5, <2"
 click = "^8.1.6"
 requests = "^2.31.0"
 
 [tool.poetry.group.dev.dependencies]
 fastapi-code-generator = "^0.4.2"
```

### Comparing `agent_protocol-0.2.0/PKG-INFO` & `agent_protocol-0.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: agent-protocol
-Version: 0.2.0
+Version: 0.2.1
 Summary: API for interacting with Agent
 Home-page: https://e2b.dev/
 License: MIT
 Author: e2b
 Author-email: hello@e2b.dev
 Requires-Python: >=3.7,<4.0.0
 Classifier: License :: OSI Approved :: MIT License
@@ -14,15 +14,15 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: click (>=8.1.6,<9.0.0)
 Requires-Dist: fastapi (>=0.100.0,<0.101.0)
 Requires-Dist: hypercorn (>=0.14.4,<0.15.0)
 Requires-Dist: pydantic (>=1.10.5,<2.0.0)
-Requires-Dist: pytest (>=7.4.0,<8.0.0)
+Requires-Dist: pytest (>=7.0.0,<8.0.0)
 Requires-Dist: requests (>=2.31.0,<3.0.0)
 Project-URL: Bug Tracker, https://github.com/e2b-dev/agent-protocol/issues
 Project-URL: Repository, https://github.com/e2b-dev/sdk/tree/main/agent/python/
 Description-Content-Type: text/markdown
 
 # Agent Communication Protocol - Python SDK
```


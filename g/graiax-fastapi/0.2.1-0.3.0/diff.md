# Comparing `tmp/graiax-fastapi-0.2.1.tar.gz` & `tmp/graiax_fastapi-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "graiax-fastapi-0.2.1.tar", last modified: Tue Nov 15 02:24:08 2022, max compression
+gzip compressed data, was "graiax_fastapi-0.3.0.tar", last modified: Tue Aug  8 11:11:16 2023, max compression
```

## Comparing `graiax-fastapi-0.2.1.tar` & `graiax_fastapi-0.3.0.tar`

### file list

```diff
@@ -1,13 +1,6 @@
--rw-r--r--   0 runner    (1001) docker     (121)     1071 2022-11-15 02:23:51.128137 graiax-fastapi-0.2.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     4526 2022-11-15 02:23:51.128137 graiax-fastapi-0.2.1/README.md
--rw-r--r--   0 runner    (1001) docker     (121)     1668 2022-11-15 02:23:51.128137 graiax-fastapi-0.2.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)      274 2022-11-15 02:23:51.128137 graiax-fastapi-0.2.1/src/graiax/fastapi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-15 02:23:51.128137 graiax-fastapi-0.2.1/src/graiax/fastapi/py.typed
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-15 02:23:51.128137 graiax-fastapi-0.2.1/src/graiax/fastapi/saya/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1582 2022-11-15 02:23:51.128137 graiax-fastapi-0.2.1/src/graiax/fastapi/saya/behaviour.py
--rw-r--r--   0 runner    (1001) docker     (121)     3520 2022-11-15 02:23:51.128137 graiax-fastapi-0.2.1/src/graiax/fastapi/saya/route.py
--rw-r--r--   0 runner    (1001) docker     (121)     1977 2022-11-15 02:23:51.128137 graiax-fastapi-0.2.1/src/graiax/fastapi/saya/schema.py
--rw-r--r--   0 runner    (1001) docker     (121)      311 2022-11-15 02:23:51.128137 graiax-fastapi-0.2.1/src/graiax/fastapi/service.py
--rw-r--r--   0 runner    (1001) docker     (121)     1360 2022-11-15 02:23:51.128137 graiax-fastapi-0.2.1/tests/schema.py
--rw-r--r--   0 runner    (1001) docker     (121)     2690 2022-11-15 02:23:51.128137 graiax-fastapi-0.2.1/tests/test.py
--rw-------   0 runner    (1001) docker     (121)     4862 2022-11-15 02:24:08.296898 graiax-fastapi-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-08-08 11:11:00.382456 graiax_fastapi-0.3.0/LICENSE
+-rw-r--r--   0        0        0     4498 2023-08-08 11:11:00.382456 graiax_fastapi-0.3.0/README.md
+-rw-r--r--   0        0        0     2067 2023-08-08 11:11:16.850573 graiax_fastapi-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     1131 2023-08-08 11:11:00.386456 graiax_fastapi-0.3.0/tests/schema.py
+-rw-r--r--   0        0        0     2867 2023-08-08 11:11:00.386456 graiax_fastapi-0.3.0/tests/test.py
+-rw-r--r--   0        0        0     4997 1970-01-01 00:00:00.000000 graiax_fastapi-0.3.0/PKG-INFO
```

### Comparing `graiax-fastapi-0.2.1/LICENSE` & `graiax_fastapi-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `graiax-fastapi-0.2.1/README.md` & `graiax_fastapi-0.3.0/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -117,14 +117,21 @@
 
 ##### 在机器人入口文件中直接添加
 
 ```python
 ...
 fastapi = FastAPI()
 
+fastapi.add_middleware(
+    CORSMiddleware,
+    allow_origins=["*"],
+    allow_credentials=True,
+    allow_methods=["*"],
+    allow_headers=["*"],
+)
 
 @fastapi.get("/main")
 async def main():
     return "main"
 
 
 app.launch_manager.add_service(FastAPIService(fastapi))
@@ -141,20 +148,13 @@
     ...
 
 
 @listen(ApplicationLaunched)
 async def function(app: Ariadne):
     mgr = app.launch_manager
     fastapi: FastAPI = mgr.get_interface(ASGIHandlerProvider).get_asgi_handler()  # type: ignore
-    fastapi.add_middleware(
-        CORSMiddleware,
-        allow_origins=['*'],
-        allow_credentials=True,
-        allow_methods=['*'],
-        allow_headers=['*'],
-    )
     fastapi.add_api_route('/', endpoint=root, methods=['GET'])
     fastapi.get('/main')(root)
     fastapi.add_api_websocket_route('/ws', endpoint=websocket)
 ```
 
 </details>
```

### Comparing `graiax-fastapi-0.2.1/pyproject.toml` & `graiax_fastapi-0.3.0/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,37 +1,35 @@
 [project]
 name = "graiax-fastapi"
-version = "0.2.1"
-description = "FastAPI for GraiaCommunity."
+version = "0.3.0"
+description = "FastAPI launcher for GraiaCommunity."
 authors = [
     { name = "BlueGlassBlock", email = "blueglassblock@outlook.com" },
     { name = "Red_lnn", email = "w731347477@gmail.com" },
 ]
 dependencies = [
-    "graia-amnesia>=0.6.0",
-    "fastapi>=0.87.0",
-    "graia-saya>=0.0.17",
-    "typing-extensions>=4.0.0",
+    "graia-amnesia>=0.7.1,<0.8.0",
+    "fastapi>=0.101.0",
+    "graia-saya>=0.0.18",
+    "typing-extensions>=4.7.1,<5.0",
 ]
 requires-python = ">=3.8"
 readme = "README.md"
 
 [project.license]
 text = "MIT"
 
 [project.urls]
 repository = "https://github.com/GraiaCommunity/graiax-fastapi"
 
-[project.optional-dependencies]
-
 [build-system]
 requires = [
-    "pdm-pep517>=1.0.0",
+    "pdm-backend",
 ]
-build-backend = "pdm.pep517.api"
+build-backend = "pdm.backend"
 
 [tool.pdm]
 includes = [
     "src/graiax",
 ]
 
 [tool.pdm.scripts.test]
@@ -39,24 +37,57 @@
     "coverage run -m pytest -vv",
     "coverage xml",
     "coverage report",
 ]
 
 [tool.pdm.dev-dependencies]
 dev = [
-    "black>=22.10.0",
-    "isort>=5.10.1",
-    "launart>=0.6.1",
-    "uvicorn[standard]>=0.19.0",
-    "coverage>=6.5.0",
-    "pytest>=7.2.0",
-    "pytest-asyncio>=0.20.2",
-    "httpx>=0.23.0",
+    "black>=23.7.0",
+    "isort>=5.12.0",
+    "launart>=0.6.4,<0.7.0",
+    "uvicorn[standard]>=0.23.2",
+    "coverage>=7.2.7",
+    "pytest>=7.4.0",
+    "pytest-asyncio>=0.21.1",
+    "httpx>=0.24.1",
+    "graia-broadcast>=0.23.1",
+]
+
+[tool.black]
+line-length = 120
+target-version = [
+    "py38",
+    "py39",
+    "py310",
+    "py311",
+]
+
+[tool.ruff]
+line-length = 120
+target-version = "py38"
+select = [
+    "E",
+    "F",
+    "UP",
+    "I",
+    "ASYNC",
+]
+exclude = [
+    ".git",
+    ".venv",
+    "__pypackages__",
+    "dist",
+]
+ignore = [
+    "F401",
 ]
 
+[tool.ruff.pydocstyle]
+convention = "google"
+
 [tool.isort]
 profile = "black"
 
 [tool.pytest.ini_options]
 asyncio_mode = "strict"
 testpaths = [
     "./tests",
@@ -88,7 +119,8 @@
     "def __repr__\\(self\\).+",
     "except ImportError:",
 ]
 partial_branches = [
     "pragma: worst case",
 ]
 precision = 2
+fail_under = 100
```

### Comparing `graiax-fastapi-0.2.1/tests/schema.py` & `graiax_fastapi-0.3.0/tests/schema.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,34 +1,28 @@
+from graia.broadcast.builtin.event import ExceptionThrown
 from graia.saya import Channel
+from graia.saya.builtins.broadcast import ListenerSchema
 from pydantic import BaseModel
 
 from graiax.fastapi import RouteSchema, route
 
 channel = Channel.current()
 
 
 class ResponseModel(BaseModel):
     code: int
     message: str
 
 
-# 如果有 graia.broadcast 可以捕获运行中出现的部分错误并对其进行处理
-
-# from graia.saya.builtins.broadcast import ListenerSchema  # noqa: E402
-# from graia.broadcast.builtin.event import ExceptionThrown  # noqa: E402
-
-# @channel.use(ListenerSchema([ExceptionThrown]))
-# async def handle_exc(exc: Exception):
-#     ...
+@channel.use(ListenerSchema([ExceptionThrown]))
+async def handle_exc(exc: Exception):
+    ...
 
 
 @route.get("/", response_model=ResponseModel)
-@route.get(
-    "/", response_model=ResponseModel
-)  # duplication will be automatically removed
 async def root():
     return {"code": 200, "message": "Hello World!"}
 
 
 @route.route(["GET"], "/xxxxx")
 async def xxxxx():
     return "xxxx"
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `graiax-fastapi-0.2.1/tests/test.py` & `graiax_fastapi-0.3.0/tests/test.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 from fastapi import FastAPI
 from fastapi.middleware.cors import CORSMiddleware
 from graia.amnesia.builtins.uvicorn import UvicornService
+from graia.broadcast import Broadcast
 from graia.saya import Saya
+from graia.saya.builtins.broadcast import BroadcastBehaviour
 from httpx import AsyncClient
 from launart import Launart, Launchable
 
 from graiax.fastapi import FastAPIBehaviour, FastAPIService
 from graiax.fastapi.saya.schema import RouteSchema
 
 fastapi = FastAPI()
@@ -70,13 +72,15 @@
                 async with AsyncClient() as client:
                     response = await client.get("http://127.0.0.1:8000/")
                     assert response.json() == {"code": 200, "message": "Hello World!"}
                     response = await client.get("http://127.0.0.1:8000/nothing")
                     assert response.status_code == 404
 
     launart = Launart()
-    saya = Saya()
+    bcc = Broadcast()
+    saya = Saya(bcc)
     saya.install_behaviours(FastAPIBehaviour(fastapi))
+    saya.install_behaviours(BroadcastBehaviour(bcc))
     launart.add_service(FastAPIService(fastapi))
     launart.add_service(UvicornService())
     launart.add_launchable(MainLaunchable())
     launart.launch_blocking()
```

### Comparing `graiax-fastapi-0.2.1/PKG-INFO` & `graiax_fastapi-0.3.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,19 @@
 Metadata-Version: 2.1
 Name: graiax-fastapi
-Version: 0.2.1
-Summary: FastAPI for GraiaCommunity.
+Version: 0.3.0
+Summary: FastAPI launcher for GraiaCommunity.
+Author-Email: BlueGlassBlock <blueglassblock@outlook.com>, Red_lnn <w731347477@gmail.com>
 License: MIT
-Author-email: BlueGlassBlock <blueglassblock@outlook.com>,Red_lnn <w731347477@gmail.com>
+Project-URL: Repository, https://github.com/GraiaCommunity/graiax-fastapi
 Requires-Python: >=3.8
-Project-URL: repository, https://github.com/GraiaCommunity/graiax-fastapi
+Requires-Dist: graia-amnesia<0.8.0,>=0.7.1
+Requires-Dist: fastapi>=0.101.0
+Requires-Dist: graia-saya>=0.0.18
+Requires-Dist: typing-extensions<5.0,>=4.7.1
 Description-Content-Type: text/markdown
 
 <div align="center">
 
 # GraiaX FastAPI
 
 > :sparkles: Easy FastAPI Access for GraiaCommunity :sparkles:
@@ -127,14 +131,21 @@
 
 ##### 在机器人入口文件中直接添加
 
 ```python
 ...
 fastapi = FastAPI()
 
+fastapi.add_middleware(
+    CORSMiddleware,
+    allow_origins=["*"],
+    allow_credentials=True,
+    allow_methods=["*"],
+    allow_headers=["*"],
+)
 
 @fastapi.get("/main")
 async def main():
     return "main"
 
 
 app.launch_manager.add_service(FastAPIService(fastapi))
@@ -151,21 +162,13 @@
     ...
 
 
 @listen(ApplicationLaunched)
 async def function(app: Ariadne):
     mgr = app.launch_manager
     fastapi: FastAPI = mgr.get_interface(ASGIHandlerProvider).get_asgi_handler()  # type: ignore
-    fastapi.add_middleware(
-        CORSMiddleware,
-        allow_origins=['*'],
-        allow_credentials=True,
-        allow_methods=['*'],
-        allow_headers=['*'],
-    )
     fastapi.add_api_route('/', endpoint=root, methods=['GET'])
     fastapi.get('/main')(root)
     fastapi.add_api_websocket_route('/ws', endpoint=websocket)
 ```
 
 </details>
-
```


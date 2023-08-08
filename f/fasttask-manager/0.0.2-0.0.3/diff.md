# Comparing `tmp/fasttask_manager-0.0.2.tar.gz` & `tmp/fasttask_manager-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fasttask_manager-0.0.2.tar", last modified: Mon Aug  7 13:18:40 2023, max compression
+gzip compressed data, was "fasttask_manager-0.0.3.tar", last modified: Tue Aug  8 18:26:21 2023, max compression
```

## Comparing `fasttask_manager-0.0.2.tar` & `fasttask_manager-0.0.3.tar`

### file list

```diff
@@ -1,15 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-08-07 13:18:40.208926 fasttask_manager-0.0.2/
--rw-rw-rw-   0        0        0     1088 2023-08-07 13:06:45.000000 fasttask_manager-0.0.2/LICENSE
--rw-rw-rw-   0        0        0      474 2023-08-07 13:18:40.205803 fasttask_manager-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0       62 2023-08-07 13:05:31.000000 fasttask_manager-0.0.2/README.md
-drwxrwxrwx   0        0        0        0 2023-08-07 13:18:40.186927 fasttask_manager-0.0.2/fasttask_manager/
--rw-rw-rw-   0        0        0       28 2023-08-07 13:17:37.000000 fasttask_manager-0.0.2/fasttask_manager/__init__.py
--rw-rw-rw-   0        0        0     2576 2023-08-07 13:13:47.000000 fasttask_manager-0.0.2/fasttask_manager/manager.py
-drwxrwxrwx   0        0        0        0 2023-08-07 13:18:40.201710 fasttask_manager-0.0.2/fasttask_manager.egg-info/
--rw-rw-rw-   0        0        0      474 2023-08-07 13:18:40.000000 fasttask_manager-0.0.2/fasttask_manager.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      282 2023-08-07 13:18:40.000000 fasttask_manager-0.0.2/fasttask_manager.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-07 13:18:40.000000 fasttask_manager-0.0.2/fasttask_manager.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2023-08-07 13:18:40.000000 fasttask_manager-0.0.2/fasttask_manager.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2023-08-07 13:18:40.000000 fasttask_manager-0.0.2/fasttask_manager.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-08-07 13:18:40.208926 fasttask_manager-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0      679 2023-08-07 13:18:25.000000 fasttask_manager-0.0.2/setup.py
+drwxr-xr-x   0 irid      (1000) irid      (1000)        0 2023-08-08 18:26:21.917756 fasttask_manager-0.0.3/
+-rw-r--r--   0 irid      (1000) irid      (1000)     1068 2023-08-08 15:54:51.000000 fasttask_manager-0.0.3/LICENSE
+-rw-r--r--   0 irid      (1000) irid      (1000)      966 2023-08-08 18:26:21.917756 fasttask_manager-0.0.3/PKG-INFO
+-rw-r--r--   0 irid      (1000) irid      (1000)      567 2023-08-08 18:25:25.000000 fasttask_manager-0.0.3/README.md
+drwxr-xr-x   0 irid      (1000) irid      (1000)        0 2023-08-08 18:26:21.917756 fasttask_manager-0.0.3/fasttask_manager/
+-rw-r--r--   0 irid      (1000) irid      (1000)       28 2023-08-08 15:54:51.000000 fasttask_manager-0.0.3/fasttask_manager/__init__.py
+-rw-r--r--   0 irid      (1000) irid      (1000)      977 2023-08-08 16:07:54.000000 fasttask_manager-0.0.3/fasttask_manager/create_project.py
+-rw-r--r--   0 irid      (1000) irid      (1000)     2506 2023-08-08 15:54:51.000000 fasttask_manager-0.0.3/fasttask_manager/manager.py
+drwxr-xr-x   0 irid      (1000) irid      (1000)        0 2023-08-08 18:26:21.917756 fasttask_manager-0.0.3/fasttask_manager.egg-info/
+-rw-r--r--   0 irid      (1000) irid      (1000)      966 2023-08-08 18:26:21.000000 fasttask_manager-0.0.3/fasttask_manager.egg-info/PKG-INFO
+-rw-r--r--   0 irid      (1000) irid      (1000)      317 2023-08-08 18:26:21.000000 fasttask_manager-0.0.3/fasttask_manager.egg-info/SOURCES.txt
+-rw-r--r--   0 irid      (1000) irid      (1000)        1 2023-08-08 18:26:21.000000 fasttask_manager-0.0.3/fasttask_manager.egg-info/dependency_links.txt
+-rw-r--r--   0 irid      (1000) irid      (1000)       15 2023-08-08 18:26:21.000000 fasttask_manager-0.0.3/fasttask_manager.egg-info/requires.txt
+-rw-r--r--   0 irid      (1000) irid      (1000)       17 2023-08-08 18:26:21.000000 fasttask_manager-0.0.3/fasttask_manager.egg-info/top_level.txt
+-rw-r--r--   0 irid      (1000) irid      (1000)       38 2023-08-08 18:26:21.917756 fasttask_manager-0.0.3/setup.cfg
+-rw-r--r--   0 irid      (1000) irid      (1000)      675 2023-08-08 18:13:40.000000 fasttask_manager-0.0.3/setup.py
```

### Comparing `fasttask_manager-0.0.2/LICENSE` & `fasttask_manager-0.0.3/LICENSE`

 * *Ordering differences only*

 * *Files 10% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-MIT License
-
-Copyright (c) [year] [fullname]
-
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+MIT License
+
+Copyright (c) [year] [fullname]
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 SOFTWARE.
```

### Comparing `fasttask_manager-0.0.2/fasttask_manager/manager.py` & `fasttask_manager-0.0.3/fasttask_manager/manager.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,70 +1,70 @@
-import time
-import requests
-from retry import retry
-from logging import Logger, StreamHandler
-
-
-class Manager:
-    def __init__(self, host: str, task_name: str, protocol: str = "http", port: int = 80, check_gap: int = 15,
-                 tries: int = 5, delay: int = 3, logger: Logger = None, log_prefix: str = "") -> None:
-
-        self.task_name = task_name
-        self.protocol = protocol
-        self.host = host
-        self.port = port
-        self.url = f"{self.protocol}://{self.host}:{self.port}"
-        self.tries = tries
-        self.delay = delay
-        self.check_gap = check_gap
-        self.logger = logger
-        self.log_prefix = f"{log_prefix}{self.task_name}:"
-        if self.logger:
-            return
-
-        self.logger = Logger(task_name)
-        self.logger.addHandler(StreamHandler())
-
-    def _req(self, path, data: dict, method="p"):
-        @retry(tries=self.tries, delay=self.delay)
-        def req():
-            if method == "p":
-                r = requests.post(f"{self.url}{path}", json=data)
-            elif method == "g":
-                r = requests.get(f"{self.url}{path}", params=data)
-
-            r.raise_for_status()
-            return r.json()
-        return req()
-
-    def run(self, params: dict) -> dict:
-        return self._req(path=f"/run/{self.task_name}/", data=params)
-
-    def create_task(self, params: dict) -> dict:
-        self.logger.info(f"{self.log_prefix}: task creating...")
-        return self._req(path=f"/create/{self.task_name}/", data=params)
-
-    def check(self, result_id: str) -> dict:
-        resp = self._req(path=f"/check/{self.task_name}/", data={"result_id": result_id}, method="g")
-        self.logger.info(f"{self.log_prefix}: check task: {resp['state']}")
-        return resp
-
-    def create_and_wait_result(self, params: dict) -> dict:
-        start = time.time()
-        resp = self.create_task(params)
-
-        if resp["state"] != "PENDING":
-            raise Exception(f"create task error: state unexpected: {resp['state']}")
-
-        result_id = resp["id"]
-
-        while True:
-            resp = self.check(result_id=result_id)
-            if resp["state"] == "FAILURE":
-                self.logger.info(f"{self.log_prefix} cost: {time.time()-start}")
-                raise Exception(f"task :{resp['result']}")
-
-            elif resp["state"] == "SUCCESS":
-                self.logger.info(f"{self.log_prefix} cost: {time.time()-start}")
-                return resp["result"]
-
-            time.sleep(self.check_gap)
+import time
+import requests
+from retry import retry
+from logging import Logger, StreamHandler
+
+
+class Manager:
+    def __init__(self, host: str, task_name: str, protocol: str = "http", port: int = 80, check_gap: int = 15,
+                 tries: int = 5, delay: int = 3, logger: Logger = None, log_prefix: str = "") -> None:
+
+        self.task_name = task_name
+        self.protocol = protocol
+        self.host = host
+        self.port = port
+        self.url = f"{self.protocol}://{self.host}:{self.port}"
+        self.tries = tries
+        self.delay = delay
+        self.check_gap = check_gap
+        self.logger = logger
+        self.log_prefix = f"{log_prefix}{self.task_name}:"
+        if self.logger:
+            return
+
+        self.logger = Logger(task_name)
+        self.logger.addHandler(StreamHandler())
+
+    def _req(self, path, data: dict, method="p"):
+        @retry(tries=self.tries, delay=self.delay)
+        def req():
+            if method == "p":
+                r = requests.post(f"{self.url}{path}", json=data)
+            elif method == "g":
+                r = requests.get(f"{self.url}{path}", params=data)
+
+            r.raise_for_status()
+            return r.json()
+        return req()
+
+    def run(self, params: dict) -> dict:
+        return self._req(path=f"/run/{self.task_name}/", data=params)
+
+    def create_task(self, params: dict) -> dict:
+        self.logger.info(f"{self.log_prefix}: task creating...")
+        return self._req(path=f"/create/{self.task_name}/", data=params)
+
+    def check(self, result_id: str) -> dict:
+        resp = self._req(path=f"/check/{self.task_name}/", data={"result_id": result_id}, method="g")
+        self.logger.info(f"{self.log_prefix}: check task: {resp['state']}")
+        return resp
+
+    def create_and_wait_result(self, params: dict) -> dict:
+        start = time.time()
+        resp = self.create_task(params)
+
+        if resp["state"] != "PENDING":
+            raise Exception(f"create task error: state unexpected: {resp['state']}")
+
+        result_id = resp["id"]
+
+        while True:
+            resp = self.check(result_id=result_id)
+            if resp["state"] == "FAILURE":
+                self.logger.info(f"{self.log_prefix} cost: {time.time()-start}")
+                raise Exception(f"task :{resp['result']}")
+
+            elif resp["state"] == "SUCCESS":
+                self.logger.info(f"{self.log_prefix} cost: {time.time()-start}")
+                return resp["result"]
+
+            time.sleep(self.check_gap)
```

### Comparing `fasttask_manager-0.0.2/setup.py` & `fasttask_manager-0.0.3/setup.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,24 +1,25 @@
-import setuptools
-
-with open("README.md", "r") as fh:
-    long_description = fh.read()
-
-setuptools.setup(
-    name="fasttask_manager",
-    version="0.0.2",
-    author="Irid",
-    author_email="irid.zzy@gmail.com",
-    description="fasttask's manager ",
-    long_description=long_description,
-    long_description_content_type="text/markdown",
-    url="https://github.com/iridesc/fasttask_manager",
-    packages=setuptools.find_packages(),
-    classifiers=[
-        "Programming Language :: Python :: 3",
-        "License :: OSI Approved :: MIT License",
-        "Operating System :: OS Independent",
-    ],
-    install_requires=[
-        "retry"
-    ],
-)
+import setuptools
+
+with open("README.md", "r") as fh:
+    long_description = fh.read()
+
+setuptools.setup(
+    name="fasttask_manager",
+    version="0.0.3",
+    author="Irid",
+    author_email="irid.zzy@gmail.com",
+    description="fasttask's manager ",
+    long_description=long_description,
+    long_description_content_type="text/markdown",
+    url="https://github.com/iridesc/fasttask_manager",
+    packages=setuptools.find_packages(),
+    classifiers=[
+        "Programming Language :: Python :: 3",
+        "License :: OSI Approved :: MIT License",
+        "Operating System :: OS Independent",
+    ],
+    install_requires=[
+        "retry",
+        "requests"
+    ],
+)
```


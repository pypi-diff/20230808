# Comparing `tmp/testflows.github.runners-1.5.230805.1023308.tar.gz` & `tmp/testflows.github.runners-1.5.230808.1180621.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "testflows.github.runners-1.5.230805.1023308.tar", last modified: Sat Aug  5 02:33:08 2023, max compression
+gzip compressed data, was "testflows.github.runners-1.5.230808.1180621.tar", last modified: Tue Aug  8 18:06:21 2023, max compression
```

## Comparing `testflows.github.runners-1.5.230805.1023308.tar` & `testflows.github.runners-1.5.230808.1180621.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-08-05 02:33:08.415555 testflows.github.runners-1.5.230805.1023308/
--rw-rw-r--   0 user      (1000) user      (1000)      630 2023-07-29 01:22:14.000000 testflows.github.runners-1.5.230805.1023308/LICENSE
--rw-rw-r--   0 user      (1000) user      (1000)    64563 2023-08-05 02:33:08.415555 testflows.github.runners-1.5.230805.1023308/PKG-INFO
--rw-rw-r--   0 user      (1000) user      (1000)    63971 2023-08-04 02:31:51.000000 testflows.github.runners-1.5.230805.1023308/README.rst
--rw-rw-r--   0 user      (1000) user      (1000)       38 2023-08-05 02:33:08.415555 testflows.github.runners-1.5.230805.1023308/setup.cfg
--rw-rw-r--   0 user      (1000) user      (1000)     2195 2023-08-05 02:33:08.000000 testflows.github.runners-1.5.230805.1023308/setup.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-08-05 02:33:08.411555 testflows.github.runners-1.5.230805.1023308/testflows/
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-08-05 02:33:08.411555 testflows.github.runners-1.5.230805.1023308/testflows/github/
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-08-05 02:33:08.415555 testflows.github.runners-1.5.230805.1023308/testflows/github/runners/
--rw-rw-r--   0 user      (1000) user      (1000)     1376 2023-08-05 02:33:08.000000 testflows.github.runners-1.5.230805.1023308/testflows/github/runners/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)     2836 2023-08-05 02:32:20.000000 testflows.github.runners-1.5.230805.1023308/testflows/github/runners/actions.py
--rw-rw-r--   0 user      (1000) user      (1000)     1995 2023-08-02 15:26:55.000000 testflows.github.runners-1.5.230805.1023308/testflows/github/runners/api_watch.py
--rw-rw-r--   0 user      (1000) user      (1000)     2933 2023-08-04 06:28:52.000000 testflows.github.runners-1.5.230805.1023308/testflows/github/runners/args.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-08-05 02:33:08.415555 testflows.github.runners-1.5.230805.1023308/testflows/github/runners/bin/
--rwxrwxr-x   0 user      (1000) user      (1000)    25874 2023-08-05 02:05:41.000000 testflows.github.runners-1.5.230805.1023308/testflows/github/runners/bin/github-runners
--rw-rw-r--   0 user      (1000) user      (1000)    14938 2023-08-05 02:06:57.000000 testflows.github.runners-1.5.230805.1023308/testflows/github/runners/cloud.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-08-05 02:33:08.415555 testflows.github.runners-1.5.230805.1023308/testflows/github/runners/config/
--rw-rw-r--   0 user      (1000) user      (1000)      903 2023-08-04 23:32:22.000000 testflows.github.runners-1.5.230805.1023308/testflows/github/runners/config/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)    16804 2023-08-05 02:11:04.000000 testflows.github.runners-1.5.230805.1023308/testflows/github/runners/config/config.py
--rw-rw-r--   0 user      (1000) user      (1000)    10337 2023-08-04 23:35:08.000000 testflows.github.runners-1.5.230805.1023308/testflows/github/runners/config/schema.json
--rw-rw-r--   0 user      (1000) user      (1000)     2473 2023-07-29 23:43:11.000000 testflows.github.runners-1.5.230805.1023308/testflows/github/runners/delete.py
--rw-rw-r--   0 user      (1000) user      (1000)     1953 2023-08-05 02:31:56.000000 testflows.github.runners-1.5.230805.1023308/testflows/github/runners/logger.py
--rw-rw-r--   0 user      (1000) user      (1000)     1926 2023-07-29 23:39:43.000000 testflows.github.runners-1.5.230805.1023308/testflows/github/runners/request.py
--rw-rw-r--   0 user      (1000) user      (1000)    18206 2023-08-04 07:57:47.000000 testflows.github.runners-1.5.230805.1023308/testflows/github/runners/scale_down.py
--rw-rw-r--   0 user      (1000) user      (1000)    30496 2023-08-04 14:49:19.000000 testflows.github.runners-1.5.230805.1023308/testflows/github/runners/scale_up.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-08-05 02:33:08.415555 testflows.github.runners-1.5.230805.1023308/testflows/github/runners/scripts/
--rw-rw-r--   0 user      (1000) user      (1000)      655 2023-08-04 04:50:46.000000 testflows.github.runners-1.5.230805.1023308/testflows/github/runners/scripts/__init__.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-08-05 02:33:08.415555 testflows.github.runners-1.5.230805.1023308/testflows/github/runners/scripts/deploy/
--rw-rw-r--   0 user      (1000) user      (1000)      655 2023-07-29 01:22:14.000000 testflows.github.runners-1.5.230805.1023308/testflows/github/runners/scripts/deploy/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)      519 2023-07-29 01:22:14.000000 testflows.github.runners-1.5.230805.1023308/testflows/github/runners/scripts/deploy/setup.sh
--rw-rw-r--   0 user      (1000) user      (1000)      260 2023-07-31 12:43:19.000000 testflows.github.runners-1.5.230805.1023308/testflows/github/runners/scripts/setup.sh
--rw-rw-r--   0 user      (1000) user      (1000)     1148 2023-07-31 12:59:30.000000 testflows.github.runners-1.5.230805.1023308/testflows/github/runners/scripts/setup_docker.sh
--rw-rw-r--   0 user      (1000) user      (1000)      775 2023-07-29 01:22:14.000000 testflows.github.runners-1.5.230805.1023308/testflows/github/runners/scripts/startup_arm64.sh
--rw-rw-r--   0 user      (1000) user      (1000)      715 2023-07-29 01:22:14.000000 testflows.github.runners-1.5.230805.1023308/testflows/github/runners/scripts/startup_x64.sh
--rw-rw-r--   0 user      (1000) user      (1000)     3206 2023-08-05 02:14:33.000000 testflows.github.runners-1.5.230805.1023308/testflows/github/runners/server.py
--rw-rw-r--   0 user      (1000) user      (1000)     2714 2023-08-04 23:23:34.000000 testflows.github.runners-1.5.230805.1023308/testflows/github/runners/servers.py
--rw-rw-r--   0 user      (1000) user      (1000)     5692 2023-08-05 01:59:34.000000 testflows.github.runners-1.5.230805.1023308/testflows/github/runners/service.py
--rw-rw-r--   0 user      (1000) user      (1000)     1694 2023-08-05 02:23:54.000000 testflows.github.runners-1.5.230805.1023308/testflows/github/runners/shell.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-08-05 02:33:08.415555 testflows.github.runners-1.5.230805.1023308/testflows.github.runners.egg-info/
--rw-rw-r--   0 user      (1000) user      (1000)    64563 2023-08-05 02:33:08.000000 testflows.github.runners-1.5.230805.1023308/testflows.github.runners.egg-info/PKG-INFO
--rw-rw-r--   0 user      (1000) user      (1000)     1323 2023-08-05 02:33:08.000000 testflows.github.runners-1.5.230805.1023308/testflows.github.runners.egg-info/SOURCES.txt
--rw-rw-r--   0 user      (1000) user      (1000)        1 2023-08-05 02:33:08.000000 testflows.github.runners-1.5.230805.1023308/testflows.github.runners.egg-info/dependency_links.txt
--rw-rw-r--   0 user      (1000) user      (1000)        1 2023-07-29 01:22:42.000000 testflows.github.runners-1.5.230805.1023308/testflows.github.runners.egg-info/not-zip-safe
--rw-rw-r--   0 user      (1000) user      (1000)       73 2023-08-05 02:33:08.000000 testflows.github.runners-1.5.230805.1023308/testflows.github.runners.egg-info/requires.txt
--rw-rw-r--   0 user      (1000) user      (1000)       10 2023-08-05 02:33:08.000000 testflows.github.runners-1.5.230805.1023308/testflows.github.runners.egg-info/top_level.txt
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-08-08 18:06:21.643252 testflows.github.runners-1.5.230808.1180621/
+-rw-rw-r--   0 user      (1000) user      (1000)      630 2023-07-29 01:22:14.000000 testflows.github.runners-1.5.230808.1180621/LICENSE
+-rw-rw-r--   0 user      (1000) user      (1000)    64563 2023-08-08 18:06:21.643252 testflows.github.runners-1.5.230808.1180621/PKG-INFO
+-rw-rw-r--   0 user      (1000) user      (1000)    63971 2023-08-04 02:31:51.000000 testflows.github.runners-1.5.230808.1180621/README.rst
+-rw-rw-r--   0 user      (1000) user      (1000)       38 2023-08-08 18:06:21.643252 testflows.github.runners-1.5.230808.1180621/setup.cfg
+-rw-rw-r--   0 user      (1000) user      (1000)     2195 2023-08-08 18:06:21.000000 testflows.github.runners-1.5.230808.1180621/setup.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-08-08 18:06:21.639252 testflows.github.runners-1.5.230808.1180621/testflows/
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-08-08 18:06:21.639252 testflows.github.runners-1.5.230808.1180621/testflows/github/
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-08-08 18:06:21.639252 testflows.github.runners-1.5.230808.1180621/testflows/github/runners/
+-rw-rw-r--   0 user      (1000) user      (1000)     1376 2023-08-08 18:06:21.000000 testflows.github.runners-1.5.230808.1180621/testflows/github/runners/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)     2520 2023-08-07 20:42:43.000000 testflows.github.runners-1.5.230808.1180621/testflows/github/runners/actions.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1995 2023-08-02 15:26:55.000000 testflows.github.runners-1.5.230808.1180621/testflows/github/runners/api_watch.py
+-rw-rw-r--   0 user      (1000) user      (1000)     3602 2023-08-08 15:59:04.000000 testflows.github.runners-1.5.230808.1180621/testflows/github/runners/args.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-08-08 18:06:21.639252 testflows.github.runners-1.5.230808.1180621/testflows/github/runners/bin/
+-rwxrwxr-x   0 user      (1000) user      (1000)    28073 2023-08-08 16:04:23.000000 testflows.github.runners-1.5.230808.1180621/testflows/github/runners/bin/github-runners
+-rw-rw-r--   0 user      (1000) user      (1000)    15795 2023-08-08 16:04:03.000000 testflows.github.runners-1.5.230808.1180621/testflows/github/runners/cloud.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-08-08 18:06:21.639252 testflows.github.runners-1.5.230808.1180621/testflows/github/runners/config/
+-rw-rw-r--   0 user      (1000) user      (1000)      943 2023-08-08 15:54:34.000000 testflows.github.runners-1.5.230808.1180621/testflows/github/runners/config/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)    21613 2023-08-08 16:04:06.000000 testflows.github.runners-1.5.230808.1180621/testflows/github/runners/config/config.py
+-rw-rw-r--   0 user      (1000) user      (1000)    13497 2023-08-08 13:52:35.000000 testflows.github.runners-1.5.230808.1180621/testflows/github/runners/config/schema.json
+-rw-rw-r--   0 user      (1000) user      (1000)     2473 2023-07-29 23:43:11.000000 testflows.github.runners-1.5.230808.1180621/testflows/github/runners/delete.py
+-rw-rw-r--   0 user      (1000) user      (1000)     4809 2023-08-08 14:27:48.000000 testflows.github.runners-1.5.230808.1180621/testflows/github/runners/logger.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1926 2023-07-29 23:39:43.000000 testflows.github.runners-1.5.230808.1180621/testflows/github/runners/request.py
+-rw-rw-r--   0 user      (1000) user      (1000)    18279 2023-08-08 14:11:28.000000 testflows.github.runners-1.5.230808.1180621/testflows/github/runners/scale_down.py
+-rw-rw-r--   0 user      (1000) user      (1000)    31285 2023-08-08 14:08:10.000000 testflows.github.runners-1.5.230808.1180621/testflows/github/runners/scale_up.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-08-08 18:06:21.639252 testflows.github.runners-1.5.230808.1180621/testflows/github/runners/scripts/
+-rw-rw-r--   0 user      (1000) user      (1000)      655 2023-08-04 04:50:46.000000 testflows.github.runners-1.5.230808.1180621/testflows/github/runners/scripts/__init__.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-08-08 18:06:21.643252 testflows.github.runners-1.5.230808.1180621/testflows/github/runners/scripts/deploy/
+-rw-rw-r--   0 user      (1000) user      (1000)      655 2023-07-29 01:22:14.000000 testflows.github.runners-1.5.230808.1180621/testflows/github/runners/scripts/deploy/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)      519 2023-07-29 01:22:14.000000 testflows.github.runners-1.5.230808.1180621/testflows/github/runners/scripts/deploy/setup.sh
+-rw-rw-r--   0 user      (1000) user      (1000)      260 2023-07-31 12:43:19.000000 testflows.github.runners-1.5.230808.1180621/testflows/github/runners/scripts/setup.sh
+-rw-rw-r--   0 user      (1000) user      (1000)     1148 2023-07-31 12:59:30.000000 testflows.github.runners-1.5.230808.1180621/testflows/github/runners/scripts/setup_docker.sh
+-rw-rw-r--   0 user      (1000) user      (1000)      775 2023-07-29 01:22:14.000000 testflows.github.runners-1.5.230808.1180621/testflows/github/runners/scripts/startup_arm64.sh
+-rw-rw-r--   0 user      (1000) user      (1000)      715 2023-07-29 01:22:14.000000 testflows.github.runners-1.5.230808.1180621/testflows/github/runners/scripts/startup_x64.sh
+-rw-rw-r--   0 user      (1000) user      (1000)     3206 2023-08-05 02:14:33.000000 testflows.github.runners-1.5.230808.1180621/testflows/github/runners/server.py
+-rw-rw-r--   0 user      (1000) user      (1000)     2714 2023-08-04 23:23:34.000000 testflows.github.runners-1.5.230808.1180621/testflows/github/runners/servers.py
+-rw-rw-r--   0 user      (1000) user      (1000)     8456 2023-08-08 14:48:27.000000 testflows.github.runners-1.5.230808.1180621/testflows/github/runners/service.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1695 2023-08-07 20:28:47.000000 testflows.github.runners-1.5.230808.1180621/testflows/github/runners/shell.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-08-08 18:06:21.639252 testflows.github.runners-1.5.230808.1180621/testflows.github.runners.egg-info/
+-rw-rw-r--   0 user      (1000) user      (1000)    64563 2023-08-08 18:06:21.000000 testflows.github.runners-1.5.230808.1180621/testflows.github.runners.egg-info/PKG-INFO
+-rw-rw-r--   0 user      (1000) user      (1000)     1323 2023-08-08 18:06:21.000000 testflows.github.runners-1.5.230808.1180621/testflows.github.runners.egg-info/SOURCES.txt
+-rw-rw-r--   0 user      (1000) user      (1000)        1 2023-08-08 18:06:21.000000 testflows.github.runners-1.5.230808.1180621/testflows.github.runners.egg-info/dependency_links.txt
+-rw-rw-r--   0 user      (1000) user      (1000)        1 2023-07-29 01:22:42.000000 testflows.github.runners-1.5.230808.1180621/testflows.github.runners.egg-info/not-zip-safe
+-rw-rw-r--   0 user      (1000) user      (1000)       73 2023-08-08 18:06:21.000000 testflows.github.runners-1.5.230808.1180621/testflows.github.runners.egg-info/requires.txt
+-rw-rw-r--   0 user      (1000) user      (1000)       10 2023-08-08 18:06:21.000000 testflows.github.runners-1.5.230808.1180621/testflows.github.runners.egg-info/top_level.txt
```

### Comparing `testflows.github.runners-1.5.230805.1023308/LICENSE` & `testflows.github.runners-1.5.230808.1180621/LICENSE`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.5.230805.1023308/PKG-INFO` & `testflows.github.runners-1.5.230808.1180621/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: testflows.github.runners
-Version: 1.5.230805.1023308
+Version: 1.5.230808.1180621
 Summary: Autoscaling GitHub Actions Runners Using Hetzner Cloud 
 Home-page: https://github.com/testflows/github-runners
 Author: Vitaliy Zakaznikov
 Author-email: vzakaznikov@testflows.com
 License: Apache-2.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3
```

### Comparing `testflows.github.runners-1.5.230805.1023308/README.rst` & `testflows.github.runners-1.5.230808.1180621/README.rst`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.5.230805.1023308/setup.py` & `testflows.github.runners-1.5.230808.1180621/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 
 with open("README.rst", "r", encoding="utf-8") as fd:
     long_description = fd.read()
 
 
 setup(
     name="testflows.github.runners",
-    version="1.5.230805.1023308",
+    version="1.5.230808.1180621",
     description="Autoscaling GitHub Actions Runners Using Hetzner Cloud ",
     author="Vitaliy Zakaznikov",
     author_email="vzakaznikov@testflows.com",
     long_description=long_description,
     long_description_content_type="text/x-rst",
     url="https://github.com/testflows/github-runners",
     classifiers=[
```

### Comparing `testflows.github.runners-1.5.230805.1023308/testflows/github/runners/__init__.py` & `testflows.github.runners-1.5.230808.1180621/testflows/github/runners/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 __author__ = "Vitaliy Zakaznikov"
-__version__ = "1.5.230805.1023308"
+__version__ = "1.5.230808.1180621"
 __license__ = f"""
 Copyright 2023 Katteli Inc.
 TestFlows.com Open-Source Software Testing Framework (http://testflows.com)
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
```

### Comparing `testflows.github.runners-1.5.230805.1023308/testflows/github/runners/actions.py` & `testflows.github.runners-1.5.230808.1180621/testflows/github/runners/actions.py`

 * *Files 11% similar despite different names*

```diff
@@ -33,58 +33,49 @@
         server_name: str = "",
         interval: int = None,
     ):
         self.name = name
         self.ignore_fail = ignore_fail
         self.level = level
         self.stacklevel = stacklevel
-        # try to parse run_id and job_id from server name if not specified
-        try:
-            _run_id, _job_id = server_name.rsplit("-", 2)[-2:]
-            _run_id = int(_run_id)
-            _job_id = int(_job_id)
-            run_id = _run_id if run_id is None else run_id
-            job_id = _job_id if job_id is None else job_id
-        except Exception:
-            pass
-
         self.extra = {
-            "job_id": job_id,
-            "run_id": run_id,
-            "server_name": server_name,
+            "job_id": job_id or "-",
+            "run_id": run_id or "-",
+            "server_name": server_name or "-",
             "interval": str(interval) if interval is not None else "-",
         }
 
     def __enter__(self):
         logger.log(
-            msg=f"➤ {self.name}",
+            msg=f"🍀 {self.name}",
             stacklevel=self.stacklevel + 1,
             level=self.level,
             extra=self.extra,
         )
         return self
 
     def note(self, message, stacklevel=None):
         logger.log(
-            msg=f"  {message}",
+            msg=f"   {message}",
             stacklevel=(self.stacklevel + 1) if stacklevel is None else stacklevel,
             level=self.level,
             extra=self.extra,
         )
 
     def __exit__(self, exc_type, exc_value, exc_traceback):
         if exc_value is not None:
-            msg = f"❌ Error: {exc_type.__name__} {exc_value}"
+            msg = f"❌ {exc_type.__name__ or 'Error'}: {exc_value}"
             if not self.debug:
                 logger.log(
                     msg=msg,
                     stacklevel=self.stacklevel + 1,
                     level=logging.ERROR,
                     extra=self.extra,
                 )
             else:
                 logger.exception(
                     msg=msg, stacklevel=self.stacklevel + 1, extra=self.extra
                 )
+            exc_value.processed = True
             if self.ignore_fail:
                 return True
             raise
```

### Comparing `testflows.github.runners-1.5.230805.1023308/testflows/github/runners/api_watch.py` & `testflows.github.runners-1.5.230808.1180621/testflows/github/runners/api_watch.py`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.5.230805.1023308/testflows/github/runners/args.py` & `testflows.github.runners-1.5.230808.1180621/testflows/github/runners/args.py`

 * *Files 19% similar despite different names*

```diff
@@ -9,25 +9,45 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 import os
-
-from importlib.machinery import SourceFileLoader
+import argparse
 
 from hcloud.images.domain import Image
 from hcloud.locations.domain import Location
 from hcloud.server_types.domain import ServerType
 
 from argparse import ArgumentTypeError
 
 from traceback import print_exception
 
+file_type = argparse.FileType
+
+
+def columns_type(v):
+    """Log columns type name:width,..."""
+    columns = []
+    columns.value = v
+    try:
+        for c in v.split(","):
+            d = {}
+            c = str(c).rsplit(":", 1)
+            d["column"] = c[0]
+            if len(c) > 1:
+                c[1] = int(c[1])
+                assert c[1] > 0
+                d["width"] = c[1]
+            columns.append(d)
+    except Exception as e:
+        raise ArgumentTypeError(f"invalid format {v}")
+    return columns
+
 
 def end_of_life_type(v):
     """Server end of life type."""
     try:
         v = int(v)
         assert v > 0 and v < 60, f"{v} must be > 0 and < 60"
     except AssertionError as e:
@@ -90,15 +110,21 @@
 def server_type(v):
     """Server type argument. Example: cx11"""
     return ServerType(name=v)
 
 
 def config_type(v):
     """Program configuration file type."""
-    from .config import parse_config
+    from .config import parse_config, default_user_config
+
+    if v == "__default_user_config__":
+        if os.path.exists(default_user_config):
+            v = default_user_config
+        else:
+            return None
 
     v = path_type(v)
     try:
         config = parse_config(v)
         config.config_file = v
     except Exception as e:
         # print_exception(e)
```

### Comparing `testflows.github.runners-1.5.230805.1023308/testflows/github/runners/bin/github-runners` & `testflows.github.runners-1.5.230808.1180621/testflows/github/runners/bin/github-runners`

 * *Files 3% similar despite different names*

```diff
@@ -33,18 +33,15 @@
 from argparse import ArgumentParser, RawTextHelpFormatter
 
 from testflows.github.runners import __version__, __license__
 from testflows.github.runners.actions import Action
 from testflows.github.runners.scale_up import scale_up
 from testflows.github.runners.scale_down import scale_down
 from testflows.github.runners.api_watch import api_watch
-from testflows.github.runners.logger import (
-    logger,
-    default_config as default_logger_config,
-)
+from testflows.github.runners.logger import logger, configure as configure_logger
 from testflows.github.runners.config import Config, check_image
 from testflows.github.runners.config import (
     check_ssh_key,
     check_location,
     check_server_type,
     check_prices,
 )
@@ -93,14 +90,15 @@
     parser.add_argument(
         "-c",
         "--config",
         metavar="yaml",
         dest="config_file",
         type=args.config_type,
         help="program yaml configuration file",
+        default="__default_user_config__",
     )
 
     parser.add_argument(
         "--github-token",
         metavar="token",
         type=str,
         help="GitHub token, default: $GITHUB_TOKEN environment variable",
@@ -150,14 +148,22 @@
         help=(
             "number of minutes in 1 hour (60 minutes) period after which a recyclable server\n"
             "is considered to have reached its end of life and thus is deleted, default: 50"
         ),
     )
 
     parser.add_argument(
+        "--delete-random",
+        action="store_true",
+        help=(
+            "delete random recyclable server when maximum number of servers is reached, by default uses server prices"
+        ),
+    )
+
+    parser.add_argument(
         "--max-runners-in-workflow-run",
         metavar="count",
         type=args.count_type,
         help="maximum number of runners allowed to be created for a single workflow run, default: not set",
     )
 
     parser.add_argument(
@@ -167,14 +173,21 @@
         help=(
             "only create runners for jobs that have the specified label,\n"
             "by default jobs are not filtered and runners will be created for any queued job"
         ),
     )
 
     parser.add_argument(
+        "--label-prefix",
+        metavar="prefix",
+        type=str,
+        help="support type, image, and location job labels with the specified prefix",
+    )
+
+    parser.add_argument(
         "--default-image",
         metavar="architecture:type:name_or_description",
         type=args.image_type,
         help=(
             "default runner server image type and name or description,\n"
             "where the architecture is either: 'x86' or 'arm' and\n"
             "the type is either: 'system','snapshot','backup','app',\n"
@@ -437,29 +450,43 @@
             f"service package version to deploy, either version number or 'latest',\n"
             f"default: this version {__version__}"
         ),
     )
 
     redeploy_cloud_parser.set_defaults(func=cloud.redeploy)
 
-    logs_cloud_parser = cloud_commands.add_parser(
-        "logs",
-        help="get cloud service logs",
-        description="Get cloud service logs.",
+    log_cloud_parser = cloud_commands.add_parser(
+        "log",
+        help="get cloud service log",
+        description="Get cloud service log.",
         formatter_class=RawTextHelpFormatter,
     )
 
-    logs_cloud_parser.add_argument(
+    log_cloud_parser.add_argument(
         "-f",
         "--follow",
         action="store_true",
-        help="follow the logs journal",
+        help="follow the log journal",
     )
 
-    logs_cloud_parser.set_defaults(func=cloud.logs)
+    log_cloud_parser.add_argument(
+        "-c",
+        "--columns",
+        metavar="name[:width][,...]",
+        type=args.columns_type,
+        help="comma separated list of columns to include and their optional width",
+    )
+
+    log_cloud_parser.add_argument(
+        "--raw",
+        action="store_true",
+        help="output raw log",
+    )
+
+    log_cloud_parser.set_defaults(func=cloud.log)
 
     status_cloud_parser = cloud_commands.add_parser(
         "status",
         help="get cloud service status",
         description="Get cloud service status.",
         formatter_class=RawTextHelpFormatter,
     )
@@ -644,27 +671,71 @@
         "status",
         help="status",
         description="Get service status.",
         formatter_class=RawTextHelpFormatter,
     )
     status_service_parser.set_defaults(func=service.status)
 
-    logs_service_parser = service_commands.add_parser(
-        "logs",
-        help="logs",
-        description="Get service logs.",
+    log_service_parser = service_commands.add_parser(
+        "log",
+        help="log",
+        description="Get service log.",
         formatter_class=RawTextHelpFormatter,
     )
-    logs_service_parser.add_argument(
+
+    log_service_parser.add_argument(
+        "-c",
+        "--columns",
+        metavar="name[:width][,...]",
+        type=args.columns_type,
+        help="comma separated list of columns to include and their optional width",
+    )
+
+    log_service_parser.add_argument(
         "-f",
         "--follow",
         action="store_true",
-        help="follow the logs journal",
+        help="follow the log",
     )
-    logs_service_parser.set_defaults(func=service.logs)
+
+    log_service_parser.add_argument(
+        "--raw",
+        action="store_true",
+        help="output raw log",
+    )
+
+    log_service_parser.set_defaults(func=service.log)
+
+    log_service_commands = log_service_parser.add_subparsers(
+        title="commands", metavar="command", description=None, help=None
+    )
+
+    format_log_service_parser = log_service_commands.add_parser(
+        "format",
+        help="format log",
+        description="Format raw service log.",
+        formatter_class=RawTextHelpFormatter,
+    )
+
+    format_log_service_parser.add_argument(
+        "input",
+        type=args.file_type(bufsize=1),
+        help="input log file, use '-' for stdout",
+    )
+
+    format_log_service_parser.set_defaults(func=service.format_log)
+
+    delete_log_service_parser = log_service_commands.add_parser(
+        "delete",
+        help="delete log",
+        description="Delete service log.",
+        formatter_class=RawTextHelpFormatter,
+    )
+
+    delete_log_service_parser.set_defaults(func=service.delete_log)
 
     return parser
 
 
 @contextmanager
 def http_cache():
     """Enable caching of HTTP requests to GitHub api."""
@@ -683,15 +754,15 @@
                 "*": DO_NOT_CACHE,
             },
         )
 
         yield
 
 
-def main(config, worker_pool: ThreadPoolExecutor, terminate_timeout=30):
+def main(config, worker_pool: ThreadPoolExecutor, terminate_timeout=60):
     """Auto-scale runners service."""
     ssh_keys: list[SSHKey] = []
     terminate = threading.Event()
 
     try:
         with Action("Logging in to Hetzner Cloud"):
             client = Client(token=config.hetzner_token)
@@ -709,16 +780,17 @@
             config.default_location = check_location(client, config.default_location)
 
         with Action("Checking if default server type exists"):
             config.default_server_type = check_server_type(
                 client, config.default_server_type
             )
 
-        with Action("Checking server prices"):
-            config.server_prices = check_prices(client)
+        if not config.delete_random:
+            with Action("Getting server prices"):
+                config.server_prices = check_prices(client)
 
         with Action(f"Checking if SSH key exists"):
             ssh_keys.append(check_ssh_key(client, config.ssh_key))
 
             if config.additional_ssh_keys:
                 for key in config.additional_ssh_keys:
                     ssh_keys.append(check_ssh_key(client, key, is_file=False))
@@ -803,33 +875,41 @@
     logging_level = logging.INFO
 
     if args.config_file:
         config = args.config_file
     else:
         config = Config()
 
-    config.update(args)
-
     if config.debug:
         Action.debug = True
         logging_level = logging.DEBUG
 
-    if not config.logger_config:
-        default_logger_config(level=logging_level, service_mode=config.service_mode)
+    config.update(args)
+
+    configure_logger(
+        config=config,
+        level=logging_level,
+        service_mode=config.service_mode,
+    )
+
+    if config.config_file is not None:
+        print(f"Using config file: {config.config_file}")
 
     if hasattr(args, "func"):
         try:
             args.func(args=args, config=config)
         except KeyboardInterrupt:
             if config.debug:
                 raise
         except BaseException as exc:
             if config.debug:
                 raise
-            logger.critical(f"❗ Error: {exc}")
+            if not hasattr(exc, "processed"):
+                logger.critical(f"❗ Error: {exc}")
+            sys.exit(1)
 
     else:
         config.check()
 
         with http_cache():
             with ThreadPoolExecutor(
                 max_workers=config.workers + 3, thread_name_prefix="worker"
```

### Comparing `testflows.github.runners-1.5.230805.1023308/testflows/github/runners/cloud.py` & `testflows.github.runners-1.5.230808.1180621/testflows/github/runners/cloud.py`

 * *Files 2% similar despite different names*

```diff
@@ -34,15 +34,15 @@
 from .server import wait_ready, wait_ssh, ssh, scp, ip_address, ssh_command
 from .servers import ssh_client as server_ssh_client
 from .servers import ssh_client_command as server_ssh_client_command
 from .service import command_options
 
 current_dir = os.path.dirname(__file__)
 deploy_scripts_folder = "/home/ubuntu/.github-runners/scripts/"
-deploy_configs_folder = "/home/ubuntu/.github-runners/configs/"
+deploy_configs_folder = "/home/ubuntu/.github-runners/"
 
 
 def deploy(args, config: Config, redeploy=False):
     """Deploy or redeploy github-runners as a service to a
     new Hetzner server instance."""
     config.check()
     version = args.version or __version__
@@ -51,14 +51,16 @@
 
     with Action("Logging in to Hetzner Cloud"):
         client = Client(token=config.hetzner_token)
 
     if redeploy:
         with Action(f"Getting server {server_name}"):
             server: BoundServer = client.servers.get_by_name(server_name)
+            if not server:
+                raise ValueError(f"server {server_name} not found")
 
         uninstall(args=args, config=config, server=server)
 
         with Action("Cleaning copied scripts"):
             ssh(server, f"rm -rf {deploy_scripts_folder}*", stacklevel=4)
 
         with Action("Cleaning copied configs"):
@@ -234,14 +236,16 @@
         server_name = config.cloud.server_name
 
         with Action("Logging in to Hetzner Cloud"):
             client = Client(token=config.hetzner_token)
 
         with Action(f"Getting server {server_name}"):
             server: BoundServer = client.servers.get_by_name(server_name)
+            if not server:
+                raise ValueError(f"server {server_name} not found")
 
     with Action("Installing service"):
         command = f"\"su - ubuntu -c '"
         command += "github-runners"
         command += command_options(
             config,
             github_token=config.github_token,
@@ -260,14 +264,16 @@
     upgrade_version = args.upgrade_version
 
     with Action("Logging in to Hetzner Cloud"):
         client = Client(token=config.hetzner_token)
 
     with Action(f"Getting server {server_name}"):
         server: BoundServer = client.servers.get_by_name(server_name)
+        if not server:
+            raise ValueError(f"server {server_name} not found")
 
     stop(args, config=config, server=server)
 
     if upgrade_version:
         with Action(f"Upgrading github-runners to version {upgrade_version}"):
             ssh(
                 server,
@@ -292,14 +298,16 @@
         server_name = config.cloud.server_name
 
         with Action("Logging in to Hetzner Cloud"):
             client = Client(token=config.hetzner_token)
 
         with Action(f"Getting server {server_name}"):
             server: BoundServer = client.servers.get_by_name(server_name)
+            if not server:
+                raise ValueError(f"server {server_name} not found")
 
     with Action("Uninstalling service"):
         command = f"\"su - ubuntu -c 'github-runners service uninstall'\""
         ssh(server, command, stacklevel=4)
 
 
 def delete(args, config: Config):
@@ -310,38 +318,42 @@
     server_name = config.cloud.server_name
 
     with Action("Logging in to Hetzner Cloud"):
         client = Client(token=config.hetzner_token)
 
     with Action(f"Getting server {server_name}"):
         server: BoundServer = client.servers.get_by_name(server_name)
+        if not server:
+            raise ValueError(f"server {server_name} not found")
 
     with Action("Uninstalling service"):
         command = f"\"su - ubuntu -c 'github-runners service uninstall'\""
         ssh(server, command, stacklevel=4)
 
     with Action(f"Deleting server {server_name}"):
         server.delete()
 
 
-def logs(args, config: Config, server: BoundServer = None):
-    """Get cloud server service logs."""
+def log(args, config: Config, server: BoundServer = None):
+    """Get cloud server service log."""
     if server is None:
         config.check("hetzner_token")
         server_name = config.cloud.server_name
 
         client = Client(token=config.hetzner_token)
         server: BoundServer = client.servers.get_by_name(server_name)
 
-    if server is None:
-        raise ValueError("server not found")
+        if not server:
+            raise ValueError(f"server {server_name} not found")
 
     command = (
-        f"\"su - ubuntu -c 'github-runners service logs"
+        f"\"su - ubuntu -c 'github-runners service log"
         + (" -f" if args.follow else "")
+        + (f" -c {args.columns.value}" if args.columns else "")
+        + (" --raw" if args.raw else "")
         + "'\""
     )
     ssh(server, command, use_logger=False, stacklevel=4)
 
 
 def status(args, config: Config, server: BoundServer = None):
     """Get cloud server service status."""
@@ -350,14 +362,16 @@
         server_name = config.cloud.server_name
 
         with Action("Logging in to Hetzner Cloud"):
             client = Client(token=config.hetzner_token)
 
         with Action(f"Getting server {server_name}"):
             server = client.servers.get_by_name(server_name)
+            if not server:
+                raise ValueError(f"server {server_name} not found")
 
     with Action("Getting status"):
         command = f"\"su - ubuntu -c 'github-runners service status'\""
         ssh(server, command, stacklevel=4)
 
 
 def start(args, config: Config, server: BoundServer = None):
@@ -367,14 +381,16 @@
         server_name = config.cloud.server_name
 
         with Action("Logging in to Hetzner Cloud"):
             client = Client(token=config.hetzner_token)
 
         with Action(f"Getting server {server_name}"):
             server = client.servers.get_by_name(server_name)
+            if not server:
+                raise ValueError(f"server {server_name} not found")
 
     with Action("Starting service"):
         command = f"\"su - ubuntu -c 'github-runners service start'\""
         ssh(server, command, stacklevel=4)
 
 
 def stop(args, config: Config, server: BoundServer = None):
@@ -384,14 +400,16 @@
         server_name = config.cloud.server_name
 
         with Action("Logging in to Hetzner Cloud"):
             client = Client(token=config.hetzner_token)
 
         with Action(f"Getting server {server_name}"):
             server = client.servers.get_by_name(server_name)
+            if not server:
+                raise ValueError(f"server {server_name} not found")
 
     with Action("Stopping service"):
         command = f"\"su - ubuntu -c 'github-runners service stop'\""
         ssh(server, command, stacklevel=4)
 
 
 def ssh_client(args, config: Config):
```

### Comparing `testflows.github.runners-1.5.230805.1023308/testflows/github/runners/config/__init__.py` & `testflows.github.runners-1.5.230808.1180621/testflows/github/runners/config/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -19,7 +19,8 @@
     check_prices,
     check_server_type,
     check_ssh_key,
 )
 from .config import standby_runner
 from .config import read, write
 from .config import parse_config
+from .config import default_user_config
```

### Comparing `testflows.github.runners-1.5.230805.1023308/testflows/github/runners/config/schema.json` & `testflows.github.runners-1.5.230808.1180621/testflows/github/runners/config/schema.json`

 * *Files 22% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9991435185185186%*

 * *Differences: {"'properties'": '{\'config\': {\'properties\': {\'recycle\': {\'description\': "Turn on recycling '*

 * *                 'of powered off servers, either \'true\' or \'false\', default: true."}, '*

 * *                 "'label_prefix': OrderedDict([('description', 'Support type, image, and location "*

 * *                 "job labels with the specified prefix.'), ('type', 'string')]), 'delete_random': "*

 * *                 "OrderedDict([('description', 'delete random recyclable server when maximum "*

 * *                 "number […]*

```diff
@@ -85,14 +85,22 @@
                 "default_server_type": {
                     "description": "The default runner server type name, default: cx11.",
                     "examples": [
                         "cx11"
                     ],
                     "type": "string"
                 },
+                "delete_random": {
+                    "description": "delete random recyclable server when maximum number of servers is reached, by default uses server prices.",
+                    "examples": [
+                        true,
+                        false
+                    ],
+                    "type": "boolean"
+                },
                 "end_of_life": {
                     "description": "Number of minutes in 1 hour (60 minutes) period after which a recyclable server is considered to have reached its end of life and thus is deleted, default: 50.",
                     "examples": [
                         50
                     ],
                     "type": "integer"
                 },
@@ -114,18 +122,87 @@
                 "hetzner_token": {
                     "description": "Hetzner project token",
                     "examples": [
                         "${HETZNER_TOKEN}"
                     ],
                     "type": "string"
                 },
+                "label_prefix": {
+                    "description": "Support type, image, and location job labels with the specified prefix.",
+                    "type": "string"
+                },
                 "logger_config": {
                     "description": "Python logging module config. See https://docs.python.org/3/library/logging.config.html#logging-config-dictschema for details.",
                     "type": "object"
                 },
+                "logger_format": {
+                    "description": "Logger format.",
+                    "properties": {
+                        "columns": {
+                            "description": "Columns definitions.",
+                            "items": {
+                                "description": "Column object.",
+                                "properties": {
+                                    "column": {
+                                        "description": "Name of the column in the log.",
+                                        "examples": [
+                                            "date",
+                                            "time",
+                                            "level",
+                                            "interval",
+                                            "run_id",
+                                            "job_id",
+                                            "server_name",
+                                            "funcName",
+                                            "threadName",
+                                            "message"
+                                        ],
+                                        "type": "string"
+                                    },
+                                    "index": {
+                                        "description": "Index of the column in the log line after splitting it by comma.",
+                                        "type": "integer"
+                                    },
+                                    "width": {
+                                        "description": "Allocated width of the column.",
+                                        "type": "integer"
+                                    }
+                                },
+                                "type": "object"
+                            },
+                            "type": "array"
+                        },
+                        "default": {
+                            "description": "Default format columns.",
+                            "items": {
+                                "description": "Default column name and width object.",
+                                "properties": {
+                                    "column": {
+                                        "description": "Column name.",
+                                        "type": "string"
+                                    },
+                                    "width": {
+                                        "description": "Column width.",
+                                        "type": "integer"
+                                    }
+                                },
+                                "type": "object"
+                            },
+                            "type": "array"
+                        },
+                        "delimiter": {
+                            "description": "Column delimiter in the log line.",
+                            "examples": [
+                                ","
+                            ],
+                            "type": "string"
+                        }
+                    },
+                    "type": "object"
+                },
                 "max_powered_off_time": {
                     "description": "The maximum time after which a powered off server is recycled or deleted, default: 60 sec.",
                     "examples": [
                         60
                     ],
                     "type": "integer"
                 },
@@ -161,15 +238,15 @@
                     "description": "The maximum time after which an unused runner is removed and its server deleted, default: 120 sec.",
                     "examples": [
                         120
                     ],
                     "type": "integer"
                 },
                 "recycle": {
-                    "description": "Turn on recycling of powered off servers, either 'true' or 'false', default: true",
+                    "description": "Turn on recycling of powered off servers, either 'true' or 'false', default: true.",
                     "examples": [
                         true,
                         false
                     ],
                     "type": "boolean"
                 },
                 "scale_down_interval": {
```

### Comparing `testflows.github.runners-1.5.230805.1023308/testflows/github/runners/delete.py` & `testflows.github.runners-1.5.230808.1180621/testflows/github/runners/delete.py`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.5.230805.1023308/testflows/github/runners/request.py` & `testflows.github.runners-1.5.230808.1180621/testflows/github/runners/request.py`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.5.230805.1023308/testflows/github/runners/scale_down.py` & `testflows.github.runners-1.5.230808.1180621/testflows/github/runners/scale_down.py`

 * *Files 1% similar despite different names*

```diff
@@ -414,14 +414,16 @@
 
             with Action(
                 "Checking which recyclable servers need to be deleted",
                 level=logging.DEBUG,
                 interval=interval,
             ):
                 for server_name in list(recyclable_servers.keys()):
+                    if terminate.is_set():
+                        break
                     recyclable_server = recyclable_servers[server_name]
                     recycle_server(
                         reason="unused recyclable",
                         server=recyclable_server,
                         ssh_key=ssh_key,
                         end_of_life=end_of_life,
                     )
```

### Comparing `testflows.github.runners-1.5.230805.1023308/testflows/github/runners/scale_up.py` & `testflows.github.runners-1.5.230808.1180621/testflows/github/runners/scale_up.py`

 * *Files 7% similar despite different names*

```diff
@@ -113,56 +113,70 @@
             f"GITHUB_RUNNER_GROUP=Default "
             f'GITHUB_RUNNER_LABELS="{runner_labels}" '
             f"bash -s' < {startup_script}",
             stacklevel=5,
         )
 
 
-def get_server_type(labels: set[str], default: ServerType, label_prefix="type-"):
+def get_server_type(labels: set[str], default: ServerType, label_prefix: str = ""):
     """Get server type for the specified job."""
     server_type = None
 
+    if label_prefix and not label_prefix.endswith("-"):
+        label_prefix += "-"
+    label_prefix += "type-"
+
     if server_type is None:
         for label in labels:
             if label.startswith(label_prefix):
                 server_type_name = label.split(label_prefix, 1)[-1].lower()
                 server_type = ServerType(name=server_type_name)
 
     if server_type is None:
         server_type = default
 
     return server_type
 
 
-def get_server_location(labels: set[str], default: Location = None, label_prefix="in-"):
+def get_server_location(
+    labels: set[str], default: Location = None, label_prefix: str = ""
+):
     """Get preferred server location for the specified job.
 
     By default, location is set to `None` to avoid server type mismatching
     the location as some server types are not available at some locations.
     """
     server_location: Location = None
 
+    if label_prefix and not label_prefix.endswith("-"):
+        label_prefix += "-"
+    label_prefix += "in-"
+
     if server_location is None:
         for label in labels:
             if label.startswith(label_prefix):
                 server_location_name = label.split(label_prefix, 1)[-1].lower()
                 server_location = Location(name=server_location_name)
 
     if server_location is None and default:
         server_location = default
 
     return server_location
 
 
 def get_server_image(
-    client: Client, labels: set[str], default: Image, label_prefix="image-"
+    client: Client, labels: set[str], default: Image, label_prefix: str = ""
 ):
     """Get preferred server image for the specified job."""
     server_image: Image = None
 
+    if label_prefix and not label_prefix.endswith("-"):
+        label_prefix += "-"
+    label_prefix += "image-"
+
     if server_image is None:
         for label in labels:
             if label.startswith(label_prefix):
                 server_image = check_image(
                     client,
                     image_type(label.split(label_prefix, 1)[-1].lower(), separator="-"),
                 )
@@ -390,14 +404,15 @@
     max_servers_in_workflow_run: int = config.max_runners_in_workflow_run
     max_server_ready_time: int = config.max_server_ready_time
     debug: bool = config.debug
     standby_runners: list[StandbyRunner] = config.standby_runners
     recycle: bool = config.recycle
     server_prices: dict[str, float] = config.server_prices
     with_label: str = config.with_label
+    label_prefix: str = config.label_prefix
     interval: int = -1
 
     with Action("Logging in to Hetzner Cloud"):
         client = Client(token=hetzner_token)
 
     def create_runner_server(
         name: str,
@@ -405,18 +420,25 @@
         setup_worker_pool: ThreadPoolExecutor,
         futures: list[Future],
         servers: list[RunnerServer],
     ):
         """Create new server that would provide a runner with given labels."""
         recyclable_servers: list[BoundServer] = []
 
-        server_type = get_server_type(labels=labels, default=default_server_type)
-        server_location = get_server_location(labels=labels, default=default_location)
+        server_type = get_server_type(
+            labels=labels, default=default_server_type, label_prefix=label_prefix
+        )
+        server_location = get_server_location(
+            labels=labels, default=default_location, label_prefix=label_prefix
+        )
         server_image = get_server_image(
-            client=client, labels=labels, default=default_image
+            client=client,
+            labels=labels,
+            default=default_image,
+            label_prefix=label_prefix,
         )
         setup_script = config.setup_script
         startup_script = get_startup_script(
             server_type=server_type,
             x64=config.startup_x64_script,
             arm64=config.startup_arm64_script,
         )
@@ -644,14 +666,17 @@
                                     run_id=run.id,
                                     servers=servers,
                                     max_servers_in_workflow_run=max_servers_in_workflow_run,
                                 ):
                                     continue
 
                             for job in run.jobs():
+                                if terminate.is_set():
+                                    raise StopIteration("terminating")
+
                                 with Action(
                                     f"Checking job {job} {job.status}",
                                     level=logging.DEBUG,
                                     run_id=run.id,
                                     job_id=job.id,
                                     interval=interval,
                                 ):
@@ -738,14 +763,16 @@
                                     servers=servers, labels=labels
                                 )
                             else:
                                 available = count_present(server=servers, labels=labels)
 
                             if available < standby_runner.count:
                                 for _ in range(standby_runner.count - available):
+                                    if terminate.is_set():
+                                        break
                                     try:
                                         with Action(
                                             f"Replenishing{' immediately' if replenish_immediately else ''} standby server with {labels}",
                                             interval=interval,
                                         ):
                                             create_runner_server(
                                                 name=f"{standby_server_name_prefix}{uid()}",
```

### Comparing `testflows.github.runners-1.5.230805.1023308/testflows/github/runners/scripts/__init__.py` & `testflows.github.runners-1.5.230808.1180621/testflows/github/runners/scripts/__init__.py`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.5.230805.1023308/testflows/github/runners/scripts/deploy/__init__.py` & `testflows.github.runners-1.5.230808.1180621/testflows/github/runners/scripts/deploy/__init__.py`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.5.230805.1023308/testflows/github/runners/scripts/deploy/setup.sh` & `testflows.github.runners-1.5.230808.1180621/testflows/github/runners/scripts/deploy/setup.sh`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.5.230805.1023308/testflows/github/runners/scripts/setup_docker.sh` & `testflows.github.runners-1.5.230808.1180621/testflows/github/runners/scripts/setup_docker.sh`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.5.230805.1023308/testflows/github/runners/scripts/startup_arm64.sh` & `testflows.github.runners-1.5.230808.1180621/testflows/github/runners/scripts/startup_arm64.sh`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.5.230805.1023308/testflows/github/runners/scripts/startup_x64.sh` & `testflows.github.runners-1.5.230808.1180621/testflows/github/runners/scripts/startup_x64.sh`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.5.230805.1023308/testflows/github/runners/server.py` & `testflows.github.runners-1.5.230808.1180621/testflows/github/runners/server.py`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.5.230805.1023308/testflows/github/runners/servers.py` & `testflows.github.runners-1.5.230808.1180621/testflows/github/runners/servers.py`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.5.230805.1023308/testflows/github/runners/shell.py` & `testflows.github.runners-1.5.230808.1180621/testflows/github/runners/shell.py`

 * *Files 0% similar despite different names*

```diff
@@ -41,15 +41,15 @@
 
     for line in iter(p.stdout.readline, ""):
         if line == "":
             time.sleep(0.1)
             continue
         if use_logger:
             logger.info(
-                f"  > {line.rstrip()}",
+                f"   > {line.rstrip()}",
                 stacklevel=stacklevel,
                 extra={"server_name": server_name},
             )
         else:
             sys.stdout.write(line.rstrip())
             sys.stdout.write("\n")
             sys.stdout.flush()
```

### Comparing `testflows.github.runners-1.5.230805.1023308/testflows.github.runners.egg-info/PKG-INFO` & `testflows.github.runners-1.5.230808.1180621/testflows.github.runners.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: testflows.github.runners
-Version: 1.5.230805.1023308
+Version: 1.5.230808.1180621
 Summary: Autoscaling GitHub Actions Runners Using Hetzner Cloud 
 Home-page: https://github.com/testflows/github-runners
 Author: Vitaliy Zakaznikov
 Author-email: vzakaznikov@testflows.com
 License: Apache-2.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3
```

### Comparing `testflows.github.runners-1.5.230805.1023308/testflows.github.runners.egg-info/SOURCES.txt` & `testflows.github.runners-1.5.230808.1180621/testflows.github.runners.egg-info/SOURCES.txt`

 * *Files identical despite different names*


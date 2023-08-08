# Comparing `tmp/suvvyapi-0.1a1.tar.gz` & `tmp/suvvyapi-0.1a2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "suvvyapi-0.1a1.tar", last modified: Sat Aug  5 20:55:48 2023, max compression
+gzip compressed data, was "suvvyapi-0.1a2.tar", last modified: Tue Aug  8 08:27:07 2023, max compression
```

## Comparing `suvvyapi-0.1a1.tar` & `suvvyapi-0.1a2.tar`

### file list

```diff
@@ -1,31 +1,30 @@
-drwxrwxrwx   0        0        0        0 2023-08-05 20:55:48.460790 suvvyapi-0.1a1/
--rw-rw-rw-   0        0        0     1096 2023-08-05 15:34:16.000000 suvvyapi-0.1a1/LICENSE
--rw-rw-rw-   0        0        0     2154 2023-08-05 20:55:48.460790 suvvyapi-0.1a1/PKG-INFO
--rw-rw-rw-   0        0        0     1275 2023-08-05 20:55:26.000000 suvvyapi-0.1a1/README.md
--rw-rw-rw-   0        0        0       23 2023-08-05 16:45:36.000000 suvvyapi-0.1a1/requirements.txt
--rw-rw-rw-   0        0        0      950 2023-08-05 20:55:48.465790 suvvyapi-0.1a1/setup.cfg
--rw-rw-rw-   0        0        0       71 2023-07-13 17:40:00.000000 suvvyapi-0.1a1/setup.py
-drwxrwxrwx   0        0        0        0 2023-08-05 20:55:48.439278 suvvyapi-0.1a1/suvvyapi/
--rw-rw-rw-   0        0        0      193 2023-08-05 20:53:40.000000 suvvyapi-0.1a1/suvvyapi/__init__.py
-drwxrwxrwx   0        0        0        0 2023-08-05 20:55:48.454790 suvvyapi-0.1a1/suvvyapi/_tools/
--rw-rw-rw-   0        0        0        0 2023-08-05 15:40:25.000000 suvvyapi-0.1a1/suvvyapi/_tools/__init__.py
--rw-rw-rw-   0        0        0        0 2023-08-05 15:40:43.000000 suvvyapi-0.1a1/suvvyapi/_tools/request.py
-drwxrwxrwx   0        0        0        0 2023-08-05 20:55:48.455791 suvvyapi-0.1a1/suvvyapi/asynchronous/
--rw-rw-rw-   0        0        0        0 2023-08-05 20:51:02.000000 suvvyapi-0.1a1/suvvyapi/asynchronous/__init__.py
--rw-rw-rw-   0        0        0     4634 2023-08-05 20:53:40.000000 suvvyapi-0.1a1/suvvyapi/asynchronous/wrapper.py
-drwxrwxrwx   0        0        0        0 2023-08-05 20:55:48.456791 suvvyapi-0.1a1/suvvyapi/exceptions/
--rw-rw-rw-   0        0        0        0 2023-08-05 15:57:07.000000 suvvyapi-0.1a1/suvvyapi/exceptions/__init__.py
--rw-rw-rw-   0        0        0     1154 2023-08-05 18:14:35.000000 suvvyapi-0.1a1/suvvyapi/exceptions/api.py
-drwxrwxrwx   0        0        0        0 2023-08-05 20:55:48.458790 suvvyapi-0.1a1/suvvyapi/models/
--rw-rw-rw-   0        0        0        0 2023-08-05 16:06:39.000000 suvvyapi-0.1a1/suvvyapi/models/__init__.py
--rw-rw-rw-   0        0        0      837 2023-08-05 18:24:09.000000 suvvyapi-0.1a1/suvvyapi/models/history.py
--rw-rw-rw-   0        0        0      896 2023-08-05 17:57:12.000000 suvvyapi-0.1a1/suvvyapi/models/responses.py
-drwxrwxrwx   0        0        0        0 2023-08-05 20:55:48.459790 suvvyapi-0.1a1/suvvyapi/sync/
--rw-rw-rw-   0        0        0        0 2023-08-05 15:43:09.000000 suvvyapi-0.1a1/suvvyapi/sync/__init__.py
--rw-rw-rw-   0        0        0     4540 2023-08-05 18:22:53.000000 suvvyapi-0.1a1/suvvyapi/sync/wrapper.py
-drwxrwxrwx   0        0        0        0 2023-08-05 20:55:48.453790 suvvyapi-0.1a1/suvvyapi.egg-info/
--rw-rw-rw-   0        0        0     2154 2023-08-05 20:55:48.000000 suvvyapi-0.1a1/suvvyapi.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      549 2023-08-05 20:55:48.000000 suvvyapi-0.1a1/suvvyapi.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-05 20:55:48.000000 suvvyapi-0.1a1/suvvyapi.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       23 2023-08-05 20:55:48.000000 suvvyapi-0.1a1/suvvyapi.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-08-05 20:55:48.000000 suvvyapi-0.1a1/suvvyapi.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-08-08 08:27:07.044370 suvvyapi-0.1a2/
+-rw-rw-rw-   0        0        0     1096 2023-08-05 15:34:16.000000 suvvyapi-0.1a2/LICENSE
+-rw-rw-rw-   0        0        0     2185 2023-08-08 08:27:07.044370 suvvyapi-0.1a2/PKG-INFO
+-rw-rw-rw-   0        0        0     1306 2023-08-06 10:32:31.000000 suvvyapi-0.1a2/README.md
+-rw-rw-rw-   0        0        0       23 2023-08-05 16:45:36.000000 suvvyapi-0.1a2/requirements.txt
+-rw-rw-rw-   0        0        0      950 2023-08-08 08:27:07.045369 suvvyapi-0.1a2/setup.cfg
+-rw-rw-rw-   0        0        0       71 2023-07-13 17:40:00.000000 suvvyapi-0.1a2/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-08 08:27:06.999370 suvvyapi-0.1a2/suvvyapi/
+-rw-rw-rw-   0        0        0      193 2023-08-05 20:53:40.000000 suvvyapi-0.1a2/suvvyapi/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-08 08:27:07.025370 suvvyapi-0.1a2/suvvyapi/asynchronous/
+-rw-rw-rw-   0        0        0        0 2023-08-05 20:51:02.000000 suvvyapi-0.1a2/suvvyapi/asynchronous/__init__.py
+-rw-rw-rw-   0        0        0     4634 2023-08-05 20:53:40.000000 suvvyapi-0.1a2/suvvyapi/asynchronous/wrapper.py
+drwxrwxrwx   0        0        0        0 2023-08-08 08:27:07.026369 suvvyapi-0.1a2/suvvyapi/enums/
+-rw-rw-rw-   0        0        0      160 2023-08-06 10:49:26.000000 suvvyapi-0.1a2/suvvyapi/enums/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-08 08:27:07.033369 suvvyapi-0.1a2/suvvyapi/exceptions/
+-rw-rw-rw-   0        0        0        0 2023-08-05 15:57:07.000000 suvvyapi-0.1a2/suvvyapi/exceptions/__init__.py
+-rw-rw-rw-   0        0        0     1154 2023-08-05 18:14:35.000000 suvvyapi-0.1a2/suvvyapi/exceptions/api.py
+drwxrwxrwx   0        0        0        0 2023-08-08 08:27:07.035371 suvvyapi-0.1a2/suvvyapi/models/
+-rw-rw-rw-   0        0        0        0 2023-08-05 16:06:39.000000 suvvyapi-0.1a2/suvvyapi/models/__init__.py
+-rw-rw-rw-   0        0        0      821 2023-08-08 08:26:28.000000 suvvyapi-0.1a2/suvvyapi/models/history.py
+-rw-rw-rw-   0        0        0      896 2023-08-05 17:57:12.000000 suvvyapi-0.1a2/suvvyapi/models/responses.py
+drwxrwxrwx   0        0        0        0 2023-08-08 08:27:07.043369 suvvyapi-0.1a2/suvvyapi/sync/
+-rw-rw-rw-   0        0        0        0 2023-08-05 15:43:09.000000 suvvyapi-0.1a2/suvvyapi/sync/__init__.py
+-rw-rw-rw-   0        0        0     4540 2023-08-05 18:22:53.000000 suvvyapi-0.1a2/suvvyapi/sync/wrapper.py
+drwxrwxrwx   0        0        0        0 2023-08-08 08:27:07.018370 suvvyapi-0.1a2/suvvyapi.egg-info/
+-rw-rw-rw-   0        0        0     2185 2023-08-08 08:27:06.000000 suvvyapi-0.1a2/suvvyapi.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      521 2023-08-08 08:27:06.000000 suvvyapi-0.1a2/suvvyapi.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-08 08:27:06.000000 suvvyapi-0.1a2/suvvyapi.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       23 2023-08-08 08:27:06.000000 suvvyapi-0.1a2/suvvyapi.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-08-08 08:27:06.000000 suvvyapi-0.1a2/suvvyapi.egg-info/top_level.txt
```

### Comparing `suvvyapi-0.1a1/LICENSE` & `suvvyapi-0.1a2/LICENSE`

 * *Files identical despite different names*

### Comparing `suvvyapi-0.1a1/PKG-INFO` & `suvvyapi-0.1a2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: suvvyapi
-Version: 0.1a1
+Version: 0.1a2
 Summary: A Python API wrapper for Suvvy AI API
 Home-page: https://github.com/barabum0/suvvyapi
 Author: Roman Poltorabatko
 Author-email: barabum@duck.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/barabum0/suvvyapi/issues
 Keywords: python,api,wrapper,chatgpt,suvvy,ai,suvvyai
@@ -18,17 +18,17 @@
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # An async API wrapper for Suvvy AI
-
+#### built on top of httpx and pydantic :)
 [![Supported Python versions](https://img.shields.io/pypi/pyversions/suvvyapi.svg?style=flat-square&logo=python&logoColor=FFE873)](https://pypi.org/project/suvvyapi)
-[![PyPI version](https://img.shields.io/pypi/v/suvvyapi.svg?style=flat-square&logo=pypi&logoColor=FFE873)](https://pypi.org/project/aiogram-translation)
+[![PyPI version](https://img.shields.io/pypi/v/suvvyapi.svg?style=flat-square&logo=pypi&logoColor=FFE873)](https://pypi.org/project/suvvyapi)
 [![PyPI downloads](https://img.shields.io/pypi/dm/suvvyapi.svg?style=flat-square)](https://pypi.org/project/suvvyapi)
 
 [![suvvy.ai](https://img.shields.io/badge/suvvy.ai-best%20AI%20website-blue?style=flat-square)](https://suvvy.ai)
 
 ## Installation
 ```shell
 pip install -U suvvyapi
```

### Comparing `suvvyapi-0.1a1/README.md` & `suvvyapi-0.1a2/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # An async API wrapper for Suvvy AI
-
+#### built on top of httpx and pydantic :)
 [![Supported Python versions](https://img.shields.io/pypi/pyversions/suvvyapi.svg?style=flat-square&logo=python&logoColor=FFE873)](https://pypi.org/project/suvvyapi)
-[![PyPI version](https://img.shields.io/pypi/v/suvvyapi.svg?style=flat-square&logo=pypi&logoColor=FFE873)](https://pypi.org/project/aiogram-translation)
+[![PyPI version](https://img.shields.io/pypi/v/suvvyapi.svg?style=flat-square&logo=pypi&logoColor=FFE873)](https://pypi.org/project/suvvyapi)
 [![PyPI downloads](https://img.shields.io/pypi/dm/suvvyapi.svg?style=flat-square)](https://pypi.org/project/suvvyapi)
 
 [![suvvy.ai](https://img.shields.io/badge/suvvy.ai-best%20AI%20website-blue?style=flat-square)](https://suvvy.ai)
 
 ## Installation
 ```shell
 pip install -U suvvyapi
```

### Comparing `suvvyapi-0.1a1/setup.cfg` & `suvvyapi-0.1a2/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2073 7576 7679 6170 690d 0a76 6572   = suvvyapi..ver
-00000020: 7369 6f6e 203d 2030 2e31 6131 0d0a 6175  sion = 0.1a1..au
+00000020: 7369 6f6e 203d 2030 2e31 6132 0d0a 6175  sion = 0.1a2..au
 00000030: 7468 6f72 203d 2052 6f6d 616e 2050 6f6c  thor = Roman Pol
 00000040: 746f 7261 6261 746b 6f0d 0a61 7574 686f  torabatko..autho
 00000050: 725f 656d 6169 6c20 3d20 6261 7261 6275  r_email = barabu
 00000060: 6d40 6475 636b 2e63 6f6d 0d0a 7572 6c20  m@duck.com..url 
 00000070: 3d20 6874 7470 733a 2f2f 6769 7468 7562  = https://github
 00000080: 2e63 6f6d 2f62 6172 6162 756d 302f 7375  .com/barabum0/su
 00000090: 7676 7961 7069 0d0a 6465 7363 7269 7074  vvyapi..descript
```

### Comparing `suvvyapi-0.1a1/suvvyapi/asynchronous/wrapper.py` & `suvvyapi-0.1a2/suvvyapi/asynchronous/wrapper.py`

 * *Files identical despite different names*

### Comparing `suvvyapi-0.1a1/suvvyapi/exceptions/api.py` & `suvvyapi-0.1a2/suvvyapi/exceptions/api.py`

 * *Files identical despite different names*

### Comparing `suvvyapi-0.1a1/suvvyapi/models/history.py` & `suvvyapi-0.1a2/suvvyapi/models/history.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 from datetime import datetime
 from typing import Literal, Optional
 
 from pydantic import BaseModel, Field
 
+from suvvyapi.enums import Role
+
 
 class FunctionDetails(BaseModel):
     name: str
     args: Optional[dict] = None
 
 
 class Message(BaseModel):
     text: str = Field(default="", description="Message text, function result")
-    role: Literal["human", "ai", "function_result", "function_call"] = "human"
+    role: Role = Role.HUMAN
     function: Optional[FunctionDetails] = Field(default=None,
                                                 description="Needed for functions. Unused if role != \"function_*\".")
 
 
 class HistoryMessage(Message):
     tokens: int = 0
     time: datetime
```

### Comparing `suvvyapi-0.1a1/suvvyapi/models/responses.py` & `suvvyapi-0.1a2/suvvyapi/models/responses.py`

 * *Files identical despite different names*

### Comparing `suvvyapi-0.1a1/suvvyapi/sync/wrapper.py` & `suvvyapi-0.1a2/suvvyapi/sync/wrapper.py`

 * *Files identical despite different names*

### Comparing `suvvyapi-0.1a1/suvvyapi.egg-info/PKG-INFO` & `suvvyapi-0.1a2/suvvyapi.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: suvvyapi
-Version: 0.1a1
+Version: 0.1a2
 Summary: A Python API wrapper for Suvvy AI API
 Home-page: https://github.com/barabum0/suvvyapi
 Author: Roman Poltorabatko
 Author-email: barabum@duck.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/barabum0/suvvyapi/issues
 Keywords: python,api,wrapper,chatgpt,suvvy,ai,suvvyai
@@ -18,17 +18,17 @@
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # An async API wrapper for Suvvy AI
-
+#### built on top of httpx and pydantic :)
 [![Supported Python versions](https://img.shields.io/pypi/pyversions/suvvyapi.svg?style=flat-square&logo=python&logoColor=FFE873)](https://pypi.org/project/suvvyapi)
-[![PyPI version](https://img.shields.io/pypi/v/suvvyapi.svg?style=flat-square&logo=pypi&logoColor=FFE873)](https://pypi.org/project/aiogram-translation)
+[![PyPI version](https://img.shields.io/pypi/v/suvvyapi.svg?style=flat-square&logo=pypi&logoColor=FFE873)](https://pypi.org/project/suvvyapi)
 [![PyPI downloads](https://img.shields.io/pypi/dm/suvvyapi.svg?style=flat-square)](https://pypi.org/project/suvvyapi)
 
 [![suvvy.ai](https://img.shields.io/badge/suvvy.ai-best%20AI%20website-blue?style=flat-square)](https://suvvy.ai)
 
 ## Installation
 ```shell
 pip install -U suvvyapi
```

### Comparing `suvvyapi-0.1a1/suvvyapi.egg-info/SOURCES.txt` & `suvvyapi-0.1a2/suvvyapi.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -5,18 +5,17 @@
 setup.py
 suvvyapi/__init__.py
 suvvyapi.egg-info/PKG-INFO
 suvvyapi.egg-info/SOURCES.txt
 suvvyapi.egg-info/dependency_links.txt
 suvvyapi.egg-info/requires.txt
 suvvyapi.egg-info/top_level.txt
-suvvyapi/_tools/__init__.py
-suvvyapi/_tools/request.py
 suvvyapi/asynchronous/__init__.py
 suvvyapi/asynchronous/wrapper.py
+suvvyapi/enums/__init__.py
 suvvyapi/exceptions/__init__.py
 suvvyapi/exceptions/api.py
 suvvyapi/models/__init__.py
 suvvyapi/models/history.py
 suvvyapi/models/responses.py
 suvvyapi/sync/__init__.py
 suvvyapi/sync/wrapper.py
```


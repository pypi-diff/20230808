# Comparing `tmp/openapify-0.3.8.tar.gz` & `tmp/openapify-0.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openapify-0.3.8.tar", last modified: Wed Apr 19 10:24:44 2023, max compression
+gzip compressed data, was "openapify-0.3.9.tar", last modified: Tue Aug  8 09:24:44 2023, max compression
```

## Comparing `openapify-0.3.8.tar` & `openapify-0.3.9.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 alexander.tikhonov   (503) staff       (20)        0 2023-04-19 10:24:44.154322 openapify-0.3.8/
--rw-r--r--   0 alexander.tikhonov   (503) staff       (20)    10763 2023-04-11 22:14:24.000000 openapify-0.3.8/LICENSE
--rw-r--r--   0 alexander.tikhonov   (503) staff       (20)    30602 2023-04-19 10:24:44.154186 openapify-0.3.8/PKG-INFO
--rw-r--r--   0 alexander.tikhonov   (503) staff       (20)    29739 2023-04-19 10:07:41.000000 openapify-0.3.8/README.md
-drwxr-xr-x   0 alexander.tikhonov   (503) staff       (20)        0 2023-04-19 10:24:44.151073 openapify-0.3.8/openapify/
--rw-r--r--   0 alexander.tikhonov   (503) staff       (20)      498 2023-04-19 10:06:31.000000 openapify-0.3.8/openapify/__init__.py
-drwxr-xr-x   0 alexander.tikhonov   (503) staff       (20)        0 2023-04-19 10:24:44.153058 openapify-0.3.8/openapify/core/
--rw-r--r--   0 alexander.tikhonov   (503) staff       (20)        0 2023-04-10 08:32:02.000000 openapify-0.3.8/openapify/core/__init__.py
--rw-r--r--   0 alexander.tikhonov   (503) staff       (20)    15792 2023-04-19 10:07:08.000000 openapify-0.3.8/openapify/core/builder.py
--rw-r--r--   0 alexander.tikhonov   (503) staff       (20)     2120 2023-04-13 11:29:19.000000 openapify-0.3.8/openapify/core/const.py
--rw-r--r--   0 alexander.tikhonov   (503) staff       (20)     2247 2023-04-14 10:18:14.000000 openapify-0.3.8/openapify/core/document.py
--rw-r--r--   0 alexander.tikhonov   (503) staff       (20)     1720 2023-04-13 18:04:05.000000 openapify-0.3.8/openapify/core/jsonschema.py
--rw-r--r--   0 alexander.tikhonov   (503) staff       (20)     1971 2023-04-14 14:51:07.000000 openapify-0.3.8/openapify/core/models.py
-drwxr-xr-x   0 alexander.tikhonov   (503) staff       (20)        0 2023-04-19 10:24:44.153384 openapify-0.3.8/openapify/core/openapi/
--rw-r--r--   0 alexander.tikhonov   (503) staff       (20)        0 2023-04-10 08:32:02.000000 openapify-0.3.8/openapify/core/openapi/__init__.py
--rw-r--r--   0 alexander.tikhonov   (503) staff       (20)     5299 2023-04-14 15:52:57.000000 openapify-0.3.8/openapify/core/openapi/models.py
--rw-r--r--   0 alexander.tikhonov   (503) staff       (20)     5409 2023-04-19 10:06:31.000000 openapify-0.3.8/openapify/decorators.py
-drwxr-xr-x   0 alexander.tikhonov   (503) staff       (20)        0 2023-04-19 10:24:44.153626 openapify-0.3.8/openapify/ext/
--rw-r--r--   0 alexander.tikhonov   (503) staff       (20)        0 2023-04-10 08:32:02.000000 openapify-0.3.8/openapify/ext/__init__.py
-drwxr-xr-x   0 alexander.tikhonov   (503) staff       (20)        0 2023-04-19 10:24:44.153814 openapify-0.3.8/openapify/ext/web/
--rw-r--r--   0 alexander.tikhonov   (503) staff       (20)        0 2023-04-10 08:32:02.000000 openapify-0.3.8/openapify/ext/web/__init__.py
--rw-r--r--   0 alexander.tikhonov   (503) staff       (20)     4767 2023-04-11 22:14:24.000000 openapify-0.3.8/openapify/ext/web/aiohttp.py
--rw-r--r--   0 alexander.tikhonov   (503) staff       (20)        0 2023-04-10 08:32:02.000000 openapify-0.3.8/openapify/py.typed
-drwxr-xr-x   0 alexander.tikhonov   (503) staff       (20)        0 2023-04-19 10:24:44.151884 openapify-0.3.8/openapify.egg-info/
--rw-r--r--   0 alexander.tikhonov   (503) staff       (20)    30602 2023-04-19 10:24:44.000000 openapify-0.3.8/openapify.egg-info/PKG-INFO
--rw-r--r--   0 alexander.tikhonov   (503) staff       (20)      613 2023-04-19 10:24:44.000000 openapify-0.3.8/openapify.egg-info/SOURCES.txt
--rw-r--r--   0 alexander.tikhonov   (503) staff       (20)        1 2023-04-19 10:24:44.000000 openapify-0.3.8/openapify.egg-info/dependency_links.txt
--rw-r--r--   0 alexander.tikhonov   (503) staff       (20)        1 2023-04-10 17:48:20.000000 openapify-0.3.8/openapify.egg-info/not-zip-safe
--rw-r--r--   0 alexander.tikhonov   (503) staff       (20)       42 2023-04-19 10:24:44.000000 openapify-0.3.8/openapify.egg-info/requires.txt
--rw-r--r--   0 alexander.tikhonov   (503) staff       (20)       10 2023-04-19 10:24:44.000000 openapify-0.3.8/openapify.egg-info/top_level.txt
--rw-r--r--   0 alexander.tikhonov   (503) staff       (20)      364 2023-04-10 08:32:02.000000 openapify-0.3.8/pyproject.toml
--rw-r--r--   0 alexander.tikhonov   (503) staff       (20)       38 2023-04-19 10:24:44.154360 openapify-0.3.8/setup.cfg
--rw-r--r--   0 alexander.tikhonov   (503) staff       (20)     1298 2023-04-19 10:24:17.000000 openapify-0.3.8/setup.py
+drwxr-xr-x   0 tikhonov_a   (501) staff       (20)        0 2023-08-08 09:24:44.493773 openapify-0.3.9/
+-rw-r--r--   0 tikhonov_a   (501) staff       (20)    10763 2023-08-08 09:24:28.000000 openapify-0.3.9/LICENSE
+-rw-r--r--   0 tikhonov_a   (501) staff       (20)    30592 2023-08-08 09:24:44.493615 openapify-0.3.9/PKG-INFO
+-rw-r--r--   0 tikhonov_a   (501) staff       (20)    29729 2023-08-08 09:24:28.000000 openapify-0.3.9/README.md
+drwxr-xr-x   0 tikhonov_a   (501) staff       (20)        0 2023-08-08 09:24:44.491606 openapify-0.3.9/openapify/
+-rw-r--r--   0 tikhonov_a   (501) staff       (20)      498 2023-08-08 09:24:28.000000 openapify-0.3.9/openapify/__init__.py
+drwxr-xr-x   0 tikhonov_a   (501) staff       (20)        0 2023-08-08 09:24:44.492939 openapify-0.3.9/openapify/core/
+-rw-r--r--   0 tikhonov_a   (501) staff       (20)        0 2023-08-08 09:24:28.000000 openapify-0.3.9/openapify/core/__init__.py
+-rw-r--r--   0 tikhonov_a   (501) staff       (20)    15792 2023-08-08 09:24:28.000000 openapify-0.3.9/openapify/core/builder.py
+-rw-r--r--   0 tikhonov_a   (501) staff       (20)     2120 2023-08-08 09:24:28.000000 openapify-0.3.9/openapify/core/const.py
+-rw-r--r--   0 tikhonov_a   (501) staff       (20)     2247 2023-08-08 09:24:28.000000 openapify-0.3.9/openapify/core/document.py
+-rw-r--r--   0 tikhonov_a   (501) staff       (20)     1720 2023-08-08 09:24:28.000000 openapify-0.3.9/openapify/core/jsonschema.py
+-rw-r--r--   0 tikhonov_a   (501) staff       (20)     1971 2023-08-08 09:24:28.000000 openapify-0.3.9/openapify/core/models.py
+drwxr-xr-x   0 tikhonov_a   (501) staff       (20)        0 2023-08-08 09:24:44.493127 openapify-0.3.9/openapify/core/openapi/
+-rw-r--r--   0 tikhonov_a   (501) staff       (20)        0 2023-08-08 09:24:28.000000 openapify-0.3.9/openapify/core/openapi/__init__.py
+-rw-r--r--   0 tikhonov_a   (501) staff       (20)     5333 2023-08-08 09:24:28.000000 openapify-0.3.9/openapify/core/openapi/models.py
+-rw-r--r--   0 tikhonov_a   (501) staff       (20)     5409 2023-08-08 09:24:28.000000 openapify-0.3.9/openapify/decorators.py
+drwxr-xr-x   0 tikhonov_a   (501) staff       (20)        0 2023-08-08 09:24:44.493227 openapify-0.3.9/openapify/ext/
+-rw-r--r--   0 tikhonov_a   (501) staff       (20)        0 2023-08-08 09:24:28.000000 openapify-0.3.9/openapify/ext/__init__.py
+drwxr-xr-x   0 tikhonov_a   (501) staff       (20)        0 2023-08-08 09:24:44.493390 openapify-0.3.9/openapify/ext/web/
+-rw-r--r--   0 tikhonov_a   (501) staff       (20)        0 2023-08-08 09:24:28.000000 openapify-0.3.9/openapify/ext/web/__init__.py
+-rw-r--r--   0 tikhonov_a   (501) staff       (20)     4767 2023-08-08 09:24:28.000000 openapify-0.3.9/openapify/ext/web/aiohttp.py
+-rw-r--r--   0 tikhonov_a   (501) staff       (20)        0 2023-08-08 09:24:28.000000 openapify-0.3.9/openapify/py.typed
+drwxr-xr-x   0 tikhonov_a   (501) staff       (20)        0 2023-08-08 09:24:44.492297 openapify-0.3.9/openapify.egg-info/
+-rw-r--r--   0 tikhonov_a   (501) staff       (20)    30592 2023-08-08 09:24:44.000000 openapify-0.3.9/openapify.egg-info/PKG-INFO
+-rw-r--r--   0 tikhonov_a   (501) staff       (20)      613 2023-08-08 09:24:44.000000 openapify-0.3.9/openapify.egg-info/SOURCES.txt
+-rw-r--r--   0 tikhonov_a   (501) staff       (20)        1 2023-08-08 09:24:44.000000 openapify-0.3.9/openapify.egg-info/dependency_links.txt
+-rw-r--r--   0 tikhonov_a   (501) staff       (20)        1 2023-08-08 09:24:44.000000 openapify-0.3.9/openapify.egg-info/not-zip-safe
+-rw-r--r--   0 tikhonov_a   (501) staff       (20)       42 2023-08-08 09:24:44.000000 openapify-0.3.9/openapify.egg-info/requires.txt
+-rw-r--r--   0 tikhonov_a   (501) staff       (20)       10 2023-08-08 09:24:44.000000 openapify-0.3.9/openapify.egg-info/top_level.txt
+-rw-r--r--   0 tikhonov_a   (501) staff       (20)      364 2023-08-08 09:24:28.000000 openapify-0.3.9/pyproject.toml
+-rw-r--r--   0 tikhonov_a   (501) staff       (20)       38 2023-08-08 09:24:44.493822 openapify-0.3.9/setup.cfg
+-rw-r--r--   0 tikhonov_a   (501) staff       (20)     1298 2023-08-08 09:24:28.000000 openapify-0.3.9/setup.py
```

### Comparing `openapify-0.3.8/LICENSE` & `openapify-0.3.9/LICENSE`

 * *Files identical despite different names*

### Comparing `openapify-0.3.8/PKG-INFO` & `openapify-0.3.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openapify
-Version: 0.3.8
+Version: 0.3.9
 Summary: Framework agnostic OpenAPI Specification generation for code lovers
 Home-page: https://github.com/Fatal1ty/openapify
 Author: Alexander Tikhonov
 Author-email: random.gauss@gmail.com
 License: Apache License, Version 2.0
 Platform: all
 Classifier: License :: OSI Approved :: Apache Software License
@@ -41,16 +41,15 @@
 
 Openapify is based on the idea of applying decorators on route handlers. Any
 web-framework has a routing system that let us link a route to a handler
 (a high-level function or a class method). By using decorators, we can add
 information about requests, responses and other details that will then be used
 to create an entire OpenAPI document.
 
-> **Warning**
->
+> [!WARNING]\
 > This library is currently in pre-release stage and may have backward
 > incompatible changes prior to version 1.0. Please use caution when using this
 > library in production environments and be sure to thoroughly test any updates
 > before upgrading to a new version.
 
 Table of contents
 --------------------------------------------------------------------------------
@@ -76,16 +75,15 @@
 ```shell
 $ pip install openapify
 ```
 
 Quickstart
 --------------------------------------------------------------------------------
 
-> **Note**
->
+> [!NOTE]\
 > In the following example, we will intentionally demonstrate the process of
 > creating an OpenAPI document without being tied to a specific web-framework.
 > However, this process may be easier on a supported web-framework.
 > See [Integration with web-frameworks](#integration-with-web-frameworks) for
 > more info.
 
 Let's see how to build an OpenAPI document with openapify. Suppose we are
@@ -1065,15 +1063,15 @@
       security:
       - x-auth-token: []
 components:
   securitySchemes:
     x-auth-token:
       type: apiKey
       name: X-Auh-Token
-      location: header
+      in: header
 ```
 
 Entity schema builders
 --------------------------------------------------------------------------------
 
 In some decorators you should pass Python data type for which the JSON Schema
 is being built by openapify in order to get the correct OpenAPI document.
```

### Comparing `openapify-0.3.8/README.md` & `openapify-0.3.9/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -18,16 +18,15 @@
 
 Openapify is based on the idea of applying decorators on route handlers. Any
 web-framework has a routing system that let us link a route to a handler
 (a high-level function or a class method). By using decorators, we can add
 information about requests, responses and other details that will then be used
 to create an entire OpenAPI document.
 
-> **Warning**
->
+> [!WARNING]\
 > This library is currently in pre-release stage and may have backward
 > incompatible changes prior to version 1.0. Please use caution when using this
 > library in production environments and be sure to thoroughly test any updates
 > before upgrading to a new version.
 
 Table of contents
 --------------------------------------------------------------------------------
@@ -53,16 +52,15 @@
 ```shell
 $ pip install openapify
 ```
 
 Quickstart
 --------------------------------------------------------------------------------
 
-> **Note**
->
+> [!NOTE]\
 > In the following example, we will intentionally demonstrate the process of
 > creating an OpenAPI document without being tied to a specific web-framework.
 > However, this process may be easier on a supported web-framework.
 > See [Integration with web-frameworks](#integration-with-web-frameworks) for
 > more info.
 
 Let's see how to build an OpenAPI document with openapify. Suppose we are
@@ -1042,15 +1040,15 @@
       security:
       - x-auth-token: []
 components:
   securitySchemes:
     x-auth-token:
       type: apiKey
       name: X-Auh-Token
-      location: header
+      in: header
 ```
 
 Entity schema builders
 --------------------------------------------------------------------------------
 
 In some decorators you should pass Python data type for which the JSON Schema
 is being built by openapify in order to get the correct OpenAPI document.
```

### Comparing `openapify-0.3.8/openapify/core/builder.py` & `openapify-0.3.9/openapify/core/builder.py`

 * *Files identical despite different names*

### Comparing `openapify-0.3.8/openapify/core/const.py` & `openapify-0.3.9/openapify/core/const.py`

 * *Files identical despite different names*

### Comparing `openapify-0.3.8/openapify/core/document.py` & `openapify-0.3.9/openapify/core/document.py`

 * *Files identical despite different names*

### Comparing `openapify-0.3.8/openapify/core/jsonschema.py` & `openapify-0.3.9/openapify/core/jsonschema.py`

 * *Files identical despite different names*

### Comparing `openapify-0.3.8/openapify/core/models.py` & `openapify-0.3.9/openapify/core/models.py`

 * *Files identical despite different names*

### Comparing `openapify-0.3.8/openapify/core/openapi/models.py` & `openapify-0.3.9/openapify/core/openapi/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -143,14 +143,15 @@
 class APIKeySecurityScheme(SecurityScheme):
     name: Optional[str] = None
     location: SecuritySchemeAPIKeyLocation = SecuritySchemeAPIKeyLocation.QUERY
     type: Literal[SecuritySchemeType.API_KEY] = SecuritySchemeType.API_KEY
     description: Optional[str] = None
 
     class Config(Object.Config):
+        serialize_by_alias = True
         aliases = {"location": "in"}
 
 
 @dataclass
 class HTTPSecurityScheme(SecurityScheme):
     scheme: str = "basic"
     type: Literal[SecuritySchemeType.HTTP] = SecuritySchemeType.HTTP
```

### Comparing `openapify-0.3.8/openapify/decorators.py` & `openapify-0.3.9/openapify/decorators.py`

 * *Files identical despite different names*

### Comparing `openapify-0.3.8/openapify/ext/web/aiohttp.py` & `openapify-0.3.9/openapify/ext/web/aiohttp.py`

 * *Files identical despite different names*

### Comparing `openapify-0.3.8/openapify.egg-info/PKG-INFO` & `openapify-0.3.9/openapify.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openapify
-Version: 0.3.8
+Version: 0.3.9
 Summary: Framework agnostic OpenAPI Specification generation for code lovers
 Home-page: https://github.com/Fatal1ty/openapify
 Author: Alexander Tikhonov
 Author-email: random.gauss@gmail.com
 License: Apache License, Version 2.0
 Platform: all
 Classifier: License :: OSI Approved :: Apache Software License
@@ -41,16 +41,15 @@
 
 Openapify is based on the idea of applying decorators on route handlers. Any
 web-framework has a routing system that let us link a route to a handler
 (a high-level function or a class method). By using decorators, we can add
 information about requests, responses and other details that will then be used
 to create an entire OpenAPI document.
 
-> **Warning**
->
+> [!WARNING]\
 > This library is currently in pre-release stage and may have backward
 > incompatible changes prior to version 1.0. Please use caution when using this
 > library in production environments and be sure to thoroughly test any updates
 > before upgrading to a new version.
 
 Table of contents
 --------------------------------------------------------------------------------
@@ -76,16 +75,15 @@
 ```shell
 $ pip install openapify
 ```
 
 Quickstart
 --------------------------------------------------------------------------------
 
-> **Note**
->
+> [!NOTE]\
 > In the following example, we will intentionally demonstrate the process of
 > creating an OpenAPI document without being tied to a specific web-framework.
 > However, this process may be easier on a supported web-framework.
 > See [Integration with web-frameworks](#integration-with-web-frameworks) for
 > more info.
 
 Let's see how to build an OpenAPI document with openapify. Suppose we are
@@ -1065,15 +1063,15 @@
       security:
       - x-auth-token: []
 components:
   securitySchemes:
     x-auth-token:
       type: apiKey
       name: X-Auh-Token
-      location: header
+      in: header
 ```
 
 Entity schema builders
 --------------------------------------------------------------------------------
 
 In some decorators you should pass Python data type for which the JSON Schema
 is being built by openapify in order to get the correct OpenAPI document.
```

### Comparing `openapify-0.3.8/openapify.egg-info/SOURCES.txt` & `openapify-0.3.9/openapify.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `openapify-0.3.8/setup.py` & `openapify-0.3.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 #!/usr/bin/env python
 
 from setuptools import find_packages, setup
 
 setup(
     name="openapify",
-    version="0.3.8",
+    version="0.3.9",
     description=(
         "Framework agnostic OpenAPI Specification generation for code lovers"
     ),
     long_description=open("README.md", encoding="utf8").read(),
     long_description_content_type="text/markdown",
     platforms="all",
     classifiers=[
```


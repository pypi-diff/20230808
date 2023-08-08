# Comparing `tmp/simple-openapi-client-0.3.0.tar.gz` & `tmp/simple_openapi_client-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "simple-openapi-client-0.3.0.tar", max compression
+gzip compressed data, was "simple_openapi_client-0.3.1.tar", max compression
```

## Comparing `simple-openapi-client-0.3.0.tar` & `simple_openapi_client-0.3.1.tar`

### file list

```diff
@@ -1,16 +1,15 @@
--rw-r--r--   0        0        0     1423 2022-12-18 02:39:16.255314 simple-openapi-client-0.3.0/README.md
--rw-r--r--   0        0        0      535 2022-12-27 03:37:52.467168 simple-openapi-client-0.3.0/pyproject.toml
--rw-r--r--   0        0        0      161 2022-12-18 02:39:16.257314 simple-openapi-client-0.3.0/simple_openapi_client/__init__.py
--rw-r--r--   0        0        0      126 2022-12-18 02:39:16.257314 simple-openapi-client-0.3.0/simple_openapi_client/config.py
--rw-r--r--   0        0        0     5929 2022-12-18 02:39:16.257314 simple-openapi-client-0.3.0/simple_openapi_client/maker.py
--rw-r--r--   0        0        0       61 2022-12-18 02:39:16.258314 simple-openapi-client-0.3.0/simple_openapi_client/openapi/__init__.py
--rw-r--r--   0        0        0      560 2022-12-18 02:39:16.258314 simple-openapi-client-0.3.0/simple_openapi_client/openapi/document.py
--rw-r--r--   0        0        0      361 2022-12-18 02:39:16.258314 simple-openapi-client-0.3.0/simple_openapi_client/openapi/info.py
--rw-r--r--   0        0        0     3461 2022-12-18 02:39:16.258314 simple-openapi-client-0.3.0/simple_openapi_client/openapi/path.py
--rw-r--r--   0        0        0      451 2022-12-18 02:39:16.259314 simple-openapi-client-0.3.0/simple_openapi_client/parser.py
--rw-r--r--   0        0        0     6255 2022-12-27 02:25:20.740487 simple-openapi-client-0.3.0/simple_openapi_client/templates/async_client.jinja
--rw-r--r--   0        0        0     4063 2022-12-18 02:39:16.259314 simple-openapi-client-0.3.0/simple_openapi_client/templates/async_method.jinja
--rw-r--r--   0        0        0     6058 2022-12-27 02:24:35.901132 simple-openapi-client-0.3.0/simple_openapi_client/templates/client.jinja
--rw-r--r--   0        0        0     4043 2022-12-18 02:39:16.260314 simple-openapi-client-0.3.0/simple_openapi_client/templates/method.jinja
--rw-r--r--   0        0        0     2306 2022-12-27 03:38:26.427436 simple-openapi-client-0.3.0/setup.py
--rw-r--r--   0        0        0     2131 2022-12-27 03:38:26.429490 simple-openapi-client-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1423 2022-12-18 02:39:16.255314 simple_openapi_client-0.3.1/README.md
+-rw-r--r--   0        0        0      535 2023-08-08 17:07:52.301162 simple_openapi_client-0.3.1/pyproject.toml
+-rw-r--r--   0        0        0      161 2022-12-18 02:39:16.257314 simple_openapi_client-0.3.1/simple_openapi_client/__init__.py
+-rw-r--r--   0        0        0      126 2022-12-18 02:39:16.257314 simple_openapi_client-0.3.1/simple_openapi_client/config.py
+-rw-r--r--   0        0        0     5929 2022-12-18 02:39:16.257314 simple_openapi_client-0.3.1/simple_openapi_client/maker.py
+-rw-r--r--   0        0        0       61 2022-12-18 02:39:16.258314 simple_openapi_client-0.3.1/simple_openapi_client/openapi/__init__.py
+-rw-r--r--   0        0        0      560 2022-12-18 02:39:16.258314 simple_openapi_client-0.3.1/simple_openapi_client/openapi/document.py
+-rw-r--r--   0        0        0      361 2022-12-18 02:39:16.258314 simple_openapi_client-0.3.1/simple_openapi_client/openapi/info.py
+-rw-r--r--   0        0        0     3461 2022-12-18 02:39:16.258314 simple_openapi_client-0.3.1/simple_openapi_client/openapi/path.py
+-rw-r--r--   0        0        0      451 2022-12-18 02:39:16.259314 simple_openapi_client-0.3.1/simple_openapi_client/parser.py
+-rw-r--r--   0        0        0     6255 2023-08-08 16:54:39.315622 simple_openapi_client-0.3.1/simple_openapi_client/templates/async_client.jinja
+-rw-r--r--   0        0        0     4063 2022-12-18 02:39:16.259314 simple_openapi_client-0.3.1/simple_openapi_client/templates/async_method.jinja
+-rw-r--r--   0        0        0     6058 2023-08-08 16:54:39.316622 simple_openapi_client-0.3.1/simple_openapi_client/templates/client.jinja
+-rw-r--r--   0        0        0     4043 2022-12-18 02:39:16.260314 simple_openapi_client-0.3.1/simple_openapi_client/templates/method.jinja
+-rw-r--r--   0        0        0     2182 1970-01-01 00:00:00.000000 simple_openapi_client-0.3.1/PKG-INFO
```

### Comparing `simple-openapi-client-0.3.0/README.md` & `simple_openapi_client-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `simple-openapi-client-0.3.0/pyproject.toml` & `simple_openapi_client-0.3.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 [tool.poetry]
 name = "simple-openapi-client"
-version = "0.3.0"
+version = "0.3.1"
 description = "OpenAPI Python client generator that follows the KISS principle."
 authors = ["Gabriel Couture <gacou54@gmail.ca>"]
 license = "BSD-3-Clause"
 readme = 'README.md'
 homepage = 'https://github.com/gacou54/openapi-client'
 
 [tool.poetry.dependencies]
 python = "^3.8"
-httpx = "^0.23.0"
+httpx = "^0.24.1"
 Jinja2 = "^3.1.2"
 black = "^22.6.0"
 
 [tool.poetry.dev-dependencies]
 pytest = "^7.1.2"
 
 [build-system]
```

### Comparing `simple-openapi-client-0.3.0/simple_openapi_client/maker.py` & `simple_openapi_client-0.3.1/simple_openapi_client/maker.py`

 * *Files identical despite different names*

### Comparing `simple-openapi-client-0.3.0/simple_openapi_client/openapi/document.py` & `simple_openapi_client-0.3.1/simple_openapi_client/openapi/document.py`

 * *Files identical despite different names*

### Comparing `simple-openapi-client-0.3.0/simple_openapi_client/openapi/path.py` & `simple_openapi_client-0.3.1/simple_openapi_client/openapi/path.py`

 * *Files identical despite different names*

### Comparing `simple-openapi-client-0.3.0/simple_openapi_client/templates/async_client.jinja` & `simple_openapi_client-0.3.1/simple_openapi_client/templates/async_client.jinja`

 * *Files identical despite different names*

### Comparing `simple-openapi-client-0.3.0/simple_openapi_client/templates/async_method.jinja` & `simple_openapi_client-0.3.1/simple_openapi_client/templates/async_method.jinja`

 * *Files identical despite different names*

### Comparing `simple-openapi-client-0.3.0/simple_openapi_client/templates/client.jinja` & `simple_openapi_client-0.3.1/simple_openapi_client/templates/client.jinja`

 * *Files identical despite different names*

### Comparing `simple-openapi-client-0.3.0/simple_openapi_client/templates/method.jinja` & `simple_openapi_client-0.3.1/simple_openapi_client/templates/method.jinja`

 * *Files identical despite different names*

### Comparing `simple-openapi-client-0.3.0/PKG-INFO` & `simple_openapi_client-0.3.1/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 Metadata-Version: 2.1
 Name: simple-openapi-client
-Version: 0.3.0
+Version: 0.3.1
 Summary: OpenAPI Python client generator that follows the KISS principle.
 Home-page: https://github.com/gacou54/openapi-client
 License: BSD-3-Clause
 Author: Gabriel Couture
 Author-email: gacou54@gmail.ca
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: Jinja2 (>=3.1.2,<4.0.0)
 Requires-Dist: black (>=22.6.0,<23.0.0)
-Requires-Dist: httpx (>=0.23.0,<0.24.0)
+Requires-Dist: httpx (>=0.24.1,<0.25.0)
 Description-Content-Type: text/markdown
 
 # Simple Open API Client generator
 
 This project was made to generate a simple client (async or not) from an openapi
 specifications (unlike other client generators, which typically produce
 code that is difficult for python beginners to use). It aims to produce a
```


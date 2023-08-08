# Comparing `tmp/highlight_io-0.5.5.tar.gz` & `tmp/highlight_io-0.5.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "highlight_io-0.5.5.tar", max compression
+gzip compressed data, was "highlight_io-0.5.6.tar", max compression
```

## Comparing `highlight_io-0.5.5.tar` & `highlight_io-0.5.6.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0      867 2023-08-04 21:53:02.985756 highlight_io-0.5.5/README.md
--rw-r--r--   0        0        0       64 2023-08-04 21:53:02.985756 highlight_io-0.5.5/highlight_io/__init__.py
--rw-r--r--   0        0        0      155 2023-08-04 21:53:02.985756 highlight_io-0.5.5/highlight_io/integrations/__init__.py
--rw-r--r--   0        0        0      717 2023-08-04 21:53:02.985756 highlight_io-0.5.5/highlight_io/integrations/aws.py
--rw-r--r--   0        0        0      740 2023-08-04 21:53:02.985756 highlight_io-0.5.5/highlight_io/integrations/azure.py
--rw-r--r--   0        0        0     1631 2023-08-04 21:53:02.985756 highlight_io-0.5.5/highlight_io/integrations/django.py
--rw-r--r--   0        0        0     1799 2023-08-04 21:53:02.985756 highlight_io-0.5.5/highlight_io/integrations/fastapi.py
--rw-r--r--   0        0        0     1519 2023-08-04 21:53:02.985756 highlight_io-0.5.5/highlight_io/integrations/flask.py
--rw-r--r--   0        0        0      747 2023-08-04 21:53:02.985756 highlight_io-0.5.5/highlight_io/integrations/gcp.py
--rw-r--r--   0        0        0     1072 2023-08-04 21:53:02.985756 highlight_io-0.5.5/highlight_io/integrations/serverless.py
--rw-r--r--   0        0        0    12453 2023-08-04 21:53:02.985756 highlight_io-0.5.5/highlight_io/sdk.py
--rw-r--r--   0        0        0     1688 2023-08-04 21:53:02.985756 highlight_io-0.5.5/pyproject.toml
--rw-r--r--   0        0        0     2567 1970-01-01 00:00:00.000000 highlight_io-0.5.5/PKG-INFO
+-rw-r--r--   0        0        0      867 2023-08-08 02:57:21.728019 highlight_io-0.5.6/README.md
+-rw-r--r--   0        0        0       64 2023-08-08 02:57:21.728019 highlight_io-0.5.6/highlight_io/__init__.py
+-rw-r--r--   0        0        0      155 2023-08-08 02:57:21.728019 highlight_io-0.5.6/highlight_io/integrations/__init__.py
+-rw-r--r--   0        0        0      717 2023-08-08 02:57:21.728019 highlight_io-0.5.6/highlight_io/integrations/aws.py
+-rw-r--r--   0        0        0      740 2023-08-08 02:57:21.728019 highlight_io-0.5.6/highlight_io/integrations/azure.py
+-rw-r--r--   0        0        0     1631 2023-08-08 02:57:21.728019 highlight_io-0.5.6/highlight_io/integrations/django.py
+-rw-r--r--   0        0        0     1799 2023-08-08 02:57:21.728019 highlight_io-0.5.6/highlight_io/integrations/fastapi.py
+-rw-r--r--   0        0        0     1519 2023-08-08 02:57:21.728019 highlight_io-0.5.6/highlight_io/integrations/flask.py
+-rw-r--r--   0        0        0      747 2023-08-08 02:57:21.728019 highlight_io-0.5.6/highlight_io/integrations/gcp.py
+-rw-r--r--   0        0        0     1072 2023-08-08 02:57:21.728019 highlight_io-0.5.6/highlight_io/integrations/serverless.py
+-rw-r--r--   0        0        0    12453 2023-08-08 02:57:21.728019 highlight_io-0.5.6/highlight_io/sdk.py
+-rw-r--r--   0        0        0     1689 2023-08-08 02:57:21.728019 highlight_io-0.5.6/pyproject.toml
+-rw-r--r--   0        0        0     2561 1970-01-01 00:00:00.000000 highlight_io-0.5.6/PKG-INFO
```

### Comparing `highlight_io-0.5.5/README.md` & `highlight_io-0.5.6/README.md`

 * *Files identical despite different names*

### Comparing `highlight_io-0.5.5/highlight_io/integrations/aws.py` & `highlight_io-0.5.6/highlight_io/integrations/aws.py`

 * *Files identical despite different names*

### Comparing `highlight_io-0.5.5/highlight_io/integrations/azure.py` & `highlight_io-0.5.6/highlight_io/integrations/azure.py`

 * *Files identical despite different names*

### Comparing `highlight_io-0.5.5/highlight_io/integrations/django.py` & `highlight_io-0.5.6/highlight_io/integrations/django.py`

 * *Files identical despite different names*

### Comparing `highlight_io-0.5.5/highlight_io/integrations/fastapi.py` & `highlight_io-0.5.6/highlight_io/integrations/fastapi.py`

 * *Files identical despite different names*

### Comparing `highlight_io-0.5.5/highlight_io/integrations/flask.py` & `highlight_io-0.5.6/highlight_io/integrations/flask.py`

 * *Files identical despite different names*

### Comparing `highlight_io-0.5.5/highlight_io/integrations/gcp.py` & `highlight_io-0.5.6/highlight_io/integrations/gcp.py`

 * *Files identical despite different names*

### Comparing `highlight_io-0.5.5/highlight_io/integrations/serverless.py` & `highlight_io-0.5.6/highlight_io/integrations/serverless.py`

 * *Files identical despite different names*

### Comparing `highlight_io-0.5.5/highlight_io/sdk.py` & `highlight_io-0.5.6/highlight_io/sdk.py`

 * *Files identical despite different names*

### Comparing `highlight_io-0.5.5/pyproject.toml` & `highlight_io-0.5.6/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "highlight-io"
-version = "0.5.5"
+version = "0.5.6"
 description = "Session replay and error monitoring: stop guessing why bugs happen!"
 license = "Apache-2.0"
 authors = [
     "Vadim Korolik <vadim@highlight.io>",
     "Jay Khatri <jay@highlight.io>",
 ]
 readme = "README.md"
@@ -26,15 +26,15 @@
 
 [tool.poetry.dependencies]
 python = "^3.8"
 blinker = { version = "^1.5", optional = true }
 django = { version = "^4.1", optional = true }
 flask = { version = "^2.2", optional = true }
 fastapi = { version = ">=0.92", optional = true }
-uvicorn = {version = "^0.20", extras = ["standard"], optional = true }
+uvicorn = {version = ">=0.20", extras = ["standard"], optional = true }
 opentelemetry-api = "1.19.0"
 opentelemetry-distro = { extras = ["otlp"], version = "0.40b0" }
 opentelemetry-exporter-otlp-proto-http = "1.19.0"
 opentelemetry-instrumentation = "0.40b0"
 opentelemetry-instrumentation-logging = "0.40b0"
 opentelemetry-proto = "1.19.0"
 opentelemetry-sdk = "1.19.0"
```

### Comparing `highlight_io-0.5.5/PKG-INFO` & `highlight_io-0.5.6/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: highlight-io
-Version: 0.5.5
+Version: 0.5.6
 Summary: Session replay and error monitoring: stop guessing why bugs happen!
 Home-page: https://www.highlight.io
 License: Apache-2.0
 Keywords: web,framework
 Author: Vadim Korolik
 Author-email: vadim@highlight.io
 Requires-Python: >=3.8,<4.0
@@ -29,15 +29,15 @@
 Requires-Dist: opentelemetry-api (==1.19.0)
 Requires-Dist: opentelemetry-distro[otlp] (==0.40b0)
 Requires-Dist: opentelemetry-exporter-otlp-proto-http (==1.19.0)
 Requires-Dist: opentelemetry-instrumentation (==0.40b0)
 Requires-Dist: opentelemetry-instrumentation-logging (==0.40b0)
 Requires-Dist: opentelemetry-proto (==1.19.0)
 Requires-Dist: opentelemetry-sdk (==1.19.0)
-Requires-Dist: uvicorn[standard] (>=0.20,<0.21) ; extra == "fastapi"
+Requires-Dist: uvicorn[standard] (>=0.20) ; extra == "fastapi"
 Project-URL: Documentation, https://www.highlight.io/docs
 Project-URL: Repository, https://github.com/highlight/highlight
 Description-Content-Type: text/markdown
 
 # highlight-io Python SDK
 
 This directory contains the source code for the Highlight Python SDK.
```


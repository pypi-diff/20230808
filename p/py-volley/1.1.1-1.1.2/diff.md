# Comparing `tmp/py_volley-1.1.1.tar.gz` & `tmp/py_volley-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py_volley-1.1.1.tar", max compression
+gzip compressed data, was "py_volley-1.1.2.tar", max compression
```

## Comparing `py_volley-1.1.1.tar` & `py_volley-1.1.2.tar`

### file list

```diff
@@ -1,29 +1,29 @@
--rw-r--r--   0        0        0     1068 2023-05-22 16:30:29.590656 py_volley-1.1.1/LICENSE.md
--rw-r--r--   0        0        0     8734 2023-05-22 16:30:29.590656 py_volley-1.1.1/README.md
--rw-r--r--   0        0        0     2728 2023-05-22 16:30:29.594656 py_volley-1.1.1/pyproject.toml
--rw-r--r--   0        0        0      132 2023-05-22 16:30:29.594656 py_volley-1.1.1/volley/__init__.py
--rw-r--r--   0        0        0     1932 2023-05-22 16:30:29.594656 py_volley-1.1.1/volley/concurrency.py
--rw-r--r--   0        0        0     4897 2023-05-22 16:30:29.594656 py_volley-1.1.1/volley/config.py
--rw-r--r--   0        0        0        0 2023-05-22 16:30:29.594656 py_volley-1.1.1/volley/connectors/__init__.py
--rw-r--r--   0        0        0     2329 2023-05-22 16:30:29.594656 py_volley-1.1.1/volley/connectors/base.py
--rw-r--r--   0        0        0    16383 2023-05-22 16:30:29.594656 py_volley-1.1.1/volley/connectors/confluent.py
--rw-r--r--   0        0        0     7372 2023-05-22 16:30:29.594656 py_volley-1.1.1/volley/connectors/rsmq.py
--rw-r--r--   0        0        0     3018 2023-05-22 16:30:29.594656 py_volley-1.1.1/volley/connectors/zmq.py
--rw-r--r--   0        0        0      393 2023-05-22 16:30:29.594656 py_volley-1.1.1/volley/data_models.py
--rw-r--r--   0        0        0    12250 2023-05-22 16:30:29.594656 py_volley-1.1.1/volley/engine.py
--rw-r--r--   0        0        0     3150 2023-05-22 16:30:29.594656 py_volley-1.1.1/volley/global.yml
--rw-r--r--   0        0        0       53 2023-05-22 16:30:29.594656 py_volley-1.1.1/volley/logging.py
--rw-r--r--   0        0        0     1686 2023-05-22 16:30:29.598657 py_volley-1.1.1/volley/metrics.py
--rw-r--r--   0        0        0      253 2023-05-22 16:30:29.598657 py_volley-1.1.1/volley/models/__init__.py
--rw-r--r--   0        0        0     4858 2023-05-22 16:30:29.598657 py_volley-1.1.1/volley/models/base.py
--rw-r--r--   0        0        0     2113 2023-05-22 16:30:29.598657 py_volley-1.1.1/volley/models/pydantic_model.py
--rw-r--r--   0        0        0     4279 2023-05-22 16:30:29.598657 py_volley-1.1.1/volley/profiles.py
--rw-r--r--   0        0        0     4078 2023-05-22 16:30:29.598657 py_volley-1.1.1/volley/queues.py
--rw-r--r--   0        0        0      285 2023-05-22 16:30:29.598657 py_volley-1.1.1/volley/serializers/__init__.py
--rw-r--r--   0        0        0      537 2023-05-22 16:30:29.598657 py_volley-1.1.1/volley/serializers/base.py
--rw-r--r--   0        0        0      453 2023-05-22 16:30:29.598657 py_volley-1.1.1/volley/serializers/json_serializer.py
--rw-r--r--   0        0        0      439 2023-05-22 16:30:29.598657 py_volley-1.1.1/volley/serializers/msgpack_serializer.py
--rw-r--r--   0        0        0      475 2023-05-22 16:30:29.598657 py_volley-1.1.1/volley/serializers/orjson_serializer.py
--rw-r--r--   0        0        0     4663 2023-05-22 16:30:29.598657 py_volley-1.1.1/volley/transport.py
--rw-r--r--   0        0        0     1742 2023-05-22 16:30:29.598657 py_volley-1.1.1/volley/util.py
--rw-r--r--   0        0        0    10074 1970-01-01 00:00:00.000000 py_volley-1.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1068 2023-08-07 22:21:17.872955 py_volley-1.1.2/LICENSE.md
+-rw-r--r--   0        0        0     8734 2023-08-07 22:21:17.872955 py_volley-1.1.2/README.md
+-rw-r--r--   0        0        0     2665 2023-08-07 22:21:17.896957 py_volley-1.1.2/pyproject.toml
+-rw-r--r--   0        0        0      132 2023-08-07 22:21:17.896957 py_volley-1.1.2/volley/__init__.py
+-rw-r--r--   0        0        0     1932 2023-08-07 22:21:17.896957 py_volley-1.1.2/volley/concurrency.py
+-rw-r--r--   0        0        0     4897 2023-08-07 22:21:17.896957 py_volley-1.1.2/volley/config.py
+-rw-r--r--   0        0        0        0 2023-08-07 22:21:17.896957 py_volley-1.1.2/volley/connectors/__init__.py
+-rw-r--r--   0        0        0     2329 2023-08-07 22:21:17.896957 py_volley-1.1.2/volley/connectors/base.py
+-rw-r--r--   0        0        0    16383 2023-08-07 22:21:17.896957 py_volley-1.1.2/volley/connectors/confluent.py
+-rw-r--r--   0        0        0     7372 2023-08-07 22:21:17.896957 py_volley-1.1.2/volley/connectors/rsmq.py
+-rw-r--r--   0        0        0     3018 2023-08-07 22:21:17.896957 py_volley-1.1.2/volley/connectors/zmq.py
+-rw-r--r--   0        0        0      393 2023-08-07 22:21:17.896957 py_volley-1.1.2/volley/data_models.py
+-rw-r--r--   0        0        0    12250 2023-08-07 22:21:17.896957 py_volley-1.1.2/volley/engine.py
+-rw-r--r--   0        0        0     3150 2023-08-07 22:21:17.896957 py_volley-1.1.2/volley/global.yml
+-rw-r--r--   0        0        0       53 2023-08-07 22:21:17.896957 py_volley-1.1.2/volley/logging.py
+-rw-r--r--   0        0        0     1686 2023-08-07 22:21:17.896957 py_volley-1.1.2/volley/metrics.py
+-rw-r--r--   0        0        0      253 2023-08-07 22:21:17.896957 py_volley-1.1.2/volley/models/__init__.py
+-rw-r--r--   0        0        0     4858 2023-08-07 22:21:17.896957 py_volley-1.1.2/volley/models/base.py
+-rw-r--r--   0        0        0     2113 2023-08-07 22:21:17.896957 py_volley-1.1.2/volley/models/pydantic_model.py
+-rw-r--r--   0        0        0     4279 2023-08-07 22:21:17.896957 py_volley-1.1.2/volley/profiles.py
+-rw-r--r--   0        0        0     4078 2023-08-07 22:21:17.896957 py_volley-1.1.2/volley/queues.py
+-rw-r--r--   0        0        0      285 2023-08-07 22:21:17.896957 py_volley-1.1.2/volley/serializers/__init__.py
+-rw-r--r--   0        0        0      537 2023-08-07 22:21:17.896957 py_volley-1.1.2/volley/serializers/base.py
+-rw-r--r--   0        0        0      453 2023-08-07 22:21:17.896957 py_volley-1.1.2/volley/serializers/json_serializer.py
+-rw-r--r--   0        0        0      439 2023-08-07 22:21:17.896957 py_volley-1.1.2/volley/serializers/msgpack_serializer.py
+-rw-r--r--   0        0        0      475 2023-08-07 22:21:17.896957 py_volley-1.1.2/volley/serializers/orjson_serializer.py
+-rw-r--r--   0        0        0     4663 2023-08-07 22:21:17.896957 py_volley-1.1.2/volley/transport.py
+-rw-r--r--   0        0        0     1742 2023-08-07 22:21:17.896957 py_volley-1.1.2/volley/util.py
+-rw-r--r--   0        0        0    10074 1970-01-01 00:00:00.000000 py_volley-1.1.2/PKG-INFO
```

### Comparing `py_volley-1.1.1/LICENSE.md` & `py_volley-1.1.2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `py_volley-1.1.1/README.md` & `py_volley-1.1.2/README.md`

 * *Files identical despite different names*

### Comparing `py_volley-1.1.1/pyproject.toml` & `py_volley-1.1.2/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,17 +1,15 @@
 [tool.poetry]
 name = "py_volley"
-version = "1.1.1"
+version = "1.1.2"
 description = "Pluggable message queueing for Python"
 authors = ["ask-machine-learning <shipt@shipt.com>"]
 readme = "README.md"
 
-packages = [
-    { include = "volley" },
-]
+packages = [{ include = "volley" }]
 
 [tool.poetry.urls]
 "Homepage" = "https://github.com/shipt/py-volley"
 "Repository" = "https://github.com/shipt/py-volley"
 "Documentation" = "https://shipt.github.io/py-volley/"
 
 [tool.poetry.dependencies]
@@ -20,31 +18,29 @@
 pydantic = "^1.8.2"
 PyYAML = "^6.0.0"
 orjson = "^3.6.4"
 msgpack = "^1.0.3"
 starlette = "^0"
 uvicorn = "^0"
 
-confluent-kafka = {version ="^2.0.0", optional = true}
-PyRSMQ = {version ="^0.4.5", optional = true}
-hiredis = {version ="^2.0", optional = true}
-tenacity = {version ="^8.0.1", optional = true}
-pyzmq = {version =">=22.3.0", optional = true}
+confluent-kafka = { version = "^2.0.0", optional = true }
+PyRSMQ = { version = "^0.4.5", optional = true }
+hiredis = { version = "^2.0", optional = true }
+tenacity = { version = "^8.0.1", optional = true }
+pyzmq = { version = ">=22.3.0", optional = true }
 
 [tool.poetry.extras]
 all = ["confluent-kafka", "PyRSMQ", "hiredis", "tenacity", "pyzmq"]
 rsmq = ["PyRSMQ", "hiredis", "tenacity"]
 kafka = ["confluent-kafka"]
 zmq = ["pyzmq"]
 
 [tool.poetry.dev-dependencies]
 flake8 = "^6.0.0"
 mypy = "^1.0.0"
-# TODo(@damon): Remove coverage
-coverage = "^6.0"
 black = "^22.3.0"
 pytest = "^7.2"
 isort = "^5.9.3"
 debugpy = "^1.5.0"
 pytest-cov = "^3.0.0"
 types-requests = "^2.25.11"
 types-pytz = "^2021.3.0"
@@ -66,36 +62,30 @@
 profile = "black"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.coverage]
-run.omit = [
-    "./example/*",
-    "./example.py",
-    "./tests/*"
-    ]
+run.omit = ["./example/*", "./example.py", "./tests/*"]
 report.show_missing = true
 report.fail_under = 98
 
 [tool.black]
 line-length = 120
 target-version = ['py310', 'py39', 'py38']
 
 [tool.pytest.ini_options]
 log_cli = true
 log_cli_level = "INFO"
 
-markers = [
-    "integration: mark a test as an integration test"
-]
+markers = ["integration: mark a test as an integration test"]
 
 [tool.pylint.master]
-ignore="example"
+ignore = "example"
 
 [tool.pylint.messages_control]
 disable = "all"
 enable = [
     "abstract-method",
     "arguments-differ",
     "differing-param-doc",
@@ -112,9 +102,9 @@
     "protected-access",
     "redundant-returns-doc",
     "redundant-yields-doc",
     "signature-differs",
     "super-init-not-called",
     "unused-argument",
     "unused-variable",
-    "useless-object-inheritance"
+    "useless-object-inheritance",
 ]
```

### Comparing `py_volley-1.1.1/volley/concurrency.py` & `py_volley-1.1.2/volley/concurrency.py`

 * *Files identical despite different names*

### Comparing `py_volley-1.1.1/volley/config.py` & `py_volley-1.1.2/volley/config.py`

 * *Files identical despite different names*

### Comparing `py_volley-1.1.1/volley/connectors/base.py` & `py_volley-1.1.2/volley/connectors/base.py`

 * *Files identical despite different names*

### Comparing `py_volley-1.1.1/volley/connectors/confluent.py` & `py_volley-1.1.2/volley/connectors/confluent.py`

 * *Files identical despite different names*

### Comparing `py_volley-1.1.1/volley/connectors/rsmq.py` & `py_volley-1.1.2/volley/connectors/rsmq.py`

 * *Files identical despite different names*

### Comparing `py_volley-1.1.1/volley/connectors/zmq.py` & `py_volley-1.1.2/volley/connectors/zmq.py`

 * *Files identical despite different names*

### Comparing `py_volley-1.1.1/volley/engine.py` & `py_volley-1.1.2/volley/engine.py`

 * *Files identical despite different names*

### Comparing `py_volley-1.1.1/volley/global.yml` & `py_volley-1.1.2/volley/global.yml`

 * *Files identical despite different names*

### Comparing `py_volley-1.1.1/volley/metrics.py` & `py_volley-1.1.2/volley/metrics.py`

 * *Files identical despite different names*

### Comparing `py_volley-1.1.1/volley/models/base.py` & `py_volley-1.1.2/volley/models/base.py`

 * *Files identical despite different names*

### Comparing `py_volley-1.1.1/volley/models/pydantic_model.py` & `py_volley-1.1.2/volley/models/pydantic_model.py`

 * *Files identical despite different names*

### Comparing `py_volley-1.1.1/volley/profiles.py` & `py_volley-1.1.2/volley/profiles.py`

 * *Files identical despite different names*

### Comparing `py_volley-1.1.1/volley/queues.py` & `py_volley-1.1.2/volley/queues.py`

 * *Files identical despite different names*

### Comparing `py_volley-1.1.1/volley/serializers/base.py` & `py_volley-1.1.2/volley/serializers/base.py`

 * *Files identical despite different names*

### Comparing `py_volley-1.1.1/volley/transport.py` & `py_volley-1.1.2/volley/transport.py`

 * *Files identical despite different names*

### Comparing `py_volley-1.1.1/volley/util.py` & `py_volley-1.1.2/volley/util.py`

 * *Files identical despite different names*

### Comparing `py_volley-1.1.1/PKG-INFO` & `py_volley-1.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py-volley
-Version: 1.1.1
+Version: 1.1.2
 Summary: Pluggable message queueing for Python
 Author: ask-machine-learning
 Author-email: shipt@shipt.com
 Requires-Python: >=3.8.1,<4.0.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```


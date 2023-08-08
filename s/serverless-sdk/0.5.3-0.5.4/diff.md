# Comparing `tmp/serverless-sdk-0.5.3.tar.gz` & `tmp/serverless-sdk-0.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/console/console/python/packages/sdk/dist/.tmp-icisettl/serverless-sdk-0.5.3.tar", last modified: Mon Jul 31 21:12:52 2023, max compression
+gzip compressed data, was "/home/runner/work/console/console/python/packages/sdk/dist/.tmp-nnf1xi4h/serverless-sdk-0.5.4.tar", last modified: Tue Aug  8 14:27:23 2023, max compression
```

## Comparing `serverless-sdk-0.5.3.tar` & `serverless-sdk-0.5.4.tar`

### file list

```diff
@@ -1,47 +1,47 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 21:12:52.000000 serverless-sdk-0.5.3/
--rw-r--r--   0 runner    (1001) docker     (123)     3186 2023-07-31 21:12:52.000000 serverless-sdk-0.5.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2355 2023-07-31 21:12:27.000000 serverless-sdk-0.5.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1766 2023-07-31 21:12:27.000000 serverless-sdk-0.5.3/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 21:12:52.000000 serverless-sdk-0.5.3/serverless_sdk/
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-07-31 21:12:27.000000 serverless-sdk-0.5.3/serverless_sdk/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 21:12:52.000000 serverless-sdk-0.5.3/serverless_sdk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3186 2023-07-31 21:12:52.000000 serverless-sdk-0.5.3/serverless_sdk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1053 2023-07-31 21:12:52.000000 serverless-sdk-0.5.3/serverless_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-31 21:12:52.000000 serverless-sdk-0.5.3/serverless_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      266 2023-07-31 21:12:52.000000 serverless-sdk-0.5.3/serverless_sdk.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-31 21:12:52.000000 serverless-sdk-0.5.3/serverless_sdk.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-31 21:12:52.000000 serverless-sdk-0.5.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 21:12:52.000000 serverless-sdk-0.5.3/sls_sdk/
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-31 21:12:27.000000 serverless-sdk-0.5.3/sls_sdk/VERSION
--rw-r--r--   0 runner    (1001) docker     (123)     5691 2023-07-31 21:12:27.000000 serverless-sdk-0.5.3/sls_sdk/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      684 2023-07-31 21:12:27.000000 serverless-sdk-0.5.3/sls_sdk/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      770 2023-07-31 21:12:27.000000 serverless-sdk-0.5.3/sls_sdk/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 21:12:52.000000 serverless-sdk-0.5.3/sls_sdk/lib/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 21:12:27.000000 serverless-sdk-0.5.3/sls_sdk/lib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2773 2023-07-31 21:12:27.000000 serverless-sdk-0.5.3/sls_sdk/lib/captured_event.py
--rw-r--r--   0 runner    (1001) docker     (123)      814 2023-07-31 21:12:27.000000 serverless-sdk-0.5.3/sls_sdk/lib/emitter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1525 2023-07-31 21:12:27.000000 serverless-sdk-0.5.3/sls_sdk/lib/error.py
--rw-r--r--   0 runner    (1001) docker     (123)     2072 2023-07-31 21:12:27.000000 serverless-sdk-0.5.3/sls_sdk/lib/error_captured_event.py
--rw-r--r--   0 runner    (1001) docker     (123)      506 2023-07-31 21:12:27.000000 serverless-sdk-0.5.3/sls_sdk/lib/id.py
--rw-r--r--   0 runner    (1001) docker     (123)     1591 2023-07-31 21:12:27.000000 serverless-sdk-0.5.3/sls_sdk/lib/imports.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 21:12:52.000000 serverless-sdk-0.5.3/sls_sdk/lib/instrumentation/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 21:12:27.000000 serverless-sdk-0.5.3/sls_sdk/lib/instrumentation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5640 2023-07-31 21:12:27.000000 serverless-sdk-0.5.3/sls_sdk/lib/instrumentation/flask.py
--rw-r--r--   0 runner    (1001) docker     (123)    18061 2023-07-31 21:12:27.000000 serverless-sdk-0.5.3/sls_sdk/lib/instrumentation/http.py
--rw-r--r--   0 runner    (1001) docker     (123)     2102 2023-07-31 21:12:27.000000 serverless-sdk-0.5.3/sls_sdk/lib/instrumentation/import_hook.py
--rw-r--r--   0 runner    (1001) docker     (123)     2475 2023-07-31 21:12:27.000000 serverless-sdk-0.5.3/sls_sdk/lib/instrumentation/logging.py
--rw-r--r--   0 runner    (1001) docker     (123)     1095 2023-07-31 21:12:27.000000 serverless-sdk-0.5.3/sls_sdk/lib/instrumentation/wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     1165 2023-07-31 21:12:27.000000 serverless-sdk-0.5.3/sls_sdk/lib/name.py
--rw-r--r--   0 runner    (1001) docker     (123)      538 2023-07-31 21:12:27.000000 serverless-sdk-0.5.3/sls_sdk/lib/notice.py
--rw-r--r--   0 runner    (1001) docker     (123)      822 2023-07-31 21:12:27.000000 serverless-sdk-0.5.3/sls_sdk/lib/stack_trace_string.py
--rw-r--r--   0 runner    (1001) docker     (123)      244 2023-07-31 21:12:27.000000 serverless-sdk-0.5.3/sls_sdk/lib/tag_value.py
--rw-r--r--   0 runner    (1001) docker     (123)     5922 2023-07-31 21:12:27.000000 serverless-sdk-0.5.3/sls_sdk/lib/tags.py
--rw-r--r--   0 runner    (1001) docker     (123)      351 2023-07-31 21:12:27.000000 serverless-sdk-0.5.3/sls_sdk/lib/timing.py
--rw-r--r--   0 runner    (1001) docker     (123)     9597 2023-07-31 21:12:27.000000 serverless-sdk-0.5.3/sls_sdk/lib/trace.py
--rw-r--r--   0 runner    (1001) docker     (123)      633 2023-07-31 21:12:27.000000 serverless-sdk-0.5.3/sls_sdk/lib/warning.py
--rw-r--r--   0 runner    (1001) docker     (123)     1568 2023-07-31 21:12:27.000000 serverless-sdk-0.5.3/sls_sdk/lib/warning_captured_event.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 21:12:27.000000 serverless-sdk-0.5.3/sls_sdk/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 21:12:52.000000 serverless-sdk-0.5.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     6982 2023-07-31 21:12:27.000000 serverless-sdk-0.5.3/tests/test_sdk.py
--rw-r--r--   0 runner    (1001) docker     (123)      247 2023-07-31 21:12:27.000000 serverless-sdk-0.5.3/tests/test_sdk_alias.py
--rw-r--r--   0 runner    (1001) docker     (123)    16668 2023-07-31 21:12:27.000000 serverless-sdk-0.5.3/tests/test_thread_safety.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 14:27:23.000000 serverless-sdk-0.5.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     3186 2023-08-08 14:27:23.000000 serverless-sdk-0.5.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2355 2023-08-08 14:27:05.000000 serverless-sdk-0.5.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1766 2023-08-08 14:27:05.000000 serverless-sdk-0.5.4/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 14:27:23.000000 serverless-sdk-0.5.4/serverless_sdk/
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-08-08 14:27:05.000000 serverless-sdk-0.5.4/serverless_sdk/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 14:27:23.000000 serverless-sdk-0.5.4/serverless_sdk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3186 2023-08-08 14:27:23.000000 serverless-sdk-0.5.4/serverless_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1053 2023-08-08 14:27:23.000000 serverless-sdk-0.5.4/serverless_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 14:27:23.000000 serverless-sdk-0.5.4/serverless_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      266 2023-08-08 14:27:23.000000 serverless-sdk-0.5.4/serverless_sdk.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-08-08 14:27:23.000000 serverless-sdk-0.5.4/serverless_sdk.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-08 14:27:23.000000 serverless-sdk-0.5.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 14:27:23.000000 serverless-sdk-0.5.4/sls_sdk/
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-08-08 14:27:05.000000 serverless-sdk-0.5.4/sls_sdk/VERSION
+-rw-r--r--   0 runner    (1001) docker     (123)     5831 2023-08-08 14:27:05.000000 serverless-sdk-0.5.4/sls_sdk/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      684 2023-08-08 14:27:05.000000 serverless-sdk-0.5.4/sls_sdk/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      770 2023-08-08 14:27:05.000000 serverless-sdk-0.5.4/sls_sdk/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 14:27:23.000000 serverless-sdk-0.5.4/sls_sdk/lib/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 14:27:05.000000 serverless-sdk-0.5.4/sls_sdk/lib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2773 2023-08-08 14:27:05.000000 serverless-sdk-0.5.4/sls_sdk/lib/captured_event.py
+-rw-r--r--   0 runner    (1001) docker     (123)      814 2023-08-08 14:27:05.000000 serverless-sdk-0.5.4/sls_sdk/lib/emitter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1525 2023-08-08 14:27:05.000000 serverless-sdk-0.5.4/sls_sdk/lib/error.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2072 2023-08-08 14:27:05.000000 serverless-sdk-0.5.4/sls_sdk/lib/error_captured_event.py
+-rw-r--r--   0 runner    (1001) docker     (123)      506 2023-08-08 14:27:05.000000 serverless-sdk-0.5.4/sls_sdk/lib/id.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1591 2023-08-08 14:27:05.000000 serverless-sdk-0.5.4/sls_sdk/lib/imports.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 14:27:23.000000 serverless-sdk-0.5.4/sls_sdk/lib/instrumentation/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 14:27:05.000000 serverless-sdk-0.5.4/sls_sdk/lib/instrumentation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5696 2023-08-08 14:27:05.000000 serverless-sdk-0.5.4/sls_sdk/lib/instrumentation/flask.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18061 2023-08-08 14:27:05.000000 serverless-sdk-0.5.4/sls_sdk/lib/instrumentation/http.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2102 2023-08-08 14:27:05.000000 serverless-sdk-0.5.4/sls_sdk/lib/instrumentation/import_hook.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2475 2023-08-08 14:27:05.000000 serverless-sdk-0.5.4/sls_sdk/lib/instrumentation/logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1095 2023-08-08 14:27:05.000000 serverless-sdk-0.5.4/sls_sdk/lib/instrumentation/wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1165 2023-08-08 14:27:05.000000 serverless-sdk-0.5.4/sls_sdk/lib/name.py
+-rw-r--r--   0 runner    (1001) docker     (123)      538 2023-08-08 14:27:05.000000 serverless-sdk-0.5.4/sls_sdk/lib/notice.py
+-rw-r--r--   0 runner    (1001) docker     (123)      822 2023-08-08 14:27:05.000000 serverless-sdk-0.5.4/sls_sdk/lib/stack_trace_string.py
+-rw-r--r--   0 runner    (1001) docker     (123)      244 2023-08-08 14:27:05.000000 serverless-sdk-0.5.4/sls_sdk/lib/tag_value.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5922 2023-08-08 14:27:05.000000 serverless-sdk-0.5.4/sls_sdk/lib/tags.py
+-rw-r--r--   0 runner    (1001) docker     (123)      351 2023-08-08 14:27:05.000000 serverless-sdk-0.5.4/sls_sdk/lib/timing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9597 2023-08-08 14:27:05.000000 serverless-sdk-0.5.4/sls_sdk/lib/trace.py
+-rw-r--r--   0 runner    (1001) docker     (123)      633 2023-08-08 14:27:05.000000 serverless-sdk-0.5.4/sls_sdk/lib/warning.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1568 2023-08-08 14:27:05.000000 serverless-sdk-0.5.4/sls_sdk/lib/warning_captured_event.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 14:27:05.000000 serverless-sdk-0.5.4/sls_sdk/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 14:27:23.000000 serverless-sdk-0.5.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     6982 2023-08-08 14:27:05.000000 serverless-sdk-0.5.4/tests/test_sdk.py
+-rw-r--r--   0 runner    (1001) docker     (123)      247 2023-08-08 14:27:05.000000 serverless-sdk-0.5.4/tests/test_sdk_alias.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16668 2023-08-08 14:27:05.000000 serverless-sdk-0.5.4/tests/test_thread_safety.py
```

### Comparing `serverless-sdk-0.5.3/PKG-INFO` & `serverless-sdk-0.5.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: serverless-sdk
-Version: 0.5.3
+Version: 0.5.4
 Summary: Serverless SDK for Python
 Author: serverlessinc
 Project-URL: changelog, https://github.com/serverless/console/blob/main/python/packages/sdk/CHANGELOG.md
 Project-URL: documentation, https://github.com/serverless/console/tree/main/python/packages/sdk
 Project-URL: homepage, https://www.serverless.com/console
 Project-URL: repository, https://github.com/serverless/console
 Classifier: Programming Language :: Python :: 3 :: Only
```

### Comparing `serverless-sdk-0.5.3/README.md` & `serverless-sdk-0.5.4/README.md`

 * *Files identical despite different names*

### Comparing `serverless-sdk-0.5.3/pyproject.toml` & `serverless-sdk-0.5.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `serverless-sdk-0.5.3/serverless_sdk.egg-info/PKG-INFO` & `serverless-sdk-0.5.4/serverless_sdk.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: serverless-sdk
-Version: 0.5.3
+Version: 0.5.4
 Summary: Serverless SDK for Python
 Author: serverlessinc
 Project-URL: changelog, https://github.com/serverless/console/blob/main/python/packages/sdk/CHANGELOG.md
 Project-URL: documentation, https://github.com/serverless/console/tree/main/python/packages/sdk
 Project-URL: homepage, https://www.serverless.com/console
 Project-URL: repository, https://github.com/serverless/console
 Classifier: Programming Language :: Python :: 3 :: Only
```

### Comparing `serverless-sdk-0.5.3/serverless_sdk.egg-info/SOURCES.txt` & `serverless-sdk-0.5.4/serverless_sdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `serverless-sdk-0.5.3/sls_sdk/__init__.py` & `serverless-sdk-0.5.4/sls_sdk/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -83,14 +83,15 @@
     org_id: Optional[str] = None
     _settings: ServerlessSdkSettings
     _custom_tags: Tags
     _is_initialized: bool
     _is_debug_mode: bool
     _is_dev_mode: bool
     _maximum_body_byte_length: int
+    _user_defined_endpoint: Optional[str] = None
 
     def __init__(self):
         self._is_initialized = False
         self.trace_spans = TraceSpans()
         self._event_emitter = event_emitter
         self._custom_tags = Tags()
 
@@ -171,9 +172,12 @@
 
     def set_tag(self, name: str, value: ValidTags):
         try:
             self._custom_tags._set(name, value)
         except Exception as ex:
             report_error(ex, type="USER")
 
+    def set_endpoint(self, endpoint: str):
+        self._user_defined_endpoint = endpoint
+
 
 serverlessSdk: Final[ServerlessSdk] = ServerlessSdk()
```

### Comparing `serverless-sdk-0.5.3/sls_sdk/base.py` & `serverless-sdk-0.5.4/sls_sdk/base.py`

 * *Files identical despite different names*

### Comparing `serverless-sdk-0.5.3/sls_sdk/exceptions.py` & `serverless-sdk-0.5.4/sls_sdk/exceptions.py`

 * *Files identical despite different names*

### Comparing `serverless-sdk-0.5.3/sls_sdk/lib/captured_event.py` & `serverless-sdk-0.5.4/sls_sdk/lib/captured_event.py`

 * *Files identical despite different names*

### Comparing `serverless-sdk-0.5.3/sls_sdk/lib/emitter.py` & `serverless-sdk-0.5.4/sls_sdk/lib/emitter.py`

 * *Files identical despite different names*

### Comparing `serverless-sdk-0.5.3/sls_sdk/lib/error.py` & `serverless-sdk-0.5.4/sls_sdk/lib/error.py`

 * *Files identical despite different names*

### Comparing `serverless-sdk-0.5.3/sls_sdk/lib/error_captured_event.py` & `serverless-sdk-0.5.4/sls_sdk/lib/error_captured_event.py`

 * *Files identical despite different names*

### Comparing `serverless-sdk-0.5.3/sls_sdk/lib/imports.py` & `serverless-sdk-0.5.4/sls_sdk/lib/imports.py`

 * *Files identical despite different names*

### Comparing `serverless-sdk-0.5.3/sls_sdk/lib/instrumentation/flask.py` & `serverless-sdk-0.5.4/sls_sdk/lib/instrumentation/flask.py`

 * *Files 7% similar despite different names*

```diff
@@ -81,19 +81,20 @@
         except Exception as ex:
             report_error(ex)
 
     def _handle_request_started(self, sender, **extra):
         if not self._flask.request.endpoint:
             return
         try:
-            if self._flask.request.path:
+            endpoint = serverlessSdk._user_defined_endpoint or self._flask.request.path
+            if endpoint:
                 del serverlessSdk.trace_spans.root.tags["aws.lambda.http_router.path"]
                 serverlessSdk.trace_spans.root.tags[
                     "aws.lambda.http_router.path"
-                ] = self._flask.request.path
+                ] = endpoint
             span_name = ".".join(
                 [
                     "flask",
                     "route",
                     self.sanitize_span_name(self._flask.request.method),
                     self.sanitize_span_name(self._flask.request.endpoint),
                 ]
```

### Comparing `serverless-sdk-0.5.3/sls_sdk/lib/instrumentation/http.py` & `serverless-sdk-0.5.4/sls_sdk/lib/instrumentation/http.py`

 * *Files identical despite different names*

### Comparing `serverless-sdk-0.5.3/sls_sdk/lib/instrumentation/import_hook.py` & `serverless-sdk-0.5.4/sls_sdk/lib/instrumentation/import_hook.py`

 * *Files identical despite different names*

### Comparing `serverless-sdk-0.5.3/sls_sdk/lib/instrumentation/logging.py` & `serverless-sdk-0.5.4/sls_sdk/lib/instrumentation/logging.py`

 * *Files identical despite different names*

### Comparing `serverless-sdk-0.5.3/sls_sdk/lib/instrumentation/wrapper.py` & `serverless-sdk-0.5.4/sls_sdk/lib/instrumentation/wrapper.py`

 * *Files identical despite different names*

### Comparing `serverless-sdk-0.5.3/sls_sdk/lib/name.py` & `serverless-sdk-0.5.4/sls_sdk/lib/name.py`

 * *Files identical despite different names*

### Comparing `serverless-sdk-0.5.3/sls_sdk/lib/notice.py` & `serverless-sdk-0.5.4/sls_sdk/lib/notice.py`

 * *Files identical despite different names*

### Comparing `serverless-sdk-0.5.3/sls_sdk/lib/stack_trace_string.py` & `serverless-sdk-0.5.4/sls_sdk/lib/stack_trace_string.py`

 * *Files identical despite different names*

### Comparing `serverless-sdk-0.5.3/sls_sdk/lib/tags.py` & `serverless-sdk-0.5.4/sls_sdk/lib/tags.py`

 * *Files identical despite different names*

### Comparing `serverless-sdk-0.5.3/sls_sdk/lib/trace.py` & `serverless-sdk-0.5.4/sls_sdk/lib/trace.py`

 * *Files identical despite different names*

### Comparing `serverless-sdk-0.5.3/sls_sdk/lib/warning.py` & `serverless-sdk-0.5.4/sls_sdk/lib/warning.py`

 * *Files identical despite different names*

### Comparing `serverless-sdk-0.5.3/sls_sdk/lib/warning_captured_event.py` & `serverless-sdk-0.5.4/sls_sdk/lib/warning_captured_event.py`

 * *Files identical despite different names*

### Comparing `serverless-sdk-0.5.3/tests/test_sdk.py` & `serverless-sdk-0.5.4/tests/test_sdk.py`

 * *Files identical despite different names*

### Comparing `serverless-sdk-0.5.3/tests/test_thread_safety.py` & `serverless-sdk-0.5.4/tests/test_thread_safety.py`

 * *Files identical despite different names*


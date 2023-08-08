# Comparing `tmp/traceloop_sdk-0.0.6.tar.gz` & `tmp/traceloop_sdk-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "traceloop_sdk-0.0.6.tar", max compression
+gzip compressed data, was "traceloop_sdk-0.0.8.tar", max compression
```

## Comparing `traceloop_sdk-0.0.6.tar` & `traceloop_sdk-0.0.8.tar`

### file list

```diff
@@ -1,18 +1,17 @@
--rw-r--r--   0        0        0        0 2023-08-02 09:25:16.062473 traceloop_sdk-0.0.6/README.md
--rw-r--r--   0        0        0      562 2023-08-02 14:40:54.585995 traceloop_sdk-0.0.6/pyproject.toml
--rw-r--r--   0        0        0        0 2023-08-02 13:35:06.247470 traceloop_sdk-0.0.6/traceloop/__init__.py
--rw-r--r--   0        0        0        0 2023-08-01 13:29:56.846025 traceloop_sdk-0.0.6/traceloop/agent/__init__.py
--rw-r--r--   0        0        0      238 2023-08-01 13:49:46.129127 traceloop_sdk-0.0.6/traceloop/agent/decorator.py
--rw-r--r--   0        0        0        0 2023-08-01 13:30:02.778279 traceloop_sdk-0.0.6/traceloop/agent/tool/__init__.py
--rw-r--r--   0        0        0      236 2023-08-01 14:31:03.279362 traceloop_sdk-0.0.6/traceloop/agent/tool/decorator.py
--rw-r--r--   0        0        0        0 2023-08-02 13:18:36.291777 traceloop_sdk-0.0.6/traceloop/instrumentation/__init__.py
--rw-r--r--   0        0        0    11253 2023-08-02 13:37:44.238046 traceloop_sdk-0.0.6/traceloop/instrumentation/openai/__init__.py
--rw-r--r--   0        0        0       37 2023-08-02 13:35:46.090364 traceloop_sdk-0.0.6/traceloop/instrumentation/openai/package.py
--rw-r--r--   0        0        0      239 2023-08-01 13:41:08.608117 traceloop_sdk-0.0.6/traceloop/semconv/__init__.py
--rw-r--r--   0        0        0        0 2023-07-30 15:13:41.585793 traceloop_sdk-0.0.6/traceloop/task/__init__.py
--rw-r--r--   0        0        0      729 2023-08-01 14:01:15.919064 traceloop_sdk-0.0.6/traceloop/task/decorator.py
--rw-r--r--   0        0        0        0 2023-07-30 15:42:25.834193 traceloop_sdk-0.0.6/traceloop/tracing/__init__.py
--rw-r--r--   0        0        0     1532 2023-08-02 14:39:48.034972 traceloop_sdk-0.0.6/traceloop/tracing/tracer.py
--rw-r--r--   0        0        0        0 2023-08-01 09:57:19.484179 traceloop_sdk-0.0.6/traceloop/workflow/__init__.py
--rw-r--r--   0        0        0      644 2023-08-01 14:01:15.916149 traceloop_sdk-0.0.6/traceloop/workflow/decorator.py
--rw-r--r--   0        0        0      676 1970-01-01 00:00:00.000000 traceloop_sdk-0.0.6/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-08-02 09:25:16.062473 traceloop_sdk-0.0.8/README.md
+-rw-r--r--   0        0        0      593 2023-08-08 06:39:38.563289 traceloop_sdk-0.0.8/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-08-02 13:35:06.247470 traceloop_sdk-0.0.8/traceloop/__init__.py
+-rw-r--r--   0        0        0        0 2023-08-01 13:29:56.846025 traceloop_sdk-0.0.8/traceloop/agent/__init__.py
+-rw-r--r--   0        0        0      238 2023-08-01 13:49:46.129127 traceloop_sdk-0.0.8/traceloop/agent/decorator.py
+-rw-r--r--   0        0        0        0 2023-08-01 13:30:02.778279 traceloop_sdk-0.0.8/traceloop/agent/tool/__init__.py
+-rw-r--r--   0        0        0      236 2023-08-01 14:31:03.279362 traceloop_sdk-0.0.8/traceloop/agent/tool/decorator.py
+-rw-r--r--   0        0        0        0 2023-08-07 14:49:43.761468 traceloop_sdk-0.0.8/traceloop/instrumentation/__init__.py
+-rw-r--r--   0        0        0    11224 2023-08-08 06:38:40.017747 traceloop_sdk-0.0.8/traceloop/instrumentation/openai/__init__.py
+-rw-r--r--   0        0        0      239 2023-08-01 13:41:08.608117 traceloop_sdk-0.0.8/traceloop/semconv/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-30 15:13:41.585792 traceloop_sdk-0.0.8/traceloop/task/__init__.py
+-rw-r--r--   0        0        0      729 2023-08-01 14:01:15.919064 traceloop_sdk-0.0.8/traceloop/task/decorator.py
+-rw-r--r--   0        0        0        0 2023-07-30 15:42:25.834193 traceloop_sdk-0.0.8/traceloop/tracing/__init__.py
+-rw-r--r--   0        0        0     1574 2023-08-07 15:40:53.475221 traceloop_sdk-0.0.8/traceloop/tracing/tracer.py
+-rw-r--r--   0        0        0        0 2023-08-01 09:57:19.484179 traceloop_sdk-0.0.8/traceloop/workflow/__init__.py
+-rw-r--r--   0        0        0      644 2023-08-01 14:01:15.916150 traceloop_sdk-0.0.8/traceloop/workflow/decorator.py
+-rw-r--r--   0        0        0      703 1970-01-01 00:00:00.000000 traceloop_sdk-0.0.8/PKG-INFO
```

### Comparing `traceloop_sdk-0.0.6/traceloop/instrumentation/openai/__init__.py` & `traceloop_sdk-0.0.8/traceloop/instrumentation/openai/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,30 +9,32 @@
 from opentelemetry.trace.status import Status, StatusCode
 
 from opentelemetry.instrumentation.instrumentor import BaseInstrumentor
 from opentelemetry.instrumentation.utils import (
     _SUPPRESS_INSTRUMENTATION_KEY,
     unwrap,
 )
-from traceloop.instrumentation.openai.package import _instruments
 
 logger = logging.getLogger(__name__)
 
+_instruments = ("openai ~= 0.27.8",)
+__version__ = "0.1.0"
+
 TO_WRAP = [
     {
         "object": "ChatCompletion",
         "method": "create",
         "span_name": "openai.chat",
         "default_inputs": {
             "temperature": 1.0,
             "top_p": 1.0,
             "n": 1,
             "stream": False,
             "stop": "",
-            "max_tokens": float('inf'),
+            "max_tokens": -1.0,
             "presence_penalty": 0.0,
             "frequency_penalty": 0.0,
             "logit_bias": "",
             "user": "",
         }
     },
     {
@@ -44,15 +46,15 @@
             "temperature": 1.0,
             "top_p": 1.0,
             "n": 1,
             "stream": False,
             "logprobs": -1,
             "echo": False,
             "stop": "",
-            "max_tokens": float('inf'),
+            "max_tokens": -1.0,
             "presence_penalty": 0.0,
             "frequency_penalty": 0.0,
             "best_of": 1,
             "logit_bias": "",
             "user": "",
         }
     },
@@ -150,15 +152,15 @@
         return str(value)
     return value
 
 
 def _set_attributes(span, name, attributes, nestings=[]):
     """
     For every nested field, set its fields as attributes.
-    Then set the remianing non-nested fields.
+    Then set the remaining non-nested fields.
     """
     attr_copy = attributes.copy()  # don't change shape of inputs!
     for nesting in nestings:
         nested = attr_copy.pop(nesting, None)
         if nested:
             for key, value in nested.items():
                 span.set_attribute(
@@ -196,14 +198,16 @@
     Unpacks 'message' input fields to separate attributes.
     For embeddings, captures count of 'input' values.
     """
 
     params = to_wrap.get("default_inputs")
     params.update(kwargs)
 
+    print(f"kwargs: {kwargs}")
+
     # "input" fields can be very large, so we handle them specially
     # depending on which api object they belong to.
     _input = params.pop("input", None)
     if _input:
         if name in ["openai.embedding"]:
             # input values for Embedding objects can be too
             # long so for that we only capture len(input)
@@ -363,16 +367,15 @@
     """An instrumenter for OpenAI's client library."""
 
     def instrumentation_dependencies(self) -> Collection[str]:
         return _instruments
 
     def _instrument(self, **kwargs):
         tracer_provider = kwargs.get("tracer_provider")
-        # TODO: dynamic version extraction
-        tracer = get_tracer(__name__, "0.0.3", tracer_provider)
+        tracer = get_tracer(__name__, __version__, tracer_provider)
         for to_wrap in TO_WRAP:
             wrap_object = to_wrap.get("object")
             wrap_method = to_wrap.get("method")
             wrap_function_wrapper(
                 "openai",
                 f"{wrap_object}.{wrap_method}",
                 _wrap(tracer, to_wrap)
```

### Comparing `traceloop_sdk-0.0.6/traceloop/task/decorator.py` & `traceloop_sdk-0.0.8/traceloop/task/decorator.py`

 * *Files identical despite different names*

### Comparing `traceloop_sdk-0.0.6/traceloop/tracing/tracer.py` & `traceloop_sdk-0.0.8/traceloop/tracing/tracer.py`

 * *Files 7% similar despite different names*

```diff
@@ -28,17 +28,19 @@
             }
         )
         processor = BatchSpanProcessor(exporter)
         provider.add_span_processor(processor)
         trace.set_tracer_provider(provider)
         Tracer.__instance = trace.get_tracer(TRACER_NAME)
 
-        # os.environ["OTEL_PYTHON_REQUESTS_EXCLUDED_URLS"] = "/openai/"
+        os.environ["OTEL_PYTHON_REQUESTS_EXCLUDED_URLS"] = "/openai/"
 
         OpenAIInstrumentor().instrument()
         RequestsInstrumentor().instrument(excluded_urls="^https://api.openai.com")
+        # MySQLInstrumentor().instrument()
+
 
     @staticmethod
     def instance():
         if Tracer.__instance is None:
             raise Exception("Tracer is not initialized")
         return Tracer.__instance
```

### Comparing `traceloop_sdk-0.0.6/traceloop/workflow/decorator.py` & `traceloop_sdk-0.0.8/traceloop/workflow/decorator.py`

 * *Files identical despite different names*

### Comparing `traceloop_sdk-0.0.6/PKG-INFO` & `traceloop_sdk-0.0.8/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: traceloop-sdk
-Version: 0.0.6
+Version: 0.0.8
 Summary: 
 Author: Gal Kleinman
 Author-email: gal@traceloop.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: openai (>=0.27.8,<0.28.0)
 Requires-Dist: opentelemetry-api (>=1.19.0,<2.0.0)
 Requires-Dist: opentelemetry-exporter-otlp-proto-http (>=1.19.0,<2.0.0)
+Requires-Dist: opentelemetry-instrumentation-mysql (>=0.40b0,<0.41)
 Requires-Dist: opentelemetry-instrumentation-requests (>=0.40b0,<0.41)
 Requires-Dist: opentelemetry-sdk (>=1.19.0,<2.0.0)
 Description-Content-Type: text/markdown
```


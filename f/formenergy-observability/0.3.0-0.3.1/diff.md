# Comparing `tmp/formenergy-observability-0.3.0.tar.gz` & `tmp/formenergy-observability-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "formenergy-observability-0.3.0.tar", last modified: Tue May 23 15:56:12 2023, max compression
+gzip compressed data, was "formenergy-observability-0.3.1.tar", last modified: Tue Aug  8 13:32:08 2023, max compression
```

## Comparing `formenergy-observability-0.3.0.tar` & `formenergy-observability-0.3.1.tar`

### file list

```diff
@@ -1,28 +1,28 @@
--rw-r--r--   0        0        0      216 2023-05-23 15:55:45.341077 formenergy-observability-0.3.0/.gitignore
--rw-r--r--   0        0        0     2038 2023-01-04 16:51:23.731215 formenergy-observability-0.3.0/.pre-commit-config.yaml
--rw-r--r--   0        0        0      112 2023-01-04 16:51:23.731215 formenergy-observability-0.3.0/.pypirc
--rw-r--r--   0        0        0     1068 2023-01-04 16:09:14.490252 formenergy-observability-0.3.0/LICENSE
--rw-r--r--   0        0        0     3497 2023-05-23 15:52:50.668752 formenergy-observability-0.3.0/README.md
--rw-r--r--   0        0        0   177939 2023-01-04 16:31:04.090964 formenergy-observability-0.3.0/examples/basics-trace.png
--rwxr-xr-x   0        0        0     2570 2023-05-09 15:42:12.623237 formenergy-observability-0.3.0/examples/basics.py
--rw-r--r--   0        0        0   156173 2023-01-04 16:31:04.090964 formenergy-observability-0.3.0/examples/dagster_job.png
--rw-r--r--   0        0        0     2621 2023-05-17 18:05:51.312379 formenergy-observability-0.3.0/examples/dagster_job.py
--rwxr-xr-x   0        0        0     1793 2023-05-23 15:52:50.668752 formenergy-observability-0.3.0/examples/linked_traces.py
--rwxr-xr-x   0        0        0     2040 2023-01-05 18:21:06.057762 formenergy-observability-0.3.0/examples/multithread.py
--rw-r--r--   0        0        0      602 2023-05-23 15:52:50.668752 formenergy-observability-0.3.0/form_observability/__init__.py
--rw-r--r--   0        0        0       61 2023-01-05 16:42:09.235771 formenergy-observability-0.3.0/form_observability/conftest.py
--rw-r--r--   0        0        0     9394 2023-05-23 15:54:38.244987 formenergy-observability-0.3.0/form_observability/context_aware.py
--rw-r--r--   0        0        0      299 2023-01-05 16:42:09.239771 formenergy-observability-0.3.0/form_observability/dagster_otel/__init__.py
--rw-r--r--   0        0        0     8827 2023-04-11 14:25:49.316307 formenergy-observability-0.3.0/form_observability/dagster_otel/otel_ops.py
--rw-r--r--   0        0        0     2344 2023-05-23 15:52:50.668752 formenergy-observability-0.3.0/form_observability/dagster_otel/test_otel_op.py
--rw-r--r--   0        0        0      955 2023-01-05 16:42:09.239771 formenergy-observability-0.3.0/form_observability/dagster_otel/test_timing.py
--rw-r--r--   0        0        0      734 2023-01-05 16:42:09.239771 formenergy-observability-0.3.0/form_observability/dagster_otel/testing.py
--rw-r--r--   0        0        0     1291 2023-01-05 16:42:09.239771 formenergy-observability-0.3.0/form_observability/dagster_otel/timing.py
--rw-r--r--   0        0        0      582 2023-01-05 16:42:09.239771 formenergy-observability-0.3.0/form_observability/dagster_otel/util.py
--rw-r--r--   0        0        0     3701 2023-01-05 16:42:09.239771 formenergy-observability-0.3.0/form_observability/log.py
--rw-r--r--   0        0        0     1422 2023-01-05 16:42:09.239771 formenergy-observability-0.3.0/form_observability/otel_value.py
--rw-r--r--   0        0        0     3239 2023-01-05 16:42:09.239771 formenergy-observability-0.3.0/form_observability/pipeline_setup.py
--rw-r--r--   0        0        0     1572 2023-01-05 16:42:09.239771 formenergy-observability-0.3.0/form_observability/test_context_aware.py
--rw-r--r--   0        0        0      941 2023-01-05 16:42:09.239771 formenergy-observability-0.3.0/form_observability/testing.py
--rw-r--r--   0        0        0     1754 2023-04-11 14:23:41.900116 formenergy-observability-0.3.0/pyproject.toml
--rw-r--r--   0        0        0     4562 1970-01-01 00:00:00.000000 formenergy-observability-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0      216 2023-08-08 13:22:34.152295 formenergy-observability-0.3.1/.gitignore
+-rw-r--r--   0        0        0     2038 2023-01-04 16:51:23.731215 formenergy-observability-0.3.1/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      112 2023-01-04 16:51:23.731215 formenergy-observability-0.3.1/.pypirc
+-rw-r--r--   0        0        0     1068 2023-01-04 16:09:14.490252 formenergy-observability-0.3.1/LICENSE
+-rw-r--r--   0        0        0     3587 2023-08-08 13:25:22.980550 formenergy-observability-0.3.1/README.md
+-rw-r--r--   0        0        0   177939 2023-01-04 16:31:04.090964 formenergy-observability-0.3.1/examples/basics-trace.png
+-rwxr-xr-x   0        0        0     2613 2023-08-08 13:23:24.068366 formenergy-observability-0.3.1/examples/basics.py
+-rw-r--r--   0        0        0   156173 2023-01-04 16:31:04.090964 formenergy-observability-0.3.1/examples/dagster_job.png
+-rw-r--r--   0        0        0     2650 2023-08-08 13:23:24.068366 formenergy-observability-0.3.1/examples/dagster_job.py
+-rwxr-xr-x   0        0        0     1885 2023-08-08 13:23:24.068366 formenergy-observability-0.3.1/examples/linked_traces.py
+-rwxr-xr-x   0        0        0     2093 2023-08-08 13:23:24.068366 formenergy-observability-0.3.1/examples/multithread.py
+-rw-r--r--   0        0        0      602 2023-08-08 13:28:52.432913 formenergy-observability-0.3.1/form_observability/__init__.py
+-rw-r--r--   0        0        0       61 2023-01-05 16:42:09.235771 formenergy-observability-0.3.1/form_observability/conftest.py
+-rw-r--r--   0        0        0     9394 2023-08-08 13:22:34.148295 formenergy-observability-0.3.1/form_observability/context_aware.py
+-rw-r--r--   0        0        0      299 2023-01-05 16:42:09.239771 formenergy-observability-0.3.1/form_observability/dagster_otel/__init__.py
+-rw-r--r--   0        0        0     8827 2023-08-08 13:22:34.140295 formenergy-observability-0.3.1/form_observability/dagster_otel/otel_ops.py
+-rw-r--r--   0        0        0     2344 2023-08-08 13:22:34.144295 formenergy-observability-0.3.1/form_observability/dagster_otel/test_otel_op.py
+-rw-r--r--   0        0        0      955 2023-01-05 16:42:09.239771 formenergy-observability-0.3.1/form_observability/dagster_otel/test_timing.py
+-rw-r--r--   0        0        0      734 2023-01-05 16:42:09.239771 formenergy-observability-0.3.1/form_observability/dagster_otel/testing.py
+-rw-r--r--   0        0        0     1291 2023-01-05 16:42:09.239771 formenergy-observability-0.3.1/form_observability/dagster_otel/timing.py
+-rw-r--r--   0        0        0      582 2023-01-05 16:42:09.239771 formenergy-observability-0.3.1/form_observability/dagster_otel/util.py
+-rw-r--r--   0        0        0     3701 2023-01-05 16:42:09.239771 formenergy-observability-0.3.1/form_observability/log.py
+-rw-r--r--   0        0        0     1422 2023-01-05 16:42:09.239771 formenergy-observability-0.3.1/form_observability/otel_value.py
+-rw-r--r--   0        0        0     3294 2023-08-08 13:22:34.140295 formenergy-observability-0.3.1/form_observability/pipeline_setup.py
+-rw-r--r--   0        0        0     1572 2023-01-05 16:42:09.239771 formenergy-observability-0.3.1/form_observability/test_context_aware.py
+-rw-r--r--   0        0        0      941 2023-01-05 16:42:09.239771 formenergy-observability-0.3.1/form_observability/testing.py
+-rw-r--r--   0        0        0     1754 2023-08-08 13:22:34.140295 formenergy-observability-0.3.1/pyproject.toml
+-rw-r--r--   0        0        0     4652 1970-01-01 00:00:00.000000 formenergy-observability-0.3.1/PKG-INFO
```

### Comparing `formenergy-observability-0.3.0/.pre-commit-config.yaml` & `formenergy-observability-0.3.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `formenergy-observability-0.3.0/LICENSE` & `formenergy-observability-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `formenergy-observability-0.3.0/README.md` & `formenergy-observability-0.3.1/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -55,26 +55,27 @@
 ```
 
 ### Running the Examples
 
 Get an API key for uploading traces to your observability service (preferably in a development environment), set it in your environment, and run the examples. This should publish traces that you can then view.
 
 ```bash
-export OTEL_EXPORTER_OTLP_HEADERS="x-honeycomb-team=<API key>"
+export OTEL_EXPORTER_OTLP_HEADERS_JSON="{'x-honeycomb-team': '<API key>'}"
 export OTEL_EXPORTER_OTLP_ENDPOINT="your observability service, defaults to Honeycomb"
 python examples/basics.py
 dagster job execute --python-file examples/dagster_job.py
 ```
 
 ## License
 
 This library is provided under the MIT license, see [LICENSE](LICENSE).
 
 ## Release Notes
 
+*   0.3.1 Fix type used for `otlp_headers` to be a `dict`. Thanks @spenczar !
 *   0.3.0 Add `ContextAwareTracer.start_new_linked_trace`.
 *   0.2.0 Switch to `context.op_handle` and `materialization.metadata` as dict for Dagster 1.2.
 *   0.1.0 Initial external release, including `ContextAwareTracer`, `ctx`, and `@otel_op`.
 
 ## Development
 
 If you contribute, please ensure you and your employer accept [the license](LICENSE) for any of your contributions.
```

### Comparing `formenergy-observability-0.3.0/examples/basics-trace.png` & `formenergy-observability-0.3.1/examples/basics-trace.png`

 * *Files identical despite different names*

### Comparing `formenergy-observability-0.3.0/examples/basics.py` & `formenergy-observability-0.3.1/examples/basics.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 #!/usr/bin/env python3
 """Demonstrate a basic program that generates OpenTelemetry tracing."""
+import json
 import logging
 import os
 import random
 import time
 
 import opentelemetry
 
@@ -43,32 +44,32 @@
         except:
             _trace.add_event("failure")
             _log.exception(f"Error during processing of {my_data=}.")
             return False
 
 
 @_trace.traced  # Open a span for this function call. In this case it's the root span.
-def main():
+def basics_main():
     _log.info("Preparing to process tests.")
     num_errors = 0
     for my_data in ("one", "two", "three", "four", "five", "six"):
         with _trace.start_as_current_span("work", attributes={"my_data": my_data}):
             if _helper_that_sometimes_catches_exceptions_internally(my_data):
                 num_errors += 1
     opentelemetry.trace.get_current_span().set_attributes({"num_errors": num_errors})
     _log.info("Demo processing complete.")
 
 
 if __name__ == "__main__":
     logging.basicConfig(level=logging.INFO)
-    header_env = "OTEL_EXPORTER_OTLP_HEADERS"
+    header_env = "OTEL_EXPORTER_OTLP_HEADERS_JSON"
     endpoint_env = "OTEL_EXPORTER_OTLP_ENDPOINT"
     if header_env not in os.environ:
         _log.error(f"To upload traces, you must set {header_env}, see README.md.")
     # Set up a simple span exporter with no sampling, suitable for data pipelines.
     configure(
         "form_observability_example",  # demo dataset name
-        otlp_headers=os.environ.get(header_env),
+        otlp_headers=json.loads(os.environ.get(header_env)),
         otlp_endpoint=os.environ.get(endpoint_env, "https://api.honeycomb.io"),
     )
     _log.addHandler(OtelSpanEventHandler())  # Add span events for log messages.
-    main()
+    basics_main()
```

### Comparing `formenergy-observability-0.3.0/examples/dagster_job.png` & `formenergy-observability-0.3.1/examples/dagster_job.png`

 * *Files identical despite different names*

### Comparing `formenergy-observability-0.3.0/examples/dagster_job.py` & `formenergy-observability-0.3.1/examples/dagster_job.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """Dagster job with OpenTelemetry trace propagation.
 
 Run with:
     dagster job execute --python-file examples/dagster_job.py
 """
+import json
 import os
 
 from dagster import (
     Output,
     job,
     op,
     resource,
@@ -27,23 +28,23 @@
 
 _trace = ContextAwareTracer(__name__)
 
 
 @resource
 def configure_observability_resource(init_context):
     """This resource sets up the span exporter (before each op executes)."""
-    header_env = "OTEL_EXPORTER_OTLP_HEADERS"
+    header_env = "OTEL_EXPORTER_OTLP_HEADERS_JSON"
     endpoint_env = "OTEL_EXPORTER_OTLP_ENDPOINT"
     if header_env not in os.environ:
         init_context.log.error(
             f"To upload traces, you must set {header_env}, see README.md."
         )
     configure(
         "form_observability_example",
-        otlp_headers=os.environ.get(header_env),
+        otlp_headers=json.loads(os.environ.get(header_env)),
         otlp_endpoint=os.environ.get(endpoint_env, "https://api.honeycomb.io"),
     )
 
 
 @op(
     required_resource_keys={CONFIGURE_OBSERVABILITY_RESOURCE_KEY},
 )
```

### Comparing `formenergy-observability-0.3.0/examples/linked_traces.py` & `formenergy-observability-0.3.1/examples/linked_traces.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 #!/usr/bin/env python3
 """Demonstrate linked traces with context carried over."""
+import json
 import logging
 import os
 import random
 import time
 
 import opentelemetry
 from opentelemetry.trace import Link
@@ -23,15 +24,15 @@
 @_tracer.traced
 def _helper() -> None:
     """Do something in a child span of the linked trace."""
     _tracer.add_event("helped", attributes={"value": random.random()})
 
 
 @_tracer.traced  # Open a span for this function call. In this case it's the root span.
-def main():
+def linked_main():
     child_links = []
     for my_data in ("one", "two", "three"):
         with ctx.set({"my_data": my_data}):
             with _tracer.start_new_linked_trace("work") as child_ctx:
                 child_links.append(Link(child_ctx))
                 _helper()
     # Add forward links to the child traces.
@@ -39,18 +40,19 @@
     # https://github.com/open-telemetry/opentelemetry-specification/issues/454 .
     with _tracer.start_as_current_span("children", links=child_links):
         pass
 
 
 if __name__ == "__main__":
     logging.basicConfig(level=logging.INFO)
-    header_env = "OTEL_EXPORTER_OTLP_HEADERS"
+    header_env = "OTEL_EXPORTER_OTLP_HEADERS_JSON"
     endpoint_env = "OTEL_EXPORTER_OTLP_ENDPOINT"
     if header_env not in os.environ:
         _log.error(f"To upload traces, you must set {header_env}, see README.md.")
     # Set up a simple span exporter with no sampling, suitable for data pipelines.
     configure(
         "form_observability_example",  # demo dataset name
-        otlp_headers=os.environ.get(header_env),
+        otlp_headers=json.loads(os.environ.get(header_env)),
         otlp_endpoint=os.environ.get(endpoint_env, "https://api.honeycomb.io"),
     )
-    main()
+    linked_main()
+    _log.info("Linked traces example complete.")
```

### Comparing `formenergy-observability-0.3.0/examples/multithread.py` & `formenergy-observability-0.3.1/examples/multithread.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 #!/usr/bin/env python3
 """Demonstrate a multithreaded program which connects child traces to a parent.
 
 This shows how to set up simple trace context propagation.
 """
+import json
 import logging
 import os
 import random
 import threading
 import time
 
 import opentelemetry
@@ -34,33 +35,33 @@
     sleep_s = random.random() * 4
     with _trace.start_as_current_span(my_data, attributes={"sleep_s": sleep_s}):
         time.sleep(sleep_s)
         _trace.add_event("success")
 
 
 @_trace.traced
-def main():
+def multithread_main():
     _log.info("Preparing to process in threads.")
     otel_ctx = opentelemetry.context.get_current()
     threads = []
     for my_data in ("one", "two", "three", "four", "five", "six"):
         thread = threading.Thread(target=_thread_worker, args=(my_data, otel_ctx))
         thread.start()
         threads.append(thread)
     for thread in threads:
         thread.join()
     _log.info("Demo processing complete.")
 
 
 if __name__ == "__main__":
     logging.basicConfig(level=logging.INFO)
-    header_env = "OTEL_EXPORTER_OTLP_HEADERS"
+    header_env = "OTEL_EXPORTER_OTLP_HEADERS_JSON"
     endpoint_env = "OTEL_EXPORTER_OTLP_ENDPOINT"
     if header_env not in os.environ:
         _log.error(f"To upload traces, you must set {header_env}, see README.md.")
     configure(
         "form_observability_example",
-        otlp_headers=os.environ.get(header_env),
+        otlp_headers=json.loads(os.environ.get(header_env)),
         otlp_endpoint=os.environ.get(endpoint_env, "https://api.honeycomb.io"),
     )
     _log.addHandler(OtelSpanEventHandler())
-    main()
+    multithread_main()
```

### Comparing `formenergy-observability-0.3.0/form_observability/__init__.py` & `formenergy-observability-0.3.1/form_observability/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """OTel tracing/logging tools, emphasizing data pipeline use cases with Dagster."""
 
 #: Semantic versioning number. The three dotted numbers are:
 #: *   Major: breaking API changes, significant feature additions.
 #: *   Minor: standard feature additions and improvements. No breaking changes.
 #: *   Micro: small bug fixes.
-__version__ = "0.3.0"
+__version__ = "0.3.1"
 
 # Make commonly used symbols importable from form_observability.
 from .context_aware import ContextAwareTracer, ctx
 from .log import OtelSpanEventHandler
 from .otel_value import EventAttrKey, EventAttrValue, SpanName
 from .pipeline_setup import configure
```

### Comparing `formenergy-observability-0.3.0/form_observability/context_aware.py` & `formenergy-observability-0.3.1/form_observability/context_aware.py`

 * *Files identical despite different names*

### Comparing `formenergy-observability-0.3.0/form_observability/dagster_otel/otel_ops.py` & `formenergy-observability-0.3.1/form_observability/dagster_otel/otel_ops.py`

 * *Files identical despite different names*

### Comparing `formenergy-observability-0.3.0/form_observability/dagster_otel/test_otel_op.py` & `formenergy-observability-0.3.1/form_observability/dagster_otel/test_otel_op.py`

 * *Files identical despite different names*

### Comparing `formenergy-observability-0.3.0/form_observability/dagster_otel/test_timing.py` & `formenergy-observability-0.3.1/form_observability/dagster_otel/test_timing.py`

 * *Files identical despite different names*

### Comparing `formenergy-observability-0.3.0/form_observability/dagster_otel/testing.py` & `formenergy-observability-0.3.1/form_observability/dagster_otel/testing.py`

 * *Files identical despite different names*

### Comparing `formenergy-observability-0.3.0/form_observability/dagster_otel/timing.py` & `formenergy-observability-0.3.1/form_observability/dagster_otel/timing.py`

 * *Files identical despite different names*

### Comparing `formenergy-observability-0.3.0/form_observability/dagster_otel/util.py` & `formenergy-observability-0.3.1/form_observability/dagster_otel/util.py`

 * *Files identical despite different names*

### Comparing `formenergy-observability-0.3.0/form_observability/log.py` & `formenergy-observability-0.3.1/form_observability/log.py`

 * *Files identical despite different names*

### Comparing `formenergy-observability-0.3.0/form_observability/otel_value.py` & `formenergy-observability-0.3.1/form_observability/otel_value.py`

 * *Files identical despite different names*

### Comparing `formenergy-observability-0.3.0/form_observability/pipeline_setup.py` & `formenergy-observability-0.3.1/form_observability/pipeline_setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,28 +4,29 @@
 
 pipeline_setup.configure(
     "my-dataset",
     "x-honeycomb-team=<API key for desired environment>",
 )
 """
 import os
+from typing import Dict, Optional
 
 import opentelemetry
 from opentelemetry.instrumentation.requests import RequestsInstrumentor
 
 # Initialize tracing and an exporter that can send data to Honeycomb, New Relic, LightStep
 from opentelemetry.exporter.otlp.proto.grpc.trace_exporter import OTLPSpanExporter
 from opentelemetry.sdk.resources import SERVICE_NAME, Resource
 from opentelemetry.sdk.trace.export import SimpleSpanProcessor
 from opentelemetry.sdk.trace import TracerProvider, SpanLimits
 
 
 def configure(
     service_name: str,
-    otlp_headers: str,
+    otlp_headers: Optional[Dict[str, str]],
     otlp_endpoint: str = "https://api.honeycomb.io",
     instrument_requests: bool = False,
 ) -> None:
     """Set up a trace provider and processor, so tracing data gets exported.
 
     This sets options which are tuned for a multithreaded data pipeline which should
     export all data (without sampling) via OTLP (not a collector).
```

### Comparing `formenergy-observability-0.3.0/form_observability/test_context_aware.py` & `formenergy-observability-0.3.1/form_observability/test_context_aware.py`

 * *Files identical despite different names*

### Comparing `formenergy-observability-0.3.0/form_observability/testing.py` & `formenergy-observability-0.3.1/form_observability/testing.py`

 * *Files identical despite different names*

### Comparing `formenergy-observability-0.3.0/pyproject.toml` & `formenergy-observability-0.3.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `formenergy-observability-0.3.0/PKG-INFO` & `formenergy-observability-0.3.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: formenergy-observability
-Version: 0.3.0
+Version: 0.3.1
 Summary: OTel tracing/logging tools, emphasizing data pipeline use cases with Dagster.
 Author-email: Form Energy Software <software@formenergy.com>
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -79,26 +79,27 @@
 ```
 
 ### Running the Examples
 
 Get an API key for uploading traces to your observability service (preferably in a development environment), set it in your environment, and run the examples. This should publish traces that you can then view.
 
 ```bash
-export OTEL_EXPORTER_OTLP_HEADERS="x-honeycomb-team=<API key>"
+export OTEL_EXPORTER_OTLP_HEADERS_JSON="{'x-honeycomb-team': '<API key>'}"
 export OTEL_EXPORTER_OTLP_ENDPOINT="your observability service, defaults to Honeycomb"
 python examples/basics.py
 dagster job execute --python-file examples/dagster_job.py
 ```
 
 ## License
 
 This library is provided under the MIT license, see [LICENSE](LICENSE).
 
 ## Release Notes
 
+*   0.3.1 Fix type used for `otlp_headers` to be a `dict`. Thanks @spenczar !
 *   0.3.0 Add `ContextAwareTracer.start_new_linked_trace`.
 *   0.2.0 Switch to `context.op_handle` and `materialization.metadata` as dict for Dagster 1.2.
 *   0.1.0 Initial external release, including `ContextAwareTracer`, `ctx`, and `@otel_op`.
 
 ## Development
 
 If you contribute, please ensure you and your employer accept [the license](LICENSE) for any of your contributions.
```


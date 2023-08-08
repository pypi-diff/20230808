# Comparing `tmp/serverless-aws-lambda-sdk-0.2.1.tar.gz` & `tmp/serverless-aws-lambda-sdk-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/console/console/python/packages/dist/.tmp-j4kltbbd/serverless-aws-lambda-sdk-0.2.1.tar", last modified: Wed Jun 21 15:42:54 2023, max compression
+gzip compressed data, was "/home/runner/work/console/console/python/packages/dist/.tmp-jxgs2262/serverless-aws-lambda-sdk-0.2.2.tar", last modified: Tue Aug  8 16:36:07 2023, max compression
```

## Comparing `serverless-aws-lambda-sdk-0.2.1.tar` & `serverless-aws-lambda-sdk-0.2.2.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 15:42:54.000000 serverless-aws-lambda-sdk-0.2.1/
--rw-r--r--   0 runner    (1001) docker     (123)     2522 2023-06-21 15:42:54.000000 serverless-aws-lambda-sdk-0.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1647 2023-06-21 15:42:34.000000 serverless-aws-lambda-sdk-0.2.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1905 2023-06-21 15:42:34.000000 serverless-aws-lambda-sdk-0.2.1/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 15:42:54.000000 serverless-aws-lambda-sdk-0.2.1/serverless_aws_lambda_sdk/
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-21 15:42:34.000000 serverless-aws-lambda-sdk-0.2.1/serverless_aws_lambda_sdk/VERSION
--rw-r--r--   0 runner    (1001) docker     (123)     2571 2023-06-21 15:42:34.000000 serverless-aws-lambda-sdk-0.2.1/serverless_aws_lambda_sdk/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 15:42:54.000000 serverless-aws-lambda-sdk-0.2.1/serverless_aws_lambda_sdk/instrument/
--rw-r--r--   0 runner    (1001) docker     (123)    21378 2023-06-21 15:42:34.000000 serverless-aws-lambda-sdk-0.2.1/serverless_aws_lambda_sdk/instrument/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 15:42:54.000000 serverless-aws-lambda-sdk-0.2.1/serverless_aws_lambda_sdk/instrument/lib/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 15:42:34.000000 serverless-aws-lambda-sdk-0.2.1/serverless_aws_lambda_sdk/instrument/lib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      351 2023-06-21 15:42:34.000000 serverless-aws-lambda-sdk-0.2.1/serverless_aws_lambda_sdk/instrument/lib/api_events.py
--rw-r--r--   0 runner    (1001) docker     (123)      494 2023-06-21 15:42:34.000000 serverless-aws-lambda-sdk-0.2.1/serverless_aws_lambda_sdk/instrument/lib/captured_event.py
--rw-r--r--   0 runner    (1001) docker     (123)     5624 2023-06-21 15:42:34.000000 serverless-aws-lambda-sdk-0.2.1/serverless_aws_lambda_sdk/instrument/lib/dev_mode.py
--rw-r--r--   0 runner    (1001) docker     (123)    10039 2023-06-21 15:42:34.000000 serverless-aws-lambda-sdk-0.2.1/serverless_aws_lambda_sdk/instrument/lib/event_tags.py
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-06-21 15:42:34.000000 serverless-aws-lambda-sdk-0.2.1/serverless_aws_lambda_sdk/instrument/lib/invocation_context.py
--rw-r--r--   0 runner    (1001) docker     (123)     1290 2023-06-21 15:42:34.000000 serverless-aws-lambda-sdk-0.2.1/serverless_aws_lambda_sdk/instrument/lib/payload_conversion.py
--rw-r--r--   0 runner    (1001) docker     (123)      637 2023-06-21 15:42:34.000000 serverless-aws-lambda-sdk-0.2.1/serverless_aws_lambda_sdk/instrument/lib/response_tags.py
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-06-21 15:42:34.000000 serverless-aws-lambda-sdk-0.2.1/serverless_aws_lambda_sdk/instrument/lib/sdk.py
--rw-r--r--   0 runner    (1001) docker     (123)     1996 2023-06-21 15:42:34.000000 serverless-aws-lambda-sdk-0.2.1/serverless_aws_lambda_sdk/instrument/lib/telemetry.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 15:42:54.000000 serverless-aws-lambda-sdk-0.2.1/serverless_aws_lambda_sdk/instrumentation/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 15:42:34.000000 serverless-aws-lambda-sdk-0.2.1/serverless_aws_lambda_sdk/instrumentation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4719 2023-06-21 15:42:34.000000 serverless-aws-lambda-sdk-0.2.1/serverless_aws_lambda_sdk/instrumentation/aws_sdk.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 15:42:54.000000 serverless-aws-lambda-sdk-0.2.1/serverless_aws_lambda_sdk/internal_extension/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 15:42:34.000000 serverless-aws-lambda-sdk-0.2.1/serverless_aws_lambda_sdk/internal_extension/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3063 2023-06-21 15:42:34.000000 serverless-aws-lambda-sdk-0.2.1/serverless_aws_lambda_sdk/internal_extension/exec_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     1815 2023-06-21 15:42:34.000000 serverless-aws-lambda-sdk-0.2.1/serverless_aws_lambda_sdk/internal_extension/wrapper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 15:42:54.000000 serverless-aws-lambda-sdk-0.2.1/serverless_aws_lambda_sdk/lib/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 15:42:54.000000 serverless-aws-lambda-sdk-0.2.1/serverless_aws_lambda_sdk/lib/instrumentation/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 15:42:54.000000 serverless-aws-lambda-sdk-0.2.1/serverless_aws_lambda_sdk/lib/instrumentation/aws_sdk/
--rw-r--r--   0 runner    (1001) docker     (123)      536 2023-06-21 15:42:34.000000 serverless-aws-lambda-sdk-0.2.1/serverless_aws_lambda_sdk/lib/instrumentation/aws_sdk/safe_stringify.py
--rw-r--r--   0 runner    (1001) docker     (123)     5134 2023-06-21 15:42:34.000000 serverless-aws-lambda-sdk-0.2.1/serverless_aws_lambda_sdk/lib/instrumentation/aws_sdk/service_mapper.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 15:42:34.000000 serverless-aws-lambda-sdk-0.2.1/serverless_aws_lambda_sdk/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 15:42:54.000000 serverless-aws-lambda-sdk-0.2.1/serverless_aws_lambda_sdk/trace_spans/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 15:42:34.000000 serverless-aws-lambda-sdk-0.2.1/serverless_aws_lambda_sdk/trace_spans/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1494 2023-06-21 15:42:34.000000 serverless-aws-lambda-sdk-0.2.1/serverless_aws_lambda_sdk/trace_spans/aws_lambda.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 15:42:54.000000 serverless-aws-lambda-sdk-0.2.1/serverless_aws_lambda_sdk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2522 2023-06-21 15:42:54.000000 serverless-aws-lambda-sdk-0.2.1/serverless_aws_lambda_sdk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1566 2023-06-21 15:42:54.000000 serverless-aws-lambda-sdk-0.2.1/serverless_aws_lambda_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 15:42:54.000000 serverless-aws-lambda-sdk-0.2.1/serverless_aws_lambda_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      326 2023-06-21 15:42:54.000000 serverless-aws-lambda-sdk-0.2.1/serverless_aws_lambda_sdk.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-06-21 15:42:54.000000 serverless-aws-lambda-sdk-0.2.1/serverless_aws_lambda_sdk.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-21 15:42:54.000000 serverless-aws-lambda-sdk-0.2.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 15:42:54.000000 serverless-aws-lambda-sdk-0.2.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      671 2023-06-21 15:42:34.000000 serverless-aws-lambda-sdk-0.2.1/tests/test_sdk.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 16:36:07.000000 serverless-aws-lambda-sdk-0.2.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     2522 2023-08-08 16:36:07.000000 serverless-aws-lambda-sdk-0.2.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1647 2023-08-08 16:35:46.000000 serverless-aws-lambda-sdk-0.2.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1929 2023-08-08 16:35:46.000000 serverless-aws-lambda-sdk-0.2.2/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 16:36:07.000000 serverless-aws-lambda-sdk-0.2.2/serverless_aws_lambda_sdk/
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-08-08 16:35:46.000000 serverless-aws-lambda-sdk-0.2.2/serverless_aws_lambda_sdk/VERSION
+-rw-r--r--   0 runner    (1001) docker     (123)     2571 2023-08-08 16:35:46.000000 serverless-aws-lambda-sdk-0.2.2/serverless_aws_lambda_sdk/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 16:36:07.000000 serverless-aws-lambda-sdk-0.2.2/serverless_aws_lambda_sdk/instrument/
+-rw-r--r--   0 runner    (1001) docker     (123)    21448 2023-08-08 16:35:46.000000 serverless-aws-lambda-sdk-0.2.2/serverless_aws_lambda_sdk/instrument/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 16:36:07.000000 serverless-aws-lambda-sdk-0.2.2/serverless_aws_lambda_sdk/instrument/lib/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 16:35:46.000000 serverless-aws-lambda-sdk-0.2.2/serverless_aws_lambda_sdk/instrument/lib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      351 2023-08-08 16:35:46.000000 serverless-aws-lambda-sdk-0.2.2/serverless_aws_lambda_sdk/instrument/lib/api_events.py
+-rw-r--r--   0 runner    (1001) docker     (123)      494 2023-08-08 16:35:46.000000 serverless-aws-lambda-sdk-0.2.2/serverless_aws_lambda_sdk/instrument/lib/captured_event.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5637 2023-08-08 16:35:46.000000 serverless-aws-lambda-sdk-0.2.2/serverless_aws_lambda_sdk/instrument/lib/dev_mode.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10039 2023-08-08 16:35:46.000000 serverless-aws-lambda-sdk-0.2.2/serverless_aws_lambda_sdk/instrument/lib/event_tags.py
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-08-08 16:35:46.000000 serverless-aws-lambda-sdk-0.2.2/serverless_aws_lambda_sdk/instrument/lib/invocation_context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1405 2023-08-08 16:35:46.000000 serverless-aws-lambda-sdk-0.2.2/serverless_aws_lambda_sdk/instrument/lib/payload_conversion.py
+-rw-r--r--   0 runner    (1001) docker     (123)      637 2023-08-08 16:35:46.000000 serverless-aws-lambda-sdk-0.2.2/serverless_aws_lambda_sdk/instrument/lib/response_tags.py
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-08-08 16:35:46.000000 serverless-aws-lambda-sdk-0.2.2/serverless_aws_lambda_sdk/instrument/lib/sdk.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1996 2023-08-08 16:35:46.000000 serverless-aws-lambda-sdk-0.2.2/serverless_aws_lambda_sdk/instrument/lib/telemetry.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 16:36:07.000000 serverless-aws-lambda-sdk-0.2.2/serverless_aws_lambda_sdk/instrumentation/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 16:35:46.000000 serverless-aws-lambda-sdk-0.2.2/serverless_aws_lambda_sdk/instrumentation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4719 2023-08-08 16:35:46.000000 serverless-aws-lambda-sdk-0.2.2/serverless_aws_lambda_sdk/instrumentation/aws_sdk.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 16:36:07.000000 serverless-aws-lambda-sdk-0.2.2/serverless_aws_lambda_sdk/internal_extension/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 16:35:46.000000 serverless-aws-lambda-sdk-0.2.2/serverless_aws_lambda_sdk/internal_extension/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3063 2023-08-08 16:35:46.000000 serverless-aws-lambda-sdk-0.2.2/serverless_aws_lambda_sdk/internal_extension/exec_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1815 2023-08-08 16:35:46.000000 serverless-aws-lambda-sdk-0.2.2/serverless_aws_lambda_sdk/internal_extension/wrapper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 16:36:07.000000 serverless-aws-lambda-sdk-0.2.2/serverless_aws_lambda_sdk/lib/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 16:36:07.000000 serverless-aws-lambda-sdk-0.2.2/serverless_aws_lambda_sdk/lib/instrumentation/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 16:36:07.000000 serverless-aws-lambda-sdk-0.2.2/serverless_aws_lambda_sdk/lib/instrumentation/aws_sdk/
+-rw-r--r--   0 runner    (1001) docker     (123)      536 2023-08-08 16:35:46.000000 serverless-aws-lambda-sdk-0.2.2/serverless_aws_lambda_sdk/lib/instrumentation/aws_sdk/safe_stringify.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5134 2023-08-08 16:35:46.000000 serverless-aws-lambda-sdk-0.2.2/serverless_aws_lambda_sdk/lib/instrumentation/aws_sdk/service_mapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 16:35:46.000000 serverless-aws-lambda-sdk-0.2.2/serverless_aws_lambda_sdk/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 16:36:07.000000 serverless-aws-lambda-sdk-0.2.2/serverless_aws_lambda_sdk/trace_spans/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 16:35:46.000000 serverless-aws-lambda-sdk-0.2.2/serverless_aws_lambda_sdk/trace_spans/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1494 2023-08-08 16:35:46.000000 serverless-aws-lambda-sdk-0.2.2/serverless_aws_lambda_sdk/trace_spans/aws_lambda.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 16:36:07.000000 serverless-aws-lambda-sdk-0.2.2/serverless_aws_lambda_sdk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2522 2023-08-08 16:36:07.000000 serverless-aws-lambda-sdk-0.2.2/serverless_aws_lambda_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1566 2023-08-08 16:36:07.000000 serverless-aws-lambda-sdk-0.2.2/serverless_aws_lambda_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 16:36:07.000000 serverless-aws-lambda-sdk-0.2.2/serverless_aws_lambda_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      343 2023-08-08 16:36:07.000000 serverless-aws-lambda-sdk-0.2.2/serverless_aws_lambda_sdk.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-08-08 16:36:07.000000 serverless-aws-lambda-sdk-0.2.2/serverless_aws_lambda_sdk.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-08 16:36:07.000000 serverless-aws-lambda-sdk-0.2.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 16:36:07.000000 serverless-aws-lambda-sdk-0.2.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      671 2023-08-08 16:35:46.000000 serverless-aws-lambda-sdk-0.2.2/tests/test_sdk.py
```

### Comparing `serverless-aws-lambda-sdk-0.2.1/PKG-INFO` & `serverless-aws-lambda-sdk-0.2.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: serverless-aws-lambda-sdk
-Version: 0.2.1
+Version: 0.2.2
 Summary: Serverless AWS Lambda SDK for Python
 Author: serverlessinc
 Project-URL: changelog, https://github.com/serverless/console/blob/main/python/packages/aws-lambda-sdk/CHANGELOG.md
 Project-URL: documentation, https://github.com/serverless/console/tree/main/python/packages/aws-lambda-sdk
 Project-URL: homepage, https://www.serverless.com/console
 Project-URL: repository, https://github.com/serverless/console
 Classifier: Programming Language :: Python :: 3 :: Only
```

### Comparing `serverless-aws-lambda-sdk-0.2.1/README.md` & `serverless-aws-lambda-sdk-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `serverless-aws-lambda-sdk-0.2.1/pyproject.toml` & `serverless-aws-lambda-sdk-0.2.2/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -19,22 +19,23 @@
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
 ]
 dynamic = [
     "version",
 ]
 dependencies = [
-    "serverless-sdk~=0.5.1",
+    "serverless-sdk~=0.5.4",
     "serverless-sdk-schema~=0.2.3",
     "typing-extensions~=4.5", # included in Python 3.8 - 3.11
 ]
 [project.optional-dependencies]
 tests = [
+    "aiobotocore>=2.5.1",
     "black>=22.12",
-    "boto3>=1.16.112",
+    "boto3>=1.25.1",
     "flask>=2.2.3",
     "importlib_metadata>=5.2", # included in Python >=3.8
     "mypy>=1.2",
     "pynamodb>=5.5",
     "pytest>=7.2",
     "pytest-aiohttp>=1.0.4",
     "pytest-httpserver>=1.0.6",
```

### Comparing `serverless-aws-lambda-sdk-0.2.1/serverless_aws_lambda_sdk/__init__.py` & `serverless-aws-lambda-sdk-0.2.2/serverless_aws_lambda_sdk/__init__.py`

 * *Files identical despite different names*

### Comparing `serverless-aws-lambda-sdk-0.2.1/serverless_aws_lambda_sdk/instrument/__init__.py` & `serverless-aws-lambda-sdk-0.2.2/serverless_aws_lambda_sdk/instrument/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,23 +16,26 @@
         from typing_extensions import Final
     import random
 
     import base64
     import gzip
 
 from sls_sdk.lib.timing import to_protobuf_epoch_timestamp
-from sls_sdk.lib.imports import internally_imported
 from sls_sdk.lib.trace import TraceSpan
 from sls_sdk.lib.captured_event import CapturedEvent
 from .lib.sdk import serverlessSdk
 from .lib.invocation_context import (
     set as set_invocation_context,
     get as get_invocation_context,
 )
-from .lib.payload_conversion import to_trace_payload, to_request_response_payload
+from .lib.payload_conversion import (
+    to_trace_payload,
+    to_request_response_payload,
+    serialize_to_string,
+)
 from .lib.event_tags import resolve as resolve_event_tags
 from .lib.response_tags import resolve as resolve_response_tags
 from .lib.api_events import is_api_event
 from .lib.captured_event import should_include as should_include_event_captured_event
 
 
 MAX_LOG_LINE_LENGTH = 256 * 1024
@@ -81,15 +84,15 @@
         },
         "spans": [_convert_span(s) for s in spans],
         "events": [e.to_protobuf_dict() for e in captured_events],
         "customTags": custom_tags,
     }
 
     payload = to_trace_payload(payload_dct)
-    compressed_payload = gzip.compress(payload.SerializeToString())
+    compressed_payload = gzip.compress(serialize_to_string(payload))
     serialized = base64.b64encode(compressed_payload).decode("utf-8")
     return f"SERVERLESS_TELEMETRY.TZ.{serialized}"
 
 
 def _resolve_outcome_enum_value(outcome: str) -> int:
     if outcome == "success":
         return 1
@@ -154,15 +157,16 @@
                 + 'Ensure "SLS_ORG_ID" environment variable is set, '
                 + "or pass it with the options\n"
             )
 
         if serverlessSdk._is_dev_mode:
             from .lib.dev_mode import get_dev_mode_thread
 
-            self.dev_mode = get_dev_mode_thread()
+            self._get_dev_mode_thread = get_dev_mode_thread
+            self.dev_mode = self._get_dev_mode_thread()
 
         serverlessSdk.trace_spans.aws_lambda_initialization.close()
 
     def _captured_event_handler(self, captured_event: CapturedEvent):
         serverlessSdk._captured_events.append(captured_event)
         # Only report captured events, if dev mode is active and the event is not
         # a dev mode server issue, to prevent infinite loops.
@@ -196,15 +200,15 @@
             "body": _resolve_body_string(event, "INPUT"),
             "origin": 1,
         }
         payload_buffer = (
             serverlessSdk._last_request_buffer
         ) = to_request_response_payload(payload_dct)
         return self.dev_mode.add_request_response_payload(
-            payload_buffer.SerializeToString(),
+            serialize_to_string(payload_buffer),
         )
 
     def _report_response(self, response, context, end_time):
         response_string = _resolve_body_string(response, "OUTPUT")
         payload_dct = serverlessSdk._last_response = {
             "slsTags": {
                 "orgId": serverlessSdk.org_id,
@@ -221,15 +225,15 @@
             "timestamp": to_protobuf_epoch_timestamp(end_time),
             "body": response_string,
             "origin": 2,
         }
         payload_buffer = (
             serverlessSdk._last_response_buffer
         ) = to_request_response_payload(payload_dct)
-        self.dev_mode.add_request_response_payload(payload_buffer.SerializeToString())
+        self.dev_mode.add_request_response_payload(serialize_to_string(payload_buffer))
 
     def _report_trace(self, is_error_outcome: bool):
         should_set_is_after_not_sampled_out_api_request = False
         _is_api_event = is_api_event()
 
         def calculate_is_sampled_out():
             # This function determines if a trace should be sampled out or not
@@ -456,15 +460,14 @@
         return print(result_log_text)
 
     def _flush_and_close_event_loop(self):
         if self.dev_mode:
             self.dev_mode.terminate()
             self.dev_mode = None
 
-    @internally_imported()
     def _close_trace(self, outcome: str, outcome_result: Optional[Any] = None):
         self.is_root_span_reset = False
         try:
             end_time = time.perf_counter_ns()
             is_error_outcome = outcome.startswith("error:")
 
             self.aws_lambda.tags["aws.lambda.outcome"] = _resolve_outcome_enum_value(
@@ -489,14 +492,20 @@
                 serverlessSdk.trace_spans.aws_lambda_initialization.close(
                     end_time=end_time
                 )
 
             if serverlessSdk.trace_spans.aws_lambda_invocation:
                 serverlessSdk.trace_spans.aws_lambda_invocation.close(end_time=end_time)
 
+            if serverlessSdk._user_defined_endpoint:
+                del self.aws_lambda.tags["aws.lambda.http_router.path"]
+                self.aws_lambda.tags[
+                    "aws.lambda.http_router.path"
+                ] = serverlessSdk._user_defined_endpoint
+
             self.aws_lambda.close(end_time=end_time)
             self._flush_and_close_event_loop()
 
             if get_invocation_context():
                 self._report_trace(is_error_outcome)
             self._clear_root_span()
 
@@ -519,57 +528,54 @@
         serverlessSdk._captured_events = []
         serverlessSdk._custom_tags.clear()
         self.is_root_span_reset = True
 
     def _handler(self, user_handler, event, context):
         request_start_time = time.perf_counter_ns()
         self.current_invocation_id += 1
-        with internally_imported():
-            try:
-                debug_log("Invocation: start")
-                set_invocation_context(context)
-
-                if self.previous_invocation_end_time:
-                    self.gaps_between_invocations.append(
-                        time.time_ns() - self.previous_invocation_end_time
-                    )
-                    self.previous_invocation_end_time = None
-                    if len(self.gaps_between_invocations) > 5:
-                        self.gaps_between_invocations.pop(0)
-
-                if self.current_invocation_id > 1:
-                    self.aws_lambda.start_time = request_start_time
-
-                self.aws_lambda.tags["aws.lambda.request_id"] = context.aws_request_id
-
-                # Event loop may already be active in case of a cold start
-                # That's why we create it only if it's not already set
-                if serverlessSdk._is_dev_mode and self.dev_mode is None:
-                    from .lib.dev_mode import get_dev_mode_thread
-
-                    self.dev_mode = get_dev_mode_thread()
-
-                serverlessSdk.trace_spans.aws_lambda_invocation = (
-                    serverlessSdk._create_trace_span(
-                        "aws.lambda.invocation", start_time=request_start_time
-                    )
+        try:
+            debug_log("Invocation: start")
+            set_invocation_context(context)
+
+            if self.previous_invocation_end_time:
+                self.gaps_between_invocations.append(
+                    time.time_ns() - self.previous_invocation_end_time
                 )
-                resolve_event_tags(event)
-                if (
-                    serverlessSdk._is_dev_mode
-                    and not serverlessSdk._settings.disable_request_response_monitoring
-                ):
-                    self._report_request(event, context)
-
-                diff = int((time.perf_counter_ns() - request_start_time) / 1000_000)
-                debug_log("Overhead duration: Internal request:" + f"{diff}ms")
-
-            except Exception as ex:
-                serverlessSdk._report_error(ex)
-                return user_handler(event, context)
+                self.previous_invocation_end_time = None
+                if len(self.gaps_between_invocations) > 5:
+                    self.gaps_between_invocations.pop(0)
+
+            if self.current_invocation_id > 1:
+                self.aws_lambda.start_time = request_start_time
+
+            self.aws_lambda.tags["aws.lambda.request_id"] = context.aws_request_id
+
+            # Event loop may already be active in case of a cold start
+            # That's why we create it only if it's not already set
+            if serverlessSdk._is_dev_mode and self.dev_mode is None:
+                self.dev_mode = self._get_dev_mode_thread()
+
+            serverlessSdk.trace_spans.aws_lambda_invocation = (
+                serverlessSdk._create_trace_span(
+                    "aws.lambda.invocation", start_time=request_start_time
+                )
+            )
+            resolve_event_tags(event)
+            if (
+                serverlessSdk._is_dev_mode
+                and not serverlessSdk._settings.disable_request_response_monitoring
+            ):
+                self._report_request(event, context)
+
+            diff = int((time.perf_counter_ns() - request_start_time) / 1000_000)
+            debug_log("Overhead duration: Internal request:" + f"{diff}ms")
+
+        except Exception as ex:
+            serverlessSdk._report_error(ex)
+            return user_handler(event, context)
 
         # Invocation of customer code
         try:
             result = user_handler(event, context)
         except BaseException as ex:  # catches all exceptions, including SystemExit.
             if isinstance(ex, Exception):
                 self._close_trace("error:handled", ex)
```

### Comparing `serverless-aws-lambda-sdk-0.2.1/serverless_aws_lambda_sdk/instrument/lib/dev_mode.py` & `serverless-aws-lambda-sdk-0.2.2/serverless_aws_lambda_sdk/instrument/lib/dev_mode.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
     import os
     import builtins
     import logging
 
 from .telemetry import send, close_connection
 from .sdk import serverlessSdk
 from .invocation_context import get as get_invocation_context
-from .payload_conversion import to_trace_payload
+from .payload_conversion import to_trace_payload, serialize_to_string
 from .captured_event import should_include as should_include_event_captured_event
 
 _original_print = builtins.print
 
 
 def _print(self, *args, **kwargs):
     # to make sure print & logging calls from multiple threads are serialized properly
@@ -83,17 +83,16 @@
         self._loop = None
         self._has_started = (
             start_event  # when the thread starts, the event will be signalled
         )
         self._buffered_data = (
             ThreadSafeBuffer()
         )  # used to buffer spans and captured events
-        self._is_stopped = Event()  # used to stop the thread
+        self._is_stopped_event = Event()  # used to stop the thread
 
-    @internally_imported()
     def _send_all(self):
         (
             spans,
             captured_events,
             request_response_payload,
         ) = self._buffered_data.get_all()
 
@@ -127,15 +126,15 @@
             "customTags": json.dumps(serverlessSdk._custom_tags),
         }
         if not get_invocation_context():
             payload["spans"] = [
                 s for s in payload["spans"] if s["name"] != "aws.lambda"
             ]
 
-        send("trace", to_trace_payload(payload).SerializeToString())
+        send("trace", serialize_to_string(to_trace_payload(payload)))
 
     def add_span(self, span):
         """Executes in the context of the main thread."""
         self._buffered_data.add_span(span)
 
     def add_captured_event(self, captured_event):
         """Executes in the context of the main thread."""
@@ -148,28 +147,28 @@
     def run(self):
         """Executes in the context of the dev-mode thread."""
 
         # signal that the thread is running
         self._has_started.set()
 
         while True:
-            is_stopped = self._is_stopped.wait(0.05)
+            is_stopped = self._is_stopped_event.wait(0.05)
             if is_stopped:
                 break
 
             self._send_all()
 
         self._send_all()
         close_connection()
 
     def terminate(self):
         """
         Signal the thread to stop, any remaining data will be flushed.
         """
-        self._is_stopped.set()
+        self._is_stopped_event.set()
         self.join()
 
 
 def get_dev_mode_thread() -> DevModeThread:
     event = Event()
     thread = DevModeThread(event)
     thread.start()
```

### Comparing `serverless-aws-lambda-sdk-0.2.1/serverless_aws_lambda_sdk/instrument/lib/event_tags.py` & `serverless-aws-lambda-sdk-0.2.2/serverless_aws_lambda_sdk/instrument/lib/event_tags.py`

 * *Files identical despite different names*

### Comparing `serverless-aws-lambda-sdk-0.2.1/serverless_aws_lambda_sdk/instrument/lib/payload_conversion.py` & `serverless-aws-lambda-sdk-0.2.2/serverless_aws_lambda_sdk/instrument/lib/payload_conversion.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,19 @@
 from sls_sdk.lib.imports import internally_imported
 
 with internally_imported():
     from serverless_sdk_schema import TracePayload, RequestResponse
     from google.protobuf import json_format
 
 
+@internally_imported()
+def serialize_to_string(trace: TracePayload) -> str:
+    return trace.SerializeToString()
+
+
 def to_trace_payload(payload_dct: dict) -> TracePayload:
     spans = payload_dct["spans"]
     events = payload_dct["events"]
     payload = json_format.ParseDict(payload_dct, TracePayload())
     for index, span in enumerate(payload.spans):
         span.id = bytes(spans[index]["id"], "utf-8")
         span.trace_id = bytes(spans[index]["traceId"], "utf-8")
```

### Comparing `serverless-aws-lambda-sdk-0.2.1/serverless_aws_lambda_sdk/instrument/lib/response_tags.py` & `serverless-aws-lambda-sdk-0.2.2/serverless_aws_lambda_sdk/instrument/lib/response_tags.py`

 * *Files identical despite different names*

### Comparing `serverless-aws-lambda-sdk-0.2.1/serverless_aws_lambda_sdk/instrument/lib/telemetry.py` & `serverless-aws-lambda-sdk-0.2.2/serverless_aws_lambda_sdk/instrument/lib/telemetry.py`

 * *Files identical despite different names*

### Comparing `serverless-aws-lambda-sdk-0.2.1/serverless_aws_lambda_sdk/instrumentation/aws_sdk.py` & `serverless-aws-lambda-sdk-0.2.2/serverless_aws_lambda_sdk/instrumentation/aws_sdk.py`

 * *Files identical despite different names*

### Comparing `serverless-aws-lambda-sdk-0.2.1/serverless_aws_lambda_sdk/internal_extension/exec_wrapper.py` & `serverless-aws-lambda-sdk-0.2.2/serverless_aws_lambda_sdk/internal_extension/exec_wrapper.py`

 * *Files identical despite different names*

### Comparing `serverless-aws-lambda-sdk-0.2.1/serverless_aws_lambda_sdk/internal_extension/wrapper.py` & `serverless-aws-lambda-sdk-0.2.2/serverless_aws_lambda_sdk/internal_extension/wrapper.py`

 * *Files identical despite different names*

### Comparing `serverless-aws-lambda-sdk-0.2.1/serverless_aws_lambda_sdk/lib/instrumentation/aws_sdk/safe_stringify.py` & `serverless-aws-lambda-sdk-0.2.2/serverless_aws_lambda_sdk/lib/instrumentation/aws_sdk/safe_stringify.py`

 * *Files identical despite different names*

### Comparing `serverless-aws-lambda-sdk-0.2.1/serverless_aws_lambda_sdk/lib/instrumentation/aws_sdk/service_mapper.py` & `serverless-aws-lambda-sdk-0.2.2/serverless_aws_lambda_sdk/lib/instrumentation/aws_sdk/service_mapper.py`

 * *Files identical despite different names*

### Comparing `serverless-aws-lambda-sdk-0.2.1/serverless_aws_lambda_sdk/trace_spans/aws_lambda.py` & `serverless-aws-lambda-sdk-0.2.2/serverless_aws_lambda_sdk/trace_spans/aws_lambda.py`

 * *Files identical despite different names*

### Comparing `serverless-aws-lambda-sdk-0.2.1/serverless_aws_lambda_sdk.egg-info/PKG-INFO` & `serverless-aws-lambda-sdk-0.2.2/serverless_aws_lambda_sdk.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: serverless-aws-lambda-sdk
-Version: 0.2.1
+Version: 0.2.2
 Summary: Serverless AWS Lambda SDK for Python
 Author: serverlessinc
 Project-URL: changelog, https://github.com/serverless/console/blob/main/python/packages/aws-lambda-sdk/CHANGELOG.md
 Project-URL: documentation, https://github.com/serverless/console/tree/main/python/packages/aws-lambda-sdk
 Project-URL: homepage, https://www.serverless.com/console
 Project-URL: repository, https://github.com/serverless/console
 Classifier: Programming Language :: Python :: 3 :: Only
```

### Comparing `serverless-aws-lambda-sdk-0.2.1/serverless_aws_lambda_sdk.egg-info/SOURCES.txt` & `serverless-aws-lambda-sdk-0.2.2/serverless_aws_lambda_sdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `serverless-aws-lambda-sdk-0.2.1/tests/test_sdk.py` & `serverless-aws-lambda-sdk-0.2.2/tests/test_sdk.py`

 * *Files identical despite different names*


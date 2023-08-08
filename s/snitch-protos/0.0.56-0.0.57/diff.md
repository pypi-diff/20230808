# Comparing `tmp/snitch-protos-0.0.56.tar.gz` & `tmp/snitch-protos-0.0.57.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "snitch-protos-0.0.56.tar", last modified: Thu Aug  3 17:21:01 2023, max compression
+gzip compressed data, was "snitch-protos-0.0.57.tar", last modified: Tue Aug  8 17:45:18 2023, max compression
```

## Comparing `snitch-protos-0.0.56.tar` & `snitch-protos-0.0.57.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 17:21:01.658234 snitch-protos-0.0.56/
--rw-r--r--   0 runner    (1001) docker     (123)      887 2023-08-03 17:21:01.658234 snitch-protos-0.0.56/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      208 2023-08-03 17:20:31.000000 snitch-protos-0.0.56/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-03 17:21:01.658234 snitch-protos-0.0.56/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1045 2023-08-03 17:21:01.000000 snitch-protos-0.0.56/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 17:21:01.658234 snitch-protos-0.0.56/snitch_protos/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 17:20:31.000000 snitch-protos-0.0.56/snitch_protos/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 17:21:01.658234 snitch-protos-0.0.56/snitch_protos/protos/
--rw-r--r--   0 runner    (1001) docker     (123)    35003 2023-08-03 17:20:31.000000 snitch-protos-0.0.56/snitch_protos/protos/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 17:21:01.658234 snitch-protos-0.0.56/snitch_protos/protos/steps/
--rw-r--r--   0 runner    (1001) docker     (123)     4952 2023-08-03 17:20:31.000000 snitch-protos-0.0.56/snitch_protos/protos/steps/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 17:21:01.658234 snitch-protos-0.0.56/snitch_protos.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      887 2023-08-03 17:21:01.000000 snitch-protos-0.0.56/snitch_protos.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      264 2023-08-03 17:21:01.000000 snitch-protos-0.0.56/snitch_protos.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-03 17:21:01.000000 snitch-protos-0.0.56/snitch_protos.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-08-03 17:21:01.000000 snitch-protos-0.0.56/snitch_protos.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 17:45:18.347193 snitch-protos-0.0.57/
+-rw-r--r--   0 runner    (1001) docker     (123)      887 2023-08-08 17:45:18.347193 snitch-protos-0.0.57/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2023-08-08 17:44:35.000000 snitch-protos-0.0.57/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-08 17:45:18.347193 snitch-protos-0.0.57/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1045 2023-08-08 17:45:17.000000 snitch-protos-0.0.57/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 17:45:18.347193 snitch-protos-0.0.57/snitch_protos/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 17:44:35.000000 snitch-protos-0.0.57/snitch_protos/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 17:45:18.347193 snitch-protos-0.0.57/snitch_protos/protos/
+-rw-r--r--   0 runner    (1001) docker     (123)    35028 2023-08-08 17:44:35.000000 snitch-protos-0.0.57/snitch_protos/protos/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 17:45:18.347193 snitch-protos-0.0.57/snitch_protos/protos/steps/
+-rw-r--r--   0 runner    (1001) docker     (123)     5057 2023-08-08 17:44:35.000000 snitch-protos-0.0.57/snitch_protos/protos/steps/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 17:45:18.347193 snitch-protos-0.0.57/snitch_protos.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      887 2023-08-08 17:45:18.000000 snitch-protos-0.0.57/snitch_protos.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      264 2023-08-08 17:45:18.000000 snitch-protos-0.0.57/snitch_protos.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 17:45:18.000000 snitch-protos-0.0.57/snitch_protos.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-08-08 17:45:18.000000 snitch-protos-0.0.57/snitch_protos.egg-info/top_level.txt
```

### Comparing `snitch-protos-0.0.56/PKG-INFO` & `snitch-protos-0.0.57/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: snitch-protos
-Version: 0.0.56
+Version: 0.0.57
 Summary: Protobuf python package for Streamdal.com Snitch
 Home-page: https://github.com/streamdal/snitch-protos
 Author: Streamdal.com
 Author-email: engineering@streamdal.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 1 - Planning
```

### Comparing `snitch-protos-0.0.56/setup.py` & `snitch-protos-0.0.57/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from pathlib import Path
 
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
     name='snitch-protos',
-    version='0.0.56',
+    version='0.0.57',
     description='Protobuf python package for Streamdal.com Snitch',
     long_description=long_description,
     long_description_content_type="text/markdown",
     url='https://github.com/streamdal/snitch-protos',
     author='Streamdal.com',
     author_email='engineering@streamdal.com',
     license='MIT',
```

### Comparing `snitch-protos-0.0.56/snitch_protos/protos/__init__.py` & `snitch-protos-0.0.57/snitch_protos/protos/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -142,21 +142,22 @@
     """What should SDK do if step fails?"""
 
     detective: "steps.DetectiveStep" = betterproto.message_field(1000, group="step")
     transform: "steps.TransformStep" = betterproto.message_field(1001, group="step")
     encode: "steps.EncodeStep" = betterproto.message_field(1002, group="step")
     decode: "steps.DecodeStep" = betterproto.message_field(1003, group="step")
     custom: "steps.CustomStep" = betterproto.message_field(1004, group="step")
-    wasm_id: str = betterproto.string_field(10000)
-    """WASM module ID (set by snitch-server)"""
-
-    wasm_bytes: bytes = betterproto.bytes_field(10001)
+    wasm_bytes: Optional[bytes] = betterproto.bytes_field(
+        10001, optional=True, group="X_wasm_bytes"
+    )
     """WASM module bytes (set by snitch-server)"""
 
-    wasm_function: str = betterproto.string_field(10002)
+    wasm_function: Optional[str] = betterproto.string_field(
+        10002, optional=True, group="X_wasm_function"
+    )
     """WASM function name to execute (set by snitch-server)"""
 
 
 @dataclass(eq=False, repr=False)
 class ServiceInfo(betterproto.Message):
     name: str = betterproto.string_field(1)
     description: str = betterproto.string_field(2)
```

### Comparing `snitch-protos-0.0.56/snitch_protos/protos/steps/__init__.py` & `snitch-protos-0.0.57/snitch_protos/protos/steps/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,17 @@
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
 # sources: steps/custom.proto, steps/decode.proto, steps/detective.proto, steps/encode.proto, steps/transform.proto
 # plugin: python-betterproto
 # This file has been @generated
 
 from dataclasses import dataclass
-from typing import List
+from typing import (
+    List,
+    Optional,
+)
 
 import betterproto
 
 
 class DetectiveType(betterproto.Enum):
     DETECTIVE_TYPE_UNKNOWN = 0
     DETECTIVE_TYPE_IS_EMPTY = 1000
@@ -138,17 +141,17 @@
     """WIP"""
 
     id: str = betterproto.string_field(1)
 
 
 @dataclass(eq=False, repr=False)
 class DetectiveStep(betterproto.Message):
-    path: str = betterproto.string_field(1)
+    path: Optional[str] = betterproto.string_field(1, optional=True, group="_path")
     args: List[str] = betterproto.string_field(2)
-    negate: bool = betterproto.bool_field(3)
+    negate: Optional[bool] = betterproto.bool_field(3, optional=True, group="_negate")
     type: "DetectiveType" = betterproto.enum_field(4)
 
 
 @dataclass(eq=False, repr=False)
 class EncodeStep(betterproto.Message):
     """WIP"""
```

### Comparing `snitch-protos-0.0.56/snitch_protos.egg-info/PKG-INFO` & `snitch-protos-0.0.57/snitch_protos.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: snitch-protos
-Version: 0.0.56
+Version: 0.0.57
 Summary: Protobuf python package for Streamdal.com Snitch
 Home-page: https://github.com/streamdal/snitch-protos
 Author: Streamdal.com
 Author-email: engineering@streamdal.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 1 - Planning
```


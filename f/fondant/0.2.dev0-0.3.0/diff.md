# Comparing `tmp/fondant-0.2.dev0.tar.gz` & `tmp/fondant-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fondant-0.2.dev0.tar", max compression
+gzip compressed data, was "fondant-0.3.0.tar", max compression
```

## Comparing `fondant-0.2.dev0.tar` & `fondant-0.3.0.tar`

### file list

```diff
@@ -1,18 +1,41 @@
--rw-r--r--   0        0        0    11356 2023-04-14 09:12:43.912402 fondant-0.2.dev0/LICENSE
--rw-r--r--   0        0        0     4290 2023-04-14 09:23:54.059098 fondant-0.2.dev0/README.md
--rw-r--r--   0        0        0        0 2023-04-14 09:12:43.929663 fondant-0.2.dev0/fondant/__init__.py
--rw-r--r--   0        0        0        1 2023-04-14 09:12:43.929762 fondant-0.2.dev0/fondant/components/__init__.py
--rw-r--r--   0        0        0    17668 2023-04-14 09:15:10.579020 fondant-0.2.dev0/fondant/components/common.py
--rw-r--r--   0        0        0     5456 2023-04-14 09:15:05.225089 fondant-0.2.dev0/fondant/components/hf_datasets_components.py
--rw-r--r--   0        0        0     4697 2023-04-14 09:15:06.732962 fondant-0.2.dev0/fondant/components/pandas_components.py
--rw-r--r--   0        0        0      342 2023-04-14 09:16:45.591739 fondant-0.2.dev0/fondant/exceptions.py
--rw-r--r--   0        0        0     5287 2023-04-14 09:19:51.255014 fondant-0.2.dev0/fondant/gcp_storage.py
--rw-r--r--   0        0        0     2241 2023-04-14 09:12:43.930278 fondant-0.2.dev0/fondant/import_utils.py
--rw-r--r--   0        0        0      874 2023-04-14 09:12:43.930343 fondant-0.2.dev0/fondant/io.py
--rw-r--r--   0        0        0      605 2023-04-14 09:12:43.930408 fondant-0.2.dev0/fondant/logger.py
--rw-r--r--   0        0        0     6594 2023-04-14 09:21:24.391801 fondant-0.2.dev0/fondant/manifest.py
--rw-r--r--   0        0        0     1444 2023-04-14 09:20:04.669266 fondant-0.2.dev0/fondant/pipeline_utils.py
--rw-r--r--   0        0        0     1672 2023-04-14 09:12:43.930673 fondant-0.2.dev0/fondant/schemas/manifest.json
--rw-r--r--   0        0        0     4361 2023-04-14 09:12:43.930743 fondant-0.2.dev0/fondant/storage_interface.py
--rw-r--r--   0        0        0     2162 2023-04-14 09:26:06.225285 fondant-0.2.dev0/pyproject.toml
--rw-r--r--   0        0        0     6225 1970-01-01 00:00:00.000000 fondant-0.2.dev0/PKG-INFO
+-rw-r--r--   0        0        0    11356 2023-08-08 12:24:05.343488 fondant-0.3.0/LICENSE
+-rw-r--r--   0        0        0    18609 2023-08-08 12:24:05.343488 fondant-0.3.0/README.md
+-rw-r--r--   0        0        0     3463 2023-08-08 12:52:42.712477 fondant-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0      130 2023-08-08 12:24:05.395492 fondant-0.3.0/src/fondant/__init__.py
+-rw-r--r--   0        0        0     1445 2023-08-08 12:24:05.395492 fondant-0.3.0/src/fondant/abstract_component_test.py
+-rw-r--r--   0        0        0    11786 2023-08-08 12:24:05.395492 fondant-0.3.0/src/fondant/cli.py
+-rw-r--r--   0        0        0     7031 2023-08-08 12:24:05.395492 fondant-0.3.0/src/fondant/compiler.py
+-rw-r--r--   0        0        0     2047 2023-08-08 12:24:05.395492 fondant-0.3.0/src/fondant/component.py
+-rw-r--r--   0        0        0    12583 2023-08-08 12:24:05.395492 fondant-0.3.0/src/fondant/component_spec.py
+-rw-r--r--   0        0        0      603 2023-08-08 12:53:00.294260 fondant-0.3.0/src/fondant/components/caption_images/fondant_component.yaml
+-rw-r--r--   0        0        0     1172 2023-08-08 12:52:59.642191 fondant-0.3.0/src/fondant/components/download_images/fondant_component.yaml
+-rw-r--r--   0        0        0      777 2023-08-08 12:53:00.438275 fondant-0.3.0/src/fondant/components/embedding_based_laion_retrieval/fondant_component.yaml
+-rw-r--r--   0        0        0      429 2023-08-08 12:53:00.538285 fondant-0.3.0/src/fondant/components/filter_comments/fondant_component.yaml
+-rw-r--r--   0        0        0      420 2023-08-08 12:53:00.094239 fondant-0.3.0/src/fondant/components/filter_image_resolution/fondant_component.yaml
+-rw-r--r--   0        0        0      616 2023-08-08 12:53:00.194249 fondant-0.3.0/src/fondant/components/filter_line_length/fondant_component.yaml
+-rw-r--r--   0        0        0      750 2023-08-08 12:52:59.990228 fondant-0.3.0/src/fondant/components/image_cropping/fondant_component.yaml
+-rw-r--r--   0        0        0      560 2023-08-08 12:52:59.890217 fondant-0.3.0/src/fondant/components/image_embedding/fondant_component.yaml
+-rw-r--r--   0        0        0      364 2023-08-08 12:53:00.246255 fondant-0.3.0/src/fondant/components/image_resolution_extraction/fondant_component.yaml
+-rw-r--r--   0        0        0      328 2023-08-08 12:52:59.838212 fondant-0.3.0/src/fondant/components/language_filter/fondant_component.yaml
+-rw-r--r--   0        0        0      345 2023-08-08 12:52:59.690196 fondant-0.3.0/src/fondant/components/load_from_files/fondant_component.yaml
+-rw-r--r--   0        0        0      845 2023-08-08 12:53:00.146244 fondant-0.3.0/src/fondant/components/load_from_hf_hub/fondant_component.yaml
+-rw-r--r--   0        0        0      426 2023-08-08 12:53:00.390270 fondant-0.3.0/src/fondant/components/minhash_generator/fondant_component.yaml
+-rw-r--r--   0        0        0      352 2023-08-08 12:53:00.046234 fondant-0.3.0/src/fondant/components/pii_redaction/fondant_component.yaml
+-rw-r--r--   0        0        0      894 2023-08-08 12:52:59.742202 fondant-0.3.0/src/fondant/components/prompt_based_laion_retrieval/fondant_component.yaml
+-rw-r--r--   0        0        0      528 2023-08-08 12:52:59.942223 fondant-0.3.0/src/fondant/components/segment_images/fondant_component.yaml
+-rw-r--r--   0        0        0      372 2023-08-08 12:53:00.342265 fondant-0.3.0/src/fondant/components/text_length_filter/fondant_component.yaml
+-rw-r--r--   0        0        0      452 2023-08-08 12:52:59.790207 fondant-0.3.0/src/fondant/components/text_normalization/fondant_component.yaml
+-rw-r--r--   0        0        0      788 2023-08-08 12:53:00.490280 fondant-0.3.0/src/fondant/components/write_to_hf_hub/fondant_component.yaml
+-rw-r--r--   0        0        0    10551 2023-08-08 12:24:05.395492 fondant-0.3.0/src/fondant/data_io.py
+-rw-r--r--   0        0        0      733 2023-08-08 12:24:05.395492 fondant-0.3.0/src/fondant/exceptions.py
+-rw-r--r--   0        0        0    15570 2023-08-08 12:24:05.395492 fondant-0.3.0/src/fondant/executor.py
+-rw-r--r--   0        0        0     1636 2023-08-08 12:24:05.395492 fondant-0.3.0/src/fondant/explorer.py
+-rw-r--r--   0        0        0     1291 2023-08-08 12:24:05.395492 fondant-0.3.0/src/fondant/import_utils.py
+-rw-r--r--   0        0        0    10406 2023-08-08 12:24:05.395492 fondant-0.3.0/src/fondant/manifest.py
+-rw-r--r--   0        0        0    24690 2023-08-08 12:24:05.395492 fondant-0.3.0/src/fondant/pipeline.py
+-rw-r--r--   0        0        0      627 2023-08-08 12:24:05.395492 fondant-0.3.0/src/fondant/runner.py
+-rw-r--r--   0        0        0     5705 2023-08-08 12:24:05.395492 fondant-0.3.0/src/fondant/schema.py
+-rw-r--r--   0        0        0     1232 2023-08-08 12:24:05.395492 fondant-0.3.0/src/fondant/schemas/common.json
+-rw-r--r--   0        0        0     2050 2023-08-08 12:24:05.395492 fondant-0.3.0/src/fondant/schemas/component_spec.json
+-rw-r--r--   0        0        0     1251 2023-08-08 12:24:05.395492 fondant-0.3.0/src/fondant/schemas/manifest.json
+-rw-r--r--   0        0        0    20478 1970-01-01 00:00:00.000000 fondant-0.3.0/PKG-INFO
```

### Comparing `fondant-0.2.dev0/LICENSE` & `fondant-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `fondant-0.2.dev0/fondant/import_utils.py` & `fondant-0.3.0/src/fondant/import_utils.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,68 +1,41 @@
-"""
-Import utils
-"""
-import logging
-import importlib.util
+"""Import utils."""
 import importlib.metadata
-from pathlib import Path
+import importlib.util
+import logging
 import sys
+from pathlib import Path
 
 logger = logging.getLogger(__name__)
 
-PANDAS_IMPORT_ERROR = """
-`{0}` requires the pandas library but it was not found in your environment. Please install express
- using the 'pandas' extra.
-"""
-
-DATASETS_IMPORT_ERROR = """
-`{0}` requires the 🤗 Datasets library but it was not found in your environment.
-Please install express using the 'datasets' extra.
-Note that if you have a local folder named `datasets` or a local python file named
- `datasets.py` in your current working directory, python may try to import this instead of the 🤗 
- Datasets library. You should rename this folder or that python file if that's the case.
-  Please note that you may need to restart your runtime after installation.
-"""
-
 KFP_IMPORT_ERROR = """
 `{0}` requires the kubeflow pipelines (kfp) library but it was not found in your environment.
-Please install express using the 'pipelines' extra.
+Please install fondant using pip install fondant [pipelines].
 """
 
 
 def is_package_available(package_name: str, import_error_msg: str) -> bool:
     """
     Function that checks if a given package is available
     Args:
         package_name (str): the name of the package
         import_error_msg (str): the error message to return if the package is not found
     Returns:
-        bool: check if package is available
+        bool: check if package is available.
     """
-
     package_available = importlib.util.find_spec(package_name) is not None
 
     try:
         package_version = importlib.metadata.version(package_name)
         logger.debug(f"Successfully imported {package_name} version {package_version}")
     except importlib.metadata.PackageNotFoundError:
         package_available = False
 
     if package_available:
         return package_available
-    else:
-        raise ModuleNotFoundError(import_error_msg.format(Path(sys.argv[0]).stem))
-
-
-def is_datasets_available():
-    """Check if 'datasets' is available"""
-    return is_package_available("datasets", DATASETS_IMPORT_ERROR)
-
 
-def is_pandas_available():
-    """Check if 'pandas' is available"""
-    return is_package_available("pandas", PANDAS_IMPORT_ERROR)
+    raise ModuleNotFoundError(import_error_msg.format(Path(sys.argv[0]).stem))
 
 
 def is_kfp_available():
-    """Check if 'pandas' is available"""
+    """Check if 'pandas' is available."""
     return is_package_available("kfp", KFP_IMPORT_ERROR)
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `fondant-0.2.dev0/fondant/schemas/manifest.json` & `fondant-0.3.0/src/fondant/schemas/common.json`

 * *Files 16% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.13666666666666666%*

 * *Differences: {"'definitions'": "{'field': {'properties': {'type': {'$ref': '#/definitions/subset_data_type', "*

 * *                  "delete: ['enum']}, 'items': OrderedDict([('oneOf', [OrderedDict([('$ref', "*

 * *                  "'#/definitions/field')]), OrderedDict([('type', 'array'), ('items', "*

 * *                  "OrderedDict([('$ref', '#/definitions/field')]))])])])}, 'additionalProperties': "*

 * *                  "False}, 'subset_data_type': OrderedDict([('type', 'string'), ('enum', ['bool', "*

 * *                  "'int8', 'i […]*

```diff
@@ -1,38 +1,27 @@
 {
-    "$schema": "http://json-schema.org/draft-04/schema#",
     "definitions": {
         "field": {
+            "additionalProperties": false,
             "properties": {
+                "items": {
+                    "oneOf": [
+                        {
+                            "$ref": "#/definitions/field"
+                        },
+                        {
+                            "items": {
+                                "$ref": "#/definitions/field"
+                            },
+                            "type": "array"
+                        }
+                    ]
+                },
                 "type": {
-                    "enum": [
-                        "bool",
-                        "int8",
-                        "int16",
-                        "int32",
-                        "uint8",
-                        "uint16",
-                        "uint32",
-                        "uint64",
-                        "float16",
-                        "float32",
-                        "float64",
-                        "decimal",
-                        "time32",
-                        "time64",
-                        "timestamp",
-                        "date32",
-                        "date64",
-                        "duration",
-                        "utf8",
-                        "binary",
-                        "categorical",
-                        "list",
-                        "struct"
-                    ],
+                    "$ref": "#/definitions/subset_data_type",
                     "type": "string"
                 }
             },
             "required": [
                 "type"
             ],
             "type": "object"
@@ -40,65 +29,39 @@
         "fields": {
             "additionalProperties": {
                 "$ref": "#/definitions/field"
             },
             "minProperties": 1,
             "type": "object"
         },
-        "subset": {
-            "properties": {
-                "fields": {
-                    "$ref": "#/definitions/fields"
-                },
-                "location": {
-                    "pattern": "/.*",
-                    "type": "string"
-                }
-            },
-            "required": [
-                "location",
-                "fields"
+        "subset_data_type": {
+            "enum": [
+                "bool",
+                "int8",
+                "int16",
+                "int32",
+                "int64",
+                "uint8",
+                "uint16",
+                "uint32",
+                "uint64",
+                "float16",
+                "float32",
+                "float64",
+                "decimal",
+                "time32",
+                "time64",
+                "timestamp",
+                "date32",
+                "date64",
+                "duration",
+                "utf8",
+                "string",
+                "binary",
+                "list",
+                "struct",
+                "array"
             ],
-            "type": "object"
-        },
-        "subsets": {
-            "additionalProperties": {
-                "$ref": "#/definitions/subset"
-            },
-            "type": "object"
-        }
-    },
-    "properties": {
-        "index": {
-            "properties": {
-                "location": {
-                    "type": "string"
-                }
-            },
-            "required": [
-                "location"
-            ],
-            "type": "object"
-        },
-        "metadata": {
-            "properties": {
-                "base_path": {
-                    "format": "uri",
-                    "type": "string"
-                }
-            },
-            "required": [
-                "base_path"
-            ],
-            "type": "object"
-        },
-        "subsets": {
-            "$ref": "#/definitions/subsets"
+            "type": "string"
         }
-    },
-    "required": [
-        "metadata",
-        "index",
-        "subsets"
-    ],
-    "type": "object"
+    }
 }
```


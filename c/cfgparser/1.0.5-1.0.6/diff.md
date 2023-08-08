# Comparing `tmp/cfgparser-1.0.5.tar.gz` & `tmp/cfgparser-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cfgparser-1.0.5.tar", last modified: Mon Aug  7 02:55:16 2023, max compression
+gzip compressed data, was "cfgparser-1.0.6.tar", last modified: Tue Aug  8 03:52:31 2023, max compression
```

## Comparing `cfgparser-1.0.5.tar` & `cfgparser-1.0.6.tar`

### file list

```diff
@@ -1,25 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 02:55:16.794769 cfgparser-1.0.5/
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-08-07 02:55:07.000000 cfgparser-1.0.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3933 2023-08-07 02:55:16.794769 cfgparser-1.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2126 2023-08-07 02:55:07.000000 cfgparser-1.0.5/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-07 02:55:16.794769 cfgparser-1.0.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     7356 2023-08-07 02:55:07.000000 cfgparser-1.0.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 02:55:16.794769 cfgparser-1.0.5/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 02:55:16.794769 cfgparser-1.0.5/src/cfgparser/
--rw-r--r--   0 runner    (1001) docker     (123)     4774 2023-08-07 02:55:07.000000 cfgparser-1.0.5/src/cfgparser/config_parser.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 02:55:16.794769 cfgparser-1.0.5/src/cfgparser/io/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 02:55:07.000000 cfgparser-1.0.5/src/cfgparser/io/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      648 2023-08-07 02:55:07.000000 cfgparser-1.0.5/src/cfgparser/io/fileloader.py
--rw-r--r--   0 runner    (1001) docker     (123)      495 2023-08-07 02:55:07.000000 cfgparser-1.0.5/src/cfgparser/io/jsonfileloader.py
--rw-r--r--   0 runner    (1001) docker     (123)      500 2023-08-07 02:55:07.000000 cfgparser-1.0.5/src/cfgparser/io/yamlfileloader.py
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-08-07 02:55:07.000000 cfgparser-1.0.5/src/cfgparser/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 02:55:16.794769 cfgparser-1.0.5/src/cfgparser/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 02:55:07.000000 cfgparser-1.0.5/src/cfgparser/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      591 2023-08-07 02:55:07.000000 cfgparser-1.0.5/src/cfgparser/utils/dynamic_type_loader.py
--rw-r--r--   0 runner    (1001) docker     (123)      447 2023-08-07 02:55:07.000000 cfgparser-1.0.5/src/cfgparser/utils/execution_timer.py
--rw-r--r--   0 runner    (1001) docker     (123)      192 2023-08-07 02:55:07.000000 cfgparser-1.0.5/src/cfgparser/utils/union_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 02:55:16.794769 cfgparser-1.0.5/src/cfgparser.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3933 2023-08-07 02:55:16.000000 cfgparser-1.0.5/src/cfgparser.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      512 2023-08-07 02:55:16.000000 cfgparser-1.0.5/src/cfgparser.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-07 02:55:16.000000 cfgparser-1.0.5/src/cfgparser.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-08-07 02:55:16.000000 cfgparser-1.0.5/src/cfgparser.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 03:52:31.974974 cfgparser-1.0.6/
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-08-08 03:52:21.000000 cfgparser-1.0.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3933 2023-08-08 03:52:31.974974 cfgparser-1.0.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2126 2023-08-08 03:52:21.000000 cfgparser-1.0.6/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-08 03:52:31.978974 cfgparser-1.0.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     7356 2023-08-08 03:52:21.000000 cfgparser-1.0.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 03:52:31.970974 cfgparser-1.0.6/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 03:52:31.970974 cfgparser-1.0.6/src/cfgparser/
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-08-08 03:52:21.000000 cfgparser-1.0.6/src/cfgparser/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4744 2023-08-08 03:52:21.000000 cfgparser-1.0.6/src/cfgparser/config_parser.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 03:52:31.974974 cfgparser-1.0.6/src/cfgparser/io/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 03:52:21.000000 cfgparser-1.0.6/src/cfgparser/io/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      648 2023-08-08 03:52:21.000000 cfgparser-1.0.6/src/cfgparser/io/fileloader.py
+-rw-r--r--   0 runner    (1001) docker     (123)      495 2023-08-08 03:52:21.000000 cfgparser-1.0.6/src/cfgparser/io/jsonfileloader.py
+-rw-r--r--   0 runner    (1001) docker     (123)      500 2023-08-08 03:52:21.000000 cfgparser-1.0.6/src/cfgparser/io/yamlfileloader.py
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-08-08 03:52:21.000000 cfgparser-1.0.6/src/cfgparser/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 03:52:31.974974 cfgparser-1.0.6/src/cfgparser/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 03:52:21.000000 cfgparser-1.0.6/src/cfgparser/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      591 2023-08-08 03:52:21.000000 cfgparser-1.0.6/src/cfgparser/utils/dynamic_type_loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)      447 2023-08-08 03:52:21.000000 cfgparser-1.0.6/src/cfgparser/utils/execution_timer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      192 2023-08-08 03:52:21.000000 cfgparser-1.0.6/src/cfgparser/utils/union_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 03:52:31.974974 cfgparser-1.0.6/src/cfgparser.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3933 2023-08-08 03:52:31.000000 cfgparser-1.0.6/src/cfgparser.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      538 2023-08-08 03:52:31.000000 cfgparser-1.0.6/src/cfgparser.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 03:52:31.000000 cfgparser-1.0.6/src/cfgparser.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-08-08 03:52:31.000000 cfgparser-1.0.6/src/cfgparser.egg-info/top_level.txt
```

### Comparing `cfgparser-1.0.5/LICENSE` & `cfgparser-1.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `cfgparser-1.0.5/PKG-INFO` & `cfgparser-1.0.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cfgparser
-Version: 1.0.5
+Version: 1.0.6
 Summary: Python package that allows to parse typed configs defined by python dataclasses
 Home-page: https://github.com/CaRniFeXeR/PythonConfigParser
 Author: Florian Kowarsch
 Author-email: flo.kowarsch@yahoo.de
 License: UNKNOWN
 Project-URL: Bug Reports, https://github.com/CaRniFeXeR/PythonConfigParser/issues
 Project-URL: Source, https://github.com/CaRniFeXeR/PythonConfigParser/
```

### Comparing `cfgparser-1.0.5/README.md` & `cfgparser-1.0.6/README.md`

 * *Files identical despite different names*

### Comparing `cfgparser-1.0.5/setup.py` & `cfgparser-1.0.6/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -31,15 +31,15 @@
     name="cfgparser",  # Required
     # Versions should comply with PEP 440:
     # https://www.python.org/dev/peps/pep-0440/
     #
     # For a discussion on single-sourcing the version across setup.py and the
     # project code, see
     # https://packaging.python.org/guides/single-sourcing-package-version/
-    version="1.0.5",  # Required
+    version="1.0.6",  # Required
     # This is a one-line description or tagline of what your project does. This
     # corresponds to the "Summary" metadata field:
     # https://packaging.python.org/specifications/core-metadata/#summary
     description="Python package that allows to parse typed configs defined by python dataclasses",  # Optional
     # This is an optional longer description of your project that represents
     # the body of text which users will see when they visit PyPI.
     #
```

### Comparing `cfgparser-1.0.5/src/cfgparser/config_parser.py` & `cfgparser-1.0.6/src/cfgparser/config_parser.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from typing import Type
 import typing
-from src.cfgparser.io.yamlfileloader import YamlFileLoader
+from .io.yamlfileloader import YamlFileLoader
 
-from src.cfgparser.utils.union_handler import is_union_type
-from src.cfgparser import settings
+from .utils.union_handler import is_union_type
+from . import settings
 from .io.jsonfileloader import JsonFileLoader
 from pathlib import Path
 from enum import Enum
 import inspect
 
 
 
@@ -19,15 +19,15 @@
     """
 
     def __init__(self, datastructure_module_name: str = "src.datastructures") -> None:
         self.datastructure_module_name = datastructure_module_name
 
     def parse_from_file(self, config_path: Path):
         """
-        loads a json config from the specified location and parses it into a typed object based on the type specified in 'type_name'
+        loads a json or yaml config from the specified location and parses it into a typed object based on the type specified in 'type_name'
         """
 
         if isinstance(config_path, str):
             config_path = Path(config_path)
         elif not isinstance(config_path, Path):
             raise TypeError("'config_path' must be a str or Path")
```

### Comparing `cfgparser-1.0.5/src/cfgparser/io/fileloader.py` & `cfgparser-1.0.6/src/cfgparser/io/fileloader.py`

 * *Files identical despite different names*

### Comparing `cfgparser-1.0.5/src/cfgparser/utils/dynamic_type_loader.py` & `cfgparser-1.0.6/src/cfgparser/utils/dynamic_type_loader.py`

 * *Files identical despite different names*

### Comparing `cfgparser-1.0.5/src/cfgparser.egg-info/PKG-INFO` & `cfgparser-1.0.6/src/cfgparser.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cfgparser
-Version: 1.0.5
+Version: 1.0.6
 Summary: Python package that allows to parse typed configs defined by python dataclasses
 Home-page: https://github.com/CaRniFeXeR/PythonConfigParser
 Author: Florian Kowarsch
 Author-email: flo.kowarsch@yahoo.de
 License: UNKNOWN
 Project-URL: Bug Reports, https://github.com/CaRniFeXeR/PythonConfigParser/issues
 Project-URL: Source, https://github.com/CaRniFeXeR/PythonConfigParser/
```

### Comparing `cfgparser-1.0.5/src/cfgparser.egg-info/SOURCES.txt` & `cfgparser-1.0.6/src/cfgparser.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 LICENSE
 README.md
 setup.py
+src/cfgparser/__init__.py
 src/cfgparser/config_parser.py
 src/cfgparser/settings.py
 src/cfgparser.egg-info/PKG-INFO
 src/cfgparser.egg-info/SOURCES.txt
 src/cfgparser.egg-info/dependency_links.txt
 src/cfgparser.egg-info/top_level.txt
 src/cfgparser/io/__init__.py
```


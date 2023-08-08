# Comparing `tmp/types-aiobotocore-lex-models-2.5.2.post2.tar.gz` & `tmp/types-aiobotocore-lex-models-2.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-lex-models-2.5.2.post2.tar", last modified: Fri Aug  4 13:59:15 2023, max compression
+gzip compressed data, was "types-aiobotocore-lex-models-2.5.4.tar", last modified: Tue Aug  8 01:23:59 2023, max compression
```

## Comparing `types-aiobotocore-lex-models-2.5.2.post2.tar` & `types-aiobotocore-lex-models-2.5.4.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:15.046643 types-aiobotocore-lex-models-2.5.2.post2/
--rw-r--r--   0 vlad      (1000) vlad      (1000)     1070 2023-08-04 13:42:30.000000 types-aiobotocore-lex-models-2.5.2.post2/LICENSE
--rw-r--r--   0 vlad      (1000) vlad      (1000)    14486 2023-08-04 13:59:15.046643 types-aiobotocore-lex-models-2.5.2.post2/PKG-INFO
--rw-r--r--   0 vlad      (1000) vlad      (1000)    12943 2023-08-04 13:42:30.000000 types-aiobotocore-lex-models-2.5.2.post2/README.md
--rw-r--r--   0 vlad      (1000) vlad      (1000)       38 2023-08-04 13:59:15.046643 types-aiobotocore-lex-models-2.5.2.post2/setup.cfg
--rw-r--r--   0 vlad      (1000) vlad      (1000)     2106 2023-08-04 13:42:30.000000 types-aiobotocore-lex-models-2.5.2.post2/setup.py
-drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:15.046643 types-aiobotocore-lex-models-2.5.2.post2/types_aiobotocore_lex_models/
--rw-r--r--   0 vlad      (1000) vlad      (1000)     2570 2023-08-04 13:42:30.000000 types-aiobotocore-lex-models-2.5.2.post2/types_aiobotocore_lex_models/__init__.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)     2569 2023-08-04 13:42:30.000000 types-aiobotocore-lex-models-2.5.2.post2/types_aiobotocore_lex_models/__init__.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)      981 2023-08-04 13:42:30.000000 types-aiobotocore-lex-models-2.5.2.post2/types_aiobotocore_lex_models/__main__.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)    37313 2023-08-04 13:42:30.000000 types-aiobotocore-lex-models-2.5.2.post2/types_aiobotocore_lex_models/client.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)    37252 2023-08-04 13:42:30.000000 types-aiobotocore-lex-models-2.5.2.post2/types_aiobotocore_lex_models/client.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)    11245 2023-08-04 13:42:30.000000 types-aiobotocore-lex-models-2.5.2.post2/types_aiobotocore_lex_models/literals.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)    11243 2023-08-04 13:42:30.000000 types-aiobotocore-lex-models-2.5.2.post2/types_aiobotocore_lex_models/literals.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)    12667 2023-08-04 13:42:30.000000 types-aiobotocore-lex-models-2.5.2.post2/types_aiobotocore_lex_models/paginator.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)    12655 2023-08-04 13:42:30.000000 types-aiobotocore-lex-models-2.5.2.post2/types_aiobotocore_lex_models/paginator.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:42:30.000000 types-aiobotocore-lex-models-2.5.2.post2/types_aiobotocore_lex_models/py.typed
--rw-r--r--   0 vlad      (1000) vlad      (1000)    46018 2023-08-04 13:42:32.000000 types-aiobotocore-lex-models-2.5.2.post2/types_aiobotocore_lex_models/type_defs.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)    45965 2023-08-04 13:42:32.000000 types-aiobotocore-lex-models-2.5.2.post2/types_aiobotocore_lex_models/type_defs.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)       65 2023-08-04 13:42:30.000000 types-aiobotocore-lex-models-2.5.2.post2/types_aiobotocore_lex_models/version.py
-drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:15.046643 types-aiobotocore-lex-models-2.5.2.post2/types_aiobotocore_lex_models.egg-info/
--rw-r--r--   0 vlad      (1000) vlad      (1000)    14486 2023-08-04 13:59:14.000000 types-aiobotocore-lex-models-2.5.2.post2/types_aiobotocore_lex_models.egg-info/PKG-INFO
--rw-r--r--   0 vlad      (1000) vlad      (1000)      870 2023-08-04 13:59:14.000000 types-aiobotocore-lex-models-2.5.2.post2/types_aiobotocore_lex_models.egg-info/SOURCES.txt
--rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:14.000000 types-aiobotocore-lex-models-2.5.2.post2/types_aiobotocore_lex_models.egg-info/dependency_links.txt
--rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:14.000000 types-aiobotocore-lex-models-2.5.2.post2/types_aiobotocore_lex_models.egg-info/not-zip-safe
--rw-r--r--   0 vlad      (1000) vlad      (1000)       52 2023-08-04 13:59:14.000000 types-aiobotocore-lex-models-2.5.2.post2/types_aiobotocore_lex_models.egg-info/requires.txt
--rw-r--r--   0 vlad      (1000) vlad      (1000)       29 2023-08-04 13:59:14.000000 types-aiobotocore-lex-models-2.5.2.post2/types_aiobotocore_lex_models.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:23:59.594722 types-aiobotocore-lex-models-2.5.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-08 01:13:54.000000 types-aiobotocore-lex-models-2.5.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    14480 2023-08-08 01:23:59.594722 types-aiobotocore-lex-models-2.5.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    12943 2023-08-08 01:13:54.000000 types-aiobotocore-lex-models-2.5.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-08 01:23:59.594722 types-aiobotocore-lex-models-2.5.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2100 2023-08-08 01:13:54.000000 types-aiobotocore-lex-models-2.5.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:23:59.594722 types-aiobotocore-lex-models-2.5.4/types_aiobotocore_lex_models/
+-rw-r--r--   0 runner    (1001) docker     (123)     2570 2023-08-08 01:13:54.000000 types-aiobotocore-lex-models-2.5.4/types_aiobotocore_lex_models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2569 2023-08-08 01:13:54.000000 types-aiobotocore-lex-models-2.5.4/types_aiobotocore_lex_models/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      969 2023-08-08 01:13:54.000000 types-aiobotocore-lex-models-2.5.4/types_aiobotocore_lex_models/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37313 2023-08-08 01:13:54.000000 types-aiobotocore-lex-models-2.5.4/types_aiobotocore_lex_models/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37252 2023-08-08 01:13:54.000000 types-aiobotocore-lex-models-2.5.4/types_aiobotocore_lex_models/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    11245 2023-08-08 01:13:54.000000 types-aiobotocore-lex-models-2.5.4/types_aiobotocore_lex_models/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11243 2023-08-08 01:13:54.000000 types-aiobotocore-lex-models-2.5.4/types_aiobotocore_lex_models/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    12667 2023-08-08 01:13:54.000000 types-aiobotocore-lex-models-2.5.4/types_aiobotocore_lex_models/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12655 2023-08-08 01:13:54.000000 types-aiobotocore-lex-models-2.5.4/types_aiobotocore_lex_models/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 01:13:54.000000 types-aiobotocore-lex-models-2.5.4/types_aiobotocore_lex_models/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    46018 2023-08-08 01:13:55.000000 types-aiobotocore-lex-models-2.5.4/types_aiobotocore_lex_models/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    45965 2023-08-08 01:13:55.000000 types-aiobotocore-lex-models-2.5.4/types_aiobotocore_lex_models/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-08-08 01:13:54.000000 types-aiobotocore-lex-models-2.5.4/types_aiobotocore_lex_models/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:23:59.594722 types-aiobotocore-lex-models-2.5.4/types_aiobotocore_lex_models.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    14480 2023-08-08 01:23:59.000000 types-aiobotocore-lex-models-2.5.4/types_aiobotocore_lex_models.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      870 2023-08-08 01:23:59.000000 types-aiobotocore-lex-models-2.5.4/types_aiobotocore_lex_models.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 01:23:59.000000 types-aiobotocore-lex-models-2.5.4/types_aiobotocore_lex_models.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 01:23:59.000000 types-aiobotocore-lex-models-2.5.4/types_aiobotocore_lex_models.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-08 01:23:59.000000 types-aiobotocore-lex-models-2.5.4/types_aiobotocore_lex_models.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-08-08 01:23:59.000000 types-aiobotocore-lex-models-2.5.4/types_aiobotocore_lex_models.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-lex-models-2.5.2.post2/LICENSE` & `types-aiobotocore-lex-models-2.5.4/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-lex-models-2.5.2.post2/PKG-INFO` & `types-aiobotocore-lex-models-2.5.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-lex-models
-Version: 2.5.2.post2
-Summary: Type annotations for aiobotocore.LexModelBuildingService 2.5.2 service generated with mypy-boto3-builder 7.17.2
+Version: 2.5.4
+Summary: Type annotations for aiobotocore.LexModelBuildingService 2.5.4 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lex_models/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-lex-models.svg?color=blue)](https://pypi.org/project/types-aiobotocore-lex-models)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lex_models/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-lex-models)](https://pepy.tech/project/types-aiobotocore-lex-models)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.LexModelBuildingService 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lex-models.html#LexModelBuildingService)
+[aiobotocore.LexModelBuildingService 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lex-models.html#LexModelBuildingService)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-lex-models-2.5.2.post2/README.md` & `types-aiobotocore-lex-models-2.5.4/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-lex-models.svg?color=blue)](https://pypi.org/project/types-aiobotocore-lex-models)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lex_models/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-lex-models)](https://pepy.tech/project/types-aiobotocore-lex-models)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.LexModelBuildingService 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lex-models.html#LexModelBuildingService)
+[aiobotocore.LexModelBuildingService 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lex-models.html#LexModelBuildingService)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-lex-models-2.5.2.post2/setup.py` & `types-aiobotocore-lex-models-2.5.4/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-lex-models",
-    version="2.5.2.post2",
+    version="2.5.4",
     packages=["types_aiobotocore_lex_models"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.LexModelBuildingService 2.5.2 service generated with"
+        "Type annotations for aiobotocore.LexModelBuildingService 2.5.4 service generated with"
         " mypy-boto3-builder 7.17.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
```

### Comparing `types-aiobotocore-lex-models-2.5.2.post2/types_aiobotocore_lex_models/__init__.py` & `types-aiobotocore-lex-models-2.5.4/types_aiobotocore_lex_models/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-lex-models-2.5.2.post2/types_aiobotocore_lex_models/__init__.pyi` & `types-aiobotocore-lex-models-2.5.4/types_aiobotocore_lex_models/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-lex-models-2.5.2.post2/types_aiobotocore_lex_models/__main__.py` & `types-aiobotocore-lex-models-2.5.4/types_aiobotocore_lex_models/__main__.py`

 * *Files 16% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.LexModelBuildingService 2.5.2\nVersion:        "
-        " 2.5.2.post2\nBuilder version: 7.17.2\nDocs:           "
+        "Type annotations for aiobotocore.LexModelBuildingService 2.5.4\nVersion:        "
+        " 2.5.4\nBuilder version: 7.17.2\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lex_models//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lex-models.html#LexModelBuildingService\nOther"
         " services:  https://pypi.org/project/boto3-stubs/\nChangelog:      "
         " https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("2.5.2.post2")
+    print("2.5.4")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `types-aiobotocore-lex-models-2.5.2.post2/types_aiobotocore_lex_models/client.py` & `types-aiobotocore-lex-models-2.5.4/types_aiobotocore_lex_models/client.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-lex-models-2.5.2.post2/types_aiobotocore_lex_models/client.pyi` & `types-aiobotocore-lex-models-2.5.4/types_aiobotocore_lex_models/client.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-lex-models-2.5.2.post2/types_aiobotocore_lex_models/literals.py` & `types-aiobotocore-lex-models-2.5.4/types_aiobotocore_lex_models/literals.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-lex-models-2.5.2.post2/types_aiobotocore_lex_models/literals.pyi` & `types-aiobotocore-lex-models-2.5.4/types_aiobotocore_lex_models/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-lex-models-2.5.2.post2/types_aiobotocore_lex_models/paginator.py` & `types-aiobotocore-lex-models-2.5.4/types_aiobotocore_lex_models/paginator.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-lex-models-2.5.2.post2/types_aiobotocore_lex_models/paginator.pyi` & `types-aiobotocore-lex-models-2.5.4/types_aiobotocore_lex_models/paginator.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-lex-models-2.5.2.post2/types_aiobotocore_lex_models/type_defs.py` & `types-aiobotocore-lex-models-2.5.4/types_aiobotocore_lex_models/type_defs.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-lex-models-2.5.2.post2/types_aiobotocore_lex_models/type_defs.pyi` & `types-aiobotocore-lex-models-2.5.4/types_aiobotocore_lex_models/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-lex-models-2.5.2.post2/types_aiobotocore_lex_models.egg-info/PKG-INFO` & `types-aiobotocore-lex-models-2.5.4/types_aiobotocore_lex_models.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-lex-models
-Version: 2.5.2.post2
-Summary: Type annotations for aiobotocore.LexModelBuildingService 2.5.2 service generated with mypy-boto3-builder 7.17.2
+Version: 2.5.4
+Summary: Type annotations for aiobotocore.LexModelBuildingService 2.5.4 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lex_models/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-lex-models.svg?color=blue)](https://pypi.org/project/types-aiobotocore-lex-models)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lex_models/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-lex-models)](https://pepy.tech/project/types-aiobotocore-lex-models)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.LexModelBuildingService 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lex-models.html#LexModelBuildingService)
+[aiobotocore.LexModelBuildingService 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lex-models.html#LexModelBuildingService)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-lex-models-2.5.2.post2/types_aiobotocore_lex_models.egg-info/SOURCES.txt` & `types-aiobotocore-lex-models-2.5.4/types_aiobotocore_lex_models.egg-info/SOURCES.txt`

 * *Files identical despite different names*


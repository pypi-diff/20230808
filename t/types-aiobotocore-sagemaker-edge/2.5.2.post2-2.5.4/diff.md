# Comparing `tmp/types-aiobotocore-sagemaker-edge-2.5.2.post2.tar.gz` & `tmp/types-aiobotocore-sagemaker-edge-2.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-sagemaker-edge-2.5.2.post2.tar", last modified: Fri Aug  4 13:59:25 2023, max compression
+gzip compressed data, was "types-aiobotocore-sagemaker-edge-2.5.4.tar", last modified: Tue Aug  8 01:24:22 2023, max compression
```

## Comparing `types-aiobotocore-sagemaker-edge-2.5.2.post2.tar` & `types-aiobotocore-sagemaker-edge-2.5.4.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:25.066643 types-aiobotocore-sagemaker-edge-2.5.2.post2/
--rw-r--r--   0 vlad      (1000) vlad      (1000)     1070 2023-08-04 13:52:25.000000 types-aiobotocore-sagemaker-edge-2.5.2.post2/LICENSE
--rw-r--r--   0 vlad      (1000) vlad      (1000)    12597 2023-08-04 13:59:25.066643 types-aiobotocore-sagemaker-edge-2.5.2.post2/PKG-INFO
--rw-r--r--   0 vlad      (1000) vlad      (1000)    11045 2023-08-04 13:52:25.000000 types-aiobotocore-sagemaker-edge-2.5.2.post2/README.md
--rw-r--r--   0 vlad      (1000) vlad      (1000)       38 2023-08-04 13:59:25.066643 types-aiobotocore-sagemaker-edge-2.5.2.post2/setup.cfg
--rw-r--r--   0 vlad      (1000) vlad      (1000)     2127 2023-08-04 13:52:24.000000 types-aiobotocore-sagemaker-edge-2.5.2.post2/setup.py
-drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:25.066643 types-aiobotocore-sagemaker-edge-2.5.2.post2/types_aiobotocore_sagemaker_edge/
--rw-r--r--   0 vlad      (1000) vlad      (1000)      528 2023-08-04 13:52:25.000000 types-aiobotocore-sagemaker-edge-2.5.2.post2/types_aiobotocore_sagemaker_edge/__init__.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)      527 2023-08-04 13:52:25.000000 types-aiobotocore-sagemaker-edge-2.5.2.post2/types_aiobotocore_sagemaker_edge/__init__.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)      983 2023-08-04 13:52:25.000000 types-aiobotocore-sagemaker-edge-2.5.2.post2/types_aiobotocore_sagemaker_edge/__main__.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)     6228 2023-08-04 13:52:25.000000 types-aiobotocore-sagemaker-edge-2.5.2.post2/types_aiobotocore_sagemaker_edge/client.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)     6217 2023-08-04 13:52:25.000000 types-aiobotocore-sagemaker-edge-2.5.2.post2/types_aiobotocore_sagemaker_edge/client.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)     8169 2023-08-04 13:52:25.000000 types-aiobotocore-sagemaker-edge-2.5.2.post2/types_aiobotocore_sagemaker_edge/literals.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)     8167 2023-08-04 13:52:25.000000 types-aiobotocore-sagemaker-edge-2.5.2.post2/types_aiobotocore_sagemaker_edge/literals.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:52:25.000000 types-aiobotocore-sagemaker-edge-2.5.2.post2/types_aiobotocore_sagemaker_edge/py.typed
--rw-r--r--   0 vlad      (1000) vlad      (1000)     4886 2023-08-04 13:52:25.000000 types-aiobotocore-sagemaker-edge-2.5.2.post2/types_aiobotocore_sagemaker_edge/type_defs.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)     4884 2023-08-04 13:52:25.000000 types-aiobotocore-sagemaker-edge-2.5.2.post2/types_aiobotocore_sagemaker_edge/type_defs.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)       65 2023-08-04 13:52:25.000000 types-aiobotocore-sagemaker-edge-2.5.2.post2/types_aiobotocore_sagemaker_edge/version.py
-drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:25.066643 types-aiobotocore-sagemaker-edge-2.5.2.post2/types_aiobotocore_sagemaker_edge.egg-info/
--rw-r--r--   0 vlad      (1000) vlad      (1000)    12597 2023-08-04 13:59:24.000000 types-aiobotocore-sagemaker-edge-2.5.2.post2/types_aiobotocore_sagemaker_edge.egg-info/PKG-INFO
--rw-r--r--   0 vlad      (1000) vlad      (1000)      853 2023-08-04 13:59:24.000000 types-aiobotocore-sagemaker-edge-2.5.2.post2/types_aiobotocore_sagemaker_edge.egg-info/SOURCES.txt
--rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:24.000000 types-aiobotocore-sagemaker-edge-2.5.2.post2/types_aiobotocore_sagemaker_edge.egg-info/dependency_links.txt
--rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:24.000000 types-aiobotocore-sagemaker-edge-2.5.2.post2/types_aiobotocore_sagemaker_edge.egg-info/not-zip-safe
--rw-r--r--   0 vlad      (1000) vlad      (1000)       52 2023-08-04 13:59:24.000000 types-aiobotocore-sagemaker-edge-2.5.2.post2/types_aiobotocore_sagemaker_edge.egg-info/requires.txt
--rw-r--r--   0 vlad      (1000) vlad      (1000)       33 2023-08-04 13:59:24.000000 types-aiobotocore-sagemaker-edge-2.5.2.post2/types_aiobotocore_sagemaker_edge.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:24:22.742771 types-aiobotocore-sagemaker-edge-2.5.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-08 01:20:26.000000 types-aiobotocore-sagemaker-edge-2.5.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    12591 2023-08-08 01:24:22.742771 types-aiobotocore-sagemaker-edge-2.5.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    11045 2023-08-08 01:20:26.000000 types-aiobotocore-sagemaker-edge-2.5.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-08 01:24:22.742771 types-aiobotocore-sagemaker-edge-2.5.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2121 2023-08-08 01:20:25.000000 types-aiobotocore-sagemaker-edge-2.5.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:24:22.742771 types-aiobotocore-sagemaker-edge-2.5.4/types_aiobotocore_sagemaker_edge/
+-rw-r--r--   0 runner    (1001) docker     (123)      528 2023-08-08 01:20:26.000000 types-aiobotocore-sagemaker-edge-2.5.4/types_aiobotocore_sagemaker_edge/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      527 2023-08-08 01:20:26.000000 types-aiobotocore-sagemaker-edge-2.5.4/types_aiobotocore_sagemaker_edge/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      971 2023-08-08 01:20:26.000000 types-aiobotocore-sagemaker-edge-2.5.4/types_aiobotocore_sagemaker_edge/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6228 2023-08-08 01:20:26.000000 types-aiobotocore-sagemaker-edge-2.5.4/types_aiobotocore_sagemaker_edge/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6217 2023-08-08 01:20:26.000000 types-aiobotocore-sagemaker-edge-2.5.4/types_aiobotocore_sagemaker_edge/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8169 2023-08-08 01:20:26.000000 types-aiobotocore-sagemaker-edge-2.5.4/types_aiobotocore_sagemaker_edge/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8167 2023-08-08 01:20:26.000000 types-aiobotocore-sagemaker-edge-2.5.4/types_aiobotocore_sagemaker_edge/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 01:20:26.000000 types-aiobotocore-sagemaker-edge-2.5.4/types_aiobotocore_sagemaker_edge/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     4886 2023-08-08 01:20:26.000000 types-aiobotocore-sagemaker-edge-2.5.4/types_aiobotocore_sagemaker_edge/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4884 2023-08-08 01:20:26.000000 types-aiobotocore-sagemaker-edge-2.5.4/types_aiobotocore_sagemaker_edge/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-08-08 01:20:26.000000 types-aiobotocore-sagemaker-edge-2.5.4/types_aiobotocore_sagemaker_edge/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:24:22.742771 types-aiobotocore-sagemaker-edge-2.5.4/types_aiobotocore_sagemaker_edge.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    12591 2023-08-08 01:24:22.000000 types-aiobotocore-sagemaker-edge-2.5.4/types_aiobotocore_sagemaker_edge.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      853 2023-08-08 01:24:22.000000 types-aiobotocore-sagemaker-edge-2.5.4/types_aiobotocore_sagemaker_edge.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 01:24:22.000000 types-aiobotocore-sagemaker-edge-2.5.4/types_aiobotocore_sagemaker_edge.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 01:24:22.000000 types-aiobotocore-sagemaker-edge-2.5.4/types_aiobotocore_sagemaker_edge.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-08 01:24:22.000000 types-aiobotocore-sagemaker-edge-2.5.4/types_aiobotocore_sagemaker_edge.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-08-08 01:24:22.000000 types-aiobotocore-sagemaker-edge-2.5.4/types_aiobotocore_sagemaker_edge.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-sagemaker-edge-2.5.2.post2/LICENSE` & `types-aiobotocore-sagemaker-edge-2.5.4/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-sagemaker-edge-2.5.2.post2/PKG-INFO` & `types-aiobotocore-sagemaker-edge-2.5.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-sagemaker-edge
-Version: 2.5.2.post2
-Summary: Type annotations for aiobotocore.SagemakerEdgeManager 2.5.2 service generated with mypy-boto3-builder 7.17.2
+Version: 2.5.4
+Summary: Type annotations for aiobotocore.SagemakerEdgeManager 2.5.4 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker_edge/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-sagemaker-edge.svg?color=blue)](https://pypi.org/project/types-aiobotocore-sagemaker-edge)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker_edge/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-sagemaker-edge)](https://pepy.tech/project/types-aiobotocore-sagemaker-edge)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.SagemakerEdgeManager 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker-edge.html#SagemakerEdgeManager)
+[aiobotocore.SagemakerEdgeManager 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker-edge.html#SagemakerEdgeManager)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-sagemaker-edge-2.5.2.post2/README.md` & `types-aiobotocore-sagemaker-edge-2.5.4/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-sagemaker-edge.svg?color=blue)](https://pypi.org/project/types-aiobotocore-sagemaker-edge)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker_edge/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-sagemaker-edge)](https://pepy.tech/project/types-aiobotocore-sagemaker-edge)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.SagemakerEdgeManager 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker-edge.html#SagemakerEdgeManager)
+[aiobotocore.SagemakerEdgeManager 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker-edge.html#SagemakerEdgeManager)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-sagemaker-edge-2.5.2.post2/setup.py` & `types-aiobotocore-sagemaker-edge-2.5.4/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-sagemaker-edge",
-    version="2.5.2.post2",
+    version="2.5.4",
     packages=["types_aiobotocore_sagemaker_edge"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.SagemakerEdgeManager 2.5.2 service generated with"
+        "Type annotations for aiobotocore.SagemakerEdgeManager 2.5.4 service generated with"
         " mypy-boto3-builder 7.17.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
```

### Comparing `types-aiobotocore-sagemaker-edge-2.5.2.post2/types_aiobotocore_sagemaker_edge/__init__.py` & `types-aiobotocore-sagemaker-edge-2.5.4/types_aiobotocore_sagemaker_edge/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-sagemaker-edge-2.5.2.post2/types_aiobotocore_sagemaker_edge/__init__.pyi` & `types-aiobotocore-sagemaker-edge-2.5.4/types_aiobotocore_sagemaker_edge/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-sagemaker-edge-2.5.2.post2/types_aiobotocore_sagemaker_edge/__main__.py` & `types-aiobotocore-sagemaker-edge-2.5.4/types_aiobotocore_sagemaker_edge/__main__.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.SagemakerEdgeManager 2.5.2\nVersion:        "
-        " 2.5.2.post2\nBuilder version: 7.17.2\nDocs:           "
+        "Type annotations for aiobotocore.SagemakerEdgeManager 2.5.4\nVersion:        "
+        " 2.5.4\nBuilder version: 7.17.2\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker_edge//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker-edge.html#SagemakerEdgeManager\nOther"
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

### Comparing `types-aiobotocore-sagemaker-edge-2.5.2.post2/types_aiobotocore_sagemaker_edge/client.py` & `types-aiobotocore-sagemaker-edge-2.5.4/types_aiobotocore_sagemaker_edge/client.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-sagemaker-edge-2.5.2.post2/types_aiobotocore_sagemaker_edge/client.pyi` & `types-aiobotocore-sagemaker-edge-2.5.4/types_aiobotocore_sagemaker_edge/client.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-sagemaker-edge-2.5.2.post2/types_aiobotocore_sagemaker_edge/literals.py` & `types-aiobotocore-sagemaker-edge-2.5.4/types_aiobotocore_sagemaker_edge/literals.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-sagemaker-edge-2.5.2.post2/types_aiobotocore_sagemaker_edge/literals.pyi` & `types-aiobotocore-sagemaker-edge-2.5.4/types_aiobotocore_sagemaker_edge/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-sagemaker-edge-2.5.2.post2/types_aiobotocore_sagemaker_edge/type_defs.py` & `types-aiobotocore-sagemaker-edge-2.5.4/types_aiobotocore_sagemaker_edge/type_defs.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-sagemaker-edge-2.5.2.post2/types_aiobotocore_sagemaker_edge/type_defs.pyi` & `types-aiobotocore-sagemaker-edge-2.5.4/types_aiobotocore_sagemaker_edge/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-sagemaker-edge-2.5.2.post2/types_aiobotocore_sagemaker_edge.egg-info/PKG-INFO` & `types-aiobotocore-sagemaker-edge-2.5.4/types_aiobotocore_sagemaker_edge.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-sagemaker-edge
-Version: 2.5.2.post2
-Summary: Type annotations for aiobotocore.SagemakerEdgeManager 2.5.2 service generated with mypy-boto3-builder 7.17.2
+Version: 2.5.4
+Summary: Type annotations for aiobotocore.SagemakerEdgeManager 2.5.4 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker_edge/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-sagemaker-edge.svg?color=blue)](https://pypi.org/project/types-aiobotocore-sagemaker-edge)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker_edge/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-sagemaker-edge)](https://pepy.tech/project/types-aiobotocore-sagemaker-edge)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.SagemakerEdgeManager 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker-edge.html#SagemakerEdgeManager)
+[aiobotocore.SagemakerEdgeManager 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker-edge.html#SagemakerEdgeManager)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-sagemaker-edge-2.5.2.post2/types_aiobotocore_sagemaker_edge.egg-info/SOURCES.txt` & `types-aiobotocore-sagemaker-edge-2.5.4/types_aiobotocore_sagemaker_edge.egg-info/SOURCES.txt`

 * *Files identical despite different names*


# Comparing `tmp/types-aiobotocore-quicksight-2.5.2.post2.tar.gz` & `tmp/types-aiobotocore-quicksight-2.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-quicksight-2.5.2.post2.tar", last modified: Fri Aug  4 13:59:22 2023, max compression
+gzip compressed data, was "types-aiobotocore-quicksight-2.5.4.tar", last modified: Tue Aug  8 01:24:16 2023, max compression
```

## Comparing `types-aiobotocore-quicksight-2.5.2.post2.tar` & `types-aiobotocore-quicksight-2.5.4.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:22.036643 types-aiobotocore-quicksight-2.5.2.post2/
--rw-r--r--   0 vlad      (1000) vlad      (1000)     1070 2023-08-04 13:49:31.000000 types-aiobotocore-quicksight-2.5.2.post2/LICENSE
--rw-r--r--   0 vlad      (1000) vlad      (1000)    16593 2023-08-04 13:59:22.036643 types-aiobotocore-quicksight-2.5.2.post2/PKG-INFO
--rw-r--r--   0 vlad      (1000) vlad      (1000)    15063 2023-08-04 13:49:31.000000 types-aiobotocore-quicksight-2.5.2.post2/README.md
--rw-r--r--   0 vlad      (1000) vlad      (1000)       38 2023-08-04 13:59:22.036643 types-aiobotocore-quicksight-2.5.2.post2/setup.cfg
--rw-r--r--   0 vlad      (1000) vlad      (1000)     2093 2023-08-04 13:49:30.000000 types-aiobotocore-quicksight-2.5.2.post2/setup.py
-drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:22.036643 types-aiobotocore-quicksight-2.5.2.post2/types_aiobotocore_quicksight/
--rw-r--r--   0 vlad      (1000) vlad      (1000)     5671 2023-08-04 13:49:31.000000 types-aiobotocore-quicksight-2.5.2.post2/types_aiobotocore_quicksight/__init__.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)     5670 2023-08-04 13:49:31.000000 types-aiobotocore-quicksight-2.5.2.post2/types_aiobotocore_quicksight/__init__.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)      955 2023-08-04 13:49:31.000000 types-aiobotocore-quicksight-2.5.2.post2/types_aiobotocore_quicksight/__main__.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)   129027 2023-08-04 13:49:32.000000 types-aiobotocore-quicksight-2.5.2.post2/types_aiobotocore_quicksight/client.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)   128832 2023-08-04 13:49:31.000000 types-aiobotocore-quicksight-2.5.2.post2/types_aiobotocore_quicksight/client.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)    36347 2023-08-04 13:49:33.000000 types-aiobotocore-quicksight-2.5.2.post2/types_aiobotocore_quicksight/literals.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)    36345 2023-08-04 13:49:32.000000 types-aiobotocore-quicksight-2.5.2.post2/types_aiobotocore_quicksight/literals.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)    30268 2023-08-04 13:49:32.000000 types-aiobotocore-quicksight-2.5.2.post2/types_aiobotocore_quicksight/paginator.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)    30241 2023-08-04 13:49:32.000000 types-aiobotocore-quicksight-2.5.2.post2/types_aiobotocore_quicksight/paginator.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:49:31.000000 types-aiobotocore-quicksight-2.5.2.post2/types_aiobotocore_quicksight/py.typed
--rw-r--r--   0 vlad      (1000) vlad      (1000)   414859 2023-08-04 13:49:47.000000 types-aiobotocore-quicksight-2.5.2.post2/types_aiobotocore_quicksight/type_defs.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)   414319 2023-08-04 13:49:42.000000 types-aiobotocore-quicksight-2.5.2.post2/types_aiobotocore_quicksight/type_defs.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)       65 2023-08-04 13:49:31.000000 types-aiobotocore-quicksight-2.5.2.post2/types_aiobotocore_quicksight/version.py
-drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:22.036643 types-aiobotocore-quicksight-2.5.2.post2/types_aiobotocore_quicksight.egg-info/
--rw-r--r--   0 vlad      (1000) vlad      (1000)    16593 2023-08-04 13:59:21.000000 types-aiobotocore-quicksight-2.5.2.post2/types_aiobotocore_quicksight.egg-info/PKG-INFO
--rw-r--r--   0 vlad      (1000) vlad      (1000)      870 2023-08-04 13:59:21.000000 types-aiobotocore-quicksight-2.5.2.post2/types_aiobotocore_quicksight.egg-info/SOURCES.txt
--rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:21.000000 types-aiobotocore-quicksight-2.5.2.post2/types_aiobotocore_quicksight.egg-info/dependency_links.txt
--rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:21.000000 types-aiobotocore-quicksight-2.5.2.post2/types_aiobotocore_quicksight.egg-info/not-zip-safe
--rw-r--r--   0 vlad      (1000) vlad      (1000)       52 2023-08-04 13:59:21.000000 types-aiobotocore-quicksight-2.5.2.post2/types_aiobotocore_quicksight.egg-info/requires.txt
--rw-r--r--   0 vlad      (1000) vlad      (1000)       29 2023-08-04 13:59:21.000000 types-aiobotocore-quicksight-2.5.2.post2/types_aiobotocore_quicksight.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:24:16.230755 types-aiobotocore-quicksight-2.5.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-08 01:18:33.000000 types-aiobotocore-quicksight-2.5.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    16587 2023-08-08 01:24:16.230755 types-aiobotocore-quicksight-2.5.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    15063 2023-08-08 01:18:33.000000 types-aiobotocore-quicksight-2.5.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-08 01:24:16.230755 types-aiobotocore-quicksight-2.5.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2087 2023-08-08 01:18:33.000000 types-aiobotocore-quicksight-2.5.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:24:16.226755 types-aiobotocore-quicksight-2.5.4/types_aiobotocore_quicksight/
+-rw-r--r--   0 runner    (1001) docker     (123)     5671 2023-08-08 01:18:33.000000 types-aiobotocore-quicksight-2.5.4/types_aiobotocore_quicksight/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5670 2023-08-08 01:18:33.000000 types-aiobotocore-quicksight-2.5.4/types_aiobotocore_quicksight/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      943 2023-08-08 01:18:33.000000 types-aiobotocore-quicksight-2.5.4/types_aiobotocore_quicksight/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   129027 2023-08-08 01:18:37.000000 types-aiobotocore-quicksight-2.5.4/types_aiobotocore_quicksight/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)   128832 2023-08-08 01:18:34.000000 types-aiobotocore-quicksight-2.5.4/types_aiobotocore_quicksight/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    36347 2023-08-08 01:18:38.000000 types-aiobotocore-quicksight-2.5.4/types_aiobotocore_quicksight/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36345 2023-08-08 01:18:38.000000 types-aiobotocore-quicksight-2.5.4/types_aiobotocore_quicksight/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    30268 2023-08-08 01:18:38.000000 types-aiobotocore-quicksight-2.5.4/types_aiobotocore_quicksight/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30241 2023-08-08 01:18:38.000000 types-aiobotocore-quicksight-2.5.4/types_aiobotocore_quicksight/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 01:18:33.000000 types-aiobotocore-quicksight-2.5.4/types_aiobotocore_quicksight/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)   414859 2023-08-08 01:18:48.000000 types-aiobotocore-quicksight-2.5.4/types_aiobotocore_quicksight/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)   414319 2023-08-08 01:18:42.000000 types-aiobotocore-quicksight-2.5.4/types_aiobotocore_quicksight/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-08-08 01:18:33.000000 types-aiobotocore-quicksight-2.5.4/types_aiobotocore_quicksight/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:24:16.230755 types-aiobotocore-quicksight-2.5.4/types_aiobotocore_quicksight.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    16587 2023-08-08 01:24:16.000000 types-aiobotocore-quicksight-2.5.4/types_aiobotocore_quicksight.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      870 2023-08-08 01:24:16.000000 types-aiobotocore-quicksight-2.5.4/types_aiobotocore_quicksight.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 01:24:16.000000 types-aiobotocore-quicksight-2.5.4/types_aiobotocore_quicksight.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 01:24:16.000000 types-aiobotocore-quicksight-2.5.4/types_aiobotocore_quicksight.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-08 01:24:16.000000 types-aiobotocore-quicksight-2.5.4/types_aiobotocore_quicksight.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-08-08 01:24:16.000000 types-aiobotocore-quicksight-2.5.4/types_aiobotocore_quicksight.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-quicksight-2.5.2.post2/LICENSE` & `types-aiobotocore-quicksight-2.5.4/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-quicksight-2.5.2.post2/PKG-INFO` & `types-aiobotocore-quicksight-2.5.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-quicksight
-Version: 2.5.2.post2
-Summary: Type annotations for aiobotocore.QuickSight 2.5.2 service generated with mypy-boto3-builder 7.17.2
+Version: 2.5.4
+Summary: Type annotations for aiobotocore.QuickSight 2.5.4 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_quicksight/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-quicksight.svg?color=blue)](https://pypi.org/project/types-aiobotocore-quicksight)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_quicksight/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-quicksight)](https://pepy.tech/project/types-aiobotocore-quicksight)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.QuickSight 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight.html#QuickSight)
+[aiobotocore.QuickSight 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight.html#QuickSight)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-quicksight-2.5.2.post2/README.md` & `types-aiobotocore-quicksight-2.5.4/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-quicksight.svg?color=blue)](https://pypi.org/project/types-aiobotocore-quicksight)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_quicksight/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-quicksight)](https://pepy.tech/project/types-aiobotocore-quicksight)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.QuickSight 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight.html#QuickSight)
+[aiobotocore.QuickSight 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight.html#QuickSight)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-quicksight-2.5.2.post2/setup.py` & `types-aiobotocore-quicksight-2.5.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-quicksight",
-    version="2.5.2.post2",
+    version="2.5.4",
     packages=["types_aiobotocore_quicksight"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.QuickSight 2.5.2 service generated with"
+        "Type annotations for aiobotocore.QuickSight 2.5.4 service generated with"
         " mypy-boto3-builder 7.17.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
```

### Comparing `types-aiobotocore-quicksight-2.5.2.post2/types_aiobotocore_quicksight/__init__.py` & `types-aiobotocore-quicksight-2.5.4/types_aiobotocore_quicksight/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-quicksight-2.5.2.post2/types_aiobotocore_quicksight/__init__.pyi` & `types-aiobotocore-quicksight-2.5.4/types_aiobotocore_quicksight/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-quicksight-2.5.2.post2/types_aiobotocore_quicksight/__main__.py` & `types-aiobotocore-quicksight-2.5.4/types_aiobotocore_quicksight/__main__.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.QuickSight 2.5.2\nVersion:         2.5.2.post2\nBuilder"
+        "Type annotations for aiobotocore.QuickSight 2.5.4\nVersion:         2.5.4\nBuilder"
         " version: 7.17.2\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_quicksight//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight.html#QuickSight\nOther"
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

### Comparing `types-aiobotocore-quicksight-2.5.2.post2/types_aiobotocore_quicksight/client.py` & `types-aiobotocore-quicksight-2.5.4/types_aiobotocore_quicksight/client.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-quicksight-2.5.2.post2/types_aiobotocore_quicksight/client.pyi` & `types-aiobotocore-quicksight-2.5.4/types_aiobotocore_quicksight/client.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-quicksight-2.5.2.post2/types_aiobotocore_quicksight/literals.py` & `types-aiobotocore-quicksight-2.5.4/types_aiobotocore_quicksight/literals.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-quicksight-2.5.2.post2/types_aiobotocore_quicksight/literals.pyi` & `types-aiobotocore-quicksight-2.5.4/types_aiobotocore_quicksight/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-quicksight-2.5.2.post2/types_aiobotocore_quicksight/paginator.py` & `types-aiobotocore-quicksight-2.5.4/types_aiobotocore_quicksight/paginator.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-quicksight-2.5.2.post2/types_aiobotocore_quicksight/paginator.pyi` & `types-aiobotocore-quicksight-2.5.4/types_aiobotocore_quicksight/paginator.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-quicksight-2.5.2.post2/types_aiobotocore_quicksight/type_defs.py` & `types-aiobotocore-quicksight-2.5.4/types_aiobotocore_quicksight/type_defs.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-quicksight-2.5.2.post2/types_aiobotocore_quicksight/type_defs.pyi` & `types-aiobotocore-quicksight-2.5.4/types_aiobotocore_quicksight/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-quicksight-2.5.2.post2/types_aiobotocore_quicksight.egg-info/PKG-INFO` & `types-aiobotocore-quicksight-2.5.4/types_aiobotocore_quicksight.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-quicksight
-Version: 2.5.2.post2
-Summary: Type annotations for aiobotocore.QuickSight 2.5.2 service generated with mypy-boto3-builder 7.17.2
+Version: 2.5.4
+Summary: Type annotations for aiobotocore.QuickSight 2.5.4 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_quicksight/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-quicksight.svg?color=blue)](https://pypi.org/project/types-aiobotocore-quicksight)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_quicksight/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-quicksight)](https://pepy.tech/project/types-aiobotocore-quicksight)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.QuickSight 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight.html#QuickSight)
+[aiobotocore.QuickSight 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight.html#QuickSight)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-quicksight-2.5.2.post2/types_aiobotocore_quicksight.egg-info/SOURCES.txt` & `types-aiobotocore-quicksight-2.5.4/types_aiobotocore_quicksight.egg-info/SOURCES.txt`

 * *Files identical despite different names*


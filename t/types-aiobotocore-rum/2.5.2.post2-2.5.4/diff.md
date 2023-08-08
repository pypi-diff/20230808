# Comparing `tmp/types-aiobotocore-rum-2.5.2.post2.tar.gz` & `tmp/types-aiobotocore-rum-2.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-rum-2.5.2.post2.tar", last modified: Fri Aug  4 13:59:24 2023, max compression
+gzip compressed data, was "types-aiobotocore-rum-2.5.4.tar", last modified: Tue Aug  8 01:24:21 2023, max compression
```

## Comparing `types-aiobotocore-rum-2.5.2.post2.tar` & `types-aiobotocore-rum-2.5.4.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:23.996643 types-aiobotocore-rum-2.5.2.post2/
--rw-r--r--   0 vlad      (1000) vlad      (1000)     1070 2023-08-04 13:51:22.000000 types-aiobotocore-rum-2.5.2.post2/LICENSE
--rw-r--r--   0 vlad      (1000) vlad      (1000)    13418 2023-08-04 13:59:23.996643 types-aiobotocore-rum-2.5.2.post2/PKG-INFO
--rw-r--r--   0 vlad      (1000) vlad      (1000)    11906 2023-08-04 13:51:22.000000 types-aiobotocore-rum-2.5.2.post2/README.md
--rw-r--r--   0 vlad      (1000) vlad      (1000)       38 2023-08-04 13:59:23.996643 types-aiobotocore-rum-2.5.2.post2/setup.cfg
--rw-r--r--   0 vlad      (1000) vlad      (1000)     2030 2023-08-04 13:51:22.000000 types-aiobotocore-rum-2.5.2.post2/setup.py
-drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:23.996643 types-aiobotocore-rum-2.5.2.post2/types_aiobotocore_rum/
--rw-r--r--   0 vlad      (1000) vlad      (1000)     1455 2023-08-04 13:51:22.000000 types-aiobotocore-rum-2.5.2.post2/types_aiobotocore_rum/__init__.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)     1454 2023-08-04 13:51:22.000000 types-aiobotocore-rum-2.5.2.post2/types_aiobotocore_rum/__init__.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)      936 2023-08-04 13:51:22.000000 types-aiobotocore-rum-2.5.2.post2/types_aiobotocore_rum/__main__.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)    18059 2023-08-04 13:51:23.000000 types-aiobotocore-rum-2.5.2.post2/types_aiobotocore_rum/client.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)    18029 2023-08-04 13:51:23.000000 types-aiobotocore-rum-2.5.2.post2/types_aiobotocore_rum/client.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)     8887 2023-08-04 13:51:23.000000 types-aiobotocore-rum-2.5.2.post2/types_aiobotocore_rum/literals.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)     8885 2023-08-04 13:51:23.000000 types-aiobotocore-rum-2.5.2.post2/types_aiobotocore_rum/literals.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)     5894 2023-08-04 13:51:23.000000 types-aiobotocore-rum-2.5.2.post2/types_aiobotocore_rum/paginator.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)     5888 2023-08-04 13:51:23.000000 types-aiobotocore-rum-2.5.2.post2/types_aiobotocore_rum/paginator.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:51:22.000000 types-aiobotocore-rum-2.5.2.post2/types_aiobotocore_rum/py.typed
--rw-r--r--   0 vlad      (1000) vlad      (1000)    20184 2023-08-04 13:51:23.000000 types-aiobotocore-rum-2.5.2.post2/types_aiobotocore_rum/type_defs.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)    20149 2023-08-04 13:51:23.000000 types-aiobotocore-rum-2.5.2.post2/types_aiobotocore_rum/type_defs.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)       65 2023-08-04 13:51:22.000000 types-aiobotocore-rum-2.5.2.post2/types_aiobotocore_rum/version.py
-drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:23.996643 types-aiobotocore-rum-2.5.2.post2/types_aiobotocore_rum.egg-info/
--rw-r--r--   0 vlad      (1000) vlad      (1000)    13418 2023-08-04 13:59:23.000000 types-aiobotocore-rum-2.5.2.post2/types_aiobotocore_rum.egg-info/PKG-INFO
--rw-r--r--   0 vlad      (1000) vlad      (1000)      737 2023-08-04 13:59:23.000000 types-aiobotocore-rum-2.5.2.post2/types_aiobotocore_rum.egg-info/SOURCES.txt
--rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:23.000000 types-aiobotocore-rum-2.5.2.post2/types_aiobotocore_rum.egg-info/dependency_links.txt
--rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:23.000000 types-aiobotocore-rum-2.5.2.post2/types_aiobotocore_rum.egg-info/not-zip-safe
--rw-r--r--   0 vlad      (1000) vlad      (1000)       52 2023-08-04 13:59:23.000000 types-aiobotocore-rum-2.5.2.post2/types_aiobotocore_rum.egg-info/requires.txt
--rw-r--r--   0 vlad      (1000) vlad      (1000)       22 2023-08-04 13:59:23.000000 types-aiobotocore-rum-2.5.2.post2/types_aiobotocore_rum.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:24:21.322768 types-aiobotocore-rum-2.5.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-08 01:19:45.000000 types-aiobotocore-rum-2.5.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    13412 2023-08-08 01:24:21.322768 types-aiobotocore-rum-2.5.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    11906 2023-08-08 01:19:45.000000 types-aiobotocore-rum-2.5.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-08 01:24:21.322768 types-aiobotocore-rum-2.5.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2024 2023-08-08 01:19:45.000000 types-aiobotocore-rum-2.5.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:24:21.322768 types-aiobotocore-rum-2.5.4/types_aiobotocore_rum/
+-rw-r--r--   0 runner    (1001) docker     (123)     1455 2023-08-08 01:19:45.000000 types-aiobotocore-rum-2.5.4/types_aiobotocore_rum/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1454 2023-08-08 01:19:45.000000 types-aiobotocore-rum-2.5.4/types_aiobotocore_rum/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      924 2023-08-08 01:19:45.000000 types-aiobotocore-rum-2.5.4/types_aiobotocore_rum/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18059 2023-08-08 01:19:45.000000 types-aiobotocore-rum-2.5.4/types_aiobotocore_rum/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18029 2023-08-08 01:19:45.000000 types-aiobotocore-rum-2.5.4/types_aiobotocore_rum/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8887 2023-08-08 01:19:45.000000 types-aiobotocore-rum-2.5.4/types_aiobotocore_rum/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8885 2023-08-08 01:19:45.000000 types-aiobotocore-rum-2.5.4/types_aiobotocore_rum/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     5894 2023-08-08 01:19:45.000000 types-aiobotocore-rum-2.5.4/types_aiobotocore_rum/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5888 2023-08-08 01:19:45.000000 types-aiobotocore-rum-2.5.4/types_aiobotocore_rum/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 01:19:45.000000 types-aiobotocore-rum-2.5.4/types_aiobotocore_rum/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    20184 2023-08-08 01:19:46.000000 types-aiobotocore-rum-2.5.4/types_aiobotocore_rum/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20149 2023-08-08 01:19:45.000000 types-aiobotocore-rum-2.5.4/types_aiobotocore_rum/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-08-08 01:19:45.000000 types-aiobotocore-rum-2.5.4/types_aiobotocore_rum/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:24:21.322768 types-aiobotocore-rum-2.5.4/types_aiobotocore_rum.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    13412 2023-08-08 01:24:21.000000 types-aiobotocore-rum-2.5.4/types_aiobotocore_rum.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      737 2023-08-08 01:24:21.000000 types-aiobotocore-rum-2.5.4/types_aiobotocore_rum.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 01:24:21.000000 types-aiobotocore-rum-2.5.4/types_aiobotocore_rum.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 01:24:21.000000 types-aiobotocore-rum-2.5.4/types_aiobotocore_rum.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-08 01:24:21.000000 types-aiobotocore-rum-2.5.4/types_aiobotocore_rum.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-08-08 01:24:21.000000 types-aiobotocore-rum-2.5.4/types_aiobotocore_rum.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-rum-2.5.2.post2/LICENSE` & `types-aiobotocore-rum-2.5.4/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-rum-2.5.2.post2/PKG-INFO` & `types-aiobotocore-rum-2.5.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-rum
-Version: 2.5.2.post2
-Summary: Type annotations for aiobotocore.CloudWatchRUM 2.5.2 service generated with mypy-boto3-builder 7.17.2
+Version: 2.5.4
+Summary: Type annotations for aiobotocore.CloudWatchRUM 2.5.4 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rum/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-rum.svg?color=blue)](https://pypi.org/project/types-aiobotocore-rum)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rum/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-rum)](https://pepy.tech/project/types-aiobotocore-rum)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.CloudWatchRUM 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rum.html#CloudWatchRUM)
+[aiobotocore.CloudWatchRUM 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rum.html#CloudWatchRUM)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-rum-2.5.2.post2/README.md` & `types-aiobotocore-rum-2.5.4/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-rum.svg?color=blue)](https://pypi.org/project/types-aiobotocore-rum)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rum/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-rum)](https://pepy.tech/project/types-aiobotocore-rum)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.CloudWatchRUM 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rum.html#CloudWatchRUM)
+[aiobotocore.CloudWatchRUM 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rum.html#CloudWatchRUM)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-rum-2.5.2.post2/setup.py` & `types-aiobotocore-rum-2.5.4/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-rum",
-    version="2.5.2.post2",
+    version="2.5.4",
     packages=["types_aiobotocore_rum"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.CloudWatchRUM 2.5.2 service generated with"
+        "Type annotations for aiobotocore.CloudWatchRUM 2.5.4 service generated with"
         " mypy-boto3-builder 7.17.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
```

### Comparing `types-aiobotocore-rum-2.5.2.post2/types_aiobotocore_rum/__init__.py` & `types-aiobotocore-rum-2.5.4/types_aiobotocore_rum/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-rum-2.5.2.post2/types_aiobotocore_rum/__init__.pyi` & `types-aiobotocore-rum-2.5.4/types_aiobotocore_rum/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-rum-2.5.2.post2/types_aiobotocore_rum/__main__.py` & `types-aiobotocore-rum-2.5.4/types_aiobotocore_rum/__main__.py`

 * *Files 15% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.CloudWatchRUM 2.5.2\nVersion:        "
-        " 2.5.2.post2\nBuilder version: 7.17.2\nDocs:           "
+        "Type annotations for aiobotocore.CloudWatchRUM 2.5.4\nVersion:         2.5.4\nBuilder"
+        " version: 7.17.2\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rum//\nBoto3 docs:    "
         "  https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rum.html#CloudWatchRUM\nOther"
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

### Comparing `types-aiobotocore-rum-2.5.2.post2/types_aiobotocore_rum/client.py` & `types-aiobotocore-rum-2.5.4/types_aiobotocore_rum/client.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-rum-2.5.2.post2/types_aiobotocore_rum/client.pyi` & `types-aiobotocore-rum-2.5.4/types_aiobotocore_rum/client.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-rum-2.5.2.post2/types_aiobotocore_rum/literals.py` & `types-aiobotocore-rum-2.5.4/types_aiobotocore_rum/literals.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-rum-2.5.2.post2/types_aiobotocore_rum/literals.pyi` & `types-aiobotocore-rum-2.5.4/types_aiobotocore_rum/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-rum-2.5.2.post2/types_aiobotocore_rum/paginator.py` & `types-aiobotocore-rum-2.5.4/types_aiobotocore_rum/paginator.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-rum-2.5.2.post2/types_aiobotocore_rum/paginator.pyi` & `types-aiobotocore-rum-2.5.4/types_aiobotocore_rum/paginator.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-rum-2.5.2.post2/types_aiobotocore_rum/type_defs.py` & `types-aiobotocore-rum-2.5.4/types_aiobotocore_rum/type_defs.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-rum-2.5.2.post2/types_aiobotocore_rum/type_defs.pyi` & `types-aiobotocore-rum-2.5.4/types_aiobotocore_rum/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-rum-2.5.2.post2/types_aiobotocore_rum.egg-info/PKG-INFO` & `types-aiobotocore-rum-2.5.4/types_aiobotocore_rum.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-rum
-Version: 2.5.2.post2
-Summary: Type annotations for aiobotocore.CloudWatchRUM 2.5.2 service generated with mypy-boto3-builder 7.17.2
+Version: 2.5.4
+Summary: Type annotations for aiobotocore.CloudWatchRUM 2.5.4 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rum/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-rum.svg?color=blue)](https://pypi.org/project/types-aiobotocore-rum)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rum/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-rum)](https://pepy.tech/project/types-aiobotocore-rum)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.CloudWatchRUM 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rum.html#CloudWatchRUM)
+[aiobotocore.CloudWatchRUM 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rum.html#CloudWatchRUM)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-rum-2.5.2.post2/types_aiobotocore_rum.egg-info/SOURCES.txt` & `types-aiobotocore-rum-2.5.4/types_aiobotocore_rum.egg-info/SOURCES.txt`

 * *Files identical despite different names*


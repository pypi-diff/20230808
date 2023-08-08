# Comparing `tmp/types-aiobotocore-rekognition-2.5.2.post2.tar.gz` & `tmp/types-aiobotocore-rekognition-2.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-rekognition-2.5.2.post2.tar", last modified: Fri Aug  4 13:59:22 2023, max compression
+gzip compressed data, was "types-aiobotocore-rekognition-2.5.4.tar", last modified: Tue Aug  8 01:24:18 2023, max compression
```

## Comparing `types-aiobotocore-rekognition-2.5.2.post2.tar` & `types-aiobotocore-rekognition-2.5.4.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:22.906643 types-aiobotocore-rekognition-2.5.2.post2/
--rw-r--r--   0 vlad      (1000) vlad      (1000)     1070 2023-08-04 13:50:34.000000 types-aiobotocore-rekognition-2.5.2.post2/LICENSE
--rw-r--r--   0 vlad      (1000) vlad      (1000)    15268 2023-08-04 13:59:22.906643 types-aiobotocore-rekognition-2.5.2.post2/PKG-INFO
--rw-r--r--   0 vlad      (1000) vlad      (1000)    13734 2023-08-04 13:50:34.000000 types-aiobotocore-rekognition-2.5.2.post2/README.md
--rw-r--r--   0 vlad      (1000) vlad      (1000)       38 2023-08-04 13:59:22.906643 types-aiobotocore-rekognition-2.5.2.post2/setup.cfg
--rw-r--r--   0 vlad      (1000) vlad      (1000)     2100 2023-08-04 13:50:34.000000 types-aiobotocore-rekognition-2.5.2.post2/setup.py
-drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:22.906643 types-aiobotocore-rekognition-2.5.2.post2/types_aiobotocore_rekognition/
--rw-r--r--   0 vlad      (1000) vlad      (1000)     2859 2023-08-04 13:50:34.000000 types-aiobotocore-rekognition-2.5.2.post2/types_aiobotocore_rekognition/__init__.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)     2858 2023-08-04 13:50:34.000000 types-aiobotocore-rekognition-2.5.2.post2/types_aiobotocore_rekognition/__init__.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)      959 2023-08-04 13:50:34.000000 types-aiobotocore-rekognition-2.5.2.post2/types_aiobotocore_rekognition/__main__.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)    60517 2023-08-04 13:50:34.000000 types-aiobotocore-rekognition-2.5.2.post2/types_aiobotocore_rekognition/client.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)    60425 2023-08-04 13:50:34.000000 types-aiobotocore-rekognition-2.5.2.post2/types_aiobotocore_rekognition/client.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)    14856 2023-08-04 13:50:35.000000 types-aiobotocore-rekognition-2.5.2.post2/types_aiobotocore_rekognition/literals.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)    14854 2023-08-04 13:50:35.000000 types-aiobotocore-rekognition-2.5.2.post2/types_aiobotocore_rekognition/literals.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)    11430 2023-08-04 13:50:34.000000 types-aiobotocore-rekognition-2.5.2.post2/types_aiobotocore_rekognition/paginator.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)    11419 2023-08-04 13:50:34.000000 types-aiobotocore-rekognition-2.5.2.post2/types_aiobotocore_rekognition/paginator.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:50:34.000000 types-aiobotocore-rekognition-2.5.2.post2/types_aiobotocore_rekognition/py.typed
--rw-r--r--   0 vlad      (1000) vlad      (1000)    97024 2023-08-04 13:50:40.000000 types-aiobotocore-rekognition-2.5.2.post2/types_aiobotocore_rekognition/type_defs.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)    96905 2023-08-04 13:50:36.000000 types-aiobotocore-rekognition-2.5.2.post2/types_aiobotocore_rekognition/type_defs.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)       65 2023-08-04 13:50:34.000000 types-aiobotocore-rekognition-2.5.2.post2/types_aiobotocore_rekognition/version.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)     3088 2023-08-04 13:50:34.000000 types-aiobotocore-rekognition-2.5.2.post2/types_aiobotocore_rekognition/waiter.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)     3086 2023-08-04 13:50:34.000000 types-aiobotocore-rekognition-2.5.2.post2/types_aiobotocore_rekognition/waiter.pyi
-drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:22.906643 types-aiobotocore-rekognition-2.5.2.post2/types_aiobotocore_rekognition.egg-info/
--rw-r--r--   0 vlad      (1000) vlad      (1000)    15268 2023-08-04 13:59:22.000000 types-aiobotocore-rekognition-2.5.2.post2/types_aiobotocore_rekognition.egg-info/PKG-INFO
--rw-r--r--   0 vlad      (1000) vlad      (1000)      970 2023-08-04 13:59:22.000000 types-aiobotocore-rekognition-2.5.2.post2/types_aiobotocore_rekognition.egg-info/SOURCES.txt
--rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:22.000000 types-aiobotocore-rekognition-2.5.2.post2/types_aiobotocore_rekognition.egg-info/dependency_links.txt
--rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:22.000000 types-aiobotocore-rekognition-2.5.2.post2/types_aiobotocore_rekognition.egg-info/not-zip-safe
--rw-r--r--   0 vlad      (1000) vlad      (1000)       52 2023-08-04 13:59:22.000000 types-aiobotocore-rekognition-2.5.2.post2/types_aiobotocore_rekognition.egg-info/requires.txt
--rw-r--r--   0 vlad      (1000) vlad      (1000)       30 2023-08-04 13:59:22.000000 types-aiobotocore-rekognition-2.5.2.post2/types_aiobotocore_rekognition.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:24:18.210760 types-aiobotocore-rekognition-2.5.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-08 01:19:17.000000 types-aiobotocore-rekognition-2.5.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    15262 2023-08-08 01:24:18.210760 types-aiobotocore-rekognition-2.5.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    13734 2023-08-08 01:19:17.000000 types-aiobotocore-rekognition-2.5.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-08 01:24:18.210760 types-aiobotocore-rekognition-2.5.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2094 2023-08-08 01:19:17.000000 types-aiobotocore-rekognition-2.5.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:24:18.206760 types-aiobotocore-rekognition-2.5.4/types_aiobotocore_rekognition/
+-rw-r--r--   0 runner    (1001) docker     (123)     2859 2023-08-08 01:19:17.000000 types-aiobotocore-rekognition-2.5.4/types_aiobotocore_rekognition/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2858 2023-08-08 01:19:17.000000 types-aiobotocore-rekognition-2.5.4/types_aiobotocore_rekognition/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      947 2023-08-08 01:19:17.000000 types-aiobotocore-rekognition-2.5.4/types_aiobotocore_rekognition/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    60517 2023-08-08 01:19:18.000000 types-aiobotocore-rekognition-2.5.4/types_aiobotocore_rekognition/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    60425 2023-08-08 01:19:18.000000 types-aiobotocore-rekognition-2.5.4/types_aiobotocore_rekognition/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    14856 2023-08-08 01:19:18.000000 types-aiobotocore-rekognition-2.5.4/types_aiobotocore_rekognition/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14854 2023-08-08 01:19:18.000000 types-aiobotocore-rekognition-2.5.4/types_aiobotocore_rekognition/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    11430 2023-08-08 01:19:18.000000 types-aiobotocore-rekognition-2.5.4/types_aiobotocore_rekognition/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11419 2023-08-08 01:19:18.000000 types-aiobotocore-rekognition-2.5.4/types_aiobotocore_rekognition/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 01:19:17.000000 types-aiobotocore-rekognition-2.5.4/types_aiobotocore_rekognition/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    97024 2023-08-08 01:19:20.000000 types-aiobotocore-rekognition-2.5.4/types_aiobotocore_rekognition/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    96905 2023-08-08 01:19:19.000000 types-aiobotocore-rekognition-2.5.4/types_aiobotocore_rekognition/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-08-08 01:19:17.000000 types-aiobotocore-rekognition-2.5.4/types_aiobotocore_rekognition/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3088 2023-08-08 01:19:18.000000 types-aiobotocore-rekognition-2.5.4/types_aiobotocore_rekognition/waiter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3086 2023-08-08 01:19:18.000000 types-aiobotocore-rekognition-2.5.4/types_aiobotocore_rekognition/waiter.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:24:18.210760 types-aiobotocore-rekognition-2.5.4/types_aiobotocore_rekognition.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    15262 2023-08-08 01:24:18.000000 types-aiobotocore-rekognition-2.5.4/types_aiobotocore_rekognition.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      970 2023-08-08 01:24:18.000000 types-aiobotocore-rekognition-2.5.4/types_aiobotocore_rekognition.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 01:24:18.000000 types-aiobotocore-rekognition-2.5.4/types_aiobotocore_rekognition.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 01:24:18.000000 types-aiobotocore-rekognition-2.5.4/types_aiobotocore_rekognition.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-08 01:24:18.000000 types-aiobotocore-rekognition-2.5.4/types_aiobotocore_rekognition.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-08-08 01:24:18.000000 types-aiobotocore-rekognition-2.5.4/types_aiobotocore_rekognition.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-rekognition-2.5.2.post2/LICENSE` & `types-aiobotocore-rekognition-2.5.4/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-rekognition-2.5.2.post2/PKG-INFO` & `types-aiobotocore-rekognition-2.5.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-rekognition
-Version: 2.5.2.post2
-Summary: Type annotations for aiobotocore.Rekognition 2.5.2 service generated with mypy-boto3-builder 7.17.2
+Version: 2.5.4
+Summary: Type annotations for aiobotocore.Rekognition 2.5.4 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rekognition/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-rekognition.svg?color=blue)](https://pypi.org/project/types-aiobotocore-rekognition)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rekognition/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-rekognition)](https://pepy.tech/project/types-aiobotocore-rekognition)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.Rekognition 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rekognition.html#Rekognition)
+[aiobotocore.Rekognition 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rekognition.html#Rekognition)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-rekognition-2.5.2.post2/README.md` & `types-aiobotocore-rekognition-2.5.4/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-rekognition.svg?color=blue)](https://pypi.org/project/types-aiobotocore-rekognition)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rekognition/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-rekognition)](https://pepy.tech/project/types-aiobotocore-rekognition)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.Rekognition 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rekognition.html#Rekognition)
+[aiobotocore.Rekognition 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rekognition.html#Rekognition)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-rekognition-2.5.2.post2/setup.py` & `types-aiobotocore-rekognition-2.5.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-rekognition",
-    version="2.5.2.post2",
+    version="2.5.4",
     packages=["types_aiobotocore_rekognition"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.Rekognition 2.5.2 service generated with"
+        "Type annotations for aiobotocore.Rekognition 2.5.4 service generated with"
         " mypy-boto3-builder 7.17.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
```

### Comparing `types-aiobotocore-rekognition-2.5.2.post2/types_aiobotocore_rekognition/__init__.py` & `types-aiobotocore-rekognition-2.5.4/types_aiobotocore_rekognition/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-rekognition-2.5.2.post2/types_aiobotocore_rekognition/__init__.pyi` & `types-aiobotocore-rekognition-2.5.4/types_aiobotocore_rekognition/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-rekognition-2.5.2.post2/types_aiobotocore_rekognition/__main__.py` & `types-aiobotocore-rekognition-2.5.4/types_aiobotocore_rekognition/__main__.py`

 * *Files 11% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.Rekognition 2.5.2\nVersion:         2.5.2.post2\nBuilder"
+        "Type annotations for aiobotocore.Rekognition 2.5.4\nVersion:         2.5.4\nBuilder"
         " version: 7.17.2\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rekognition//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rekognition.html#Rekognition\nOther"
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

### Comparing `types-aiobotocore-rekognition-2.5.2.post2/types_aiobotocore_rekognition/client.py` & `types-aiobotocore-rekognition-2.5.4/types_aiobotocore_rekognition/client.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-rekognition-2.5.2.post2/types_aiobotocore_rekognition/client.pyi` & `types-aiobotocore-rekognition-2.5.4/types_aiobotocore_rekognition/client.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-rekognition-2.5.2.post2/types_aiobotocore_rekognition/literals.py` & `types-aiobotocore-rekognition-2.5.4/types_aiobotocore_rekognition/literals.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-rekognition-2.5.2.post2/types_aiobotocore_rekognition/literals.pyi` & `types-aiobotocore-rekognition-2.5.4/types_aiobotocore_rekognition/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-rekognition-2.5.2.post2/types_aiobotocore_rekognition/paginator.py` & `types-aiobotocore-rekognition-2.5.4/types_aiobotocore_rekognition/paginator.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-rekognition-2.5.2.post2/types_aiobotocore_rekognition/paginator.pyi` & `types-aiobotocore-rekognition-2.5.4/types_aiobotocore_rekognition/paginator.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-rekognition-2.5.2.post2/types_aiobotocore_rekognition/type_defs.py` & `types-aiobotocore-rekognition-2.5.4/types_aiobotocore_rekognition/type_defs.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-rekognition-2.5.2.post2/types_aiobotocore_rekognition/type_defs.pyi` & `types-aiobotocore-rekognition-2.5.4/types_aiobotocore_rekognition/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-rekognition-2.5.2.post2/types_aiobotocore_rekognition/waiter.py` & `types-aiobotocore-rekognition-2.5.4/types_aiobotocore_rekognition/waiter.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-rekognition-2.5.2.post2/types_aiobotocore_rekognition/waiter.pyi` & `types-aiobotocore-rekognition-2.5.4/types_aiobotocore_rekognition/waiter.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-rekognition-2.5.2.post2/types_aiobotocore_rekognition.egg-info/PKG-INFO` & `types-aiobotocore-rekognition-2.5.4/types_aiobotocore_rekognition.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-rekognition
-Version: 2.5.2.post2
-Summary: Type annotations for aiobotocore.Rekognition 2.5.2 service generated with mypy-boto3-builder 7.17.2
+Version: 2.5.4
+Summary: Type annotations for aiobotocore.Rekognition 2.5.4 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rekognition/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-rekognition.svg?color=blue)](https://pypi.org/project/types-aiobotocore-rekognition)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rekognition/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-rekognition)](https://pepy.tech/project/types-aiobotocore-rekognition)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.Rekognition 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rekognition.html#Rekognition)
+[aiobotocore.Rekognition 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rekognition.html#Rekognition)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-rekognition-2.5.2.post2/types_aiobotocore_rekognition.egg-info/SOURCES.txt` & `types-aiobotocore-rekognition-2.5.4/types_aiobotocore_rekognition.egg-info/SOURCES.txt`

 * *Files identical despite different names*


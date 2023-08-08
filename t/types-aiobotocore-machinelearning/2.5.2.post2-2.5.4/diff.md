# Comparing `tmp/types-aiobotocore-machinelearning-2.5.2.post2.tar.gz` & `tmp/types-aiobotocore-machinelearning-2.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-machinelearning-2.5.2.post2.tar", last modified: Fri Aug  4 13:59:16 2023, max compression
+gzip compressed data, was "types-aiobotocore-machinelearning-2.5.4.tar", last modified: Tue Aug  8 01:24:02 2023, max compression
```

## Comparing `types-aiobotocore-machinelearning-2.5.2.post2.tar` & `types-aiobotocore-machinelearning-2.5.4.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:16.366643 types-aiobotocore-machinelearning-2.5.2.post2/
--rw-r--r--   0 vlad      (1000) vlad      (1000)     1070 2023-08-04 13:43:36.000000 types-aiobotocore-machinelearning-2.5.2.post2/LICENSE
--rw-r--r--   0 vlad      (1000) vlad      (1000)    15096 2023-08-04 13:59:16.366643 types-aiobotocore-machinelearning-2.5.2.post2/PKG-INFO
--rw-r--r--   0 vlad      (1000) vlad      (1000)    13546 2023-08-04 13:43:36.000000 types-aiobotocore-machinelearning-2.5.2.post2/README.md
--rw-r--r--   0 vlad      (1000) vlad      (1000)       38 2023-08-04 13:59:16.366643 types-aiobotocore-machinelearning-2.5.2.post2/setup.cfg
--rw-r--r--   0 vlad      (1000) vlad      (1000)     2128 2023-08-04 13:43:35.000000 types-aiobotocore-machinelearning-2.5.2.post2/setup.py
-drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:16.366643 types-aiobotocore-machinelearning-2.5.2.post2/types_aiobotocore_machinelearning/
--rw-r--r--   0 vlad      (1000) vlad      (1000)     2294 2023-08-04 13:43:36.000000 types-aiobotocore-machinelearning-2.5.2.post2/types_aiobotocore_machinelearning/__init__.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)     2293 2023-08-04 13:43:36.000000 types-aiobotocore-machinelearning-2.5.2.post2/types_aiobotocore_machinelearning/__init__.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)      975 2023-08-04 13:43:36.000000 types-aiobotocore-machinelearning-2.5.2.post2/types_aiobotocore_machinelearning/__main__.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)    28039 2023-08-04 13:43:37.000000 types-aiobotocore-machinelearning-2.5.2.post2/types_aiobotocore_machinelearning/client.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)    27994 2023-08-04 13:43:36.000000 types-aiobotocore-machinelearning-2.5.2.post2/types_aiobotocore_machinelearning/client.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)    10382 2023-08-04 13:43:37.000000 types-aiobotocore-machinelearning-2.5.2.post2/types_aiobotocore_machinelearning/literals.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)    10380 2023-08-04 13:43:37.000000 types-aiobotocore-machinelearning-2.5.2.post2/types_aiobotocore_machinelearning/literals.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)     6983 2023-08-04 13:43:37.000000 types-aiobotocore-machinelearning-2.5.2.post2/types_aiobotocore_machinelearning/paginator.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)     6977 2023-08-04 13:43:37.000000 types-aiobotocore-machinelearning-2.5.2.post2/types_aiobotocore_machinelearning/paginator.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:43:36.000000 types-aiobotocore-machinelearning-2.5.2.post2/types_aiobotocore_machinelearning/py.typed
--rw-r--r--   0 vlad      (1000) vlad      (1000)    31653 2023-08-04 13:43:38.000000 types-aiobotocore-machinelearning-2.5.2.post2/types_aiobotocore_machinelearning/type_defs.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)    31628 2023-08-04 13:43:38.000000 types-aiobotocore-machinelearning-2.5.2.post2/types_aiobotocore_machinelearning/type_defs.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)       65 2023-08-04 13:43:36.000000 types-aiobotocore-machinelearning-2.5.2.post2/types_aiobotocore_machinelearning/version.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)     6335 2023-08-04 13:43:37.000000 types-aiobotocore-machinelearning-2.5.2.post2/types_aiobotocore_machinelearning/waiter.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)     6331 2023-08-04 13:43:37.000000 types-aiobotocore-machinelearning-2.5.2.post2/types_aiobotocore_machinelearning/waiter.pyi
-drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:16.366643 types-aiobotocore-machinelearning-2.5.2.post2/types_aiobotocore_machinelearning.egg-info/
--rw-r--r--   0 vlad      (1000) vlad      (1000)    15096 2023-08-04 13:59:16.000000 types-aiobotocore-machinelearning-2.5.2.post2/types_aiobotocore_machinelearning.egg-info/PKG-INFO
--rw-r--r--   0 vlad      (1000) vlad      (1000)     1054 2023-08-04 13:59:16.000000 types-aiobotocore-machinelearning-2.5.2.post2/types_aiobotocore_machinelearning.egg-info/SOURCES.txt
--rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:16.000000 types-aiobotocore-machinelearning-2.5.2.post2/types_aiobotocore_machinelearning.egg-info/dependency_links.txt
--rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:16.000000 types-aiobotocore-machinelearning-2.5.2.post2/types_aiobotocore_machinelearning.egg-info/not-zip-safe
--rw-r--r--   0 vlad      (1000) vlad      (1000)       52 2023-08-04 13:59:16.000000 types-aiobotocore-machinelearning-2.5.2.post2/types_aiobotocore_machinelearning.egg-info/requires.txt
--rw-r--r--   0 vlad      (1000) vlad      (1000)       34 2023-08-04 13:59:16.000000 types-aiobotocore-machinelearning-2.5.2.post2/types_aiobotocore_machinelearning.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:24:02.246725 types-aiobotocore-machinelearning-2.5.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-08 01:14:37.000000 types-aiobotocore-machinelearning-2.5.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    15090 2023-08-08 01:24:02.246725 types-aiobotocore-machinelearning-2.5.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    13546 2023-08-08 01:14:37.000000 types-aiobotocore-machinelearning-2.5.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-08 01:24:02.246725 types-aiobotocore-machinelearning-2.5.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2122 2023-08-08 01:14:37.000000 types-aiobotocore-machinelearning-2.5.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:24:02.226725 types-aiobotocore-machinelearning-2.5.4/types_aiobotocore_machinelearning/
+-rw-r--r--   0 runner    (1001) docker     (123)     2294 2023-08-08 01:14:37.000000 types-aiobotocore-machinelearning-2.5.4/types_aiobotocore_machinelearning/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2293 2023-08-08 01:14:37.000000 types-aiobotocore-machinelearning-2.5.4/types_aiobotocore_machinelearning/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      963 2023-08-08 01:14:37.000000 types-aiobotocore-machinelearning-2.5.4/types_aiobotocore_machinelearning/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28039 2023-08-08 01:14:37.000000 types-aiobotocore-machinelearning-2.5.4/types_aiobotocore_machinelearning/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27994 2023-08-08 01:14:37.000000 types-aiobotocore-machinelearning-2.5.4/types_aiobotocore_machinelearning/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    10382 2023-08-08 01:14:38.000000 types-aiobotocore-machinelearning-2.5.4/types_aiobotocore_machinelearning/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10380 2023-08-08 01:14:37.000000 types-aiobotocore-machinelearning-2.5.4/types_aiobotocore_machinelearning/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     6983 2023-08-08 01:14:37.000000 types-aiobotocore-machinelearning-2.5.4/types_aiobotocore_machinelearning/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6977 2023-08-08 01:14:37.000000 types-aiobotocore-machinelearning-2.5.4/types_aiobotocore_machinelearning/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 01:14:37.000000 types-aiobotocore-machinelearning-2.5.4/types_aiobotocore_machinelearning/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    31653 2023-08-08 01:14:40.000000 types-aiobotocore-machinelearning-2.5.4/types_aiobotocore_machinelearning/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31628 2023-08-08 01:14:40.000000 types-aiobotocore-machinelearning-2.5.4/types_aiobotocore_machinelearning/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-08-08 01:14:37.000000 types-aiobotocore-machinelearning-2.5.4/types_aiobotocore_machinelearning/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6335 2023-08-08 01:14:37.000000 types-aiobotocore-machinelearning-2.5.4/types_aiobotocore_machinelearning/waiter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6331 2023-08-08 01:14:37.000000 types-aiobotocore-machinelearning-2.5.4/types_aiobotocore_machinelearning/waiter.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:24:02.246725 types-aiobotocore-machinelearning-2.5.4/types_aiobotocore_machinelearning.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    15090 2023-08-08 01:24:02.000000 types-aiobotocore-machinelearning-2.5.4/types_aiobotocore_machinelearning.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1054 2023-08-08 01:24:02.000000 types-aiobotocore-machinelearning-2.5.4/types_aiobotocore_machinelearning.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 01:24:02.000000 types-aiobotocore-machinelearning-2.5.4/types_aiobotocore_machinelearning.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 01:24:02.000000 types-aiobotocore-machinelearning-2.5.4/types_aiobotocore_machinelearning.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-08 01:24:02.000000 types-aiobotocore-machinelearning-2.5.4/types_aiobotocore_machinelearning.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-08-08 01:24:02.000000 types-aiobotocore-machinelearning-2.5.4/types_aiobotocore_machinelearning.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-machinelearning-2.5.2.post2/LICENSE` & `types-aiobotocore-machinelearning-2.5.4/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-machinelearning-2.5.2.post2/PKG-INFO` & `types-aiobotocore-machinelearning-2.5.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-machinelearning
-Version: 2.5.2.post2
-Summary: Type annotations for aiobotocore.MachineLearning 2.5.2 service generated with mypy-boto3-builder 7.17.2
+Version: 2.5.4
+Summary: Type annotations for aiobotocore.MachineLearning 2.5.4 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_machinelearning/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-machinelearning.svg?color=blue)](https://pypi.org/project/types-aiobotocore-machinelearning)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_machinelearning/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-machinelearning)](https://pepy.tech/project/types-aiobotocore-machinelearning)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.MachineLearning 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/machinelearning.html#MachineLearning)
+[aiobotocore.MachineLearning 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/machinelearning.html#MachineLearning)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-machinelearning-2.5.2.post2/README.md` & `types-aiobotocore-machinelearning-2.5.4/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-machinelearning.svg?color=blue)](https://pypi.org/project/types-aiobotocore-machinelearning)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_machinelearning/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-machinelearning)](https://pepy.tech/project/types-aiobotocore-machinelearning)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.MachineLearning 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/machinelearning.html#MachineLearning)
+[aiobotocore.MachineLearning 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/machinelearning.html#MachineLearning)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-machinelearning-2.5.2.post2/setup.py` & `types-aiobotocore-machinelearning-2.5.4/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-machinelearning",
-    version="2.5.2.post2",
+    version="2.5.4",
     packages=["types_aiobotocore_machinelearning"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.MachineLearning 2.5.2 service generated with"
+        "Type annotations for aiobotocore.MachineLearning 2.5.4 service generated with"
         " mypy-boto3-builder 7.17.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
```

### Comparing `types-aiobotocore-machinelearning-2.5.2.post2/types_aiobotocore_machinelearning/__init__.py` & `types-aiobotocore-machinelearning-2.5.4/types_aiobotocore_machinelearning/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-machinelearning-2.5.2.post2/types_aiobotocore_machinelearning/__init__.pyi` & `types-aiobotocore-machinelearning-2.5.4/types_aiobotocore_machinelearning/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-machinelearning-2.5.2.post2/types_aiobotocore_machinelearning/__main__.py` & `types-aiobotocore-machinelearning-2.5.4/types_aiobotocore_machinelearning/__main__.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.MachineLearning 2.5.2\nVersion:        "
-        " 2.5.2.post2\nBuilder version: 7.17.2\nDocs:           "
+        "Type annotations for aiobotocore.MachineLearning 2.5.4\nVersion:         2.5.4\nBuilder"
+        " version: 7.17.2\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_machinelearning//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/machinelearning.html#MachineLearning\nOther"
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

### Comparing `types-aiobotocore-machinelearning-2.5.2.post2/types_aiobotocore_machinelearning/client.py` & `types-aiobotocore-machinelearning-2.5.4/types_aiobotocore_machinelearning/client.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-machinelearning-2.5.2.post2/types_aiobotocore_machinelearning/client.pyi` & `types-aiobotocore-machinelearning-2.5.4/types_aiobotocore_machinelearning/client.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-machinelearning-2.5.2.post2/types_aiobotocore_machinelearning/literals.py` & `types-aiobotocore-machinelearning-2.5.4/types_aiobotocore_machinelearning/literals.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-machinelearning-2.5.2.post2/types_aiobotocore_machinelearning/literals.pyi` & `types-aiobotocore-machinelearning-2.5.4/types_aiobotocore_machinelearning/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-machinelearning-2.5.2.post2/types_aiobotocore_machinelearning/paginator.py` & `types-aiobotocore-machinelearning-2.5.4/types_aiobotocore_machinelearning/paginator.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-machinelearning-2.5.2.post2/types_aiobotocore_machinelearning/paginator.pyi` & `types-aiobotocore-machinelearning-2.5.4/types_aiobotocore_machinelearning/paginator.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-machinelearning-2.5.2.post2/types_aiobotocore_machinelearning/type_defs.py` & `types-aiobotocore-machinelearning-2.5.4/types_aiobotocore_machinelearning/type_defs.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-machinelearning-2.5.2.post2/types_aiobotocore_machinelearning/type_defs.pyi` & `types-aiobotocore-machinelearning-2.5.4/types_aiobotocore_machinelearning/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-machinelearning-2.5.2.post2/types_aiobotocore_machinelearning/waiter.py` & `types-aiobotocore-machinelearning-2.5.4/types_aiobotocore_machinelearning/waiter.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-machinelearning-2.5.2.post2/types_aiobotocore_machinelearning/waiter.pyi` & `types-aiobotocore-machinelearning-2.5.4/types_aiobotocore_machinelearning/waiter.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-machinelearning-2.5.2.post2/types_aiobotocore_machinelearning.egg-info/PKG-INFO` & `types-aiobotocore-machinelearning-2.5.4/types_aiobotocore_machinelearning.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-machinelearning
-Version: 2.5.2.post2
-Summary: Type annotations for aiobotocore.MachineLearning 2.5.2 service generated with mypy-boto3-builder 7.17.2
+Version: 2.5.4
+Summary: Type annotations for aiobotocore.MachineLearning 2.5.4 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_machinelearning/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-machinelearning.svg?color=blue)](https://pypi.org/project/types-aiobotocore-machinelearning)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_machinelearning/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-machinelearning)](https://pepy.tech/project/types-aiobotocore-machinelearning)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.MachineLearning 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/machinelearning.html#MachineLearning)
+[aiobotocore.MachineLearning 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/machinelearning.html#MachineLearning)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-machinelearning-2.5.2.post2/types_aiobotocore_machinelearning.egg-info/SOURCES.txt` & `types-aiobotocore-machinelearning-2.5.4/types_aiobotocore_machinelearning.egg-info/SOURCES.txt`

 * *Files identical despite different names*


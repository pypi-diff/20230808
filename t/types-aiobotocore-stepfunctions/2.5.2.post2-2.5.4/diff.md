# Comparing `tmp/types-aiobotocore-stepfunctions-2.5.2.post2.tar.gz` & `tmp/types-aiobotocore-stepfunctions-2.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-stepfunctions-2.5.2.post2.tar", last modified: Fri Aug  4 13:59:28 2023, max compression
+gzip compressed data, was "types-aiobotocore-stepfunctions-2.5.4.tar", last modified: Tue Aug  8 01:24:31 2023, max compression
```

## Comparing `types-aiobotocore-stepfunctions-2.5.2.post2.tar` & `types-aiobotocore-stepfunctions-2.5.4.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:28.306643 types-aiobotocore-stepfunctions-2.5.2.post2/
--rw-r--r--   0 vlad      (1000) vlad      (1000)     1070 2023-08-04 13:54:35.000000 types-aiobotocore-stepfunctions-2.5.2.post2/LICENSE
--rw-r--r--   0 vlad      (1000) vlad      (1000)    13736 2023-08-04 13:59:28.306643 types-aiobotocore-stepfunctions-2.5.2.post2/PKG-INFO
--rw-r--r--   0 vlad      (1000) vlad      (1000)    12204 2023-08-04 13:54:35.000000 types-aiobotocore-stepfunctions-2.5.2.post2/README.md
--rw-r--r--   0 vlad      (1000) vlad      (1000)       38 2023-08-04 13:59:28.306643 types-aiobotocore-stepfunctions-2.5.2.post2/setup.cfg
--rw-r--r--   0 vlad      (1000) vlad      (1000)     2104 2023-08-04 13:54:35.000000 types-aiobotocore-stepfunctions-2.5.2.post2/setup.py
-drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:28.306643 types-aiobotocore-stepfunctions-2.5.2.post2/types_aiobotocore_stepfunctions/
--rw-r--r--   0 vlad      (1000) vlad      (1000)     1465 2023-08-04 13:54:35.000000 types-aiobotocore-stepfunctions-2.5.2.post2/types_aiobotocore_stepfunctions/__init__.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)     1464 2023-08-04 13:54:35.000000 types-aiobotocore-stepfunctions-2.5.2.post2/types_aiobotocore_stepfunctions/__init__.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)      947 2023-08-04 13:54:35.000000 types-aiobotocore-stepfunctions-2.5.2.post2/types_aiobotocore_stepfunctions/__main__.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)    30282 2023-08-04 13:54:36.000000 types-aiobotocore-stepfunctions-2.5.2.post2/types_aiobotocore_stepfunctions/client.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)    30234 2023-08-04 13:54:35.000000 types-aiobotocore-stepfunctions-2.5.2.post2/types_aiobotocore_stepfunctions/client.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)    10946 2023-08-04 13:54:36.000000 types-aiobotocore-stepfunctions-2.5.2.post2/types_aiobotocore_stepfunctions/literals.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)    10944 2023-08-04 13:54:36.000000 types-aiobotocore-stepfunctions-2.5.2.post2/types_aiobotocore_stepfunctions/literals.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)     6689 2023-08-04 13:54:36.000000 types-aiobotocore-stepfunctions-2.5.2.post2/types_aiobotocore_stepfunctions/paginator.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)     6682 2023-08-04 13:54:36.000000 types-aiobotocore-stepfunctions-2.5.2.post2/types_aiobotocore_stepfunctions/paginator.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:54:35.000000 types-aiobotocore-stepfunctions-2.5.2.post2/types_aiobotocore_stepfunctions/py.typed
--rw-r--r--   0 vlad      (1000) vlad      (1000)    43905 2023-08-04 13:54:37.000000 types-aiobotocore-stepfunctions-2.5.2.post2/types_aiobotocore_stepfunctions/type_defs.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)    43840 2023-08-04 13:54:36.000000 types-aiobotocore-stepfunctions-2.5.2.post2/types_aiobotocore_stepfunctions/type_defs.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)       65 2023-08-04 13:54:35.000000 types-aiobotocore-stepfunctions-2.5.2.post2/types_aiobotocore_stepfunctions/version.py
-drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:28.306643 types-aiobotocore-stepfunctions-2.5.2.post2/types_aiobotocore_stepfunctions.egg-info/
--rw-r--r--   0 vlad      (1000) vlad      (1000)    13736 2023-08-04 13:59:28.000000 types-aiobotocore-stepfunctions-2.5.2.post2/types_aiobotocore_stepfunctions.egg-info/PKG-INFO
--rw-r--r--   0 vlad      (1000) vlad      (1000)      927 2023-08-04 13:59:28.000000 types-aiobotocore-stepfunctions-2.5.2.post2/types_aiobotocore_stepfunctions.egg-info/SOURCES.txt
--rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:28.000000 types-aiobotocore-stepfunctions-2.5.2.post2/types_aiobotocore_stepfunctions.egg-info/dependency_links.txt
--rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:28.000000 types-aiobotocore-stepfunctions-2.5.2.post2/types_aiobotocore_stepfunctions.egg-info/not-zip-safe
--rw-r--r--   0 vlad      (1000) vlad      (1000)       52 2023-08-04 13:59:28.000000 types-aiobotocore-stepfunctions-2.5.2.post2/types_aiobotocore_stepfunctions.egg-info/requires.txt
--rw-r--r--   0 vlad      (1000) vlad      (1000)       32 2023-08-04 13:59:28.000000 types-aiobotocore-stepfunctions-2.5.2.post2/types_aiobotocore_stepfunctions.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:24:31.126792 types-aiobotocore-stepfunctions-2.5.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-08 01:21:44.000000 types-aiobotocore-stepfunctions-2.5.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    13730 2023-08-08 01:24:31.118792 types-aiobotocore-stepfunctions-2.5.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    12204 2023-08-08 01:21:44.000000 types-aiobotocore-stepfunctions-2.5.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-08 01:24:31.126792 types-aiobotocore-stepfunctions-2.5.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2098 2023-08-08 01:21:44.000000 types-aiobotocore-stepfunctions-2.5.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:24:31.118792 types-aiobotocore-stepfunctions-2.5.4/types_aiobotocore_stepfunctions/
+-rw-r--r--   0 runner    (1001) docker     (123)     1465 2023-08-08 01:21:44.000000 types-aiobotocore-stepfunctions-2.5.4/types_aiobotocore_stepfunctions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1464 2023-08-08 01:21:44.000000 types-aiobotocore-stepfunctions-2.5.4/types_aiobotocore_stepfunctions/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      935 2023-08-08 01:21:44.000000 types-aiobotocore-stepfunctions-2.5.4/types_aiobotocore_stepfunctions/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30282 2023-08-08 01:21:44.000000 types-aiobotocore-stepfunctions-2.5.4/types_aiobotocore_stepfunctions/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30234 2023-08-08 01:21:44.000000 types-aiobotocore-stepfunctions-2.5.4/types_aiobotocore_stepfunctions/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    10946 2023-08-08 01:21:44.000000 types-aiobotocore-stepfunctions-2.5.4/types_aiobotocore_stepfunctions/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10944 2023-08-08 01:21:44.000000 types-aiobotocore-stepfunctions-2.5.4/types_aiobotocore_stepfunctions/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     6689 2023-08-08 01:21:44.000000 types-aiobotocore-stepfunctions-2.5.4/types_aiobotocore_stepfunctions/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6682 2023-08-08 01:21:44.000000 types-aiobotocore-stepfunctions-2.5.4/types_aiobotocore_stepfunctions/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 01:21:44.000000 types-aiobotocore-stepfunctions-2.5.4/types_aiobotocore_stepfunctions/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    43905 2023-08-08 01:21:45.000000 types-aiobotocore-stepfunctions-2.5.4/types_aiobotocore_stepfunctions/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    43840 2023-08-08 01:21:45.000000 types-aiobotocore-stepfunctions-2.5.4/types_aiobotocore_stepfunctions/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-08-08 01:21:44.000000 types-aiobotocore-stepfunctions-2.5.4/types_aiobotocore_stepfunctions/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:24:31.118792 types-aiobotocore-stepfunctions-2.5.4/types_aiobotocore_stepfunctions.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    13730 2023-08-08 01:24:30.000000 types-aiobotocore-stepfunctions-2.5.4/types_aiobotocore_stepfunctions.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      927 2023-08-08 01:24:30.000000 types-aiobotocore-stepfunctions-2.5.4/types_aiobotocore_stepfunctions.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 01:24:30.000000 types-aiobotocore-stepfunctions-2.5.4/types_aiobotocore_stepfunctions.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 01:24:30.000000 types-aiobotocore-stepfunctions-2.5.4/types_aiobotocore_stepfunctions.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-08 01:24:30.000000 types-aiobotocore-stepfunctions-2.5.4/types_aiobotocore_stepfunctions.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-08-08 01:24:30.000000 types-aiobotocore-stepfunctions-2.5.4/types_aiobotocore_stepfunctions.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-stepfunctions-2.5.2.post2/LICENSE` & `types-aiobotocore-stepfunctions-2.5.4/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-stepfunctions-2.5.2.post2/PKG-INFO` & `types-aiobotocore-stepfunctions-2.5.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-stepfunctions
-Version: 2.5.2.post2
-Summary: Type annotations for aiobotocore.SFN 2.5.2 service generated with mypy-boto3-builder 7.17.2
+Version: 2.5.4
+Summary: Type annotations for aiobotocore.SFN 2.5.4 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_stepfunctions/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-stepfunctions.svg?color=blue)](https://pypi.org/project/types-aiobotocore-stepfunctions)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_stepfunctions/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-stepfunctions)](https://pepy.tech/project/types-aiobotocore-stepfunctions)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.SFN 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/stepfunctions.html#SFN)
+[aiobotocore.SFN 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/stepfunctions.html#SFN)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-stepfunctions-2.5.2.post2/README.md` & `types-aiobotocore-stepfunctions-2.5.4/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-stepfunctions.svg?color=blue)](https://pypi.org/project/types-aiobotocore-stepfunctions)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_stepfunctions/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-stepfunctions)](https://pepy.tech/project/types-aiobotocore-stepfunctions)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.SFN 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/stepfunctions.html#SFN)
+[aiobotocore.SFN 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/stepfunctions.html#SFN)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-stepfunctions-2.5.2.post2/setup.py` & `types-aiobotocore-stepfunctions-2.5.4/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-stepfunctions",
-    version="2.5.2.post2",
+    version="2.5.4",
     packages=["types_aiobotocore_stepfunctions"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.SFN 2.5.2 service generated with mypy-boto3-builder"
+        "Type annotations for aiobotocore.SFN 2.5.4 service generated with mypy-boto3-builder"
         " 7.17.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
```

### Comparing `types-aiobotocore-stepfunctions-2.5.2.post2/types_aiobotocore_stepfunctions/__init__.py` & `types-aiobotocore-stepfunctions-2.5.4/types_aiobotocore_stepfunctions/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-stepfunctions-2.5.2.post2/types_aiobotocore_stepfunctions/__init__.pyi` & `types-aiobotocore-stepfunctions-2.5.4/types_aiobotocore_stepfunctions/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-stepfunctions-2.5.2.post2/types_aiobotocore_stepfunctions/__main__.py` & `types-aiobotocore-stepfunctions-2.5.4/types_aiobotocore_stepfunctions/__main__.py`

 * *Files 13% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.SFN 2.5.2\nVersion:         2.5.2.post2\nBuilder version:"
+        "Type annotations for aiobotocore.SFN 2.5.4\nVersion:         2.5.4\nBuilder version:"
         " 7.17.2\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_stepfunctions//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/stepfunctions.html#SFN\nOther"
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

### Comparing `types-aiobotocore-stepfunctions-2.5.2.post2/types_aiobotocore_stepfunctions/client.py` & `types-aiobotocore-stepfunctions-2.5.4/types_aiobotocore_stepfunctions/client.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-stepfunctions-2.5.2.post2/types_aiobotocore_stepfunctions/client.pyi` & `types-aiobotocore-stepfunctions-2.5.4/types_aiobotocore_stepfunctions/client.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-stepfunctions-2.5.2.post2/types_aiobotocore_stepfunctions/literals.py` & `types-aiobotocore-stepfunctions-2.5.4/types_aiobotocore_stepfunctions/literals.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-stepfunctions-2.5.2.post2/types_aiobotocore_stepfunctions/literals.pyi` & `types-aiobotocore-stepfunctions-2.5.4/types_aiobotocore_stepfunctions/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-stepfunctions-2.5.2.post2/types_aiobotocore_stepfunctions/paginator.py` & `types-aiobotocore-stepfunctions-2.5.4/types_aiobotocore_stepfunctions/paginator.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-stepfunctions-2.5.2.post2/types_aiobotocore_stepfunctions/paginator.pyi` & `types-aiobotocore-stepfunctions-2.5.4/types_aiobotocore_stepfunctions/paginator.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-stepfunctions-2.5.2.post2/types_aiobotocore_stepfunctions/type_defs.py` & `types-aiobotocore-stepfunctions-2.5.4/types_aiobotocore_stepfunctions/type_defs.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-stepfunctions-2.5.2.post2/types_aiobotocore_stepfunctions/type_defs.pyi` & `types-aiobotocore-stepfunctions-2.5.4/types_aiobotocore_stepfunctions/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-stepfunctions-2.5.2.post2/types_aiobotocore_stepfunctions.egg-info/PKG-INFO` & `types-aiobotocore-stepfunctions-2.5.4/types_aiobotocore_stepfunctions.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-stepfunctions
-Version: 2.5.2.post2
-Summary: Type annotations for aiobotocore.SFN 2.5.2 service generated with mypy-boto3-builder 7.17.2
+Version: 2.5.4
+Summary: Type annotations for aiobotocore.SFN 2.5.4 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_stepfunctions/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-stepfunctions.svg?color=blue)](https://pypi.org/project/types-aiobotocore-stepfunctions)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_stepfunctions/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-stepfunctions)](https://pepy.tech/project/types-aiobotocore-stepfunctions)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.SFN 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/stepfunctions.html#SFN)
+[aiobotocore.SFN 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/stepfunctions.html#SFN)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-stepfunctions-2.5.2.post2/types_aiobotocore_stepfunctions.egg-info/SOURCES.txt` & `types-aiobotocore-stepfunctions-2.5.4/types_aiobotocore_stepfunctions.egg-info/SOURCES.txt`

 * *Files identical despite different names*


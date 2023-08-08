# Comparing `tmp/types-aiobotocore-macie2-2.5.2.post2.tar.gz` & `tmp/types-aiobotocore-macie2-2.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-macie2-2.5.2.post2.tar", last modified: Fri Aug  4 13:59:16 2023, max compression
+gzip compressed data, was "types-aiobotocore-macie2-2.5.4.tar", last modified: Tue Aug  8 01:24:02 2023, max compression
```

## Comparing `types-aiobotocore-macie2-2.5.2.post2.tar` & `types-aiobotocore-macie2-2.5.4.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:16.296643 types-aiobotocore-macie2-2.5.2.post2/
--rw-r--r--   0 vlad      (1000) vlad      (1000)     1070 2023-08-04 13:43:42.000000 types-aiobotocore-macie2-2.5.2.post2/LICENSE
--rw-r--r--   0 vlad      (1000) vlad      (1000)    16082 2023-08-04 13:59:16.296643 types-aiobotocore-macie2-2.5.2.post2/PKG-INFO
--rw-r--r--   0 vlad      (1000) vlad      (1000)    14568 2023-08-04 13:43:42.000000 types-aiobotocore-macie2-2.5.2.post2/README.md
--rw-r--r--   0 vlad      (1000) vlad      (1000)       38 2023-08-04 13:59:16.296643 types-aiobotocore-macie2-2.5.2.post2/setup.cfg
--rw-r--r--   0 vlad      (1000) vlad      (1000)     2065 2023-08-04 13:43:41.000000 types-aiobotocore-macie2-2.5.2.post2/setup.py
-drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:16.286643 types-aiobotocore-macie2-2.5.2.post2/types_aiobotocore_macie2/
--rw-r--r--   0 vlad      (1000) vlad      (1000)     4413 2023-08-04 13:43:42.000000 types-aiobotocore-macie2-2.5.2.post2/types_aiobotocore_macie2/__init__.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)     4412 2023-08-04 13:43:42.000000 types-aiobotocore-macie2-2.5.2.post2/types_aiobotocore_macie2/__init__.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)      928 2023-08-04 13:43:42.000000 types-aiobotocore-macie2-2.5.2.post2/types_aiobotocore_macie2/__main__.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)    63125 2023-08-04 13:43:43.000000 types-aiobotocore-macie2-2.5.2.post2/types_aiobotocore_macie2/client.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)    63020 2023-08-04 13:43:43.000000 types-aiobotocore-macie2-2.5.2.post2/types_aiobotocore_macie2/client.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)    17444 2023-08-04 13:43:44.000000 types-aiobotocore-macie2-2.5.2.post2/types_aiobotocore_macie2/literals.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)    17442 2023-08-04 13:43:43.000000 types-aiobotocore-macie2-2.5.2.post2/types_aiobotocore_macie2/literals.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)    20353 2023-08-04 13:43:43.000000 types-aiobotocore-macie2-2.5.2.post2/types_aiobotocore_macie2/paginator.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)    20335 2023-08-04 13:43:43.000000 types-aiobotocore-macie2-2.5.2.post2/types_aiobotocore_macie2/paginator.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:43:42.000000 types-aiobotocore-macie2-2.5.2.post2/types_aiobotocore_macie2/py.typed
--rw-r--r--   0 vlad      (1000) vlad      (1000)    88777 2023-08-04 13:43:47.000000 types-aiobotocore-macie2-2.5.2.post2/types_aiobotocore_macie2/type_defs.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)    88722 2023-08-04 13:43:45.000000 types-aiobotocore-macie2-2.5.2.post2/types_aiobotocore_macie2/type_defs.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)       65 2023-08-04 13:43:42.000000 types-aiobotocore-macie2-2.5.2.post2/types_aiobotocore_macie2/version.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)     1516 2023-08-04 13:43:43.000000 types-aiobotocore-macie2-2.5.2.post2/types_aiobotocore_macie2/waiter.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)     1515 2023-08-04 13:43:43.000000 types-aiobotocore-macie2-2.5.2.post2/types_aiobotocore_macie2/waiter.pyi
-drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:16.296643 types-aiobotocore-macie2-2.5.2.post2/types_aiobotocore_macie2.egg-info/
--rw-r--r--   0 vlad      (1000) vlad      (1000)    16082 2023-08-04 13:59:16.000000 types-aiobotocore-macie2-2.5.2.post2/types_aiobotocore_macie2.egg-info/PKG-INFO
--rw-r--r--   0 vlad      (1000) vlad      (1000)      865 2023-08-04 13:59:16.000000 types-aiobotocore-macie2-2.5.2.post2/types_aiobotocore_macie2.egg-info/SOURCES.txt
--rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:16.000000 types-aiobotocore-macie2-2.5.2.post2/types_aiobotocore_macie2.egg-info/dependency_links.txt
--rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:16.000000 types-aiobotocore-macie2-2.5.2.post2/types_aiobotocore_macie2.egg-info/not-zip-safe
--rw-r--r--   0 vlad      (1000) vlad      (1000)       52 2023-08-04 13:59:16.000000 types-aiobotocore-macie2-2.5.2.post2/types_aiobotocore_macie2.egg-info/requires.txt
--rw-r--r--   0 vlad      (1000) vlad      (1000)       25 2023-08-04 13:59:16.000000 types-aiobotocore-macie2-2.5.2.post2/types_aiobotocore_macie2.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:24:02.418725 types-aiobotocore-macie2-2.5.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-08 01:14:41.000000 types-aiobotocore-macie2-2.5.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    16076 2023-08-08 01:24:02.418725 types-aiobotocore-macie2-2.5.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    14568 2023-08-08 01:14:41.000000 types-aiobotocore-macie2-2.5.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-08 01:24:02.418725 types-aiobotocore-macie2-2.5.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2059 2023-08-08 01:14:41.000000 types-aiobotocore-macie2-2.5.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:24:02.414725 types-aiobotocore-macie2-2.5.4/types_aiobotocore_macie2/
+-rw-r--r--   0 runner    (1001) docker     (123)     4413 2023-08-08 01:14:41.000000 types-aiobotocore-macie2-2.5.4/types_aiobotocore_macie2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4412 2023-08-08 01:14:41.000000 types-aiobotocore-macie2-2.5.4/types_aiobotocore_macie2/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      916 2023-08-08 01:14:41.000000 types-aiobotocore-macie2-2.5.4/types_aiobotocore_macie2/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    63125 2023-08-08 01:14:42.000000 types-aiobotocore-macie2-2.5.4/types_aiobotocore_macie2/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    63020 2023-08-08 01:14:42.000000 types-aiobotocore-macie2-2.5.4/types_aiobotocore_macie2/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    17444 2023-08-08 01:14:42.000000 types-aiobotocore-macie2-2.5.4/types_aiobotocore_macie2/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17442 2023-08-08 01:14:42.000000 types-aiobotocore-macie2-2.5.4/types_aiobotocore_macie2/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    20353 2023-08-08 01:14:42.000000 types-aiobotocore-macie2-2.5.4/types_aiobotocore_macie2/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20335 2023-08-08 01:14:42.000000 types-aiobotocore-macie2-2.5.4/types_aiobotocore_macie2/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 01:14:41.000000 types-aiobotocore-macie2-2.5.4/types_aiobotocore_macie2/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    88777 2023-08-08 01:14:44.000000 types-aiobotocore-macie2-2.5.4/types_aiobotocore_macie2/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    88722 2023-08-08 01:14:43.000000 types-aiobotocore-macie2-2.5.4/types_aiobotocore_macie2/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-08-08 01:14:41.000000 types-aiobotocore-macie2-2.5.4/types_aiobotocore_macie2/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1516 2023-08-08 01:14:42.000000 types-aiobotocore-macie2-2.5.4/types_aiobotocore_macie2/waiter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1515 2023-08-08 01:14:42.000000 types-aiobotocore-macie2-2.5.4/types_aiobotocore_macie2/waiter.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:24:02.414725 types-aiobotocore-macie2-2.5.4/types_aiobotocore_macie2.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    16076 2023-08-08 01:24:02.000000 types-aiobotocore-macie2-2.5.4/types_aiobotocore_macie2.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      865 2023-08-08 01:24:02.000000 types-aiobotocore-macie2-2.5.4/types_aiobotocore_macie2.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 01:24:02.000000 types-aiobotocore-macie2-2.5.4/types_aiobotocore_macie2.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 01:24:02.000000 types-aiobotocore-macie2-2.5.4/types_aiobotocore_macie2.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-08 01:24:02.000000 types-aiobotocore-macie2-2.5.4/types_aiobotocore_macie2.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-08-08 01:24:02.000000 types-aiobotocore-macie2-2.5.4/types_aiobotocore_macie2.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-macie2-2.5.2.post2/LICENSE` & `types-aiobotocore-macie2-2.5.4/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-macie2-2.5.2.post2/PKG-INFO` & `types-aiobotocore-macie2-2.5.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-macie2
-Version: 2.5.2.post2
-Summary: Type annotations for aiobotocore.Macie2 2.5.2 service generated with mypy-boto3-builder 7.17.2
+Version: 2.5.4
+Summary: Type annotations for aiobotocore.Macie2 2.5.4 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_macie2/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-macie2.svg?color=blue)](https://pypi.org/project/types-aiobotocore-macie2)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_macie2/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-macie2)](https://pepy.tech/project/types-aiobotocore-macie2)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.Macie2 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/macie2.html#Macie2)
+[aiobotocore.Macie2 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/macie2.html#Macie2)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-macie2-2.5.2.post2/README.md` & `types-aiobotocore-macie2-2.5.4/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-macie2.svg?color=blue)](https://pypi.org/project/types-aiobotocore-macie2)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_macie2/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-macie2)](https://pepy.tech/project/types-aiobotocore-macie2)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.Macie2 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/macie2.html#Macie2)
+[aiobotocore.Macie2 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/macie2.html#Macie2)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-macie2-2.5.2.post2/setup.py` & `types-aiobotocore-macie2-2.5.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-macie2",
-    version="2.5.2.post2",
+    version="2.5.4",
     packages=["types_aiobotocore_macie2"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.Macie2 2.5.2 service generated with mypy-boto3-builder"
+        "Type annotations for aiobotocore.Macie2 2.5.4 service generated with mypy-boto3-builder"
         " 7.17.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
```

### Comparing `types-aiobotocore-macie2-2.5.2.post2/types_aiobotocore_macie2/__init__.py` & `types-aiobotocore-macie2-2.5.4/types_aiobotocore_macie2/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-macie2-2.5.2.post2/types_aiobotocore_macie2/__init__.pyi` & `types-aiobotocore-macie2-2.5.4/types_aiobotocore_macie2/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-macie2-2.5.2.post2/types_aiobotocore_macie2/__main__.py` & `types-aiobotocore-macie2-2.5.4/types_aiobotocore_macie2/__main__.py`

 * *Files 15% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.Macie2 2.5.2\nVersion:         2.5.2.post2\nBuilder"
-        " version: 7.17.2\nDocs:           "
+        "Type annotations for aiobotocore.Macie2 2.5.4\nVersion:         2.5.4\nBuilder version:"
+        " 7.17.2\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_macie2//\nBoto3 docs: "
         "     https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/macie2.html#Macie2\nOther"
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

### Comparing `types-aiobotocore-macie2-2.5.2.post2/types_aiobotocore_macie2/client.py` & `types-aiobotocore-macie2-2.5.4/types_aiobotocore_macie2/client.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-macie2-2.5.2.post2/types_aiobotocore_macie2/client.pyi` & `types-aiobotocore-macie2-2.5.4/types_aiobotocore_macie2/client.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-macie2-2.5.2.post2/types_aiobotocore_macie2/literals.py` & `types-aiobotocore-macie2-2.5.4/types_aiobotocore_macie2/literals.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-macie2-2.5.2.post2/types_aiobotocore_macie2/literals.pyi` & `types-aiobotocore-macie2-2.5.4/types_aiobotocore_macie2/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-macie2-2.5.2.post2/types_aiobotocore_macie2/paginator.py` & `types-aiobotocore-macie2-2.5.4/types_aiobotocore_macie2/paginator.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-macie2-2.5.2.post2/types_aiobotocore_macie2/paginator.pyi` & `types-aiobotocore-macie2-2.5.4/types_aiobotocore_macie2/paginator.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-macie2-2.5.2.post2/types_aiobotocore_macie2/type_defs.py` & `types-aiobotocore-macie2-2.5.4/types_aiobotocore_macie2/type_defs.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-macie2-2.5.2.post2/types_aiobotocore_macie2/type_defs.pyi` & `types-aiobotocore-macie2-2.5.4/types_aiobotocore_macie2/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-macie2-2.5.2.post2/types_aiobotocore_macie2/waiter.py` & `types-aiobotocore-macie2-2.5.4/types_aiobotocore_macie2/waiter.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-macie2-2.5.2.post2/types_aiobotocore_macie2/waiter.pyi` & `types-aiobotocore-macie2-2.5.4/types_aiobotocore_macie2/waiter.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-macie2-2.5.2.post2/types_aiobotocore_macie2.egg-info/PKG-INFO` & `types-aiobotocore-macie2-2.5.4/types_aiobotocore_macie2.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-macie2
-Version: 2.5.2.post2
-Summary: Type annotations for aiobotocore.Macie2 2.5.2 service generated with mypy-boto3-builder 7.17.2
+Version: 2.5.4
+Summary: Type annotations for aiobotocore.Macie2 2.5.4 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_macie2/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-macie2.svg?color=blue)](https://pypi.org/project/types-aiobotocore-macie2)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_macie2/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-macie2)](https://pepy.tech/project/types-aiobotocore-macie2)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.Macie2 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/macie2.html#Macie2)
+[aiobotocore.Macie2 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/macie2.html#Macie2)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-macie2-2.5.2.post2/types_aiobotocore_macie2.egg-info/SOURCES.txt` & `types-aiobotocore-macie2-2.5.4/types_aiobotocore_macie2.egg-info/SOURCES.txt`

 * *Files identical despite different names*


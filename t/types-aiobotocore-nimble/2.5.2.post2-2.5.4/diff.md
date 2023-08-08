# Comparing `tmp/types-aiobotocore-nimble-2.5.2.post2.tar.gz` & `tmp/types-aiobotocore-nimble-2.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-nimble-2.5.2.post2.tar", last modified: Fri Aug  4 13:59:19 2023, max compression
+gzip compressed data, was "types-aiobotocore-nimble-2.5.4.tar", last modified: Tue Aug  8 01:24:10 2023, max compression
```

## Comparing `types-aiobotocore-nimble-2.5.2.post2.tar` & `types-aiobotocore-nimble-2.5.4.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:19.616643 types-aiobotocore-nimble-2.5.2.post2/
--rw-r--r--   0 vlad      (1000) vlad      (1000)     1070 2023-08-04 13:45:43.000000 types-aiobotocore-nimble-2.5.2.post2/LICENSE
--rw-r--r--   0 vlad      (1000) vlad      (1000)    16801 2023-08-04 13:59:19.616643 types-aiobotocore-nimble-2.5.2.post2/PKG-INFO
--rw-r--r--   0 vlad      (1000) vlad      (1000)    15281 2023-08-04 13:45:43.000000 types-aiobotocore-nimble-2.5.2.post2/README.md
--rw-r--r--   0 vlad      (1000) vlad      (1000)       38 2023-08-04 13:59:19.616643 types-aiobotocore-nimble-2.5.2.post2/setup.cfg
--rw-r--r--   0 vlad      (1000) vlad      (1000)     2071 2023-08-04 13:45:43.000000 types-aiobotocore-nimble-2.5.2.post2/setup.py
-drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:19.616643 types-aiobotocore-nimble-2.5.2.post2/types_aiobotocore_nimble/
--rw-r--r--   0 vlad      (1000) vlad      (1000)     5224 2023-08-04 13:45:43.000000 types-aiobotocore-nimble-2.5.2.post2/types_aiobotocore_nimble/__init__.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)     5223 2023-08-04 13:45:43.000000 types-aiobotocore-nimble-2.5.2.post2/types_aiobotocore_nimble/__init__.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)      940 2023-08-04 13:45:43.000000 types-aiobotocore-nimble-2.5.2.post2/types_aiobotocore_nimble/__main__.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)    47143 2023-08-04 13:45:45.000000 types-aiobotocore-nimble-2.5.2.post2/types_aiobotocore_nimble/client.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)    47063 2023-08-04 13:45:44.000000 types-aiobotocore-nimble-2.5.2.post2/types_aiobotocore_nimble/client.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)    18174 2023-08-04 13:45:45.000000 types-aiobotocore-nimble-2.5.2.post2/types_aiobotocore_nimble/literals.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)    18172 2023-08-04 13:45:45.000000 types-aiobotocore-nimble-2.5.2.post2/types_aiobotocore_nimble/literals.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)    12886 2023-08-04 13:45:45.000000 types-aiobotocore-nimble-2.5.2.post2/types_aiobotocore_nimble/paginator.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)    12874 2023-08-04 13:45:45.000000 types-aiobotocore-nimble-2.5.2.post2/types_aiobotocore_nimble/paginator.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:45:43.000000 types-aiobotocore-nimble-2.5.2.post2/types_aiobotocore_nimble/py.typed
--rw-r--r--   0 vlad      (1000) vlad      (1000)    70018 2023-08-04 13:45:47.000000 types-aiobotocore-nimble-2.5.2.post2/types_aiobotocore_nimble/type_defs.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)    69901 2023-08-04 13:45:46.000000 types-aiobotocore-nimble-2.5.2.post2/types_aiobotocore_nimble/type_defs.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)       65 2023-08-04 13:45:43.000000 types-aiobotocore-nimble-2.5.2.post2/types_aiobotocore_nimble/version.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)    13016 2023-08-04 13:45:45.000000 types-aiobotocore-nimble-2.5.2.post2/types_aiobotocore_nimble/waiter.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)    13004 2023-08-04 13:45:45.000000 types-aiobotocore-nimble-2.5.2.post2/types_aiobotocore_nimble/waiter.pyi
-drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:19.616643 types-aiobotocore-nimble-2.5.2.post2/types_aiobotocore_nimble.egg-info/
--rw-r--r--   0 vlad      (1000) vlad      (1000)    16801 2023-08-04 13:59:19.000000 types-aiobotocore-nimble-2.5.2.post2/types_aiobotocore_nimble.egg-info/PKG-INFO
--rw-r--r--   0 vlad      (1000) vlad      (1000)      865 2023-08-04 13:59:19.000000 types-aiobotocore-nimble-2.5.2.post2/types_aiobotocore_nimble.egg-info/SOURCES.txt
--rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:19.000000 types-aiobotocore-nimble-2.5.2.post2/types_aiobotocore_nimble.egg-info/dependency_links.txt
--rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:19.000000 types-aiobotocore-nimble-2.5.2.post2/types_aiobotocore_nimble.egg-info/not-zip-safe
--rw-r--r--   0 vlad      (1000) vlad      (1000)       52 2023-08-04 13:59:19.000000 types-aiobotocore-nimble-2.5.2.post2/types_aiobotocore_nimble.egg-info/requires.txt
--rw-r--r--   0 vlad      (1000) vlad      (1000)       25 2023-08-04 13:59:19.000000 types-aiobotocore-nimble-2.5.2.post2/types_aiobotocore_nimble.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:24:10.034742 types-aiobotocore-nimble-2.5.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-08 01:15:58.000000 types-aiobotocore-nimble-2.5.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    16795 2023-08-08 01:24:10.034742 types-aiobotocore-nimble-2.5.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    15281 2023-08-08 01:15:58.000000 types-aiobotocore-nimble-2.5.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-08 01:24:10.034742 types-aiobotocore-nimble-2.5.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2065 2023-08-08 01:15:58.000000 types-aiobotocore-nimble-2.5.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:24:10.034742 types-aiobotocore-nimble-2.5.4/types_aiobotocore_nimble/
+-rw-r--r--   0 runner    (1001) docker     (123)     5224 2023-08-08 01:15:58.000000 types-aiobotocore-nimble-2.5.4/types_aiobotocore_nimble/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5223 2023-08-08 01:15:58.000000 types-aiobotocore-nimble-2.5.4/types_aiobotocore_nimble/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      928 2023-08-08 01:15:58.000000 types-aiobotocore-nimble-2.5.4/types_aiobotocore_nimble/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    47143 2023-08-08 01:15:58.000000 types-aiobotocore-nimble-2.5.4/types_aiobotocore_nimble/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    47063 2023-08-08 01:15:58.000000 types-aiobotocore-nimble-2.5.4/types_aiobotocore_nimble/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    18174 2023-08-08 01:15:59.000000 types-aiobotocore-nimble-2.5.4/types_aiobotocore_nimble/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18172 2023-08-08 01:15:59.000000 types-aiobotocore-nimble-2.5.4/types_aiobotocore_nimble/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    12886 2023-08-08 01:15:59.000000 types-aiobotocore-nimble-2.5.4/types_aiobotocore_nimble/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12874 2023-08-08 01:15:59.000000 types-aiobotocore-nimble-2.5.4/types_aiobotocore_nimble/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 01:15:58.000000 types-aiobotocore-nimble-2.5.4/types_aiobotocore_nimble/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    70018 2023-08-08 01:16:00.000000 types-aiobotocore-nimble-2.5.4/types_aiobotocore_nimble/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    69901 2023-08-08 01:16:00.000000 types-aiobotocore-nimble-2.5.4/types_aiobotocore_nimble/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-08-08 01:15:58.000000 types-aiobotocore-nimble-2.5.4/types_aiobotocore_nimble/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13016 2023-08-08 01:15:59.000000 types-aiobotocore-nimble-2.5.4/types_aiobotocore_nimble/waiter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13004 2023-08-08 01:15:59.000000 types-aiobotocore-nimble-2.5.4/types_aiobotocore_nimble/waiter.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:24:10.034742 types-aiobotocore-nimble-2.5.4/types_aiobotocore_nimble.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    16795 2023-08-08 01:24:09.000000 types-aiobotocore-nimble-2.5.4/types_aiobotocore_nimble.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      865 2023-08-08 01:24:09.000000 types-aiobotocore-nimble-2.5.4/types_aiobotocore_nimble.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 01:24:09.000000 types-aiobotocore-nimble-2.5.4/types_aiobotocore_nimble.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 01:24:09.000000 types-aiobotocore-nimble-2.5.4/types_aiobotocore_nimble.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-08 01:24:09.000000 types-aiobotocore-nimble-2.5.4/types_aiobotocore_nimble.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-08-08 01:24:09.000000 types-aiobotocore-nimble-2.5.4/types_aiobotocore_nimble.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-nimble-2.5.2.post2/LICENSE` & `types-aiobotocore-nimble-2.5.4/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-nimble-2.5.2.post2/PKG-INFO` & `types-aiobotocore-nimble-2.5.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-nimble
-Version: 2.5.2.post2
-Summary: Type annotations for aiobotocore.NimbleStudio 2.5.2 service generated with mypy-boto3-builder 7.17.2
+Version: 2.5.4
+Summary: Type annotations for aiobotocore.NimbleStudio 2.5.4 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_nimble/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-nimble.svg?color=blue)](https://pypi.org/project/types-aiobotocore-nimble)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_nimble/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-nimble)](https://pepy.tech/project/types-aiobotocore-nimble)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.NimbleStudio 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/nimble.html#NimbleStudio)
+[aiobotocore.NimbleStudio 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/nimble.html#NimbleStudio)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-nimble-2.5.2.post2/README.md` & `types-aiobotocore-nimble-2.5.4/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-nimble.svg?color=blue)](https://pypi.org/project/types-aiobotocore-nimble)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_nimble/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-nimble)](https://pepy.tech/project/types-aiobotocore-nimble)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.NimbleStudio 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/nimble.html#NimbleStudio)
+[aiobotocore.NimbleStudio 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/nimble.html#NimbleStudio)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-nimble-2.5.2.post2/setup.py` & `types-aiobotocore-nimble-2.5.4/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-nimble",
-    version="2.5.2.post2",
+    version="2.5.4",
     packages=["types_aiobotocore_nimble"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.NimbleStudio 2.5.2 service generated with"
+        "Type annotations for aiobotocore.NimbleStudio 2.5.4 service generated with"
         " mypy-boto3-builder 7.17.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
```

### Comparing `types-aiobotocore-nimble-2.5.2.post2/types_aiobotocore_nimble/__init__.py` & `types-aiobotocore-nimble-2.5.4/types_aiobotocore_nimble/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-nimble-2.5.2.post2/types_aiobotocore_nimble/__init__.pyi` & `types-aiobotocore-nimble-2.5.4/types_aiobotocore_nimble/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-nimble-2.5.2.post2/types_aiobotocore_nimble/__main__.py` & `types-aiobotocore-nimble-2.5.4/types_aiobotocore_nimble/__main__.py`

 * *Files 15% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.NimbleStudio 2.5.2\nVersion:         2.5.2.post2\nBuilder"
+        "Type annotations for aiobotocore.NimbleStudio 2.5.4\nVersion:         2.5.4\nBuilder"
         " version: 7.17.2\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_nimble//\nBoto3 docs: "
         "     https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/nimble.html#NimbleStudio\nOther"
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

### Comparing `types-aiobotocore-nimble-2.5.2.post2/types_aiobotocore_nimble/client.py` & `types-aiobotocore-nimble-2.5.4/types_aiobotocore_nimble/client.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-nimble-2.5.2.post2/types_aiobotocore_nimble/client.pyi` & `types-aiobotocore-nimble-2.5.4/types_aiobotocore_nimble/client.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-nimble-2.5.2.post2/types_aiobotocore_nimble/literals.py` & `types-aiobotocore-nimble-2.5.4/types_aiobotocore_nimble/literals.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-nimble-2.5.2.post2/types_aiobotocore_nimble/literals.pyi` & `types-aiobotocore-nimble-2.5.4/types_aiobotocore_nimble/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-nimble-2.5.2.post2/types_aiobotocore_nimble/paginator.py` & `types-aiobotocore-nimble-2.5.4/types_aiobotocore_nimble/paginator.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-nimble-2.5.2.post2/types_aiobotocore_nimble/paginator.pyi` & `types-aiobotocore-nimble-2.5.4/types_aiobotocore_nimble/paginator.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-nimble-2.5.2.post2/types_aiobotocore_nimble/type_defs.py` & `types-aiobotocore-nimble-2.5.4/types_aiobotocore_nimble/type_defs.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-nimble-2.5.2.post2/types_aiobotocore_nimble/type_defs.pyi` & `types-aiobotocore-nimble-2.5.4/types_aiobotocore_nimble/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-nimble-2.5.2.post2/types_aiobotocore_nimble/waiter.py` & `types-aiobotocore-nimble-2.5.4/types_aiobotocore_nimble/waiter.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-nimble-2.5.2.post2/types_aiobotocore_nimble/waiter.pyi` & `types-aiobotocore-nimble-2.5.4/types_aiobotocore_nimble/waiter.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-nimble-2.5.2.post2/types_aiobotocore_nimble.egg-info/PKG-INFO` & `types-aiobotocore-nimble-2.5.4/types_aiobotocore_nimble.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-nimble
-Version: 2.5.2.post2
-Summary: Type annotations for aiobotocore.NimbleStudio 2.5.2 service generated with mypy-boto3-builder 7.17.2
+Version: 2.5.4
+Summary: Type annotations for aiobotocore.NimbleStudio 2.5.4 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_nimble/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-nimble.svg?color=blue)](https://pypi.org/project/types-aiobotocore-nimble)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_nimble/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-nimble)](https://pepy.tech/project/types-aiobotocore-nimble)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.NimbleStudio 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/nimble.html#NimbleStudio)
+[aiobotocore.NimbleStudio 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/nimble.html#NimbleStudio)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-nimble-2.5.2.post2/types_aiobotocore_nimble.egg-info/SOURCES.txt` & `types-aiobotocore-nimble-2.5.4/types_aiobotocore_nimble.egg-info/SOURCES.txt`

 * *Files identical despite different names*


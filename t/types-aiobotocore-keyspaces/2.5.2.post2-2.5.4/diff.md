# Comparing `tmp/types-aiobotocore-keyspaces-2.5.2.post2.tar.gz` & `tmp/types-aiobotocore-keyspaces-2.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-keyspaces-2.5.2.post2.tar", last modified: Fri Aug  4 13:59:14 2023, max compression
+gzip compressed data, was "types-aiobotocore-keyspaces-2.5.4.tar", last modified: Tue Aug  8 01:23:57 2023, max compression
```

## Comparing `types-aiobotocore-keyspaces-2.5.2.post2.tar` & `types-aiobotocore-keyspaces-2.5.4.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:14.116643 types-aiobotocore-keyspaces-2.5.2.post2/
--rw-r--r--   0 vlad      (1000) vlad      (1000)     1070 2023-08-04 13:41:54.000000 types-aiobotocore-keyspaces-2.5.2.post2/LICENSE
--rw-r--r--   0 vlad      (1000) vlad      (1000)    13348 2023-08-04 13:59:14.116643 types-aiobotocore-keyspaces-2.5.2.post2/PKG-INFO
--rw-r--r--   0 vlad      (1000) vlad      (1000)    11822 2023-08-04 13:41:54.000000 types-aiobotocore-keyspaces-2.5.2.post2/README.md
--rw-r--r--   0 vlad      (1000) vlad      (1000)       38 2023-08-04 13:59:14.116643 types-aiobotocore-keyspaces-2.5.2.post2/setup.cfg
--rw-r--r--   0 vlad      (1000) vlad      (1000)     2086 2023-08-04 13:41:54.000000 types-aiobotocore-keyspaces-2.5.2.post2/setup.py
-drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:14.116643 types-aiobotocore-keyspaces-2.5.2.post2/types_aiobotocore_keyspaces/
--rw-r--r--   0 vlad      (1000) vlad      (1000)     1054 2023-08-04 13:41:54.000000 types-aiobotocore-keyspaces-2.5.2.post2/types_aiobotocore_keyspaces/__init__.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)     1053 2023-08-04 13:41:54.000000 types-aiobotocore-keyspaces-2.5.2.post2/types_aiobotocore_keyspaces/__init__.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)      951 2023-08-04 13:41:54.000000 types-aiobotocore-keyspaces-2.5.2.post2/types_aiobotocore_keyspaces/__main__.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)    14806 2023-08-04 13:41:54.000000 types-aiobotocore-keyspaces-2.5.2.post2/types_aiobotocore_keyspaces/client.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)    14781 2023-08-04 13:41:54.000000 types-aiobotocore-keyspaces-2.5.2.post2/types_aiobotocore_keyspaces/client.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)     9176 2023-08-04 13:41:54.000000 types-aiobotocore-keyspaces-2.5.2.post2/types_aiobotocore_keyspaces/literals.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)     9174 2023-08-04 13:41:54.000000 types-aiobotocore-keyspaces-2.5.2.post2/types_aiobotocore_keyspaces/literals.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)     4190 2023-08-04 13:41:54.000000 types-aiobotocore-keyspaces-2.5.2.post2/types_aiobotocore_keyspaces/paginator.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)     4185 2023-08-04 13:41:54.000000 types-aiobotocore-keyspaces-2.5.2.post2/types_aiobotocore_keyspaces/paginator.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:41:54.000000 types-aiobotocore-keyspaces-2.5.2.post2/types_aiobotocore_keyspaces/py.typed
--rw-r--r--   0 vlad      (1000) vlad      (1000)    16671 2023-08-04 13:41:56.000000 types-aiobotocore-keyspaces-2.5.2.post2/types_aiobotocore_keyspaces/type_defs.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)    16640 2023-08-04 13:41:55.000000 types-aiobotocore-keyspaces-2.5.2.post2/types_aiobotocore_keyspaces/type_defs.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)       65 2023-08-04 13:41:54.000000 types-aiobotocore-keyspaces-2.5.2.post2/types_aiobotocore_keyspaces/version.py
-drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:14.116643 types-aiobotocore-keyspaces-2.5.2.post2/types_aiobotocore_keyspaces.egg-info/
--rw-r--r--   0 vlad      (1000) vlad      (1000)    13348 2023-08-04 13:59:14.000000 types-aiobotocore-keyspaces-2.5.2.post2/types_aiobotocore_keyspaces.egg-info/PKG-INFO
--rw-r--r--   0 vlad      (1000) vlad      (1000)      851 2023-08-04 13:59:14.000000 types-aiobotocore-keyspaces-2.5.2.post2/types_aiobotocore_keyspaces.egg-info/SOURCES.txt
--rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:14.000000 types-aiobotocore-keyspaces-2.5.2.post2/types_aiobotocore_keyspaces.egg-info/dependency_links.txt
--rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:14.000000 types-aiobotocore-keyspaces-2.5.2.post2/types_aiobotocore_keyspaces.egg-info/not-zip-safe
--rw-r--r--   0 vlad      (1000) vlad      (1000)       52 2023-08-04 13:59:14.000000 types-aiobotocore-keyspaces-2.5.2.post2/types_aiobotocore_keyspaces.egg-info/requires.txt
--rw-r--r--   0 vlad      (1000) vlad      (1000)       28 2023-08-04 13:59:14.000000 types-aiobotocore-keyspaces-2.5.2.post2/types_aiobotocore_keyspaces.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:23:57.038717 types-aiobotocore-keyspaces-2.5.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-08 01:13:31.000000 types-aiobotocore-keyspaces-2.5.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    13342 2023-08-08 01:23:57.038717 types-aiobotocore-keyspaces-2.5.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    11822 2023-08-08 01:13:31.000000 types-aiobotocore-keyspaces-2.5.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-08 01:23:57.038717 types-aiobotocore-keyspaces-2.5.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2080 2023-08-08 01:13:31.000000 types-aiobotocore-keyspaces-2.5.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:23:57.038717 types-aiobotocore-keyspaces-2.5.4/types_aiobotocore_keyspaces/
+-rw-r--r--   0 runner    (1001) docker     (123)     1054 2023-08-08 01:13:31.000000 types-aiobotocore-keyspaces-2.5.4/types_aiobotocore_keyspaces/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1053 2023-08-08 01:13:31.000000 types-aiobotocore-keyspaces-2.5.4/types_aiobotocore_keyspaces/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      939 2023-08-08 01:13:31.000000 types-aiobotocore-keyspaces-2.5.4/types_aiobotocore_keyspaces/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14806 2023-08-08 01:13:31.000000 types-aiobotocore-keyspaces-2.5.4/types_aiobotocore_keyspaces/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14781 2023-08-08 01:13:31.000000 types-aiobotocore-keyspaces-2.5.4/types_aiobotocore_keyspaces/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9176 2023-08-08 01:13:31.000000 types-aiobotocore-keyspaces-2.5.4/types_aiobotocore_keyspaces/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9174 2023-08-08 01:13:31.000000 types-aiobotocore-keyspaces-2.5.4/types_aiobotocore_keyspaces/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     4190 2023-08-08 01:13:31.000000 types-aiobotocore-keyspaces-2.5.4/types_aiobotocore_keyspaces/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4185 2023-08-08 01:13:31.000000 types-aiobotocore-keyspaces-2.5.4/types_aiobotocore_keyspaces/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 01:13:31.000000 types-aiobotocore-keyspaces-2.5.4/types_aiobotocore_keyspaces/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    16671 2023-08-08 01:13:32.000000 types-aiobotocore-keyspaces-2.5.4/types_aiobotocore_keyspaces/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16640 2023-08-08 01:13:31.000000 types-aiobotocore-keyspaces-2.5.4/types_aiobotocore_keyspaces/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-08-08 01:13:31.000000 types-aiobotocore-keyspaces-2.5.4/types_aiobotocore_keyspaces/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:23:57.038717 types-aiobotocore-keyspaces-2.5.4/types_aiobotocore_keyspaces.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    13342 2023-08-08 01:23:56.000000 types-aiobotocore-keyspaces-2.5.4/types_aiobotocore_keyspaces.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      851 2023-08-08 01:23:56.000000 types-aiobotocore-keyspaces-2.5.4/types_aiobotocore_keyspaces.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 01:23:56.000000 types-aiobotocore-keyspaces-2.5.4/types_aiobotocore_keyspaces.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 01:23:56.000000 types-aiobotocore-keyspaces-2.5.4/types_aiobotocore_keyspaces.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-08 01:23:56.000000 types-aiobotocore-keyspaces-2.5.4/types_aiobotocore_keyspaces.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-08-08 01:23:56.000000 types-aiobotocore-keyspaces-2.5.4/types_aiobotocore_keyspaces.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-keyspaces-2.5.2.post2/LICENSE` & `types-aiobotocore-keyspaces-2.5.4/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-keyspaces-2.5.2.post2/PKG-INFO` & `types-aiobotocore-keyspaces-2.5.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-keyspaces
-Version: 2.5.2.post2
-Summary: Type annotations for aiobotocore.Keyspaces 2.5.2 service generated with mypy-boto3-builder 7.17.2
+Version: 2.5.4
+Summary: Type annotations for aiobotocore.Keyspaces 2.5.4 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_keyspaces/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-keyspaces.svg?color=blue)](https://pypi.org/project/types-aiobotocore-keyspaces)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_keyspaces/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-keyspaces)](https://pepy.tech/project/types-aiobotocore-keyspaces)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.Keyspaces 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/keyspaces.html#Keyspaces)
+[aiobotocore.Keyspaces 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/keyspaces.html#Keyspaces)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-keyspaces-2.5.2.post2/README.md` & `types-aiobotocore-keyspaces-2.5.4/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-keyspaces.svg?color=blue)](https://pypi.org/project/types-aiobotocore-keyspaces)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_keyspaces/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-keyspaces)](https://pepy.tech/project/types-aiobotocore-keyspaces)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.Keyspaces 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/keyspaces.html#Keyspaces)
+[aiobotocore.Keyspaces 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/keyspaces.html#Keyspaces)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-keyspaces-2.5.2.post2/setup.py` & `types-aiobotocore-keyspaces-2.5.4/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-keyspaces",
-    version="2.5.2.post2",
+    version="2.5.4",
     packages=["types_aiobotocore_keyspaces"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.Keyspaces 2.5.2 service generated with mypy-boto3-builder"
+        "Type annotations for aiobotocore.Keyspaces 2.5.4 service generated with mypy-boto3-builder"
         " 7.17.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
```

### Comparing `types-aiobotocore-keyspaces-2.5.2.post2/types_aiobotocore_keyspaces/__init__.py` & `types-aiobotocore-keyspaces-2.5.4/types_aiobotocore_keyspaces/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-keyspaces-2.5.2.post2/types_aiobotocore_keyspaces/__init__.pyi` & `types-aiobotocore-keyspaces-2.5.4/types_aiobotocore_keyspaces/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-keyspaces-2.5.2.post2/types_aiobotocore_keyspaces/__main__.py` & `types-aiobotocore-keyspaces-2.5.4/types_aiobotocore_keyspaces/__main__.py`

 * *Files 9% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.Keyspaces 2.5.2\nVersion:         2.5.2.post2\nBuilder"
-        " version: 7.17.2\nDocs:           "
+        "Type annotations for aiobotocore.Keyspaces 2.5.4\nVersion:         2.5.4\nBuilder version:"
+        " 7.17.2\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_keyspaces//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/keyspaces.html#Keyspaces\nOther"
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

### Comparing `types-aiobotocore-keyspaces-2.5.2.post2/types_aiobotocore_keyspaces/client.py` & `types-aiobotocore-keyspaces-2.5.4/types_aiobotocore_keyspaces/client.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-keyspaces-2.5.2.post2/types_aiobotocore_keyspaces/client.pyi` & `types-aiobotocore-keyspaces-2.5.4/types_aiobotocore_keyspaces/client.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-keyspaces-2.5.2.post2/types_aiobotocore_keyspaces/literals.py` & `types-aiobotocore-keyspaces-2.5.4/types_aiobotocore_keyspaces/literals.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-keyspaces-2.5.2.post2/types_aiobotocore_keyspaces/literals.pyi` & `types-aiobotocore-keyspaces-2.5.4/types_aiobotocore_keyspaces/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-keyspaces-2.5.2.post2/types_aiobotocore_keyspaces/paginator.py` & `types-aiobotocore-keyspaces-2.5.4/types_aiobotocore_keyspaces/paginator.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-keyspaces-2.5.2.post2/types_aiobotocore_keyspaces/paginator.pyi` & `types-aiobotocore-keyspaces-2.5.4/types_aiobotocore_keyspaces/paginator.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-keyspaces-2.5.2.post2/types_aiobotocore_keyspaces/type_defs.py` & `types-aiobotocore-keyspaces-2.5.4/types_aiobotocore_keyspaces/type_defs.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-keyspaces-2.5.2.post2/types_aiobotocore_keyspaces/type_defs.pyi` & `types-aiobotocore-keyspaces-2.5.4/types_aiobotocore_keyspaces/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-keyspaces-2.5.2.post2/types_aiobotocore_keyspaces.egg-info/PKG-INFO` & `types-aiobotocore-keyspaces-2.5.4/types_aiobotocore_keyspaces.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-keyspaces
-Version: 2.5.2.post2
-Summary: Type annotations for aiobotocore.Keyspaces 2.5.2 service generated with mypy-boto3-builder 7.17.2
+Version: 2.5.4
+Summary: Type annotations for aiobotocore.Keyspaces 2.5.4 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_keyspaces/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-keyspaces.svg?color=blue)](https://pypi.org/project/types-aiobotocore-keyspaces)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_keyspaces/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-keyspaces)](https://pepy.tech/project/types-aiobotocore-keyspaces)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.Keyspaces 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/keyspaces.html#Keyspaces)
+[aiobotocore.Keyspaces 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/keyspaces.html#Keyspaces)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-keyspaces-2.5.2.post2/types_aiobotocore_keyspaces.egg-info/SOURCES.txt` & `types-aiobotocore-keyspaces-2.5.4/types_aiobotocore_keyspaces.egg-info/SOURCES.txt`

 * *Files identical despite different names*


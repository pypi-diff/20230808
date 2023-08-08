# Comparing `tmp/types-aiobotocore-networkmanager-2.5.2.post2.tar.gz` & `tmp/types-aiobotocore-networkmanager-2.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-networkmanager-2.5.2.post2.tar", last modified: Fri Aug  4 13:59:19 2023, max compression
+gzip compressed data, was "types-aiobotocore-networkmanager-2.5.4.tar", last modified: Tue Aug  8 01:24:09 2023, max compression
```

## Comparing `types-aiobotocore-networkmanager-2.5.2.post2.tar` & `types-aiobotocore-networkmanager-2.5.4.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:19.466643 types-aiobotocore-networkmanager-2.5.2.post2/
--rw-r--r--   0 vlad      (1000) vlad      (1000)     1070 2023-08-04 13:45:36.000000 types-aiobotocore-networkmanager-2.5.2.post2/LICENSE
--rw-r--r--   0 vlad      (1000) vlad      (1000)    16689 2023-08-04 13:59:19.466643 types-aiobotocore-networkmanager-2.5.2.post2/PKG-INFO
--rw-r--r--   0 vlad      (1000) vlad      (1000)    15143 2023-08-04 13:45:36.000000 types-aiobotocore-networkmanager-2.5.2.post2/README.md
--rw-r--r--   0 vlad      (1000) vlad      (1000)       38 2023-08-04 13:59:19.466643 types-aiobotocore-networkmanager-2.5.2.post2/setup.cfg
--rw-r--r--   0 vlad      (1000) vlad      (1000)     2121 2023-08-04 13:45:36.000000 types-aiobotocore-networkmanager-2.5.2.post2/setup.py
-drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:19.466643 types-aiobotocore-networkmanager-2.5.2.post2/types_aiobotocore_networkmanager/
--rw-r--r--   0 vlad      (1000) vlad      (1000)     5443 2023-08-04 13:45:36.000000 types-aiobotocore-networkmanager-2.5.2.post2/types_aiobotocore_networkmanager/__init__.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)     5442 2023-08-04 13:45:36.000000 types-aiobotocore-networkmanager-2.5.2.post2/types_aiobotocore_networkmanager/__init__.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)      971 2023-08-04 13:45:36.000000 types-aiobotocore-networkmanager-2.5.2.post2/types_aiobotocore_networkmanager/__main__.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)    73474 2023-08-04 13:45:37.000000 types-aiobotocore-networkmanager-2.5.2.post2/types_aiobotocore_networkmanager/client.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)    73359 2023-08-04 13:45:37.000000 types-aiobotocore-networkmanager-2.5.2.post2/types_aiobotocore_networkmanager/client.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)    14728 2023-08-04 13:45:39.000000 types-aiobotocore-networkmanager-2.5.2.post2/types_aiobotocore_networkmanager/literals.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)    14726 2023-08-04 13:45:39.000000 types-aiobotocore-networkmanager-2.5.2.post2/types_aiobotocore_networkmanager/literals.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)    28537 2023-08-04 13:45:37.000000 types-aiobotocore-networkmanager-2.5.2.post2/types_aiobotocore_networkmanager/paginator.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)    28513 2023-08-04 13:45:37.000000 types-aiobotocore-networkmanager-2.5.2.post2/types_aiobotocore_networkmanager/paginator.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:45:36.000000 types-aiobotocore-networkmanager-2.5.2.post2/types_aiobotocore_networkmanager/py.typed
--rw-r--r--   0 vlad      (1000) vlad      (1000)    95682 2023-08-04 13:45:41.000000 types-aiobotocore-networkmanager-2.5.2.post2/types_aiobotocore_networkmanager/type_defs.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)    95565 2023-08-04 13:45:40.000000 types-aiobotocore-networkmanager-2.5.2.post2/types_aiobotocore_networkmanager/type_defs.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)       65 2023-08-04 13:45:36.000000 types-aiobotocore-networkmanager-2.5.2.post2/types_aiobotocore_networkmanager/version.py
-drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:19.466643 types-aiobotocore-networkmanager-2.5.2.post2/types_aiobotocore_networkmanager.egg-info/
--rw-r--r--   0 vlad      (1000) vlad      (1000)    16689 2023-08-04 13:59:19.000000 types-aiobotocore-networkmanager-2.5.2.post2/types_aiobotocore_networkmanager.egg-info/PKG-INFO
--rw-r--r--   0 vlad      (1000) vlad      (1000)      946 2023-08-04 13:59:19.000000 types-aiobotocore-networkmanager-2.5.2.post2/types_aiobotocore_networkmanager.egg-info/SOURCES.txt
--rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:19.000000 types-aiobotocore-networkmanager-2.5.2.post2/types_aiobotocore_networkmanager.egg-info/dependency_links.txt
--rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:19.000000 types-aiobotocore-networkmanager-2.5.2.post2/types_aiobotocore_networkmanager.egg-info/not-zip-safe
--rw-r--r--   0 vlad      (1000) vlad      (1000)       52 2023-08-04 13:59:19.000000 types-aiobotocore-networkmanager-2.5.2.post2/types_aiobotocore_networkmanager.egg-info/requires.txt
--rw-r--r--   0 vlad      (1000) vlad      (1000)       33 2023-08-04 13:59:19.000000 types-aiobotocore-networkmanager-2.5.2.post2/types_aiobotocore_networkmanager.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:24:09.390741 types-aiobotocore-networkmanager-2.5.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-08 01:15:53.000000 types-aiobotocore-networkmanager-2.5.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    16683 2023-08-08 01:24:09.386741 types-aiobotocore-networkmanager-2.5.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    15143 2023-08-08 01:15:53.000000 types-aiobotocore-networkmanager-2.5.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-08 01:24:09.390741 types-aiobotocore-networkmanager-2.5.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2115 2023-08-08 01:15:53.000000 types-aiobotocore-networkmanager-2.5.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:24:09.386741 types-aiobotocore-networkmanager-2.5.4/types_aiobotocore_networkmanager/
+-rw-r--r--   0 runner    (1001) docker     (123)     5443 2023-08-08 01:15:53.000000 types-aiobotocore-networkmanager-2.5.4/types_aiobotocore_networkmanager/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5442 2023-08-08 01:15:53.000000 types-aiobotocore-networkmanager-2.5.4/types_aiobotocore_networkmanager/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      959 2023-08-08 01:15:53.000000 types-aiobotocore-networkmanager-2.5.4/types_aiobotocore_networkmanager/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    73474 2023-08-08 01:15:53.000000 types-aiobotocore-networkmanager-2.5.4/types_aiobotocore_networkmanager/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    73359 2023-08-08 01:15:53.000000 types-aiobotocore-networkmanager-2.5.4/types_aiobotocore_networkmanager/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    14728 2023-08-08 01:15:56.000000 types-aiobotocore-networkmanager-2.5.4/types_aiobotocore_networkmanager/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14726 2023-08-08 01:15:55.000000 types-aiobotocore-networkmanager-2.5.4/types_aiobotocore_networkmanager/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    28537 2023-08-08 01:15:55.000000 types-aiobotocore-networkmanager-2.5.4/types_aiobotocore_networkmanager/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28513 2023-08-08 01:15:53.000000 types-aiobotocore-networkmanager-2.5.4/types_aiobotocore_networkmanager/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 01:15:53.000000 types-aiobotocore-networkmanager-2.5.4/types_aiobotocore_networkmanager/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    95682 2023-08-08 01:15:57.000000 types-aiobotocore-networkmanager-2.5.4/types_aiobotocore_networkmanager/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    95565 2023-08-08 01:15:56.000000 types-aiobotocore-networkmanager-2.5.4/types_aiobotocore_networkmanager/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-08-08 01:15:53.000000 types-aiobotocore-networkmanager-2.5.4/types_aiobotocore_networkmanager/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:24:09.386741 types-aiobotocore-networkmanager-2.5.4/types_aiobotocore_networkmanager.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    16683 2023-08-08 01:24:09.000000 types-aiobotocore-networkmanager-2.5.4/types_aiobotocore_networkmanager.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      946 2023-08-08 01:24:09.000000 types-aiobotocore-networkmanager-2.5.4/types_aiobotocore_networkmanager.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 01:24:09.000000 types-aiobotocore-networkmanager-2.5.4/types_aiobotocore_networkmanager.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 01:24:09.000000 types-aiobotocore-networkmanager-2.5.4/types_aiobotocore_networkmanager.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-08 01:24:09.000000 types-aiobotocore-networkmanager-2.5.4/types_aiobotocore_networkmanager.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-08-08 01:24:09.000000 types-aiobotocore-networkmanager-2.5.4/types_aiobotocore_networkmanager.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-networkmanager-2.5.2.post2/LICENSE` & `types-aiobotocore-networkmanager-2.5.4/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-networkmanager-2.5.2.post2/PKG-INFO` & `types-aiobotocore-networkmanager-2.5.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-networkmanager
-Version: 2.5.2.post2
-Summary: Type annotations for aiobotocore.NetworkManager 2.5.2 service generated with mypy-boto3-builder 7.17.2
+Version: 2.5.4
+Summary: Type annotations for aiobotocore.NetworkManager 2.5.4 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_networkmanager/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-networkmanager.svg?color=blue)](https://pypi.org/project/types-aiobotocore-networkmanager)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_networkmanager/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-networkmanager)](https://pepy.tech/project/types-aiobotocore-networkmanager)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.NetworkManager 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/networkmanager.html#NetworkManager)
+[aiobotocore.NetworkManager 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/networkmanager.html#NetworkManager)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-networkmanager-2.5.2.post2/README.md` & `types-aiobotocore-networkmanager-2.5.4/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-networkmanager.svg?color=blue)](https://pypi.org/project/types-aiobotocore-networkmanager)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_networkmanager/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-networkmanager)](https://pepy.tech/project/types-aiobotocore-networkmanager)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.NetworkManager 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/networkmanager.html#NetworkManager)
+[aiobotocore.NetworkManager 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/networkmanager.html#NetworkManager)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-networkmanager-2.5.2.post2/setup.py` & `types-aiobotocore-networkmanager-2.5.4/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-networkmanager",
-    version="2.5.2.post2",
+    version="2.5.4",
     packages=["types_aiobotocore_networkmanager"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.NetworkManager 2.5.2 service generated with"
+        "Type annotations for aiobotocore.NetworkManager 2.5.4 service generated with"
         " mypy-boto3-builder 7.17.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
```

### Comparing `types-aiobotocore-networkmanager-2.5.2.post2/types_aiobotocore_networkmanager/__init__.py` & `types-aiobotocore-networkmanager-2.5.4/types_aiobotocore_networkmanager/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-networkmanager-2.5.2.post2/types_aiobotocore_networkmanager/__init__.pyi` & `types-aiobotocore-networkmanager-2.5.4/types_aiobotocore_networkmanager/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-networkmanager-2.5.2.post2/types_aiobotocore_networkmanager/__main__.py` & `types-aiobotocore-networkmanager-2.5.4/types_aiobotocore_networkmanager/__main__.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.NetworkManager 2.5.2\nVersion:        "
-        " 2.5.2.post2\nBuilder version: 7.17.2\nDocs:           "
+        "Type annotations for aiobotocore.NetworkManager 2.5.4\nVersion:         2.5.4\nBuilder"
+        " version: 7.17.2\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_networkmanager//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/networkmanager.html#NetworkManager\nOther"
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

### Comparing `types-aiobotocore-networkmanager-2.5.2.post2/types_aiobotocore_networkmanager/client.py` & `types-aiobotocore-networkmanager-2.5.4/types_aiobotocore_networkmanager/client.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-networkmanager-2.5.2.post2/types_aiobotocore_networkmanager/client.pyi` & `types-aiobotocore-networkmanager-2.5.4/types_aiobotocore_networkmanager/client.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-networkmanager-2.5.2.post2/types_aiobotocore_networkmanager/literals.py` & `types-aiobotocore-networkmanager-2.5.4/types_aiobotocore_networkmanager/literals.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-networkmanager-2.5.2.post2/types_aiobotocore_networkmanager/literals.pyi` & `types-aiobotocore-networkmanager-2.5.4/types_aiobotocore_networkmanager/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-networkmanager-2.5.2.post2/types_aiobotocore_networkmanager/paginator.py` & `types-aiobotocore-networkmanager-2.5.4/types_aiobotocore_networkmanager/paginator.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-networkmanager-2.5.2.post2/types_aiobotocore_networkmanager/paginator.pyi` & `types-aiobotocore-networkmanager-2.5.4/types_aiobotocore_networkmanager/paginator.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-networkmanager-2.5.2.post2/types_aiobotocore_networkmanager/type_defs.py` & `types-aiobotocore-networkmanager-2.5.4/types_aiobotocore_networkmanager/type_defs.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-networkmanager-2.5.2.post2/types_aiobotocore_networkmanager/type_defs.pyi` & `types-aiobotocore-networkmanager-2.5.4/types_aiobotocore_networkmanager/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-networkmanager-2.5.2.post2/types_aiobotocore_networkmanager.egg-info/PKG-INFO` & `types-aiobotocore-networkmanager-2.5.4/types_aiobotocore_networkmanager.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-networkmanager
-Version: 2.5.2.post2
-Summary: Type annotations for aiobotocore.NetworkManager 2.5.2 service generated with mypy-boto3-builder 7.17.2
+Version: 2.5.4
+Summary: Type annotations for aiobotocore.NetworkManager 2.5.4 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_networkmanager/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-networkmanager.svg?color=blue)](https://pypi.org/project/types-aiobotocore-networkmanager)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_networkmanager/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-networkmanager)](https://pepy.tech/project/types-aiobotocore-networkmanager)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.NetworkManager 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/networkmanager.html#NetworkManager)
+[aiobotocore.NetworkManager 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/networkmanager.html#NetworkManager)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-networkmanager-2.5.2.post2/types_aiobotocore_networkmanager.egg-info/SOURCES.txt` & `types-aiobotocore-networkmanager-2.5.4/types_aiobotocore_networkmanager.egg-info/SOURCES.txt`

 * *Files identical despite different names*


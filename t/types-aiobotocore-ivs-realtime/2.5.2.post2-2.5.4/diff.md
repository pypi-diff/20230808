# Comparing `tmp/types-aiobotocore-ivs-realtime-2.5.2.post2.tar.gz` & `tmp/types-aiobotocore-ivs-realtime-2.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-ivs-realtime-2.5.2.post2.tar", last modified: Fri Aug  4 13:59:13 2023, max compression
+gzip compressed data, was "types-aiobotocore-ivs-realtime-2.5.4.tar", last modified: Tue Aug  8 01:23:54 2023, max compression
```

## Comparing `types-aiobotocore-ivs-realtime-2.5.2.post2.tar` & `types-aiobotocore-ivs-realtime-2.5.4.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:13.276642 types-aiobotocore-ivs-realtime-2.5.2.post2/
--rw-r--r--   0 vlad      (1000) vlad      (1000)     1070 2023-08-04 13:41:33.000000 types-aiobotocore-ivs-realtime-2.5.2.post2/LICENSE
--rw-r--r--   0 vlad      (1000) vlad      (1000)    12488 2023-08-04 13:59:13.276642 types-aiobotocore-ivs-realtime-2.5.2.post2/PKG-INFO
--rw-r--r--   0 vlad      (1000) vlad      (1000)    10951 2023-08-04 13:41:33.000000 types-aiobotocore-ivs-realtime-2.5.2.post2/README.md
--rw-r--r--   0 vlad      (1000) vlad      (1000)       38 2023-08-04 13:59:13.276642 types-aiobotocore-ivs-realtime-2.5.2.post2/setup.cfg
--rw-r--r--   0 vlad      (1000) vlad      (1000)     2106 2023-08-04 13:41:33.000000 types-aiobotocore-ivs-realtime-2.5.2.post2/setup.py
-drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:13.276642 types-aiobotocore-ivs-realtime-2.5.2.post2/types_aiobotocore_ivs_realtime/
--rw-r--r--   0 vlad      (1000) vlad      (1000)      477 2023-08-04 13:41:33.000000 types-aiobotocore-ivs-realtime-2.5.2.post2/types_aiobotocore_ivs_realtime/__init__.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)      476 2023-08-04 13:41:33.000000 types-aiobotocore-ivs-realtime-2.5.2.post2/types_aiobotocore_ivs_realtime/__init__.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)      961 2023-08-04 13:41:33.000000 types-aiobotocore-ivs-realtime-2.5.2.post2/types_aiobotocore_ivs_realtime/__main__.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)    13425 2023-08-04 13:41:33.000000 types-aiobotocore-ivs-realtime-2.5.2.post2/types_aiobotocore_ivs_realtime/client.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)    13402 2023-08-04 13:41:33.000000 types-aiobotocore-ivs-realtime-2.5.2.post2/types_aiobotocore_ivs_realtime/client.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)     8343 2023-08-04 13:41:34.000000 types-aiobotocore-ivs-realtime-2.5.2.post2/types_aiobotocore_ivs_realtime/literals.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)     8341 2023-08-04 13:41:33.000000 types-aiobotocore-ivs-realtime-2.5.2.post2/types_aiobotocore_ivs_realtime/literals.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:41:33.000000 types-aiobotocore-ivs-realtime-2.5.2.post2/types_aiobotocore_ivs_realtime/py.typed
--rw-r--r--   0 vlad      (1000) vlad      (1000)    12189 2023-08-04 13:41:34.000000 types-aiobotocore-ivs-realtime-2.5.2.post2/types_aiobotocore_ivs_realtime/type_defs.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)    12172 2023-08-04 13:41:34.000000 types-aiobotocore-ivs-realtime-2.5.2.post2/types_aiobotocore_ivs_realtime/type_defs.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)       65 2023-08-04 13:41:33.000000 types-aiobotocore-ivs-realtime-2.5.2.post2/types_aiobotocore_ivs_realtime/version.py
-drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:13.276642 types-aiobotocore-ivs-realtime-2.5.2.post2/types_aiobotocore_ivs_realtime.egg-info/
--rw-r--r--   0 vlad      (1000) vlad      (1000)    12488 2023-08-04 13:59:13.000000 types-aiobotocore-ivs-realtime-2.5.2.post2/types_aiobotocore_ivs_realtime.egg-info/PKG-INFO
--rw-r--r--   0 vlad      (1000) vlad      (1000)      819 2023-08-04 13:59:13.000000 types-aiobotocore-ivs-realtime-2.5.2.post2/types_aiobotocore_ivs_realtime.egg-info/SOURCES.txt
--rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:13.000000 types-aiobotocore-ivs-realtime-2.5.2.post2/types_aiobotocore_ivs_realtime.egg-info/dependency_links.txt
--rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:13.000000 types-aiobotocore-ivs-realtime-2.5.2.post2/types_aiobotocore_ivs_realtime.egg-info/not-zip-safe
--rw-r--r--   0 vlad      (1000) vlad      (1000)       52 2023-08-04 13:59:13.000000 types-aiobotocore-ivs-realtime-2.5.2.post2/types_aiobotocore_ivs_realtime.egg-info/requires.txt
--rw-r--r--   0 vlad      (1000) vlad      (1000)       31 2023-08-04 13:59:13.000000 types-aiobotocore-ivs-realtime-2.5.2.post2/types_aiobotocore_ivs_realtime.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:23:54.978711 types-aiobotocore-ivs-realtime-2.5.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-08 01:13:18.000000 types-aiobotocore-ivs-realtime-2.5.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    12482 2023-08-08 01:23:54.978711 types-aiobotocore-ivs-realtime-2.5.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10951 2023-08-08 01:13:18.000000 types-aiobotocore-ivs-realtime-2.5.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-08 01:23:54.978711 types-aiobotocore-ivs-realtime-2.5.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2100 2023-08-08 01:13:18.000000 types-aiobotocore-ivs-realtime-2.5.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:23:54.958711 types-aiobotocore-ivs-realtime-2.5.4/types_aiobotocore_ivs_realtime/
+-rw-r--r--   0 runner    (1001) docker     (123)      477 2023-08-08 01:13:18.000000 types-aiobotocore-ivs-realtime-2.5.4/types_aiobotocore_ivs_realtime/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      476 2023-08-08 01:13:18.000000 types-aiobotocore-ivs-realtime-2.5.4/types_aiobotocore_ivs_realtime/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      949 2023-08-08 01:13:18.000000 types-aiobotocore-ivs-realtime-2.5.4/types_aiobotocore_ivs_realtime/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13425 2023-08-08 01:13:18.000000 types-aiobotocore-ivs-realtime-2.5.4/types_aiobotocore_ivs_realtime/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13402 2023-08-08 01:13:18.000000 types-aiobotocore-ivs-realtime-2.5.4/types_aiobotocore_ivs_realtime/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8343 2023-08-08 01:13:18.000000 types-aiobotocore-ivs-realtime-2.5.4/types_aiobotocore_ivs_realtime/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8341 2023-08-08 01:13:18.000000 types-aiobotocore-ivs-realtime-2.5.4/types_aiobotocore_ivs_realtime/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 01:13:18.000000 types-aiobotocore-ivs-realtime-2.5.4/types_aiobotocore_ivs_realtime/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    12189 2023-08-08 01:13:19.000000 types-aiobotocore-ivs-realtime-2.5.4/types_aiobotocore_ivs_realtime/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12172 2023-08-08 01:13:19.000000 types-aiobotocore-ivs-realtime-2.5.4/types_aiobotocore_ivs_realtime/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-08-08 01:13:18.000000 types-aiobotocore-ivs-realtime-2.5.4/types_aiobotocore_ivs_realtime/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:23:54.978711 types-aiobotocore-ivs-realtime-2.5.4/types_aiobotocore_ivs_realtime.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    12482 2023-08-08 01:23:54.000000 types-aiobotocore-ivs-realtime-2.5.4/types_aiobotocore_ivs_realtime.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      819 2023-08-08 01:23:54.000000 types-aiobotocore-ivs-realtime-2.5.4/types_aiobotocore_ivs_realtime.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 01:23:54.000000 types-aiobotocore-ivs-realtime-2.5.4/types_aiobotocore_ivs_realtime.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 01:23:54.000000 types-aiobotocore-ivs-realtime-2.5.4/types_aiobotocore_ivs_realtime.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-08 01:23:54.000000 types-aiobotocore-ivs-realtime-2.5.4/types_aiobotocore_ivs_realtime.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-08-08 01:23:54.000000 types-aiobotocore-ivs-realtime-2.5.4/types_aiobotocore_ivs_realtime.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-ivs-realtime-2.5.2.post2/LICENSE` & `types-aiobotocore-ivs-realtime-2.5.4/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-ivs-realtime-2.5.2.post2/PKG-INFO` & `types-aiobotocore-ivs-realtime-2.5.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-ivs-realtime
-Version: 2.5.2.post2
-Summary: Type annotations for aiobotocore.ivsrealtime 2.5.2 service generated with mypy-boto3-builder 7.17.2
+Version: 2.5.4
+Summary: Type annotations for aiobotocore.ivsrealtime 2.5.4 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ivs_realtime/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-ivs-realtime.svg?color=blue)](https://pypi.org/project/types-aiobotocore-ivs-realtime)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ivs_realtime/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-ivs-realtime)](https://pepy.tech/project/types-aiobotocore-ivs-realtime)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.ivsrealtime 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ivs-realtime.html#ivsrealtime)
+[aiobotocore.ivsrealtime 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ivs-realtime.html#ivsrealtime)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-ivs-realtime-2.5.2.post2/README.md` & `types-aiobotocore-ivs-realtime-2.5.4/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-ivs-realtime.svg?color=blue)](https://pypi.org/project/types-aiobotocore-ivs-realtime)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ivs_realtime/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-ivs-realtime)](https://pepy.tech/project/types-aiobotocore-ivs-realtime)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.ivsrealtime 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ivs-realtime.html#ivsrealtime)
+[aiobotocore.ivsrealtime 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ivs-realtime.html#ivsrealtime)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-ivs-realtime-2.5.2.post2/setup.py` & `types-aiobotocore-ivs-realtime-2.5.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-ivs-realtime",
-    version="2.5.2.post2",
+    version="2.5.4",
     packages=["types_aiobotocore_ivs_realtime"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.ivsrealtime 2.5.2 service generated with"
+        "Type annotations for aiobotocore.ivsrealtime 2.5.4 service generated with"
         " mypy-boto3-builder 7.17.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
```

### Comparing `types-aiobotocore-ivs-realtime-2.5.2.post2/types_aiobotocore_ivs_realtime/__main__.py` & `types-aiobotocore-ivs-realtime-2.5.4/types_aiobotocore_ivs_realtime/__main__.py`

 * *Files 24% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.ivsrealtime 2.5.2\nVersion:         2.5.2.post2\nBuilder"
+        "Type annotations for aiobotocore.ivsrealtime 2.5.4\nVersion:         2.5.4\nBuilder"
         " version: 7.17.2\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ivs_realtime//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ivs-realtime.html#ivsrealtime\nOther"
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

### Comparing `types-aiobotocore-ivs-realtime-2.5.2.post2/types_aiobotocore_ivs_realtime/client.py` & `types-aiobotocore-ivs-realtime-2.5.4/types_aiobotocore_ivs_realtime/client.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-ivs-realtime-2.5.2.post2/types_aiobotocore_ivs_realtime/client.pyi` & `types-aiobotocore-ivs-realtime-2.5.4/types_aiobotocore_ivs_realtime/client.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-ivs-realtime-2.5.2.post2/types_aiobotocore_ivs_realtime/literals.py` & `types-aiobotocore-ivs-realtime-2.5.4/types_aiobotocore_ivs_realtime/literals.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-ivs-realtime-2.5.2.post2/types_aiobotocore_ivs_realtime/literals.pyi` & `types-aiobotocore-ivs-realtime-2.5.4/types_aiobotocore_ivs_realtime/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-ivs-realtime-2.5.2.post2/types_aiobotocore_ivs_realtime/type_defs.py` & `types-aiobotocore-ivs-realtime-2.5.4/types_aiobotocore_ivs_realtime/type_defs.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-ivs-realtime-2.5.2.post2/types_aiobotocore_ivs_realtime/type_defs.pyi` & `types-aiobotocore-ivs-realtime-2.5.4/types_aiobotocore_ivs_realtime/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-ivs-realtime-2.5.2.post2/types_aiobotocore_ivs_realtime.egg-info/PKG-INFO` & `types-aiobotocore-ivs-realtime-2.5.4/types_aiobotocore_ivs_realtime.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-ivs-realtime
-Version: 2.5.2.post2
-Summary: Type annotations for aiobotocore.ivsrealtime 2.5.2 service generated with mypy-boto3-builder 7.17.2
+Version: 2.5.4
+Summary: Type annotations for aiobotocore.ivsrealtime 2.5.4 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ivs_realtime/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-ivs-realtime.svg?color=blue)](https://pypi.org/project/types-aiobotocore-ivs-realtime)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ivs_realtime/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-ivs-realtime)](https://pepy.tech/project/types-aiobotocore-ivs-realtime)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.ivsrealtime 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ivs-realtime.html#ivsrealtime)
+[aiobotocore.ivsrealtime 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ivs-realtime.html#ivsrealtime)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-ivs-realtime-2.5.2.post2/types_aiobotocore_ivs_realtime.egg-info/SOURCES.txt` & `types-aiobotocore-ivs-realtime-2.5.4/types_aiobotocore_ivs_realtime.egg-info/SOURCES.txt`

 * *Files identical despite different names*


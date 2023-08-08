# Comparing `tmp/types-aiobotocore-iotevents-2.5.2.post2.tar.gz` & `tmp/types-aiobotocore-iotevents-2.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-iotevents-2.5.2.post2.tar", last modified: Fri Aug  4 13:59:12 2023, max compression
+gzip compressed data, was "types-aiobotocore-iotevents-2.5.4.tar", last modified: Tue Aug  8 01:23:52 2023, max compression
```

## Comparing `types-aiobotocore-iotevents-2.5.2.post2.tar` & `types-aiobotocore-iotevents-2.5.4.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:58:49.596642 types-aiobotocore-iotevents-2.5.2.post2/
--rw-r--r--   0 vlad      (1000) vlad      (1000)     1070 2023-08-04 13:40:59.000000 types-aiobotocore-iotevents-2.5.2.post2/LICENSE
--rw-r--r--   0 vlad      (1000) vlad      (1000)    12314 2023-08-04 13:59:12.396643 types-aiobotocore-iotevents-2.5.2.post2/PKG-INFO
--rw-r--r--   0 vlad      (1000) vlad      (1000)    10788 2023-08-04 13:40:59.000000 types-aiobotocore-iotevents-2.5.2.post2/README.md
--rw-r--r--   0 vlad      (1000) vlad      (1000)       38 2023-08-04 13:59:12.406643 types-aiobotocore-iotevents-2.5.2.post2/setup.cfg
--rw-r--r--   0 vlad      (1000) vlad      (1000)     2086 2023-08-04 13:40:59.000000 types-aiobotocore-iotevents-2.5.2.post2/setup.py
-drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:58:49.596642 types-aiobotocore-iotevents-2.5.2.post2/types_aiobotocore_iotevents/
--rw-r--r--   0 vlad      (1000) vlad      (1000)      458 2023-08-04 13:40:59.000000 types-aiobotocore-iotevents-2.5.2.post2/types_aiobotocore_iotevents/__init__.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)      457 2023-08-04 13:40:59.000000 types-aiobotocore-iotevents-2.5.2.post2/types_aiobotocore_iotevents/__init__.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)      951 2023-08-04 13:40:59.000000 types-aiobotocore-iotevents-2.5.2.post2/types_aiobotocore_iotevents/__main__.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)    20395 2023-08-04 13:40:59.000000 types-aiobotocore-iotevents-2.5.2.post2/types_aiobotocore_iotevents/client.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)    20361 2023-08-04 13:40:59.000000 types-aiobotocore-iotevents-2.5.2.post2/types_aiobotocore_iotevents/client.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)     8849 2023-08-04 13:41:00.000000 types-aiobotocore-iotevents-2.5.2.post2/types_aiobotocore_iotevents/literals.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)     8847 2023-08-04 13:41:00.000000 types-aiobotocore-iotevents-2.5.2.post2/types_aiobotocore_iotevents/literals.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:40:59.000000 types-aiobotocore-iotevents-2.5.2.post2/types_aiobotocore_iotevents/py.typed
--rw-r--r--   0 vlad      (1000) vlad      (1000)    37370 2023-08-04 13:41:01.000000 types-aiobotocore-iotevents-2.5.2.post2/types_aiobotocore_iotevents/type_defs.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)    37305 2023-08-04 13:41:00.000000 types-aiobotocore-iotevents-2.5.2.post2/types_aiobotocore_iotevents/type_defs.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)       65 2023-08-04 13:40:59.000000 types-aiobotocore-iotevents-2.5.2.post2/types_aiobotocore_iotevents/version.py
-drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:12.396643 types-aiobotocore-iotevents-2.5.2.post2/types_aiobotocore_iotevents.egg-info/
--rw-r--r--   0 vlad      (1000) vlad      (1000)    12314 2023-08-04 13:59:12.000000 types-aiobotocore-iotevents-2.5.2.post2/types_aiobotocore_iotevents.egg-info/PKG-INFO
--rw-r--r--   0 vlad      (1000) vlad      (1000)      768 2023-08-04 13:59:12.000000 types-aiobotocore-iotevents-2.5.2.post2/types_aiobotocore_iotevents.egg-info/SOURCES.txt
--rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:12.000000 types-aiobotocore-iotevents-2.5.2.post2/types_aiobotocore_iotevents.egg-info/dependency_links.txt
--rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:12.000000 types-aiobotocore-iotevents-2.5.2.post2/types_aiobotocore_iotevents.egg-info/not-zip-safe
--rw-r--r--   0 vlad      (1000) vlad      (1000)       52 2023-08-04 13:59:12.000000 types-aiobotocore-iotevents-2.5.2.post2/types_aiobotocore_iotevents.egg-info/requires.txt
--rw-r--r--   0 vlad      (1000) vlad      (1000)       28 2023-08-04 13:59:12.000000 types-aiobotocore-iotevents-2.5.2.post2/types_aiobotocore_iotevents.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:23:52.738705 types-aiobotocore-iotevents-2.5.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-08 01:12:55.000000 types-aiobotocore-iotevents-2.5.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    12308 2023-08-08 01:23:52.738705 types-aiobotocore-iotevents-2.5.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10788 2023-08-08 01:12:55.000000 types-aiobotocore-iotevents-2.5.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-08 01:23:52.738705 types-aiobotocore-iotevents-2.5.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2080 2023-08-08 01:12:55.000000 types-aiobotocore-iotevents-2.5.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:23:52.726706 types-aiobotocore-iotevents-2.5.4/types_aiobotocore_iotevents/
+-rw-r--r--   0 runner    (1001) docker     (123)      458 2023-08-08 01:12:55.000000 types-aiobotocore-iotevents-2.5.4/types_aiobotocore_iotevents/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      457 2023-08-08 01:12:55.000000 types-aiobotocore-iotevents-2.5.4/types_aiobotocore_iotevents/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      939 2023-08-08 01:12:55.000000 types-aiobotocore-iotevents-2.5.4/types_aiobotocore_iotevents/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20395 2023-08-08 01:12:56.000000 types-aiobotocore-iotevents-2.5.4/types_aiobotocore_iotevents/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20361 2023-08-08 01:12:55.000000 types-aiobotocore-iotevents-2.5.4/types_aiobotocore_iotevents/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8849 2023-08-08 01:12:57.000000 types-aiobotocore-iotevents-2.5.4/types_aiobotocore_iotevents/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8847 2023-08-08 01:12:57.000000 types-aiobotocore-iotevents-2.5.4/types_aiobotocore_iotevents/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 01:12:55.000000 types-aiobotocore-iotevents-2.5.4/types_aiobotocore_iotevents/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    37370 2023-08-08 01:12:58.000000 types-aiobotocore-iotevents-2.5.4/types_aiobotocore_iotevents/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37305 2023-08-08 01:12:57.000000 types-aiobotocore-iotevents-2.5.4/types_aiobotocore_iotevents/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-08-08 01:12:55.000000 types-aiobotocore-iotevents-2.5.4/types_aiobotocore_iotevents/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:23:52.738705 types-aiobotocore-iotevents-2.5.4/types_aiobotocore_iotevents.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    12308 2023-08-08 01:23:52.000000 types-aiobotocore-iotevents-2.5.4/types_aiobotocore_iotevents.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      768 2023-08-08 01:23:52.000000 types-aiobotocore-iotevents-2.5.4/types_aiobotocore_iotevents.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 01:23:52.000000 types-aiobotocore-iotevents-2.5.4/types_aiobotocore_iotevents.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 01:23:52.000000 types-aiobotocore-iotevents-2.5.4/types_aiobotocore_iotevents.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-08 01:23:52.000000 types-aiobotocore-iotevents-2.5.4/types_aiobotocore_iotevents.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-08-08 01:23:52.000000 types-aiobotocore-iotevents-2.5.4/types_aiobotocore_iotevents.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-iotevents-2.5.2.post2/LICENSE` & `types-aiobotocore-iotevents-2.5.4/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-iotevents-2.5.2.post2/PKG-INFO` & `types-aiobotocore-iotevents-2.5.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-iotevents
-Version: 2.5.2.post2
-Summary: Type annotations for aiobotocore.IoTEvents 2.5.2 service generated with mypy-boto3-builder 7.17.2
+Version: 2.5.4
+Summary: Type annotations for aiobotocore.IoTEvents 2.5.4 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotevents/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-iotevents.svg?color=blue)](https://pypi.org/project/types-aiobotocore-iotevents)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotevents/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-iotevents)](https://pepy.tech/project/types-aiobotocore-iotevents)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.IoTEvents 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotevents.html#IoTEvents)
+[aiobotocore.IoTEvents 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotevents.html#IoTEvents)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-iotevents-2.5.2.post2/README.md` & `types-aiobotocore-iotevents-2.5.4/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-iotevents.svg?color=blue)](https://pypi.org/project/types-aiobotocore-iotevents)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotevents/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-iotevents)](https://pepy.tech/project/types-aiobotocore-iotevents)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.IoTEvents 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotevents.html#IoTEvents)
+[aiobotocore.IoTEvents 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotevents.html#IoTEvents)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-iotevents-2.5.2.post2/setup.py` & `types-aiobotocore-iotevents-2.5.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-iotevents",
-    version="2.5.2.post2",
+    version="2.5.4",
     packages=["types_aiobotocore_iotevents"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.IoTEvents 2.5.2 service generated with mypy-boto3-builder"
+        "Type annotations for aiobotocore.IoTEvents 2.5.4 service generated with mypy-boto3-builder"
         " 7.17.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
```

### Comparing `types-aiobotocore-iotevents-2.5.2.post2/types_aiobotocore_iotevents/__main__.py` & `types-aiobotocore-iotevents-2.5.4/types_aiobotocore_iotevents/__main__.py`

 * *Files 9% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.IoTEvents 2.5.2\nVersion:         2.5.2.post2\nBuilder"
-        " version: 7.17.2\nDocs:           "
+        "Type annotations for aiobotocore.IoTEvents 2.5.4\nVersion:         2.5.4\nBuilder version:"
+        " 7.17.2\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotevents//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotevents.html#IoTEvents\nOther"
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

### Comparing `types-aiobotocore-iotevents-2.5.2.post2/types_aiobotocore_iotevents/client.py` & `types-aiobotocore-iotevents-2.5.4/types_aiobotocore_iotevents/client.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-iotevents-2.5.2.post2/types_aiobotocore_iotevents/client.pyi` & `types-aiobotocore-iotevents-2.5.4/types_aiobotocore_iotevents/client.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-iotevents-2.5.2.post2/types_aiobotocore_iotevents/literals.py` & `types-aiobotocore-iotevents-2.5.4/types_aiobotocore_iotevents/literals.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-iotevents-2.5.2.post2/types_aiobotocore_iotevents/literals.pyi` & `types-aiobotocore-iotevents-2.5.4/types_aiobotocore_iotevents/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-iotevents-2.5.2.post2/types_aiobotocore_iotevents/type_defs.py` & `types-aiobotocore-iotevents-2.5.4/types_aiobotocore_iotevents/type_defs.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-iotevents-2.5.2.post2/types_aiobotocore_iotevents/type_defs.pyi` & `types-aiobotocore-iotevents-2.5.4/types_aiobotocore_iotevents/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-iotevents-2.5.2.post2/types_aiobotocore_iotevents.egg-info/PKG-INFO` & `types-aiobotocore-iotevents-2.5.4/types_aiobotocore_iotevents.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-iotevents
-Version: 2.5.2.post2
-Summary: Type annotations for aiobotocore.IoTEvents 2.5.2 service generated with mypy-boto3-builder 7.17.2
+Version: 2.5.4
+Summary: Type annotations for aiobotocore.IoTEvents 2.5.4 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotevents/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-iotevents.svg?color=blue)](https://pypi.org/project/types-aiobotocore-iotevents)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotevents/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-iotevents)](https://pepy.tech/project/types-aiobotocore-iotevents)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.IoTEvents 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotevents.html#IoTEvents)
+[aiobotocore.IoTEvents 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotevents.html#IoTEvents)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-iotevents-2.5.2.post2/types_aiobotocore_iotevents.egg-info/SOURCES.txt` & `types-aiobotocore-iotevents-2.5.4/types_aiobotocore_iotevents.egg-info/SOURCES.txt`

 * *Files identical despite different names*


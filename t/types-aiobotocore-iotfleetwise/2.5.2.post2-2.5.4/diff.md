# Comparing `tmp/types-aiobotocore-iotfleetwise-2.5.2.post2.tar.gz` & `tmp/types-aiobotocore-iotfleetwise-2.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-iotfleetwise-2.5.2.post2.tar", last modified: Fri Aug  4 13:59:12 2023, max compression
+gzip compressed data, was "types-aiobotocore-iotfleetwise-2.5.4.tar", last modified: Tue Aug  8 01:23:52 2023, max compression
```

## Comparing `types-aiobotocore-iotfleetwise-2.5.2.post2.tar` & `types-aiobotocore-iotfleetwise-2.5.4.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:12.466642 types-aiobotocore-iotfleetwise-2.5.2.post2/
--rw-r--r--   0 vlad      (1000) vlad      (1000)     1070 2023-08-04 13:41:06.000000 types-aiobotocore-iotfleetwise-2.5.2.post2/LICENSE
--rw-r--r--   0 vlad      (1000) vlad      (1000)    15159 2023-08-04 13:59:12.466642 types-aiobotocore-iotfleetwise-2.5.2.post2/PKG-INFO
--rw-r--r--   0 vlad      (1000) vlad      (1000)    13621 2023-08-04 13:41:06.000000 types-aiobotocore-iotfleetwise-2.5.2.post2/README.md
--rw-r--r--   0 vlad      (1000) vlad      (1000)       38 2023-08-04 13:59:12.466642 types-aiobotocore-iotfleetwise-2.5.2.post2/setup.cfg
--rw-r--r--   0 vlad      (1000) vlad      (1000)     2107 2023-08-04 13:41:05.000000 types-aiobotocore-iotfleetwise-2.5.2.post2/setup.py
-drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:12.466642 types-aiobotocore-iotfleetwise-2.5.2.post2/types_aiobotocore_iotfleetwise/
--rw-r--r--   0 vlad      (1000) vlad      (1000)     3445 2023-08-04 13:41:06.000000 types-aiobotocore-iotfleetwise-2.5.2.post2/types_aiobotocore_iotfleetwise/__init__.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)     3444 2023-08-04 13:41:06.000000 types-aiobotocore-iotfleetwise-2.5.2.post2/types_aiobotocore_iotfleetwise/__init__.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)      963 2023-08-04 13:41:06.000000 types-aiobotocore-iotfleetwise-2.5.2.post2/types_aiobotocore_iotfleetwise/__main__.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)    43340 2023-08-04 13:41:06.000000 types-aiobotocore-iotfleetwise-2.5.2.post2/types_aiobotocore_iotfleetwise/client.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)    43268 2023-08-04 13:41:06.000000 types-aiobotocore-iotfleetwise-2.5.2.post2/types_aiobotocore_iotfleetwise/client.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)    11527 2023-08-04 13:41:07.000000 types-aiobotocore-iotfleetwise-2.5.2.post2/types_aiobotocore_iotfleetwise/literals.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)    11525 2023-08-04 13:41:06.000000 types-aiobotocore-iotfleetwise-2.5.2.post2/types_aiobotocore_iotfleetwise/literals.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)    16193 2023-08-04 13:41:06.000000 types-aiobotocore-iotfleetwise-2.5.2.post2/types_aiobotocore_iotfleetwise/paginator.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)    16178 2023-08-04 13:41:06.000000 types-aiobotocore-iotfleetwise-2.5.2.post2/types_aiobotocore_iotfleetwise/paginator.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:41:06.000000 types-aiobotocore-iotfleetwise-2.5.2.post2/types_aiobotocore_iotfleetwise/py.typed
--rw-r--r--   0 vlad      (1000) vlad      (1000)    58195 2023-08-04 13:41:08.000000 types-aiobotocore-iotfleetwise-2.5.2.post2/types_aiobotocore_iotfleetwise/type_defs.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)    58094 2023-08-04 13:41:08.000000 types-aiobotocore-iotfleetwise-2.5.2.post2/types_aiobotocore_iotfleetwise/type_defs.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)       65 2023-08-04 13:41:06.000000 types-aiobotocore-iotfleetwise-2.5.2.post2/types_aiobotocore_iotfleetwise/version.py
-drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:12.466642 types-aiobotocore-iotfleetwise-2.5.2.post2/types_aiobotocore_iotfleetwise.egg-info/
--rw-r--r--   0 vlad      (1000) vlad      (1000)    15159 2023-08-04 13:59:12.000000 types-aiobotocore-iotfleetwise-2.5.2.post2/types_aiobotocore_iotfleetwise.egg-info/PKG-INFO
--rw-r--r--   0 vlad      (1000) vlad      (1000)      908 2023-08-04 13:59:12.000000 types-aiobotocore-iotfleetwise-2.5.2.post2/types_aiobotocore_iotfleetwise.egg-info/SOURCES.txt
--rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:12.000000 types-aiobotocore-iotfleetwise-2.5.2.post2/types_aiobotocore_iotfleetwise.egg-info/dependency_links.txt
--rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:12.000000 types-aiobotocore-iotfleetwise-2.5.2.post2/types_aiobotocore_iotfleetwise.egg-info/not-zip-safe
--rw-r--r--   0 vlad      (1000) vlad      (1000)       52 2023-08-04 13:59:12.000000 types-aiobotocore-iotfleetwise-2.5.2.post2/types_aiobotocore_iotfleetwise.egg-info/requires.txt
--rw-r--r--   0 vlad      (1000) vlad      (1000)       31 2023-08-04 13:59:12.000000 types-aiobotocore-iotfleetwise-2.5.2.post2/types_aiobotocore_iotfleetwise.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:23:52.918706 types-aiobotocore-iotfleetwise-2.5.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-08 01:13:00.000000 types-aiobotocore-iotfleetwise-2.5.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    15153 2023-08-08 01:23:52.918706 types-aiobotocore-iotfleetwise-2.5.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    13621 2023-08-08 01:13:00.000000 types-aiobotocore-iotfleetwise-2.5.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-08 01:23:52.918706 types-aiobotocore-iotfleetwise-2.5.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2101 2023-08-08 01:13:00.000000 types-aiobotocore-iotfleetwise-2.5.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:23:52.914706 types-aiobotocore-iotfleetwise-2.5.4/types_aiobotocore_iotfleetwise/
+-rw-r--r--   0 runner    (1001) docker     (123)     3445 2023-08-08 01:13:00.000000 types-aiobotocore-iotfleetwise-2.5.4/types_aiobotocore_iotfleetwise/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3444 2023-08-08 01:13:00.000000 types-aiobotocore-iotfleetwise-2.5.4/types_aiobotocore_iotfleetwise/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      951 2023-08-08 01:13:00.000000 types-aiobotocore-iotfleetwise-2.5.4/types_aiobotocore_iotfleetwise/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    43340 2023-08-08 01:13:00.000000 types-aiobotocore-iotfleetwise-2.5.4/types_aiobotocore_iotfleetwise/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    43268 2023-08-08 01:13:00.000000 types-aiobotocore-iotfleetwise-2.5.4/types_aiobotocore_iotfleetwise/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    11527 2023-08-08 01:13:00.000000 types-aiobotocore-iotfleetwise-2.5.4/types_aiobotocore_iotfleetwise/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11525 2023-08-08 01:13:00.000000 types-aiobotocore-iotfleetwise-2.5.4/types_aiobotocore_iotfleetwise/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    16193 2023-08-08 01:13:00.000000 types-aiobotocore-iotfleetwise-2.5.4/types_aiobotocore_iotfleetwise/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16178 2023-08-08 01:13:00.000000 types-aiobotocore-iotfleetwise-2.5.4/types_aiobotocore_iotfleetwise/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 01:13:00.000000 types-aiobotocore-iotfleetwise-2.5.4/types_aiobotocore_iotfleetwise/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    58195 2023-08-08 01:13:01.000000 types-aiobotocore-iotfleetwise-2.5.4/types_aiobotocore_iotfleetwise/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    58094 2023-08-08 01:13:01.000000 types-aiobotocore-iotfleetwise-2.5.4/types_aiobotocore_iotfleetwise/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-08-08 01:13:00.000000 types-aiobotocore-iotfleetwise-2.5.4/types_aiobotocore_iotfleetwise/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:23:52.918706 types-aiobotocore-iotfleetwise-2.5.4/types_aiobotocore_iotfleetwise.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    15153 2023-08-08 01:23:52.000000 types-aiobotocore-iotfleetwise-2.5.4/types_aiobotocore_iotfleetwise.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      908 2023-08-08 01:23:52.000000 types-aiobotocore-iotfleetwise-2.5.4/types_aiobotocore_iotfleetwise.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 01:23:52.000000 types-aiobotocore-iotfleetwise-2.5.4/types_aiobotocore_iotfleetwise.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 01:23:52.000000 types-aiobotocore-iotfleetwise-2.5.4/types_aiobotocore_iotfleetwise.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-08 01:23:52.000000 types-aiobotocore-iotfleetwise-2.5.4/types_aiobotocore_iotfleetwise.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-08-08 01:23:52.000000 types-aiobotocore-iotfleetwise-2.5.4/types_aiobotocore_iotfleetwise.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-iotfleetwise-2.5.2.post2/LICENSE` & `types-aiobotocore-iotfleetwise-2.5.4/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-iotfleetwise-2.5.2.post2/PKG-INFO` & `types-aiobotocore-iotfleetwise-2.5.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-iotfleetwise
-Version: 2.5.2.post2
-Summary: Type annotations for aiobotocore.IoTFleetWise 2.5.2 service generated with mypy-boto3-builder 7.17.2
+Version: 2.5.4
+Summary: Type annotations for aiobotocore.IoTFleetWise 2.5.4 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotfleetwise/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-iotfleetwise.svg?color=blue)](https://pypi.org/project/types-aiobotocore-iotfleetwise)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotfleetwise/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-iotfleetwise)](https://pepy.tech/project/types-aiobotocore-iotfleetwise)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.IoTFleetWise 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotfleetwise.html#IoTFleetWise)
+[aiobotocore.IoTFleetWise 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotfleetwise.html#IoTFleetWise)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-iotfleetwise-2.5.2.post2/README.md` & `types-aiobotocore-iotfleetwise-2.5.4/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-iotfleetwise.svg?color=blue)](https://pypi.org/project/types-aiobotocore-iotfleetwise)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotfleetwise/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-iotfleetwise)](https://pepy.tech/project/types-aiobotocore-iotfleetwise)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.IoTFleetWise 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotfleetwise.html#IoTFleetWise)
+[aiobotocore.IoTFleetWise 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotfleetwise.html#IoTFleetWise)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-iotfleetwise-2.5.2.post2/setup.py` & `types-aiobotocore-iotfleetwise-2.5.4/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-iotfleetwise",
-    version="2.5.2.post2",
+    version="2.5.4",
     packages=["types_aiobotocore_iotfleetwise"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.IoTFleetWise 2.5.2 service generated with"
+        "Type annotations for aiobotocore.IoTFleetWise 2.5.4 service generated with"
         " mypy-boto3-builder 7.17.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
```

### Comparing `types-aiobotocore-iotfleetwise-2.5.2.post2/types_aiobotocore_iotfleetwise/__init__.py` & `types-aiobotocore-iotfleetwise-2.5.4/types_aiobotocore_iotfleetwise/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-iotfleetwise-2.5.2.post2/types_aiobotocore_iotfleetwise/__init__.pyi` & `types-aiobotocore-iotfleetwise-2.5.4/types_aiobotocore_iotfleetwise/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-iotfleetwise-2.5.2.post2/types_aiobotocore_iotfleetwise/__main__.py` & `types-aiobotocore-iotfleetwise-2.5.4/types_aiobotocore_iotfleetwise/__main__.py`

 * *Files 11% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.IoTFleetWise 2.5.2\nVersion:         2.5.2.post2\nBuilder"
+        "Type annotations for aiobotocore.IoTFleetWise 2.5.4\nVersion:         2.5.4\nBuilder"
         " version: 7.17.2\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotfleetwise//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotfleetwise.html#IoTFleetWise\nOther"
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

### Comparing `types-aiobotocore-iotfleetwise-2.5.2.post2/types_aiobotocore_iotfleetwise/client.py` & `types-aiobotocore-iotfleetwise-2.5.4/types_aiobotocore_iotfleetwise/client.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-iotfleetwise-2.5.2.post2/types_aiobotocore_iotfleetwise/client.pyi` & `types-aiobotocore-iotfleetwise-2.5.4/types_aiobotocore_iotfleetwise/client.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-iotfleetwise-2.5.2.post2/types_aiobotocore_iotfleetwise/literals.py` & `types-aiobotocore-iotfleetwise-2.5.4/types_aiobotocore_iotfleetwise/literals.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-iotfleetwise-2.5.2.post2/types_aiobotocore_iotfleetwise/literals.pyi` & `types-aiobotocore-iotfleetwise-2.5.4/types_aiobotocore_iotfleetwise/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-iotfleetwise-2.5.2.post2/types_aiobotocore_iotfleetwise/paginator.py` & `types-aiobotocore-iotfleetwise-2.5.4/types_aiobotocore_iotfleetwise/paginator.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-iotfleetwise-2.5.2.post2/types_aiobotocore_iotfleetwise/paginator.pyi` & `types-aiobotocore-iotfleetwise-2.5.4/types_aiobotocore_iotfleetwise/paginator.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-iotfleetwise-2.5.2.post2/types_aiobotocore_iotfleetwise/type_defs.py` & `types-aiobotocore-iotfleetwise-2.5.4/types_aiobotocore_iotfleetwise/type_defs.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-iotfleetwise-2.5.2.post2/types_aiobotocore_iotfleetwise/type_defs.pyi` & `types-aiobotocore-iotfleetwise-2.5.4/types_aiobotocore_iotfleetwise/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-iotfleetwise-2.5.2.post2/types_aiobotocore_iotfleetwise.egg-info/PKG-INFO` & `types-aiobotocore-iotfleetwise-2.5.4/types_aiobotocore_iotfleetwise.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-iotfleetwise
-Version: 2.5.2.post2
-Summary: Type annotations for aiobotocore.IoTFleetWise 2.5.2 service generated with mypy-boto3-builder 7.17.2
+Version: 2.5.4
+Summary: Type annotations for aiobotocore.IoTFleetWise 2.5.4 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotfleetwise/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-iotfleetwise.svg?color=blue)](https://pypi.org/project/types-aiobotocore-iotfleetwise)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotfleetwise/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-iotfleetwise)](https://pepy.tech/project/types-aiobotocore-iotfleetwise)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.IoTFleetWise 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotfleetwise.html#IoTFleetWise)
+[aiobotocore.IoTFleetWise 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotfleetwise.html#IoTFleetWise)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-iotfleetwise-2.5.2.post2/types_aiobotocore_iotfleetwise.egg-info/SOURCES.txt` & `types-aiobotocore-iotfleetwise-2.5.4/types_aiobotocore_iotfleetwise.egg-info/SOURCES.txt`

 * *Files identical despite different names*


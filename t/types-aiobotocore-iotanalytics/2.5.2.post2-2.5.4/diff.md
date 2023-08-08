# Comparing `tmp/types-aiobotocore-iotanalytics-2.5.2.post2.tar.gz` & `tmp/types-aiobotocore-iotanalytics-2.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-iotanalytics-2.5.2.post2.tar", last modified: Fri Aug  4 13:59:12 2023, max compression
+gzip compressed data, was "types-aiobotocore-iotanalytics-2.5.4.tar", last modified: Tue Aug  8 01:23:52 2023, max compression
```

## Comparing `types-aiobotocore-iotanalytics-2.5.2.post2.tar` & `types-aiobotocore-iotanalytics-2.5.4.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:12.386643 types-aiobotocore-iotanalytics-2.5.2.post2/
--rw-r--r--   0 vlad      (1000) vlad      (1000)     1070 2023-08-04 13:40:53.000000 types-aiobotocore-iotanalytics-2.5.2.post2/LICENSE
--rw-r--r--   0 vlad      (1000) vlad      (1000)    13735 2023-08-04 13:59:12.386643 types-aiobotocore-iotanalytics-2.5.2.post2/PKG-INFO
--rw-r--r--   0 vlad      (1000) vlad      (1000)    12197 2023-08-04 13:40:53.000000 types-aiobotocore-iotanalytics-2.5.2.post2/README.md
--rw-r--r--   0 vlad      (1000) vlad      (1000)       38 2023-08-04 13:59:12.386643 types-aiobotocore-iotanalytics-2.5.2.post2/setup.cfg
--rw-r--r--   0 vlad      (1000) vlad      (1000)     2107 2023-08-04 13:40:53.000000 types-aiobotocore-iotanalytics-2.5.2.post2/setup.py
-drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:12.386643 types-aiobotocore-iotanalytics-2.5.2.post2/types_aiobotocore_iotanalytics/
--rw-r--r--   0 vlad      (1000) vlad      (1000)     1473 2023-08-04 13:40:53.000000 types-aiobotocore-iotanalytics-2.5.2.post2/types_aiobotocore_iotanalytics/__init__.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)     1472 2023-08-04 13:40:53.000000 types-aiobotocore-iotanalytics-2.5.2.post2/types_aiobotocore_iotanalytics/__init__.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)      963 2023-08-04 13:40:53.000000 types-aiobotocore-iotanalytics-2.5.2.post2/types_aiobotocore_iotanalytics/__main__.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)    28127 2023-08-04 13:40:54.000000 types-aiobotocore-iotanalytics-2.5.2.post2/types_aiobotocore_iotanalytics/client.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)    28079 2023-08-04 13:40:53.000000 types-aiobotocore-iotanalytics-2.5.2.post2/types_aiobotocore_iotanalytics/client.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)     9201 2023-08-04 13:40:54.000000 types-aiobotocore-iotanalytics-2.5.2.post2/types_aiobotocore_iotanalytics/literals.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)     9199 2023-08-04 13:40:54.000000 types-aiobotocore-iotanalytics-2.5.2.post2/types_aiobotocore_iotanalytics/literals.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)     6582 2023-08-04 13:40:54.000000 types-aiobotocore-iotanalytics-2.5.2.post2/types_aiobotocore_iotanalytics/paginator.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)     6575 2023-08-04 13:40:54.000000 types-aiobotocore-iotanalytics-2.5.2.post2/types_aiobotocore_iotanalytics/paginator.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:40:53.000000 types-aiobotocore-iotanalytics-2.5.2.post2/types_aiobotocore_iotanalytics/py.typed
--rw-r--r--   0 vlad      (1000) vlad      (1000)    46249 2023-08-04 13:40:55.000000 types-aiobotocore-iotanalytics-2.5.2.post2/types_aiobotocore_iotanalytics/type_defs.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)    46178 2023-08-04 13:40:54.000000 types-aiobotocore-iotanalytics-2.5.2.post2/types_aiobotocore_iotanalytics/type_defs.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)       65 2023-08-04 13:40:53.000000 types-aiobotocore-iotanalytics-2.5.2.post2/types_aiobotocore_iotanalytics/version.py
-drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:12.386643 types-aiobotocore-iotanalytics-2.5.2.post2/types_aiobotocore_iotanalytics.egg-info/
--rw-r--r--   0 vlad      (1000) vlad      (1000)    13735 2023-08-04 13:59:12.000000 types-aiobotocore-iotanalytics-2.5.2.post2/types_aiobotocore_iotanalytics.egg-info/PKG-INFO
--rw-r--r--   0 vlad      (1000) vlad      (1000)      908 2023-08-04 13:59:12.000000 types-aiobotocore-iotanalytics-2.5.2.post2/types_aiobotocore_iotanalytics.egg-info/SOURCES.txt
--rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:12.000000 types-aiobotocore-iotanalytics-2.5.2.post2/types_aiobotocore_iotanalytics.egg-info/dependency_links.txt
--rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:12.000000 types-aiobotocore-iotanalytics-2.5.2.post2/types_aiobotocore_iotanalytics.egg-info/not-zip-safe
--rw-r--r--   0 vlad      (1000) vlad      (1000)       52 2023-08-04 13:59:12.000000 types-aiobotocore-iotanalytics-2.5.2.post2/types_aiobotocore_iotanalytics.egg-info/requires.txt
--rw-r--r--   0 vlad      (1000) vlad      (1000)       31 2023-08-04 13:59:12.000000 types-aiobotocore-iotanalytics-2.5.2.post2/types_aiobotocore_iotanalytics.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:23:52.438706 types-aiobotocore-iotanalytics-2.5.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-08 01:12:52.000000 types-aiobotocore-iotanalytics-2.5.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    13729 2023-08-08 01:23:52.438706 types-aiobotocore-iotanalytics-2.5.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    12197 2023-08-08 01:12:52.000000 types-aiobotocore-iotanalytics-2.5.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-08 01:23:52.438706 types-aiobotocore-iotanalytics-2.5.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2101 2023-08-08 01:12:52.000000 types-aiobotocore-iotanalytics-2.5.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:23:52.438706 types-aiobotocore-iotanalytics-2.5.4/types_aiobotocore_iotanalytics/
+-rw-r--r--   0 runner    (1001) docker     (123)     1473 2023-08-08 01:12:52.000000 types-aiobotocore-iotanalytics-2.5.4/types_aiobotocore_iotanalytics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1472 2023-08-08 01:12:52.000000 types-aiobotocore-iotanalytics-2.5.4/types_aiobotocore_iotanalytics/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      951 2023-08-08 01:12:52.000000 types-aiobotocore-iotanalytics-2.5.4/types_aiobotocore_iotanalytics/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28127 2023-08-08 01:12:53.000000 types-aiobotocore-iotanalytics-2.5.4/types_aiobotocore_iotanalytics/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28079 2023-08-08 01:12:53.000000 types-aiobotocore-iotanalytics-2.5.4/types_aiobotocore_iotanalytics/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9201 2023-08-08 01:12:53.000000 types-aiobotocore-iotanalytics-2.5.4/types_aiobotocore_iotanalytics/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9199 2023-08-08 01:12:53.000000 types-aiobotocore-iotanalytics-2.5.4/types_aiobotocore_iotanalytics/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     6582 2023-08-08 01:12:53.000000 types-aiobotocore-iotanalytics-2.5.4/types_aiobotocore_iotanalytics/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6575 2023-08-08 01:12:53.000000 types-aiobotocore-iotanalytics-2.5.4/types_aiobotocore_iotanalytics/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 01:12:52.000000 types-aiobotocore-iotanalytics-2.5.4/types_aiobotocore_iotanalytics/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    46249 2023-08-08 01:12:54.000000 types-aiobotocore-iotanalytics-2.5.4/types_aiobotocore_iotanalytics/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46178 2023-08-08 01:12:53.000000 types-aiobotocore-iotanalytics-2.5.4/types_aiobotocore_iotanalytics/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-08-08 01:12:52.000000 types-aiobotocore-iotanalytics-2.5.4/types_aiobotocore_iotanalytics/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:23:52.438706 types-aiobotocore-iotanalytics-2.5.4/types_aiobotocore_iotanalytics.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    13729 2023-08-08 01:23:52.000000 types-aiobotocore-iotanalytics-2.5.4/types_aiobotocore_iotanalytics.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      908 2023-08-08 01:23:52.000000 types-aiobotocore-iotanalytics-2.5.4/types_aiobotocore_iotanalytics.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 01:23:52.000000 types-aiobotocore-iotanalytics-2.5.4/types_aiobotocore_iotanalytics.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 01:23:52.000000 types-aiobotocore-iotanalytics-2.5.4/types_aiobotocore_iotanalytics.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-08 01:23:52.000000 types-aiobotocore-iotanalytics-2.5.4/types_aiobotocore_iotanalytics.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-08-08 01:23:52.000000 types-aiobotocore-iotanalytics-2.5.4/types_aiobotocore_iotanalytics.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-iotanalytics-2.5.2.post2/LICENSE` & `types-aiobotocore-iotanalytics-2.5.4/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-iotanalytics-2.5.2.post2/PKG-INFO` & `types-aiobotocore-iotanalytics-2.5.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-iotanalytics
-Version: 2.5.2.post2
-Summary: Type annotations for aiobotocore.IoTAnalytics 2.5.2 service generated with mypy-boto3-builder 7.17.2
+Version: 2.5.4
+Summary: Type annotations for aiobotocore.IoTAnalytics 2.5.4 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotanalytics/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-iotanalytics.svg?color=blue)](https://pypi.org/project/types-aiobotocore-iotanalytics)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotanalytics/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-iotanalytics)](https://pepy.tech/project/types-aiobotocore-iotanalytics)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.IoTAnalytics 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotanalytics.html#IoTAnalytics)
+[aiobotocore.IoTAnalytics 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotanalytics.html#IoTAnalytics)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-iotanalytics-2.5.2.post2/README.md` & `types-aiobotocore-iotanalytics-2.5.4/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-iotanalytics.svg?color=blue)](https://pypi.org/project/types-aiobotocore-iotanalytics)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotanalytics/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-iotanalytics)](https://pepy.tech/project/types-aiobotocore-iotanalytics)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.IoTAnalytics 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotanalytics.html#IoTAnalytics)
+[aiobotocore.IoTAnalytics 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotanalytics.html#IoTAnalytics)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-iotanalytics-2.5.2.post2/setup.py` & `types-aiobotocore-iotanalytics-2.5.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-iotanalytics",
-    version="2.5.2.post2",
+    version="2.5.4",
     packages=["types_aiobotocore_iotanalytics"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.IoTAnalytics 2.5.2 service generated with"
+        "Type annotations for aiobotocore.IoTAnalytics 2.5.4 service generated with"
         " mypy-boto3-builder 7.17.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
```

### Comparing `types-aiobotocore-iotanalytics-2.5.2.post2/types_aiobotocore_iotanalytics/__init__.py` & `types-aiobotocore-iotanalytics-2.5.4/types_aiobotocore_iotanalytics/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-iotanalytics-2.5.2.post2/types_aiobotocore_iotanalytics/__init__.pyi` & `types-aiobotocore-iotanalytics-2.5.4/types_aiobotocore_iotanalytics/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-iotanalytics-2.5.2.post2/types_aiobotocore_iotanalytics/client.py` & `types-aiobotocore-iotanalytics-2.5.4/types_aiobotocore_iotanalytics/client.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-iotanalytics-2.5.2.post2/types_aiobotocore_iotanalytics/client.pyi` & `types-aiobotocore-iotanalytics-2.5.4/types_aiobotocore_iotanalytics/client.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-iotanalytics-2.5.2.post2/types_aiobotocore_iotanalytics/literals.py` & `types-aiobotocore-iotanalytics-2.5.4/types_aiobotocore_iotanalytics/literals.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-iotanalytics-2.5.2.post2/types_aiobotocore_iotanalytics/literals.pyi` & `types-aiobotocore-iotanalytics-2.5.4/types_aiobotocore_iotanalytics/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-iotanalytics-2.5.2.post2/types_aiobotocore_iotanalytics/paginator.py` & `types-aiobotocore-iotanalytics-2.5.4/types_aiobotocore_iotanalytics/paginator.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-iotanalytics-2.5.2.post2/types_aiobotocore_iotanalytics/paginator.pyi` & `types-aiobotocore-iotanalytics-2.5.4/types_aiobotocore_iotanalytics/paginator.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-iotanalytics-2.5.2.post2/types_aiobotocore_iotanalytics/type_defs.py` & `types-aiobotocore-iotanalytics-2.5.4/types_aiobotocore_iotanalytics/type_defs.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-iotanalytics-2.5.2.post2/types_aiobotocore_iotanalytics/type_defs.pyi` & `types-aiobotocore-iotanalytics-2.5.4/types_aiobotocore_iotanalytics/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-iotanalytics-2.5.2.post2/types_aiobotocore_iotanalytics.egg-info/PKG-INFO` & `types-aiobotocore-iotanalytics-2.5.4/types_aiobotocore_iotanalytics.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-iotanalytics
-Version: 2.5.2.post2
-Summary: Type annotations for aiobotocore.IoTAnalytics 2.5.2 service generated with mypy-boto3-builder 7.17.2
+Version: 2.5.4
+Summary: Type annotations for aiobotocore.IoTAnalytics 2.5.4 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotanalytics/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-iotanalytics.svg?color=blue)](https://pypi.org/project/types-aiobotocore-iotanalytics)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotanalytics/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-iotanalytics)](https://pepy.tech/project/types-aiobotocore-iotanalytics)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.IoTAnalytics 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotanalytics.html#IoTAnalytics)
+[aiobotocore.IoTAnalytics 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotanalytics.html#IoTAnalytics)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-iotanalytics-2.5.2.post2/types_aiobotocore_iotanalytics.egg-info/SOURCES.txt` & `types-aiobotocore-iotanalytics-2.5.4/types_aiobotocore_iotanalytics.egg-info/SOURCES.txt`

 * *Files identical despite different names*


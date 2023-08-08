# Comparing `tmp/types-aiobotocore-kinesisanalytics-2.5.2.post2.tar.gz` & `tmp/types-aiobotocore-kinesisanalytics-2.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-kinesisanalytics-2.5.2.post2.tar", last modified: Fri Aug  4 13:59:14 2023, max compression
+gzip compressed data, was "types-aiobotocore-kinesisanalytics-2.5.4.tar", last modified: Tue Aug  8 01:23:57 2023, max compression
```

## Comparing `types-aiobotocore-kinesisanalytics-2.5.2.post2.tar` & `types-aiobotocore-kinesisanalytics-2.5.4.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:14.256643 types-aiobotocore-kinesisanalytics-2.5.2.post2/
--rw-r--r--   0 vlad      (1000) vlad      (1000)     1070 2023-08-04 13:42:05.000000 types-aiobotocore-kinesisanalytics-2.5.2.post2/LICENSE
--rw-r--r--   0 vlad      (1000) vlad      (1000)    12689 2023-08-04 13:59:14.256643 types-aiobotocore-kinesisanalytics-2.5.2.post2/PKG-INFO
--rw-r--r--   0 vlad      (1000) vlad      (1000)    11135 2023-08-04 13:42:05.000000 types-aiobotocore-kinesisanalytics-2.5.2.post2/README.md
--rw-r--r--   0 vlad      (1000) vlad      (1000)       38 2023-08-04 13:59:14.256643 types-aiobotocore-kinesisanalytics-2.5.2.post2/setup.cfg
--rw-r--r--   0 vlad      (1000) vlad      (1000)     2135 2023-08-04 13:42:05.000000 types-aiobotocore-kinesisanalytics-2.5.2.post2/setup.py
-drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:14.246643 types-aiobotocore-kinesisanalytics-2.5.2.post2/types_aiobotocore_kinesisanalytics/
--rw-r--r--   0 vlad      (1000) vlad      (1000)      514 2023-08-04 13:42:05.000000 types-aiobotocore-kinesisanalytics-2.5.2.post2/types_aiobotocore_kinesisanalytics/__init__.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)      513 2023-08-04 13:42:05.000000 types-aiobotocore-kinesisanalytics-2.5.2.post2/types_aiobotocore_kinesisanalytics/__init__.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)      979 2023-08-04 13:42:05.000000 types-aiobotocore-kinesisanalytics-2.5.2.post2/types_aiobotocore_kinesisanalytics/__main__.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)    17025 2023-08-04 13:42:05.000000 types-aiobotocore-kinesisanalytics-2.5.2.post2/types_aiobotocore_kinesisanalytics/client.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)    16997 2023-08-04 13:42:05.000000 types-aiobotocore-kinesisanalytics-2.5.2.post2/types_aiobotocore_kinesisanalytics/client.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)     8548 2023-08-04 13:42:06.000000 types-aiobotocore-kinesisanalytics-2.5.2.post2/types_aiobotocore_kinesisanalytics/literals.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)     8546 2023-08-04 13:42:05.000000 types-aiobotocore-kinesisanalytics-2.5.2.post2/types_aiobotocore_kinesisanalytics/literals.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:42:05.000000 types-aiobotocore-kinesisanalytics-2.5.2.post2/types_aiobotocore_kinesisanalytics/py.typed
--rw-r--r--   0 vlad      (1000) vlad      (1000)    26021 2023-08-04 13:42:06.000000 types-aiobotocore-kinesisanalytics-2.5.2.post2/types_aiobotocore_kinesisanalytics/type_defs.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)    25990 2023-08-04 13:42:06.000000 types-aiobotocore-kinesisanalytics-2.5.2.post2/types_aiobotocore_kinesisanalytics/type_defs.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)       65 2023-08-04 13:42:05.000000 types-aiobotocore-kinesisanalytics-2.5.2.post2/types_aiobotocore_kinesisanalytics/version.py
-drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:14.256643 types-aiobotocore-kinesisanalytics-2.5.2.post2/types_aiobotocore_kinesisanalytics.egg-info/
--rw-r--r--   0 vlad      (1000) vlad      (1000)    12689 2023-08-04 13:59:14.000000 types-aiobotocore-kinesisanalytics-2.5.2.post2/types_aiobotocore_kinesisanalytics.egg-info/PKG-INFO
--rw-r--r--   0 vlad      (1000) vlad      (1000)      887 2023-08-04 13:59:14.000000 types-aiobotocore-kinesisanalytics-2.5.2.post2/types_aiobotocore_kinesisanalytics.egg-info/SOURCES.txt
--rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:14.000000 types-aiobotocore-kinesisanalytics-2.5.2.post2/types_aiobotocore_kinesisanalytics.egg-info/dependency_links.txt
--rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:14.000000 types-aiobotocore-kinesisanalytics-2.5.2.post2/types_aiobotocore_kinesisanalytics.egg-info/not-zip-safe
--rw-r--r--   0 vlad      (1000) vlad      (1000)       52 2023-08-04 13:59:14.000000 types-aiobotocore-kinesisanalytics-2.5.2.post2/types_aiobotocore_kinesisanalytics.egg-info/requires.txt
--rw-r--r--   0 vlad      (1000) vlad      (1000)       35 2023-08-04 13:59:14.000000 types-aiobotocore-kinesisanalytics-2.5.2.post2/types_aiobotocore_kinesisanalytics.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:23:57.530718 types-aiobotocore-kinesisanalytics-2.5.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-08 01:13:37.000000 types-aiobotocore-kinesisanalytics-2.5.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    12683 2023-08-08 01:23:57.526718 types-aiobotocore-kinesisanalytics-2.5.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    11135 2023-08-08 01:13:37.000000 types-aiobotocore-kinesisanalytics-2.5.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-08 01:23:57.530718 types-aiobotocore-kinesisanalytics-2.5.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2129 2023-08-08 01:13:37.000000 types-aiobotocore-kinesisanalytics-2.5.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:23:57.526718 types-aiobotocore-kinesisanalytics-2.5.4/types_aiobotocore_kinesisanalytics/
+-rw-r--r--   0 runner    (1001) docker     (123)      514 2023-08-08 01:13:37.000000 types-aiobotocore-kinesisanalytics-2.5.4/types_aiobotocore_kinesisanalytics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      513 2023-08-08 01:13:37.000000 types-aiobotocore-kinesisanalytics-2.5.4/types_aiobotocore_kinesisanalytics/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      967 2023-08-08 01:13:37.000000 types-aiobotocore-kinesisanalytics-2.5.4/types_aiobotocore_kinesisanalytics/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17025 2023-08-08 01:13:37.000000 types-aiobotocore-kinesisanalytics-2.5.4/types_aiobotocore_kinesisanalytics/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16997 2023-08-08 01:13:37.000000 types-aiobotocore-kinesisanalytics-2.5.4/types_aiobotocore_kinesisanalytics/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8548 2023-08-08 01:13:37.000000 types-aiobotocore-kinesisanalytics-2.5.4/types_aiobotocore_kinesisanalytics/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8546 2023-08-08 01:13:37.000000 types-aiobotocore-kinesisanalytics-2.5.4/types_aiobotocore_kinesisanalytics/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 01:13:37.000000 types-aiobotocore-kinesisanalytics-2.5.4/types_aiobotocore_kinesisanalytics/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    26021 2023-08-08 01:13:38.000000 types-aiobotocore-kinesisanalytics-2.5.4/types_aiobotocore_kinesisanalytics/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25990 2023-08-08 01:13:38.000000 types-aiobotocore-kinesisanalytics-2.5.4/types_aiobotocore_kinesisanalytics/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-08-08 01:13:37.000000 types-aiobotocore-kinesisanalytics-2.5.4/types_aiobotocore_kinesisanalytics/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:23:57.526718 types-aiobotocore-kinesisanalytics-2.5.4/types_aiobotocore_kinesisanalytics.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    12683 2023-08-08 01:23:57.000000 types-aiobotocore-kinesisanalytics-2.5.4/types_aiobotocore_kinesisanalytics.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      887 2023-08-08 01:23:57.000000 types-aiobotocore-kinesisanalytics-2.5.4/types_aiobotocore_kinesisanalytics.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 01:23:57.000000 types-aiobotocore-kinesisanalytics-2.5.4/types_aiobotocore_kinesisanalytics.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 01:23:57.000000 types-aiobotocore-kinesisanalytics-2.5.4/types_aiobotocore_kinesisanalytics.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-08 01:23:57.000000 types-aiobotocore-kinesisanalytics-2.5.4/types_aiobotocore_kinesisanalytics.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-08-08 01:23:57.000000 types-aiobotocore-kinesisanalytics-2.5.4/types_aiobotocore_kinesisanalytics.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-kinesisanalytics-2.5.2.post2/LICENSE` & `types-aiobotocore-kinesisanalytics-2.5.4/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-kinesisanalytics-2.5.2.post2/PKG-INFO` & `types-aiobotocore-kinesisanalytics-2.5.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-kinesisanalytics
-Version: 2.5.2.post2
-Summary: Type annotations for aiobotocore.KinesisAnalytics 2.5.2 service generated with mypy-boto3-builder 7.17.2
+Version: 2.5.4
+Summary: Type annotations for aiobotocore.KinesisAnalytics 2.5.4 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kinesisanalytics/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-kinesisanalytics.svg?color=blue)](https://pypi.org/project/types-aiobotocore-kinesisanalytics)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kinesisanalytics/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-kinesisanalytics)](https://pepy.tech/project/types-aiobotocore-kinesisanalytics)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.KinesisAnalytics 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesisanalytics.html#KinesisAnalytics)
+[aiobotocore.KinesisAnalytics 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesisanalytics.html#KinesisAnalytics)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-kinesisanalytics-2.5.2.post2/README.md` & `types-aiobotocore-kinesisanalytics-2.5.4/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-kinesisanalytics.svg?color=blue)](https://pypi.org/project/types-aiobotocore-kinesisanalytics)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kinesisanalytics/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-kinesisanalytics)](https://pepy.tech/project/types-aiobotocore-kinesisanalytics)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.KinesisAnalytics 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesisanalytics.html#KinesisAnalytics)
+[aiobotocore.KinesisAnalytics 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesisanalytics.html#KinesisAnalytics)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-kinesisanalytics-2.5.2.post2/setup.py` & `types-aiobotocore-kinesisanalytics-2.5.4/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-kinesisanalytics",
-    version="2.5.2.post2",
+    version="2.5.4",
     packages=["types_aiobotocore_kinesisanalytics"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.KinesisAnalytics 2.5.2 service generated with"
+        "Type annotations for aiobotocore.KinesisAnalytics 2.5.4 service generated with"
         " mypy-boto3-builder 7.17.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
```

### Comparing `types-aiobotocore-kinesisanalytics-2.5.2.post2/types_aiobotocore_kinesisanalytics/__init__.py` & `types-aiobotocore-kinesisanalytics-2.5.4/types_aiobotocore_kinesisanalytics/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-kinesisanalytics-2.5.2.post2/types_aiobotocore_kinesisanalytics/__init__.pyi` & `types-aiobotocore-kinesisanalytics-2.5.4/types_aiobotocore_kinesisanalytics/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-kinesisanalytics-2.5.2.post2/types_aiobotocore_kinesisanalytics/client.py` & `types-aiobotocore-kinesisanalytics-2.5.4/types_aiobotocore_kinesisanalytics/client.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-kinesisanalytics-2.5.2.post2/types_aiobotocore_kinesisanalytics/client.pyi` & `types-aiobotocore-kinesisanalytics-2.5.4/types_aiobotocore_kinesisanalytics/client.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-kinesisanalytics-2.5.2.post2/types_aiobotocore_kinesisanalytics/literals.py` & `types-aiobotocore-kinesisanalytics-2.5.4/types_aiobotocore_kinesisanalytics/literals.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-kinesisanalytics-2.5.2.post2/types_aiobotocore_kinesisanalytics/literals.pyi` & `types-aiobotocore-kinesisanalytics-2.5.4/types_aiobotocore_kinesisanalytics/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-kinesisanalytics-2.5.2.post2/types_aiobotocore_kinesisanalytics/type_defs.py` & `types-aiobotocore-kinesisanalytics-2.5.4/types_aiobotocore_kinesisanalytics/type_defs.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-kinesisanalytics-2.5.2.post2/types_aiobotocore_kinesisanalytics/type_defs.pyi` & `types-aiobotocore-kinesisanalytics-2.5.4/types_aiobotocore_kinesisanalytics/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-kinesisanalytics-2.5.2.post2/types_aiobotocore_kinesisanalytics.egg-info/PKG-INFO` & `types-aiobotocore-kinesisanalytics-2.5.4/types_aiobotocore_kinesisanalytics.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-kinesisanalytics
-Version: 2.5.2.post2
-Summary: Type annotations for aiobotocore.KinesisAnalytics 2.5.2 service generated with mypy-boto3-builder 7.17.2
+Version: 2.5.4
+Summary: Type annotations for aiobotocore.KinesisAnalytics 2.5.4 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kinesisanalytics/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-kinesisanalytics.svg?color=blue)](https://pypi.org/project/types-aiobotocore-kinesisanalytics)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kinesisanalytics/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-kinesisanalytics)](https://pepy.tech/project/types-aiobotocore-kinesisanalytics)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.KinesisAnalytics 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesisanalytics.html#KinesisAnalytics)
+[aiobotocore.KinesisAnalytics 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesisanalytics.html#KinesisAnalytics)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-kinesisanalytics-2.5.2.post2/types_aiobotocore_kinesisanalytics.egg-info/SOURCES.txt` & `types-aiobotocore-kinesisanalytics-2.5.4/types_aiobotocore_kinesisanalytics.egg-info/SOURCES.txt`

 * *Files identical despite different names*


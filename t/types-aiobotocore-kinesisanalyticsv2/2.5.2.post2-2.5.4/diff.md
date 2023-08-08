# Comparing `tmp/types-aiobotocore-kinesisanalyticsv2-2.5.2.post2.tar.gz` & `tmp/types-aiobotocore-kinesisanalyticsv2-2.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-kinesisanalyticsv2-2.5.2.post2.tar", last modified: Fri Aug  4 13:59:14 2023, max compression
+gzip compressed data, was "types-aiobotocore-kinesisanalyticsv2-2.5.4.tar", last modified: Tue Aug  8 01:23:57 2023, max compression
```

## Comparing `types-aiobotocore-kinesisanalyticsv2-2.5.2.post2.tar` & `types-aiobotocore-kinesisanalyticsv2-2.5.4.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:14.326643 types-aiobotocore-kinesisanalyticsv2-2.5.2.post2/
--rw-r--r--   0 vlad      (1000) vlad      (1000)     1070 2023-08-04 13:42:08.000000 types-aiobotocore-kinesisanalyticsv2-2.5.2.post2/LICENSE
--rw-r--r--   0 vlad      (1000) vlad      (1000)    13781 2023-08-04 13:59:14.316643 types-aiobotocore-kinesisanalyticsv2-2.5.2.post2/PKG-INFO
--rw-r--r--   0 vlad      (1000) vlad      (1000)    12219 2023-08-04 13:42:08.000000 types-aiobotocore-kinesisanalyticsv2-2.5.2.post2/README.md
--rw-r--r--   0 vlad      (1000) vlad      (1000)       38 2023-08-04 13:59:14.326643 types-aiobotocore-kinesisanalyticsv2-2.5.2.post2/setup.cfg
--rw-r--r--   0 vlad      (1000) vlad      (1000)     2149 2023-08-04 13:42:08.000000 types-aiobotocore-kinesisanalyticsv2-2.5.2.post2/setup.py
-drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:14.316643 types-aiobotocore-kinesisanalyticsv2-2.5.2.post2/types_aiobotocore_kinesisanalyticsv2/
--rw-r--r--   0 vlad      (1000) vlad      (1000)     1010 2023-08-04 13:42:08.000000 types-aiobotocore-kinesisanalyticsv2-2.5.2.post2/types_aiobotocore_kinesisanalyticsv2/__init__.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)     1009 2023-08-04 13:42:08.000000 types-aiobotocore-kinesisanalyticsv2-2.5.2.post2/types_aiobotocore_kinesisanalyticsv2/__init__.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)      987 2023-08-04 13:42:08.000000 types-aiobotocore-kinesisanalyticsv2-2.5.2.post2/types_aiobotocore_kinesisanalyticsv2/__main__.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)    29367 2023-08-04 13:42:09.000000 types-aiobotocore-kinesisanalyticsv2-2.5.2.post2/types_aiobotocore_kinesisanalyticsv2/client.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)    29325 2023-08-04 13:42:09.000000 types-aiobotocore-kinesisanalyticsv2-2.5.2.post2/types_aiobotocore_kinesisanalyticsv2/client.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)    10103 2023-08-04 13:42:09.000000 types-aiobotocore-kinesisanalyticsv2-2.5.2.post2/types_aiobotocore_kinesisanalyticsv2/literals.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)    10101 2023-08-04 13:42:09.000000 types-aiobotocore-kinesisanalyticsv2-2.5.2.post2/types_aiobotocore_kinesisanalyticsv2/literals.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)     3422 2023-08-04 13:42:09.000000 types-aiobotocore-kinesisanalyticsv2-2.5.2.post2/types_aiobotocore_kinesisanalyticsv2/paginator.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)     3418 2023-08-04 13:42:09.000000 types-aiobotocore-kinesisanalyticsv2-2.5.2.post2/types_aiobotocore_kinesisanalyticsv2/paginator.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:42:08.000000 types-aiobotocore-kinesisanalyticsv2-2.5.2.post2/types_aiobotocore_kinesisanalyticsv2/py.typed
--rw-r--r--   0 vlad      (1000) vlad      (1000)    69136 2023-08-04 13:42:11.000000 types-aiobotocore-kinesisanalyticsv2-2.5.2.post2/types_aiobotocore_kinesisanalyticsv2/type_defs.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)    69035 2023-08-04 13:42:10.000000 types-aiobotocore-kinesisanalyticsv2-2.5.2.post2/types_aiobotocore_kinesisanalyticsv2/type_defs.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)       65 2023-08-04 13:42:08.000000 types-aiobotocore-kinesisanalyticsv2-2.5.2.post2/types_aiobotocore_kinesisanalyticsv2/version.py
-drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:14.316643 types-aiobotocore-kinesisanalyticsv2-2.5.2.post2/types_aiobotocore_kinesisanalyticsv2.egg-info/
--rw-r--r--   0 vlad      (1000) vlad      (1000)    13781 2023-08-04 13:59:14.000000 types-aiobotocore-kinesisanalyticsv2-2.5.2.post2/types_aiobotocore_kinesisanalyticsv2.egg-info/PKG-INFO
--rw-r--r--   0 vlad      (1000) vlad      (1000)     1022 2023-08-04 13:59:14.000000 types-aiobotocore-kinesisanalyticsv2-2.5.2.post2/types_aiobotocore_kinesisanalyticsv2.egg-info/SOURCES.txt
--rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:14.000000 types-aiobotocore-kinesisanalyticsv2-2.5.2.post2/types_aiobotocore_kinesisanalyticsv2.egg-info/dependency_links.txt
--rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:14.000000 types-aiobotocore-kinesisanalyticsv2-2.5.2.post2/types_aiobotocore_kinesisanalyticsv2.egg-info/not-zip-safe
--rw-r--r--   0 vlad      (1000) vlad      (1000)       52 2023-08-04 13:59:14.000000 types-aiobotocore-kinesisanalyticsv2-2.5.2.post2/types_aiobotocore_kinesisanalyticsv2.egg-info/requires.txt
--rw-r--r--   0 vlad      (1000) vlad      (1000)       37 2023-08-04 13:59:14.000000 types-aiobotocore-kinesisanalyticsv2-2.5.2.post2/types_aiobotocore_kinesisanalyticsv2.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:23:57.630718 types-aiobotocore-kinesisanalyticsv2-2.5.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-08 01:13:38.000000 types-aiobotocore-kinesisanalyticsv2-2.5.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    13775 2023-08-08 01:23:57.626718 types-aiobotocore-kinesisanalyticsv2-2.5.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    12219 2023-08-08 01:13:38.000000 types-aiobotocore-kinesisanalyticsv2-2.5.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-08 01:23:57.630718 types-aiobotocore-kinesisanalyticsv2-2.5.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2143 2023-08-08 01:13:38.000000 types-aiobotocore-kinesisanalyticsv2-2.5.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:23:57.622718 types-aiobotocore-kinesisanalyticsv2-2.5.4/types_aiobotocore_kinesisanalyticsv2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1010 2023-08-08 01:13:38.000000 types-aiobotocore-kinesisanalyticsv2-2.5.4/types_aiobotocore_kinesisanalyticsv2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1009 2023-08-08 01:13:38.000000 types-aiobotocore-kinesisanalyticsv2-2.5.4/types_aiobotocore_kinesisanalyticsv2/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      975 2023-08-08 01:13:38.000000 types-aiobotocore-kinesisanalyticsv2-2.5.4/types_aiobotocore_kinesisanalyticsv2/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29367 2023-08-08 01:13:39.000000 types-aiobotocore-kinesisanalyticsv2-2.5.4/types_aiobotocore_kinesisanalyticsv2/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29325 2023-08-08 01:13:39.000000 types-aiobotocore-kinesisanalyticsv2-2.5.4/types_aiobotocore_kinesisanalyticsv2/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    10103 2023-08-08 01:13:39.000000 types-aiobotocore-kinesisanalyticsv2-2.5.4/types_aiobotocore_kinesisanalyticsv2/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10101 2023-08-08 01:13:39.000000 types-aiobotocore-kinesisanalyticsv2-2.5.4/types_aiobotocore_kinesisanalyticsv2/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     3422 2023-08-08 01:13:39.000000 types-aiobotocore-kinesisanalyticsv2-2.5.4/types_aiobotocore_kinesisanalyticsv2/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3418 2023-08-08 01:13:39.000000 types-aiobotocore-kinesisanalyticsv2-2.5.4/types_aiobotocore_kinesisanalyticsv2/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 01:13:38.000000 types-aiobotocore-kinesisanalyticsv2-2.5.4/types_aiobotocore_kinesisanalyticsv2/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    69136 2023-08-08 01:13:42.000000 types-aiobotocore-kinesisanalyticsv2-2.5.4/types_aiobotocore_kinesisanalyticsv2/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    69035 2023-08-08 01:13:41.000000 types-aiobotocore-kinesisanalyticsv2-2.5.4/types_aiobotocore_kinesisanalyticsv2/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-08-08 01:13:38.000000 types-aiobotocore-kinesisanalyticsv2-2.5.4/types_aiobotocore_kinesisanalyticsv2/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:23:57.626718 types-aiobotocore-kinesisanalyticsv2-2.5.4/types_aiobotocore_kinesisanalyticsv2.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    13775 2023-08-08 01:23:57.000000 types-aiobotocore-kinesisanalyticsv2-2.5.4/types_aiobotocore_kinesisanalyticsv2.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1022 2023-08-08 01:23:57.000000 types-aiobotocore-kinesisanalyticsv2-2.5.4/types_aiobotocore_kinesisanalyticsv2.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 01:23:57.000000 types-aiobotocore-kinesisanalyticsv2-2.5.4/types_aiobotocore_kinesisanalyticsv2.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 01:23:57.000000 types-aiobotocore-kinesisanalyticsv2-2.5.4/types_aiobotocore_kinesisanalyticsv2.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-08 01:23:57.000000 types-aiobotocore-kinesisanalyticsv2-2.5.4/types_aiobotocore_kinesisanalyticsv2.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-08-08 01:23:57.000000 types-aiobotocore-kinesisanalyticsv2-2.5.4/types_aiobotocore_kinesisanalyticsv2.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-kinesisanalyticsv2-2.5.2.post2/LICENSE` & `types-aiobotocore-kinesisanalyticsv2-2.5.4/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-kinesisanalyticsv2-2.5.2.post2/PKG-INFO` & `types-aiobotocore-kinesisanalyticsv2-2.5.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-kinesisanalyticsv2
-Version: 2.5.2.post2
-Summary: Type annotations for aiobotocore.KinesisAnalyticsV2 2.5.2 service generated with mypy-boto3-builder 7.17.2
+Version: 2.5.4
+Summary: Type annotations for aiobotocore.KinesisAnalyticsV2 2.5.4 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kinesisanalyticsv2/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-kinesisanalyticsv2.svg?color=blue)](https://pypi.org/project/types-aiobotocore-kinesisanalyticsv2)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kinesisanalyticsv2/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-kinesisanalyticsv2)](https://pepy.tech/project/types-aiobotocore-kinesisanalyticsv2)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.KinesisAnalyticsV2 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesisanalyticsv2.html#KinesisAnalyticsV2)
+[aiobotocore.KinesisAnalyticsV2 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesisanalyticsv2.html#KinesisAnalyticsV2)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-kinesisanalyticsv2-2.5.2.post2/README.md` & `types-aiobotocore-kinesisanalyticsv2-2.5.4/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-kinesisanalyticsv2.svg?color=blue)](https://pypi.org/project/types-aiobotocore-kinesisanalyticsv2)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kinesisanalyticsv2/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-kinesisanalyticsv2)](https://pepy.tech/project/types-aiobotocore-kinesisanalyticsv2)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.KinesisAnalyticsV2 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesisanalyticsv2.html#KinesisAnalyticsV2)
+[aiobotocore.KinesisAnalyticsV2 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesisanalyticsv2.html#KinesisAnalyticsV2)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-kinesisanalyticsv2-2.5.2.post2/setup.py` & `types-aiobotocore-kinesisanalyticsv2-2.5.4/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-kinesisanalyticsv2",
-    version="2.5.2.post2",
+    version="2.5.4",
     packages=["types_aiobotocore_kinesisanalyticsv2"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.KinesisAnalyticsV2 2.5.2 service generated with"
+        "Type annotations for aiobotocore.KinesisAnalyticsV2 2.5.4 service generated with"
         " mypy-boto3-builder 7.17.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
```

### Comparing `types-aiobotocore-kinesisanalyticsv2-2.5.2.post2/types_aiobotocore_kinesisanalyticsv2/__init__.py` & `types-aiobotocore-kinesisanalyticsv2-2.5.4/types_aiobotocore_kinesisanalyticsv2/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-kinesisanalyticsv2-2.5.2.post2/types_aiobotocore_kinesisanalyticsv2/__init__.pyi` & `types-aiobotocore-kinesisanalyticsv2-2.5.4/types_aiobotocore_kinesisanalyticsv2/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-kinesisanalyticsv2-2.5.2.post2/types_aiobotocore_kinesisanalyticsv2/__main__.py` & `types-aiobotocore-kinesisanalyticsv2-2.5.4/types_aiobotocore_kinesisanalyticsv2/__main__.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.KinesisAnalyticsV2 2.5.2\nVersion:        "
-        " 2.5.2.post2\nBuilder version: 7.17.2\nDocs:           "
+        "Type annotations for aiobotocore.KinesisAnalyticsV2 2.5.4\nVersion:         2.5.4\nBuilder"
+        " version: 7.17.2\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kinesisanalyticsv2//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesisanalyticsv2.html#KinesisAnalyticsV2\nOther"
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

### Comparing `types-aiobotocore-kinesisanalyticsv2-2.5.2.post2/types_aiobotocore_kinesisanalyticsv2/client.py` & `types-aiobotocore-kinesisanalyticsv2-2.5.4/types_aiobotocore_kinesisanalyticsv2/client.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-kinesisanalyticsv2-2.5.2.post2/types_aiobotocore_kinesisanalyticsv2/client.pyi` & `types-aiobotocore-kinesisanalyticsv2-2.5.4/types_aiobotocore_kinesisanalyticsv2/client.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-kinesisanalyticsv2-2.5.2.post2/types_aiobotocore_kinesisanalyticsv2/literals.py` & `types-aiobotocore-kinesisanalyticsv2-2.5.4/types_aiobotocore_kinesisanalyticsv2/literals.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-kinesisanalyticsv2-2.5.2.post2/types_aiobotocore_kinesisanalyticsv2/literals.pyi` & `types-aiobotocore-kinesisanalyticsv2-2.5.4/types_aiobotocore_kinesisanalyticsv2/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-kinesisanalyticsv2-2.5.2.post2/types_aiobotocore_kinesisanalyticsv2/paginator.py` & `types-aiobotocore-kinesisanalyticsv2-2.5.4/types_aiobotocore_kinesisanalyticsv2/paginator.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-kinesisanalyticsv2-2.5.2.post2/types_aiobotocore_kinesisanalyticsv2/paginator.pyi` & `types-aiobotocore-kinesisanalyticsv2-2.5.4/types_aiobotocore_kinesisanalyticsv2/paginator.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-kinesisanalyticsv2-2.5.2.post2/types_aiobotocore_kinesisanalyticsv2/type_defs.py` & `types-aiobotocore-kinesisanalyticsv2-2.5.4/types_aiobotocore_kinesisanalyticsv2/type_defs.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-kinesisanalyticsv2-2.5.2.post2/types_aiobotocore_kinesisanalyticsv2/type_defs.pyi` & `types-aiobotocore-kinesisanalyticsv2-2.5.4/types_aiobotocore_kinesisanalyticsv2/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-kinesisanalyticsv2-2.5.2.post2/types_aiobotocore_kinesisanalyticsv2.egg-info/PKG-INFO` & `types-aiobotocore-kinesisanalyticsv2-2.5.4/types_aiobotocore_kinesisanalyticsv2.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-kinesisanalyticsv2
-Version: 2.5.2.post2
-Summary: Type annotations for aiobotocore.KinesisAnalyticsV2 2.5.2 service generated with mypy-boto3-builder 7.17.2
+Version: 2.5.4
+Summary: Type annotations for aiobotocore.KinesisAnalyticsV2 2.5.4 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kinesisanalyticsv2/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-kinesisanalyticsv2.svg?color=blue)](https://pypi.org/project/types-aiobotocore-kinesisanalyticsv2)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kinesisanalyticsv2/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-kinesisanalyticsv2)](https://pepy.tech/project/types-aiobotocore-kinesisanalyticsv2)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.KinesisAnalyticsV2 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesisanalyticsv2.html#KinesisAnalyticsV2)
+[aiobotocore.KinesisAnalyticsV2 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesisanalyticsv2.html#KinesisAnalyticsV2)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-kinesisanalyticsv2-2.5.2.post2/types_aiobotocore_kinesisanalyticsv2.egg-info/SOURCES.txt` & `types-aiobotocore-kinesisanalyticsv2-2.5.4/types_aiobotocore_kinesisanalyticsv2.egg-info/SOURCES.txt`

 * *Files identical despite different names*


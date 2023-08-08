# Comparing `tmp/types-aiobotocore-kinesisvideo-2.5.2.post2.tar.gz` & `tmp/types-aiobotocore-kinesisvideo-2.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-kinesisvideo-2.5.2.post2.tar", last modified: Fri Aug  4 13:59:14 2023, max compression
+gzip compressed data, was "types-aiobotocore-kinesisvideo-2.5.4.tar", last modified: Tue Aug  8 01:23:58 2023, max compression
```

## Comparing `types-aiobotocore-kinesisvideo-2.5.2.post2.tar` & `types-aiobotocore-kinesisvideo-2.5.4.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:14.406643 types-aiobotocore-kinesisvideo-2.5.2.post2/
--rw-r--r--   0 vlad      (1000) vlad      (1000)     1070 2023-08-04 13:42:12.000000 types-aiobotocore-kinesisvideo-2.5.2.post2/LICENSE
--rw-r--r--   0 vlad      (1000) vlad      (1000)    13795 2023-08-04 13:59:14.396643 types-aiobotocore-kinesisvideo-2.5.2.post2/PKG-INFO
--rw-r--r--   0 vlad      (1000) vlad      (1000)    12257 2023-08-04 13:42:12.000000 types-aiobotocore-kinesisvideo-2.5.2.post2/README.md
--rw-r--r--   0 vlad      (1000) vlad      (1000)       38 2023-08-04 13:59:14.406643 types-aiobotocore-kinesisvideo-2.5.2.post2/setup.cfg
--rw-r--r--   0 vlad      (1000) vlad      (1000)     2107 2023-08-04 13:42:12.000000 types-aiobotocore-kinesisvideo-2.5.2.post2/setup.py
-drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:14.396643 types-aiobotocore-kinesisvideo-2.5.2.post2/types_aiobotocore_kinesisvideo/
--rw-r--r--   0 vlad      (1000) vlad      (1000)     1519 2023-08-04 13:42:12.000000 types-aiobotocore-kinesisvideo-2.5.2.post2/types_aiobotocore_kinesisvideo/__init__.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)     1518 2023-08-04 13:42:12.000000 types-aiobotocore-kinesisvideo-2.5.2.post2/types_aiobotocore_kinesisvideo/__init__.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)      963 2023-08-04 13:42:12.000000 types-aiobotocore-kinesisvideo-2.5.2.post2/types_aiobotocore_kinesisvideo/__main__.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)    26786 2023-08-04 13:42:13.000000 types-aiobotocore-kinesisvideo-2.5.2.post2/types_aiobotocore_kinesisvideo/client.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)    26743 2023-08-04 13:42:12.000000 types-aiobotocore-kinesisvideo-2.5.2.post2/types_aiobotocore_kinesisvideo/client.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)    10404 2023-08-04 13:42:13.000000 types-aiobotocore-kinesisvideo-2.5.2.post2/types_aiobotocore_kinesisvideo/literals.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)    10402 2023-08-04 13:42:13.000000 types-aiobotocore-kinesisvideo-2.5.2.post2/types_aiobotocore_kinesisvideo/literals.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)     6098 2023-08-04 13:42:13.000000 types-aiobotocore-kinesisvideo-2.5.2.post2/types_aiobotocore_kinesisvideo/paginator.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)     6092 2023-08-04 13:42:13.000000 types-aiobotocore-kinesisvideo-2.5.2.post2/types_aiobotocore_kinesisvideo/paginator.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:42:12.000000 types-aiobotocore-kinesisvideo-2.5.2.post2/types_aiobotocore_kinesisvideo/py.typed
--rw-r--r--   0 vlad      (1000) vlad      (1000)    28618 2023-08-04 13:42:14.000000 types-aiobotocore-kinesisvideo-2.5.2.post2/types_aiobotocore_kinesisvideo/type_defs.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)    28579 2023-08-04 13:42:13.000000 types-aiobotocore-kinesisvideo-2.5.2.post2/types_aiobotocore_kinesisvideo/type_defs.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)       65 2023-08-04 13:42:12.000000 types-aiobotocore-kinesisvideo-2.5.2.post2/types_aiobotocore_kinesisvideo/version.py
-drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:14.396643 types-aiobotocore-kinesisvideo-2.5.2.post2/types_aiobotocore_kinesisvideo.egg-info/
--rw-r--r--   0 vlad      (1000) vlad      (1000)    13795 2023-08-04 13:59:14.000000 types-aiobotocore-kinesisvideo-2.5.2.post2/types_aiobotocore_kinesisvideo.egg-info/PKG-INFO
--rw-r--r--   0 vlad      (1000) vlad      (1000)      908 2023-08-04 13:59:14.000000 types-aiobotocore-kinesisvideo-2.5.2.post2/types_aiobotocore_kinesisvideo.egg-info/SOURCES.txt
--rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:14.000000 types-aiobotocore-kinesisvideo-2.5.2.post2/types_aiobotocore_kinesisvideo.egg-info/dependency_links.txt
--rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:14.000000 types-aiobotocore-kinesisvideo-2.5.2.post2/types_aiobotocore_kinesisvideo.egg-info/not-zip-safe
--rw-r--r--   0 vlad      (1000) vlad      (1000)       52 2023-08-04 13:59:14.000000 types-aiobotocore-kinesisvideo-2.5.2.post2/types_aiobotocore_kinesisvideo.egg-info/requires.txt
--rw-r--r--   0 vlad      (1000) vlad      (1000)       31 2023-08-04 13:59:14.000000 types-aiobotocore-kinesisvideo-2.5.2.post2/types_aiobotocore_kinesisvideo.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:23:58.010719 types-aiobotocore-kinesisvideo-2.5.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-08 01:13:42.000000 types-aiobotocore-kinesisvideo-2.5.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    13789 2023-08-08 01:23:58.010719 types-aiobotocore-kinesisvideo-2.5.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    12257 2023-08-08 01:13:42.000000 types-aiobotocore-kinesisvideo-2.5.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-08 01:23:58.010719 types-aiobotocore-kinesisvideo-2.5.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2101 2023-08-08 01:13:42.000000 types-aiobotocore-kinesisvideo-2.5.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:23:58.010719 types-aiobotocore-kinesisvideo-2.5.4/types_aiobotocore_kinesisvideo/
+-rw-r--r--   0 runner    (1001) docker     (123)     1519 2023-08-08 01:13:42.000000 types-aiobotocore-kinesisvideo-2.5.4/types_aiobotocore_kinesisvideo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1518 2023-08-08 01:13:42.000000 types-aiobotocore-kinesisvideo-2.5.4/types_aiobotocore_kinesisvideo/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      951 2023-08-08 01:13:42.000000 types-aiobotocore-kinesisvideo-2.5.4/types_aiobotocore_kinesisvideo/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26786 2023-08-08 01:13:42.000000 types-aiobotocore-kinesisvideo-2.5.4/types_aiobotocore_kinesisvideo/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26743 2023-08-08 01:13:42.000000 types-aiobotocore-kinesisvideo-2.5.4/types_aiobotocore_kinesisvideo/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    10404 2023-08-08 01:13:42.000000 types-aiobotocore-kinesisvideo-2.5.4/types_aiobotocore_kinesisvideo/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10402 2023-08-08 01:13:42.000000 types-aiobotocore-kinesisvideo-2.5.4/types_aiobotocore_kinesisvideo/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     6098 2023-08-08 01:13:42.000000 types-aiobotocore-kinesisvideo-2.5.4/types_aiobotocore_kinesisvideo/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6092 2023-08-08 01:13:42.000000 types-aiobotocore-kinesisvideo-2.5.4/types_aiobotocore_kinesisvideo/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 01:13:42.000000 types-aiobotocore-kinesisvideo-2.5.4/types_aiobotocore_kinesisvideo/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    28618 2023-08-08 01:13:43.000000 types-aiobotocore-kinesisvideo-2.5.4/types_aiobotocore_kinesisvideo/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28579 2023-08-08 01:13:43.000000 types-aiobotocore-kinesisvideo-2.5.4/types_aiobotocore_kinesisvideo/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-08-08 01:13:42.000000 types-aiobotocore-kinesisvideo-2.5.4/types_aiobotocore_kinesisvideo/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:23:58.010719 types-aiobotocore-kinesisvideo-2.5.4/types_aiobotocore_kinesisvideo.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    13789 2023-08-08 01:23:57.000000 types-aiobotocore-kinesisvideo-2.5.4/types_aiobotocore_kinesisvideo.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      908 2023-08-08 01:23:57.000000 types-aiobotocore-kinesisvideo-2.5.4/types_aiobotocore_kinesisvideo.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 01:23:57.000000 types-aiobotocore-kinesisvideo-2.5.4/types_aiobotocore_kinesisvideo.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 01:23:57.000000 types-aiobotocore-kinesisvideo-2.5.4/types_aiobotocore_kinesisvideo.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-08 01:23:57.000000 types-aiobotocore-kinesisvideo-2.5.4/types_aiobotocore_kinesisvideo.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-08-08 01:23:57.000000 types-aiobotocore-kinesisvideo-2.5.4/types_aiobotocore_kinesisvideo.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-kinesisvideo-2.5.2.post2/LICENSE` & `types-aiobotocore-kinesisvideo-2.5.4/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-kinesisvideo-2.5.2.post2/PKG-INFO` & `types-aiobotocore-kinesisvideo-2.5.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-kinesisvideo
-Version: 2.5.2.post2
-Summary: Type annotations for aiobotocore.KinesisVideo 2.5.2 service generated with mypy-boto3-builder 7.17.2
+Version: 2.5.4
+Summary: Type annotations for aiobotocore.KinesisVideo 2.5.4 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kinesisvideo/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-kinesisvideo.svg?color=blue)](https://pypi.org/project/types-aiobotocore-kinesisvideo)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kinesisvideo/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-kinesisvideo)](https://pepy.tech/project/types-aiobotocore-kinesisvideo)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.KinesisVideo 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesisvideo.html#KinesisVideo)
+[aiobotocore.KinesisVideo 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesisvideo.html#KinesisVideo)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-kinesisvideo-2.5.2.post2/README.md` & `types-aiobotocore-kinesisvideo-2.5.4/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-kinesisvideo.svg?color=blue)](https://pypi.org/project/types-aiobotocore-kinesisvideo)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kinesisvideo/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-kinesisvideo)](https://pepy.tech/project/types-aiobotocore-kinesisvideo)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.KinesisVideo 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesisvideo.html#KinesisVideo)
+[aiobotocore.KinesisVideo 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesisvideo.html#KinesisVideo)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-kinesisvideo-2.5.2.post2/setup.py` & `types-aiobotocore-kinesisvideo-2.5.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-kinesisvideo",
-    version="2.5.2.post2",
+    version="2.5.4",
     packages=["types_aiobotocore_kinesisvideo"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.KinesisVideo 2.5.2 service generated with"
+        "Type annotations for aiobotocore.KinesisVideo 2.5.4 service generated with"
         " mypy-boto3-builder 7.17.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
```

### Comparing `types-aiobotocore-kinesisvideo-2.5.2.post2/types_aiobotocore_kinesisvideo/__init__.py` & `types-aiobotocore-kinesisvideo-2.5.4/types_aiobotocore_kinesisvideo/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-kinesisvideo-2.5.2.post2/types_aiobotocore_kinesisvideo/__init__.pyi` & `types-aiobotocore-kinesisvideo-2.5.4/types_aiobotocore_kinesisvideo/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-kinesisvideo-2.5.2.post2/types_aiobotocore_kinesisvideo/__main__.py` & `types-aiobotocore-kinesisvideo-2.5.4/types_aiobotocore_kinesisvideo/__main__.py`

 * *Files 20% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.KinesisVideo 2.5.2\nVersion:         2.5.2.post2\nBuilder"
+        "Type annotations for aiobotocore.KinesisVideo 2.5.4\nVersion:         2.5.4\nBuilder"
         " version: 7.17.2\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kinesisvideo//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesisvideo.html#KinesisVideo\nOther"
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

### Comparing `types-aiobotocore-kinesisvideo-2.5.2.post2/types_aiobotocore_kinesisvideo/client.py` & `types-aiobotocore-kinesisvideo-2.5.4/types_aiobotocore_kinesisvideo/client.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-kinesisvideo-2.5.2.post2/types_aiobotocore_kinesisvideo/client.pyi` & `types-aiobotocore-kinesisvideo-2.5.4/types_aiobotocore_kinesisvideo/client.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-kinesisvideo-2.5.2.post2/types_aiobotocore_kinesisvideo/literals.py` & `types-aiobotocore-kinesisvideo-2.5.4/types_aiobotocore_kinesisvideo/literals.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-kinesisvideo-2.5.2.post2/types_aiobotocore_kinesisvideo/literals.pyi` & `types-aiobotocore-kinesisvideo-2.5.4/types_aiobotocore_kinesisvideo/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-kinesisvideo-2.5.2.post2/types_aiobotocore_kinesisvideo/paginator.py` & `types-aiobotocore-kinesisvideo-2.5.4/types_aiobotocore_kinesisvideo/paginator.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-kinesisvideo-2.5.2.post2/types_aiobotocore_kinesisvideo/paginator.pyi` & `types-aiobotocore-kinesisvideo-2.5.4/types_aiobotocore_kinesisvideo/paginator.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-kinesisvideo-2.5.2.post2/types_aiobotocore_kinesisvideo/type_defs.py` & `types-aiobotocore-kinesisvideo-2.5.4/types_aiobotocore_kinesisvideo/type_defs.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-kinesisvideo-2.5.2.post2/types_aiobotocore_kinesisvideo/type_defs.pyi` & `types-aiobotocore-kinesisvideo-2.5.4/types_aiobotocore_kinesisvideo/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-kinesisvideo-2.5.2.post2/types_aiobotocore_kinesisvideo.egg-info/PKG-INFO` & `types-aiobotocore-kinesisvideo-2.5.4/types_aiobotocore_kinesisvideo.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-kinesisvideo
-Version: 2.5.2.post2
-Summary: Type annotations for aiobotocore.KinesisVideo 2.5.2 service generated with mypy-boto3-builder 7.17.2
+Version: 2.5.4
+Summary: Type annotations for aiobotocore.KinesisVideo 2.5.4 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kinesisvideo/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-kinesisvideo.svg?color=blue)](https://pypi.org/project/types-aiobotocore-kinesisvideo)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kinesisvideo/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-kinesisvideo)](https://pepy.tech/project/types-aiobotocore-kinesisvideo)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.KinesisVideo 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesisvideo.html#KinesisVideo)
+[aiobotocore.KinesisVideo 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesisvideo.html#KinesisVideo)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-kinesisvideo-2.5.2.post2/types_aiobotocore_kinesisvideo.egg-info/SOURCES.txt` & `types-aiobotocore-kinesisvideo-2.5.4/types_aiobotocore_kinesisvideo.egg-info/SOURCES.txt`

 * *Files identical despite different names*


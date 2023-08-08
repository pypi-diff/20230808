# Comparing `tmp/types-aiobotocore-mediaconnect-2.5.2.post2.tar.gz` & `tmp/types-aiobotocore-mediaconnect-2.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-mediaconnect-2.5.2.post2.tar", last modified: Fri Aug  4 13:59:17 2023, max compression
+gzip compressed data, was "types-aiobotocore-mediaconnect-2.5.4.tar", last modified: Tue Aug  8 01:24:04 2023, max compression
```

## Comparing `types-aiobotocore-mediaconnect-2.5.2.post2.tar` & `types-aiobotocore-mediaconnect-2.5.4.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:17.326643 types-aiobotocore-mediaconnect-2.5.2.post2/
--rw-r--r--   0 vlad      (1000) vlad      (1000)     1070 2023-08-04 13:43:58.000000 types-aiobotocore-mediaconnect-2.5.2.post2/LICENSE
--rw-r--r--   0 vlad      (1000) vlad      (1000)    14917 2023-08-04 13:59:17.326643 types-aiobotocore-mediaconnect-2.5.2.post2/PKG-INFO
--rw-r--r--   0 vlad      (1000) vlad      (1000)    13379 2023-08-04 13:43:58.000000 types-aiobotocore-mediaconnect-2.5.2.post2/README.md
--rw-r--r--   0 vlad      (1000) vlad      (1000)       38 2023-08-04 13:59:17.326643 types-aiobotocore-mediaconnect-2.5.2.post2/setup.cfg
--rw-r--r--   0 vlad      (1000) vlad      (1000)     2107 2023-08-04 13:43:58.000000 types-aiobotocore-mediaconnect-2.5.2.post2/setup.py
-drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:17.326643 types-aiobotocore-mediaconnect-2.5.2.post2/types_aiobotocore_mediaconnect/
--rw-r--r--   0 vlad      (1000) vlad      (1000)     2311 2023-08-04 13:43:58.000000 types-aiobotocore-mediaconnect-2.5.2.post2/types_aiobotocore_mediaconnect/__init__.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)     2310 2023-08-04 13:43:58.000000 types-aiobotocore-mediaconnect-2.5.2.post2/types_aiobotocore_mediaconnect/__init__.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)      963 2023-08-04 13:43:58.000000 types-aiobotocore-mediaconnect-2.5.2.post2/types_aiobotocore_mediaconnect/__main__.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)    42802 2023-08-04 13:43:58.000000 types-aiobotocore-mediaconnect-2.5.2.post2/types_aiobotocore_mediaconnect/client.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)    42733 2023-08-04 13:43:58.000000 types-aiobotocore-mediaconnect-2.5.2.post2/types_aiobotocore_mediaconnect/client.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)    11974 2023-08-04 13:43:59.000000 types-aiobotocore-mediaconnect-2.5.2.post2/types_aiobotocore_mediaconnect/literals.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)    11972 2023-08-04 13:43:59.000000 types-aiobotocore-mediaconnect-2.5.2.post2/types_aiobotocore_mediaconnect/literals.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)     8625 2023-08-04 13:43:58.000000 types-aiobotocore-mediaconnect-2.5.2.post2/types_aiobotocore_mediaconnect/paginator.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)     8616 2023-08-04 13:43:58.000000 types-aiobotocore-mediaconnect-2.5.2.post2/types_aiobotocore_mediaconnect/paginator.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:43:58.000000 types-aiobotocore-mediaconnect-2.5.2.post2/types_aiobotocore_mediaconnect/py.typed
--rw-r--r--   0 vlad      (1000) vlad      (1000)    64964 2023-08-04 13:44:01.000000 types-aiobotocore-mediaconnect-2.5.2.post2/types_aiobotocore_mediaconnect/type_defs.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)    64873 2023-08-04 13:44:01.000000 types-aiobotocore-mediaconnect-2.5.2.post2/types_aiobotocore_mediaconnect/type_defs.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)       65 2023-08-04 13:43:58.000000 types-aiobotocore-mediaconnect-2.5.2.post2/types_aiobotocore_mediaconnect/version.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)     3403 2023-08-04 13:43:58.000000 types-aiobotocore-mediaconnect-2.5.2.post2/types_aiobotocore_mediaconnect/waiter.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)     3400 2023-08-04 13:43:58.000000 types-aiobotocore-mediaconnect-2.5.2.post2/types_aiobotocore_mediaconnect/waiter.pyi
-drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:17.326643 types-aiobotocore-mediaconnect-2.5.2.post2/types_aiobotocore_mediaconnect.egg-info/
--rw-r--r--   0 vlad      (1000) vlad      (1000)    14917 2023-08-04 13:59:17.000000 types-aiobotocore-mediaconnect-2.5.2.post2/types_aiobotocore_mediaconnect.egg-info/PKG-INFO
--rw-r--r--   0 vlad      (1000) vlad      (1000)      991 2023-08-04 13:59:17.000000 types-aiobotocore-mediaconnect-2.5.2.post2/types_aiobotocore_mediaconnect.egg-info/SOURCES.txt
--rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:17.000000 types-aiobotocore-mediaconnect-2.5.2.post2/types_aiobotocore_mediaconnect.egg-info/dependency_links.txt
--rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:17.000000 types-aiobotocore-mediaconnect-2.5.2.post2/types_aiobotocore_mediaconnect.egg-info/not-zip-safe
--rw-r--r--   0 vlad      (1000) vlad      (1000)       52 2023-08-04 13:59:17.000000 types-aiobotocore-mediaconnect-2.5.2.post2/types_aiobotocore_mediaconnect.egg-info/requires.txt
--rw-r--r--   0 vlad      (1000) vlad      (1000)       31 2023-08-04 13:59:17.000000 types-aiobotocore-mediaconnect-2.5.2.post2/types_aiobotocore_mediaconnect.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:24:04.370730 types-aiobotocore-mediaconnect-2.5.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-08 01:14:50.000000 types-aiobotocore-mediaconnect-2.5.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    14911 2023-08-08 01:24:04.366730 types-aiobotocore-mediaconnect-2.5.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    13379 2023-08-08 01:14:50.000000 types-aiobotocore-mediaconnect-2.5.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-08 01:24:04.370730 types-aiobotocore-mediaconnect-2.5.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2101 2023-08-08 01:14:50.000000 types-aiobotocore-mediaconnect-2.5.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:24:04.366730 types-aiobotocore-mediaconnect-2.5.4/types_aiobotocore_mediaconnect/
+-rw-r--r--   0 runner    (1001) docker     (123)     2311 2023-08-08 01:14:50.000000 types-aiobotocore-mediaconnect-2.5.4/types_aiobotocore_mediaconnect/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2310 2023-08-08 01:14:50.000000 types-aiobotocore-mediaconnect-2.5.4/types_aiobotocore_mediaconnect/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      951 2023-08-08 01:14:50.000000 types-aiobotocore-mediaconnect-2.5.4/types_aiobotocore_mediaconnect/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42802 2023-08-08 01:14:50.000000 types-aiobotocore-mediaconnect-2.5.4/types_aiobotocore_mediaconnect/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42733 2023-08-08 01:14:50.000000 types-aiobotocore-mediaconnect-2.5.4/types_aiobotocore_mediaconnect/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    11974 2023-08-08 01:14:51.000000 types-aiobotocore-mediaconnect-2.5.4/types_aiobotocore_mediaconnect/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11972 2023-08-08 01:14:51.000000 types-aiobotocore-mediaconnect-2.5.4/types_aiobotocore_mediaconnect/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8625 2023-08-08 01:14:51.000000 types-aiobotocore-mediaconnect-2.5.4/types_aiobotocore_mediaconnect/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8616 2023-08-08 01:14:50.000000 types-aiobotocore-mediaconnect-2.5.4/types_aiobotocore_mediaconnect/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 01:14:50.000000 types-aiobotocore-mediaconnect-2.5.4/types_aiobotocore_mediaconnect/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    64964 2023-08-08 01:14:54.000000 types-aiobotocore-mediaconnect-2.5.4/types_aiobotocore_mediaconnect/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    64873 2023-08-08 01:14:51.000000 types-aiobotocore-mediaconnect-2.5.4/types_aiobotocore_mediaconnect/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-08-08 01:14:50.000000 types-aiobotocore-mediaconnect-2.5.4/types_aiobotocore_mediaconnect/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3403 2023-08-08 01:14:51.000000 types-aiobotocore-mediaconnect-2.5.4/types_aiobotocore_mediaconnect/waiter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3400 2023-08-08 01:14:51.000000 types-aiobotocore-mediaconnect-2.5.4/types_aiobotocore_mediaconnect/waiter.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:24:04.366730 types-aiobotocore-mediaconnect-2.5.4/types_aiobotocore_mediaconnect.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    14911 2023-08-08 01:24:04.000000 types-aiobotocore-mediaconnect-2.5.4/types_aiobotocore_mediaconnect.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      991 2023-08-08 01:24:04.000000 types-aiobotocore-mediaconnect-2.5.4/types_aiobotocore_mediaconnect.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 01:24:04.000000 types-aiobotocore-mediaconnect-2.5.4/types_aiobotocore_mediaconnect.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 01:24:04.000000 types-aiobotocore-mediaconnect-2.5.4/types_aiobotocore_mediaconnect.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-08 01:24:04.000000 types-aiobotocore-mediaconnect-2.5.4/types_aiobotocore_mediaconnect.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-08-08 01:24:04.000000 types-aiobotocore-mediaconnect-2.5.4/types_aiobotocore_mediaconnect.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-mediaconnect-2.5.2.post2/LICENSE` & `types-aiobotocore-mediaconnect-2.5.4/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-mediaconnect-2.5.2.post2/PKG-INFO` & `types-aiobotocore-mediaconnect-2.5.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-mediaconnect
-Version: 2.5.2.post2
-Summary: Type annotations for aiobotocore.MediaConnect 2.5.2 service generated with mypy-boto3-builder 7.17.2
+Version: 2.5.4
+Summary: Type annotations for aiobotocore.MediaConnect 2.5.4 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mediaconnect/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-mediaconnect.svg?color=blue)](https://pypi.org/project/types-aiobotocore-mediaconnect)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mediaconnect/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-mediaconnect)](https://pepy.tech/project/types-aiobotocore-mediaconnect)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.MediaConnect 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediaconnect.html#MediaConnect)
+[aiobotocore.MediaConnect 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediaconnect.html#MediaConnect)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-mediaconnect-2.5.2.post2/README.md` & `types-aiobotocore-mediaconnect-2.5.4/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-mediaconnect.svg?color=blue)](https://pypi.org/project/types-aiobotocore-mediaconnect)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mediaconnect/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-mediaconnect)](https://pepy.tech/project/types-aiobotocore-mediaconnect)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.MediaConnect 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediaconnect.html#MediaConnect)
+[aiobotocore.MediaConnect 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediaconnect.html#MediaConnect)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-mediaconnect-2.5.2.post2/setup.py` & `types-aiobotocore-mediaconnect-2.5.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-mediaconnect",
-    version="2.5.2.post2",
+    version="2.5.4",
     packages=["types_aiobotocore_mediaconnect"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.MediaConnect 2.5.2 service generated with"
+        "Type annotations for aiobotocore.MediaConnect 2.5.4 service generated with"
         " mypy-boto3-builder 7.17.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
```

### Comparing `types-aiobotocore-mediaconnect-2.5.2.post2/types_aiobotocore_mediaconnect/__init__.py` & `types-aiobotocore-mediaconnect-2.5.4/types_aiobotocore_mediaconnect/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-mediaconnect-2.5.2.post2/types_aiobotocore_mediaconnect/__init__.pyi` & `types-aiobotocore-mediaconnect-2.5.4/types_aiobotocore_mediaconnect/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-mediaconnect-2.5.2.post2/types_aiobotocore_mediaconnect/__main__.py` & `types-aiobotocore-mediaconnect-2.5.4/types_aiobotocore_mediaconnect/__main__.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.MediaConnect 2.5.2\nVersion:         2.5.2.post2\nBuilder"
+        "Type annotations for aiobotocore.MediaConnect 2.5.4\nVersion:         2.5.4\nBuilder"
         " version: 7.17.2\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mediaconnect//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediaconnect.html#MediaConnect\nOther"
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

### Comparing `types-aiobotocore-mediaconnect-2.5.2.post2/types_aiobotocore_mediaconnect/client.py` & `types-aiobotocore-mediaconnect-2.5.4/types_aiobotocore_mediaconnect/client.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-mediaconnect-2.5.2.post2/types_aiobotocore_mediaconnect/client.pyi` & `types-aiobotocore-mediaconnect-2.5.4/types_aiobotocore_mediaconnect/client.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-mediaconnect-2.5.2.post2/types_aiobotocore_mediaconnect/literals.py` & `types-aiobotocore-mediaconnect-2.5.4/types_aiobotocore_mediaconnect/literals.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-mediaconnect-2.5.2.post2/types_aiobotocore_mediaconnect/literals.pyi` & `types-aiobotocore-mediaconnect-2.5.4/types_aiobotocore_mediaconnect/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-mediaconnect-2.5.2.post2/types_aiobotocore_mediaconnect/paginator.py` & `types-aiobotocore-mediaconnect-2.5.4/types_aiobotocore_mediaconnect/paginator.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-mediaconnect-2.5.2.post2/types_aiobotocore_mediaconnect/paginator.pyi` & `types-aiobotocore-mediaconnect-2.5.4/types_aiobotocore_mediaconnect/paginator.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-mediaconnect-2.5.2.post2/types_aiobotocore_mediaconnect/type_defs.py` & `types-aiobotocore-mediaconnect-2.5.4/types_aiobotocore_mediaconnect/type_defs.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-mediaconnect-2.5.2.post2/types_aiobotocore_mediaconnect/type_defs.pyi` & `types-aiobotocore-mediaconnect-2.5.4/types_aiobotocore_mediaconnect/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-mediaconnect-2.5.2.post2/types_aiobotocore_mediaconnect/waiter.py` & `types-aiobotocore-mediaconnect-2.5.4/types_aiobotocore_mediaconnect/waiter.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-mediaconnect-2.5.2.post2/types_aiobotocore_mediaconnect/waiter.pyi` & `types-aiobotocore-mediaconnect-2.5.4/types_aiobotocore_mediaconnect/waiter.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-mediaconnect-2.5.2.post2/types_aiobotocore_mediaconnect.egg-info/PKG-INFO` & `types-aiobotocore-mediaconnect-2.5.4/types_aiobotocore_mediaconnect.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-mediaconnect
-Version: 2.5.2.post2
-Summary: Type annotations for aiobotocore.MediaConnect 2.5.2 service generated with mypy-boto3-builder 7.17.2
+Version: 2.5.4
+Summary: Type annotations for aiobotocore.MediaConnect 2.5.4 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mediaconnect/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-mediaconnect.svg?color=blue)](https://pypi.org/project/types-aiobotocore-mediaconnect)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mediaconnect/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-mediaconnect)](https://pepy.tech/project/types-aiobotocore-mediaconnect)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.MediaConnect 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediaconnect.html#MediaConnect)
+[aiobotocore.MediaConnect 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediaconnect.html#MediaConnect)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-mediaconnect-2.5.2.post2/types_aiobotocore_mediaconnect.egg-info/SOURCES.txt` & `types-aiobotocore-mediaconnect-2.5.4/types_aiobotocore_mediaconnect.egg-info/SOURCES.txt`

 * *Files identical despite different names*


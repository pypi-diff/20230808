# Comparing `tmp/types-aiobotocore-mediaconvert-2.5.2.post2.tar.gz` & `tmp/types-aiobotocore-mediaconvert-2.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-mediaconvert-2.5.2.post2.tar", last modified: Fri Aug  4 13:59:17 2023, max compression
+gzip compressed data, was "types-aiobotocore-mediaconvert-2.5.4.tar", last modified: Tue Aug  8 01:24:04 2023, max compression
```

## Comparing `types-aiobotocore-mediaconvert-2.5.2.post2.tar` & `types-aiobotocore-mediaconvert-2.5.4.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:17.286643 types-aiobotocore-mediaconvert-2.5.2.post2/
--rw-r--r--   0 vlad      (1000) vlad      (1000)     1070 2023-08-04 13:44:11.000000 types-aiobotocore-mediaconvert-2.5.2.post2/LICENSE
--rw-r--r--   0 vlad      (1000) vlad      (1000)    13737 2023-08-04 13:59:17.286643 types-aiobotocore-mediaconvert-2.5.2.post2/PKG-INFO
--rw-r--r--   0 vlad      (1000) vlad      (1000)    12199 2023-08-04 13:44:11.000000 types-aiobotocore-mediaconvert-2.5.2.post2/README.md
--rw-r--r--   0 vlad      (1000) vlad      (1000)       38 2023-08-04 13:59:17.286643 types-aiobotocore-mediaconvert-2.5.2.post2/setup.cfg
--rw-r--r--   0 vlad      (1000) vlad      (1000)     2107 2023-08-04 13:44:11.000000 types-aiobotocore-mediaconvert-2.5.2.post2/setup.py
-drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:17.286643 types-aiobotocore-mediaconvert-2.5.2.post2/types_aiobotocore_mediaconvert/
--rw-r--r--   0 vlad      (1000) vlad      (1000)     1425 2023-08-04 13:44:11.000000 types-aiobotocore-mediaconvert-2.5.2.post2/types_aiobotocore_mediaconvert/__init__.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)     1424 2023-08-04 13:44:11.000000 types-aiobotocore-mediaconvert-2.5.2.post2/types_aiobotocore_mediaconvert/__init__.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)      963 2023-08-04 13:44:11.000000 types-aiobotocore-mediaconvert-2.5.2.post2/types_aiobotocore_mediaconvert/__main__.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)    24276 2023-08-04 13:44:11.000000 types-aiobotocore-mediaconvert-2.5.2.post2/types_aiobotocore_mediaconvert/client.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)    24234 2023-08-04 13:44:11.000000 types-aiobotocore-mediaconvert-2.5.2.post2/types_aiobotocore_mediaconvert/client.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)    55626 2023-08-04 13:44:13.000000 types-aiobotocore-mediaconvert-2.5.2.post2/types_aiobotocore_mediaconvert/literals.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)    55624 2023-08-04 13:44:12.000000 types-aiobotocore-mediaconvert-2.5.2.post2/types_aiobotocore_mediaconvert/literals.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)     6982 2023-08-04 13:44:11.000000 types-aiobotocore-mediaconvert-2.5.2.post2/types_aiobotocore_mediaconvert/paginator.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)     6975 2023-08-04 13:44:11.000000 types-aiobotocore-mediaconvert-2.5.2.post2/types_aiobotocore_mediaconvert/paginator.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:44:11.000000 types-aiobotocore-mediaconvert-2.5.2.post2/types_aiobotocore_mediaconvert/py.typed
--rw-r--r--   0 vlad      (1000) vlad      (1000)   103337 2023-08-04 13:44:16.000000 types-aiobotocore-mediaconvert-2.5.2.post2/types_aiobotocore_mediaconvert/type_defs.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)   103312 2023-08-04 13:44:15.000000 types-aiobotocore-mediaconvert-2.5.2.post2/types_aiobotocore_mediaconvert/type_defs.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)       65 2023-08-04 13:44:11.000000 types-aiobotocore-mediaconvert-2.5.2.post2/types_aiobotocore_mediaconvert/version.py
-drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:17.286643 types-aiobotocore-mediaconvert-2.5.2.post2/types_aiobotocore_mediaconvert.egg-info/
--rw-r--r--   0 vlad      (1000) vlad      (1000)    13737 2023-08-04 13:59:17.000000 types-aiobotocore-mediaconvert-2.5.2.post2/types_aiobotocore_mediaconvert.egg-info/PKG-INFO
--rw-r--r--   0 vlad      (1000) vlad      (1000)      908 2023-08-04 13:59:17.000000 types-aiobotocore-mediaconvert-2.5.2.post2/types_aiobotocore_mediaconvert.egg-info/SOURCES.txt
--rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:17.000000 types-aiobotocore-mediaconvert-2.5.2.post2/types_aiobotocore_mediaconvert.egg-info/dependency_links.txt
--rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:17.000000 types-aiobotocore-mediaconvert-2.5.2.post2/types_aiobotocore_mediaconvert.egg-info/not-zip-safe
--rw-r--r--   0 vlad      (1000) vlad      (1000)       52 2023-08-04 13:59:17.000000 types-aiobotocore-mediaconvert-2.5.2.post2/types_aiobotocore_mediaconvert.egg-info/requires.txt
--rw-r--r--   0 vlad      (1000) vlad      (1000)       31 2023-08-04 13:59:17.000000 types-aiobotocore-mediaconvert-2.5.2.post2/types_aiobotocore_mediaconvert.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:24:04.490730 types-aiobotocore-mediaconvert-2.5.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-08 01:14:59.000000 types-aiobotocore-mediaconvert-2.5.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    13731 2023-08-08 01:24:04.482730 types-aiobotocore-mediaconvert-2.5.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    12199 2023-08-08 01:14:59.000000 types-aiobotocore-mediaconvert-2.5.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-08 01:24:04.490730 types-aiobotocore-mediaconvert-2.5.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2101 2023-08-08 01:14:59.000000 types-aiobotocore-mediaconvert-2.5.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:24:04.482730 types-aiobotocore-mediaconvert-2.5.4/types_aiobotocore_mediaconvert/
+-rw-r--r--   0 runner    (1001) docker     (123)     1425 2023-08-08 01:14:59.000000 types-aiobotocore-mediaconvert-2.5.4/types_aiobotocore_mediaconvert/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1424 2023-08-08 01:14:59.000000 types-aiobotocore-mediaconvert-2.5.4/types_aiobotocore_mediaconvert/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      951 2023-08-08 01:14:59.000000 types-aiobotocore-mediaconvert-2.5.4/types_aiobotocore_mediaconvert/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24276 2023-08-08 01:15:01.000000 types-aiobotocore-mediaconvert-2.5.4/types_aiobotocore_mediaconvert/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24234 2023-08-08 01:14:59.000000 types-aiobotocore-mediaconvert-2.5.4/types_aiobotocore_mediaconvert/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    55626 2023-08-08 01:15:02.000000 types-aiobotocore-mediaconvert-2.5.4/types_aiobotocore_mediaconvert/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    55624 2023-08-08 01:15:01.000000 types-aiobotocore-mediaconvert-2.5.4/types_aiobotocore_mediaconvert/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     6982 2023-08-08 01:15:01.000000 types-aiobotocore-mediaconvert-2.5.4/types_aiobotocore_mediaconvert/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6975 2023-08-08 01:15:01.000000 types-aiobotocore-mediaconvert-2.5.4/types_aiobotocore_mediaconvert/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 01:14:59.000000 types-aiobotocore-mediaconvert-2.5.4/types_aiobotocore_mediaconvert/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)   103337 2023-08-08 01:15:04.000000 types-aiobotocore-mediaconvert-2.5.4/types_aiobotocore_mediaconvert/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)   103312 2023-08-08 01:15:03.000000 types-aiobotocore-mediaconvert-2.5.4/types_aiobotocore_mediaconvert/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-08-08 01:14:59.000000 types-aiobotocore-mediaconvert-2.5.4/types_aiobotocore_mediaconvert/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:24:04.482730 types-aiobotocore-mediaconvert-2.5.4/types_aiobotocore_mediaconvert.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    13731 2023-08-08 01:24:04.000000 types-aiobotocore-mediaconvert-2.5.4/types_aiobotocore_mediaconvert.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      908 2023-08-08 01:24:04.000000 types-aiobotocore-mediaconvert-2.5.4/types_aiobotocore_mediaconvert.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 01:24:04.000000 types-aiobotocore-mediaconvert-2.5.4/types_aiobotocore_mediaconvert.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 01:24:04.000000 types-aiobotocore-mediaconvert-2.5.4/types_aiobotocore_mediaconvert.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-08 01:24:04.000000 types-aiobotocore-mediaconvert-2.5.4/types_aiobotocore_mediaconvert.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-08-08 01:24:04.000000 types-aiobotocore-mediaconvert-2.5.4/types_aiobotocore_mediaconvert.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-mediaconvert-2.5.2.post2/LICENSE` & `types-aiobotocore-mediaconvert-2.5.4/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-mediaconvert-2.5.2.post2/PKG-INFO` & `types-aiobotocore-mediaconvert-2.5.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-mediaconvert
-Version: 2.5.2.post2
-Summary: Type annotations for aiobotocore.MediaConvert 2.5.2 service generated with mypy-boto3-builder 7.17.2
+Version: 2.5.4
+Summary: Type annotations for aiobotocore.MediaConvert 2.5.4 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mediaconvert/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-mediaconvert.svg?color=blue)](https://pypi.org/project/types-aiobotocore-mediaconvert)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mediaconvert/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-mediaconvert)](https://pepy.tech/project/types-aiobotocore-mediaconvert)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.MediaConvert 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediaconvert.html#MediaConvert)
+[aiobotocore.MediaConvert 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediaconvert.html#MediaConvert)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-mediaconvert-2.5.2.post2/README.md` & `types-aiobotocore-mediaconvert-2.5.4/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-mediaconvert.svg?color=blue)](https://pypi.org/project/types-aiobotocore-mediaconvert)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mediaconvert/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-mediaconvert)](https://pepy.tech/project/types-aiobotocore-mediaconvert)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.MediaConvert 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediaconvert.html#MediaConvert)
+[aiobotocore.MediaConvert 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediaconvert.html#MediaConvert)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-mediaconvert-2.5.2.post2/setup.py` & `types-aiobotocore-mediaconvert-2.5.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-mediaconvert",
-    version="2.5.2.post2",
+    version="2.5.4",
     packages=["types_aiobotocore_mediaconvert"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.MediaConvert 2.5.2 service generated with"
+        "Type annotations for aiobotocore.MediaConvert 2.5.4 service generated with"
         " mypy-boto3-builder 7.17.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
```

### Comparing `types-aiobotocore-mediaconvert-2.5.2.post2/types_aiobotocore_mediaconvert/__init__.py` & `types-aiobotocore-mediaconvert-2.5.4/types_aiobotocore_mediaconvert/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-mediaconvert-2.5.2.post2/types_aiobotocore_mediaconvert/__init__.pyi` & `types-aiobotocore-mediaconvert-2.5.4/types_aiobotocore_mediaconvert/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-mediaconvert-2.5.2.post2/types_aiobotocore_mediaconvert/__main__.py` & `types-aiobotocore-mediaconvert-2.5.4/types_aiobotocore_mediaconvert/__main__.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.MediaConvert 2.5.2\nVersion:         2.5.2.post2\nBuilder"
+        "Type annotations for aiobotocore.MediaConvert 2.5.4\nVersion:         2.5.4\nBuilder"
         " version: 7.17.2\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mediaconvert//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediaconvert.html#MediaConvert\nOther"
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

### Comparing `types-aiobotocore-mediaconvert-2.5.2.post2/types_aiobotocore_mediaconvert/client.py` & `types-aiobotocore-mediaconvert-2.5.4/types_aiobotocore_mediaconvert/client.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-mediaconvert-2.5.2.post2/types_aiobotocore_mediaconvert/client.pyi` & `types-aiobotocore-mediaconvert-2.5.4/types_aiobotocore_mediaconvert/client.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-mediaconvert-2.5.2.post2/types_aiobotocore_mediaconvert/literals.py` & `types-aiobotocore-mediaconvert-2.5.4/types_aiobotocore_mediaconvert/literals.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-mediaconvert-2.5.2.post2/types_aiobotocore_mediaconvert/literals.pyi` & `types-aiobotocore-mediaconvert-2.5.4/types_aiobotocore_mediaconvert/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-mediaconvert-2.5.2.post2/types_aiobotocore_mediaconvert/paginator.py` & `types-aiobotocore-mediaconvert-2.5.4/types_aiobotocore_mediaconvert/paginator.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-mediaconvert-2.5.2.post2/types_aiobotocore_mediaconvert/paginator.pyi` & `types-aiobotocore-mediaconvert-2.5.4/types_aiobotocore_mediaconvert/paginator.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-mediaconvert-2.5.2.post2/types_aiobotocore_mediaconvert/type_defs.py` & `types-aiobotocore-mediaconvert-2.5.4/types_aiobotocore_mediaconvert/type_defs.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-mediaconvert-2.5.2.post2/types_aiobotocore_mediaconvert/type_defs.pyi` & `types-aiobotocore-mediaconvert-2.5.4/types_aiobotocore_mediaconvert/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-mediaconvert-2.5.2.post2/types_aiobotocore_mediaconvert.egg-info/PKG-INFO` & `types-aiobotocore-mediaconvert-2.5.4/types_aiobotocore_mediaconvert.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-mediaconvert
-Version: 2.5.2.post2
-Summary: Type annotations for aiobotocore.MediaConvert 2.5.2 service generated with mypy-boto3-builder 7.17.2
+Version: 2.5.4
+Summary: Type annotations for aiobotocore.MediaConvert 2.5.4 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mediaconvert/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-mediaconvert.svg?color=blue)](https://pypi.org/project/types-aiobotocore-mediaconvert)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mediaconvert/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-mediaconvert)](https://pepy.tech/project/types-aiobotocore-mediaconvert)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.MediaConvert 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediaconvert.html#MediaConvert)
+[aiobotocore.MediaConvert 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediaconvert.html#MediaConvert)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-mediaconvert-2.5.2.post2/types_aiobotocore_mediaconvert.egg-info/SOURCES.txt` & `types-aiobotocore-mediaconvert-2.5.4/types_aiobotocore_mediaconvert.egg-info/SOURCES.txt`

 * *Files identical despite different names*


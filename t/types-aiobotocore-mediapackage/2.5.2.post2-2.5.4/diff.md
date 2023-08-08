# Comparing `tmp/types-aiobotocore-mediapackage-2.5.2.post2.tar.gz` & `tmp/types-aiobotocore-mediapackage-2.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-mediapackage-2.5.2.post2.tar", last modified: Fri Aug  4 13:59:17 2023, max compression
+gzip compressed data, was "types-aiobotocore-mediapackage-2.5.4.tar", last modified: Tue Aug  8 01:24:04 2023, max compression
```

## Comparing `types-aiobotocore-mediapackage-2.5.2.post2.tar` & `types-aiobotocore-mediapackage-2.5.4.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:17.376643 types-aiobotocore-mediapackage-2.5.2.post2/
--rw-r--r--   0 vlad      (1000) vlad      (1000)     1070 2023-08-04 13:44:31.000000 types-aiobotocore-mediapackage-2.5.2.post2/LICENSE
--rw-r--r--   0 vlad      (1000) vlad      (1000)    13491 2023-08-04 13:59:17.376643 types-aiobotocore-mediapackage-2.5.2.post2/PKG-INFO
--rw-r--r--   0 vlad      (1000) vlad      (1000)    11953 2023-08-04 13:44:31.000000 types-aiobotocore-mediapackage-2.5.2.post2/README.md
--rw-r--r--   0 vlad      (1000) vlad      (1000)       38 2023-08-04 13:59:17.376643 types-aiobotocore-mediapackage-2.5.2.post2/setup.cfg
--rw-r--r--   0 vlad      (1000) vlad      (1000)     2107 2023-08-04 13:44:31.000000 types-aiobotocore-mediapackage-2.5.2.post2/setup.py
-drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:17.376643 types-aiobotocore-mediapackage-2.5.2.post2/types_aiobotocore_mediapackage/
--rw-r--r--   0 vlad      (1000) vlad      (1000)     1102 2023-08-04 13:44:31.000000 types-aiobotocore-mediapackage-2.5.2.post2/types_aiobotocore_mediapackage/__init__.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)     1101 2023-08-04 13:44:31.000000 types-aiobotocore-mediapackage-2.5.2.post2/types_aiobotocore_mediapackage/__init__.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)      963 2023-08-04 13:44:31.000000 types-aiobotocore-mediapackage-2.5.2.post2/types_aiobotocore_mediapackage/__main__.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)    18424 2023-08-04 13:44:31.000000 types-aiobotocore-mediapackage-2.5.2.post2/types_aiobotocore_mediapackage/client.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)    18393 2023-08-04 13:44:31.000000 types-aiobotocore-mediapackage-2.5.2.post2/types_aiobotocore_mediapackage/client.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)    10349 2023-08-04 13:44:31.000000 types-aiobotocore-mediapackage-2.5.2.post2/types_aiobotocore_mediapackage/literals.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)    10347 2023-08-04 13:44:31.000000 types-aiobotocore-mediapackage-2.5.2.post2/types_aiobotocore_mediapackage/literals.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)     4385 2023-08-04 13:44:31.000000 types-aiobotocore-mediapackage-2.5.2.post2/types_aiobotocore_mediapackage/paginator.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)     4380 2023-08-04 13:44:31.000000 types-aiobotocore-mediapackage-2.5.2.post2/types_aiobotocore_mediapackage/paginator.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:44:31.000000 types-aiobotocore-mediapackage-2.5.2.post2/types_aiobotocore_mediapackage/py.typed
--rw-r--r--   0 vlad      (1000) vlad      (1000)    25745 2023-08-04 13:44:32.000000 types-aiobotocore-mediapackage-2.5.2.post2/types_aiobotocore_mediapackage/type_defs.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)    25722 2023-08-04 13:44:32.000000 types-aiobotocore-mediapackage-2.5.2.post2/types_aiobotocore_mediapackage/type_defs.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)       65 2023-08-04 13:44:31.000000 types-aiobotocore-mediapackage-2.5.2.post2/types_aiobotocore_mediapackage/version.py
-drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:17.376643 types-aiobotocore-mediapackage-2.5.2.post2/types_aiobotocore_mediapackage.egg-info/
--rw-r--r--   0 vlad      (1000) vlad      (1000)    13491 2023-08-04 13:59:17.000000 types-aiobotocore-mediapackage-2.5.2.post2/types_aiobotocore_mediapackage.egg-info/PKG-INFO
--rw-r--r--   0 vlad      (1000) vlad      (1000)      908 2023-08-04 13:59:17.000000 types-aiobotocore-mediapackage-2.5.2.post2/types_aiobotocore_mediapackage.egg-info/SOURCES.txt
--rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:17.000000 types-aiobotocore-mediapackage-2.5.2.post2/types_aiobotocore_mediapackage.egg-info/dependency_links.txt
--rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:17.000000 types-aiobotocore-mediapackage-2.5.2.post2/types_aiobotocore_mediapackage.egg-info/not-zip-safe
--rw-r--r--   0 vlad      (1000) vlad      (1000)       52 2023-08-04 13:59:17.000000 types-aiobotocore-mediapackage-2.5.2.post2/types_aiobotocore_mediapackage.egg-info/requires.txt
--rw-r--r--   0 vlad      (1000) vlad      (1000)       31 2023-08-04 13:59:17.000000 types-aiobotocore-mediapackage-2.5.2.post2/types_aiobotocore_mediapackage.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:24:04.854731 types-aiobotocore-mediapackage-2.5.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-08 01:15:14.000000 types-aiobotocore-mediapackage-2.5.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    13485 2023-08-08 01:24:04.854731 types-aiobotocore-mediapackage-2.5.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    11953 2023-08-08 01:15:14.000000 types-aiobotocore-mediapackage-2.5.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-08 01:24:04.854731 types-aiobotocore-mediapackage-2.5.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2101 2023-08-08 01:15:14.000000 types-aiobotocore-mediapackage-2.5.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:24:04.830731 types-aiobotocore-mediapackage-2.5.4/types_aiobotocore_mediapackage/
+-rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-08-08 01:15:14.000000 types-aiobotocore-mediapackage-2.5.4/types_aiobotocore_mediapackage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1101 2023-08-08 01:15:14.000000 types-aiobotocore-mediapackage-2.5.4/types_aiobotocore_mediapackage/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      951 2023-08-08 01:15:14.000000 types-aiobotocore-mediapackage-2.5.4/types_aiobotocore_mediapackage/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18424 2023-08-08 01:15:14.000000 types-aiobotocore-mediapackage-2.5.4/types_aiobotocore_mediapackage/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18393 2023-08-08 01:15:14.000000 types-aiobotocore-mediapackage-2.5.4/types_aiobotocore_mediapackage/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    10349 2023-08-08 01:15:14.000000 types-aiobotocore-mediapackage-2.5.4/types_aiobotocore_mediapackage/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10347 2023-08-08 01:15:14.000000 types-aiobotocore-mediapackage-2.5.4/types_aiobotocore_mediapackage/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     4385 2023-08-08 01:15:14.000000 types-aiobotocore-mediapackage-2.5.4/types_aiobotocore_mediapackage/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4380 2023-08-08 01:15:14.000000 types-aiobotocore-mediapackage-2.5.4/types_aiobotocore_mediapackage/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 01:15:14.000000 types-aiobotocore-mediapackage-2.5.4/types_aiobotocore_mediapackage/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    25745 2023-08-08 01:15:15.000000 types-aiobotocore-mediapackage-2.5.4/types_aiobotocore_mediapackage/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25722 2023-08-08 01:15:15.000000 types-aiobotocore-mediapackage-2.5.4/types_aiobotocore_mediapackage/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-08-08 01:15:14.000000 types-aiobotocore-mediapackage-2.5.4/types_aiobotocore_mediapackage/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:24:04.830731 types-aiobotocore-mediapackage-2.5.4/types_aiobotocore_mediapackage.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    13485 2023-08-08 01:24:04.000000 types-aiobotocore-mediapackage-2.5.4/types_aiobotocore_mediapackage.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      908 2023-08-08 01:24:04.000000 types-aiobotocore-mediapackage-2.5.4/types_aiobotocore_mediapackage.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 01:24:04.000000 types-aiobotocore-mediapackage-2.5.4/types_aiobotocore_mediapackage.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 01:24:04.000000 types-aiobotocore-mediapackage-2.5.4/types_aiobotocore_mediapackage.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-08 01:24:04.000000 types-aiobotocore-mediapackage-2.5.4/types_aiobotocore_mediapackage.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-08-08 01:24:04.000000 types-aiobotocore-mediapackage-2.5.4/types_aiobotocore_mediapackage.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-mediapackage-2.5.2.post2/LICENSE` & `types-aiobotocore-mediapackage-2.5.4/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-mediapackage-2.5.2.post2/PKG-INFO` & `types-aiobotocore-mediapackage-2.5.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-mediapackage
-Version: 2.5.2.post2
-Summary: Type annotations for aiobotocore.MediaPackage 2.5.2 service generated with mypy-boto3-builder 7.17.2
+Version: 2.5.4
+Summary: Type annotations for aiobotocore.MediaPackage 2.5.4 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mediapackage/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-mediapackage.svg?color=blue)](https://pypi.org/project/types-aiobotocore-mediapackage)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mediapackage/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-mediapackage)](https://pepy.tech/project/types-aiobotocore-mediapackage)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.MediaPackage 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediapackage.html#MediaPackage)
+[aiobotocore.MediaPackage 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediapackage.html#MediaPackage)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-mediapackage-2.5.2.post2/README.md` & `types-aiobotocore-mediapackage-2.5.4/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-mediapackage.svg?color=blue)](https://pypi.org/project/types-aiobotocore-mediapackage)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mediapackage/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-mediapackage)](https://pepy.tech/project/types-aiobotocore-mediapackage)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.MediaPackage 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediapackage.html#MediaPackage)
+[aiobotocore.MediaPackage 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediapackage.html#MediaPackage)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-mediapackage-2.5.2.post2/setup.py` & `types-aiobotocore-mediapackage-2.5.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-mediapackage",
-    version="2.5.2.post2",
+    version="2.5.4",
     packages=["types_aiobotocore_mediapackage"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.MediaPackage 2.5.2 service generated with"
+        "Type annotations for aiobotocore.MediaPackage 2.5.4 service generated with"
         " mypy-boto3-builder 7.17.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
```

### Comparing `types-aiobotocore-mediapackage-2.5.2.post2/types_aiobotocore_mediapackage/__init__.py` & `types-aiobotocore-mediapackage-2.5.4/types_aiobotocore_mediapackage/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-mediapackage-2.5.2.post2/types_aiobotocore_mediapackage/__init__.pyi` & `types-aiobotocore-mediapackage-2.5.4/types_aiobotocore_mediapackage/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-mediapackage-2.5.2.post2/types_aiobotocore_mediapackage/__main__.py` & `types-aiobotocore-mediapackage-2.5.4/types_aiobotocore_mediapackage/__main__.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.MediaPackage 2.5.2\nVersion:         2.5.2.post2\nBuilder"
+        "Type annotations for aiobotocore.MediaPackage 2.5.4\nVersion:         2.5.4\nBuilder"
         " version: 7.17.2\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mediapackage//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediapackage.html#MediaPackage\nOther"
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

### Comparing `types-aiobotocore-mediapackage-2.5.2.post2/types_aiobotocore_mediapackage/client.py` & `types-aiobotocore-mediapackage-2.5.4/types_aiobotocore_mediapackage/client.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-mediapackage-2.5.2.post2/types_aiobotocore_mediapackage/client.pyi` & `types-aiobotocore-mediapackage-2.5.4/types_aiobotocore_mediapackage/client.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-mediapackage-2.5.2.post2/types_aiobotocore_mediapackage/literals.py` & `types-aiobotocore-mediapackage-2.5.4/types_aiobotocore_mediapackage/literals.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-mediapackage-2.5.2.post2/types_aiobotocore_mediapackage/literals.pyi` & `types-aiobotocore-mediapackage-2.5.4/types_aiobotocore_mediapackage/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-mediapackage-2.5.2.post2/types_aiobotocore_mediapackage/paginator.py` & `types-aiobotocore-mediapackage-2.5.4/types_aiobotocore_mediapackage/paginator.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-mediapackage-2.5.2.post2/types_aiobotocore_mediapackage/paginator.pyi` & `types-aiobotocore-mediapackage-2.5.4/types_aiobotocore_mediapackage/paginator.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-mediapackage-2.5.2.post2/types_aiobotocore_mediapackage/type_defs.py` & `types-aiobotocore-mediapackage-2.5.4/types_aiobotocore_mediapackage/type_defs.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-mediapackage-2.5.2.post2/types_aiobotocore_mediapackage/type_defs.pyi` & `types-aiobotocore-mediapackage-2.5.4/types_aiobotocore_mediapackage/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-mediapackage-2.5.2.post2/types_aiobotocore_mediapackage.egg-info/PKG-INFO` & `types-aiobotocore-mediapackage-2.5.4/types_aiobotocore_mediapackage.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-mediapackage
-Version: 2.5.2.post2
-Summary: Type annotations for aiobotocore.MediaPackage 2.5.2 service generated with mypy-boto3-builder 7.17.2
+Version: 2.5.4
+Summary: Type annotations for aiobotocore.MediaPackage 2.5.4 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mediapackage/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-mediapackage.svg?color=blue)](https://pypi.org/project/types-aiobotocore-mediapackage)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mediapackage/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-mediapackage)](https://pepy.tech/project/types-aiobotocore-mediapackage)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.MediaPackage 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediapackage.html#MediaPackage)
+[aiobotocore.MediaPackage 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediapackage.html#MediaPackage)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-mediapackage-2.5.2.post2/types_aiobotocore_mediapackage.egg-info/SOURCES.txt` & `types-aiobotocore-mediapackage-2.5.4/types_aiobotocore_mediapackage.egg-info/SOURCES.txt`

 * *Files identical despite different names*


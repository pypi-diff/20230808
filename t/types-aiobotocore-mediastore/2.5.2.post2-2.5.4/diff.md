# Comparing `tmp/types-aiobotocore-mediastore-2.5.2.post2.tar.gz` & `tmp/types-aiobotocore-mediastore-2.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-mediastore-2.5.2.post2.tar", last modified: Fri Aug  4 13:59:18 2023, max compression
+gzip compressed data, was "types-aiobotocore-mediastore-2.5.4.tar", last modified: Tue Aug  8 01:24:06 2023, max compression
```

## Comparing `types-aiobotocore-mediastore-2.5.2.post2.tar` & `types-aiobotocore-mediastore-2.5.4.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:18.276643 types-aiobotocore-mediastore-2.5.2.post2/
--rw-r--r--   0 vlad      (1000) vlad      (1000)     1070 2023-08-04 13:44:39.000000 types-aiobotocore-mediastore-2.5.2.post2/LICENSE
--rw-r--r--   0 vlad      (1000) vlad      (1000)    13080 2023-08-04 13:59:18.276643 types-aiobotocore-mediastore-2.5.2.post2/PKG-INFO
--rw-r--r--   0 vlad      (1000) vlad      (1000)    11550 2023-08-04 13:44:39.000000 types-aiobotocore-mediastore-2.5.2.post2/README.md
--rw-r--r--   0 vlad      (1000) vlad      (1000)       38 2023-08-04 13:59:18.276643 types-aiobotocore-mediastore-2.5.2.post2/setup.cfg
--rw-r--r--   0 vlad      (1000) vlad      (1000)     2093 2023-08-04 13:44:39.000000 types-aiobotocore-mediastore-2.5.2.post2/setup.py
-drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:18.276643 types-aiobotocore-mediastore-2.5.2.post2/types_aiobotocore_mediastore/
--rw-r--r--   0 vlad      (1000) vlad      (1000)      671 2023-08-04 13:44:39.000000 types-aiobotocore-mediastore-2.5.2.post2/types_aiobotocore_mediastore/__init__.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)      670 2023-08-04 13:44:39.000000 types-aiobotocore-mediastore-2.5.2.post2/types_aiobotocore_mediastore/__init__.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)      955 2023-08-04 13:44:39.000000 types-aiobotocore-mediastore-2.5.2.post2/types_aiobotocore_mediastore/__main__.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)    16111 2023-08-04 13:44:39.000000 types-aiobotocore-mediastore-2.5.2.post2/types_aiobotocore_mediastore/client.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)    16080 2023-08-04 13:44:39.000000 types-aiobotocore-mediastore-2.5.2.post2/types_aiobotocore_mediastore/client.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)     8280 2023-08-04 13:44:39.000000 types-aiobotocore-mediastore-2.5.2.post2/types_aiobotocore_mediastore/literals.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)     8278 2023-08-04 13:44:39.000000 types-aiobotocore-mediastore-2.5.2.post2/types_aiobotocore_mediastore/literals.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)     2014 2023-08-04 13:44:39.000000 types-aiobotocore-mediastore-2.5.2.post2/types_aiobotocore_mediastore/paginator.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)     2011 2023-08-04 13:44:39.000000 types-aiobotocore-mediastore-2.5.2.post2/types_aiobotocore_mediastore/paginator.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:44:39.000000 types-aiobotocore-mediastore-2.5.2.post2/types_aiobotocore_mediastore/py.typed
--rw-r--r--   0 vlad      (1000) vlad      (1000)     9296 2023-08-04 13:44:39.000000 types-aiobotocore-mediastore-2.5.2.post2/types_aiobotocore_mediastore/type_defs.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)     9287 2023-08-04 13:44:39.000000 types-aiobotocore-mediastore-2.5.2.post2/types_aiobotocore_mediastore/type_defs.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)       65 2023-08-04 13:44:39.000000 types-aiobotocore-mediastore-2.5.2.post2/types_aiobotocore_mediastore/version.py
-drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:18.276643 types-aiobotocore-mediastore-2.5.2.post2/types_aiobotocore_mediastore.egg-info/
--rw-r--r--   0 vlad      (1000) vlad      (1000)    13080 2023-08-04 13:59:18.000000 types-aiobotocore-mediastore-2.5.2.post2/types_aiobotocore_mediastore.egg-info/PKG-INFO
--rw-r--r--   0 vlad      (1000) vlad      (1000)      870 2023-08-04 13:59:18.000000 types-aiobotocore-mediastore-2.5.2.post2/types_aiobotocore_mediastore.egg-info/SOURCES.txt
--rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:18.000000 types-aiobotocore-mediastore-2.5.2.post2/types_aiobotocore_mediastore.egg-info/dependency_links.txt
--rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:18.000000 types-aiobotocore-mediastore-2.5.2.post2/types_aiobotocore_mediastore.egg-info/not-zip-safe
--rw-r--r--   0 vlad      (1000) vlad      (1000)       52 2023-08-04 13:59:18.000000 types-aiobotocore-mediastore-2.5.2.post2/types_aiobotocore_mediastore.egg-info/requires.txt
--rw-r--r--   0 vlad      (1000) vlad      (1000)       29 2023-08-04 13:59:18.000000 types-aiobotocore-mediastore-2.5.2.post2/types_aiobotocore_mediastore.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:24:06.434735 types-aiobotocore-mediastore-2.5.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-08 01:15:19.000000 types-aiobotocore-mediastore-2.5.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    13074 2023-08-08 01:24:06.434735 types-aiobotocore-mediastore-2.5.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    11550 2023-08-08 01:15:19.000000 types-aiobotocore-mediastore-2.5.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-08 01:24:06.434735 types-aiobotocore-mediastore-2.5.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2087 2023-08-08 01:15:19.000000 types-aiobotocore-mediastore-2.5.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:24:06.434735 types-aiobotocore-mediastore-2.5.4/types_aiobotocore_mediastore/
+-rw-r--r--   0 runner    (1001) docker     (123)      671 2023-08-08 01:15:19.000000 types-aiobotocore-mediastore-2.5.4/types_aiobotocore_mediastore/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      670 2023-08-08 01:15:19.000000 types-aiobotocore-mediastore-2.5.4/types_aiobotocore_mediastore/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      943 2023-08-08 01:15:19.000000 types-aiobotocore-mediastore-2.5.4/types_aiobotocore_mediastore/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16111 2023-08-08 01:15:19.000000 types-aiobotocore-mediastore-2.5.4/types_aiobotocore_mediastore/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16080 2023-08-08 01:15:19.000000 types-aiobotocore-mediastore-2.5.4/types_aiobotocore_mediastore/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8280 2023-08-08 01:15:20.000000 types-aiobotocore-mediastore-2.5.4/types_aiobotocore_mediastore/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8278 2023-08-08 01:15:19.000000 types-aiobotocore-mediastore-2.5.4/types_aiobotocore_mediastore/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2014 2023-08-08 01:15:19.000000 types-aiobotocore-mediastore-2.5.4/types_aiobotocore_mediastore/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2011 2023-08-08 01:15:19.000000 types-aiobotocore-mediastore-2.5.4/types_aiobotocore_mediastore/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 01:15:19.000000 types-aiobotocore-mediastore-2.5.4/types_aiobotocore_mediastore/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     9296 2023-08-08 01:15:20.000000 types-aiobotocore-mediastore-2.5.4/types_aiobotocore_mediastore/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9287 2023-08-08 01:15:20.000000 types-aiobotocore-mediastore-2.5.4/types_aiobotocore_mediastore/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-08-08 01:15:19.000000 types-aiobotocore-mediastore-2.5.4/types_aiobotocore_mediastore/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:24:06.434735 types-aiobotocore-mediastore-2.5.4/types_aiobotocore_mediastore.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    13074 2023-08-08 01:24:06.000000 types-aiobotocore-mediastore-2.5.4/types_aiobotocore_mediastore.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      870 2023-08-08 01:24:06.000000 types-aiobotocore-mediastore-2.5.4/types_aiobotocore_mediastore.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 01:24:06.000000 types-aiobotocore-mediastore-2.5.4/types_aiobotocore_mediastore.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 01:24:06.000000 types-aiobotocore-mediastore-2.5.4/types_aiobotocore_mediastore.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-08 01:24:06.000000 types-aiobotocore-mediastore-2.5.4/types_aiobotocore_mediastore.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-08-08 01:24:06.000000 types-aiobotocore-mediastore-2.5.4/types_aiobotocore_mediastore.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-mediastore-2.5.2.post2/LICENSE` & `types-aiobotocore-mediastore-2.5.4/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-mediastore-2.5.2.post2/PKG-INFO` & `types-aiobotocore-mediastore-2.5.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-mediastore
-Version: 2.5.2.post2
-Summary: Type annotations for aiobotocore.MediaStore 2.5.2 service generated with mypy-boto3-builder 7.17.2
+Version: 2.5.4
+Summary: Type annotations for aiobotocore.MediaStore 2.5.4 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mediastore/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-mediastore.svg?color=blue)](https://pypi.org/project/types-aiobotocore-mediastore)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mediastore/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-mediastore)](https://pepy.tech/project/types-aiobotocore-mediastore)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.MediaStore 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediastore.html#MediaStore)
+[aiobotocore.MediaStore 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediastore.html#MediaStore)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-mediastore-2.5.2.post2/README.md` & `types-aiobotocore-mediastore-2.5.4/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-mediastore.svg?color=blue)](https://pypi.org/project/types-aiobotocore-mediastore)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mediastore/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-mediastore)](https://pepy.tech/project/types-aiobotocore-mediastore)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.MediaStore 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediastore.html#MediaStore)
+[aiobotocore.MediaStore 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediastore.html#MediaStore)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-mediastore-2.5.2.post2/setup.py` & `types-aiobotocore-mediastore-2.5.4/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-mediastore",
-    version="2.5.2.post2",
+    version="2.5.4",
     packages=["types_aiobotocore_mediastore"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.MediaStore 2.5.2 service generated with"
+        "Type annotations for aiobotocore.MediaStore 2.5.4 service generated with"
         " mypy-boto3-builder 7.17.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
```

### Comparing `types-aiobotocore-mediastore-2.5.2.post2/types_aiobotocore_mediastore/__init__.py` & `types-aiobotocore-mediastore-2.5.4/types_aiobotocore_mediastore/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-mediastore-2.5.2.post2/types_aiobotocore_mediastore/__init__.pyi` & `types-aiobotocore-mediastore-2.5.4/types_aiobotocore_mediastore/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-mediastore-2.5.2.post2/types_aiobotocore_mediastore/__main__.py` & `types-aiobotocore-mediastore-2.5.4/types_aiobotocore_mediastore/__main__.py`

 * *Files 13% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.MediaStore 2.5.2\nVersion:         2.5.2.post2\nBuilder"
+        "Type annotations for aiobotocore.MediaStore 2.5.4\nVersion:         2.5.4\nBuilder"
         " version: 7.17.2\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mediastore//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediastore.html#MediaStore\nOther"
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

### Comparing `types-aiobotocore-mediastore-2.5.2.post2/types_aiobotocore_mediastore/client.py` & `types-aiobotocore-mediastore-2.5.4/types_aiobotocore_mediastore/client.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-mediastore-2.5.2.post2/types_aiobotocore_mediastore/client.pyi` & `types-aiobotocore-mediastore-2.5.4/types_aiobotocore_mediastore/client.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-mediastore-2.5.2.post2/types_aiobotocore_mediastore/literals.py` & `types-aiobotocore-mediastore-2.5.4/types_aiobotocore_mediastore/literals.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-mediastore-2.5.2.post2/types_aiobotocore_mediastore/literals.pyi` & `types-aiobotocore-mediastore-2.5.4/types_aiobotocore_mediastore/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-mediastore-2.5.2.post2/types_aiobotocore_mediastore/paginator.py` & `types-aiobotocore-mediastore-2.5.4/types_aiobotocore_mediastore/paginator.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-mediastore-2.5.2.post2/types_aiobotocore_mediastore/paginator.pyi` & `types-aiobotocore-mediastore-2.5.4/types_aiobotocore_mediastore/paginator.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-mediastore-2.5.2.post2/types_aiobotocore_mediastore/type_defs.py` & `types-aiobotocore-mediastore-2.5.4/types_aiobotocore_mediastore/type_defs.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-mediastore-2.5.2.post2/types_aiobotocore_mediastore/type_defs.pyi` & `types-aiobotocore-mediastore-2.5.4/types_aiobotocore_mediastore/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-mediastore-2.5.2.post2/types_aiobotocore_mediastore.egg-info/PKG-INFO` & `types-aiobotocore-mediastore-2.5.4/types_aiobotocore_mediastore.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-mediastore
-Version: 2.5.2.post2
-Summary: Type annotations for aiobotocore.MediaStore 2.5.2 service generated with mypy-boto3-builder 7.17.2
+Version: 2.5.4
+Summary: Type annotations for aiobotocore.MediaStore 2.5.4 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mediastore/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-mediastore.svg?color=blue)](https://pypi.org/project/types-aiobotocore-mediastore)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mediastore/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-mediastore)](https://pepy.tech/project/types-aiobotocore-mediastore)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.MediaStore 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediastore.html#MediaStore)
+[aiobotocore.MediaStore 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediastore.html#MediaStore)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-mediastore-2.5.2.post2/types_aiobotocore_mediastore.egg-info/SOURCES.txt` & `types-aiobotocore-mediastore-2.5.4/types_aiobotocore_mediastore.egg-info/SOURCES.txt`

 * *Files identical despite different names*


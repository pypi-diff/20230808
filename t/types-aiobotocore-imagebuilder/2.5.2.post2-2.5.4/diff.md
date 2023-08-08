# Comparing `tmp/types-aiobotocore-imagebuilder-2.5.2.post2.tar.gz` & `tmp/types-aiobotocore-imagebuilder-2.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-imagebuilder-2.5.2.post2.tar", last modified: Fri Aug  4 13:59:11 2023, max compression
+gzip compressed data, was "types-aiobotocore-imagebuilder-2.5.4.tar", last modified: Tue Aug  8 01:23:49 2023, max compression
```

## Comparing `types-aiobotocore-imagebuilder-2.5.2.post2.tar` & `types-aiobotocore-imagebuilder-2.5.4.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:11.286642 types-aiobotocore-imagebuilder-2.5.2.post2/
--rw-r--r--   0 vlad      (1000) vlad      (1000)     1070 2023-08-04 13:40:12.000000 types-aiobotocore-imagebuilder-2.5.2.post2/LICENSE
--rw-r--r--   0 vlad      (1000) vlad      (1000)    12443 2023-08-04 13:59:11.286642 types-aiobotocore-imagebuilder-2.5.2.post2/PKG-INFO
--rw-r--r--   0 vlad      (1000) vlad      (1000)    10905 2023-08-04 13:40:12.000000 types-aiobotocore-imagebuilder-2.5.2.post2/README.md
--rw-r--r--   0 vlad      (1000) vlad      (1000)       38 2023-08-04 13:59:11.286642 types-aiobotocore-imagebuilder-2.5.2.post2/setup.cfg
--rw-r--r--   0 vlad      (1000) vlad      (1000)     2107 2023-08-04 13:40:12.000000 types-aiobotocore-imagebuilder-2.5.2.post2/setup.py
-drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:11.286642 types-aiobotocore-imagebuilder-2.5.2.post2/types_aiobotocore_imagebuilder/
--rw-r--r--   0 vlad      (1000) vlad      (1000)      482 2023-08-04 13:40:12.000000 types-aiobotocore-imagebuilder-2.5.2.post2/types_aiobotocore_imagebuilder/__init__.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)      481 2023-08-04 13:40:12.000000 types-aiobotocore-imagebuilder-2.5.2.post2/types_aiobotocore_imagebuilder/__init__.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)      963 2023-08-04 13:40:12.000000 types-aiobotocore-imagebuilder-2.5.2.post2/types_aiobotocore_imagebuilder/__main__.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)    44284 2023-08-04 13:40:13.000000 types-aiobotocore-imagebuilder-2.5.2.post2/types_aiobotocore_imagebuilder/client.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)    44219 2023-08-04 13:40:13.000000 types-aiobotocore-imagebuilder-2.5.2.post2/types_aiobotocore_imagebuilder/client.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)     9785 2023-08-04 13:40:13.000000 types-aiobotocore-imagebuilder-2.5.2.post2/types_aiobotocore_imagebuilder/literals.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)     9783 2023-08-04 13:40:13.000000 types-aiobotocore-imagebuilder-2.5.2.post2/types_aiobotocore_imagebuilder/literals.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:40:12.000000 types-aiobotocore-imagebuilder-2.5.2.post2/types_aiobotocore_imagebuilder/py.typed
--rw-r--r--   0 vlad      (1000) vlad      (1000)    66585 2023-08-04 13:40:15.000000 types-aiobotocore-imagebuilder-2.5.2.post2/types_aiobotocore_imagebuilder/type_defs.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)    66530 2023-08-04 13:40:14.000000 types-aiobotocore-imagebuilder-2.5.2.post2/types_aiobotocore_imagebuilder/type_defs.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)       65 2023-08-04 13:40:12.000000 types-aiobotocore-imagebuilder-2.5.2.post2/types_aiobotocore_imagebuilder/version.py
-drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:11.286642 types-aiobotocore-imagebuilder-2.5.2.post2/types_aiobotocore_imagebuilder.egg-info/
--rw-r--r--   0 vlad      (1000) vlad      (1000)    12443 2023-08-04 13:59:11.000000 types-aiobotocore-imagebuilder-2.5.2.post2/types_aiobotocore_imagebuilder.egg-info/PKG-INFO
--rw-r--r--   0 vlad      (1000) vlad      (1000)      819 2023-08-04 13:59:11.000000 types-aiobotocore-imagebuilder-2.5.2.post2/types_aiobotocore_imagebuilder.egg-info/SOURCES.txt
--rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:11.000000 types-aiobotocore-imagebuilder-2.5.2.post2/types_aiobotocore_imagebuilder.egg-info/dependency_links.txt
--rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:11.000000 types-aiobotocore-imagebuilder-2.5.2.post2/types_aiobotocore_imagebuilder.egg-info/not-zip-safe
--rw-r--r--   0 vlad      (1000) vlad      (1000)       52 2023-08-04 13:59:11.000000 types-aiobotocore-imagebuilder-2.5.2.post2/types_aiobotocore_imagebuilder.egg-info/requires.txt
--rw-r--r--   0 vlad      (1000) vlad      (1000)       31 2023-08-04 13:59:11.000000 types-aiobotocore-imagebuilder-2.5.2.post2/types_aiobotocore_imagebuilder.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:23:49.954733 types-aiobotocore-imagebuilder-2.5.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-08 01:12:25.000000 types-aiobotocore-imagebuilder-2.5.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    12437 2023-08-08 01:23:49.954733 types-aiobotocore-imagebuilder-2.5.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10905 2023-08-08 01:12:25.000000 types-aiobotocore-imagebuilder-2.5.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-08 01:23:49.954733 types-aiobotocore-imagebuilder-2.5.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2101 2023-08-08 01:12:25.000000 types-aiobotocore-imagebuilder-2.5.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:23:49.954733 types-aiobotocore-imagebuilder-2.5.4/types_aiobotocore_imagebuilder/
+-rw-r--r--   0 runner    (1001) docker     (123)      482 2023-08-08 01:12:25.000000 types-aiobotocore-imagebuilder-2.5.4/types_aiobotocore_imagebuilder/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      481 2023-08-08 01:12:25.000000 types-aiobotocore-imagebuilder-2.5.4/types_aiobotocore_imagebuilder/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      951 2023-08-08 01:12:25.000000 types-aiobotocore-imagebuilder-2.5.4/types_aiobotocore_imagebuilder/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    44284 2023-08-08 01:12:26.000000 types-aiobotocore-imagebuilder-2.5.4/types_aiobotocore_imagebuilder/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    44219 2023-08-08 01:12:25.000000 types-aiobotocore-imagebuilder-2.5.4/types_aiobotocore_imagebuilder/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9785 2023-08-08 01:12:26.000000 types-aiobotocore-imagebuilder-2.5.4/types_aiobotocore_imagebuilder/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9783 2023-08-08 01:12:26.000000 types-aiobotocore-imagebuilder-2.5.4/types_aiobotocore_imagebuilder/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 01:12:25.000000 types-aiobotocore-imagebuilder-2.5.4/types_aiobotocore_imagebuilder/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    66585 2023-08-08 01:12:27.000000 types-aiobotocore-imagebuilder-2.5.4/types_aiobotocore_imagebuilder/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    66530 2023-08-08 01:12:26.000000 types-aiobotocore-imagebuilder-2.5.4/types_aiobotocore_imagebuilder/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-08-08 01:12:25.000000 types-aiobotocore-imagebuilder-2.5.4/types_aiobotocore_imagebuilder/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:23:49.954733 types-aiobotocore-imagebuilder-2.5.4/types_aiobotocore_imagebuilder.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    12437 2023-08-08 01:23:49.000000 types-aiobotocore-imagebuilder-2.5.4/types_aiobotocore_imagebuilder.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      819 2023-08-08 01:23:49.000000 types-aiobotocore-imagebuilder-2.5.4/types_aiobotocore_imagebuilder.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 01:23:49.000000 types-aiobotocore-imagebuilder-2.5.4/types_aiobotocore_imagebuilder.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 01:23:49.000000 types-aiobotocore-imagebuilder-2.5.4/types_aiobotocore_imagebuilder.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-08 01:23:49.000000 types-aiobotocore-imagebuilder-2.5.4/types_aiobotocore_imagebuilder.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-08-08 01:23:49.000000 types-aiobotocore-imagebuilder-2.5.4/types_aiobotocore_imagebuilder.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-imagebuilder-2.5.2.post2/LICENSE` & `types-aiobotocore-imagebuilder-2.5.4/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-imagebuilder-2.5.2.post2/PKG-INFO` & `types-aiobotocore-imagebuilder-2.5.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-imagebuilder
-Version: 2.5.2.post2
-Summary: Type annotations for aiobotocore.imagebuilder 2.5.2 service generated with mypy-boto3-builder 7.17.2
+Version: 2.5.4
+Summary: Type annotations for aiobotocore.imagebuilder 2.5.4 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_imagebuilder/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-imagebuilder.svg?color=blue)](https://pypi.org/project/types-aiobotocore-imagebuilder)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_imagebuilder/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-imagebuilder)](https://pepy.tech/project/types-aiobotocore-imagebuilder)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.imagebuilder 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/imagebuilder.html#imagebuilder)
+[aiobotocore.imagebuilder 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/imagebuilder.html#imagebuilder)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-imagebuilder-2.5.2.post2/README.md` & `types-aiobotocore-imagebuilder-2.5.4/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-imagebuilder.svg?color=blue)](https://pypi.org/project/types-aiobotocore-imagebuilder)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_imagebuilder/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-imagebuilder)](https://pepy.tech/project/types-aiobotocore-imagebuilder)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.imagebuilder 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/imagebuilder.html#imagebuilder)
+[aiobotocore.imagebuilder 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/imagebuilder.html#imagebuilder)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-imagebuilder-2.5.2.post2/setup.py` & `types-aiobotocore-imagebuilder-2.5.4/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-imagebuilder",
-    version="2.5.2.post2",
+    version="2.5.4",
     packages=["types_aiobotocore_imagebuilder"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.imagebuilder 2.5.2 service generated with"
+        "Type annotations for aiobotocore.imagebuilder 2.5.4 service generated with"
         " mypy-boto3-builder 7.17.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
```

### Comparing `types-aiobotocore-imagebuilder-2.5.2.post2/types_aiobotocore_imagebuilder/client.py` & `types-aiobotocore-imagebuilder-2.5.4/types_aiobotocore_imagebuilder/client.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-imagebuilder-2.5.2.post2/types_aiobotocore_imagebuilder/client.pyi` & `types-aiobotocore-imagebuilder-2.5.4/types_aiobotocore_imagebuilder/client.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-imagebuilder-2.5.2.post2/types_aiobotocore_imagebuilder/literals.py` & `types-aiobotocore-imagebuilder-2.5.4/types_aiobotocore_imagebuilder/literals.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-imagebuilder-2.5.2.post2/types_aiobotocore_imagebuilder/literals.pyi` & `types-aiobotocore-imagebuilder-2.5.4/types_aiobotocore_imagebuilder/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-imagebuilder-2.5.2.post2/types_aiobotocore_imagebuilder/type_defs.py` & `types-aiobotocore-imagebuilder-2.5.4/types_aiobotocore_imagebuilder/type_defs.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-imagebuilder-2.5.2.post2/types_aiobotocore_imagebuilder/type_defs.pyi` & `types-aiobotocore-imagebuilder-2.5.4/types_aiobotocore_imagebuilder/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-imagebuilder-2.5.2.post2/types_aiobotocore_imagebuilder.egg-info/PKG-INFO` & `types-aiobotocore-imagebuilder-2.5.4/types_aiobotocore_imagebuilder.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-imagebuilder
-Version: 2.5.2.post2
-Summary: Type annotations for aiobotocore.imagebuilder 2.5.2 service generated with mypy-boto3-builder 7.17.2
+Version: 2.5.4
+Summary: Type annotations for aiobotocore.imagebuilder 2.5.4 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_imagebuilder/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-imagebuilder.svg?color=blue)](https://pypi.org/project/types-aiobotocore-imagebuilder)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_imagebuilder/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-imagebuilder)](https://pepy.tech/project/types-aiobotocore-imagebuilder)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.imagebuilder 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/imagebuilder.html#imagebuilder)
+[aiobotocore.imagebuilder 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/imagebuilder.html#imagebuilder)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-imagebuilder-2.5.2.post2/types_aiobotocore_imagebuilder.egg-info/SOURCES.txt` & `types-aiobotocore-imagebuilder-2.5.4/types_aiobotocore_imagebuilder.egg-info/SOURCES.txt`

 * *Files identical despite different names*


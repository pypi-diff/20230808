# Comparing `tmp/types-aiobotocore-worklink-2.5.2.post2.tar.gz` & `tmp/types-aiobotocore-worklink-2.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-worklink-2.5.2.post2.tar", last modified: Fri Aug  4 13:59:30 2023, max compression
+gzip compressed data, was "types-aiobotocore-worklink-2.5.4.tar", last modified: Tue Aug  8 01:24:36 2023, max compression
```

## Comparing `types-aiobotocore-worklink-2.5.2.post2.tar` & `types-aiobotocore-worklink-2.5.4.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:30.256643 types-aiobotocore-worklink-2.5.2.post2/
--rw-r--r--   0 vlad      (1000) vlad      (1000)     1070 2023-08-04 13:56:11.000000 types-aiobotocore-worklink-2.5.2.post2/LICENSE
--rw-r--r--   0 vlad      (1000) vlad      (1000)    12293 2023-08-04 13:59:30.256643 types-aiobotocore-worklink-2.5.2.post2/PKG-INFO
--rw-r--r--   0 vlad      (1000) vlad      (1000)    10771 2023-08-04 13:56:11.000000 types-aiobotocore-worklink-2.5.2.post2/README.md
--rw-r--r--   0 vlad      (1000) vlad      (1000)       38 2023-08-04 13:59:30.256643 types-aiobotocore-worklink-2.5.2.post2/setup.cfg
--rw-r--r--   0 vlad      (1000) vlad      (1000)     2079 2023-08-04 13:56:11.000000 types-aiobotocore-worklink-2.5.2.post2/setup.py
-drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:30.256643 types-aiobotocore-worklink-2.5.2.post2/types_aiobotocore_worklink/
--rw-r--r--   0 vlad      (1000) vlad      (1000)      450 2023-08-04 13:56:11.000000 types-aiobotocore-worklink-2.5.2.post2/types_aiobotocore_worklink/__init__.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)      449 2023-08-04 13:56:11.000000 types-aiobotocore-worklink-2.5.2.post2/types_aiobotocore_worklink/__init__.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)      947 2023-08-04 13:56:12.000000 types-aiobotocore-worklink-2.5.2.post2/types_aiobotocore_worklink/__main__.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)    23834 2023-08-04 13:56:12.000000 types-aiobotocore-worklink-2.5.2.post2/types_aiobotocore_worklink/client.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)    23792 2023-08-04 13:56:12.000000 types-aiobotocore-worklink-2.5.2.post2/types_aiobotocore_worklink/client.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)     8244 2023-08-04 13:56:12.000000 types-aiobotocore-worklink-2.5.2.post2/types_aiobotocore_worklink/literals.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)     8242 2023-08-04 13:56:12.000000 types-aiobotocore-worklink-2.5.2.post2/types_aiobotocore_worklink/literals.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:56:12.000000 types-aiobotocore-worklink-2.5.2.post2/types_aiobotocore_worklink/py.typed
--rw-r--r--   0 vlad      (1000) vlad      (1000)    21237 2023-08-04 13:56:12.000000 types-aiobotocore-worklink-2.5.2.post2/types_aiobotocore_worklink/type_defs.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)    21206 2023-08-04 13:56:12.000000 types-aiobotocore-worklink-2.5.2.post2/types_aiobotocore_worklink/type_defs.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)       65 2023-08-04 13:56:11.000000 types-aiobotocore-worklink-2.5.2.post2/types_aiobotocore_worklink/version.py
-drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:30.256643 types-aiobotocore-worklink-2.5.2.post2/types_aiobotocore_worklink.egg-info/
--rw-r--r--   0 vlad      (1000) vlad      (1000)    12293 2023-08-04 13:59:30.000000 types-aiobotocore-worklink-2.5.2.post2/types_aiobotocore_worklink.egg-info/PKG-INFO
--rw-r--r--   0 vlad      (1000) vlad      (1000)      751 2023-08-04 13:59:30.000000 types-aiobotocore-worklink-2.5.2.post2/types_aiobotocore_worklink.egg-info/SOURCES.txt
--rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:30.000000 types-aiobotocore-worklink-2.5.2.post2/types_aiobotocore_worklink.egg-info/dependency_links.txt
--rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:30.000000 types-aiobotocore-worklink-2.5.2.post2/types_aiobotocore_worklink.egg-info/not-zip-safe
--rw-r--r--   0 vlad      (1000) vlad      (1000)       52 2023-08-04 13:59:30.000000 types-aiobotocore-worklink-2.5.2.post2/types_aiobotocore_worklink.egg-info/requires.txt
--rw-r--r--   0 vlad      (1000) vlad      (1000)       27 2023-08-04 13:59:30.000000 types-aiobotocore-worklink-2.5.2.post2/types_aiobotocore_worklink.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:24:36.386805 types-aiobotocore-worklink-2.5.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-08 01:22:42.000000 types-aiobotocore-worklink-2.5.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    12287 2023-08-08 01:24:36.386805 types-aiobotocore-worklink-2.5.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10771 2023-08-08 01:22:42.000000 types-aiobotocore-worklink-2.5.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-08 01:24:36.386805 types-aiobotocore-worklink-2.5.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2073 2023-08-08 01:22:42.000000 types-aiobotocore-worklink-2.5.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:24:36.386805 types-aiobotocore-worklink-2.5.4/types_aiobotocore_worklink/
+-rw-r--r--   0 runner    (1001) docker     (123)      450 2023-08-08 01:22:42.000000 types-aiobotocore-worklink-2.5.4/types_aiobotocore_worklink/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      449 2023-08-08 01:22:42.000000 types-aiobotocore-worklink-2.5.4/types_aiobotocore_worklink/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      935 2023-08-08 01:22:42.000000 types-aiobotocore-worklink-2.5.4/types_aiobotocore_worklink/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23834 2023-08-08 01:22:42.000000 types-aiobotocore-worklink-2.5.4/types_aiobotocore_worklink/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23792 2023-08-08 01:22:42.000000 types-aiobotocore-worklink-2.5.4/types_aiobotocore_worklink/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8244 2023-08-08 01:22:42.000000 types-aiobotocore-worklink-2.5.4/types_aiobotocore_worklink/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8242 2023-08-08 01:22:42.000000 types-aiobotocore-worklink-2.5.4/types_aiobotocore_worklink/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 01:22:42.000000 types-aiobotocore-worklink-2.5.4/types_aiobotocore_worklink/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    21237 2023-08-08 01:22:42.000000 types-aiobotocore-worklink-2.5.4/types_aiobotocore_worklink/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21206 2023-08-08 01:22:42.000000 types-aiobotocore-worklink-2.5.4/types_aiobotocore_worklink/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-08-08 01:22:42.000000 types-aiobotocore-worklink-2.5.4/types_aiobotocore_worklink/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:24:36.386805 types-aiobotocore-worklink-2.5.4/types_aiobotocore_worklink.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    12287 2023-08-08 01:24:36.000000 types-aiobotocore-worklink-2.5.4/types_aiobotocore_worklink.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      751 2023-08-08 01:24:36.000000 types-aiobotocore-worklink-2.5.4/types_aiobotocore_worklink.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 01:24:36.000000 types-aiobotocore-worklink-2.5.4/types_aiobotocore_worklink.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 01:24:36.000000 types-aiobotocore-worklink-2.5.4/types_aiobotocore_worklink.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-08 01:24:36.000000 types-aiobotocore-worklink-2.5.4/types_aiobotocore_worklink.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-08-08 01:24:36.000000 types-aiobotocore-worklink-2.5.4/types_aiobotocore_worklink.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-worklink-2.5.2.post2/LICENSE` & `types-aiobotocore-worklink-2.5.4/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-worklink-2.5.2.post2/PKG-INFO` & `types-aiobotocore-worklink-2.5.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-worklink
-Version: 2.5.2.post2
-Summary: Type annotations for aiobotocore.WorkLink 2.5.2 service generated with mypy-boto3-builder 7.17.2
+Version: 2.5.4
+Summary: Type annotations for aiobotocore.WorkLink 2.5.4 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_worklink/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-worklink.svg?color=blue)](https://pypi.org/project/types-aiobotocore-worklink)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_worklink/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-worklink)](https://pepy.tech/project/types-aiobotocore-worklink)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.WorkLink 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/worklink.html#WorkLink)
+[aiobotocore.WorkLink 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/worklink.html#WorkLink)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-worklink-2.5.2.post2/README.md` & `types-aiobotocore-worklink-2.5.4/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-worklink.svg?color=blue)](https://pypi.org/project/types-aiobotocore-worklink)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_worklink/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-worklink)](https://pepy.tech/project/types-aiobotocore-worklink)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.WorkLink 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/worklink.html#WorkLink)
+[aiobotocore.WorkLink 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/worklink.html#WorkLink)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-worklink-2.5.2.post2/setup.py` & `types-aiobotocore-worklink-2.5.4/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-worklink",
-    version="2.5.2.post2",
+    version="2.5.4",
     packages=["types_aiobotocore_worklink"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.WorkLink 2.5.2 service generated with mypy-boto3-builder"
+        "Type annotations for aiobotocore.WorkLink 2.5.4 service generated with mypy-boto3-builder"
         " 7.17.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
```

### Comparing `types-aiobotocore-worklink-2.5.2.post2/types_aiobotocore_worklink/client.py` & `types-aiobotocore-worklink-2.5.4/types_aiobotocore_worklink/client.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-worklink-2.5.2.post2/types_aiobotocore_worklink/client.pyi` & `types-aiobotocore-worklink-2.5.4/types_aiobotocore_worklink/client.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-worklink-2.5.2.post2/types_aiobotocore_worklink/literals.py` & `types-aiobotocore-worklink-2.5.4/types_aiobotocore_worklink/literals.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-worklink-2.5.2.post2/types_aiobotocore_worklink/literals.pyi` & `types-aiobotocore-worklink-2.5.4/types_aiobotocore_worklink/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-worklink-2.5.2.post2/types_aiobotocore_worklink/type_defs.py` & `types-aiobotocore-worklink-2.5.4/types_aiobotocore_worklink/type_defs.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-worklink-2.5.2.post2/types_aiobotocore_worklink/type_defs.pyi` & `types-aiobotocore-worklink-2.5.4/types_aiobotocore_worklink/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-worklink-2.5.2.post2/types_aiobotocore_worklink.egg-info/PKG-INFO` & `types-aiobotocore-worklink-2.5.4/types_aiobotocore_worklink.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-worklink
-Version: 2.5.2.post2
-Summary: Type annotations for aiobotocore.WorkLink 2.5.2 service generated with mypy-boto3-builder 7.17.2
+Version: 2.5.4
+Summary: Type annotations for aiobotocore.WorkLink 2.5.4 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_worklink/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-worklink.svg?color=blue)](https://pypi.org/project/types-aiobotocore-worklink)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_worklink/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-worklink)](https://pepy.tech/project/types-aiobotocore-worklink)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.WorkLink 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/worklink.html#WorkLink)
+[aiobotocore.WorkLink 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/worklink.html#WorkLink)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-worklink-2.5.2.post2/types_aiobotocore_worklink.egg-info/SOURCES.txt` & `types-aiobotocore-worklink-2.5.4/types_aiobotocore_worklink.egg-info/SOURCES.txt`

 * *Files identical despite different names*


# Comparing `tmp/types-aiobotocore-mobile-2.5.2.post2.tar.gz` & `tmp/types-aiobotocore-mobile-2.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-mobile-2.5.2.post2.tar", last modified: Fri Aug  4 13:59:19 2023, max compression
+gzip compressed data, was "types-aiobotocore-mobile-2.5.4.tar", last modified: Tue Aug  8 01:24:08 2023, max compression
```

## Comparing `types-aiobotocore-mobile-2.5.2.post2.tar` & `types-aiobotocore-mobile-2.5.4.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:19.126643 types-aiobotocore-mobile-2.5.2.post2/
--rw-r--r--   0 vlad      (1000) vlad      (1000)     1070 2023-08-04 13:45:13.000000 types-aiobotocore-mobile-2.5.2.post2/LICENSE
--rw-r--r--   0 vlad      (1000) vlad      (1000)    12934 2023-08-04 13:59:19.126643 types-aiobotocore-mobile-2.5.2.post2/PKG-INFO
--rw-r--r--   0 vlad      (1000) vlad      (1000)    11420 2023-08-04 13:45:13.000000 types-aiobotocore-mobile-2.5.2.post2/README.md
--rw-r--r--   0 vlad      (1000) vlad      (1000)       38 2023-08-04 13:59:19.126643 types-aiobotocore-mobile-2.5.2.post2/setup.cfg
--rw-r--r--   0 vlad      (1000) vlad      (1000)     2065 2023-08-04 13:45:13.000000 types-aiobotocore-mobile-2.5.2.post2/setup.py
-drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:19.126643 types-aiobotocore-mobile-2.5.2.post2/types_aiobotocore_mobile/
--rw-r--r--   0 vlad      (1000) vlad      (1000)      791 2023-08-04 13:45:13.000000 types-aiobotocore-mobile-2.5.2.post2/types_aiobotocore_mobile/__init__.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)      790 2023-08-04 13:45:13.000000 types-aiobotocore-mobile-2.5.2.post2/types_aiobotocore_mobile/__init__.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)      928 2023-08-04 13:45:13.000000 types-aiobotocore-mobile-2.5.2.post2/types_aiobotocore_mobile/__main__.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)    10204 2023-08-04 13:45:13.000000 types-aiobotocore-mobile-2.5.2.post2/types_aiobotocore_mobile/client.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)    10184 2023-08-04 13:45:13.000000 types-aiobotocore-mobile-2.5.2.post2/types_aiobotocore_mobile/client.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)     8070 2023-08-04 13:45:15.000000 types-aiobotocore-mobile-2.5.2.post2/types_aiobotocore_mobile/literals.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)     8068 2023-08-04 13:45:13.000000 types-aiobotocore-mobile-2.5.2.post2/types_aiobotocore_mobile/literals.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)     2941 2023-08-04 13:45:13.000000 types-aiobotocore-mobile-2.5.2.post2/types_aiobotocore_mobile/paginator.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)     2937 2023-08-04 13:45:13.000000 types-aiobotocore-mobile-2.5.2.post2/types_aiobotocore_mobile/paginator.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:45:13.000000 types-aiobotocore-mobile-2.5.2.post2/types_aiobotocore_mobile/py.typed
--rw-r--r--   0 vlad      (1000) vlad      (1000)     7655 2023-08-04 13:45:15.000000 types-aiobotocore-mobile-2.5.2.post2/types_aiobotocore_mobile/type_defs.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)     7648 2023-08-04 13:45:15.000000 types-aiobotocore-mobile-2.5.2.post2/types_aiobotocore_mobile/type_defs.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)       65 2023-08-04 13:45:13.000000 types-aiobotocore-mobile-2.5.2.post2/types_aiobotocore_mobile/version.py
-drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:19.126643 types-aiobotocore-mobile-2.5.2.post2/types_aiobotocore_mobile.egg-info/
--rw-r--r--   0 vlad      (1000) vlad      (1000)    12934 2023-08-04 13:59:19.000000 types-aiobotocore-mobile-2.5.2.post2/types_aiobotocore_mobile.egg-info/PKG-INFO
--rw-r--r--   0 vlad      (1000) vlad      (1000)      794 2023-08-04 13:59:19.000000 types-aiobotocore-mobile-2.5.2.post2/types_aiobotocore_mobile.egg-info/SOURCES.txt
--rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:19.000000 types-aiobotocore-mobile-2.5.2.post2/types_aiobotocore_mobile.egg-info/dependency_links.txt
--rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:19.000000 types-aiobotocore-mobile-2.5.2.post2/types_aiobotocore_mobile.egg-info/not-zip-safe
--rw-r--r--   0 vlad      (1000) vlad      (1000)       52 2023-08-04 13:59:19.000000 types-aiobotocore-mobile-2.5.2.post2/types_aiobotocore_mobile.egg-info/requires.txt
--rw-r--r--   0 vlad      (1000) vlad      (1000)       25 2023-08-04 13:59:19.000000 types-aiobotocore-mobile-2.5.2.post2/types_aiobotocore_mobile.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:24:08.686739 types-aiobotocore-mobile-2.5.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-08 01:15:38.000000 types-aiobotocore-mobile-2.5.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    12928 2023-08-08 01:24:08.686739 types-aiobotocore-mobile-2.5.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    11420 2023-08-08 01:15:38.000000 types-aiobotocore-mobile-2.5.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-08 01:24:08.686739 types-aiobotocore-mobile-2.5.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2059 2023-08-08 01:15:38.000000 types-aiobotocore-mobile-2.5.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:24:08.686739 types-aiobotocore-mobile-2.5.4/types_aiobotocore_mobile/
+-rw-r--r--   0 runner    (1001) docker     (123)      791 2023-08-08 01:15:38.000000 types-aiobotocore-mobile-2.5.4/types_aiobotocore_mobile/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      790 2023-08-08 01:15:38.000000 types-aiobotocore-mobile-2.5.4/types_aiobotocore_mobile/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      916 2023-08-08 01:15:38.000000 types-aiobotocore-mobile-2.5.4/types_aiobotocore_mobile/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10204 2023-08-08 01:15:38.000000 types-aiobotocore-mobile-2.5.4/types_aiobotocore_mobile/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10184 2023-08-08 01:15:38.000000 types-aiobotocore-mobile-2.5.4/types_aiobotocore_mobile/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8070 2023-08-08 01:15:39.000000 types-aiobotocore-mobile-2.5.4/types_aiobotocore_mobile/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8068 2023-08-08 01:15:39.000000 types-aiobotocore-mobile-2.5.4/types_aiobotocore_mobile/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2941 2023-08-08 01:15:38.000000 types-aiobotocore-mobile-2.5.4/types_aiobotocore_mobile/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2937 2023-08-08 01:15:38.000000 types-aiobotocore-mobile-2.5.4/types_aiobotocore_mobile/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 01:15:38.000000 types-aiobotocore-mobile-2.5.4/types_aiobotocore_mobile/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     7655 2023-08-08 01:15:39.000000 types-aiobotocore-mobile-2.5.4/types_aiobotocore_mobile/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7648 2023-08-08 01:15:39.000000 types-aiobotocore-mobile-2.5.4/types_aiobotocore_mobile/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-08-08 01:15:38.000000 types-aiobotocore-mobile-2.5.4/types_aiobotocore_mobile/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:24:08.686739 types-aiobotocore-mobile-2.5.4/types_aiobotocore_mobile.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    12928 2023-08-08 01:24:08.000000 types-aiobotocore-mobile-2.5.4/types_aiobotocore_mobile.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      794 2023-08-08 01:24:08.000000 types-aiobotocore-mobile-2.5.4/types_aiobotocore_mobile.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 01:24:08.000000 types-aiobotocore-mobile-2.5.4/types_aiobotocore_mobile.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 01:24:08.000000 types-aiobotocore-mobile-2.5.4/types_aiobotocore_mobile.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-08 01:24:08.000000 types-aiobotocore-mobile-2.5.4/types_aiobotocore_mobile.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-08-08 01:24:08.000000 types-aiobotocore-mobile-2.5.4/types_aiobotocore_mobile.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-mobile-2.5.2.post2/LICENSE` & `types-aiobotocore-mobile-2.5.4/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-mobile-2.5.2.post2/PKG-INFO` & `types-aiobotocore-mobile-2.5.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-mobile
-Version: 2.5.2.post2
-Summary: Type annotations for aiobotocore.Mobile 2.5.2 service generated with mypy-boto3-builder 7.17.2
+Version: 2.5.4
+Summary: Type annotations for aiobotocore.Mobile 2.5.4 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mobile/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-mobile.svg?color=blue)](https://pypi.org/project/types-aiobotocore-mobile)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mobile/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-mobile)](https://pepy.tech/project/types-aiobotocore-mobile)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.Mobile 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mobile.html#Mobile)
+[aiobotocore.Mobile 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mobile.html#Mobile)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-mobile-2.5.2.post2/README.md` & `types-aiobotocore-mobile-2.5.4/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-mobile.svg?color=blue)](https://pypi.org/project/types-aiobotocore-mobile)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mobile/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-mobile)](https://pepy.tech/project/types-aiobotocore-mobile)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.Mobile 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mobile.html#Mobile)
+[aiobotocore.Mobile 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mobile.html#Mobile)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-mobile-2.5.2.post2/setup.py` & `types-aiobotocore-mobile-2.5.4/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-mobile",
-    version="2.5.2.post2",
+    version="2.5.4",
     packages=["types_aiobotocore_mobile"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.Mobile 2.5.2 service generated with mypy-boto3-builder"
+        "Type annotations for aiobotocore.Mobile 2.5.4 service generated with mypy-boto3-builder"
         " 7.17.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
```

### Comparing `types-aiobotocore-mobile-2.5.2.post2/types_aiobotocore_mobile/__init__.py` & `types-aiobotocore-mobile-2.5.4/types_aiobotocore_mobile/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-mobile-2.5.2.post2/types_aiobotocore_mobile/__init__.pyi` & `types-aiobotocore-mobile-2.5.4/types_aiobotocore_mobile/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-mobile-2.5.2.post2/types_aiobotocore_mobile/client.py` & `types-aiobotocore-mobile-2.5.4/types_aiobotocore_mobile/client.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-mobile-2.5.2.post2/types_aiobotocore_mobile/client.pyi` & `types-aiobotocore-mobile-2.5.4/types_aiobotocore_mobile/client.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-mobile-2.5.2.post2/types_aiobotocore_mobile/literals.py` & `types-aiobotocore-mobile-2.5.4/types_aiobotocore_mobile/literals.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-mobile-2.5.2.post2/types_aiobotocore_mobile/literals.pyi` & `types-aiobotocore-mobile-2.5.4/types_aiobotocore_mobile/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-mobile-2.5.2.post2/types_aiobotocore_mobile/paginator.py` & `types-aiobotocore-mobile-2.5.4/types_aiobotocore_mobile/paginator.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-mobile-2.5.2.post2/types_aiobotocore_mobile/paginator.pyi` & `types-aiobotocore-mobile-2.5.4/types_aiobotocore_mobile/paginator.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-mobile-2.5.2.post2/types_aiobotocore_mobile/type_defs.py` & `types-aiobotocore-mobile-2.5.4/types_aiobotocore_mobile/type_defs.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-mobile-2.5.2.post2/types_aiobotocore_mobile/type_defs.pyi` & `types-aiobotocore-mobile-2.5.4/types_aiobotocore_mobile/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-mobile-2.5.2.post2/types_aiobotocore_mobile.egg-info/PKG-INFO` & `types-aiobotocore-mobile-2.5.4/types_aiobotocore_mobile.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-mobile
-Version: 2.5.2.post2
-Summary: Type annotations for aiobotocore.Mobile 2.5.2 service generated with mypy-boto3-builder 7.17.2
+Version: 2.5.4
+Summary: Type annotations for aiobotocore.Mobile 2.5.4 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mobile/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-mobile.svg?color=blue)](https://pypi.org/project/types-aiobotocore-mobile)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mobile/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-mobile)](https://pepy.tech/project/types-aiobotocore-mobile)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.Mobile 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mobile.html#Mobile)
+[aiobotocore.Mobile 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mobile.html#Mobile)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-mobile-2.5.2.post2/types_aiobotocore_mobile.egg-info/SOURCES.txt` & `types-aiobotocore-mobile-2.5.4/types_aiobotocore_mobile.egg-info/SOURCES.txt`

 * *Files identical despite different names*


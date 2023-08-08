# Comparing `tmp/types-aiobotocore-personalize-2.5.2.post2.tar.gz` & `tmp/types-aiobotocore-personalize-2.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-personalize-2.5.2.post2.tar", last modified: Fri Aug  4 13:59:20 2023, max compression
+gzip compressed data, was "types-aiobotocore-personalize-2.5.4.tar", last modified: Tue Aug  8 01:24:13 2023, max compression
```

## Comparing `types-aiobotocore-personalize-2.5.2.post2.tar` & `types-aiobotocore-personalize-2.5.4.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:20.946643 types-aiobotocore-personalize-2.5.2.post2/
--rw-r--r--   0 vlad      (1000) vlad      (1000)     1070 2023-08-04 13:46:30.000000 types-aiobotocore-personalize-2.5.2.post2/LICENSE
--rw-r--r--   0 vlad      (1000) vlad      (1000)    15392 2023-08-04 13:59:20.946643 types-aiobotocore-personalize-2.5.2.post2/PKG-INFO
--rw-r--r--   0 vlad      (1000) vlad      (1000)    13858 2023-08-04 13:46:30.000000 types-aiobotocore-personalize-2.5.2.post2/README.md
--rw-r--r--   0 vlad      (1000) vlad      (1000)       38 2023-08-04 13:59:20.946643 types-aiobotocore-personalize-2.5.2.post2/setup.cfg
--rw-r--r--   0 vlad      (1000) vlad      (1000)     2100 2023-08-04 13:46:30.000000 types-aiobotocore-personalize-2.5.2.post2/setup.py
-drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:20.946643 types-aiobotocore-personalize-2.5.2.post2/types_aiobotocore_personalize/
--rw-r--r--   0 vlad      (1000) vlad      (1000)     3887 2023-08-04 13:46:30.000000 types-aiobotocore-personalize-2.5.2.post2/types_aiobotocore_personalize/__init__.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)     3886 2023-08-04 13:46:30.000000 types-aiobotocore-personalize-2.5.2.post2/types_aiobotocore_personalize/__init__.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)      959 2023-08-04 13:46:30.000000 types-aiobotocore-personalize-2.5.2.post2/types_aiobotocore_personalize/__main__.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)    54521 2023-08-04 13:46:32.000000 types-aiobotocore-personalize-2.5.2.post2/types_aiobotocore_personalize/client.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)    54429 2023-08-04 13:46:31.000000 types-aiobotocore-personalize-2.5.2.post2/types_aiobotocore_personalize/client.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)    10451 2023-08-04 13:46:32.000000 types-aiobotocore-personalize-2.5.2.post2/types_aiobotocore_personalize/literals.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)    10449 2023-08-04 13:46:32.000000 types-aiobotocore-personalize-2.5.2.post2/types_aiobotocore_personalize/literals.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)    19533 2023-08-04 13:46:32.000000 types-aiobotocore-personalize-2.5.2.post2/types_aiobotocore_personalize/paginator.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)    19514 2023-08-04 13:46:32.000000 types-aiobotocore-personalize-2.5.2.post2/types_aiobotocore_personalize/paginator.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:46:30.000000 types-aiobotocore-personalize-2.5.2.post2/types_aiobotocore_personalize/py.typed
--rw-r--r--   0 vlad      (1000) vlad      (1000)    63287 2023-08-04 13:46:34.000000 types-aiobotocore-personalize-2.5.2.post2/types_aiobotocore_personalize/type_defs.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)    63252 2023-08-04 13:46:33.000000 types-aiobotocore-personalize-2.5.2.post2/types_aiobotocore_personalize/type_defs.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)       65 2023-08-04 13:46:30.000000 types-aiobotocore-personalize-2.5.2.post2/types_aiobotocore_personalize/version.py
-drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:20.946643 types-aiobotocore-personalize-2.5.2.post2/types_aiobotocore_personalize.egg-info/
--rw-r--r--   0 vlad      (1000) vlad      (1000)    15392 2023-08-04 13:59:20.000000 types-aiobotocore-personalize-2.5.2.post2/types_aiobotocore_personalize.egg-info/PKG-INFO
--rw-r--r--   0 vlad      (1000) vlad      (1000)      889 2023-08-04 13:59:20.000000 types-aiobotocore-personalize-2.5.2.post2/types_aiobotocore_personalize.egg-info/SOURCES.txt
--rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:20.000000 types-aiobotocore-personalize-2.5.2.post2/types_aiobotocore_personalize.egg-info/dependency_links.txt
--rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:20.000000 types-aiobotocore-personalize-2.5.2.post2/types_aiobotocore_personalize.egg-info/not-zip-safe
--rw-r--r--   0 vlad      (1000) vlad      (1000)       52 2023-08-04 13:59:20.000000 types-aiobotocore-personalize-2.5.2.post2/types_aiobotocore_personalize.egg-info/requires.txt
--rw-r--r--   0 vlad      (1000) vlad      (1000)       30 2023-08-04 13:59:20.000000 types-aiobotocore-personalize-2.5.2.post2/types_aiobotocore_personalize.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:24:13.210748 types-aiobotocore-personalize-2.5.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-08 01:16:29.000000 types-aiobotocore-personalize-2.5.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    15386 2023-08-08 01:24:13.206748 types-aiobotocore-personalize-2.5.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    13858 2023-08-08 01:16:29.000000 types-aiobotocore-personalize-2.5.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-08 01:24:13.210748 types-aiobotocore-personalize-2.5.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2094 2023-08-08 01:16:29.000000 types-aiobotocore-personalize-2.5.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:24:13.206748 types-aiobotocore-personalize-2.5.4/types_aiobotocore_personalize/
+-rw-r--r--   0 runner    (1001) docker     (123)     3887 2023-08-08 01:16:29.000000 types-aiobotocore-personalize-2.5.4/types_aiobotocore_personalize/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3886 2023-08-08 01:16:29.000000 types-aiobotocore-personalize-2.5.4/types_aiobotocore_personalize/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      947 2023-08-08 01:16:29.000000 types-aiobotocore-personalize-2.5.4/types_aiobotocore_personalize/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    54521 2023-08-08 01:16:29.000000 types-aiobotocore-personalize-2.5.4/types_aiobotocore_personalize/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    54429 2023-08-08 01:16:29.000000 types-aiobotocore-personalize-2.5.4/types_aiobotocore_personalize/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    10451 2023-08-08 01:16:29.000000 types-aiobotocore-personalize-2.5.4/types_aiobotocore_personalize/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10449 2023-08-08 01:16:29.000000 types-aiobotocore-personalize-2.5.4/types_aiobotocore_personalize/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    19533 2023-08-08 01:16:29.000000 types-aiobotocore-personalize-2.5.4/types_aiobotocore_personalize/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19514 2023-08-08 01:16:29.000000 types-aiobotocore-personalize-2.5.4/types_aiobotocore_personalize/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 01:16:29.000000 types-aiobotocore-personalize-2.5.4/types_aiobotocore_personalize/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    63287 2023-08-08 01:16:31.000000 types-aiobotocore-personalize-2.5.4/types_aiobotocore_personalize/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    63252 2023-08-08 01:16:30.000000 types-aiobotocore-personalize-2.5.4/types_aiobotocore_personalize/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-08-08 01:16:29.000000 types-aiobotocore-personalize-2.5.4/types_aiobotocore_personalize/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:24:13.206748 types-aiobotocore-personalize-2.5.4/types_aiobotocore_personalize.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    15386 2023-08-08 01:24:13.000000 types-aiobotocore-personalize-2.5.4/types_aiobotocore_personalize.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      889 2023-08-08 01:24:13.000000 types-aiobotocore-personalize-2.5.4/types_aiobotocore_personalize.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 01:24:13.000000 types-aiobotocore-personalize-2.5.4/types_aiobotocore_personalize.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 01:24:13.000000 types-aiobotocore-personalize-2.5.4/types_aiobotocore_personalize.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-08 01:24:13.000000 types-aiobotocore-personalize-2.5.4/types_aiobotocore_personalize.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-08-08 01:24:13.000000 types-aiobotocore-personalize-2.5.4/types_aiobotocore_personalize.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-personalize-2.5.2.post2/LICENSE` & `types-aiobotocore-personalize-2.5.4/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-personalize-2.5.2.post2/PKG-INFO` & `types-aiobotocore-personalize-2.5.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-personalize
-Version: 2.5.2.post2
-Summary: Type annotations for aiobotocore.Personalize 2.5.2 service generated with mypy-boto3-builder 7.17.2
+Version: 2.5.4
+Summary: Type annotations for aiobotocore.Personalize 2.5.4 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_personalize/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-personalize.svg?color=blue)](https://pypi.org/project/types-aiobotocore-personalize)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_personalize/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-personalize)](https://pepy.tech/project/types-aiobotocore-personalize)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.Personalize 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize)
+[aiobotocore.Personalize 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-personalize-2.5.2.post2/README.md` & `types-aiobotocore-personalize-2.5.4/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-personalize.svg?color=blue)](https://pypi.org/project/types-aiobotocore-personalize)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_personalize/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-personalize)](https://pepy.tech/project/types-aiobotocore-personalize)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.Personalize 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize)
+[aiobotocore.Personalize 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-personalize-2.5.2.post2/setup.py` & `types-aiobotocore-personalize-2.5.4/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-personalize",
-    version="2.5.2.post2",
+    version="2.5.4",
     packages=["types_aiobotocore_personalize"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.Personalize 2.5.2 service generated with"
+        "Type annotations for aiobotocore.Personalize 2.5.4 service generated with"
         " mypy-boto3-builder 7.17.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
```

### Comparing `types-aiobotocore-personalize-2.5.2.post2/types_aiobotocore_personalize/__init__.py` & `types-aiobotocore-personalize-2.5.4/types_aiobotocore_personalize/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-personalize-2.5.2.post2/types_aiobotocore_personalize/__init__.pyi` & `types-aiobotocore-personalize-2.5.4/types_aiobotocore_personalize/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-personalize-2.5.2.post2/types_aiobotocore_personalize/__main__.py` & `types-aiobotocore-personalize-2.5.4/types_aiobotocore_personalize/__main__.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.Personalize 2.5.2\nVersion:         2.5.2.post2\nBuilder"
+        "Type annotations for aiobotocore.Personalize 2.5.4\nVersion:         2.5.4\nBuilder"
         " version: 7.17.2\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_personalize//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize\nOther"
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

### Comparing `types-aiobotocore-personalize-2.5.2.post2/types_aiobotocore_personalize/client.py` & `types-aiobotocore-personalize-2.5.4/types_aiobotocore_personalize/client.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-personalize-2.5.2.post2/types_aiobotocore_personalize/client.pyi` & `types-aiobotocore-personalize-2.5.4/types_aiobotocore_personalize/client.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-personalize-2.5.2.post2/types_aiobotocore_personalize/literals.py` & `types-aiobotocore-personalize-2.5.4/types_aiobotocore_personalize/literals.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-personalize-2.5.2.post2/types_aiobotocore_personalize/literals.pyi` & `types-aiobotocore-personalize-2.5.4/types_aiobotocore_personalize/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-personalize-2.5.2.post2/types_aiobotocore_personalize/paginator.py` & `types-aiobotocore-personalize-2.5.4/types_aiobotocore_personalize/paginator.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-personalize-2.5.2.post2/types_aiobotocore_personalize/paginator.pyi` & `types-aiobotocore-personalize-2.5.4/types_aiobotocore_personalize/paginator.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-personalize-2.5.2.post2/types_aiobotocore_personalize/type_defs.py` & `types-aiobotocore-personalize-2.5.4/types_aiobotocore_personalize/type_defs.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-personalize-2.5.2.post2/types_aiobotocore_personalize/type_defs.pyi` & `types-aiobotocore-personalize-2.5.4/types_aiobotocore_personalize/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-personalize-2.5.2.post2/types_aiobotocore_personalize.egg-info/PKG-INFO` & `types-aiobotocore-personalize-2.5.4/types_aiobotocore_personalize.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-personalize
-Version: 2.5.2.post2
-Summary: Type annotations for aiobotocore.Personalize 2.5.2 service generated with mypy-boto3-builder 7.17.2
+Version: 2.5.4
+Summary: Type annotations for aiobotocore.Personalize 2.5.4 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_personalize/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-personalize.svg?color=blue)](https://pypi.org/project/types-aiobotocore-personalize)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_personalize/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-personalize)](https://pepy.tech/project/types-aiobotocore-personalize)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.Personalize 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize)
+[aiobotocore.Personalize 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-personalize-2.5.2.post2/types_aiobotocore_personalize.egg-info/SOURCES.txt` & `types-aiobotocore-personalize-2.5.4/types_aiobotocore_personalize.egg-info/SOURCES.txt`

 * *Files identical despite different names*

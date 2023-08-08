# Comparing `tmp/types-aiobotocore-secretsmanager-2.5.2.post2.tar.gz` & `tmp/types-aiobotocore-secretsmanager-2.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-secretsmanager-2.5.2.post2.tar", last modified: Fri Aug  4 13:59:25 2023, max compression
+gzip compressed data, was "types-aiobotocore-secretsmanager-2.5.4.tar", last modified: Tue Aug  8 01:24:24 2023, max compression
```

## Comparing `types-aiobotocore-secretsmanager-2.5.2.post2.tar` & `types-aiobotocore-secretsmanager-2.5.4.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:25.766643 types-aiobotocore-secretsmanager-2.5.2.post2/
--rw-r--r--   0 vlad      (1000) vlad      (1000)     1070 2023-08-04 13:52:43.000000 types-aiobotocore-secretsmanager-2.5.2.post2/LICENSE
--rw-r--r--   0 vlad      (1000) vlad      (1000)    13292 2023-08-04 13:59:25.766643 types-aiobotocore-secretsmanager-2.5.2.post2/PKG-INFO
--rw-r--r--   0 vlad      (1000) vlad      (1000)    11746 2023-08-04 13:52:43.000000 types-aiobotocore-secretsmanager-2.5.2.post2/README.md
--rw-r--r--   0 vlad      (1000) vlad      (1000)       38 2023-08-04 13:59:25.766643 types-aiobotocore-secretsmanager-2.5.2.post2/setup.cfg
--rw-r--r--   0 vlad      (1000) vlad      (1000)     2121 2023-08-04 13:52:43.000000 types-aiobotocore-secretsmanager-2.5.2.post2/setup.py
-drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:25.756643 types-aiobotocore-secretsmanager-2.5.2.post2/types_aiobotocore_secretsmanager/
--rw-r--r--   0 vlad      (1000) vlad      (1000)      685 2023-08-04 13:52:43.000000 types-aiobotocore-secretsmanager-2.5.2.post2/types_aiobotocore_secretsmanager/__init__.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)      684 2023-08-04 13:52:43.000000 types-aiobotocore-secretsmanager-2.5.2.post2/types_aiobotocore_secretsmanager/__init__.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)      971 2023-08-04 13:52:43.000000 types-aiobotocore-secretsmanager-2.5.2.post2/types_aiobotocore_secretsmanager/__main__.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)    20286 2023-08-04 13:52:43.000000 types-aiobotocore-secretsmanager-2.5.2.post2/types_aiobotocore_secretsmanager/client.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)    20254 2023-08-04 13:52:43.000000 types-aiobotocore-secretsmanager-2.5.2.post2/types_aiobotocore_secretsmanager/client.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)     8696 2023-08-04 13:52:43.000000 types-aiobotocore-secretsmanager-2.5.2.post2/types_aiobotocore_secretsmanager/literals.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)     8694 2023-08-04 13:52:43.000000 types-aiobotocore-secretsmanager-2.5.2.post2/types_aiobotocore_secretsmanager/literals.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)     2251 2023-08-04 13:52:43.000000 types-aiobotocore-secretsmanager-2.5.2.post2/types_aiobotocore_secretsmanager/paginator.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)     2248 2023-08-04 13:52:43.000000 types-aiobotocore-secretsmanager-2.5.2.post2/types_aiobotocore_secretsmanager/paginator.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:52:43.000000 types-aiobotocore-secretsmanager-2.5.2.post2/types_aiobotocore_secretsmanager/py.typed
--rw-r--r--   0 vlad      (1000) vlad      (1000)    19547 2023-08-04 13:52:44.000000 types-aiobotocore-secretsmanager-2.5.2.post2/types_aiobotocore_secretsmanager/type_defs.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)    19524 2023-08-04 13:52:44.000000 types-aiobotocore-secretsmanager-2.5.2.post2/types_aiobotocore_secretsmanager/type_defs.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)       65 2023-08-04 13:52:43.000000 types-aiobotocore-secretsmanager-2.5.2.post2/types_aiobotocore_secretsmanager/version.py
-drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:25.766643 types-aiobotocore-secretsmanager-2.5.2.post2/types_aiobotocore_secretsmanager.egg-info/
--rw-r--r--   0 vlad      (1000) vlad      (1000)    13292 2023-08-04 13:59:25.000000 types-aiobotocore-secretsmanager-2.5.2.post2/types_aiobotocore_secretsmanager.egg-info/PKG-INFO
--rw-r--r--   0 vlad      (1000) vlad      (1000)      946 2023-08-04 13:59:25.000000 types-aiobotocore-secretsmanager-2.5.2.post2/types_aiobotocore_secretsmanager.egg-info/SOURCES.txt
--rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:25.000000 types-aiobotocore-secretsmanager-2.5.2.post2/types_aiobotocore_secretsmanager.egg-info/dependency_links.txt
--rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:25.000000 types-aiobotocore-secretsmanager-2.5.2.post2/types_aiobotocore_secretsmanager.egg-info/not-zip-safe
--rw-r--r--   0 vlad      (1000) vlad      (1000)       52 2023-08-04 13:59:25.000000 types-aiobotocore-secretsmanager-2.5.2.post2/types_aiobotocore_secretsmanager.egg-info/requires.txt
--rw-r--r--   0 vlad      (1000) vlad      (1000)       33 2023-08-04 13:59:25.000000 types-aiobotocore-secretsmanager-2.5.2.post2/types_aiobotocore_secretsmanager.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:24:24.950777 types-aiobotocore-secretsmanager-2.5.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-08 01:20:36.000000 types-aiobotocore-secretsmanager-2.5.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    13286 2023-08-08 01:24:24.950777 types-aiobotocore-secretsmanager-2.5.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    11746 2023-08-08 01:20:36.000000 types-aiobotocore-secretsmanager-2.5.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-08 01:24:24.950777 types-aiobotocore-secretsmanager-2.5.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2115 2023-08-08 01:20:36.000000 types-aiobotocore-secretsmanager-2.5.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:24:24.946777 types-aiobotocore-secretsmanager-2.5.4/types_aiobotocore_secretsmanager/
+-rw-r--r--   0 runner    (1001) docker     (123)      685 2023-08-08 01:20:36.000000 types-aiobotocore-secretsmanager-2.5.4/types_aiobotocore_secretsmanager/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      684 2023-08-08 01:20:36.000000 types-aiobotocore-secretsmanager-2.5.4/types_aiobotocore_secretsmanager/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      959 2023-08-08 01:20:36.000000 types-aiobotocore-secretsmanager-2.5.4/types_aiobotocore_secretsmanager/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20286 2023-08-08 01:20:36.000000 types-aiobotocore-secretsmanager-2.5.4/types_aiobotocore_secretsmanager/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20254 2023-08-08 01:20:36.000000 types-aiobotocore-secretsmanager-2.5.4/types_aiobotocore_secretsmanager/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8696 2023-08-08 01:20:36.000000 types-aiobotocore-secretsmanager-2.5.4/types_aiobotocore_secretsmanager/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8694 2023-08-08 01:20:36.000000 types-aiobotocore-secretsmanager-2.5.4/types_aiobotocore_secretsmanager/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2251 2023-08-08 01:20:36.000000 types-aiobotocore-secretsmanager-2.5.4/types_aiobotocore_secretsmanager/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2248 2023-08-08 01:20:36.000000 types-aiobotocore-secretsmanager-2.5.4/types_aiobotocore_secretsmanager/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 01:20:36.000000 types-aiobotocore-secretsmanager-2.5.4/types_aiobotocore_secretsmanager/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    19547 2023-08-08 01:20:37.000000 types-aiobotocore-secretsmanager-2.5.4/types_aiobotocore_secretsmanager/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19524 2023-08-08 01:20:36.000000 types-aiobotocore-secretsmanager-2.5.4/types_aiobotocore_secretsmanager/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-08-08 01:20:36.000000 types-aiobotocore-secretsmanager-2.5.4/types_aiobotocore_secretsmanager/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:24:24.950777 types-aiobotocore-secretsmanager-2.5.4/types_aiobotocore_secretsmanager.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    13286 2023-08-08 01:24:24.000000 types-aiobotocore-secretsmanager-2.5.4/types_aiobotocore_secretsmanager.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      946 2023-08-08 01:24:24.000000 types-aiobotocore-secretsmanager-2.5.4/types_aiobotocore_secretsmanager.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 01:24:24.000000 types-aiobotocore-secretsmanager-2.5.4/types_aiobotocore_secretsmanager.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 01:24:24.000000 types-aiobotocore-secretsmanager-2.5.4/types_aiobotocore_secretsmanager.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-08 01:24:24.000000 types-aiobotocore-secretsmanager-2.5.4/types_aiobotocore_secretsmanager.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-08-08 01:24:24.000000 types-aiobotocore-secretsmanager-2.5.4/types_aiobotocore_secretsmanager.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-secretsmanager-2.5.2.post2/LICENSE` & `types-aiobotocore-secretsmanager-2.5.4/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-secretsmanager-2.5.2.post2/PKG-INFO` & `types-aiobotocore-secretsmanager-2.5.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-secretsmanager
-Version: 2.5.2.post2
-Summary: Type annotations for aiobotocore.SecretsManager 2.5.2 service generated with mypy-boto3-builder 7.17.2
+Version: 2.5.4
+Summary: Type annotations for aiobotocore.SecretsManager 2.5.4 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_secretsmanager/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-secretsmanager.svg?color=blue)](https://pypi.org/project/types-aiobotocore-secretsmanager)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_secretsmanager/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-secretsmanager)](https://pepy.tech/project/types-aiobotocore-secretsmanager)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.SecretsManager 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/secretsmanager.html#SecretsManager)
+[aiobotocore.SecretsManager 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/secretsmanager.html#SecretsManager)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-secretsmanager-2.5.2.post2/README.md` & `types-aiobotocore-secretsmanager-2.5.4/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-secretsmanager.svg?color=blue)](https://pypi.org/project/types-aiobotocore-secretsmanager)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_secretsmanager/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-secretsmanager)](https://pepy.tech/project/types-aiobotocore-secretsmanager)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.SecretsManager 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/secretsmanager.html#SecretsManager)
+[aiobotocore.SecretsManager 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/secretsmanager.html#SecretsManager)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-secretsmanager-2.5.2.post2/setup.py` & `types-aiobotocore-secretsmanager-2.5.4/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-secretsmanager",
-    version="2.5.2.post2",
+    version="2.5.4",
     packages=["types_aiobotocore_secretsmanager"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.SecretsManager 2.5.2 service generated with"
+        "Type annotations for aiobotocore.SecretsManager 2.5.4 service generated with"
         " mypy-boto3-builder 7.17.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
```

### Comparing `types-aiobotocore-secretsmanager-2.5.2.post2/types_aiobotocore_secretsmanager/__init__.py` & `types-aiobotocore-secretsmanager-2.5.4/types_aiobotocore_secretsmanager/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-secretsmanager-2.5.2.post2/types_aiobotocore_secretsmanager/__init__.pyi` & `types-aiobotocore-secretsmanager-2.5.4/types_aiobotocore_secretsmanager/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-secretsmanager-2.5.2.post2/types_aiobotocore_secretsmanager/__main__.py` & `types-aiobotocore-secretsmanager-2.5.4/types_aiobotocore_secretsmanager/__main__.py`

 * *Files 20% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.SecretsManager 2.5.2\nVersion:        "
-        " 2.5.2.post2\nBuilder version: 7.17.2\nDocs:           "
+        "Type annotations for aiobotocore.SecretsManager 2.5.4\nVersion:         2.5.4\nBuilder"
+        " version: 7.17.2\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_secretsmanager//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/secretsmanager.html#SecretsManager\nOther"
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

### Comparing `types-aiobotocore-secretsmanager-2.5.2.post2/types_aiobotocore_secretsmanager/client.py` & `types-aiobotocore-secretsmanager-2.5.4/types_aiobotocore_secretsmanager/client.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-secretsmanager-2.5.2.post2/types_aiobotocore_secretsmanager/client.pyi` & `types-aiobotocore-secretsmanager-2.5.4/types_aiobotocore_secretsmanager/client.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-secretsmanager-2.5.2.post2/types_aiobotocore_secretsmanager/literals.py` & `types-aiobotocore-secretsmanager-2.5.4/types_aiobotocore_secretsmanager/literals.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-secretsmanager-2.5.2.post2/types_aiobotocore_secretsmanager/literals.pyi` & `types-aiobotocore-secretsmanager-2.5.4/types_aiobotocore_secretsmanager/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-secretsmanager-2.5.2.post2/types_aiobotocore_secretsmanager/paginator.py` & `types-aiobotocore-secretsmanager-2.5.4/types_aiobotocore_secretsmanager/paginator.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-secretsmanager-2.5.2.post2/types_aiobotocore_secretsmanager/paginator.pyi` & `types-aiobotocore-secretsmanager-2.5.4/types_aiobotocore_secretsmanager/paginator.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-secretsmanager-2.5.2.post2/types_aiobotocore_secretsmanager/type_defs.py` & `types-aiobotocore-secretsmanager-2.5.4/types_aiobotocore_secretsmanager/type_defs.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-secretsmanager-2.5.2.post2/types_aiobotocore_secretsmanager/type_defs.pyi` & `types-aiobotocore-secretsmanager-2.5.4/types_aiobotocore_secretsmanager/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-secretsmanager-2.5.2.post2/types_aiobotocore_secretsmanager.egg-info/PKG-INFO` & `types-aiobotocore-secretsmanager-2.5.4/types_aiobotocore_secretsmanager.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-secretsmanager
-Version: 2.5.2.post2
-Summary: Type annotations for aiobotocore.SecretsManager 2.5.2 service generated with mypy-boto3-builder 7.17.2
+Version: 2.5.4
+Summary: Type annotations for aiobotocore.SecretsManager 2.5.4 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_secretsmanager/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-secretsmanager.svg?color=blue)](https://pypi.org/project/types-aiobotocore-secretsmanager)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_secretsmanager/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-secretsmanager)](https://pepy.tech/project/types-aiobotocore-secretsmanager)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.SecretsManager 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/secretsmanager.html#SecretsManager)
+[aiobotocore.SecretsManager 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/secretsmanager.html#SecretsManager)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-secretsmanager-2.5.2.post2/types_aiobotocore_secretsmanager.egg-info/SOURCES.txt` & `types-aiobotocore-secretsmanager-2.5.4/types_aiobotocore_secretsmanager.egg-info/SOURCES.txt`

 * *Files identical despite different names*


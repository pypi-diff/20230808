# Comparing `tmp/types-aiobotocore-opsworkscm-2.5.2.post2.tar.gz` & `tmp/types-aiobotocore-opsworkscm-2.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-opsworkscm-2.5.2.post2.tar", last modified: Fri Aug  4 13:59:20 2023, max compression
+gzip compressed data, was "types-aiobotocore-opsworkscm-2.5.4.tar", last modified: Tue Aug  8 01:24:11 2023, max compression
```

## Comparing `types-aiobotocore-opsworkscm-2.5.2.post2.tar` & `types-aiobotocore-opsworkscm-2.5.4.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:20.276643 types-aiobotocore-opsworkscm-2.5.2.post2/
--rw-r--r--   0 vlad      (1000) vlad      (1000)     1070 2023-08-04 13:46:11.000000 types-aiobotocore-opsworkscm-2.5.2.post2/LICENSE
--rw-r--r--   0 vlad      (1000) vlad      (1000)    14212 2023-08-04 13:59:20.276643 types-aiobotocore-opsworkscm-2.5.2.post2/PKG-INFO
--rw-r--r--   0 vlad      (1000) vlad      (1000)    12682 2023-08-04 13:46:11.000000 types-aiobotocore-opsworkscm-2.5.2.post2/README.md
--rw-r--r--   0 vlad      (1000) vlad      (1000)       38 2023-08-04 13:59:20.276643 types-aiobotocore-opsworkscm-2.5.2.post2/setup.cfg
--rw-r--r--   0 vlad      (1000) vlad      (1000)     2093 2023-08-04 13:46:11.000000 types-aiobotocore-opsworkscm-2.5.2.post2/setup.py
-drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:20.276643 types-aiobotocore-opsworkscm-2.5.2.post2/types_aiobotocore_opsworkscm/
--rw-r--r--   0 vlad      (1000) vlad      (1000)     1499 2023-08-04 13:46:11.000000 types-aiobotocore-opsworkscm-2.5.2.post2/types_aiobotocore_opsworkscm/__init__.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)     1498 2023-08-04 13:46:11.000000 types-aiobotocore-opsworkscm-2.5.2.post2/types_aiobotocore_opsworkscm/__init__.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)      955 2023-08-04 13:46:11.000000 types-aiobotocore-opsworkscm-2.5.2.post2/types_aiobotocore_opsworkscm/__main__.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)    19181 2023-08-04 13:46:11.000000 types-aiobotocore-opsworkscm-2.5.2.post2/types_aiobotocore_opsworkscm/client.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)    19148 2023-08-04 13:46:11.000000 types-aiobotocore-opsworkscm-2.5.2.post2/types_aiobotocore_opsworkscm/client.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)     9143 2023-08-04 13:46:12.000000 types-aiobotocore-opsworkscm-2.5.2.post2/types_aiobotocore_opsworkscm/literals.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)     9141 2023-08-04 13:46:11.000000 types-aiobotocore-opsworkscm-2.5.2.post2/types_aiobotocore_opsworkscm/literals.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)     5487 2023-08-04 13:46:11.000000 types-aiobotocore-opsworkscm-2.5.2.post2/types_aiobotocore_opsworkscm/paginator.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)     5481 2023-08-04 13:46:11.000000 types-aiobotocore-opsworkscm-2.5.2.post2/types_aiobotocore_opsworkscm/paginator.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:46:11.000000 types-aiobotocore-opsworkscm-2.5.2.post2/types_aiobotocore_opsworkscm/py.typed
--rw-r--r--   0 vlad      (1000) vlad      (1000)    18776 2023-08-04 13:46:12.000000 types-aiobotocore-opsworkscm-2.5.2.post2/types_aiobotocore_opsworkscm/type_defs.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)    18749 2023-08-04 13:46:12.000000 types-aiobotocore-opsworkscm-2.5.2.post2/types_aiobotocore_opsworkscm/type_defs.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)       65 2023-08-04 13:46:11.000000 types-aiobotocore-opsworkscm-2.5.2.post2/types_aiobotocore_opsworkscm/version.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)     1638 2023-08-04 13:46:11.000000 types-aiobotocore-opsworkscm-2.5.2.post2/types_aiobotocore_opsworkscm/waiter.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)     1637 2023-08-04 13:46:11.000000 types-aiobotocore-opsworkscm-2.5.2.post2/types_aiobotocore_opsworkscm/waiter.pyi
-drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:20.276643 types-aiobotocore-opsworkscm-2.5.2.post2/types_aiobotocore_opsworkscm.egg-info/
--rw-r--r--   0 vlad      (1000) vlad      (1000)    14212 2023-08-04 13:59:20.000000 types-aiobotocore-opsworkscm-2.5.2.post2/types_aiobotocore_opsworkscm.egg-info/PKG-INFO
--rw-r--r--   0 vlad      (1000) vlad      (1000)      949 2023-08-04 13:59:20.000000 types-aiobotocore-opsworkscm-2.5.2.post2/types_aiobotocore_opsworkscm.egg-info/SOURCES.txt
--rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:20.000000 types-aiobotocore-opsworkscm-2.5.2.post2/types_aiobotocore_opsworkscm.egg-info/dependency_links.txt
--rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:20.000000 types-aiobotocore-opsworkscm-2.5.2.post2/types_aiobotocore_opsworkscm.egg-info/not-zip-safe
--rw-r--r--   0 vlad      (1000) vlad      (1000)       52 2023-08-04 13:59:20.000000 types-aiobotocore-opsworkscm-2.5.2.post2/types_aiobotocore_opsworkscm.egg-info/requires.txt
--rw-r--r--   0 vlad      (1000) vlad      (1000)       29 2023-08-04 13:59:20.000000 types-aiobotocore-opsworkscm-2.5.2.post2/types_aiobotocore_opsworkscm.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:24:11.258744 types-aiobotocore-opsworkscm-2.5.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-08 01:16:16.000000 types-aiobotocore-opsworkscm-2.5.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    14206 2023-08-08 01:24:11.254744 types-aiobotocore-opsworkscm-2.5.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    12682 2023-08-08 01:16:16.000000 types-aiobotocore-opsworkscm-2.5.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-08 01:24:11.258744 types-aiobotocore-opsworkscm-2.5.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2087 2023-08-08 01:16:16.000000 types-aiobotocore-opsworkscm-2.5.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:24:11.254744 types-aiobotocore-opsworkscm-2.5.4/types_aiobotocore_opsworkscm/
+-rw-r--r--   0 runner    (1001) docker     (123)     1499 2023-08-08 01:16:16.000000 types-aiobotocore-opsworkscm-2.5.4/types_aiobotocore_opsworkscm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1498 2023-08-08 01:16:16.000000 types-aiobotocore-opsworkscm-2.5.4/types_aiobotocore_opsworkscm/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      943 2023-08-08 01:16:16.000000 types-aiobotocore-opsworkscm-2.5.4/types_aiobotocore_opsworkscm/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19181 2023-08-08 01:16:16.000000 types-aiobotocore-opsworkscm-2.5.4/types_aiobotocore_opsworkscm/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19148 2023-08-08 01:16:16.000000 types-aiobotocore-opsworkscm-2.5.4/types_aiobotocore_opsworkscm/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9143 2023-08-08 01:16:16.000000 types-aiobotocore-opsworkscm-2.5.4/types_aiobotocore_opsworkscm/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9141 2023-08-08 01:16:16.000000 types-aiobotocore-opsworkscm-2.5.4/types_aiobotocore_opsworkscm/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     5487 2023-08-08 01:16:16.000000 types-aiobotocore-opsworkscm-2.5.4/types_aiobotocore_opsworkscm/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5481 2023-08-08 01:16:16.000000 types-aiobotocore-opsworkscm-2.5.4/types_aiobotocore_opsworkscm/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 01:16:16.000000 types-aiobotocore-opsworkscm-2.5.4/types_aiobotocore_opsworkscm/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    18776 2023-08-08 01:16:18.000000 types-aiobotocore-opsworkscm-2.5.4/types_aiobotocore_opsworkscm/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18749 2023-08-08 01:16:18.000000 types-aiobotocore-opsworkscm-2.5.4/types_aiobotocore_opsworkscm/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-08-08 01:16:16.000000 types-aiobotocore-opsworkscm-2.5.4/types_aiobotocore_opsworkscm/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1638 2023-08-08 01:16:16.000000 types-aiobotocore-opsworkscm-2.5.4/types_aiobotocore_opsworkscm/waiter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1637 2023-08-08 01:16:16.000000 types-aiobotocore-opsworkscm-2.5.4/types_aiobotocore_opsworkscm/waiter.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:24:11.254744 types-aiobotocore-opsworkscm-2.5.4/types_aiobotocore_opsworkscm.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    14206 2023-08-08 01:24:11.000000 types-aiobotocore-opsworkscm-2.5.4/types_aiobotocore_opsworkscm.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      949 2023-08-08 01:24:11.000000 types-aiobotocore-opsworkscm-2.5.4/types_aiobotocore_opsworkscm.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 01:24:11.000000 types-aiobotocore-opsworkscm-2.5.4/types_aiobotocore_opsworkscm.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 01:24:11.000000 types-aiobotocore-opsworkscm-2.5.4/types_aiobotocore_opsworkscm.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-08 01:24:11.000000 types-aiobotocore-opsworkscm-2.5.4/types_aiobotocore_opsworkscm.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-08-08 01:24:11.000000 types-aiobotocore-opsworkscm-2.5.4/types_aiobotocore_opsworkscm.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-opsworkscm-2.5.2.post2/LICENSE` & `types-aiobotocore-opsworkscm-2.5.4/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-opsworkscm-2.5.2.post2/PKG-INFO` & `types-aiobotocore-opsworkscm-2.5.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-opsworkscm
-Version: 2.5.2.post2
-Summary: Type annotations for aiobotocore.OpsWorksCM 2.5.2 service generated with mypy-boto3-builder 7.17.2
+Version: 2.5.4
+Summary: Type annotations for aiobotocore.OpsWorksCM 2.5.4 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_opsworkscm/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-opsworkscm.svg?color=blue)](https://pypi.org/project/types-aiobotocore-opsworkscm)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_opsworkscm/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-opsworkscm)](https://pepy.tech/project/types-aiobotocore-opsworkscm)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.OpsWorksCM 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opsworkscm.html#OpsWorksCM)
+[aiobotocore.OpsWorksCM 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opsworkscm.html#OpsWorksCM)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-opsworkscm-2.5.2.post2/README.md` & `types-aiobotocore-opsworkscm-2.5.4/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-opsworkscm.svg?color=blue)](https://pypi.org/project/types-aiobotocore-opsworkscm)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_opsworkscm/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-opsworkscm)](https://pepy.tech/project/types-aiobotocore-opsworkscm)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.OpsWorksCM 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opsworkscm.html#OpsWorksCM)
+[aiobotocore.OpsWorksCM 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opsworkscm.html#OpsWorksCM)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-opsworkscm-2.5.2.post2/setup.py` & `types-aiobotocore-opsworkscm-2.5.4/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-opsworkscm",
-    version="2.5.2.post2",
+    version="2.5.4",
     packages=["types_aiobotocore_opsworkscm"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.OpsWorksCM 2.5.2 service generated with"
+        "Type annotations for aiobotocore.OpsWorksCM 2.5.4 service generated with"
         " mypy-boto3-builder 7.17.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
```

### Comparing `types-aiobotocore-opsworkscm-2.5.2.post2/types_aiobotocore_opsworkscm/__init__.py` & `types-aiobotocore-opsworkscm-2.5.4/types_aiobotocore_opsworkscm/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-opsworkscm-2.5.2.post2/types_aiobotocore_opsworkscm/__init__.pyi` & `types-aiobotocore-opsworkscm-2.5.4/types_aiobotocore_opsworkscm/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-opsworkscm-2.5.2.post2/types_aiobotocore_opsworkscm/__main__.py` & `types-aiobotocore-opsworkscm-2.5.4/types_aiobotocore_opsworkscm/__main__.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.OpsWorksCM 2.5.2\nVersion:         2.5.2.post2\nBuilder"
+        "Type annotations for aiobotocore.OpsWorksCM 2.5.4\nVersion:         2.5.4\nBuilder"
         " version: 7.17.2\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_opsworkscm//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opsworkscm.html#OpsWorksCM\nOther"
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

### Comparing `types-aiobotocore-opsworkscm-2.5.2.post2/types_aiobotocore_opsworkscm/client.py` & `types-aiobotocore-opsworkscm-2.5.4/types_aiobotocore_opsworkscm/client.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-opsworkscm-2.5.2.post2/types_aiobotocore_opsworkscm/client.pyi` & `types-aiobotocore-opsworkscm-2.5.4/types_aiobotocore_opsworkscm/client.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-opsworkscm-2.5.2.post2/types_aiobotocore_opsworkscm/literals.py` & `types-aiobotocore-opsworkscm-2.5.4/types_aiobotocore_opsworkscm/literals.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-opsworkscm-2.5.2.post2/types_aiobotocore_opsworkscm/literals.pyi` & `types-aiobotocore-opsworkscm-2.5.4/types_aiobotocore_opsworkscm/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-opsworkscm-2.5.2.post2/types_aiobotocore_opsworkscm/paginator.py` & `types-aiobotocore-opsworkscm-2.5.4/types_aiobotocore_opsworkscm/paginator.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-opsworkscm-2.5.2.post2/types_aiobotocore_opsworkscm/paginator.pyi` & `types-aiobotocore-opsworkscm-2.5.4/types_aiobotocore_opsworkscm/paginator.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-opsworkscm-2.5.2.post2/types_aiobotocore_opsworkscm/type_defs.py` & `types-aiobotocore-opsworkscm-2.5.4/types_aiobotocore_opsworkscm/type_defs.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-opsworkscm-2.5.2.post2/types_aiobotocore_opsworkscm/type_defs.pyi` & `types-aiobotocore-opsworkscm-2.5.4/types_aiobotocore_opsworkscm/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-opsworkscm-2.5.2.post2/types_aiobotocore_opsworkscm/waiter.py` & `types-aiobotocore-opsworkscm-2.5.4/types_aiobotocore_opsworkscm/waiter.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-opsworkscm-2.5.2.post2/types_aiobotocore_opsworkscm/waiter.pyi` & `types-aiobotocore-opsworkscm-2.5.4/types_aiobotocore_opsworkscm/waiter.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-opsworkscm-2.5.2.post2/types_aiobotocore_opsworkscm.egg-info/PKG-INFO` & `types-aiobotocore-opsworkscm-2.5.4/types_aiobotocore_opsworkscm.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-opsworkscm
-Version: 2.5.2.post2
-Summary: Type annotations for aiobotocore.OpsWorksCM 2.5.2 service generated with mypy-boto3-builder 7.17.2
+Version: 2.5.4
+Summary: Type annotations for aiobotocore.OpsWorksCM 2.5.4 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_opsworkscm/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-opsworkscm.svg?color=blue)](https://pypi.org/project/types-aiobotocore-opsworkscm)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_opsworkscm/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-opsworkscm)](https://pepy.tech/project/types-aiobotocore-opsworkscm)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.OpsWorksCM 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opsworkscm.html#OpsWorksCM)
+[aiobotocore.OpsWorksCM 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opsworkscm.html#OpsWorksCM)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-opsworkscm-2.5.2.post2/types_aiobotocore_opsworkscm.egg-info/SOURCES.txt` & `types-aiobotocore-opsworkscm-2.5.4/types_aiobotocore_opsworkscm.egg-info/SOURCES.txt`

 * *Files identical despite different names*


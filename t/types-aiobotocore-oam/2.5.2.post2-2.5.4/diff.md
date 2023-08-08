# Comparing `tmp/types-aiobotocore-oam-2.5.2.post2.tar.gz` & `tmp/types-aiobotocore-oam-2.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-oam-2.5.2.post2.tar", last modified: Fri Aug  4 13:59:19 2023, max compression
+gzip compressed data, was "types-aiobotocore-oam-2.5.4.tar", last modified: Tue Aug  8 01:24:10 2023, max compression
```

## Comparing `types-aiobotocore-oam-2.5.2.post2.tar` & `types-aiobotocore-oam-2.5.4.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:19.956643 types-aiobotocore-oam-2.5.2.post2/
--rw-r--r--   0 vlad      (1000) vlad      (1000)     1070 2023-08-04 13:45:48.000000 types-aiobotocore-oam-2.5.2.post2/LICENSE
--rw-r--r--   0 vlad      (1000) vlad      (1000)    13313 2023-08-04 13:59:19.956643 types-aiobotocore-oam-2.5.2.post2/PKG-INFO
--rw-r--r--   0 vlad      (1000) vlad      (1000)    11778 2023-08-04 13:45:48.000000 types-aiobotocore-oam-2.5.2.post2/README.md
--rw-r--r--   0 vlad      (1000) vlad      (1000)       38 2023-08-04 13:59:19.956643 types-aiobotocore-oam-2.5.2.post2/setup.cfg
--rw-r--r--   0 vlad      (1000) vlad      (1000)     2053 2023-08-04 13:45:47.000000 types-aiobotocore-oam-2.5.2.post2/setup.py
-drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:19.956643 types-aiobotocore-oam-2.5.2.post2/types_aiobotocore_oam/
--rw-r--r--   0 vlad      (1000) vlad      (1000)     1127 2023-08-04 13:45:48.000000 types-aiobotocore-oam-2.5.2.post2/types_aiobotocore_oam/__init__.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)     1126 2023-08-04 13:45:48.000000 types-aiobotocore-oam-2.5.2.post2/types_aiobotocore_oam/__init__.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)      982 2023-08-04 13:45:48.000000 types-aiobotocore-oam-2.5.2.post2/types_aiobotocore_oam/__main__.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)    14752 2023-08-04 13:45:48.000000 types-aiobotocore-oam-2.5.2.post2/types_aiobotocore_oam/client.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)    14725 2023-08-04 13:45:48.000000 types-aiobotocore-oam-2.5.2.post2/types_aiobotocore_oam/client.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)     8741 2023-08-04 13:45:48.000000 types-aiobotocore-oam-2.5.2.post2/types_aiobotocore_oam/literals.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)     8739 2023-08-04 13:45:48.000000 types-aiobotocore-oam-2.5.2.post2/types_aiobotocore_oam/literals.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)     4190 2023-08-04 13:45:48.000000 types-aiobotocore-oam-2.5.2.post2/types_aiobotocore_oam/paginator.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)     4185 2023-08-04 13:45:48.000000 types-aiobotocore-oam-2.5.2.post2/types_aiobotocore_oam/paginator.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:45:48.000000 types-aiobotocore-oam-2.5.2.post2/types_aiobotocore_oam/py.typed
--rw-r--r--   0 vlad      (1000) vlad      (1000)     9647 2023-08-04 13:45:48.000000 types-aiobotocore-oam-2.5.2.post2/types_aiobotocore_oam/type_defs.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)     9638 2023-08-04 13:45:48.000000 types-aiobotocore-oam-2.5.2.post2/types_aiobotocore_oam/type_defs.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)       65 2023-08-04 13:45:48.000000 types-aiobotocore-oam-2.5.2.post2/types_aiobotocore_oam/version.py
-drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:19.956643 types-aiobotocore-oam-2.5.2.post2/types_aiobotocore_oam.egg-info/
--rw-r--r--   0 vlad      (1000) vlad      (1000)    13313 2023-08-04 13:59:19.000000 types-aiobotocore-oam-2.5.2.post2/types_aiobotocore_oam.egg-info/PKG-INFO
--rw-r--r--   0 vlad      (1000) vlad      (1000)      737 2023-08-04 13:59:19.000000 types-aiobotocore-oam-2.5.2.post2/types_aiobotocore_oam.egg-info/SOURCES.txt
--rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:19.000000 types-aiobotocore-oam-2.5.2.post2/types_aiobotocore_oam.egg-info/dependency_links.txt
--rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:19.000000 types-aiobotocore-oam-2.5.2.post2/types_aiobotocore_oam.egg-info/not-zip-safe
--rw-r--r--   0 vlad      (1000) vlad      (1000)       52 2023-08-04 13:59:19.000000 types-aiobotocore-oam-2.5.2.post2/types_aiobotocore_oam.egg-info/requires.txt
--rw-r--r--   0 vlad      (1000) vlad      (1000)       22 2023-08-04 13:59:19.000000 types-aiobotocore-oam-2.5.2.post2/types_aiobotocore_oam.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:24:10.806743 types-aiobotocore-oam-2.5.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-08 01:16:00.000000 types-aiobotocore-oam-2.5.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    13307 2023-08-08 01:24:10.802744 types-aiobotocore-oam-2.5.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    11778 2023-08-08 01:16:00.000000 types-aiobotocore-oam-2.5.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-08 01:24:10.806743 types-aiobotocore-oam-2.5.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2047 2023-08-08 01:16:00.000000 types-aiobotocore-oam-2.5.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:24:10.802744 types-aiobotocore-oam-2.5.4/types_aiobotocore_oam/
+-rw-r--r--   0 runner    (1001) docker     (123)     1127 2023-08-08 01:16:00.000000 types-aiobotocore-oam-2.5.4/types_aiobotocore_oam/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1126 2023-08-08 01:16:00.000000 types-aiobotocore-oam-2.5.4/types_aiobotocore_oam/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      970 2023-08-08 01:16:00.000000 types-aiobotocore-oam-2.5.4/types_aiobotocore_oam/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14752 2023-08-08 01:16:00.000000 types-aiobotocore-oam-2.5.4/types_aiobotocore_oam/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14725 2023-08-08 01:16:00.000000 types-aiobotocore-oam-2.5.4/types_aiobotocore_oam/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8741 2023-08-08 01:16:01.000000 types-aiobotocore-oam-2.5.4/types_aiobotocore_oam/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8739 2023-08-08 01:16:01.000000 types-aiobotocore-oam-2.5.4/types_aiobotocore_oam/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     4190 2023-08-08 01:16:01.000000 types-aiobotocore-oam-2.5.4/types_aiobotocore_oam/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4185 2023-08-08 01:16:01.000000 types-aiobotocore-oam-2.5.4/types_aiobotocore_oam/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 01:16:00.000000 types-aiobotocore-oam-2.5.4/types_aiobotocore_oam/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     9647 2023-08-08 01:16:03.000000 types-aiobotocore-oam-2.5.4/types_aiobotocore_oam/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9638 2023-08-08 01:16:01.000000 types-aiobotocore-oam-2.5.4/types_aiobotocore_oam/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-08-08 01:16:00.000000 types-aiobotocore-oam-2.5.4/types_aiobotocore_oam/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:24:10.802744 types-aiobotocore-oam-2.5.4/types_aiobotocore_oam.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    13307 2023-08-08 01:24:10.000000 types-aiobotocore-oam-2.5.4/types_aiobotocore_oam.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      737 2023-08-08 01:24:10.000000 types-aiobotocore-oam-2.5.4/types_aiobotocore_oam.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 01:24:10.000000 types-aiobotocore-oam-2.5.4/types_aiobotocore_oam.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 01:24:10.000000 types-aiobotocore-oam-2.5.4/types_aiobotocore_oam.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-08 01:24:10.000000 types-aiobotocore-oam-2.5.4/types_aiobotocore_oam.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-08-08 01:24:10.000000 types-aiobotocore-oam-2.5.4/types_aiobotocore_oam.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-oam-2.5.2.post2/LICENSE` & `types-aiobotocore-oam-2.5.4/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-oam-2.5.2.post2/PKG-INFO` & `types-aiobotocore-oam-2.5.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-oam
-Version: 2.5.2.post2
-Summary: Type annotations for aiobotocore.CloudWatchObservabilityAccessManager 2.5.2 service generated with mypy-boto3-builder 7.17.2
+Version: 2.5.4
+Summary: Type annotations for aiobotocore.CloudWatchObservabilityAccessManager 2.5.4 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_oam/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-oam.svg?color=blue)](https://pypi.org/project/types-aiobotocore-oam)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_oam/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-oam)](https://pepy.tech/project/types-aiobotocore-oam)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.CloudWatchObservabilityAccessManager 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/oam.html#CloudWatchObservabilityAccessManager)
+[aiobotocore.CloudWatchObservabilityAccessManager 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/oam.html#CloudWatchObservabilityAccessManager)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-oam-2.5.2.post2/README.md` & `types-aiobotocore-oam-2.5.4/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-oam.svg?color=blue)](https://pypi.org/project/types-aiobotocore-oam)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_oam/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-oam)](https://pepy.tech/project/types-aiobotocore-oam)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.CloudWatchObservabilityAccessManager 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/oam.html#CloudWatchObservabilityAccessManager)
+[aiobotocore.CloudWatchObservabilityAccessManager 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/oam.html#CloudWatchObservabilityAccessManager)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-oam-2.5.2.post2/setup.py` & `types-aiobotocore-oam-2.5.4/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-oam",
-    version="2.5.2.post2",
+    version="2.5.4",
     packages=["types_aiobotocore_oam"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.CloudWatchObservabilityAccessManager 2.5.2 service"
+        "Type annotations for aiobotocore.CloudWatchObservabilityAccessManager 2.5.4 service"
         " generated with mypy-boto3-builder 7.17.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
```

### Comparing `types-aiobotocore-oam-2.5.2.post2/types_aiobotocore_oam/__init__.py` & `types-aiobotocore-oam-2.5.4/types_aiobotocore_oam/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-oam-2.5.2.post2/types_aiobotocore_oam/__init__.pyi` & `types-aiobotocore-oam-2.5.4/types_aiobotocore_oam/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-oam-2.5.2.post2/types_aiobotocore_oam/__main__.py` & `types-aiobotocore-oam-2.5.4/types_aiobotocore_oam/__main__.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.CloudWatchObservabilityAccessManager 2.5.2\nVersion:     "
-        "    2.5.2.post2\nBuilder version: 7.17.2\nDocs:           "
+        "Type annotations for aiobotocore.CloudWatchObservabilityAccessManager 2.5.4\nVersion:     "
+        "    2.5.4\nBuilder version: 7.17.2\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_oam//\nBoto3 docs:    "
         "  https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/oam.html#CloudWatchObservabilityAccessManager\nOther"
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

### Comparing `types-aiobotocore-oam-2.5.2.post2/types_aiobotocore_oam/client.py` & `types-aiobotocore-oam-2.5.4/types_aiobotocore_oam/client.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-oam-2.5.2.post2/types_aiobotocore_oam/client.pyi` & `types-aiobotocore-oam-2.5.4/types_aiobotocore_oam/client.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-oam-2.5.2.post2/types_aiobotocore_oam/literals.py` & `types-aiobotocore-oam-2.5.4/types_aiobotocore_oam/literals.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-oam-2.5.2.post2/types_aiobotocore_oam/literals.pyi` & `types-aiobotocore-oam-2.5.4/types_aiobotocore_oam/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-oam-2.5.2.post2/types_aiobotocore_oam/paginator.py` & `types-aiobotocore-oam-2.5.4/types_aiobotocore_oam/paginator.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-oam-2.5.2.post2/types_aiobotocore_oam/paginator.pyi` & `types-aiobotocore-oam-2.5.4/types_aiobotocore_oam/paginator.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-oam-2.5.2.post2/types_aiobotocore_oam/type_defs.py` & `types-aiobotocore-oam-2.5.4/types_aiobotocore_oam/type_defs.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-oam-2.5.2.post2/types_aiobotocore_oam/type_defs.pyi` & `types-aiobotocore-oam-2.5.4/types_aiobotocore_oam/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-oam-2.5.2.post2/types_aiobotocore_oam.egg-info/PKG-INFO` & `types-aiobotocore-oam-2.5.4/types_aiobotocore_oam.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-oam
-Version: 2.5.2.post2
-Summary: Type annotations for aiobotocore.CloudWatchObservabilityAccessManager 2.5.2 service generated with mypy-boto3-builder 7.17.2
+Version: 2.5.4
+Summary: Type annotations for aiobotocore.CloudWatchObservabilityAccessManager 2.5.4 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_oam/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-oam.svg?color=blue)](https://pypi.org/project/types-aiobotocore-oam)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_oam/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-oam)](https://pepy.tech/project/types-aiobotocore-oam)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.CloudWatchObservabilityAccessManager 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/oam.html#CloudWatchObservabilityAccessManager)
+[aiobotocore.CloudWatchObservabilityAccessManager 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/oam.html#CloudWatchObservabilityAccessManager)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-oam-2.5.2.post2/types_aiobotocore_oam.egg-info/SOURCES.txt` & `types-aiobotocore-oam-2.5.4/types_aiobotocore_oam.egg-info/SOURCES.txt`

 * *Files identical despite different names*


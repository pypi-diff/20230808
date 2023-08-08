# Comparing `tmp/types-aiobotocore-securitylake-2.5.2.post2.tar.gz` & `tmp/types-aiobotocore-securitylake-2.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-securitylake-2.5.2.post2.tar", last modified: Fri Aug  4 13:59:25 2023, max compression
+gzip compressed data, was "types-aiobotocore-securitylake-2.5.4.tar", last modified: Tue Aug  8 01:24:25 2023, max compression
```

## Comparing `types-aiobotocore-securitylake-2.5.2.post2.tar` & `types-aiobotocore-securitylake-2.5.4.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:25.846643 types-aiobotocore-securitylake-2.5.2.post2/
--rw-r--r--   0 vlad      (1000) vlad      (1000)     1070 2023-08-04 13:53:07.000000 types-aiobotocore-securitylake-2.5.2.post2/LICENSE
--rw-r--r--   0 vlad      (1000) vlad      (1000)    13657 2023-08-04 13:59:25.846643 types-aiobotocore-securitylake-2.5.2.post2/PKG-INFO
--rw-r--r--   0 vlad      (1000) vlad      (1000)    12119 2023-08-04 13:53:07.000000 types-aiobotocore-securitylake-2.5.2.post2/README.md
--rw-r--r--   0 vlad      (1000) vlad      (1000)       38 2023-08-04 13:59:25.846643 types-aiobotocore-securitylake-2.5.2.post2/setup.cfg
--rw-r--r--   0 vlad      (1000) vlad      (1000)     2107 2023-08-04 13:53:07.000000 types-aiobotocore-securitylake-2.5.2.post2/setup.py
-drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:25.846643 types-aiobotocore-securitylake-2.5.2.post2/types_aiobotocore_securitylake/
--rw-r--r--   0 vlad      (1000) vlad      (1000)     1369 2023-08-04 13:53:07.000000 types-aiobotocore-securitylake-2.5.2.post2/types_aiobotocore_securitylake/__init__.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)     1368 2023-08-04 13:53:07.000000 types-aiobotocore-securitylake-2.5.2.post2/types_aiobotocore_securitylake/__init__.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)      963 2023-08-04 13:53:07.000000 types-aiobotocore-securitylake-2.5.2.post2/types_aiobotocore_securitylake/__main__.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)    27925 2023-08-04 13:53:07.000000 types-aiobotocore-securitylake-2.5.2.post2/types_aiobotocore_securitylake/client.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)    27881 2023-08-04 13:53:07.000000 types-aiobotocore-securitylake-2.5.2.post2/types_aiobotocore_securitylake/client.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)     9101 2023-08-04 13:53:08.000000 types-aiobotocore-securitylake-2.5.2.post2/types_aiobotocore_securitylake/literals.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)     9099 2023-08-04 13:53:08.000000 types-aiobotocore-securitylake-2.5.2.post2/types_aiobotocore_securitylake/literals.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)     5746 2023-08-04 13:53:07.000000 types-aiobotocore-securitylake-2.5.2.post2/types_aiobotocore_securitylake/paginator.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)     5740 2023-08-04 13:53:07.000000 types-aiobotocore-securitylake-2.5.2.post2/types_aiobotocore_securitylake/paginator.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:53:07.000000 types-aiobotocore-securitylake-2.5.2.post2/types_aiobotocore_securitylake/py.typed
--rw-r--r--   0 vlad      (1000) vlad      (1000)    25502 2023-08-04 13:53:08.000000 types-aiobotocore-securitylake-2.5.2.post2/types_aiobotocore_securitylake/type_defs.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)    25477 2023-08-04 13:53:08.000000 types-aiobotocore-securitylake-2.5.2.post2/types_aiobotocore_securitylake/type_defs.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)       65 2023-08-04 13:53:07.000000 types-aiobotocore-securitylake-2.5.2.post2/types_aiobotocore_securitylake/version.py
-drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:25.846643 types-aiobotocore-securitylake-2.5.2.post2/types_aiobotocore_securitylake.egg-info/
--rw-r--r--   0 vlad      (1000) vlad      (1000)    13657 2023-08-04 13:59:25.000000 types-aiobotocore-securitylake-2.5.2.post2/types_aiobotocore_securitylake.egg-info/PKG-INFO
--rw-r--r--   0 vlad      (1000) vlad      (1000)      908 2023-08-04 13:59:25.000000 types-aiobotocore-securitylake-2.5.2.post2/types_aiobotocore_securitylake.egg-info/SOURCES.txt
--rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:25.000000 types-aiobotocore-securitylake-2.5.2.post2/types_aiobotocore_securitylake.egg-info/dependency_links.txt
--rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:25.000000 types-aiobotocore-securitylake-2.5.2.post2/types_aiobotocore_securitylake.egg-info/not-zip-safe
--rw-r--r--   0 vlad      (1000) vlad      (1000)       52 2023-08-04 13:59:25.000000 types-aiobotocore-securitylake-2.5.2.post2/types_aiobotocore_securitylake.egg-info/requires.txt
--rw-r--r--   0 vlad      (1000) vlad      (1000)       31 2023-08-04 13:59:25.000000 types-aiobotocore-securitylake-2.5.2.post2/types_aiobotocore_securitylake.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:24:25.238778 types-aiobotocore-securitylake-2.5.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-08 01:20:53.000000 types-aiobotocore-securitylake-2.5.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    13651 2023-08-08 01:24:25.234778 types-aiobotocore-securitylake-2.5.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    12119 2023-08-08 01:20:53.000000 types-aiobotocore-securitylake-2.5.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-08 01:24:25.238778 types-aiobotocore-securitylake-2.5.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2101 2023-08-08 01:20:53.000000 types-aiobotocore-securitylake-2.5.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:24:25.226778 types-aiobotocore-securitylake-2.5.4/types_aiobotocore_securitylake/
+-rw-r--r--   0 runner    (1001) docker     (123)     1369 2023-08-08 01:20:53.000000 types-aiobotocore-securitylake-2.5.4/types_aiobotocore_securitylake/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1368 2023-08-08 01:20:53.000000 types-aiobotocore-securitylake-2.5.4/types_aiobotocore_securitylake/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      951 2023-08-08 01:20:53.000000 types-aiobotocore-securitylake-2.5.4/types_aiobotocore_securitylake/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27925 2023-08-08 01:20:53.000000 types-aiobotocore-securitylake-2.5.4/types_aiobotocore_securitylake/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27881 2023-08-08 01:20:53.000000 types-aiobotocore-securitylake-2.5.4/types_aiobotocore_securitylake/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9101 2023-08-08 01:20:53.000000 types-aiobotocore-securitylake-2.5.4/types_aiobotocore_securitylake/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9099 2023-08-08 01:20:53.000000 types-aiobotocore-securitylake-2.5.4/types_aiobotocore_securitylake/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     5746 2023-08-08 01:20:53.000000 types-aiobotocore-securitylake-2.5.4/types_aiobotocore_securitylake/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5740 2023-08-08 01:20:53.000000 types-aiobotocore-securitylake-2.5.4/types_aiobotocore_securitylake/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 01:20:53.000000 types-aiobotocore-securitylake-2.5.4/types_aiobotocore_securitylake/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    25502 2023-08-08 01:20:54.000000 types-aiobotocore-securitylake-2.5.4/types_aiobotocore_securitylake/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25477 2023-08-08 01:20:53.000000 types-aiobotocore-securitylake-2.5.4/types_aiobotocore_securitylake/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-08-08 01:20:53.000000 types-aiobotocore-securitylake-2.5.4/types_aiobotocore_securitylake/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:24:25.234778 types-aiobotocore-securitylake-2.5.4/types_aiobotocore_securitylake.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    13651 2023-08-08 01:24:25.000000 types-aiobotocore-securitylake-2.5.4/types_aiobotocore_securitylake.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      908 2023-08-08 01:24:25.000000 types-aiobotocore-securitylake-2.5.4/types_aiobotocore_securitylake.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 01:24:25.000000 types-aiobotocore-securitylake-2.5.4/types_aiobotocore_securitylake.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 01:24:25.000000 types-aiobotocore-securitylake-2.5.4/types_aiobotocore_securitylake.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-08 01:24:25.000000 types-aiobotocore-securitylake-2.5.4/types_aiobotocore_securitylake.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-08-08 01:24:25.000000 types-aiobotocore-securitylake-2.5.4/types_aiobotocore_securitylake.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-securitylake-2.5.2.post2/LICENSE` & `types-aiobotocore-securitylake-2.5.4/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-securitylake-2.5.2.post2/PKG-INFO` & `types-aiobotocore-securitylake-2.5.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-securitylake
-Version: 2.5.2.post2
-Summary: Type annotations for aiobotocore.SecurityLake 2.5.2 service generated with mypy-boto3-builder 7.17.2
+Version: 2.5.4
+Summary: Type annotations for aiobotocore.SecurityLake 2.5.4 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_securitylake/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-securitylake.svg?color=blue)](https://pypi.org/project/types-aiobotocore-securitylake)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_securitylake/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-securitylake)](https://pepy.tech/project/types-aiobotocore-securitylake)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.SecurityLake 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securitylake.html#SecurityLake)
+[aiobotocore.SecurityLake 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securitylake.html#SecurityLake)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-securitylake-2.5.2.post2/README.md` & `types-aiobotocore-securitylake-2.5.4/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-securitylake.svg?color=blue)](https://pypi.org/project/types-aiobotocore-securitylake)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_securitylake/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-securitylake)](https://pepy.tech/project/types-aiobotocore-securitylake)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.SecurityLake 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securitylake.html#SecurityLake)
+[aiobotocore.SecurityLake 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securitylake.html#SecurityLake)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-securitylake-2.5.2.post2/setup.py` & `types-aiobotocore-securitylake-2.5.4/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-securitylake",
-    version="2.5.2.post2",
+    version="2.5.4",
     packages=["types_aiobotocore_securitylake"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.SecurityLake 2.5.2 service generated with"
+        "Type annotations for aiobotocore.SecurityLake 2.5.4 service generated with"
         " mypy-boto3-builder 7.17.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
```

### Comparing `types-aiobotocore-securitylake-2.5.2.post2/types_aiobotocore_securitylake/__init__.py` & `types-aiobotocore-securitylake-2.5.4/types_aiobotocore_securitylake/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-securitylake-2.5.2.post2/types_aiobotocore_securitylake/__init__.pyi` & `types-aiobotocore-securitylake-2.5.4/types_aiobotocore_securitylake/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-securitylake-2.5.2.post2/types_aiobotocore_securitylake/__main__.py` & `types-aiobotocore-securitylake-2.5.4/types_aiobotocore_securitylake/__main__.py`

 * *Files 10% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.SecurityLake 2.5.2\nVersion:         2.5.2.post2\nBuilder"
+        "Type annotations for aiobotocore.SecurityLake 2.5.4\nVersion:         2.5.4\nBuilder"
         " version: 7.17.2\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_securitylake//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securitylake.html#SecurityLake\nOther"
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

### Comparing `types-aiobotocore-securitylake-2.5.2.post2/types_aiobotocore_securitylake/client.py` & `types-aiobotocore-securitylake-2.5.4/types_aiobotocore_securitylake/client.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-securitylake-2.5.2.post2/types_aiobotocore_securitylake/client.pyi` & `types-aiobotocore-securitylake-2.5.4/types_aiobotocore_securitylake/client.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-securitylake-2.5.2.post2/types_aiobotocore_securitylake/literals.py` & `types-aiobotocore-securitylake-2.5.4/types_aiobotocore_securitylake/literals.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-securitylake-2.5.2.post2/types_aiobotocore_securitylake/literals.pyi` & `types-aiobotocore-securitylake-2.5.4/types_aiobotocore_securitylake/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-securitylake-2.5.2.post2/types_aiobotocore_securitylake/paginator.py` & `types-aiobotocore-securitylake-2.5.4/types_aiobotocore_securitylake/paginator.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-securitylake-2.5.2.post2/types_aiobotocore_securitylake/paginator.pyi` & `types-aiobotocore-securitylake-2.5.4/types_aiobotocore_securitylake/paginator.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-securitylake-2.5.2.post2/types_aiobotocore_securitylake/type_defs.py` & `types-aiobotocore-securitylake-2.5.4/types_aiobotocore_securitylake/type_defs.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-securitylake-2.5.2.post2/types_aiobotocore_securitylake/type_defs.pyi` & `types-aiobotocore-securitylake-2.5.4/types_aiobotocore_securitylake/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-securitylake-2.5.2.post2/types_aiobotocore_securitylake.egg-info/PKG-INFO` & `types-aiobotocore-securitylake-2.5.4/types_aiobotocore_securitylake.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-securitylake
-Version: 2.5.2.post2
-Summary: Type annotations for aiobotocore.SecurityLake 2.5.2 service generated with mypy-boto3-builder 7.17.2
+Version: 2.5.4
+Summary: Type annotations for aiobotocore.SecurityLake 2.5.4 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_securitylake/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-securitylake.svg?color=blue)](https://pypi.org/project/types-aiobotocore-securitylake)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_securitylake/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-securitylake)](https://pepy.tech/project/types-aiobotocore-securitylake)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.SecurityLake 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securitylake.html#SecurityLake)
+[aiobotocore.SecurityLake 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securitylake.html#SecurityLake)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-securitylake-2.5.2.post2/types_aiobotocore_securitylake.egg-info/SOURCES.txt` & `types-aiobotocore-securitylake-2.5.4/types_aiobotocore_securitylake.egg-info/SOURCES.txt`

 * *Files identical despite different names*


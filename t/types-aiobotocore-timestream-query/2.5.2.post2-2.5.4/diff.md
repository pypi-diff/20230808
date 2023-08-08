# Comparing `tmp/types-aiobotocore-timestream-query-2.5.2.post2.tar.gz` & `tmp/types-aiobotocore-timestream-query-2.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-timestream-query-2.5.2.post2.tar", last modified: Fri Aug  4 13:59:28 2023, max compression
+gzip compressed data, was "types-aiobotocore-timestream-query-2.5.4.tar", last modified: Tue Aug  8 01:24:32 2023, max compression
```

## Comparing `types-aiobotocore-timestream-query-2.5.2.post2.tar` & `types-aiobotocore-timestream-query-2.5.4.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:28.636643 types-aiobotocore-timestream-query-2.5.2.post2/
--rw-r--r--   0 vlad      (1000) vlad      (1000)     1070 2023-08-04 13:55:03.000000 types-aiobotocore-timestream-query-2.5.2.post2/LICENSE
--rw-r--r--   0 vlad      (1000) vlad      (1000)    13750 2023-08-04 13:59:28.636643 types-aiobotocore-timestream-query-2.5.2.post2/PKG-INFO
--rw-r--r--   0 vlad      (1000) vlad      (1000)    12197 2023-08-04 13:55:03.000000 types-aiobotocore-timestream-query-2.5.2.post2/README.md
--rw-r--r--   0 vlad      (1000) vlad      (1000)       38 2023-08-04 13:59:28.636643 types-aiobotocore-timestream-query-2.5.2.post2/setup.cfg
--rw-r--r--   0 vlad      (1000) vlad      (1000)     2134 2023-08-04 13:55:03.000000 types-aiobotocore-timestream-query-2.5.2.post2/setup.py
-drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:28.636643 types-aiobotocore-timestream-query-2.5.2.post2/types_aiobotocore_timestream_query/
--rw-r--r--   0 vlad      (1000) vlad      (1000)     1117 2023-08-04 13:55:03.000000 types-aiobotocore-timestream-query-2.5.2.post2/types_aiobotocore_timestream_query/__init__.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)     1116 2023-08-04 13:55:03.000000 types-aiobotocore-timestream-query-2.5.2.post2/types_aiobotocore_timestream_query/__init__.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)      977 2023-08-04 13:55:03.000000 types-aiobotocore-timestream-query-2.5.2.post2/types_aiobotocore_timestream_query/__main__.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)    14504 2023-08-04 13:55:03.000000 types-aiobotocore-timestream-query-2.5.2.post2/types_aiobotocore_timestream_query/client.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)    14479 2023-08-04 13:55:03.000000 types-aiobotocore-timestream-query-2.5.2.post2/types_aiobotocore_timestream_query/client.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)     8978 2023-08-04 13:55:04.000000 types-aiobotocore-timestream-query-2.5.2.post2/types_aiobotocore_timestream_query/literals.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)     8976 2023-08-04 13:55:03.000000 types-aiobotocore-timestream-query-2.5.2.post2/types_aiobotocore_timestream_query/literals.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)     4436 2023-08-04 13:55:03.000000 types-aiobotocore-timestream-query-2.5.2.post2/types_aiobotocore_timestream_query/paginator.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)     4431 2023-08-04 13:55:03.000000 types-aiobotocore-timestream-query-2.5.2.post2/types_aiobotocore_timestream_query/paginator.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:55:03.000000 types-aiobotocore-timestream-query-2.5.2.post2/types_aiobotocore_timestream_query/py.typed
--rw-r--r--   0 vlad      (1000) vlad      (1000)    19511 2023-08-04 13:55:04.000000 types-aiobotocore-timestream-query-2.5.2.post2/types_aiobotocore_timestream_query/type_defs.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)    19480 2023-08-04 13:55:04.000000 types-aiobotocore-timestream-query-2.5.2.post2/types_aiobotocore_timestream_query/type_defs.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)       65 2023-08-04 13:55:03.000000 types-aiobotocore-timestream-query-2.5.2.post2/types_aiobotocore_timestream_query/version.py
-drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:28.636643 types-aiobotocore-timestream-query-2.5.2.post2/types_aiobotocore_timestream_query.egg-info/
--rw-r--r--   0 vlad      (1000) vlad      (1000)    13750 2023-08-04 13:59:28.000000 types-aiobotocore-timestream-query-2.5.2.post2/types_aiobotocore_timestream_query.egg-info/PKG-INFO
--rw-r--r--   0 vlad      (1000) vlad      (1000)      984 2023-08-04 13:59:28.000000 types-aiobotocore-timestream-query-2.5.2.post2/types_aiobotocore_timestream_query.egg-info/SOURCES.txt
--rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:28.000000 types-aiobotocore-timestream-query-2.5.2.post2/types_aiobotocore_timestream_query.egg-info/dependency_links.txt
--rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:28.000000 types-aiobotocore-timestream-query-2.5.2.post2/types_aiobotocore_timestream_query.egg-info/not-zip-safe
--rw-r--r--   0 vlad      (1000) vlad      (1000)       52 2023-08-04 13:59:28.000000 types-aiobotocore-timestream-query-2.5.2.post2/types_aiobotocore_timestream_query.egg-info/requires.txt
--rw-r--r--   0 vlad      (1000) vlad      (1000)       35 2023-08-04 13:59:28.000000 types-aiobotocore-timestream-query-2.5.2.post2/types_aiobotocore_timestream_query.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:24:32.514796 types-aiobotocore-timestream-query-2.5.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-08 01:21:59.000000 types-aiobotocore-timestream-query-2.5.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    13744 2023-08-08 01:24:32.514796 types-aiobotocore-timestream-query-2.5.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    12197 2023-08-08 01:21:59.000000 types-aiobotocore-timestream-query-2.5.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-08 01:24:32.514796 types-aiobotocore-timestream-query-2.5.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2128 2023-08-08 01:21:59.000000 types-aiobotocore-timestream-query-2.5.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:24:32.514796 types-aiobotocore-timestream-query-2.5.4/types_aiobotocore_timestream_query/
+-rw-r--r--   0 runner    (1001) docker     (123)     1117 2023-08-08 01:21:59.000000 types-aiobotocore-timestream-query-2.5.4/types_aiobotocore_timestream_query/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1116 2023-08-08 01:21:59.000000 types-aiobotocore-timestream-query-2.5.4/types_aiobotocore_timestream_query/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      965 2023-08-08 01:21:59.000000 types-aiobotocore-timestream-query-2.5.4/types_aiobotocore_timestream_query/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14504 2023-08-08 01:21:59.000000 types-aiobotocore-timestream-query-2.5.4/types_aiobotocore_timestream_query/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14479 2023-08-08 01:21:59.000000 types-aiobotocore-timestream-query-2.5.4/types_aiobotocore_timestream_query/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8978 2023-08-08 01:21:59.000000 types-aiobotocore-timestream-query-2.5.4/types_aiobotocore_timestream_query/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8976 2023-08-08 01:21:59.000000 types-aiobotocore-timestream-query-2.5.4/types_aiobotocore_timestream_query/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     4436 2023-08-08 01:21:59.000000 types-aiobotocore-timestream-query-2.5.4/types_aiobotocore_timestream_query/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4431 2023-08-08 01:21:59.000000 types-aiobotocore-timestream-query-2.5.4/types_aiobotocore_timestream_query/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 01:21:59.000000 types-aiobotocore-timestream-query-2.5.4/types_aiobotocore_timestream_query/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    19511 2023-08-08 01:22:00.000000 types-aiobotocore-timestream-query-2.5.4/types_aiobotocore_timestream_query/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19480 2023-08-08 01:22:00.000000 types-aiobotocore-timestream-query-2.5.4/types_aiobotocore_timestream_query/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-08-08 01:21:59.000000 types-aiobotocore-timestream-query-2.5.4/types_aiobotocore_timestream_query/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:24:32.514796 types-aiobotocore-timestream-query-2.5.4/types_aiobotocore_timestream_query.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    13744 2023-08-08 01:24:32.000000 types-aiobotocore-timestream-query-2.5.4/types_aiobotocore_timestream_query.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      984 2023-08-08 01:24:32.000000 types-aiobotocore-timestream-query-2.5.4/types_aiobotocore_timestream_query.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 01:24:32.000000 types-aiobotocore-timestream-query-2.5.4/types_aiobotocore_timestream_query.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 01:24:32.000000 types-aiobotocore-timestream-query-2.5.4/types_aiobotocore_timestream_query.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-08 01:24:32.000000 types-aiobotocore-timestream-query-2.5.4/types_aiobotocore_timestream_query.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-08-08 01:24:32.000000 types-aiobotocore-timestream-query-2.5.4/types_aiobotocore_timestream_query.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-timestream-query-2.5.2.post2/LICENSE` & `types-aiobotocore-timestream-query-2.5.4/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-timestream-query-2.5.2.post2/PKG-INFO` & `types-aiobotocore-timestream-query-2.5.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-timestream-query
-Version: 2.5.2.post2
-Summary: Type annotations for aiobotocore.TimestreamQuery 2.5.2 service generated with mypy-boto3-builder 7.17.2
+Version: 2.5.4
+Summary: Type annotations for aiobotocore.TimestreamQuery 2.5.4 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_timestream_query/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-timestream-query.svg?color=blue)](https://pypi.org/project/types-aiobotocore-timestream-query)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_timestream_query/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-timestream-query)](https://pepy.tech/project/types-aiobotocore-timestream-query)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.TimestreamQuery 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/timestream-query.html#TimestreamQuery)
+[aiobotocore.TimestreamQuery 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/timestream-query.html#TimestreamQuery)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-timestream-query-2.5.2.post2/README.md` & `types-aiobotocore-timestream-query-2.5.4/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-timestream-query.svg?color=blue)](https://pypi.org/project/types-aiobotocore-timestream-query)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_timestream_query/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-timestream-query)](https://pepy.tech/project/types-aiobotocore-timestream-query)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.TimestreamQuery 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/timestream-query.html#TimestreamQuery)
+[aiobotocore.TimestreamQuery 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/timestream-query.html#TimestreamQuery)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-timestream-query-2.5.2.post2/setup.py` & `types-aiobotocore-timestream-query-2.5.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-timestream-query",
-    version="2.5.2.post2",
+    version="2.5.4",
     packages=["types_aiobotocore_timestream_query"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.TimestreamQuery 2.5.2 service generated with"
+        "Type annotations for aiobotocore.TimestreamQuery 2.5.4 service generated with"
         " mypy-boto3-builder 7.17.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
```

### Comparing `types-aiobotocore-timestream-query-2.5.2.post2/types_aiobotocore_timestream_query/__init__.py` & `types-aiobotocore-timestream-query-2.5.4/types_aiobotocore_timestream_query/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-timestream-query-2.5.2.post2/types_aiobotocore_timestream_query/__init__.pyi` & `types-aiobotocore-timestream-query-2.5.4/types_aiobotocore_timestream_query/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-timestream-query-2.5.2.post2/types_aiobotocore_timestream_query/__main__.py` & `types-aiobotocore-timestream-query-2.5.4/types_aiobotocore_timestream_query/__main__.py`

 * *Files 13% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.TimestreamQuery 2.5.2\nVersion:        "
-        " 2.5.2.post2\nBuilder version: 7.17.2\nDocs:           "
+        "Type annotations for aiobotocore.TimestreamQuery 2.5.4\nVersion:         2.5.4\nBuilder"
+        " version: 7.17.2\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_timestream_query//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/timestream-query.html#TimestreamQuery\nOther"
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

### Comparing `types-aiobotocore-timestream-query-2.5.2.post2/types_aiobotocore_timestream_query/client.py` & `types-aiobotocore-timestream-query-2.5.4/types_aiobotocore_timestream_query/client.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-timestream-query-2.5.2.post2/types_aiobotocore_timestream_query/client.pyi` & `types-aiobotocore-timestream-query-2.5.4/types_aiobotocore_timestream_query/client.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-timestream-query-2.5.2.post2/types_aiobotocore_timestream_query/literals.py` & `types-aiobotocore-timestream-query-2.5.4/types_aiobotocore_timestream_query/literals.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-timestream-query-2.5.2.post2/types_aiobotocore_timestream_query/literals.pyi` & `types-aiobotocore-timestream-query-2.5.4/types_aiobotocore_timestream_query/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-timestream-query-2.5.2.post2/types_aiobotocore_timestream_query/paginator.py` & `types-aiobotocore-timestream-query-2.5.4/types_aiobotocore_timestream_query/paginator.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-timestream-query-2.5.2.post2/types_aiobotocore_timestream_query/paginator.pyi` & `types-aiobotocore-timestream-query-2.5.4/types_aiobotocore_timestream_query/paginator.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-timestream-query-2.5.2.post2/types_aiobotocore_timestream_query/type_defs.py` & `types-aiobotocore-timestream-query-2.5.4/types_aiobotocore_timestream_query/type_defs.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-timestream-query-2.5.2.post2/types_aiobotocore_timestream_query/type_defs.pyi` & `types-aiobotocore-timestream-query-2.5.4/types_aiobotocore_timestream_query/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-timestream-query-2.5.2.post2/types_aiobotocore_timestream_query.egg-info/PKG-INFO` & `types-aiobotocore-timestream-query-2.5.4/types_aiobotocore_timestream_query.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-timestream-query
-Version: 2.5.2.post2
-Summary: Type annotations for aiobotocore.TimestreamQuery 2.5.2 service generated with mypy-boto3-builder 7.17.2
+Version: 2.5.4
+Summary: Type annotations for aiobotocore.TimestreamQuery 2.5.4 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_timestream_query/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-timestream-query.svg?color=blue)](https://pypi.org/project/types-aiobotocore-timestream-query)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_timestream_query/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-timestream-query)](https://pepy.tech/project/types-aiobotocore-timestream-query)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.TimestreamQuery 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/timestream-query.html#TimestreamQuery)
+[aiobotocore.TimestreamQuery 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/timestream-query.html#TimestreamQuery)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-timestream-query-2.5.2.post2/types_aiobotocore_timestream_query.egg-info/SOURCES.txt` & `types-aiobotocore-timestream-query-2.5.4/types_aiobotocore_timestream_query.egg-info/SOURCES.txt`

 * *Files identical despite different names*


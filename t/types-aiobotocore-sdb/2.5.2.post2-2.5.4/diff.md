# Comparing `tmp/types-aiobotocore-sdb-2.5.2.post2.tar.gz` & `tmp/types-aiobotocore-sdb-2.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-sdb-2.5.2.post2.tar", last modified: Fri Aug  4 13:59:25 2023, max compression
+gzip compressed data, was "types-aiobotocore-sdb-2.5.4.tar", last modified: Tue Aug  8 01:24:24 2023, max compression
```

## Comparing `types-aiobotocore-sdb-2.5.2.post2.tar` & `types-aiobotocore-sdb-2.5.4.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:25.716643 types-aiobotocore-sdb-2.5.2.post2/
--rw-r--r--   0 vlad      (1000) vlad      (1000)     1070 2023-08-04 13:52:41.000000 types-aiobotocore-sdb-2.5.2.post2/LICENSE
--rw-r--r--   0 vlad      (1000) vlad      (1000)    12794 2023-08-04 13:59:25.716643 types-aiobotocore-sdb-2.5.2.post2/PKG-INFO
--rw-r--r--   0 vlad      (1000) vlad      (1000)    11287 2023-08-04 13:52:41.000000 types-aiobotocore-sdb-2.5.2.post2/README.md
--rw-r--r--   0 vlad      (1000) vlad      (1000)       38 2023-08-04 13:59:25.716643 types-aiobotocore-sdb-2.5.2.post2/setup.cfg
--rw-r--r--   0 vlad      (1000) vlad      (1000)     2025 2023-08-04 13:52:41.000000 types-aiobotocore-sdb-2.5.2.post2/setup.py
-drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:25.716643 types-aiobotocore-sdb-2.5.2.post2/types_aiobotocore_sdb/
--rw-r--r--   0 vlad      (1000) vlad      (1000)      754 2023-08-04 13:52:41.000000 types-aiobotocore-sdb-2.5.2.post2/types_aiobotocore_sdb/__init__.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)      753 2023-08-04 13:52:41.000000 types-aiobotocore-sdb-2.5.2.post2/types_aiobotocore_sdb/__init__.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)      926 2023-08-04 13:52:41.000000 types-aiobotocore-sdb-2.5.2.post2/types_aiobotocore_sdb/__main__.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)    11703 2023-08-04 13:52:41.000000 types-aiobotocore-sdb-2.5.2.post2/types_aiobotocore_sdb/client.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)    11682 2023-08-04 13:52:41.000000 types-aiobotocore-sdb-2.5.2.post2/types_aiobotocore_sdb/client.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)     8032 2023-08-04 13:52:42.000000 types-aiobotocore-sdb-2.5.2.post2/types_aiobotocore_sdb/literals.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)     8030 2023-08-04 13:52:42.000000 types-aiobotocore-sdb-2.5.2.post2/types_aiobotocore_sdb/literals.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)     2923 2023-08-04 13:52:41.000000 types-aiobotocore-sdb-2.5.2.post2/types_aiobotocore_sdb/paginator.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)     2919 2023-08-04 13:52:41.000000 types-aiobotocore-sdb-2.5.2.post2/types_aiobotocore_sdb/paginator.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:52:41.000000 types-aiobotocore-sdb-2.5.2.post2/types_aiobotocore_sdb/py.typed
--rw-r--r--   0 vlad      (1000) vlad      (1000)     8650 2023-08-04 13:52:42.000000 types-aiobotocore-sdb-2.5.2.post2/types_aiobotocore_sdb/type_defs.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)     8631 2023-08-04 13:52:42.000000 types-aiobotocore-sdb-2.5.2.post2/types_aiobotocore_sdb/type_defs.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)       65 2023-08-04 13:52:41.000000 types-aiobotocore-sdb-2.5.2.post2/types_aiobotocore_sdb/version.py
-drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:25.716643 types-aiobotocore-sdb-2.5.2.post2/types_aiobotocore_sdb.egg-info/
--rw-r--r--   0 vlad      (1000) vlad      (1000)    12794 2023-08-04 13:59:25.000000 types-aiobotocore-sdb-2.5.2.post2/types_aiobotocore_sdb.egg-info/PKG-INFO
--rw-r--r--   0 vlad      (1000) vlad      (1000)      737 2023-08-04 13:59:25.000000 types-aiobotocore-sdb-2.5.2.post2/types_aiobotocore_sdb.egg-info/SOURCES.txt
--rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:25.000000 types-aiobotocore-sdb-2.5.2.post2/types_aiobotocore_sdb.egg-info/dependency_links.txt
--rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:25.000000 types-aiobotocore-sdb-2.5.2.post2/types_aiobotocore_sdb.egg-info/not-zip-safe
--rw-r--r--   0 vlad      (1000) vlad      (1000)       52 2023-08-04 13:59:25.000000 types-aiobotocore-sdb-2.5.2.post2/types_aiobotocore_sdb.egg-info/requires.txt
--rw-r--r--   0 vlad      (1000) vlad      (1000)       22 2023-08-04 13:59:25.000000 types-aiobotocore-sdb-2.5.2.post2/types_aiobotocore_sdb.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:24:24.922777 types-aiobotocore-sdb-2.5.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-08 01:20:35.000000 types-aiobotocore-sdb-2.5.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    12788 2023-08-08 01:24:24.914777 types-aiobotocore-sdb-2.5.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    11287 2023-08-08 01:20:35.000000 types-aiobotocore-sdb-2.5.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-08 01:24:24.922777 types-aiobotocore-sdb-2.5.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2019 2023-08-08 01:20:35.000000 types-aiobotocore-sdb-2.5.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:24:24.914777 types-aiobotocore-sdb-2.5.4/types_aiobotocore_sdb/
+-rw-r--r--   0 runner    (1001) docker     (123)      754 2023-08-08 01:20:35.000000 types-aiobotocore-sdb-2.5.4/types_aiobotocore_sdb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      753 2023-08-08 01:20:35.000000 types-aiobotocore-sdb-2.5.4/types_aiobotocore_sdb/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      914 2023-08-08 01:20:35.000000 types-aiobotocore-sdb-2.5.4/types_aiobotocore_sdb/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11703 2023-08-08 01:20:35.000000 types-aiobotocore-sdb-2.5.4/types_aiobotocore_sdb/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11682 2023-08-08 01:20:35.000000 types-aiobotocore-sdb-2.5.4/types_aiobotocore_sdb/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8032 2023-08-08 01:20:35.000000 types-aiobotocore-sdb-2.5.4/types_aiobotocore_sdb/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8030 2023-08-08 01:20:35.000000 types-aiobotocore-sdb-2.5.4/types_aiobotocore_sdb/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2923 2023-08-08 01:20:35.000000 types-aiobotocore-sdb-2.5.4/types_aiobotocore_sdb/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2919 2023-08-08 01:20:35.000000 types-aiobotocore-sdb-2.5.4/types_aiobotocore_sdb/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 01:20:35.000000 types-aiobotocore-sdb-2.5.4/types_aiobotocore_sdb/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     8650 2023-08-08 01:20:35.000000 types-aiobotocore-sdb-2.5.4/types_aiobotocore_sdb/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8631 2023-08-08 01:20:35.000000 types-aiobotocore-sdb-2.5.4/types_aiobotocore_sdb/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-08-08 01:20:35.000000 types-aiobotocore-sdb-2.5.4/types_aiobotocore_sdb/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:24:24.914777 types-aiobotocore-sdb-2.5.4/types_aiobotocore_sdb.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    12788 2023-08-08 01:24:24.000000 types-aiobotocore-sdb-2.5.4/types_aiobotocore_sdb.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      737 2023-08-08 01:24:24.000000 types-aiobotocore-sdb-2.5.4/types_aiobotocore_sdb.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 01:24:24.000000 types-aiobotocore-sdb-2.5.4/types_aiobotocore_sdb.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 01:24:24.000000 types-aiobotocore-sdb-2.5.4/types_aiobotocore_sdb.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-08 01:24:24.000000 types-aiobotocore-sdb-2.5.4/types_aiobotocore_sdb.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-08-08 01:24:24.000000 types-aiobotocore-sdb-2.5.4/types_aiobotocore_sdb.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-sdb-2.5.2.post2/LICENSE` & `types-aiobotocore-sdb-2.5.4/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-sdb-2.5.2.post2/PKG-INFO` & `types-aiobotocore-sdb-2.5.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-sdb
-Version: 2.5.2.post2
-Summary: Type annotations for aiobotocore.SimpleDB 2.5.2 service generated with mypy-boto3-builder 7.17.2
+Version: 2.5.4
+Summary: Type annotations for aiobotocore.SimpleDB 2.5.4 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sdb/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-sdb.svg?color=blue)](https://pypi.org/project/types-aiobotocore-sdb)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sdb/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-sdb)](https://pepy.tech/project/types-aiobotocore-sdb)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.SimpleDB 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sdb.html#SimpleDB)
+[aiobotocore.SimpleDB 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sdb.html#SimpleDB)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-sdb-2.5.2.post2/README.md` & `types-aiobotocore-sdb-2.5.4/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-sdb.svg?color=blue)](https://pypi.org/project/types-aiobotocore-sdb)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sdb/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-sdb)](https://pepy.tech/project/types-aiobotocore-sdb)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.SimpleDB 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sdb.html#SimpleDB)
+[aiobotocore.SimpleDB 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sdb.html#SimpleDB)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-sdb-2.5.2.post2/setup.py` & `types-aiobotocore-sdb-2.5.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-sdb",
-    version="2.5.2.post2",
+    version="2.5.4",
     packages=["types_aiobotocore_sdb"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.SimpleDB 2.5.2 service generated with mypy-boto3-builder"
+        "Type annotations for aiobotocore.SimpleDB 2.5.4 service generated with mypy-boto3-builder"
         " 7.17.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
```

### Comparing `types-aiobotocore-sdb-2.5.2.post2/types_aiobotocore_sdb/__init__.py` & `types-aiobotocore-sdb-2.5.4/types_aiobotocore_sdb/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-sdb-2.5.2.post2/types_aiobotocore_sdb/__init__.pyi` & `types-aiobotocore-sdb-2.5.4/types_aiobotocore_sdb/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-sdb-2.5.2.post2/types_aiobotocore_sdb/__main__.py` & `types-aiobotocore-sdb-2.5.4/types_aiobotocore_sdb/__main__.py`

 * *Files 18% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.SimpleDB 2.5.2\nVersion:         2.5.2.post2\nBuilder"
-        " version: 7.17.2\nDocs:           "
+        "Type annotations for aiobotocore.SimpleDB 2.5.4\nVersion:         2.5.4\nBuilder version:"
+        " 7.17.2\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sdb//\nBoto3 docs:    "
         "  https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sdb.html#SimpleDB\nOther"
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

### Comparing `types-aiobotocore-sdb-2.5.2.post2/types_aiobotocore_sdb/client.py` & `types-aiobotocore-sdb-2.5.4/types_aiobotocore_sdb/client.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-sdb-2.5.2.post2/types_aiobotocore_sdb/client.pyi` & `types-aiobotocore-sdb-2.5.4/types_aiobotocore_sdb/client.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-sdb-2.5.2.post2/types_aiobotocore_sdb/literals.py` & `types-aiobotocore-sdb-2.5.4/types_aiobotocore_sdb/literals.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-sdb-2.5.2.post2/types_aiobotocore_sdb/literals.pyi` & `types-aiobotocore-sdb-2.5.4/types_aiobotocore_sdb/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-sdb-2.5.2.post2/types_aiobotocore_sdb/paginator.py` & `types-aiobotocore-sdb-2.5.4/types_aiobotocore_sdb/paginator.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-sdb-2.5.2.post2/types_aiobotocore_sdb/paginator.pyi` & `types-aiobotocore-sdb-2.5.4/types_aiobotocore_sdb/paginator.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-sdb-2.5.2.post2/types_aiobotocore_sdb/type_defs.py` & `types-aiobotocore-sdb-2.5.4/types_aiobotocore_sdb/type_defs.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-sdb-2.5.2.post2/types_aiobotocore_sdb/type_defs.pyi` & `types-aiobotocore-sdb-2.5.4/types_aiobotocore_sdb/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-sdb-2.5.2.post2/types_aiobotocore_sdb.egg-info/PKG-INFO` & `types-aiobotocore-sdb-2.5.4/types_aiobotocore_sdb.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-sdb
-Version: 2.5.2.post2
-Summary: Type annotations for aiobotocore.SimpleDB 2.5.2 service generated with mypy-boto3-builder 7.17.2
+Version: 2.5.4
+Summary: Type annotations for aiobotocore.SimpleDB 2.5.4 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sdb/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-sdb.svg?color=blue)](https://pypi.org/project/types-aiobotocore-sdb)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sdb/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-sdb)](https://pepy.tech/project/types-aiobotocore-sdb)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.SimpleDB 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sdb.html#SimpleDB)
+[aiobotocore.SimpleDB 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sdb.html#SimpleDB)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-sdb-2.5.2.post2/types_aiobotocore_sdb.egg-info/SOURCES.txt` & `types-aiobotocore-sdb-2.5.4/types_aiobotocore_sdb.egg-info/SOURCES.txt`

 * *Files identical despite different names*


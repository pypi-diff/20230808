# Comparing `tmp/types-aiobotocore-rbin-2.5.2.post2.tar.gz` & `tmp/types-aiobotocore-rbin-2.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-rbin-2.5.2.post2.tar", last modified: Fri Aug  4 13:59:22 2023, max compression
+gzip compressed data, was "types-aiobotocore-rbin-2.5.4.tar", last modified: Tue Aug  8 01:24:16 2023, max compression
```

## Comparing `types-aiobotocore-rbin-2.5.2.post2.tar` & `types-aiobotocore-rbin-2.5.4.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:22.226643 types-aiobotocore-rbin-2.5.2.post2/
--rw-r--r--   0 vlad      (1000) vlad      (1000)     1070 2023-08-04 13:49:54.000000 types-aiobotocore-rbin-2.5.2.post2/LICENSE
--rw-r--r--   0 vlad      (1000) vlad      (1000)    12768 2023-08-04 13:59:22.226643 types-aiobotocore-rbin-2.5.2.post2/PKG-INFO
--rw-r--r--   0 vlad      (1000) vlad      (1000)    11256 2023-08-04 13:49:54.000000 types-aiobotocore-rbin-2.5.2.post2/README.md
--rw-r--r--   0 vlad      (1000) vlad      (1000)       38 2023-08-04 13:59:22.226643 types-aiobotocore-rbin-2.5.2.post2/setup.cfg
--rw-r--r--   0 vlad      (1000) vlad      (1000)     2033 2023-08-04 13:49:54.000000 types-aiobotocore-rbin-2.5.2.post2/setup.py
-drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:22.216643 types-aiobotocore-rbin-2.5.2.post2/types_aiobotocore_rbin/
--rw-r--r--   0 vlad      (1000) vlad      (1000)      623 2023-08-04 13:49:54.000000 types-aiobotocore-rbin-2.5.2.post2/types_aiobotocore_rbin/__init__.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)      622 2023-08-04 13:49:54.000000 types-aiobotocore-rbin-2.5.2.post2/types_aiobotocore_rbin/__init__.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)      932 2023-08-04 13:49:54.000000 types-aiobotocore-rbin-2.5.2.post2/types_aiobotocore_rbin/__main__.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)    10323 2023-08-04 13:49:54.000000 types-aiobotocore-rbin-2.5.2.post2/types_aiobotocore_rbin/client.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)    10303 2023-08-04 13:49:54.000000 types-aiobotocore-rbin-2.5.2.post2/types_aiobotocore_rbin/client.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)     8705 2023-08-04 13:49:54.000000 types-aiobotocore-rbin-2.5.2.post2/types_aiobotocore_rbin/literals.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)     8703 2023-08-04 13:49:54.000000 types-aiobotocore-rbin-2.5.2.post2/types_aiobotocore_rbin/literals.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)     2142 2023-08-04 13:49:54.000000 types-aiobotocore-rbin-2.5.2.post2/types_aiobotocore_rbin/paginator.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)     2139 2023-08-04 13:49:54.000000 types-aiobotocore-rbin-2.5.2.post2/types_aiobotocore_rbin/paginator.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:49:54.000000 types-aiobotocore-rbin-2.5.2.post2/types_aiobotocore_rbin/py.typed
--rw-r--r--   0 vlad      (1000) vlad      (1000)     9441 2023-08-04 13:49:55.000000 types-aiobotocore-rbin-2.5.2.post2/types_aiobotocore_rbin/type_defs.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)     9430 2023-08-04 13:49:54.000000 types-aiobotocore-rbin-2.5.2.post2/types_aiobotocore_rbin/type_defs.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)       65 2023-08-04 13:49:54.000000 types-aiobotocore-rbin-2.5.2.post2/types_aiobotocore_rbin/version.py
-drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:22.216643 types-aiobotocore-rbin-2.5.2.post2/types_aiobotocore_rbin.egg-info/
--rw-r--r--   0 vlad      (1000) vlad      (1000)    12768 2023-08-04 13:59:22.000000 types-aiobotocore-rbin-2.5.2.post2/types_aiobotocore_rbin.egg-info/PKG-INFO
--rw-r--r--   0 vlad      (1000) vlad      (1000)      756 2023-08-04 13:59:22.000000 types-aiobotocore-rbin-2.5.2.post2/types_aiobotocore_rbin.egg-info/SOURCES.txt
--rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:22.000000 types-aiobotocore-rbin-2.5.2.post2/types_aiobotocore_rbin.egg-info/dependency_links.txt
--rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:22.000000 types-aiobotocore-rbin-2.5.2.post2/types_aiobotocore_rbin.egg-info/not-zip-safe
--rw-r--r--   0 vlad      (1000) vlad      (1000)       52 2023-08-04 13:59:22.000000 types-aiobotocore-rbin-2.5.2.post2/types_aiobotocore_rbin.egg-info/requires.txt
--rw-r--r--   0 vlad      (1000) vlad      (1000)       23 2023-08-04 13:59:22.000000 types-aiobotocore-rbin-2.5.2.post2/types_aiobotocore_rbin.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:24:16.862757 types-aiobotocore-rbin-2.5.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-08 01:18:50.000000 types-aiobotocore-rbin-2.5.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    12762 2023-08-08 01:24:16.862757 types-aiobotocore-rbin-2.5.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    11256 2023-08-08 01:18:50.000000 types-aiobotocore-rbin-2.5.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-08 01:24:16.862757 types-aiobotocore-rbin-2.5.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2027 2023-08-08 01:18:50.000000 types-aiobotocore-rbin-2.5.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:24:16.858757 types-aiobotocore-rbin-2.5.4/types_aiobotocore_rbin/
+-rw-r--r--   0 runner    (1001) docker     (123)      623 2023-08-08 01:18:50.000000 types-aiobotocore-rbin-2.5.4/types_aiobotocore_rbin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      622 2023-08-08 01:18:50.000000 types-aiobotocore-rbin-2.5.4/types_aiobotocore_rbin/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      920 2023-08-08 01:18:50.000000 types-aiobotocore-rbin-2.5.4/types_aiobotocore_rbin/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10323 2023-08-08 01:18:50.000000 types-aiobotocore-rbin-2.5.4/types_aiobotocore_rbin/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10303 2023-08-08 01:18:50.000000 types-aiobotocore-rbin-2.5.4/types_aiobotocore_rbin/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8705 2023-08-08 01:18:51.000000 types-aiobotocore-rbin-2.5.4/types_aiobotocore_rbin/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8703 2023-08-08 01:18:51.000000 types-aiobotocore-rbin-2.5.4/types_aiobotocore_rbin/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2142 2023-08-08 01:18:50.000000 types-aiobotocore-rbin-2.5.4/types_aiobotocore_rbin/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2139 2023-08-08 01:18:50.000000 types-aiobotocore-rbin-2.5.4/types_aiobotocore_rbin/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 01:18:50.000000 types-aiobotocore-rbin-2.5.4/types_aiobotocore_rbin/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     9441 2023-08-08 01:18:51.000000 types-aiobotocore-rbin-2.5.4/types_aiobotocore_rbin/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9430 2023-08-08 01:18:51.000000 types-aiobotocore-rbin-2.5.4/types_aiobotocore_rbin/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-08-08 01:18:50.000000 types-aiobotocore-rbin-2.5.4/types_aiobotocore_rbin/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:24:16.862757 types-aiobotocore-rbin-2.5.4/types_aiobotocore_rbin.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    12762 2023-08-08 01:24:16.000000 types-aiobotocore-rbin-2.5.4/types_aiobotocore_rbin.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      756 2023-08-08 01:24:16.000000 types-aiobotocore-rbin-2.5.4/types_aiobotocore_rbin.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 01:24:16.000000 types-aiobotocore-rbin-2.5.4/types_aiobotocore_rbin.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 01:24:16.000000 types-aiobotocore-rbin-2.5.4/types_aiobotocore_rbin.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-08 01:24:16.000000 types-aiobotocore-rbin-2.5.4/types_aiobotocore_rbin.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-08-08 01:24:16.000000 types-aiobotocore-rbin-2.5.4/types_aiobotocore_rbin.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-rbin-2.5.2.post2/LICENSE` & `types-aiobotocore-rbin-2.5.4/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-rbin-2.5.2.post2/PKG-INFO` & `types-aiobotocore-rbin-2.5.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-rbin
-Version: 2.5.2.post2
-Summary: Type annotations for aiobotocore.RecycleBin 2.5.2 service generated with mypy-boto3-builder 7.17.2
+Version: 2.5.4
+Summary: Type annotations for aiobotocore.RecycleBin 2.5.4 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rbin/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-rbin.svg?color=blue)](https://pypi.org/project/types-aiobotocore-rbin)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rbin/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-rbin)](https://pepy.tech/project/types-aiobotocore-rbin)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.RecycleBin 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rbin.html#RecycleBin)
+[aiobotocore.RecycleBin 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rbin.html#RecycleBin)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-rbin-2.5.2.post2/README.md` & `types-aiobotocore-rbin-2.5.4/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-rbin.svg?color=blue)](https://pypi.org/project/types-aiobotocore-rbin)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rbin/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-rbin)](https://pepy.tech/project/types-aiobotocore-rbin)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.RecycleBin 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rbin.html#RecycleBin)
+[aiobotocore.RecycleBin 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rbin.html#RecycleBin)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-rbin-2.5.2.post2/setup.py` & `types-aiobotocore-rbin-2.5.4/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-rbin",
-    version="2.5.2.post2",
+    version="2.5.4",
     packages=["types_aiobotocore_rbin"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.RecycleBin 2.5.2 service generated with"
+        "Type annotations for aiobotocore.RecycleBin 2.5.4 service generated with"
         " mypy-boto3-builder 7.17.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
```

### Comparing `types-aiobotocore-rbin-2.5.2.post2/types_aiobotocore_rbin/__init__.py` & `types-aiobotocore-rbin-2.5.4/types_aiobotocore_rbin/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-rbin-2.5.2.post2/types_aiobotocore_rbin/__init__.pyi` & `types-aiobotocore-rbin-2.5.4/types_aiobotocore_rbin/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-rbin-2.5.2.post2/types_aiobotocore_rbin/__main__.py` & `types-aiobotocore-rbin-2.5.4/types_aiobotocore_rbin/__main__.py`

 * *Files 13% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.RecycleBin 2.5.2\nVersion:         2.5.2.post2\nBuilder"
+        "Type annotations for aiobotocore.RecycleBin 2.5.4\nVersion:         2.5.4\nBuilder"
         " version: 7.17.2\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rbin//\nBoto3 docs:   "
         "   https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rbin.html#RecycleBin\nOther"
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

### Comparing `types-aiobotocore-rbin-2.5.2.post2/types_aiobotocore_rbin/client.py` & `types-aiobotocore-rbin-2.5.4/types_aiobotocore_rbin/client.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-rbin-2.5.2.post2/types_aiobotocore_rbin/client.pyi` & `types-aiobotocore-rbin-2.5.4/types_aiobotocore_rbin/client.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-rbin-2.5.2.post2/types_aiobotocore_rbin/literals.py` & `types-aiobotocore-rbin-2.5.4/types_aiobotocore_rbin/literals.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-rbin-2.5.2.post2/types_aiobotocore_rbin/literals.pyi` & `types-aiobotocore-rbin-2.5.4/types_aiobotocore_rbin/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-rbin-2.5.2.post2/types_aiobotocore_rbin/paginator.py` & `types-aiobotocore-rbin-2.5.4/types_aiobotocore_rbin/paginator.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-rbin-2.5.2.post2/types_aiobotocore_rbin/paginator.pyi` & `types-aiobotocore-rbin-2.5.4/types_aiobotocore_rbin/paginator.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-rbin-2.5.2.post2/types_aiobotocore_rbin/type_defs.py` & `types-aiobotocore-rbin-2.5.4/types_aiobotocore_rbin/type_defs.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-rbin-2.5.2.post2/types_aiobotocore_rbin/type_defs.pyi` & `types-aiobotocore-rbin-2.5.4/types_aiobotocore_rbin/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-rbin-2.5.2.post2/types_aiobotocore_rbin.egg-info/PKG-INFO` & `types-aiobotocore-rbin-2.5.4/types_aiobotocore_rbin.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-rbin
-Version: 2.5.2.post2
-Summary: Type annotations for aiobotocore.RecycleBin 2.5.2 service generated with mypy-boto3-builder 7.17.2
+Version: 2.5.4
+Summary: Type annotations for aiobotocore.RecycleBin 2.5.4 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rbin/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-rbin.svg?color=blue)](https://pypi.org/project/types-aiobotocore-rbin)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rbin/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-rbin)](https://pepy.tech/project/types-aiobotocore-rbin)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.RecycleBin 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rbin.html#RecycleBin)
+[aiobotocore.RecycleBin 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rbin.html#RecycleBin)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-rbin-2.5.2.post2/types_aiobotocore_rbin.egg-info/SOURCES.txt` & `types-aiobotocore-rbin-2.5.4/types_aiobotocore_rbin.egg-info/SOURCES.txt`

 * *Files identical despite different names*


# Comparing `tmp/types-aiobotocore-kendra-2.5.2.post2.tar.gz` & `tmp/types-aiobotocore-kendra-2.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-kendra-2.5.2.post2.tar", last modified: Fri Aug  4 13:59:13 2023, max compression
+gzip compressed data, was "types-aiobotocore-kendra-2.5.4.tar", last modified: Tue Aug  8 01:23:55 2023, max compression
```

## Comparing `types-aiobotocore-kendra-2.5.2.post2.tar` & `types-aiobotocore-kendra-2.5.4.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:13.416643 types-aiobotocore-kendra-2.5.2.post2/
--rw-r--r--   0 vlad      (1000) vlad      (1000)     1070 2023-08-04 13:41:48.000000 types-aiobotocore-kendra-2.5.2.post2/LICENSE
--rw-r--r--   0 vlad      (1000) vlad      (1000)    12213 2023-08-04 13:59:13.416643 types-aiobotocore-kendra-2.5.2.post2/PKG-INFO
--rw-r--r--   0 vlad      (1000) vlad      (1000)    10699 2023-08-04 13:41:48.000000 types-aiobotocore-kendra-2.5.2.post2/README.md
--rw-r--r--   0 vlad      (1000) vlad      (1000)       38 2023-08-04 13:59:13.426643 types-aiobotocore-kendra-2.5.2.post2/setup.cfg
--rw-r--r--   0 vlad      (1000) vlad      (1000)     2065 2023-08-04 13:41:48.000000 types-aiobotocore-kendra-2.5.2.post2/setup.py
-drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:13.416643 types-aiobotocore-kendra-2.5.2.post2/types_aiobotocore_kendra/
--rw-r--r--   0 vlad      (1000) vlad      (1000)      434 2023-08-04 13:41:48.000000 types-aiobotocore-kendra-2.5.2.post2/types_aiobotocore_kendra/__init__.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)      433 2023-08-04 13:41:48.000000 types-aiobotocore-kendra-2.5.2.post2/types_aiobotocore_kendra/__init__.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)      928 2023-08-04 13:41:48.000000 types-aiobotocore-kendra-2.5.2.post2/types_aiobotocore_kendra/__main__.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)    50591 2023-08-04 13:41:48.000000 types-aiobotocore-kendra-2.5.2.post2/types_aiobotocore_kendra/client.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)    50517 2023-08-04 13:41:48.000000 types-aiobotocore-kendra-2.5.2.post2/types_aiobotocore_kendra/client.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)    15441 2023-08-04 13:41:49.000000 types-aiobotocore-kendra-2.5.2.post2/types_aiobotocore_kendra/literals.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)    15439 2023-08-04 13:41:48.000000 types-aiobotocore-kendra-2.5.2.post2/types_aiobotocore_kendra/literals.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:41:48.000000 types-aiobotocore-kendra-2.5.2.post2/types_aiobotocore_kendra/py.typed
--rw-r--r--   0 vlad      (1000) vlad      (1000)   110892 2023-08-04 13:41:52.000000 types-aiobotocore-kendra-2.5.2.post2/types_aiobotocore_kendra/type_defs.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)   110739 2023-08-04 13:41:50.000000 types-aiobotocore-kendra-2.5.2.post2/types_aiobotocore_kendra/type_defs.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)       65 2023-08-04 13:41:48.000000 types-aiobotocore-kendra-2.5.2.post2/types_aiobotocore_kendra/version.py
-drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:13.416643 types-aiobotocore-kendra-2.5.2.post2/types_aiobotocore_kendra.egg-info/
--rw-r--r--   0 vlad      (1000) vlad      (1000)    12213 2023-08-04 13:59:13.000000 types-aiobotocore-kendra-2.5.2.post2/types_aiobotocore_kendra.egg-info/PKG-INFO
--rw-r--r--   0 vlad      (1000) vlad      (1000)      717 2023-08-04 13:59:13.000000 types-aiobotocore-kendra-2.5.2.post2/types_aiobotocore_kendra.egg-info/SOURCES.txt
--rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:13.000000 types-aiobotocore-kendra-2.5.2.post2/types_aiobotocore_kendra.egg-info/dependency_links.txt
--rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:13.000000 types-aiobotocore-kendra-2.5.2.post2/types_aiobotocore_kendra.egg-info/not-zip-safe
--rw-r--r--   0 vlad      (1000) vlad      (1000)       52 2023-08-04 13:59:13.000000 types-aiobotocore-kendra-2.5.2.post2/types_aiobotocore_kendra.egg-info/requires.txt
--rw-r--r--   0 vlad      (1000) vlad      (1000)       25 2023-08-04 13:59:13.000000 types-aiobotocore-kendra-2.5.2.post2/types_aiobotocore_kendra.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:23:55.570713 types-aiobotocore-kendra-2.5.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-08 01:13:26.000000 types-aiobotocore-kendra-2.5.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    12207 2023-08-08 01:23:55.570713 types-aiobotocore-kendra-2.5.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10699 2023-08-08 01:13:26.000000 types-aiobotocore-kendra-2.5.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-08 01:23:55.570713 types-aiobotocore-kendra-2.5.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2059 2023-08-08 01:13:26.000000 types-aiobotocore-kendra-2.5.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:23:55.566713 types-aiobotocore-kendra-2.5.4/types_aiobotocore_kendra/
+-rw-r--r--   0 runner    (1001) docker     (123)      434 2023-08-08 01:13:26.000000 types-aiobotocore-kendra-2.5.4/types_aiobotocore_kendra/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      433 2023-08-08 01:13:26.000000 types-aiobotocore-kendra-2.5.4/types_aiobotocore_kendra/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      916 2023-08-08 01:13:26.000000 types-aiobotocore-kendra-2.5.4/types_aiobotocore_kendra/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    50591 2023-08-08 01:13:28.000000 types-aiobotocore-kendra-2.5.4/types_aiobotocore_kendra/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    50517 2023-08-08 01:13:28.000000 types-aiobotocore-kendra-2.5.4/types_aiobotocore_kendra/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    15441 2023-08-08 01:13:28.000000 types-aiobotocore-kendra-2.5.4/types_aiobotocore_kendra/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15439 2023-08-08 01:13:28.000000 types-aiobotocore-kendra-2.5.4/types_aiobotocore_kendra/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 01:13:26.000000 types-aiobotocore-kendra-2.5.4/types_aiobotocore_kendra/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)   110892 2023-08-08 01:13:30.000000 types-aiobotocore-kendra-2.5.4/types_aiobotocore_kendra/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)   110739 2023-08-08 01:13:29.000000 types-aiobotocore-kendra-2.5.4/types_aiobotocore_kendra/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-08-08 01:13:26.000000 types-aiobotocore-kendra-2.5.4/types_aiobotocore_kendra/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:23:55.570713 types-aiobotocore-kendra-2.5.4/types_aiobotocore_kendra.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    12207 2023-08-08 01:23:55.000000 types-aiobotocore-kendra-2.5.4/types_aiobotocore_kendra.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      717 2023-08-08 01:23:55.000000 types-aiobotocore-kendra-2.5.4/types_aiobotocore_kendra.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 01:23:55.000000 types-aiobotocore-kendra-2.5.4/types_aiobotocore_kendra.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 01:23:55.000000 types-aiobotocore-kendra-2.5.4/types_aiobotocore_kendra.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-08 01:23:55.000000 types-aiobotocore-kendra-2.5.4/types_aiobotocore_kendra.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-08-08 01:23:55.000000 types-aiobotocore-kendra-2.5.4/types_aiobotocore_kendra.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-kendra-2.5.2.post2/LICENSE` & `types-aiobotocore-kendra-2.5.4/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-kendra-2.5.2.post2/PKG-INFO` & `types-aiobotocore-kendra-2.5.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-kendra
-Version: 2.5.2.post2
-Summary: Type annotations for aiobotocore.kendra 2.5.2 service generated with mypy-boto3-builder 7.17.2
+Version: 2.5.4
+Summary: Type annotations for aiobotocore.kendra 2.5.4 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kendra/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-kendra.svg?color=blue)](https://pypi.org/project/types-aiobotocore-kendra)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kendra/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-kendra)](https://pepy.tech/project/types-aiobotocore-kendra)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.kendra 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kendra.html#kendra)
+[aiobotocore.kendra 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kendra.html#kendra)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-kendra-2.5.2.post2/README.md` & `types-aiobotocore-kendra-2.5.4/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-kendra.svg?color=blue)](https://pypi.org/project/types-aiobotocore-kendra)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kendra/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-kendra)](https://pepy.tech/project/types-aiobotocore-kendra)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.kendra 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kendra.html#kendra)
+[aiobotocore.kendra 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kendra.html#kendra)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-kendra-2.5.2.post2/setup.py` & `types-aiobotocore-kendra-2.5.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-kendra",
-    version="2.5.2.post2",
+    version="2.5.4",
     packages=["types_aiobotocore_kendra"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.kendra 2.5.2 service generated with mypy-boto3-builder"
+        "Type annotations for aiobotocore.kendra 2.5.4 service generated with mypy-boto3-builder"
         " 7.17.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
```

### Comparing `types-aiobotocore-kendra-2.5.2.post2/types_aiobotocore_kendra/__main__.py` & `types-aiobotocore-kendra-2.5.4/types_aiobotocore_kendra/__main__.py`

 * *Files 15% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.kendra 2.5.2\nVersion:         2.5.2.post2\nBuilder"
-        " version: 7.17.2\nDocs:           "
+        "Type annotations for aiobotocore.kendra 2.5.4\nVersion:         2.5.4\nBuilder version:"
+        " 7.17.2\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kendra//\nBoto3 docs: "
         "     https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kendra.html#kendra\nOther"
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

### Comparing `types-aiobotocore-kendra-2.5.2.post2/types_aiobotocore_kendra/client.py` & `types-aiobotocore-kendra-2.5.4/types_aiobotocore_kendra/client.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-kendra-2.5.2.post2/types_aiobotocore_kendra/client.pyi` & `types-aiobotocore-kendra-2.5.4/types_aiobotocore_kendra/client.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-kendra-2.5.2.post2/types_aiobotocore_kendra/literals.py` & `types-aiobotocore-kendra-2.5.4/types_aiobotocore_kendra/literals.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-kendra-2.5.2.post2/types_aiobotocore_kendra/literals.pyi` & `types-aiobotocore-kendra-2.5.4/types_aiobotocore_kendra/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-kendra-2.5.2.post2/types_aiobotocore_kendra/type_defs.py` & `types-aiobotocore-kendra-2.5.4/types_aiobotocore_kendra/type_defs.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-kendra-2.5.2.post2/types_aiobotocore_kendra/type_defs.pyi` & `types-aiobotocore-kendra-2.5.4/types_aiobotocore_kendra/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-kendra-2.5.2.post2/types_aiobotocore_kendra.egg-info/PKG-INFO` & `types-aiobotocore-kendra-2.5.4/types_aiobotocore_kendra.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-kendra
-Version: 2.5.2.post2
-Summary: Type annotations for aiobotocore.kendra 2.5.2 service generated with mypy-boto3-builder 7.17.2
+Version: 2.5.4
+Summary: Type annotations for aiobotocore.kendra 2.5.4 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kendra/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-kendra.svg?color=blue)](https://pypi.org/project/types-aiobotocore-kendra)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kendra/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-kendra)](https://pepy.tech/project/types-aiobotocore-kendra)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.kendra 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kendra.html#kendra)
+[aiobotocore.kendra 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kendra.html#kendra)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-kendra-2.5.2.post2/types_aiobotocore_kendra.egg-info/SOURCES.txt` & `types-aiobotocore-kendra-2.5.4/types_aiobotocore_kendra.egg-info/SOURCES.txt`

 * *Files identical despite different names*


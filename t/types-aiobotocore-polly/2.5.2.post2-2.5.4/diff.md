# Comparing `tmp/types-aiobotocore-polly-2.5.2.post2.tar.gz` & `tmp/types-aiobotocore-polly-2.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-polly-2.5.2.post2.tar", last modified: Fri Aug  4 13:59:21 2023, max compression
+gzip compressed data, was "types-aiobotocore-polly-2.5.4.tar", last modified: Tue Aug  8 01:24:15 2023, max compression
```

## Comparing `types-aiobotocore-polly-2.5.2.post2.tar` & `types-aiobotocore-polly-2.5.4.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:21.756643 types-aiobotocore-polly-2.5.2.post2/
--rw-r--r--   0 vlad      (1000) vlad      (1000)     1070 2023-08-04 13:47:05.000000 types-aiobotocore-polly-2.5.2.post2/LICENSE
--rw-r--r--   0 vlad      (1000) vlad      (1000)    13130 2023-08-04 13:59:21.756643 types-aiobotocore-polly-2.5.2.post2/PKG-INFO
--rw-r--r--   0 vlad      (1000) vlad      (1000)    11620 2023-08-04 13:47:05.000000 types-aiobotocore-polly-2.5.2.post2/README.md
--rw-r--r--   0 vlad      (1000) vlad      (1000)       38 2023-08-04 13:59:21.756643 types-aiobotocore-polly-2.5.2.post2/setup.cfg
--rw-r--r--   0 vlad      (1000) vlad      (1000)     2058 2023-08-04 13:47:05.000000 types-aiobotocore-polly-2.5.2.post2/setup.py
-drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:21.746643 types-aiobotocore-polly-2.5.2.post2/types_aiobotocore_polly/
--rw-r--r--   0 vlad      (1000) vlad      (1000)     1087 2023-08-04 13:47:05.000000 types-aiobotocore-polly-2.5.2.post2/types_aiobotocore_polly/__init__.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)     1086 2023-08-04 13:47:05.000000 types-aiobotocore-polly-2.5.2.post2/types_aiobotocore_polly/__init__.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)      924 2023-08-04 13:47:05.000000 types-aiobotocore-polly-2.5.2.post2/types_aiobotocore_polly/__main__.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)    12645 2023-08-04 13:47:05.000000 types-aiobotocore-polly-2.5.2.post2/types_aiobotocore_polly/client.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)    12624 2023-08-04 13:47:05.000000 types-aiobotocore-polly-2.5.2.post2/types_aiobotocore_polly/client.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)    10758 2023-08-04 13:47:05.000000 types-aiobotocore-polly-2.5.2.post2/types_aiobotocore_polly/literals.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)    10756 2023-08-04 13:47:05.000000 types-aiobotocore-polly-2.5.2.post2/types_aiobotocore_polly/literals.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)     4382 2023-08-04 13:47:05.000000 types-aiobotocore-polly-2.5.2.post2/types_aiobotocore_polly/paginator.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)     4377 2023-08-04 13:47:05.000000 types-aiobotocore-polly-2.5.2.post2/types_aiobotocore_polly/paginator.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:47:05.000000 types-aiobotocore-polly-2.5.2.post2/types_aiobotocore_polly/py.typed
--rw-r--r--   0 vlad      (1000) vlad      (1000)     8921 2023-08-04 13:47:06.000000 types-aiobotocore-polly-2.5.2.post2/types_aiobotocore_polly/type_defs.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)     8916 2023-08-04 13:47:06.000000 types-aiobotocore-polly-2.5.2.post2/types_aiobotocore_polly/type_defs.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)       65 2023-08-04 13:47:05.000000 types-aiobotocore-polly-2.5.2.post2/types_aiobotocore_polly/version.py
-drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:21.746643 types-aiobotocore-polly-2.5.2.post2/types_aiobotocore_polly.egg-info/
--rw-r--r--   0 vlad      (1000) vlad      (1000)    13130 2023-08-04 13:59:21.000000 types-aiobotocore-polly-2.5.2.post2/types_aiobotocore_polly.egg-info/PKG-INFO
--rw-r--r--   0 vlad      (1000) vlad      (1000)      775 2023-08-04 13:59:21.000000 types-aiobotocore-polly-2.5.2.post2/types_aiobotocore_polly.egg-info/SOURCES.txt
--rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:21.000000 types-aiobotocore-polly-2.5.2.post2/types_aiobotocore_polly.egg-info/dependency_links.txt
--rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:21.000000 types-aiobotocore-polly-2.5.2.post2/types_aiobotocore_polly.egg-info/not-zip-safe
--rw-r--r--   0 vlad      (1000) vlad      (1000)       52 2023-08-04 13:59:21.000000 types-aiobotocore-polly-2.5.2.post2/types_aiobotocore_polly.egg-info/requires.txt
--rw-r--r--   0 vlad      (1000) vlad      (1000)       24 2023-08-04 13:59:21.000000 types-aiobotocore-polly-2.5.2.post2/types_aiobotocore_polly.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:24:15.474753 types-aiobotocore-polly-2.5.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-08 01:16:50.000000 types-aiobotocore-polly-2.5.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    13124 2023-08-08 01:24:15.470754 types-aiobotocore-polly-2.5.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    11620 2023-08-08 01:16:50.000000 types-aiobotocore-polly-2.5.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-08 01:24:15.474753 types-aiobotocore-polly-2.5.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2052 2023-08-08 01:16:50.000000 types-aiobotocore-polly-2.5.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:24:15.470754 types-aiobotocore-polly-2.5.4/types_aiobotocore_polly/
+-rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-08-08 01:16:50.000000 types-aiobotocore-polly-2.5.4/types_aiobotocore_polly/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1086 2023-08-08 01:16:50.000000 types-aiobotocore-polly-2.5.4/types_aiobotocore_polly/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      912 2023-08-08 01:16:50.000000 types-aiobotocore-polly-2.5.4/types_aiobotocore_polly/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12645 2023-08-08 01:16:51.000000 types-aiobotocore-polly-2.5.4/types_aiobotocore_polly/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12624 2023-08-08 01:16:50.000000 types-aiobotocore-polly-2.5.4/types_aiobotocore_polly/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    10758 2023-08-08 01:16:51.000000 types-aiobotocore-polly-2.5.4/types_aiobotocore_polly/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10756 2023-08-08 01:16:51.000000 types-aiobotocore-polly-2.5.4/types_aiobotocore_polly/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     4382 2023-08-08 01:16:51.000000 types-aiobotocore-polly-2.5.4/types_aiobotocore_polly/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4377 2023-08-08 01:16:51.000000 types-aiobotocore-polly-2.5.4/types_aiobotocore_polly/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 01:16:50.000000 types-aiobotocore-polly-2.5.4/types_aiobotocore_polly/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     8921 2023-08-08 01:16:51.000000 types-aiobotocore-polly-2.5.4/types_aiobotocore_polly/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8916 2023-08-08 01:16:51.000000 types-aiobotocore-polly-2.5.4/types_aiobotocore_polly/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-08-08 01:16:50.000000 types-aiobotocore-polly-2.5.4/types_aiobotocore_polly/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:24:15.470754 types-aiobotocore-polly-2.5.4/types_aiobotocore_polly.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    13124 2023-08-08 01:24:15.000000 types-aiobotocore-polly-2.5.4/types_aiobotocore_polly.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      775 2023-08-08 01:24:15.000000 types-aiobotocore-polly-2.5.4/types_aiobotocore_polly.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 01:24:15.000000 types-aiobotocore-polly-2.5.4/types_aiobotocore_polly.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 01:24:15.000000 types-aiobotocore-polly-2.5.4/types_aiobotocore_polly.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-08 01:24:15.000000 types-aiobotocore-polly-2.5.4/types_aiobotocore_polly.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-08-08 01:24:15.000000 types-aiobotocore-polly-2.5.4/types_aiobotocore_polly.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-polly-2.5.2.post2/LICENSE` & `types-aiobotocore-polly-2.5.4/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-polly-2.5.2.post2/PKG-INFO` & `types-aiobotocore-polly-2.5.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-polly
-Version: 2.5.2.post2
-Summary: Type annotations for aiobotocore.Polly 2.5.2 service generated with mypy-boto3-builder 7.17.2
+Version: 2.5.4
+Summary: Type annotations for aiobotocore.Polly 2.5.4 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_polly/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-polly.svg?color=blue)](https://pypi.org/project/types-aiobotocore-polly)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_polly/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-polly)](https://pepy.tech/project/types-aiobotocore-polly)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.Polly 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/polly.html#Polly)
+[aiobotocore.Polly 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/polly.html#Polly)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-polly-2.5.2.post2/README.md` & `types-aiobotocore-polly-2.5.4/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-polly.svg?color=blue)](https://pypi.org/project/types-aiobotocore-polly)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_polly/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-polly)](https://pepy.tech/project/types-aiobotocore-polly)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.Polly 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/polly.html#Polly)
+[aiobotocore.Polly 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/polly.html#Polly)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-polly-2.5.2.post2/setup.py` & `types-aiobotocore-polly-2.5.4/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-polly",
-    version="2.5.2.post2",
+    version="2.5.4",
     packages=["types_aiobotocore_polly"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.Polly 2.5.2 service generated with mypy-boto3-builder"
+        "Type annotations for aiobotocore.Polly 2.5.4 service generated with mypy-boto3-builder"
         " 7.17.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
```

### Comparing `types-aiobotocore-polly-2.5.2.post2/types_aiobotocore_polly/__init__.py` & `types-aiobotocore-polly-2.5.4/types_aiobotocore_polly/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-polly-2.5.2.post2/types_aiobotocore_polly/__init__.pyi` & `types-aiobotocore-polly-2.5.4/types_aiobotocore_polly/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-polly-2.5.2.post2/types_aiobotocore_polly/__main__.py` & `types-aiobotocore-polly-2.5.4/types_aiobotocore_polly/__main__.py`

 * *Files 9% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.Polly 2.5.2\nVersion:         2.5.2.post2\nBuilder"
-        " version: 7.17.2\nDocs:           "
+        "Type annotations for aiobotocore.Polly 2.5.4\nVersion:         2.5.4\nBuilder version:"
+        " 7.17.2\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_polly//\nBoto3 docs:  "
         "    https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/polly.html#Polly\nOther"
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

### Comparing `types-aiobotocore-polly-2.5.2.post2/types_aiobotocore_polly/client.py` & `types-aiobotocore-polly-2.5.4/types_aiobotocore_polly/client.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-polly-2.5.2.post2/types_aiobotocore_polly/client.pyi` & `types-aiobotocore-polly-2.5.4/types_aiobotocore_polly/client.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-polly-2.5.2.post2/types_aiobotocore_polly/literals.py` & `types-aiobotocore-polly-2.5.4/types_aiobotocore_polly/literals.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-polly-2.5.2.post2/types_aiobotocore_polly/literals.pyi` & `types-aiobotocore-polly-2.5.4/types_aiobotocore_polly/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-polly-2.5.2.post2/types_aiobotocore_polly/paginator.py` & `types-aiobotocore-polly-2.5.4/types_aiobotocore_polly/paginator.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-polly-2.5.2.post2/types_aiobotocore_polly/paginator.pyi` & `types-aiobotocore-polly-2.5.4/types_aiobotocore_polly/paginator.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-polly-2.5.2.post2/types_aiobotocore_polly/type_defs.py` & `types-aiobotocore-polly-2.5.4/types_aiobotocore_polly/type_defs.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-polly-2.5.2.post2/types_aiobotocore_polly/type_defs.pyi` & `types-aiobotocore-polly-2.5.4/types_aiobotocore_polly/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-polly-2.5.2.post2/types_aiobotocore_polly.egg-info/PKG-INFO` & `types-aiobotocore-polly-2.5.4/types_aiobotocore_polly.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-polly
-Version: 2.5.2.post2
-Summary: Type annotations for aiobotocore.Polly 2.5.2 service generated with mypy-boto3-builder 7.17.2
+Version: 2.5.4
+Summary: Type annotations for aiobotocore.Polly 2.5.4 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_polly/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-polly.svg?color=blue)](https://pypi.org/project/types-aiobotocore-polly)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_polly/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-polly)](https://pepy.tech/project/types-aiobotocore-polly)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.Polly 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/polly.html#Polly)
+[aiobotocore.Polly 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/polly.html#Polly)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-polly-2.5.2.post2/types_aiobotocore_polly.egg-info/SOURCES.txt` & `types-aiobotocore-polly-2.5.4/types_aiobotocore_polly.egg-info/SOURCES.txt`

 * *Files identical despite different names*


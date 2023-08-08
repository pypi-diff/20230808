# Comparing `tmp/types-aiobotocore-omics-2.5.2.post2.tar.gz` & `tmp/types-aiobotocore-omics-2.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-omics-2.5.2.post2.tar", last modified: Fri Aug  4 13:59:20 2023, max compression
+gzip compressed data, was "types-aiobotocore-omics-2.5.4.tar", last modified: Tue Aug  8 01:24:10 2023, max compression
```

## Comparing `types-aiobotocore-omics-2.5.2.post2.tar` & `types-aiobotocore-omics-2.5.4.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:20.026643 types-aiobotocore-omics-2.5.2.post2/
--rw-r--r--   0 vlad      (1000) vlad      (1000)     1070 2023-08-04 13:45:50.000000 types-aiobotocore-omics-2.5.2.post2/LICENSE
--rw-r--r--   0 vlad      (1000) vlad      (1000)    18326 2023-08-04 13:59:20.026643 types-aiobotocore-omics-2.5.2.post2/PKG-INFO
--rw-r--r--   0 vlad      (1000) vlad      (1000)    16816 2023-08-04 13:45:50.000000 types-aiobotocore-omics-2.5.2.post2/README.md
--rw-r--r--   0 vlad      (1000) vlad      (1000)       38 2023-08-04 13:59:20.026643 types-aiobotocore-omics-2.5.2.post2/setup.cfg
--rw-r--r--   0 vlad      (1000) vlad      (1000)     2058 2023-08-04 13:45:50.000000 types-aiobotocore-omics-2.5.2.post2/setup.py
-drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:20.016643 types-aiobotocore-omics-2.5.2.post2/types_aiobotocore_omics/
--rw-r--r--   0 vlad      (1000) vlad      (1000)     7574 2023-08-04 13:45:50.000000 types-aiobotocore-omics-2.5.2.post2/types_aiobotocore_omics/__init__.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)     7573 2023-08-04 13:45:50.000000 types-aiobotocore-omics-2.5.2.post2/types_aiobotocore_omics/__init__.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)      924 2023-08-04 13:45:50.000000 types-aiobotocore-omics-2.5.2.post2/types_aiobotocore_omics/__main__.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)    64683 2023-08-04 13:45:52.000000 types-aiobotocore-omics-2.5.2.post2/types_aiobotocore_omics/client.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)    64569 2023-08-04 13:45:51.000000 types-aiobotocore-omics-2.5.2.post2/types_aiobotocore_omics/client.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)    15939 2023-08-04 13:45:52.000000 types-aiobotocore-omics-2.5.2.post2/types_aiobotocore_omics/literals.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)    15937 2023-08-04 13:45:52.000000 types-aiobotocore-omics-2.5.2.post2/types_aiobotocore_omics/literals.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)    22901 2023-08-04 13:45:52.000000 types-aiobotocore-omics-2.5.2.post2/types_aiobotocore_omics/paginator.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)    22881 2023-08-04 13:45:52.000000 types-aiobotocore-omics-2.5.2.post2/types_aiobotocore_omics/paginator.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:45:50.000000 types-aiobotocore-omics-2.5.2.post2/types_aiobotocore_omics/py.typed
--rw-r--r--   0 vlad      (1000) vlad      (1000)    97568 2023-08-04 13:45:56.000000 types-aiobotocore-omics-2.5.2.post2/types_aiobotocore_omics/type_defs.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)    97412 2023-08-04 13:45:53.000000 types-aiobotocore-omics-2.5.2.post2/types_aiobotocore_omics/type_defs.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)       65 2023-08-04 13:45:50.000000 types-aiobotocore-omics-2.5.2.post2/types_aiobotocore_omics/version.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)    15945 2023-08-04 13:45:52.000000 types-aiobotocore-omics-2.5.2.post2/types_aiobotocore_omics/waiter.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)    15929 2023-08-04 13:45:52.000000 types-aiobotocore-omics-2.5.2.post2/types_aiobotocore_omics/waiter.pyi
-drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:20.026643 types-aiobotocore-omics-2.5.2.post2/types_aiobotocore_omics.egg-info/
--rw-r--r--   0 vlad      (1000) vlad      (1000)    18326 2023-08-04 13:59:19.000000 types-aiobotocore-omics-2.5.2.post2/types_aiobotocore_omics.egg-info/PKG-INFO
--rw-r--r--   0 vlad      (1000) vlad      (1000)      844 2023-08-04 13:59:19.000000 types-aiobotocore-omics-2.5.2.post2/types_aiobotocore_omics.egg-info/SOURCES.txt
--rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:19.000000 types-aiobotocore-omics-2.5.2.post2/types_aiobotocore_omics.egg-info/dependency_links.txt
--rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:19.000000 types-aiobotocore-omics-2.5.2.post2/types_aiobotocore_omics.egg-info/not-zip-safe
--rw-r--r--   0 vlad      (1000) vlad      (1000)       52 2023-08-04 13:59:19.000000 types-aiobotocore-omics-2.5.2.post2/types_aiobotocore_omics.egg-info/requires.txt
--rw-r--r--   0 vlad      (1000) vlad      (1000)       24 2023-08-04 13:59:19.000000 types-aiobotocore-omics-2.5.2.post2/types_aiobotocore_omics.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:24:10.886744 types-aiobotocore-omics-2.5.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-08 01:16:04.000000 types-aiobotocore-omics-2.5.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    18320 2023-08-08 01:24:10.882744 types-aiobotocore-omics-2.5.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    16816 2023-08-08 01:16:04.000000 types-aiobotocore-omics-2.5.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-08 01:24:10.886744 types-aiobotocore-omics-2.5.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2052 2023-08-08 01:16:04.000000 types-aiobotocore-omics-2.5.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:24:10.878744 types-aiobotocore-omics-2.5.4/types_aiobotocore_omics/
+-rw-r--r--   0 runner    (1001) docker     (123)     7574 2023-08-08 01:16:04.000000 types-aiobotocore-omics-2.5.4/types_aiobotocore_omics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7573 2023-08-08 01:16:04.000000 types-aiobotocore-omics-2.5.4/types_aiobotocore_omics/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      912 2023-08-08 01:16:04.000000 types-aiobotocore-omics-2.5.4/types_aiobotocore_omics/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    64683 2023-08-08 01:16:04.000000 types-aiobotocore-omics-2.5.4/types_aiobotocore_omics/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    64569 2023-08-08 01:16:04.000000 types-aiobotocore-omics-2.5.4/types_aiobotocore_omics/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    15939 2023-08-08 01:16:05.000000 types-aiobotocore-omics-2.5.4/types_aiobotocore_omics/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15937 2023-08-08 01:16:04.000000 types-aiobotocore-omics-2.5.4/types_aiobotocore_omics/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    22901 2023-08-08 01:16:04.000000 types-aiobotocore-omics-2.5.4/types_aiobotocore_omics/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22881 2023-08-08 01:16:04.000000 types-aiobotocore-omics-2.5.4/types_aiobotocore_omics/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 01:16:04.000000 types-aiobotocore-omics-2.5.4/types_aiobotocore_omics/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    97568 2023-08-08 01:16:06.000000 types-aiobotocore-omics-2.5.4/types_aiobotocore_omics/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    97412 2023-08-08 01:16:06.000000 types-aiobotocore-omics-2.5.4/types_aiobotocore_omics/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-08-08 01:16:04.000000 types-aiobotocore-omics-2.5.4/types_aiobotocore_omics/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15945 2023-08-08 01:16:04.000000 types-aiobotocore-omics-2.5.4/types_aiobotocore_omics/waiter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15929 2023-08-08 01:16:04.000000 types-aiobotocore-omics-2.5.4/types_aiobotocore_omics/waiter.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:24:10.882744 types-aiobotocore-omics-2.5.4/types_aiobotocore_omics.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    18320 2023-08-08 01:24:10.000000 types-aiobotocore-omics-2.5.4/types_aiobotocore_omics.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      844 2023-08-08 01:24:10.000000 types-aiobotocore-omics-2.5.4/types_aiobotocore_omics.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 01:24:10.000000 types-aiobotocore-omics-2.5.4/types_aiobotocore_omics.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 01:24:10.000000 types-aiobotocore-omics-2.5.4/types_aiobotocore_omics.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-08 01:24:10.000000 types-aiobotocore-omics-2.5.4/types_aiobotocore_omics.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-08-08 01:24:10.000000 types-aiobotocore-omics-2.5.4/types_aiobotocore_omics.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-omics-2.5.2.post2/LICENSE` & `types-aiobotocore-omics-2.5.4/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-omics-2.5.2.post2/PKG-INFO` & `types-aiobotocore-omics-2.5.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-omics
-Version: 2.5.2.post2
-Summary: Type annotations for aiobotocore.Omics 2.5.2 service generated with mypy-boto3-builder 7.17.2
+Version: 2.5.4
+Summary: Type annotations for aiobotocore.Omics 2.5.4 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_omics/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-omics.svg?color=blue)](https://pypi.org/project/types-aiobotocore-omics)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_omics/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-omics)](https://pepy.tech/project/types-aiobotocore-omics)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.Omics 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/omics.html#Omics)
+[aiobotocore.Omics 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/omics.html#Omics)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-omics-2.5.2.post2/README.md` & `types-aiobotocore-omics-2.5.4/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-omics.svg?color=blue)](https://pypi.org/project/types-aiobotocore-omics)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_omics/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-omics)](https://pepy.tech/project/types-aiobotocore-omics)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.Omics 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/omics.html#Omics)
+[aiobotocore.Omics 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/omics.html#Omics)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-omics-2.5.2.post2/setup.py` & `types-aiobotocore-omics-2.5.4/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-omics",
-    version="2.5.2.post2",
+    version="2.5.4",
     packages=["types_aiobotocore_omics"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.Omics 2.5.2 service generated with mypy-boto3-builder"
+        "Type annotations for aiobotocore.Omics 2.5.4 service generated with mypy-boto3-builder"
         " 7.17.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
```

### Comparing `types-aiobotocore-omics-2.5.2.post2/types_aiobotocore_omics/__init__.py` & `types-aiobotocore-omics-2.5.4/types_aiobotocore_omics/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-omics-2.5.2.post2/types_aiobotocore_omics/__init__.pyi` & `types-aiobotocore-omics-2.5.4/types_aiobotocore_omics/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-omics-2.5.2.post2/types_aiobotocore_omics/__main__.py` & `types-aiobotocore-omics-2.5.4/types_aiobotocore_omics/__main__.py`

 * *Files 18% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.Omics 2.5.2\nVersion:         2.5.2.post2\nBuilder"
-        " version: 7.17.2\nDocs:           "
+        "Type annotations for aiobotocore.Omics 2.5.4\nVersion:         2.5.4\nBuilder version:"
+        " 7.17.2\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_omics//\nBoto3 docs:  "
         "    https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/omics.html#Omics\nOther"
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

### Comparing `types-aiobotocore-omics-2.5.2.post2/types_aiobotocore_omics/client.py` & `types-aiobotocore-omics-2.5.4/types_aiobotocore_omics/client.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-omics-2.5.2.post2/types_aiobotocore_omics/client.pyi` & `types-aiobotocore-omics-2.5.4/types_aiobotocore_omics/client.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-omics-2.5.2.post2/types_aiobotocore_omics/literals.py` & `types-aiobotocore-omics-2.5.4/types_aiobotocore_omics/literals.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-omics-2.5.2.post2/types_aiobotocore_omics/literals.pyi` & `types-aiobotocore-omics-2.5.4/types_aiobotocore_omics/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-omics-2.5.2.post2/types_aiobotocore_omics/paginator.py` & `types-aiobotocore-omics-2.5.4/types_aiobotocore_omics/paginator.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-omics-2.5.2.post2/types_aiobotocore_omics/paginator.pyi` & `types-aiobotocore-omics-2.5.4/types_aiobotocore_omics/paginator.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-omics-2.5.2.post2/types_aiobotocore_omics/type_defs.py` & `types-aiobotocore-omics-2.5.4/types_aiobotocore_omics/type_defs.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-omics-2.5.2.post2/types_aiobotocore_omics/type_defs.pyi` & `types-aiobotocore-omics-2.5.4/types_aiobotocore_omics/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-omics-2.5.2.post2/types_aiobotocore_omics/waiter.py` & `types-aiobotocore-omics-2.5.4/types_aiobotocore_omics/waiter.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-omics-2.5.2.post2/types_aiobotocore_omics/waiter.pyi` & `types-aiobotocore-omics-2.5.4/types_aiobotocore_omics/waiter.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-omics-2.5.2.post2/types_aiobotocore_omics.egg-info/PKG-INFO` & `types-aiobotocore-omics-2.5.4/types_aiobotocore_omics.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-omics
-Version: 2.5.2.post2
-Summary: Type annotations for aiobotocore.Omics 2.5.2 service generated with mypy-boto3-builder 7.17.2
+Version: 2.5.4
+Summary: Type annotations for aiobotocore.Omics 2.5.4 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_omics/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-omics.svg?color=blue)](https://pypi.org/project/types-aiobotocore-omics)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_omics/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-omics)](https://pepy.tech/project/types-aiobotocore-omics)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.Omics 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/omics.html#Omics)
+[aiobotocore.Omics 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/omics.html#Omics)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-omics-2.5.2.post2/types_aiobotocore_omics.egg-info/SOURCES.txt` & `types-aiobotocore-omics-2.5.4/types_aiobotocore_omics.egg-info/SOURCES.txt`

 * *Files identical despite different names*


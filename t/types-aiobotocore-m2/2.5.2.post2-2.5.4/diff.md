# Comparing `tmp/types-aiobotocore-m2-2.5.2.post2.tar.gz` & `tmp/types-aiobotocore-m2-2.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-m2-2.5.2.post2.tar", last modified: Fri Aug  4 13:59:16 2023, max compression
+gzip compressed data, was "types-aiobotocore-m2-2.5.4.tar", last modified: Tue Aug  8 01:24:02 2023, max compression
```

## Comparing `types-aiobotocore-m2-2.5.2.post2.tar` & `types-aiobotocore-m2-2.5.4.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:16.246643 types-aiobotocore-m2-2.5.2.post2/
--rw-r--r--   0 vlad      (1000) vlad      (1000)     1070 2023-08-04 13:43:33.000000 types-aiobotocore-m2-2.5.2.post2/LICENSE
--rw-r--r--   0 vlad      (1000) vlad      (1000)    14159 2023-08-04 13:59:16.246643 types-aiobotocore-m2-2.5.2.post2/PKG-INFO
--rw-r--r--   0 vlad      (1000) vlad      (1000)    12641 2023-08-04 13:43:33.000000 types-aiobotocore-m2-2.5.2.post2/README.md
--rw-r--r--   0 vlad      (1000) vlad      (1000)       38 2023-08-04 13:59:16.256643 types-aiobotocore-m2-2.5.2.post2/setup.cfg
--rw-r--r--   0 vlad      (1000) vlad      (1000)     2033 2023-08-04 13:43:32.000000 types-aiobotocore-m2-2.5.2.post2/setup.py
-drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:16.246643 types-aiobotocore-m2-2.5.2.post2/types_aiobotocore_m2/
--rw-r--r--   0 vlad      (1000) vlad      (1000)     2529 2023-08-04 13:43:33.000000 types-aiobotocore-m2-2.5.2.post2/types_aiobotocore_m2/__init__.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)     2528 2023-08-04 13:43:33.000000 types-aiobotocore-m2-2.5.2.post2/types_aiobotocore_m2/__init__.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)      952 2023-08-04 13:43:33.000000 types-aiobotocore-m2-2.5.2.post2/types_aiobotocore_m2/__main__.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)    29883 2023-08-04 13:43:33.000000 types-aiobotocore-m2-2.5.2.post2/types_aiobotocore_m2/client.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)    29832 2023-08-04 13:43:33.000000 types-aiobotocore-m2-2.5.2.post2/types_aiobotocore_m2/client.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)    10455 2023-08-04 13:43:33.000000 types-aiobotocore-m2-2.5.2.post2/types_aiobotocore_m2/literals.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)    10453 2023-08-04 13:43:33.000000 types-aiobotocore-m2-2.5.2.post2/types_aiobotocore_m2/literals.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)    11866 2023-08-04 13:43:33.000000 types-aiobotocore-m2-2.5.2.post2/types_aiobotocore_m2/paginator.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)    11855 2023-08-04 13:43:33.000000 types-aiobotocore-m2-2.5.2.post2/types_aiobotocore_m2/paginator.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:43:33.000000 types-aiobotocore-m2-2.5.2.post2/types_aiobotocore_m2/py.typed
--rw-r--r--   0 vlad      (1000) vlad      (1000)    42562 2023-08-04 13:43:34.000000 types-aiobotocore-m2-2.5.2.post2/types_aiobotocore_m2/type_defs.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)    42494 2023-08-04 13:43:34.000000 types-aiobotocore-m2-2.5.2.post2/types_aiobotocore_m2/type_defs.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)       65 2023-08-04 13:43:33.000000 types-aiobotocore-m2-2.5.2.post2/types_aiobotocore_m2/version.py
-drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:16.246643 types-aiobotocore-m2-2.5.2.post2/types_aiobotocore_m2.egg-info/
--rw-r--r--   0 vlad      (1000) vlad      (1000)    14159 2023-08-04 13:59:16.000000 types-aiobotocore-m2-2.5.2.post2/types_aiobotocore_m2.egg-info/PKG-INFO
--rw-r--r--   0 vlad      (1000) vlad      (1000)      718 2023-08-04 13:59:16.000000 types-aiobotocore-m2-2.5.2.post2/types_aiobotocore_m2.egg-info/SOURCES.txt
--rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:16.000000 types-aiobotocore-m2-2.5.2.post2/types_aiobotocore_m2.egg-info/dependency_links.txt
--rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:16.000000 types-aiobotocore-m2-2.5.2.post2/types_aiobotocore_m2.egg-info/not-zip-safe
--rw-r--r--   0 vlad      (1000) vlad      (1000)       52 2023-08-04 13:59:16.000000 types-aiobotocore-m2-2.5.2.post2/types_aiobotocore_m2.egg-info/requires.txt
--rw-r--r--   0 vlad      (1000) vlad      (1000)       21 2023-08-04 13:59:16.000000 types-aiobotocore-m2-2.5.2.post2/types_aiobotocore_m2.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:24:02.138725 types-aiobotocore-m2-2.5.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-08 01:14:35.000000 types-aiobotocore-m2-2.5.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    14153 2023-08-08 01:24:02.138725 types-aiobotocore-m2-2.5.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    12641 2023-08-08 01:14:35.000000 types-aiobotocore-m2-2.5.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-08 01:24:02.138725 types-aiobotocore-m2-2.5.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2027 2023-08-08 01:14:35.000000 types-aiobotocore-m2-2.5.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:24:02.138725 types-aiobotocore-m2-2.5.4/types_aiobotocore_m2/
+-rw-r--r--   0 runner    (1001) docker     (123)     2529 2023-08-08 01:14:35.000000 types-aiobotocore-m2-2.5.4/types_aiobotocore_m2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2528 2023-08-08 01:14:35.000000 types-aiobotocore-m2-2.5.4/types_aiobotocore_m2/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      940 2023-08-08 01:14:35.000000 types-aiobotocore-m2-2.5.4/types_aiobotocore_m2/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29883 2023-08-08 01:14:35.000000 types-aiobotocore-m2-2.5.4/types_aiobotocore_m2/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29832 2023-08-08 01:14:35.000000 types-aiobotocore-m2-2.5.4/types_aiobotocore_m2/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    10455 2023-08-08 01:14:36.000000 types-aiobotocore-m2-2.5.4/types_aiobotocore_m2/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10453 2023-08-08 01:14:36.000000 types-aiobotocore-m2-2.5.4/types_aiobotocore_m2/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    11866 2023-08-08 01:14:36.000000 types-aiobotocore-m2-2.5.4/types_aiobotocore_m2/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11855 2023-08-08 01:14:36.000000 types-aiobotocore-m2-2.5.4/types_aiobotocore_m2/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 01:14:35.000000 types-aiobotocore-m2-2.5.4/types_aiobotocore_m2/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    42562 2023-08-08 01:14:37.000000 types-aiobotocore-m2-2.5.4/types_aiobotocore_m2/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42494 2023-08-08 01:14:36.000000 types-aiobotocore-m2-2.5.4/types_aiobotocore_m2/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-08-08 01:14:35.000000 types-aiobotocore-m2-2.5.4/types_aiobotocore_m2/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:24:02.138725 types-aiobotocore-m2-2.5.4/types_aiobotocore_m2.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    14153 2023-08-08 01:24:01.000000 types-aiobotocore-m2-2.5.4/types_aiobotocore_m2.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      718 2023-08-08 01:24:01.000000 types-aiobotocore-m2-2.5.4/types_aiobotocore_m2.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 01:24:01.000000 types-aiobotocore-m2-2.5.4/types_aiobotocore_m2.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 01:24:01.000000 types-aiobotocore-m2-2.5.4/types_aiobotocore_m2.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-08 01:24:01.000000 types-aiobotocore-m2-2.5.4/types_aiobotocore_m2.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-08-08 01:24:01.000000 types-aiobotocore-m2-2.5.4/types_aiobotocore_m2.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-m2-2.5.2.post2/LICENSE` & `types-aiobotocore-m2-2.5.4/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-m2-2.5.2.post2/PKG-INFO` & `types-aiobotocore-m2-2.5.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-m2
-Version: 2.5.2.post2
-Summary: Type annotations for aiobotocore.MainframeModernization 2.5.2 service generated with mypy-boto3-builder 7.17.2
+Version: 2.5.4
+Summary: Type annotations for aiobotocore.MainframeModernization 2.5.4 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_m2/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-m2.svg?color=blue)](https://pypi.org/project/types-aiobotocore-m2)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_m2/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-m2)](https://pepy.tech/project/types-aiobotocore-m2)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.MainframeModernization 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/m2.html#MainframeModernization)
+[aiobotocore.MainframeModernization 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/m2.html#MainframeModernization)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-m2-2.5.2.post2/README.md` & `types-aiobotocore-m2-2.5.4/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-m2.svg?color=blue)](https://pypi.org/project/types-aiobotocore-m2)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_m2/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-m2)](https://pepy.tech/project/types-aiobotocore-m2)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.MainframeModernization 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/m2.html#MainframeModernization)
+[aiobotocore.MainframeModernization 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/m2.html#MainframeModernization)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-m2-2.5.2.post2/setup.py` & `types-aiobotocore-m2-2.5.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-m2",
-    version="2.5.2.post2",
+    version="2.5.4",
     packages=["types_aiobotocore_m2"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.MainframeModernization 2.5.2 service generated with"
+        "Type annotations for aiobotocore.MainframeModernization 2.5.4 service generated with"
         " mypy-boto3-builder 7.17.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
```

### Comparing `types-aiobotocore-m2-2.5.2.post2/types_aiobotocore_m2/__init__.py` & `types-aiobotocore-m2-2.5.4/types_aiobotocore_m2/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-m2-2.5.2.post2/types_aiobotocore_m2/__init__.pyi` & `types-aiobotocore-m2-2.5.4/types_aiobotocore_m2/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-m2-2.5.2.post2/types_aiobotocore_m2/__main__.py` & `types-aiobotocore-m2-2.5.4/types_aiobotocore_m2/__main__.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.MainframeModernization 2.5.2\nVersion:        "
-        " 2.5.2.post2\nBuilder version: 7.17.2\nDocs:           "
+        "Type annotations for aiobotocore.MainframeModernization 2.5.4\nVersion:        "
+        " 2.5.4\nBuilder version: 7.17.2\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_m2//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/m2.html#MainframeModernization\nOther"
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

### Comparing `types-aiobotocore-m2-2.5.2.post2/types_aiobotocore_m2/client.py` & `types-aiobotocore-m2-2.5.4/types_aiobotocore_m2/client.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-m2-2.5.2.post2/types_aiobotocore_m2/client.pyi` & `types-aiobotocore-m2-2.5.4/types_aiobotocore_m2/client.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-m2-2.5.2.post2/types_aiobotocore_m2/literals.py` & `types-aiobotocore-m2-2.5.4/types_aiobotocore_m2/literals.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-m2-2.5.2.post2/types_aiobotocore_m2/literals.pyi` & `types-aiobotocore-m2-2.5.4/types_aiobotocore_m2/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-m2-2.5.2.post2/types_aiobotocore_m2/paginator.py` & `types-aiobotocore-m2-2.5.4/types_aiobotocore_m2/paginator.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-m2-2.5.2.post2/types_aiobotocore_m2/paginator.pyi` & `types-aiobotocore-m2-2.5.4/types_aiobotocore_m2/paginator.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-m2-2.5.2.post2/types_aiobotocore_m2/type_defs.py` & `types-aiobotocore-m2-2.5.4/types_aiobotocore_m2/type_defs.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-m2-2.5.2.post2/types_aiobotocore_m2/type_defs.pyi` & `types-aiobotocore-m2-2.5.4/types_aiobotocore_m2/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-m2-2.5.2.post2/types_aiobotocore_m2.egg-info/PKG-INFO` & `types-aiobotocore-m2-2.5.4/types_aiobotocore_m2.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-m2
-Version: 2.5.2.post2
-Summary: Type annotations for aiobotocore.MainframeModernization 2.5.2 service generated with mypy-boto3-builder 7.17.2
+Version: 2.5.4
+Summary: Type annotations for aiobotocore.MainframeModernization 2.5.4 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_m2/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-m2.svg?color=blue)](https://pypi.org/project/types-aiobotocore-m2)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_m2/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-m2)](https://pepy.tech/project/types-aiobotocore-m2)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.MainframeModernization 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/m2.html#MainframeModernization)
+[aiobotocore.MainframeModernization 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/m2.html#MainframeModernization)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-m2-2.5.2.post2/types_aiobotocore_m2.egg-info/SOURCES.txt` & `types-aiobotocore-m2-2.5.4/types_aiobotocore_m2.egg-info/SOURCES.txt`

 * *Files identical despite different names*


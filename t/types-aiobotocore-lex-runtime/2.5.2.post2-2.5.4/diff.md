# Comparing `tmp/types-aiobotocore-lex-runtime-2.5.2.post2.tar.gz` & `tmp/types-aiobotocore-lex-runtime-2.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-lex-runtime-2.5.2.post2.tar", last modified: Fri Aug  4 13:59:15 2023, max compression
+gzip compressed data, was "types-aiobotocore-lex-runtime-2.5.4.tar", last modified: Tue Aug  8 01:23:59 2023, max compression
```

## Comparing `types-aiobotocore-lex-runtime-2.5.2.post2.tar` & `types-aiobotocore-lex-runtime-2.5.4.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:15.166643 types-aiobotocore-lex-runtime-2.5.2.post2/
--rw-r--r--   0 vlad      (1000) vlad      (1000)     1070 2023-08-04 13:42:33.000000 types-aiobotocore-lex-runtime-2.5.2.post2/LICENSE
--rw-r--r--   0 vlad      (1000) vlad      (1000)    12480 2023-08-04 13:59:15.166643 types-aiobotocore-lex-runtime-2.5.2.post2/PKG-INFO
--rw-r--r--   0 vlad      (1000) vlad      (1000)    10940 2023-08-04 13:42:33.000000 types-aiobotocore-lex-runtime-2.5.2.post2/README.md
--rw-r--r--   0 vlad      (1000) vlad      (1000)       38 2023-08-04 13:59:15.176643 types-aiobotocore-lex-runtime-2.5.2.post2/setup.cfg
--rw-r--r--   0 vlad      (1000) vlad      (1000)     2106 2023-08-04 13:42:33.000000 types-aiobotocore-lex-runtime-2.5.2.post2/setup.py
-drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:15.166643 types-aiobotocore-lex-runtime-2.5.2.post2/types_aiobotocore_lex_runtime/
--rw-r--r--   0 vlad      (1000) vlad      (1000)      504 2023-08-04 13:42:33.000000 types-aiobotocore-lex-runtime-2.5.2.post2/types_aiobotocore_lex_runtime/__init__.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)      503 2023-08-04 13:42:33.000000 types-aiobotocore-lex-runtime-2.5.2.post2/types_aiobotocore_lex_runtime/__init__.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)      971 2023-08-04 13:42:33.000000 types-aiobotocore-lex-runtime-2.5.2.post2/types_aiobotocore_lex_runtime/__main__.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)     8265 2023-08-04 13:42:33.000000 types-aiobotocore-lex-runtime-2.5.2.post2/types_aiobotocore_lex_runtime/client.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)     8252 2023-08-04 13:42:33.000000 types-aiobotocore-lex-runtime-2.5.2.post2/types_aiobotocore_lex_runtime/client.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)     8534 2023-08-04 13:42:34.000000 types-aiobotocore-lex-runtime-2.5.2.post2/types_aiobotocore_lex_runtime/literals.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)     8532 2023-08-04 13:42:34.000000 types-aiobotocore-lex-runtime-2.5.2.post2/types_aiobotocore_lex_runtime/literals.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:42:33.000000 types-aiobotocore-lex-runtime-2.5.2.post2/types_aiobotocore_lex_runtime/py.typed
--rw-r--r--   0 vlad      (1000) vlad      (1000)     9729 2023-08-04 13:42:34.000000 types-aiobotocore-lex-runtime-2.5.2.post2/types_aiobotocore_lex_runtime/type_defs.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)     9716 2023-08-04 13:42:34.000000 types-aiobotocore-lex-runtime-2.5.2.post2/types_aiobotocore_lex_runtime/type_defs.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)       65 2023-08-04 13:42:33.000000 types-aiobotocore-lex-runtime-2.5.2.post2/types_aiobotocore_lex_runtime/version.py
-drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:15.166643 types-aiobotocore-lex-runtime-2.5.2.post2/types_aiobotocore_lex_runtime.egg-info/
--rw-r--r--   0 vlad      (1000) vlad      (1000)    12480 2023-08-04 13:59:15.000000 types-aiobotocore-lex-runtime-2.5.2.post2/types_aiobotocore_lex_runtime.egg-info/PKG-INFO
--rw-r--r--   0 vlad      (1000) vlad      (1000)      802 2023-08-04 13:59:15.000000 types-aiobotocore-lex-runtime-2.5.2.post2/types_aiobotocore_lex_runtime.egg-info/SOURCES.txt
--rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:15.000000 types-aiobotocore-lex-runtime-2.5.2.post2/types_aiobotocore_lex_runtime.egg-info/dependency_links.txt
--rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:15.000000 types-aiobotocore-lex-runtime-2.5.2.post2/types_aiobotocore_lex_runtime.egg-info/not-zip-safe
--rw-r--r--   0 vlad      (1000) vlad      (1000)       52 2023-08-04 13:59:15.000000 types-aiobotocore-lex-runtime-2.5.2.post2/types_aiobotocore_lex_runtime.egg-info/requires.txt
--rw-r--r--   0 vlad      (1000) vlad      (1000)       30 2023-08-04 13:59:15.000000 types-aiobotocore-lex-runtime-2.5.2.post2/types_aiobotocore_lex_runtime.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:23:59.594722 types-aiobotocore-lex-runtime-2.5.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-08 01:13:56.000000 types-aiobotocore-lex-runtime-2.5.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    12474 2023-08-08 01:23:59.594722 types-aiobotocore-lex-runtime-2.5.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10940 2023-08-08 01:13:56.000000 types-aiobotocore-lex-runtime-2.5.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-08 01:23:59.594722 types-aiobotocore-lex-runtime-2.5.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2100 2023-08-08 01:13:55.000000 types-aiobotocore-lex-runtime-2.5.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:23:59.594722 types-aiobotocore-lex-runtime-2.5.4/types_aiobotocore_lex_runtime/
+-rw-r--r--   0 runner    (1001) docker     (123)      504 2023-08-08 01:13:56.000000 types-aiobotocore-lex-runtime-2.5.4/types_aiobotocore_lex_runtime/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      503 2023-08-08 01:13:56.000000 types-aiobotocore-lex-runtime-2.5.4/types_aiobotocore_lex_runtime/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      959 2023-08-08 01:13:56.000000 types-aiobotocore-lex-runtime-2.5.4/types_aiobotocore_lex_runtime/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8265 2023-08-08 01:13:56.000000 types-aiobotocore-lex-runtime-2.5.4/types_aiobotocore_lex_runtime/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8252 2023-08-08 01:13:56.000000 types-aiobotocore-lex-runtime-2.5.4/types_aiobotocore_lex_runtime/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8534 2023-08-08 01:13:56.000000 types-aiobotocore-lex-runtime-2.5.4/types_aiobotocore_lex_runtime/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8532 2023-08-08 01:13:56.000000 types-aiobotocore-lex-runtime-2.5.4/types_aiobotocore_lex_runtime/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 01:13:56.000000 types-aiobotocore-lex-runtime-2.5.4/types_aiobotocore_lex_runtime/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     9729 2023-08-08 01:13:56.000000 types-aiobotocore-lex-runtime-2.5.4/types_aiobotocore_lex_runtime/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9716 2023-08-08 01:13:56.000000 types-aiobotocore-lex-runtime-2.5.4/types_aiobotocore_lex_runtime/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-08-08 01:13:56.000000 types-aiobotocore-lex-runtime-2.5.4/types_aiobotocore_lex_runtime/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:23:59.594722 types-aiobotocore-lex-runtime-2.5.4/types_aiobotocore_lex_runtime.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    12474 2023-08-08 01:23:59.000000 types-aiobotocore-lex-runtime-2.5.4/types_aiobotocore_lex_runtime.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      802 2023-08-08 01:23:59.000000 types-aiobotocore-lex-runtime-2.5.4/types_aiobotocore_lex_runtime.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 01:23:59.000000 types-aiobotocore-lex-runtime-2.5.4/types_aiobotocore_lex_runtime.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 01:23:59.000000 types-aiobotocore-lex-runtime-2.5.4/types_aiobotocore_lex_runtime.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-08 01:23:59.000000 types-aiobotocore-lex-runtime-2.5.4/types_aiobotocore_lex_runtime.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-08-08 01:23:59.000000 types-aiobotocore-lex-runtime-2.5.4/types_aiobotocore_lex_runtime.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-lex-runtime-2.5.2.post2/LICENSE` & `types-aiobotocore-lex-runtime-2.5.4/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-lex-runtime-2.5.2.post2/PKG-INFO` & `types-aiobotocore-lex-runtime-2.5.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-lex-runtime
-Version: 2.5.2.post2
-Summary: Type annotations for aiobotocore.LexRuntimeService 2.5.2 service generated with mypy-boto3-builder 7.17.2
+Version: 2.5.4
+Summary: Type annotations for aiobotocore.LexRuntimeService 2.5.4 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lex_runtime/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-lex-runtime.svg?color=blue)](https://pypi.org/project/types-aiobotocore-lex-runtime)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lex_runtime/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-lex-runtime)](https://pepy.tech/project/types-aiobotocore-lex-runtime)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.LexRuntimeService 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lex-runtime.html#LexRuntimeService)
+[aiobotocore.LexRuntimeService 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lex-runtime.html#LexRuntimeService)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-lex-runtime-2.5.2.post2/README.md` & `types-aiobotocore-lex-runtime-2.5.4/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-lex-runtime.svg?color=blue)](https://pypi.org/project/types-aiobotocore-lex-runtime)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lex_runtime/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-lex-runtime)](https://pepy.tech/project/types-aiobotocore-lex-runtime)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.LexRuntimeService 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lex-runtime.html#LexRuntimeService)
+[aiobotocore.LexRuntimeService 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lex-runtime.html#LexRuntimeService)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-lex-runtime-2.5.2.post2/setup.py` & `types-aiobotocore-lex-runtime-2.5.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-lex-runtime",
-    version="2.5.2.post2",
+    version="2.5.4",
     packages=["types_aiobotocore_lex_runtime"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.LexRuntimeService 2.5.2 service generated with"
+        "Type annotations for aiobotocore.LexRuntimeService 2.5.4 service generated with"
         " mypy-boto3-builder 7.17.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
```

### Comparing `types-aiobotocore-lex-runtime-2.5.2.post2/types_aiobotocore_lex_runtime/__main__.py` & `types-aiobotocore-lex-runtime-2.5.4/types_aiobotocore_lex_runtime/__main__.py`

 * *Files 10% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.LexRuntimeService 2.5.2\nVersion:        "
-        " 2.5.2.post2\nBuilder version: 7.17.2\nDocs:           "
+        "Type annotations for aiobotocore.LexRuntimeService 2.5.4\nVersion:         2.5.4\nBuilder"
+        " version: 7.17.2\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lex_runtime//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lex-runtime.html#LexRuntimeService\nOther"
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

### Comparing `types-aiobotocore-lex-runtime-2.5.2.post2/types_aiobotocore_lex_runtime/client.py` & `types-aiobotocore-lex-runtime-2.5.4/types_aiobotocore_lex_runtime/client.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-lex-runtime-2.5.2.post2/types_aiobotocore_lex_runtime/client.pyi` & `types-aiobotocore-lex-runtime-2.5.4/types_aiobotocore_lex_runtime/client.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-lex-runtime-2.5.2.post2/types_aiobotocore_lex_runtime/literals.py` & `types-aiobotocore-lex-runtime-2.5.4/types_aiobotocore_lex_runtime/literals.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-lex-runtime-2.5.2.post2/types_aiobotocore_lex_runtime/literals.pyi` & `types-aiobotocore-lex-runtime-2.5.4/types_aiobotocore_lex_runtime/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-lex-runtime-2.5.2.post2/types_aiobotocore_lex_runtime/type_defs.py` & `types-aiobotocore-lex-runtime-2.5.4/types_aiobotocore_lex_runtime/type_defs.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-lex-runtime-2.5.2.post2/types_aiobotocore_lex_runtime/type_defs.pyi` & `types-aiobotocore-lex-runtime-2.5.4/types_aiobotocore_lex_runtime/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-lex-runtime-2.5.2.post2/types_aiobotocore_lex_runtime.egg-info/PKG-INFO` & `types-aiobotocore-lex-runtime-2.5.4/types_aiobotocore_lex_runtime.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-lex-runtime
-Version: 2.5.2.post2
-Summary: Type annotations for aiobotocore.LexRuntimeService 2.5.2 service generated with mypy-boto3-builder 7.17.2
+Version: 2.5.4
+Summary: Type annotations for aiobotocore.LexRuntimeService 2.5.4 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lex_runtime/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-lex-runtime.svg?color=blue)](https://pypi.org/project/types-aiobotocore-lex-runtime)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lex_runtime/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-lex-runtime)](https://pepy.tech/project/types-aiobotocore-lex-runtime)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.LexRuntimeService 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lex-runtime.html#LexRuntimeService)
+[aiobotocore.LexRuntimeService 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lex-runtime.html#LexRuntimeService)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-lex-runtime-2.5.2.post2/types_aiobotocore_lex_runtime.egg-info/SOURCES.txt` & `types-aiobotocore-lex-runtime-2.5.4/types_aiobotocore_lex_runtime.egg-info/SOURCES.txt`

 * *Files identical despite different names*


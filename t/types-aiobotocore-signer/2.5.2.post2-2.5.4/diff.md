# Comparing `tmp/types-aiobotocore-signer-2.5.2.post2.tar.gz` & `tmp/types-aiobotocore-signer-2.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-signer-2.5.2.post2.tar", last modified: Fri Aug  4 13:59:26 2023, max compression
+gzip compressed data, was "types-aiobotocore-signer-2.5.4.tar", last modified: Tue Aug  8 01:24:27 2023, max compression
```

## Comparing `types-aiobotocore-signer-2.5.2.post2.tar` & `types-aiobotocore-signer-2.5.4.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:26.746643 types-aiobotocore-signer-2.5.2.post2/
--rw-r--r--   0 vlad      (1000) vlad      (1000)     1070 2023-08-04 13:53:43.000000 types-aiobotocore-signer-2.5.2.post2/LICENSE
--rw-r--r--   0 vlad      (1000) vlad      (1000)    13944 2023-08-04 13:59:26.746643 types-aiobotocore-signer-2.5.2.post2/PKG-INFO
--rw-r--r--   0 vlad      (1000) vlad      (1000)    12430 2023-08-04 13:53:43.000000 types-aiobotocore-signer-2.5.2.post2/README.md
--rw-r--r--   0 vlad      (1000) vlad      (1000)       38 2023-08-04 13:59:26.746643 types-aiobotocore-signer-2.5.2.post2/setup.cfg
--rw-r--r--   0 vlad      (1000) vlad      (1000)     2065 2023-08-04 13:53:43.000000 types-aiobotocore-signer-2.5.2.post2/setup.py
-drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:26.746643 types-aiobotocore-signer-2.5.2.post2/types_aiobotocore_signer/
--rw-r--r--   0 vlad      (1000) vlad      (1000)     1347 2023-08-04 13:53:43.000000 types-aiobotocore-signer-2.5.2.post2/types_aiobotocore_signer/__init__.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)     1346 2023-08-04 13:53:43.000000 types-aiobotocore-signer-2.5.2.post2/types_aiobotocore_signer/__init__.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)      928 2023-08-04 13:53:43.000000 types-aiobotocore-signer-2.5.2.post2/types_aiobotocore_signer/__main__.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)    18592 2023-08-04 13:53:43.000000 types-aiobotocore-signer-2.5.2.post2/types_aiobotocore_signer/client.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)    18560 2023-08-04 13:53:43.000000 types-aiobotocore-signer-2.5.2.post2/types_aiobotocore_signer/client.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)     9173 2023-08-04 13:53:43.000000 types-aiobotocore-signer-2.5.2.post2/types_aiobotocore_signer/literals.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)     9171 2023-08-04 13:53:43.000000 types-aiobotocore-signer-2.5.2.post2/types_aiobotocore_signer/literals.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)     4874 2023-08-04 13:53:43.000000 types-aiobotocore-signer-2.5.2.post2/types_aiobotocore_signer/paginator.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)     4869 2023-08-04 13:53:43.000000 types-aiobotocore-signer-2.5.2.post2/types_aiobotocore_signer/paginator.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:53:43.000000 types-aiobotocore-signer-2.5.2.post2/types_aiobotocore_signer/py.typed
--rw-r--r--   0 vlad      (1000) vlad      (1000)    21630 2023-08-04 13:53:44.000000 types-aiobotocore-signer-2.5.2.post2/types_aiobotocore_signer/type_defs.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)    21613 2023-08-04 13:53:44.000000 types-aiobotocore-signer-2.5.2.post2/types_aiobotocore_signer/type_defs.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)       65 2023-08-04 13:53:43.000000 types-aiobotocore-signer-2.5.2.post2/types_aiobotocore_signer/version.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)     1564 2023-08-04 13:53:43.000000 types-aiobotocore-signer-2.5.2.post2/types_aiobotocore_signer/waiter.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)     1563 2023-08-04 13:53:43.000000 types-aiobotocore-signer-2.5.2.post2/types_aiobotocore_signer/waiter.pyi
-drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:26.746643 types-aiobotocore-signer-2.5.2.post2/types_aiobotocore_signer.egg-info/
--rw-r--r--   0 vlad      (1000) vlad      (1000)    13944 2023-08-04 13:59:26.000000 types-aiobotocore-signer-2.5.2.post2/types_aiobotocore_signer.egg-info/PKG-INFO
--rw-r--r--   0 vlad      (1000) vlad      (1000)      865 2023-08-04 13:59:26.000000 types-aiobotocore-signer-2.5.2.post2/types_aiobotocore_signer.egg-info/SOURCES.txt
--rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:26.000000 types-aiobotocore-signer-2.5.2.post2/types_aiobotocore_signer.egg-info/dependency_links.txt
--rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:26.000000 types-aiobotocore-signer-2.5.2.post2/types_aiobotocore_signer.egg-info/not-zip-safe
--rw-r--r--   0 vlad      (1000) vlad      (1000)       52 2023-08-04 13:59:26.000000 types-aiobotocore-signer-2.5.2.post2/types_aiobotocore_signer.egg-info/requires.txt
--rw-r--r--   0 vlad      (1000) vlad      (1000)       25 2023-08-04 13:59:26.000000 types-aiobotocore-signer-2.5.2.post2/types_aiobotocore_signer.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:24:27.514783 types-aiobotocore-signer-2.5.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-08 01:21:11.000000 types-aiobotocore-signer-2.5.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    13938 2023-08-08 01:24:27.514783 types-aiobotocore-signer-2.5.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    12430 2023-08-08 01:21:11.000000 types-aiobotocore-signer-2.5.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-08 01:24:27.514783 types-aiobotocore-signer-2.5.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2059 2023-08-08 01:21:11.000000 types-aiobotocore-signer-2.5.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:24:27.514783 types-aiobotocore-signer-2.5.4/types_aiobotocore_signer/
+-rw-r--r--   0 runner    (1001) docker     (123)     1347 2023-08-08 01:21:11.000000 types-aiobotocore-signer-2.5.4/types_aiobotocore_signer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1346 2023-08-08 01:21:11.000000 types-aiobotocore-signer-2.5.4/types_aiobotocore_signer/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      916 2023-08-08 01:21:11.000000 types-aiobotocore-signer-2.5.4/types_aiobotocore_signer/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18592 2023-08-08 01:21:11.000000 types-aiobotocore-signer-2.5.4/types_aiobotocore_signer/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18560 2023-08-08 01:21:11.000000 types-aiobotocore-signer-2.5.4/types_aiobotocore_signer/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9173 2023-08-08 01:21:11.000000 types-aiobotocore-signer-2.5.4/types_aiobotocore_signer/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9171 2023-08-08 01:21:11.000000 types-aiobotocore-signer-2.5.4/types_aiobotocore_signer/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     4874 2023-08-08 01:21:11.000000 types-aiobotocore-signer-2.5.4/types_aiobotocore_signer/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4869 2023-08-08 01:21:11.000000 types-aiobotocore-signer-2.5.4/types_aiobotocore_signer/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 01:21:11.000000 types-aiobotocore-signer-2.5.4/types_aiobotocore_signer/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    21630 2023-08-08 01:21:11.000000 types-aiobotocore-signer-2.5.4/types_aiobotocore_signer/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21613 2023-08-08 01:21:11.000000 types-aiobotocore-signer-2.5.4/types_aiobotocore_signer/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-08-08 01:21:11.000000 types-aiobotocore-signer-2.5.4/types_aiobotocore_signer/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1564 2023-08-08 01:21:11.000000 types-aiobotocore-signer-2.5.4/types_aiobotocore_signer/waiter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1563 2023-08-08 01:21:11.000000 types-aiobotocore-signer-2.5.4/types_aiobotocore_signer/waiter.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:24:27.514783 types-aiobotocore-signer-2.5.4/types_aiobotocore_signer.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    13938 2023-08-08 01:24:27.000000 types-aiobotocore-signer-2.5.4/types_aiobotocore_signer.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      865 2023-08-08 01:24:27.000000 types-aiobotocore-signer-2.5.4/types_aiobotocore_signer.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 01:24:27.000000 types-aiobotocore-signer-2.5.4/types_aiobotocore_signer.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 01:24:27.000000 types-aiobotocore-signer-2.5.4/types_aiobotocore_signer.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-08 01:24:27.000000 types-aiobotocore-signer-2.5.4/types_aiobotocore_signer.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-08-08 01:24:27.000000 types-aiobotocore-signer-2.5.4/types_aiobotocore_signer.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-signer-2.5.2.post2/LICENSE` & `types-aiobotocore-signer-2.5.4/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-signer-2.5.2.post2/PKG-INFO` & `types-aiobotocore-signer-2.5.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-signer
-Version: 2.5.2.post2
-Summary: Type annotations for aiobotocore.signer 2.5.2 service generated with mypy-boto3-builder 7.17.2
+Version: 2.5.4
+Summary: Type annotations for aiobotocore.signer 2.5.4 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_signer/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-signer.svg?color=blue)](https://pypi.org/project/types-aiobotocore-signer)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_signer/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-signer)](https://pepy.tech/project/types-aiobotocore-signer)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.signer 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/signer.html#signer)
+[aiobotocore.signer 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/signer.html#signer)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-signer-2.5.2.post2/README.md` & `types-aiobotocore-signer-2.5.4/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-signer.svg?color=blue)](https://pypi.org/project/types-aiobotocore-signer)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_signer/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-signer)](https://pepy.tech/project/types-aiobotocore-signer)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.signer 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/signer.html#signer)
+[aiobotocore.signer 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/signer.html#signer)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-signer-2.5.2.post2/setup.py` & `types-aiobotocore-signer-2.5.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-signer",
-    version="2.5.2.post2",
+    version="2.5.4",
     packages=["types_aiobotocore_signer"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.signer 2.5.2 service generated with mypy-boto3-builder"
+        "Type annotations for aiobotocore.signer 2.5.4 service generated with mypy-boto3-builder"
         " 7.17.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
```

### Comparing `types-aiobotocore-signer-2.5.2.post2/types_aiobotocore_signer/__init__.py` & `types-aiobotocore-signer-2.5.4/types_aiobotocore_signer/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-signer-2.5.2.post2/types_aiobotocore_signer/__init__.pyi` & `types-aiobotocore-signer-2.5.4/types_aiobotocore_signer/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-signer-2.5.2.post2/types_aiobotocore_signer/__main__.py` & `types-aiobotocore-signer-2.5.4/types_aiobotocore_signer/__main__.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.signer 2.5.2\nVersion:         2.5.2.post2\nBuilder"
-        " version: 7.17.2\nDocs:           "
+        "Type annotations for aiobotocore.signer 2.5.4\nVersion:         2.5.4\nBuilder version:"
+        " 7.17.2\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_signer//\nBoto3 docs: "
         "     https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/signer.html#signer\nOther"
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

### Comparing `types-aiobotocore-signer-2.5.2.post2/types_aiobotocore_signer/client.py` & `types-aiobotocore-signer-2.5.4/types_aiobotocore_signer/client.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-signer-2.5.2.post2/types_aiobotocore_signer/client.pyi` & `types-aiobotocore-signer-2.5.4/types_aiobotocore_signer/client.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-signer-2.5.2.post2/types_aiobotocore_signer/literals.py` & `types-aiobotocore-signer-2.5.4/types_aiobotocore_signer/literals.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-signer-2.5.2.post2/types_aiobotocore_signer/literals.pyi` & `types-aiobotocore-signer-2.5.4/types_aiobotocore_signer/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-signer-2.5.2.post2/types_aiobotocore_signer/paginator.py` & `types-aiobotocore-signer-2.5.4/types_aiobotocore_signer/paginator.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-signer-2.5.2.post2/types_aiobotocore_signer/paginator.pyi` & `types-aiobotocore-signer-2.5.4/types_aiobotocore_signer/paginator.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-signer-2.5.2.post2/types_aiobotocore_signer/type_defs.py` & `types-aiobotocore-signer-2.5.4/types_aiobotocore_signer/type_defs.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-signer-2.5.2.post2/types_aiobotocore_signer/type_defs.pyi` & `types-aiobotocore-signer-2.5.4/types_aiobotocore_signer/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-signer-2.5.2.post2/types_aiobotocore_signer/waiter.py` & `types-aiobotocore-signer-2.5.4/types_aiobotocore_signer/waiter.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-signer-2.5.2.post2/types_aiobotocore_signer/waiter.pyi` & `types-aiobotocore-signer-2.5.4/types_aiobotocore_signer/waiter.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-signer-2.5.2.post2/types_aiobotocore_signer.egg-info/PKG-INFO` & `types-aiobotocore-signer-2.5.4/types_aiobotocore_signer.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-signer
-Version: 2.5.2.post2
-Summary: Type annotations for aiobotocore.signer 2.5.2 service generated with mypy-boto3-builder 7.17.2
+Version: 2.5.4
+Summary: Type annotations for aiobotocore.signer 2.5.4 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_signer/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-signer.svg?color=blue)](https://pypi.org/project/types-aiobotocore-signer)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_signer/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-signer)](https://pepy.tech/project/types-aiobotocore-signer)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.signer 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/signer.html#signer)
+[aiobotocore.signer 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/signer.html#signer)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-signer-2.5.2.post2/types_aiobotocore_signer.egg-info/SOURCES.txt` & `types-aiobotocore-signer-2.5.4/types_aiobotocore_signer.egg-info/SOURCES.txt`

 * *Files identical despite different names*


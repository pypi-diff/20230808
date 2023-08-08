# Comparing `tmp/types-aiobotocore-opensearchserverless-2.5.2.post2.tar.gz` & `tmp/types-aiobotocore-opensearchserverless-2.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-opensearchserverless-2.5.2.post2.tar", last modified: Fri Aug  4 13:59:20 2023, max compression
+gzip compressed data, was "types-aiobotocore-opensearchserverless-2.5.4.tar", last modified: Tue Aug  8 01:24:10 2023, max compression
```

## Comparing `types-aiobotocore-opensearchserverless-2.5.2.post2.tar` & `types-aiobotocore-opensearchserverless-2.5.4.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:20.096643 types-aiobotocore-opensearchserverless-2.5.2.post2/
--rw-r--r--   0 vlad      (1000) vlad      (1000)     1070 2023-08-04 13:46:02.000000 types-aiobotocore-opensearchserverless-2.5.2.post2/LICENSE
--rw-r--r--   0 vlad      (1000) vlad      (1000)    12952 2023-08-04 13:59:20.096643 types-aiobotocore-opensearchserverless-2.5.2.post2/PKG-INFO
--rw-r--r--   0 vlad      (1000) vlad      (1000)    11375 2023-08-04 13:46:02.000000 types-aiobotocore-opensearchserverless-2.5.2.post2/README.md
--rw-r--r--   0 vlad      (1000) vlad      (1000)       38 2023-08-04 13:59:20.096643 types-aiobotocore-opensearchserverless-2.5.2.post2/setup.cfg
--rw-r--r--   0 vlad      (1000) vlad      (1000)     2162 2023-08-04 13:46:02.000000 types-aiobotocore-opensearchserverless-2.5.2.post2/setup.py
-drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:20.096643 types-aiobotocore-opensearchserverless-2.5.2.post2/types_aiobotocore_opensearchserverless/
--rw-r--r--   0 vlad      (1000) vlad      (1000)      581 2023-08-04 13:46:03.000000 types-aiobotocore-opensearchserverless-2.5.2.post2/types_aiobotocore_opensearchserverless/__init__.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)      580 2023-08-04 13:46:03.000000 types-aiobotocore-opensearchserverless-2.5.2.post2/types_aiobotocore_opensearchserverless/__init__.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)     1009 2023-08-04 13:46:03.000000 types-aiobotocore-opensearchserverless-2.5.2.post2/types_aiobotocore_opensearchserverless/__main__.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)    25784 2023-08-04 13:46:03.000000 types-aiobotocore-opensearchserverless-2.5.2.post2/types_aiobotocore_opensearchserverless/client.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)    25744 2023-08-04 13:46:03.000000 types-aiobotocore-opensearchserverless-2.5.2.post2/types_aiobotocore_opensearchserverless/client.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)     8432 2023-08-04 13:46:03.000000 types-aiobotocore-opensearchserverless-2.5.2.post2/types_aiobotocore_opensearchserverless/literals.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)     8430 2023-08-04 13:46:03.000000 types-aiobotocore-opensearchserverless-2.5.2.post2/types_aiobotocore_opensearchserverless/literals.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:46:03.000000 types-aiobotocore-opensearchserverless-2.5.2.post2/types_aiobotocore_opensearchserverless/py.typed
--rw-r--r--   0 vlad      (1000) vlad      (1000)    29369 2023-08-04 13:46:04.000000 types-aiobotocore-opensearchserverless-2.5.2.post2/types_aiobotocore_opensearchserverless/type_defs.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)    29330 2023-08-04 13:46:03.000000 types-aiobotocore-opensearchserverless-2.5.2.post2/types_aiobotocore_opensearchserverless/type_defs.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)       65 2023-08-04 13:46:03.000000 types-aiobotocore-opensearchserverless-2.5.2.post2/types_aiobotocore_opensearchserverless/version.py
-drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:20.096643 types-aiobotocore-opensearchserverless-2.5.2.post2/types_aiobotocore_opensearchserverless.egg-info/
--rw-r--r--   0 vlad      (1000) vlad      (1000)    12952 2023-08-04 13:59:20.000000 types-aiobotocore-opensearchserverless-2.5.2.post2/types_aiobotocore_opensearchserverless.egg-info/PKG-INFO
--rw-r--r--   0 vlad      (1000) vlad      (1000)      955 2023-08-04 13:59:20.000000 types-aiobotocore-opensearchserverless-2.5.2.post2/types_aiobotocore_opensearchserverless.egg-info/SOURCES.txt
--rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:20.000000 types-aiobotocore-opensearchserverless-2.5.2.post2/types_aiobotocore_opensearchserverless.egg-info/dependency_links.txt
--rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:20.000000 types-aiobotocore-opensearchserverless-2.5.2.post2/types_aiobotocore_opensearchserverless.egg-info/not-zip-safe
--rw-r--r--   0 vlad      (1000) vlad      (1000)       52 2023-08-04 13:59:20.000000 types-aiobotocore-opensearchserverless-2.5.2.post2/types_aiobotocore_opensearchserverless.egg-info/requires.txt
--rw-r--r--   0 vlad      (1000) vlad      (1000)       39 2023-08-04 13:59:20.000000 types-aiobotocore-opensearchserverless-2.5.2.post2/types_aiobotocore_opensearchserverless.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:24:10.966744 types-aiobotocore-opensearchserverless-2.5.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-08 01:16:11.000000 types-aiobotocore-opensearchserverless-2.5.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    12946 2023-08-08 01:24:10.966744 types-aiobotocore-opensearchserverless-2.5.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    11375 2023-08-08 01:16:11.000000 types-aiobotocore-opensearchserverless-2.5.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-08 01:24:10.966744 types-aiobotocore-opensearchserverless-2.5.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2156 2023-08-08 01:16:11.000000 types-aiobotocore-opensearchserverless-2.5.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:24:10.962744 types-aiobotocore-opensearchserverless-2.5.4/types_aiobotocore_opensearchserverless/
+-rw-r--r--   0 runner    (1001) docker     (123)      581 2023-08-08 01:16:11.000000 types-aiobotocore-opensearchserverless-2.5.4/types_aiobotocore_opensearchserverless/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      580 2023-08-08 01:16:11.000000 types-aiobotocore-opensearchserverless-2.5.4/types_aiobotocore_opensearchserverless/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      997 2023-08-08 01:16:11.000000 types-aiobotocore-opensearchserverless-2.5.4/types_aiobotocore_opensearchserverless/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25784 2023-08-08 01:16:12.000000 types-aiobotocore-opensearchserverless-2.5.4/types_aiobotocore_opensearchserverless/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25744 2023-08-08 01:16:12.000000 types-aiobotocore-opensearchserverless-2.5.4/types_aiobotocore_opensearchserverless/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8432 2023-08-08 01:16:12.000000 types-aiobotocore-opensearchserverless-2.5.4/types_aiobotocore_opensearchserverless/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8430 2023-08-08 01:16:12.000000 types-aiobotocore-opensearchserverless-2.5.4/types_aiobotocore_opensearchserverless/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 01:16:11.000000 types-aiobotocore-opensearchserverless-2.5.4/types_aiobotocore_opensearchserverless/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    29369 2023-08-08 01:16:12.000000 types-aiobotocore-opensearchserverless-2.5.4/types_aiobotocore_opensearchserverless/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29330 2023-08-08 01:16:12.000000 types-aiobotocore-opensearchserverless-2.5.4/types_aiobotocore_opensearchserverless/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-08-08 01:16:11.000000 types-aiobotocore-opensearchserverless-2.5.4/types_aiobotocore_opensearchserverless/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:24:10.966744 types-aiobotocore-opensearchserverless-2.5.4/types_aiobotocore_opensearchserverless.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    12946 2023-08-08 01:24:10.000000 types-aiobotocore-opensearchserverless-2.5.4/types_aiobotocore_opensearchserverless.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      955 2023-08-08 01:24:10.000000 types-aiobotocore-opensearchserverless-2.5.4/types_aiobotocore_opensearchserverless.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 01:24:10.000000 types-aiobotocore-opensearchserverless-2.5.4/types_aiobotocore_opensearchserverless.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 01:24:10.000000 types-aiobotocore-opensearchserverless-2.5.4/types_aiobotocore_opensearchserverless.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-08 01:24:10.000000 types-aiobotocore-opensearchserverless-2.5.4/types_aiobotocore_opensearchserverless.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-08-08 01:24:10.000000 types-aiobotocore-opensearchserverless-2.5.4/types_aiobotocore_opensearchserverless.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-opensearchserverless-2.5.2.post2/LICENSE` & `types-aiobotocore-opensearchserverless-2.5.4/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-opensearchserverless-2.5.2.post2/PKG-INFO` & `types-aiobotocore-opensearchserverless-2.5.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-opensearchserverless
-Version: 2.5.2.post2
-Summary: Type annotations for aiobotocore.OpenSearchServiceServerless 2.5.2 service generated with mypy-boto3-builder 7.17.2
+Version: 2.5.4
+Summary: Type annotations for aiobotocore.OpenSearchServiceServerless 2.5.4 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_opensearchserverless/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-opensearchserverless.svg?color=blue)](https://pypi.org/project/types-aiobotocore-opensearchserverless)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_opensearchserverless/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-opensearchserverless)](https://pepy.tech/project/types-aiobotocore-opensearchserverless)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.OpenSearchServiceServerless 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opensearchserverless.html#OpenSearchServiceServerless)
+[aiobotocore.OpenSearchServiceServerless 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opensearchserverless.html#OpenSearchServiceServerless)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-opensearchserverless-2.5.2.post2/README.md` & `types-aiobotocore-opensearchserverless-2.5.4/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-opensearchserverless.svg?color=blue)](https://pypi.org/project/types-aiobotocore-opensearchserverless)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_opensearchserverless/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-opensearchserverless)](https://pepy.tech/project/types-aiobotocore-opensearchserverless)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.OpenSearchServiceServerless 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opensearchserverless.html#OpenSearchServiceServerless)
+[aiobotocore.OpenSearchServiceServerless 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opensearchserverless.html#OpenSearchServiceServerless)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-opensearchserverless-2.5.2.post2/setup.py` & `types-aiobotocore-opensearchserverless-2.5.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-opensearchserverless",
-    version="2.5.2.post2",
+    version="2.5.4",
     packages=["types_aiobotocore_opensearchserverless"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.OpenSearchServiceServerless 2.5.2 service generated with"
+        "Type annotations for aiobotocore.OpenSearchServiceServerless 2.5.4 service generated with"
         " mypy-boto3-builder 7.17.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
```

### Comparing `types-aiobotocore-opensearchserverless-2.5.2.post2/types_aiobotocore_opensearchserverless/__init__.py` & `types-aiobotocore-opensearchserverless-2.5.4/types_aiobotocore_opensearchserverless/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-opensearchserverless-2.5.2.post2/types_aiobotocore_opensearchserverless/__init__.pyi` & `types-aiobotocore-opensearchserverless-2.5.4/types_aiobotocore_opensearchserverless/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-opensearchserverless-2.5.2.post2/types_aiobotocore_opensearchserverless/__main__.py` & `types-aiobotocore-opensearchserverless-2.5.4/types_aiobotocore_opensearchserverless/__main__.py`

 * *Files 10% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.OpenSearchServiceServerless 2.5.2\nVersion:        "
-        " 2.5.2.post2\nBuilder version: 7.17.2\nDocs:           "
+        "Type annotations for aiobotocore.OpenSearchServiceServerless 2.5.4\nVersion:        "
+        " 2.5.4\nBuilder version: 7.17.2\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_opensearchserverless//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opensearchserverless.html#OpenSearchServiceServerless\nOther"
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

### Comparing `types-aiobotocore-opensearchserverless-2.5.2.post2/types_aiobotocore_opensearchserverless/client.py` & `types-aiobotocore-opensearchserverless-2.5.4/types_aiobotocore_opensearchserverless/client.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-opensearchserverless-2.5.2.post2/types_aiobotocore_opensearchserverless/client.pyi` & `types-aiobotocore-opensearchserverless-2.5.4/types_aiobotocore_opensearchserverless/client.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-opensearchserverless-2.5.2.post2/types_aiobotocore_opensearchserverless/literals.py` & `types-aiobotocore-opensearchserverless-2.5.4/types_aiobotocore_opensearchserverless/literals.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-opensearchserverless-2.5.2.post2/types_aiobotocore_opensearchserverless/literals.pyi` & `types-aiobotocore-opensearchserverless-2.5.4/types_aiobotocore_opensearchserverless/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-opensearchserverless-2.5.2.post2/types_aiobotocore_opensearchserverless/type_defs.py` & `types-aiobotocore-opensearchserverless-2.5.4/types_aiobotocore_opensearchserverless/type_defs.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-opensearchserverless-2.5.2.post2/types_aiobotocore_opensearchserverless/type_defs.pyi` & `types-aiobotocore-opensearchserverless-2.5.4/types_aiobotocore_opensearchserverless/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-opensearchserverless-2.5.2.post2/types_aiobotocore_opensearchserverless.egg-info/PKG-INFO` & `types-aiobotocore-opensearchserverless-2.5.4/types_aiobotocore_opensearchserverless.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-opensearchserverless
-Version: 2.5.2.post2
-Summary: Type annotations for aiobotocore.OpenSearchServiceServerless 2.5.2 service generated with mypy-boto3-builder 7.17.2
+Version: 2.5.4
+Summary: Type annotations for aiobotocore.OpenSearchServiceServerless 2.5.4 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_opensearchserverless/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-opensearchserverless.svg?color=blue)](https://pypi.org/project/types-aiobotocore-opensearchserverless)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_opensearchserverless/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-opensearchserverless)](https://pepy.tech/project/types-aiobotocore-opensearchserverless)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.OpenSearchServiceServerless 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opensearchserverless.html#OpenSearchServiceServerless)
+[aiobotocore.OpenSearchServiceServerless 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opensearchserverless.html#OpenSearchServiceServerless)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-opensearchserverless-2.5.2.post2/types_aiobotocore_opensearchserverless.egg-info/SOURCES.txt` & `types-aiobotocore-opensearchserverless-2.5.4/types_aiobotocore_opensearchserverless.egg-info/SOURCES.txt`

 * *Files identical despite different names*


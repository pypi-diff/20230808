# Comparing `tmp/types-aiobotocore-managedblockchain-2.5.2.post2.tar.gz` & `tmp/types-aiobotocore-managedblockchain-2.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-managedblockchain-2.5.2.post2.tar", last modified: Fri Aug  4 13:59:16 2023, max compression
+gzip compressed data, was "types-aiobotocore-managedblockchain-2.5.4.tar", last modified: Tue Aug  8 01:24:03 2023, max compression
```

## Comparing `types-aiobotocore-managedblockchain-2.5.2.post2.tar` & `types-aiobotocore-managedblockchain-2.5.4.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:16.706643 types-aiobotocore-managedblockchain-2.5.2.post2/
--rw-r--r--   0 vlad      (1000) vlad      (1000)     1070 2023-08-04 13:43:48.000000 types-aiobotocore-managedblockchain-2.5.2.post2/LICENSE
--rw-r--r--   0 vlad      (1000) vlad      (1000)    13487 2023-08-04 13:59:16.706643 types-aiobotocore-managedblockchain-2.5.2.post2/PKG-INFO
--rw-r--r--   0 vlad      (1000) vlad      (1000)    11929 2023-08-04 13:43:48.000000 types-aiobotocore-managedblockchain-2.5.2.post2/README.md
--rw-r--r--   0 vlad      (1000) vlad      (1000)       38 2023-08-04 13:59:16.706643 types-aiobotocore-managedblockchain-2.5.2.post2/setup.cfg
--rw-r--r--   0 vlad      (1000) vlad      (1000)     2142 2023-08-04 13:43:48.000000 types-aiobotocore-managedblockchain-2.5.2.post2/setup.py
-drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:16.706643 types-aiobotocore-managedblockchain-2.5.2.post2/types_aiobotocore_managedblockchain/
--rw-r--r--   0 vlad      (1000) vlad      (1000)      721 2023-08-04 13:43:48.000000 types-aiobotocore-managedblockchain-2.5.2.post2/types_aiobotocore_managedblockchain/__init__.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)      720 2023-08-04 13:43:48.000000 types-aiobotocore-managedblockchain-2.5.2.post2/types_aiobotocore_managedblockchain/__init__.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)      983 2023-08-04 13:43:48.000000 types-aiobotocore-managedblockchain-2.5.2.post2/types_aiobotocore_managedblockchain/__main__.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)    22333 2023-08-04 13:43:48.000000 types-aiobotocore-managedblockchain-2.5.2.post2/types_aiobotocore_managedblockchain/client.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)    22296 2023-08-04 13:43:48.000000 types-aiobotocore-managedblockchain-2.5.2.post2/types_aiobotocore_managedblockchain/client.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)     9280 2023-08-04 13:43:49.000000 types-aiobotocore-managedblockchain-2.5.2.post2/types_aiobotocore_managedblockchain/literals.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)     9278 2023-08-04 13:43:48.000000 types-aiobotocore-managedblockchain-2.5.2.post2/types_aiobotocore_managedblockchain/literals.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)     2093 2023-08-04 13:43:48.000000 types-aiobotocore-managedblockchain-2.5.2.post2/types_aiobotocore_managedblockchain/paginator.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)     2090 2023-08-04 13:43:48.000000 types-aiobotocore-managedblockchain-2.5.2.post2/types_aiobotocore_managedblockchain/paginator.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:43:48.000000 types-aiobotocore-managedblockchain-2.5.2.post2/types_aiobotocore_managedblockchain/py.typed
--rw-r--r--   0 vlad      (1000) vlad      (1000)    26442 2023-08-04 13:43:49.000000 types-aiobotocore-managedblockchain-2.5.2.post2/types_aiobotocore_managedblockchain/type_defs.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)    26413 2023-08-04 13:43:49.000000 types-aiobotocore-managedblockchain-2.5.2.post2/types_aiobotocore_managedblockchain/type_defs.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)       65 2023-08-04 13:43:48.000000 types-aiobotocore-managedblockchain-2.5.2.post2/types_aiobotocore_managedblockchain/version.py
-drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:16.706643 types-aiobotocore-managedblockchain-2.5.2.post2/types_aiobotocore_managedblockchain.egg-info/
--rw-r--r--   0 vlad      (1000) vlad      (1000)    13487 2023-08-04 13:59:16.000000 types-aiobotocore-managedblockchain-2.5.2.post2/types_aiobotocore_managedblockchain.egg-info/PKG-INFO
--rw-r--r--   0 vlad      (1000) vlad      (1000)     1003 2023-08-04 13:59:16.000000 types-aiobotocore-managedblockchain-2.5.2.post2/types_aiobotocore_managedblockchain.egg-info/SOURCES.txt
--rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:16.000000 types-aiobotocore-managedblockchain-2.5.2.post2/types_aiobotocore_managedblockchain.egg-info/dependency_links.txt
--rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:16.000000 types-aiobotocore-managedblockchain-2.5.2.post2/types_aiobotocore_managedblockchain.egg-info/not-zip-safe
--rw-r--r--   0 vlad      (1000) vlad      (1000)       52 2023-08-04 13:59:16.000000 types-aiobotocore-managedblockchain-2.5.2.post2/types_aiobotocore_managedblockchain.egg-info/requires.txt
--rw-r--r--   0 vlad      (1000) vlad      (1000)       36 2023-08-04 13:59:16.000000 types-aiobotocore-managedblockchain-2.5.2.post2/types_aiobotocore_managedblockchain.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:24:03.422728 types-aiobotocore-managedblockchain-2.5.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-08 01:14:44.000000 types-aiobotocore-managedblockchain-2.5.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    13481 2023-08-08 01:24:03.422728 types-aiobotocore-managedblockchain-2.5.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    11929 2023-08-08 01:14:44.000000 types-aiobotocore-managedblockchain-2.5.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-08 01:24:03.422728 types-aiobotocore-managedblockchain-2.5.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2136 2023-08-08 01:14:44.000000 types-aiobotocore-managedblockchain-2.5.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:24:03.418728 types-aiobotocore-managedblockchain-2.5.4/types_aiobotocore_managedblockchain/
+-rw-r--r--   0 runner    (1001) docker     (123)      721 2023-08-08 01:14:44.000000 types-aiobotocore-managedblockchain-2.5.4/types_aiobotocore_managedblockchain/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      720 2023-08-08 01:14:44.000000 types-aiobotocore-managedblockchain-2.5.4/types_aiobotocore_managedblockchain/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      971 2023-08-08 01:14:44.000000 types-aiobotocore-managedblockchain-2.5.4/types_aiobotocore_managedblockchain/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22333 2023-08-08 01:14:44.000000 types-aiobotocore-managedblockchain-2.5.4/types_aiobotocore_managedblockchain/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22296 2023-08-08 01:14:44.000000 types-aiobotocore-managedblockchain-2.5.4/types_aiobotocore_managedblockchain/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9280 2023-08-08 01:14:45.000000 types-aiobotocore-managedblockchain-2.5.4/types_aiobotocore_managedblockchain/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9278 2023-08-08 01:14:44.000000 types-aiobotocore-managedblockchain-2.5.4/types_aiobotocore_managedblockchain/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2093 2023-08-08 01:14:44.000000 types-aiobotocore-managedblockchain-2.5.4/types_aiobotocore_managedblockchain/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2090 2023-08-08 01:14:44.000000 types-aiobotocore-managedblockchain-2.5.4/types_aiobotocore_managedblockchain/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 01:14:44.000000 types-aiobotocore-managedblockchain-2.5.4/types_aiobotocore_managedblockchain/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    26442 2023-08-08 01:14:47.000000 types-aiobotocore-managedblockchain-2.5.4/types_aiobotocore_managedblockchain/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26413 2023-08-08 01:14:47.000000 types-aiobotocore-managedblockchain-2.5.4/types_aiobotocore_managedblockchain/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-08-08 01:14:44.000000 types-aiobotocore-managedblockchain-2.5.4/types_aiobotocore_managedblockchain/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:24:03.422728 types-aiobotocore-managedblockchain-2.5.4/types_aiobotocore_managedblockchain.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    13481 2023-08-08 01:24:03.000000 types-aiobotocore-managedblockchain-2.5.4/types_aiobotocore_managedblockchain.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1003 2023-08-08 01:24:03.000000 types-aiobotocore-managedblockchain-2.5.4/types_aiobotocore_managedblockchain.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 01:24:03.000000 types-aiobotocore-managedblockchain-2.5.4/types_aiobotocore_managedblockchain.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 01:24:03.000000 types-aiobotocore-managedblockchain-2.5.4/types_aiobotocore_managedblockchain.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-08 01:24:03.000000 types-aiobotocore-managedblockchain-2.5.4/types_aiobotocore_managedblockchain.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-08-08 01:24:03.000000 types-aiobotocore-managedblockchain-2.5.4/types_aiobotocore_managedblockchain.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-managedblockchain-2.5.2.post2/LICENSE` & `types-aiobotocore-managedblockchain-2.5.4/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-managedblockchain-2.5.2.post2/PKG-INFO` & `types-aiobotocore-managedblockchain-2.5.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-managedblockchain
-Version: 2.5.2.post2
-Summary: Type annotations for aiobotocore.ManagedBlockchain 2.5.2 service generated with mypy-boto3-builder 7.17.2
+Version: 2.5.4
+Summary: Type annotations for aiobotocore.ManagedBlockchain 2.5.4 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_managedblockchain/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-managedblockchain.svg?color=blue)](https://pypi.org/project/types-aiobotocore-managedblockchain)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_managedblockchain/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-managedblockchain)](https://pepy.tech/project/types-aiobotocore-managedblockchain)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.ManagedBlockchain 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/managedblockchain.html#ManagedBlockchain)
+[aiobotocore.ManagedBlockchain 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/managedblockchain.html#ManagedBlockchain)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-managedblockchain-2.5.2.post2/README.md` & `types-aiobotocore-managedblockchain-2.5.4/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-managedblockchain.svg?color=blue)](https://pypi.org/project/types-aiobotocore-managedblockchain)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_managedblockchain/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-managedblockchain)](https://pepy.tech/project/types-aiobotocore-managedblockchain)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.ManagedBlockchain 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/managedblockchain.html#ManagedBlockchain)
+[aiobotocore.ManagedBlockchain 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/managedblockchain.html#ManagedBlockchain)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-managedblockchain-2.5.2.post2/setup.py` & `types-aiobotocore-managedblockchain-2.5.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-managedblockchain",
-    version="2.5.2.post2",
+    version="2.5.4",
     packages=["types_aiobotocore_managedblockchain"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.ManagedBlockchain 2.5.2 service generated with"
+        "Type annotations for aiobotocore.ManagedBlockchain 2.5.4 service generated with"
         " mypy-boto3-builder 7.17.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
```

### Comparing `types-aiobotocore-managedblockchain-2.5.2.post2/types_aiobotocore_managedblockchain/__init__.py` & `types-aiobotocore-managedblockchain-2.5.4/types_aiobotocore_managedblockchain/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-managedblockchain-2.5.2.post2/types_aiobotocore_managedblockchain/__init__.pyi` & `types-aiobotocore-managedblockchain-2.5.4/types_aiobotocore_managedblockchain/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-managedblockchain-2.5.2.post2/types_aiobotocore_managedblockchain/__main__.py` & `types-aiobotocore-managedblockchain-2.5.4/types_aiobotocore_managedblockchain/__main__.py`

 * *Files 9% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.ManagedBlockchain 2.5.2\nVersion:        "
-        " 2.5.2.post2\nBuilder version: 7.17.2\nDocs:           "
+        "Type annotations for aiobotocore.ManagedBlockchain 2.5.4\nVersion:         2.5.4\nBuilder"
+        " version: 7.17.2\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_managedblockchain//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/managedblockchain.html#ManagedBlockchain\nOther"
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

### Comparing `types-aiobotocore-managedblockchain-2.5.2.post2/types_aiobotocore_managedblockchain/client.py` & `types-aiobotocore-managedblockchain-2.5.4/types_aiobotocore_managedblockchain/client.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-managedblockchain-2.5.2.post2/types_aiobotocore_managedblockchain/client.pyi` & `types-aiobotocore-managedblockchain-2.5.4/types_aiobotocore_managedblockchain/client.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-managedblockchain-2.5.2.post2/types_aiobotocore_managedblockchain/literals.py` & `types-aiobotocore-managedblockchain-2.5.4/types_aiobotocore_managedblockchain/literals.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-managedblockchain-2.5.2.post2/types_aiobotocore_managedblockchain/literals.pyi` & `types-aiobotocore-managedblockchain-2.5.4/types_aiobotocore_managedblockchain/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-managedblockchain-2.5.2.post2/types_aiobotocore_managedblockchain/paginator.py` & `types-aiobotocore-managedblockchain-2.5.4/types_aiobotocore_managedblockchain/paginator.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-managedblockchain-2.5.2.post2/types_aiobotocore_managedblockchain/paginator.pyi` & `types-aiobotocore-managedblockchain-2.5.4/types_aiobotocore_managedblockchain/paginator.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-managedblockchain-2.5.2.post2/types_aiobotocore_managedblockchain/type_defs.py` & `types-aiobotocore-managedblockchain-2.5.4/types_aiobotocore_managedblockchain/type_defs.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-managedblockchain-2.5.2.post2/types_aiobotocore_managedblockchain/type_defs.pyi` & `types-aiobotocore-managedblockchain-2.5.4/types_aiobotocore_managedblockchain/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-managedblockchain-2.5.2.post2/types_aiobotocore_managedblockchain.egg-info/PKG-INFO` & `types-aiobotocore-managedblockchain-2.5.4/types_aiobotocore_managedblockchain.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-managedblockchain
-Version: 2.5.2.post2
-Summary: Type annotations for aiobotocore.ManagedBlockchain 2.5.2 service generated with mypy-boto3-builder 7.17.2
+Version: 2.5.4
+Summary: Type annotations for aiobotocore.ManagedBlockchain 2.5.4 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_managedblockchain/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-managedblockchain.svg?color=blue)](https://pypi.org/project/types-aiobotocore-managedblockchain)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_managedblockchain/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-managedblockchain)](https://pepy.tech/project/types-aiobotocore-managedblockchain)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.ManagedBlockchain 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/managedblockchain.html#ManagedBlockchain)
+[aiobotocore.ManagedBlockchain 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/managedblockchain.html#ManagedBlockchain)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-managedblockchain-2.5.2.post2/types_aiobotocore_managedblockchain.egg-info/SOURCES.txt` & `types-aiobotocore-managedblockchain-2.5.4/types_aiobotocore_managedblockchain.egg-info/SOURCES.txt`

 * *Files identical despite different names*


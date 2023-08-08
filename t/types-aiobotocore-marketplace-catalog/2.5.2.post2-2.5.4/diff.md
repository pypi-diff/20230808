# Comparing `tmp/types-aiobotocore-marketplace-catalog-2.5.2.post2.tar.gz` & `tmp/types-aiobotocore-marketplace-catalog-2.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-marketplace-catalog-2.5.2.post2.tar", last modified: Fri Aug  4 13:59:17 2023, max compression
+gzip compressed data, was "types-aiobotocore-marketplace-catalog-2.5.4.tar", last modified: Tue Aug  8 01:24:04 2023, max compression
```

## Comparing `types-aiobotocore-marketplace-catalog-2.5.2.post2.tar` & `types-aiobotocore-marketplace-catalog-2.5.4.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:17.156643 types-aiobotocore-marketplace-catalog-2.5.2.post2/
--rw-r--r--   0 vlad      (1000) vlad      (1000)     1070 2023-08-04 13:43:52.000000 types-aiobotocore-marketplace-catalog-2.5.2.post2/LICENSE
--rw-r--r--   0 vlad      (1000) vlad      (1000)    13751 2023-08-04 13:59:17.156643 types-aiobotocore-marketplace-catalog-2.5.2.post2/PKG-INFO
--rw-r--r--   0 vlad      (1000) vlad      (1000)    12186 2023-08-04 13:43:52.000000 types-aiobotocore-marketplace-catalog-2.5.2.post2/README.md
--rw-r--r--   0 vlad      (1000) vlad      (1000)       38 2023-08-04 13:59:17.156643 types-aiobotocore-marketplace-catalog-2.5.2.post2/setup.cfg
--rw-r--r--   0 vlad      (1000) vlad      (1000)     2131 2023-08-04 13:43:52.000000 types-aiobotocore-marketplace-catalog-2.5.2.post2/setup.py
-drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:17.156643 types-aiobotocore-marketplace-catalog-2.5.2.post2/types_aiobotocore_marketplace_catalog/
--rw-r--r--   0 vlad      (1000) vlad      (1000)      910 2023-08-04 13:43:52.000000 types-aiobotocore-marketplace-catalog-2.5.2.post2/types_aiobotocore_marketplace_catalog/__init__.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)      909 2023-08-04 13:43:52.000000 types-aiobotocore-marketplace-catalog-2.5.2.post2/types_aiobotocore_marketplace_catalog/__init__.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)      989 2023-08-04 13:43:52.000000 types-aiobotocore-marketplace-catalog-2.5.2.post2/types_aiobotocore_marketplace_catalog/__main__.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)    13997 2023-08-04 13:43:52.000000 types-aiobotocore-marketplace-catalog-2.5.2.post2/types_aiobotocore_marketplace_catalog/client.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)    13974 2023-08-04 13:43:52.000000 types-aiobotocore-marketplace-catalog-2.5.2.post2/types_aiobotocore_marketplace_catalog/client.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)     8331 2023-08-04 13:43:52.000000 types-aiobotocore-marketplace-catalog-2.5.2.post2/types_aiobotocore_marketplace_catalog/literals.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)     8329 2023-08-04 13:43:52.000000 types-aiobotocore-marketplace-catalog-2.5.2.post2/types_aiobotocore_marketplace_catalog/literals.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)     3648 2023-08-04 13:43:52.000000 types-aiobotocore-marketplace-catalog-2.5.2.post2/types_aiobotocore_marketplace_catalog/paginator.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)     3644 2023-08-04 13:43:52.000000 types-aiobotocore-marketplace-catalog-2.5.2.post2/types_aiobotocore_marketplace_catalog/paginator.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:43:52.000000 types-aiobotocore-marketplace-catalog-2.5.2.post2/types_aiobotocore_marketplace_catalog/py.typed
--rw-r--r--   0 vlad      (1000) vlad      (1000)    11091 2023-08-04 13:43:53.000000 types-aiobotocore-marketplace-catalog-2.5.2.post2/types_aiobotocore_marketplace_catalog/type_defs.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)    11077 2023-08-04 13:43:52.000000 types-aiobotocore-marketplace-catalog-2.5.2.post2/types_aiobotocore_marketplace_catalog/type_defs.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)       65 2023-08-04 13:43:52.000000 types-aiobotocore-marketplace-catalog-2.5.2.post2/types_aiobotocore_marketplace_catalog/version.py
-drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:17.156643 types-aiobotocore-marketplace-catalog-2.5.2.post2/types_aiobotocore_marketplace_catalog.egg-info/
--rw-r--r--   0 vlad      (1000) vlad      (1000)    13751 2023-08-04 13:59:17.000000 types-aiobotocore-marketplace-catalog-2.5.2.post2/types_aiobotocore_marketplace_catalog.egg-info/PKG-INFO
--rw-r--r--   0 vlad      (1000) vlad      (1000)     1041 2023-08-04 13:59:17.000000 types-aiobotocore-marketplace-catalog-2.5.2.post2/types_aiobotocore_marketplace_catalog.egg-info/SOURCES.txt
--rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:17.000000 types-aiobotocore-marketplace-catalog-2.5.2.post2/types_aiobotocore_marketplace_catalog.egg-info/dependency_links.txt
--rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:17.000000 types-aiobotocore-marketplace-catalog-2.5.2.post2/types_aiobotocore_marketplace_catalog.egg-info/not-zip-safe
--rw-r--r--   0 vlad      (1000) vlad      (1000)       52 2023-08-04 13:59:17.000000 types-aiobotocore-marketplace-catalog-2.5.2.post2/types_aiobotocore_marketplace_catalog.egg-info/requires.txt
--rw-r--r--   0 vlad      (1000) vlad      (1000)       38 2023-08-04 13:59:17.000000 types-aiobotocore-marketplace-catalog-2.5.2.post2/types_aiobotocore_marketplace_catalog.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:24:04.182729 types-aiobotocore-marketplace-catalog-2.5.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-08 01:14:48.000000 types-aiobotocore-marketplace-catalog-2.5.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    13745 2023-08-08 01:24:04.182729 types-aiobotocore-marketplace-catalog-2.5.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    12186 2023-08-08 01:14:48.000000 types-aiobotocore-marketplace-catalog-2.5.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-08 01:24:04.182729 types-aiobotocore-marketplace-catalog-2.5.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2125 2023-08-08 01:14:48.000000 types-aiobotocore-marketplace-catalog-2.5.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:24:04.182729 types-aiobotocore-marketplace-catalog-2.5.4/types_aiobotocore_marketplace_catalog/
+-rw-r--r--   0 runner    (1001) docker     (123)      910 2023-08-08 01:14:48.000000 types-aiobotocore-marketplace-catalog-2.5.4/types_aiobotocore_marketplace_catalog/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      909 2023-08-08 01:14:48.000000 types-aiobotocore-marketplace-catalog-2.5.4/types_aiobotocore_marketplace_catalog/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      977 2023-08-08 01:14:48.000000 types-aiobotocore-marketplace-catalog-2.5.4/types_aiobotocore_marketplace_catalog/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13997 2023-08-08 01:14:48.000000 types-aiobotocore-marketplace-catalog-2.5.4/types_aiobotocore_marketplace_catalog/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13974 2023-08-08 01:14:48.000000 types-aiobotocore-marketplace-catalog-2.5.4/types_aiobotocore_marketplace_catalog/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8331 2023-08-08 01:14:48.000000 types-aiobotocore-marketplace-catalog-2.5.4/types_aiobotocore_marketplace_catalog/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8329 2023-08-08 01:14:48.000000 types-aiobotocore-marketplace-catalog-2.5.4/types_aiobotocore_marketplace_catalog/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     3648 2023-08-08 01:14:48.000000 types-aiobotocore-marketplace-catalog-2.5.4/types_aiobotocore_marketplace_catalog/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3644 2023-08-08 01:14:48.000000 types-aiobotocore-marketplace-catalog-2.5.4/types_aiobotocore_marketplace_catalog/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 01:14:48.000000 types-aiobotocore-marketplace-catalog-2.5.4/types_aiobotocore_marketplace_catalog/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    11091 2023-08-08 01:14:48.000000 types-aiobotocore-marketplace-catalog-2.5.4/types_aiobotocore_marketplace_catalog/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11077 2023-08-08 01:14:48.000000 types-aiobotocore-marketplace-catalog-2.5.4/types_aiobotocore_marketplace_catalog/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-08-08 01:14:48.000000 types-aiobotocore-marketplace-catalog-2.5.4/types_aiobotocore_marketplace_catalog/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:24:04.182729 types-aiobotocore-marketplace-catalog-2.5.4/types_aiobotocore_marketplace_catalog.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    13745 2023-08-08 01:24:04.000000 types-aiobotocore-marketplace-catalog-2.5.4/types_aiobotocore_marketplace_catalog.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1041 2023-08-08 01:24:04.000000 types-aiobotocore-marketplace-catalog-2.5.4/types_aiobotocore_marketplace_catalog.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 01:24:04.000000 types-aiobotocore-marketplace-catalog-2.5.4/types_aiobotocore_marketplace_catalog.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 01:24:04.000000 types-aiobotocore-marketplace-catalog-2.5.4/types_aiobotocore_marketplace_catalog.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-08 01:24:04.000000 types-aiobotocore-marketplace-catalog-2.5.4/types_aiobotocore_marketplace_catalog.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-08 01:24:04.000000 types-aiobotocore-marketplace-catalog-2.5.4/types_aiobotocore_marketplace_catalog.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-marketplace-catalog-2.5.2.post2/LICENSE` & `types-aiobotocore-marketplace-catalog-2.5.4/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-marketplace-catalog-2.5.2.post2/PKG-INFO` & `types-aiobotocore-marketplace-catalog-2.5.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-marketplace-catalog
-Version: 2.5.2.post2
-Summary: Type annotations for aiobotocore.MarketplaceCatalog 2.5.2 service generated with mypy-boto3-builder 7.17.2
+Version: 2.5.4
+Summary: Type annotations for aiobotocore.MarketplaceCatalog 2.5.4 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_marketplace_catalog/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-marketplace-catalog.svg?color=blue)](https://pypi.org/project/types-aiobotocore-marketplace-catalog)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_marketplace_catalog/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-marketplace-catalog)](https://pepy.tech/project/types-aiobotocore-marketplace-catalog)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.MarketplaceCatalog 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/marketplace-catalog.html#MarketplaceCatalog)
+[aiobotocore.MarketplaceCatalog 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/marketplace-catalog.html#MarketplaceCatalog)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-marketplace-catalog-2.5.2.post2/README.md` & `types-aiobotocore-marketplace-catalog-2.5.4/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-marketplace-catalog.svg?color=blue)](https://pypi.org/project/types-aiobotocore-marketplace-catalog)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_marketplace_catalog/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-marketplace-catalog)](https://pepy.tech/project/types-aiobotocore-marketplace-catalog)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.MarketplaceCatalog 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/marketplace-catalog.html#MarketplaceCatalog)
+[aiobotocore.MarketplaceCatalog 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/marketplace-catalog.html#MarketplaceCatalog)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-marketplace-catalog-2.5.2.post2/setup.py` & `types-aiobotocore-marketplace-catalog-2.5.4/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-marketplace-catalog",
-    version="2.5.2.post2",
+    version="2.5.4",
     packages=["types_aiobotocore_marketplace_catalog"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.MarketplaceCatalog 2.5.2 service generated with"
+        "Type annotations for aiobotocore.MarketplaceCatalog 2.5.4 service generated with"
         " mypy-boto3-builder 7.17.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
```

### Comparing `types-aiobotocore-marketplace-catalog-2.5.2.post2/types_aiobotocore_marketplace_catalog/__init__.py` & `types-aiobotocore-marketplace-catalog-2.5.4/types_aiobotocore_marketplace_catalog/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-marketplace-catalog-2.5.2.post2/types_aiobotocore_marketplace_catalog/__init__.pyi` & `types-aiobotocore-marketplace-catalog-2.5.4/types_aiobotocore_marketplace_catalog/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-marketplace-catalog-2.5.2.post2/types_aiobotocore_marketplace_catalog/__main__.py` & `types-aiobotocore-marketplace-catalog-2.5.4/types_aiobotocore_marketplace_catalog/__main__.py`

 * *Files 10% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.MarketplaceCatalog 2.5.2\nVersion:        "
-        " 2.5.2.post2\nBuilder version: 7.17.2\nDocs:           "
+        "Type annotations for aiobotocore.MarketplaceCatalog 2.5.4\nVersion:         2.5.4\nBuilder"
+        " version: 7.17.2\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_marketplace_catalog//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/marketplace-catalog.html#MarketplaceCatalog\nOther"
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

### Comparing `types-aiobotocore-marketplace-catalog-2.5.2.post2/types_aiobotocore_marketplace_catalog/client.py` & `types-aiobotocore-marketplace-catalog-2.5.4/types_aiobotocore_marketplace_catalog/client.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-marketplace-catalog-2.5.2.post2/types_aiobotocore_marketplace_catalog/client.pyi` & `types-aiobotocore-marketplace-catalog-2.5.4/types_aiobotocore_marketplace_catalog/client.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-marketplace-catalog-2.5.2.post2/types_aiobotocore_marketplace_catalog/literals.py` & `types-aiobotocore-marketplace-catalog-2.5.4/types_aiobotocore_marketplace_catalog/literals.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-marketplace-catalog-2.5.2.post2/types_aiobotocore_marketplace_catalog/literals.pyi` & `types-aiobotocore-marketplace-catalog-2.5.4/types_aiobotocore_marketplace_catalog/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-marketplace-catalog-2.5.2.post2/types_aiobotocore_marketplace_catalog/paginator.py` & `types-aiobotocore-marketplace-catalog-2.5.4/types_aiobotocore_marketplace_catalog/paginator.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-marketplace-catalog-2.5.2.post2/types_aiobotocore_marketplace_catalog/paginator.pyi` & `types-aiobotocore-marketplace-catalog-2.5.4/types_aiobotocore_marketplace_catalog/paginator.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-marketplace-catalog-2.5.2.post2/types_aiobotocore_marketplace_catalog/type_defs.py` & `types-aiobotocore-marketplace-catalog-2.5.4/types_aiobotocore_marketplace_catalog/type_defs.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-marketplace-catalog-2.5.2.post2/types_aiobotocore_marketplace_catalog/type_defs.pyi` & `types-aiobotocore-marketplace-catalog-2.5.4/types_aiobotocore_marketplace_catalog/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-marketplace-catalog-2.5.2.post2/types_aiobotocore_marketplace_catalog.egg-info/PKG-INFO` & `types-aiobotocore-marketplace-catalog-2.5.4/types_aiobotocore_marketplace_catalog.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-marketplace-catalog
-Version: 2.5.2.post2
-Summary: Type annotations for aiobotocore.MarketplaceCatalog 2.5.2 service generated with mypy-boto3-builder 7.17.2
+Version: 2.5.4
+Summary: Type annotations for aiobotocore.MarketplaceCatalog 2.5.4 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_marketplace_catalog/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-marketplace-catalog.svg?color=blue)](https://pypi.org/project/types-aiobotocore-marketplace-catalog)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_marketplace_catalog/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-marketplace-catalog)](https://pepy.tech/project/types-aiobotocore-marketplace-catalog)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.MarketplaceCatalog 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/marketplace-catalog.html#MarketplaceCatalog)
+[aiobotocore.MarketplaceCatalog 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/marketplace-catalog.html#MarketplaceCatalog)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-marketplace-catalog-2.5.2.post2/types_aiobotocore_marketplace_catalog.egg-info/SOURCES.txt` & `types-aiobotocore-marketplace-catalog-2.5.4/types_aiobotocore_marketplace_catalog.egg-info/SOURCES.txt`

 * *Files identical despite different names*


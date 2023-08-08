# Comparing `tmp/types-aiobotocore-marketplace-entitlement-2.5.2.post2.tar.gz` & `tmp/types-aiobotocore-marketplace-entitlement-2.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-marketplace-entitlement-2.5.2.post2.tar", last modified: Fri Aug  4 13:59:17 2023, max compression
+gzip compressed data, was "types-aiobotocore-marketplace-entitlement-2.5.4.tar", last modified: Tue Aug  8 01:24:04 2023, max compression
```

## Comparing `types-aiobotocore-marketplace-entitlement-2.5.2.post2.tar` & `types-aiobotocore-marketplace-entitlement-2.5.4.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:17.256643 types-aiobotocore-marketplace-entitlement-2.5.2.post2/
--rw-r--r--   0 vlad      (1000) vlad      (1000)     1070 2023-08-04 13:43:54.000000 types-aiobotocore-marketplace-entitlement-2.5.2.post2/LICENSE
--rw-r--r--   0 vlad      (1000) vlad      (1000)    13937 2023-08-04 13:59:17.256643 types-aiobotocore-marketplace-entitlement-2.5.2.post2/PKG-INFO
--rw-r--r--   0 vlad      (1000) vlad      (1000)    12349 2023-08-04 13:43:54.000000 types-aiobotocore-marketplace-entitlement-2.5.2.post2/README.md
--rw-r--r--   0 vlad      (1000) vlad      (1000)       38 2023-08-04 13:59:17.256643 types-aiobotocore-marketplace-entitlement-2.5.2.post2/setup.cfg
--rw-r--r--   0 vlad      (1000) vlad      (1000)     2182 2023-08-04 13:43:53.000000 types-aiobotocore-marketplace-entitlement-2.5.2.post2/setup.py
-drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:17.256643 types-aiobotocore-marketplace-entitlement-2.5.2.post2/types_aiobotocore_marketplace_entitlement/
--rw-r--r--   0 vlad      (1000) vlad      (1000)      811 2023-08-04 13:43:54.000000 types-aiobotocore-marketplace-entitlement-2.5.2.post2/types_aiobotocore_marketplace_entitlement/__init__.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)      810 2023-08-04 13:43:54.000000 types-aiobotocore-marketplace-entitlement-2.5.2.post2/types_aiobotocore_marketplace_entitlement/__init__.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)     1019 2023-08-04 13:43:54.000000 types-aiobotocore-marketplace-entitlement-2.5.2.post2/types_aiobotocore_marketplace_entitlement/__main__.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)     6002 2023-08-04 13:43:54.000000 types-aiobotocore-marketplace-entitlement-2.5.2.post2/types_aiobotocore_marketplace_entitlement/client.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)     5991 2023-08-04 13:43:54.000000 types-aiobotocore-marketplace-entitlement-2.5.2.post2/types_aiobotocore_marketplace_entitlement/client.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)     8078 2023-08-04 13:43:55.000000 types-aiobotocore-marketplace-entitlement-2.5.2.post2/types_aiobotocore_marketplace_entitlement/literals.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)     8076 2023-08-04 13:43:54.000000 types-aiobotocore-marketplace-entitlement-2.5.2.post2/types_aiobotocore_marketplace_entitlement/literals.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)     2407 2023-08-04 13:43:54.000000 types-aiobotocore-marketplace-entitlement-2.5.2.post2/types_aiobotocore_marketplace_entitlement/paginator.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)     2404 2023-08-04 13:43:54.000000 types-aiobotocore-marketplace-entitlement-2.5.2.post2/types_aiobotocore_marketplace_entitlement/paginator.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:43:54.000000 types-aiobotocore-marketplace-entitlement-2.5.2.post2/types_aiobotocore_marketplace_entitlement/py.typed
--rw-r--r--   0 vlad      (1000) vlad      (1000)     3289 2023-08-04 13:43:55.000000 types-aiobotocore-marketplace-entitlement-2.5.2.post2/types_aiobotocore_marketplace_entitlement/type_defs.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)     3284 2023-08-04 13:43:55.000000 types-aiobotocore-marketplace-entitlement-2.5.2.post2/types_aiobotocore_marketplace_entitlement/type_defs.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)       65 2023-08-04 13:43:54.000000 types-aiobotocore-marketplace-entitlement-2.5.2.post2/types_aiobotocore_marketplace_entitlement/version.py
-drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:17.256643 types-aiobotocore-marketplace-entitlement-2.5.2.post2/types_aiobotocore_marketplace_entitlement.egg-info/
--rw-r--r--   0 vlad      (1000) vlad      (1000)    13937 2023-08-04 13:59:17.000000 types-aiobotocore-marketplace-entitlement-2.5.2.post2/types_aiobotocore_marketplace_entitlement.egg-info/PKG-INFO
--rw-r--r--   0 vlad      (1000) vlad      (1000)     1117 2023-08-04 13:59:17.000000 types-aiobotocore-marketplace-entitlement-2.5.2.post2/types_aiobotocore_marketplace_entitlement.egg-info/SOURCES.txt
--rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:17.000000 types-aiobotocore-marketplace-entitlement-2.5.2.post2/types_aiobotocore_marketplace_entitlement.egg-info/dependency_links.txt
--rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:17.000000 types-aiobotocore-marketplace-entitlement-2.5.2.post2/types_aiobotocore_marketplace_entitlement.egg-info/not-zip-safe
--rw-r--r--   0 vlad      (1000) vlad      (1000)       52 2023-08-04 13:59:17.000000 types-aiobotocore-marketplace-entitlement-2.5.2.post2/types_aiobotocore_marketplace_entitlement.egg-info/requires.txt
--rw-r--r--   0 vlad      (1000) vlad      (1000)       42 2023-08-04 13:59:17.000000 types-aiobotocore-marketplace-entitlement-2.5.2.post2/types_aiobotocore_marketplace_entitlement.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:24:04.250730 types-aiobotocore-marketplace-entitlement-2.5.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-08 01:14:49.000000 types-aiobotocore-marketplace-entitlement-2.5.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    13931 2023-08-08 01:24:04.250730 types-aiobotocore-marketplace-entitlement-2.5.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    12349 2023-08-08 01:14:49.000000 types-aiobotocore-marketplace-entitlement-2.5.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-08 01:24:04.250730 types-aiobotocore-marketplace-entitlement-2.5.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2176 2023-08-08 01:14:49.000000 types-aiobotocore-marketplace-entitlement-2.5.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:24:04.250730 types-aiobotocore-marketplace-entitlement-2.5.4/types_aiobotocore_marketplace_entitlement/
+-rw-r--r--   0 runner    (1001) docker     (123)      811 2023-08-08 01:14:49.000000 types-aiobotocore-marketplace-entitlement-2.5.4/types_aiobotocore_marketplace_entitlement/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      810 2023-08-08 01:14:49.000000 types-aiobotocore-marketplace-entitlement-2.5.4/types_aiobotocore_marketplace_entitlement/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1007 2023-08-08 01:14:49.000000 types-aiobotocore-marketplace-entitlement-2.5.4/types_aiobotocore_marketplace_entitlement/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6002 2023-08-08 01:14:49.000000 types-aiobotocore-marketplace-entitlement-2.5.4/types_aiobotocore_marketplace_entitlement/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5991 2023-08-08 01:14:49.000000 types-aiobotocore-marketplace-entitlement-2.5.4/types_aiobotocore_marketplace_entitlement/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8078 2023-08-08 01:14:49.000000 types-aiobotocore-marketplace-entitlement-2.5.4/types_aiobotocore_marketplace_entitlement/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8076 2023-08-08 01:14:49.000000 types-aiobotocore-marketplace-entitlement-2.5.4/types_aiobotocore_marketplace_entitlement/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2407 2023-08-08 01:14:49.000000 types-aiobotocore-marketplace-entitlement-2.5.4/types_aiobotocore_marketplace_entitlement/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2404 2023-08-08 01:14:49.000000 types-aiobotocore-marketplace-entitlement-2.5.4/types_aiobotocore_marketplace_entitlement/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 01:14:49.000000 types-aiobotocore-marketplace-entitlement-2.5.4/types_aiobotocore_marketplace_entitlement/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     3289 2023-08-08 01:14:49.000000 types-aiobotocore-marketplace-entitlement-2.5.4/types_aiobotocore_marketplace_entitlement/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3284 2023-08-08 01:14:49.000000 types-aiobotocore-marketplace-entitlement-2.5.4/types_aiobotocore_marketplace_entitlement/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-08-08 01:14:49.000000 types-aiobotocore-marketplace-entitlement-2.5.4/types_aiobotocore_marketplace_entitlement/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:24:04.250730 types-aiobotocore-marketplace-entitlement-2.5.4/types_aiobotocore_marketplace_entitlement.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    13931 2023-08-08 01:24:04.000000 types-aiobotocore-marketplace-entitlement-2.5.4/types_aiobotocore_marketplace_entitlement.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1117 2023-08-08 01:24:04.000000 types-aiobotocore-marketplace-entitlement-2.5.4/types_aiobotocore_marketplace_entitlement.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 01:24:04.000000 types-aiobotocore-marketplace-entitlement-2.5.4/types_aiobotocore_marketplace_entitlement.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 01:24:04.000000 types-aiobotocore-marketplace-entitlement-2.5.4/types_aiobotocore_marketplace_entitlement.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-08 01:24:04.000000 types-aiobotocore-marketplace-entitlement-2.5.4/types_aiobotocore_marketplace_entitlement.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-08-08 01:24:04.000000 types-aiobotocore-marketplace-entitlement-2.5.4/types_aiobotocore_marketplace_entitlement.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-marketplace-entitlement-2.5.2.post2/LICENSE` & `types-aiobotocore-marketplace-entitlement-2.5.4/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-marketplace-entitlement-2.5.2.post2/PKG-INFO` & `types-aiobotocore-marketplace-entitlement-2.5.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-marketplace-entitlement
-Version: 2.5.2.post2
-Summary: Type annotations for aiobotocore.MarketplaceEntitlementService 2.5.2 service generated with mypy-boto3-builder 7.17.2
+Version: 2.5.4
+Summary: Type annotations for aiobotocore.MarketplaceEntitlementService 2.5.4 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_marketplace_entitlement/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-marketplace-entitlement.svg?color=blue)](https://pypi.org/project/types-aiobotocore-marketplace-entitlement)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_marketplace_entitlement/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-marketplace-entitlement)](https://pepy.tech/project/types-aiobotocore-marketplace-entitlement)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.MarketplaceEntitlementService 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/marketplace-entitlement.html#MarketplaceEntitlementService)
+[aiobotocore.MarketplaceEntitlementService 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/marketplace-entitlement.html#MarketplaceEntitlementService)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-marketplace-entitlement-2.5.2.post2/README.md` & `types-aiobotocore-marketplace-entitlement-2.5.4/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-marketplace-entitlement.svg?color=blue)](https://pypi.org/project/types-aiobotocore-marketplace-entitlement)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_marketplace_entitlement/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-marketplace-entitlement)](https://pepy.tech/project/types-aiobotocore-marketplace-entitlement)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.MarketplaceEntitlementService 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/marketplace-entitlement.html#MarketplaceEntitlementService)
+[aiobotocore.MarketplaceEntitlementService 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/marketplace-entitlement.html#MarketplaceEntitlementService)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-marketplace-entitlement-2.5.2.post2/setup.py` & `types-aiobotocore-marketplace-entitlement-2.5.4/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-marketplace-entitlement",
-    version="2.5.2.post2",
+    version="2.5.4",
     packages=["types_aiobotocore_marketplace_entitlement"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.MarketplaceEntitlementService 2.5.2 service generated"
+        "Type annotations for aiobotocore.MarketplaceEntitlementService 2.5.4 service generated"
         " with mypy-boto3-builder 7.17.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
```

### Comparing `types-aiobotocore-marketplace-entitlement-2.5.2.post2/types_aiobotocore_marketplace_entitlement/__init__.py` & `types-aiobotocore-marketplace-entitlement-2.5.4/types_aiobotocore_marketplace_entitlement/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-marketplace-entitlement-2.5.2.post2/types_aiobotocore_marketplace_entitlement/__init__.pyi` & `types-aiobotocore-marketplace-entitlement-2.5.4/types_aiobotocore_marketplace_entitlement/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-marketplace-entitlement-2.5.2.post2/types_aiobotocore_marketplace_entitlement/__main__.py` & `types-aiobotocore-marketplace-entitlement-2.5.4/types_aiobotocore_marketplace_entitlement/__main__.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.MarketplaceEntitlementService 2.5.2\nVersion:        "
-        " 2.5.2.post2\nBuilder version: 7.17.2\nDocs:           "
+        "Type annotations for aiobotocore.MarketplaceEntitlementService 2.5.4\nVersion:        "
+        " 2.5.4\nBuilder version: 7.17.2\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_marketplace_entitlement//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/marketplace-entitlement.html#MarketplaceEntitlementService\nOther"
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

### Comparing `types-aiobotocore-marketplace-entitlement-2.5.2.post2/types_aiobotocore_marketplace_entitlement/client.py` & `types-aiobotocore-marketplace-entitlement-2.5.4/types_aiobotocore_marketplace_entitlement/client.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-marketplace-entitlement-2.5.2.post2/types_aiobotocore_marketplace_entitlement/client.pyi` & `types-aiobotocore-marketplace-entitlement-2.5.4/types_aiobotocore_marketplace_entitlement/client.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-marketplace-entitlement-2.5.2.post2/types_aiobotocore_marketplace_entitlement/literals.py` & `types-aiobotocore-marketplace-entitlement-2.5.4/types_aiobotocore_marketplace_entitlement/literals.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-marketplace-entitlement-2.5.2.post2/types_aiobotocore_marketplace_entitlement/literals.pyi` & `types-aiobotocore-marketplace-entitlement-2.5.4/types_aiobotocore_marketplace_entitlement/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-marketplace-entitlement-2.5.2.post2/types_aiobotocore_marketplace_entitlement/paginator.py` & `types-aiobotocore-marketplace-entitlement-2.5.4/types_aiobotocore_marketplace_entitlement/paginator.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-marketplace-entitlement-2.5.2.post2/types_aiobotocore_marketplace_entitlement/paginator.pyi` & `types-aiobotocore-marketplace-entitlement-2.5.4/types_aiobotocore_marketplace_entitlement/paginator.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-marketplace-entitlement-2.5.2.post2/types_aiobotocore_marketplace_entitlement/type_defs.py` & `types-aiobotocore-marketplace-entitlement-2.5.4/types_aiobotocore_marketplace_entitlement/type_defs.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-marketplace-entitlement-2.5.2.post2/types_aiobotocore_marketplace_entitlement/type_defs.pyi` & `types-aiobotocore-marketplace-entitlement-2.5.4/types_aiobotocore_marketplace_entitlement/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-marketplace-entitlement-2.5.2.post2/types_aiobotocore_marketplace_entitlement.egg-info/PKG-INFO` & `types-aiobotocore-marketplace-entitlement-2.5.4/types_aiobotocore_marketplace_entitlement.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-marketplace-entitlement
-Version: 2.5.2.post2
-Summary: Type annotations for aiobotocore.MarketplaceEntitlementService 2.5.2 service generated with mypy-boto3-builder 7.17.2
+Version: 2.5.4
+Summary: Type annotations for aiobotocore.MarketplaceEntitlementService 2.5.4 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_marketplace_entitlement/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-marketplace-entitlement.svg?color=blue)](https://pypi.org/project/types-aiobotocore-marketplace-entitlement)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_marketplace_entitlement/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-marketplace-entitlement)](https://pepy.tech/project/types-aiobotocore-marketplace-entitlement)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.MarketplaceEntitlementService 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/marketplace-entitlement.html#MarketplaceEntitlementService)
+[aiobotocore.MarketplaceEntitlementService 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/marketplace-entitlement.html#MarketplaceEntitlementService)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-marketplace-entitlement-2.5.2.post2/types_aiobotocore_marketplace_entitlement.egg-info/SOURCES.txt` & `types-aiobotocore-marketplace-entitlement-2.5.4/types_aiobotocore_marketplace_entitlement.egg-info/SOURCES.txt`

 * *Files identical despite different names*


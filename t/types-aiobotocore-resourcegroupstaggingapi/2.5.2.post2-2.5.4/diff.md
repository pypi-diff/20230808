# Comparing `tmp/types-aiobotocore-resourcegroupstaggingapi-2.5.2.post2.tar.gz` & `tmp/types-aiobotocore-resourcegroupstaggingapi-2.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-resourcegroupstaggingapi-2.5.2.post2.tar", last modified: Fri Aug  4 13:59:23 2023, max compression
+gzip compressed data, was "types-aiobotocore-resourcegroupstaggingapi-2.5.4.tar", last modified: Tue Aug  8 01:24:19 2023, max compression
```

## Comparing `types-aiobotocore-resourcegroupstaggingapi-2.5.2.post2.tar` & `types-aiobotocore-resourcegroupstaggingapi-2.5.4.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:23.386643 types-aiobotocore-resourcegroupstaggingapi-2.5.2.post2/
--rw-r--r--   0 vlad      (1000) vlad      (1000)     1070 2023-08-04 13:50:49.000000 types-aiobotocore-resourcegroupstaggingapi-2.5.2.post2/LICENSE
--rw-r--r--   0 vlad      (1000) vlad      (1000)    14297 2023-08-04 13:59:23.386643 types-aiobotocore-resourcegroupstaggingapi-2.5.2.post2/PKG-INFO
--rw-r--r--   0 vlad      (1000) vlad      (1000)    12711 2023-08-04 13:50:49.000000 types-aiobotocore-resourcegroupstaggingapi-2.5.2.post2/README.md
--rw-r--r--   0 vlad      (1000) vlad      (1000)       38 2023-08-04 13:59:23.386643 types-aiobotocore-resourcegroupstaggingapi-2.5.2.post2/setup.cfg
--rw-r--r--   0 vlad      (1000) vlad      (1000)     2183 2023-08-04 13:50:48.000000 types-aiobotocore-resourcegroupstaggingapi-2.5.2.post2/setup.py
-drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:23.386643 types-aiobotocore-resourcegroupstaggingapi-2.5.2.post2/types_aiobotocore_resourcegroupstaggingapi/
--rw-r--r--   0 vlad      (1000) vlad      (1000)     1371 2023-08-04 13:50:49.000000 types-aiobotocore-resourcegroupstaggingapi-2.5.2.post2/types_aiobotocore_resourcegroupstaggingapi/__init__.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)     1370 2023-08-04 13:50:49.000000 types-aiobotocore-resourcegroupstaggingapi-2.5.2.post2/types_aiobotocore_resourcegroupstaggingapi/__init__.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)     1011 2023-08-04 13:50:49.000000 types-aiobotocore-resourcegroupstaggingapi-2.5.2.post2/types_aiobotocore_resourcegroupstaggingapi/__main__.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)    12694 2023-08-04 13:50:49.000000 types-aiobotocore-resourcegroupstaggingapi-2.5.2.post2/types_aiobotocore_resourcegroupstaggingapi/client.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)    12673 2023-08-04 13:50:49.000000 types-aiobotocore-resourcegroupstaggingapi-2.5.2.post2/types_aiobotocore_resourcegroupstaggingapi/client.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)     9063 2023-08-04 13:50:49.000000 types-aiobotocore-resourcegroupstaggingapi-2.5.2.post2/types_aiobotocore_resourcegroupstaggingapi/literals.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)     9061 2023-08-04 13:50:49.000000 types-aiobotocore-resourcegroupstaggingapi-2.5.2.post2/types_aiobotocore_resourcegroupstaggingapi/literals.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)     6296 2023-08-04 13:50:49.000000 types-aiobotocore-resourcegroupstaggingapi-2.5.2.post2/types_aiobotocore_resourcegroupstaggingapi/paginator.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)     6290 2023-08-04 13:50:49.000000 types-aiobotocore-resourcegroupstaggingapi-2.5.2.post2/types_aiobotocore_resourcegroupstaggingapi/paginator.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:50:49.000000 types-aiobotocore-resourcegroupstaggingapi-2.5.2.post2/types_aiobotocore_resourcegroupstaggingapi/py.typed
--rw-r--r--   0 vlad      (1000) vlad      (1000)     8261 2023-08-04 13:50:52.000000 types-aiobotocore-resourcegroupstaggingapi-2.5.2.post2/types_aiobotocore_resourcegroupstaggingapi/type_defs.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)     8256 2023-08-04 13:50:52.000000 types-aiobotocore-resourcegroupstaggingapi-2.5.2.post2/types_aiobotocore_resourcegroupstaggingapi/type_defs.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)       65 2023-08-04 13:50:49.000000 types-aiobotocore-resourcegroupstaggingapi-2.5.2.post2/types_aiobotocore_resourcegroupstaggingapi/version.py
-drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:23.386643 types-aiobotocore-resourcegroupstaggingapi-2.5.2.post2/types_aiobotocore_resourcegroupstaggingapi.egg-info/
--rw-r--r--   0 vlad      (1000) vlad      (1000)    14297 2023-08-04 13:59:23.000000 types-aiobotocore-resourcegroupstaggingapi-2.5.2.post2/types_aiobotocore_resourcegroupstaggingapi.egg-info/PKG-INFO
--rw-r--r--   0 vlad      (1000) vlad      (1000)     1136 2023-08-04 13:59:23.000000 types-aiobotocore-resourcegroupstaggingapi-2.5.2.post2/types_aiobotocore_resourcegroupstaggingapi.egg-info/SOURCES.txt
--rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:23.000000 types-aiobotocore-resourcegroupstaggingapi-2.5.2.post2/types_aiobotocore_resourcegroupstaggingapi.egg-info/dependency_links.txt
--rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:23.000000 types-aiobotocore-resourcegroupstaggingapi-2.5.2.post2/types_aiobotocore_resourcegroupstaggingapi.egg-info/not-zip-safe
--rw-r--r--   0 vlad      (1000) vlad      (1000)       52 2023-08-04 13:59:23.000000 types-aiobotocore-resourcegroupstaggingapi-2.5.2.post2/types_aiobotocore_resourcegroupstaggingapi.egg-info/requires.txt
--rw-r--r--   0 vlad      (1000) vlad      (1000)       43 2023-08-04 13:59:23.000000 types-aiobotocore-resourcegroupstaggingapi-2.5.2.post2/types_aiobotocore_resourcegroupstaggingapi.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:24:19.142763 types-aiobotocore-resourcegroupstaggingapi-2.5.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-08 01:19:27.000000 types-aiobotocore-resourcegroupstaggingapi-2.5.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    14291 2023-08-08 01:24:19.138763 types-aiobotocore-resourcegroupstaggingapi-2.5.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    12711 2023-08-08 01:19:27.000000 types-aiobotocore-resourcegroupstaggingapi-2.5.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-08 01:24:19.142763 types-aiobotocore-resourcegroupstaggingapi-2.5.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2177 2023-08-08 01:19:27.000000 types-aiobotocore-resourcegroupstaggingapi-2.5.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:24:19.122763 types-aiobotocore-resourcegroupstaggingapi-2.5.4/types_aiobotocore_resourcegroupstaggingapi/
+-rw-r--r--   0 runner    (1001) docker     (123)     1371 2023-08-08 01:19:27.000000 types-aiobotocore-resourcegroupstaggingapi-2.5.4/types_aiobotocore_resourcegroupstaggingapi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1370 2023-08-08 01:19:27.000000 types-aiobotocore-resourcegroupstaggingapi-2.5.4/types_aiobotocore_resourcegroupstaggingapi/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      999 2023-08-08 01:19:27.000000 types-aiobotocore-resourcegroupstaggingapi-2.5.4/types_aiobotocore_resourcegroupstaggingapi/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12694 2023-08-08 01:19:27.000000 types-aiobotocore-resourcegroupstaggingapi-2.5.4/types_aiobotocore_resourcegroupstaggingapi/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12673 2023-08-08 01:19:27.000000 types-aiobotocore-resourcegroupstaggingapi-2.5.4/types_aiobotocore_resourcegroupstaggingapi/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9063 2023-08-08 01:19:28.000000 types-aiobotocore-resourcegroupstaggingapi-2.5.4/types_aiobotocore_resourcegroupstaggingapi/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9061 2023-08-08 01:19:28.000000 types-aiobotocore-resourcegroupstaggingapi-2.5.4/types_aiobotocore_resourcegroupstaggingapi/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     6296 2023-08-08 01:19:27.000000 types-aiobotocore-resourcegroupstaggingapi-2.5.4/types_aiobotocore_resourcegroupstaggingapi/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6290 2023-08-08 01:19:27.000000 types-aiobotocore-resourcegroupstaggingapi-2.5.4/types_aiobotocore_resourcegroupstaggingapi/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 01:19:27.000000 types-aiobotocore-resourcegroupstaggingapi-2.5.4/types_aiobotocore_resourcegroupstaggingapi/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     8261 2023-08-08 01:19:28.000000 types-aiobotocore-resourcegroupstaggingapi-2.5.4/types_aiobotocore_resourcegroupstaggingapi/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8256 2023-08-08 01:19:28.000000 types-aiobotocore-resourcegroupstaggingapi-2.5.4/types_aiobotocore_resourcegroupstaggingapi/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-08-08 01:19:27.000000 types-aiobotocore-resourcegroupstaggingapi-2.5.4/types_aiobotocore_resourcegroupstaggingapi/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:24:19.138763 types-aiobotocore-resourcegroupstaggingapi-2.5.4/types_aiobotocore_resourcegroupstaggingapi.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    14291 2023-08-08 01:24:18.000000 types-aiobotocore-resourcegroupstaggingapi-2.5.4/types_aiobotocore_resourcegroupstaggingapi.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1136 2023-08-08 01:24:18.000000 types-aiobotocore-resourcegroupstaggingapi-2.5.4/types_aiobotocore_resourcegroupstaggingapi.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 01:24:18.000000 types-aiobotocore-resourcegroupstaggingapi-2.5.4/types_aiobotocore_resourcegroupstaggingapi.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 01:24:18.000000 types-aiobotocore-resourcegroupstaggingapi-2.5.4/types_aiobotocore_resourcegroupstaggingapi.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-08 01:24:18.000000 types-aiobotocore-resourcegroupstaggingapi-2.5.4/types_aiobotocore_resourcegroupstaggingapi.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-08-08 01:24:18.000000 types-aiobotocore-resourcegroupstaggingapi-2.5.4/types_aiobotocore_resourcegroupstaggingapi.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-resourcegroupstaggingapi-2.5.2.post2/LICENSE` & `types-aiobotocore-resourcegroupstaggingapi-2.5.4/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-resourcegroupstaggingapi-2.5.2.post2/PKG-INFO` & `types-aiobotocore-resourcegroupstaggingapi-2.5.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-resourcegroupstaggingapi
-Version: 2.5.2.post2
-Summary: Type annotations for aiobotocore.ResourceGroupsTaggingAPI 2.5.2 service generated with mypy-boto3-builder 7.17.2
+Version: 2.5.4
+Summary: Type annotations for aiobotocore.ResourceGroupsTaggingAPI 2.5.4 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_resourcegroupstaggingapi/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-resourcegroupstaggingapi.svg?color=blue)](https://pypi.org/project/types-aiobotocore-resourcegroupstaggingapi)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_resourcegroupstaggingapi/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-resourcegroupstaggingapi)](https://pepy.tech/project/types-aiobotocore-resourcegroupstaggingapi)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.ResourceGroupsTaggingAPI 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resourcegroupstaggingapi.html#ResourceGroupsTaggingAPI)
+[aiobotocore.ResourceGroupsTaggingAPI 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resourcegroupstaggingapi.html#ResourceGroupsTaggingAPI)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-resourcegroupstaggingapi-2.5.2.post2/README.md` & `types-aiobotocore-resourcegroupstaggingapi-2.5.4/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-resourcegroupstaggingapi.svg?color=blue)](https://pypi.org/project/types-aiobotocore-resourcegroupstaggingapi)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_resourcegroupstaggingapi/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-resourcegroupstaggingapi)](https://pepy.tech/project/types-aiobotocore-resourcegroupstaggingapi)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.ResourceGroupsTaggingAPI 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resourcegroupstaggingapi.html#ResourceGroupsTaggingAPI)
+[aiobotocore.ResourceGroupsTaggingAPI 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resourcegroupstaggingapi.html#ResourceGroupsTaggingAPI)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-resourcegroupstaggingapi-2.5.2.post2/setup.py` & `types-aiobotocore-resourcegroupstaggingapi-2.5.4/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-resourcegroupstaggingapi",
-    version="2.5.2.post2",
+    version="2.5.4",
     packages=["types_aiobotocore_resourcegroupstaggingapi"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.ResourceGroupsTaggingAPI 2.5.2 service generated with"
+        "Type annotations for aiobotocore.ResourceGroupsTaggingAPI 2.5.4 service generated with"
         " mypy-boto3-builder 7.17.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
```

### Comparing `types-aiobotocore-resourcegroupstaggingapi-2.5.2.post2/types_aiobotocore_resourcegroupstaggingapi/__init__.py` & `types-aiobotocore-resourcegroupstaggingapi-2.5.4/types_aiobotocore_resourcegroupstaggingapi/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-resourcegroupstaggingapi-2.5.2.post2/types_aiobotocore_resourcegroupstaggingapi/__init__.pyi` & `types-aiobotocore-resourcegroupstaggingapi-2.5.4/types_aiobotocore_resourcegroupstaggingapi/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-resourcegroupstaggingapi-2.5.2.post2/types_aiobotocore_resourcegroupstaggingapi/__main__.py` & `types-aiobotocore-resourcegroupstaggingapi-2.5.4/types_aiobotocore_resourcegroupstaggingapi/__main__.py`

 * *Files 10% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.ResourceGroupsTaggingAPI 2.5.2\nVersion:        "
-        " 2.5.2.post2\nBuilder version: 7.17.2\nDocs:           "
+        "Type annotations for aiobotocore.ResourceGroupsTaggingAPI 2.5.4\nVersion:        "
+        " 2.5.4\nBuilder version: 7.17.2\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_resourcegroupstaggingapi//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resourcegroupstaggingapi.html#ResourceGroupsTaggingAPI\nOther"
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

### Comparing `types-aiobotocore-resourcegroupstaggingapi-2.5.2.post2/types_aiobotocore_resourcegroupstaggingapi/client.py` & `types-aiobotocore-resourcegroupstaggingapi-2.5.4/types_aiobotocore_resourcegroupstaggingapi/client.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-resourcegroupstaggingapi-2.5.2.post2/types_aiobotocore_resourcegroupstaggingapi/client.pyi` & `types-aiobotocore-resourcegroupstaggingapi-2.5.4/types_aiobotocore_resourcegroupstaggingapi/client.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-resourcegroupstaggingapi-2.5.2.post2/types_aiobotocore_resourcegroupstaggingapi/literals.py` & `types-aiobotocore-resourcegroupstaggingapi-2.5.4/types_aiobotocore_resourcegroupstaggingapi/literals.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-resourcegroupstaggingapi-2.5.2.post2/types_aiobotocore_resourcegroupstaggingapi/literals.pyi` & `types-aiobotocore-resourcegroupstaggingapi-2.5.4/types_aiobotocore_resourcegroupstaggingapi/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-resourcegroupstaggingapi-2.5.2.post2/types_aiobotocore_resourcegroupstaggingapi/paginator.py` & `types-aiobotocore-resourcegroupstaggingapi-2.5.4/types_aiobotocore_resourcegroupstaggingapi/paginator.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-resourcegroupstaggingapi-2.5.2.post2/types_aiobotocore_resourcegroupstaggingapi/paginator.pyi` & `types-aiobotocore-resourcegroupstaggingapi-2.5.4/types_aiobotocore_resourcegroupstaggingapi/paginator.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-resourcegroupstaggingapi-2.5.2.post2/types_aiobotocore_resourcegroupstaggingapi/type_defs.py` & `types-aiobotocore-resourcegroupstaggingapi-2.5.4/types_aiobotocore_resourcegroupstaggingapi/type_defs.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-resourcegroupstaggingapi-2.5.2.post2/types_aiobotocore_resourcegroupstaggingapi/type_defs.pyi` & `types-aiobotocore-resourcegroupstaggingapi-2.5.4/types_aiobotocore_resourcegroupstaggingapi/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-resourcegroupstaggingapi-2.5.2.post2/types_aiobotocore_resourcegroupstaggingapi.egg-info/PKG-INFO` & `types-aiobotocore-resourcegroupstaggingapi-2.5.4/types_aiobotocore_resourcegroupstaggingapi.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-resourcegroupstaggingapi
-Version: 2.5.2.post2
-Summary: Type annotations for aiobotocore.ResourceGroupsTaggingAPI 2.5.2 service generated with mypy-boto3-builder 7.17.2
+Version: 2.5.4
+Summary: Type annotations for aiobotocore.ResourceGroupsTaggingAPI 2.5.4 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_resourcegroupstaggingapi/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-resourcegroupstaggingapi.svg?color=blue)](https://pypi.org/project/types-aiobotocore-resourcegroupstaggingapi)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_resourcegroupstaggingapi/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-resourcegroupstaggingapi)](https://pepy.tech/project/types-aiobotocore-resourcegroupstaggingapi)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.ResourceGroupsTaggingAPI 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resourcegroupstaggingapi.html#ResourceGroupsTaggingAPI)
+[aiobotocore.ResourceGroupsTaggingAPI 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resourcegroupstaggingapi.html#ResourceGroupsTaggingAPI)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-resourcegroupstaggingapi-2.5.2.post2/types_aiobotocore_resourcegroupstaggingapi.egg-info/SOURCES.txt` & `types-aiobotocore-resourcegroupstaggingapi-2.5.4/types_aiobotocore_resourcegroupstaggingapi.egg-info/SOURCES.txt`

 * *Files identical despite different names*


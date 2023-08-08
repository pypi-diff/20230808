# Comparing `tmp/types-aiobotocore-schemas-2.5.2.post2.tar.gz` & `tmp/types-aiobotocore-schemas-2.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-schemas-2.5.2.post2.tar", last modified: Fri Aug  4 13:59:25 2023, max compression
+gzip compressed data, was "types-aiobotocore-schemas-2.5.4.tar", last modified: Tue Aug  8 01:24:24 2023, max compression
```

## Comparing `types-aiobotocore-schemas-2.5.2.post2.tar` & `types-aiobotocore-schemas-2.5.4.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:25.696643 types-aiobotocore-schemas-2.5.2.post2/
--rw-r--r--   0 vlad      (1000) vlad      (1000)     1070 2023-08-04 13:52:39.000000 types-aiobotocore-schemas-2.5.2.post2/LICENSE
--rw-r--r--   0 vlad      (1000) vlad      (1000)    14181 2023-08-04 13:59:25.696643 types-aiobotocore-schemas-2.5.2.post2/PKG-INFO
--rw-r--r--   0 vlad      (1000) vlad      (1000)    12663 2023-08-04 13:52:39.000000 types-aiobotocore-schemas-2.5.2.post2/README.md
--rw-r--r--   0 vlad      (1000) vlad      (1000)       38 2023-08-04 13:59:25.696643 types-aiobotocore-schemas-2.5.2.post2/setup.cfg
--rw-r--r--   0 vlad      (1000) vlad      (1000)     2072 2023-08-04 13:52:39.000000 types-aiobotocore-schemas-2.5.2.post2/setup.py
-drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:25.696643 types-aiobotocore-schemas-2.5.2.post2/types_aiobotocore_schemas/
--rw-r--r--   0 vlad      (1000) vlad      (1000)     1647 2023-08-04 13:52:39.000000 types-aiobotocore-schemas-2.5.2.post2/types_aiobotocore_schemas/__init__.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)     1646 2023-08-04 13:52:39.000000 types-aiobotocore-schemas-2.5.2.post2/types_aiobotocore_schemas/__init__.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)      943 2023-08-04 13:52:39.000000 types-aiobotocore-schemas-2.5.2.post2/types_aiobotocore_schemas/__main__.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)    25263 2023-08-04 13:52:39.000000 types-aiobotocore-schemas-2.5.2.post2/types_aiobotocore_schemas/client.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)    25217 2023-08-04 13:52:39.000000 types-aiobotocore-schemas-2.5.2.post2/types_aiobotocore_schemas/client.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)     9045 2023-08-04 13:52:40.000000 types-aiobotocore-schemas-2.5.2.post2/types_aiobotocore_schemas/literals.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)     9043 2023-08-04 13:52:39.000000 types-aiobotocore-schemas-2.5.2.post2/types_aiobotocore_schemas/literals.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)     6566 2023-08-04 13:52:39.000000 types-aiobotocore-schemas-2.5.2.post2/types_aiobotocore_schemas/paginator.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)     6559 2023-08-04 13:52:39.000000 types-aiobotocore-schemas-2.5.2.post2/types_aiobotocore_schemas/paginator.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:52:39.000000 types-aiobotocore-schemas-2.5.2.post2/types_aiobotocore_schemas/py.typed
--rw-r--r--   0 vlad      (1000) vlad      (1000)    26134 2023-08-04 13:52:40.000000 types-aiobotocore-schemas-2.5.2.post2/types_aiobotocore_schemas/type_defs.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)    26095 2023-08-04 13:52:40.000000 types-aiobotocore-schemas-2.5.2.post2/types_aiobotocore_schemas/type_defs.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)       65 2023-08-04 13:52:39.000000 types-aiobotocore-schemas-2.5.2.post2/types_aiobotocore_schemas/version.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)     1674 2023-08-04 13:52:39.000000 types-aiobotocore-schemas-2.5.2.post2/types_aiobotocore_schemas/waiter.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)     1673 2023-08-04 13:52:39.000000 types-aiobotocore-schemas-2.5.2.post2/types_aiobotocore_schemas/waiter.pyi
-drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:25.696643 types-aiobotocore-schemas-2.5.2.post2/types_aiobotocore_schemas.egg-info/
--rw-r--r--   0 vlad      (1000) vlad      (1000)    14181 2023-08-04 13:59:25.000000 types-aiobotocore-schemas-2.5.2.post2/types_aiobotocore_schemas.egg-info/PKG-INFO
--rw-r--r--   0 vlad      (1000) vlad      (1000)      886 2023-08-04 13:59:25.000000 types-aiobotocore-schemas-2.5.2.post2/types_aiobotocore_schemas.egg-info/SOURCES.txt
--rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:25.000000 types-aiobotocore-schemas-2.5.2.post2/types_aiobotocore_schemas.egg-info/dependency_links.txt
--rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:25.000000 types-aiobotocore-schemas-2.5.2.post2/types_aiobotocore_schemas.egg-info/not-zip-safe
--rw-r--r--   0 vlad      (1000) vlad      (1000)       52 2023-08-04 13:59:25.000000 types-aiobotocore-schemas-2.5.2.post2/types_aiobotocore_schemas.egg-info/requires.txt
--rw-r--r--   0 vlad      (1000) vlad      (1000)       26 2023-08-04 13:59:25.000000 types-aiobotocore-schemas-2.5.2.post2/types_aiobotocore_schemas.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:24:24.630776 types-aiobotocore-schemas-2.5.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-08 01:20:34.000000 types-aiobotocore-schemas-2.5.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    14175 2023-08-08 01:24:24.622776 types-aiobotocore-schemas-2.5.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    12663 2023-08-08 01:20:34.000000 types-aiobotocore-schemas-2.5.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-08 01:24:24.630776 types-aiobotocore-schemas-2.5.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2066 2023-08-08 01:20:34.000000 types-aiobotocore-schemas-2.5.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:24:24.622776 types-aiobotocore-schemas-2.5.4/types_aiobotocore_schemas/
+-rw-r--r--   0 runner    (1001) docker     (123)     1647 2023-08-08 01:20:34.000000 types-aiobotocore-schemas-2.5.4/types_aiobotocore_schemas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1646 2023-08-08 01:20:34.000000 types-aiobotocore-schemas-2.5.4/types_aiobotocore_schemas/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      931 2023-08-08 01:20:34.000000 types-aiobotocore-schemas-2.5.4/types_aiobotocore_schemas/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25263 2023-08-08 01:20:34.000000 types-aiobotocore-schemas-2.5.4/types_aiobotocore_schemas/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25217 2023-08-08 01:20:34.000000 types-aiobotocore-schemas-2.5.4/types_aiobotocore_schemas/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9045 2023-08-08 01:20:34.000000 types-aiobotocore-schemas-2.5.4/types_aiobotocore_schemas/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9043 2023-08-08 01:20:34.000000 types-aiobotocore-schemas-2.5.4/types_aiobotocore_schemas/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     6566 2023-08-08 01:20:34.000000 types-aiobotocore-schemas-2.5.4/types_aiobotocore_schemas/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6559 2023-08-08 01:20:34.000000 types-aiobotocore-schemas-2.5.4/types_aiobotocore_schemas/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 01:20:34.000000 types-aiobotocore-schemas-2.5.4/types_aiobotocore_schemas/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    26134 2023-08-08 01:20:35.000000 types-aiobotocore-schemas-2.5.4/types_aiobotocore_schemas/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26095 2023-08-08 01:20:35.000000 types-aiobotocore-schemas-2.5.4/types_aiobotocore_schemas/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-08-08 01:20:34.000000 types-aiobotocore-schemas-2.5.4/types_aiobotocore_schemas/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1674 2023-08-08 01:20:34.000000 types-aiobotocore-schemas-2.5.4/types_aiobotocore_schemas/waiter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1673 2023-08-08 01:20:34.000000 types-aiobotocore-schemas-2.5.4/types_aiobotocore_schemas/waiter.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:24:24.622776 types-aiobotocore-schemas-2.5.4/types_aiobotocore_schemas.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    14175 2023-08-08 01:24:24.000000 types-aiobotocore-schemas-2.5.4/types_aiobotocore_schemas.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      886 2023-08-08 01:24:24.000000 types-aiobotocore-schemas-2.5.4/types_aiobotocore_schemas.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 01:24:24.000000 types-aiobotocore-schemas-2.5.4/types_aiobotocore_schemas.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 01:24:24.000000 types-aiobotocore-schemas-2.5.4/types_aiobotocore_schemas.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-08 01:24:24.000000 types-aiobotocore-schemas-2.5.4/types_aiobotocore_schemas.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-08-08 01:24:24.000000 types-aiobotocore-schemas-2.5.4/types_aiobotocore_schemas.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-schemas-2.5.2.post2/LICENSE` & `types-aiobotocore-schemas-2.5.4/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-schemas-2.5.2.post2/PKG-INFO` & `types-aiobotocore-schemas-2.5.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-schemas
-Version: 2.5.2.post2
-Summary: Type annotations for aiobotocore.Schemas 2.5.2 service generated with mypy-boto3-builder 7.17.2
+Version: 2.5.4
+Summary: Type annotations for aiobotocore.Schemas 2.5.4 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_schemas/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-schemas.svg?color=blue)](https://pypi.org/project/types-aiobotocore-schemas)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_schemas/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-schemas)](https://pepy.tech/project/types-aiobotocore-schemas)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.Schemas 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/schemas.html#Schemas)
+[aiobotocore.Schemas 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/schemas.html#Schemas)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-schemas-2.5.2.post2/README.md` & `types-aiobotocore-schemas-2.5.4/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-schemas.svg?color=blue)](https://pypi.org/project/types-aiobotocore-schemas)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_schemas/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-schemas)](https://pepy.tech/project/types-aiobotocore-schemas)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.Schemas 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/schemas.html#Schemas)
+[aiobotocore.Schemas 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/schemas.html#Schemas)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-schemas-2.5.2.post2/setup.py` & `types-aiobotocore-schemas-2.5.4/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-schemas",
-    version="2.5.2.post2",
+    version="2.5.4",
     packages=["types_aiobotocore_schemas"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.Schemas 2.5.2 service generated with mypy-boto3-builder"
+        "Type annotations for aiobotocore.Schemas 2.5.4 service generated with mypy-boto3-builder"
         " 7.17.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
```

### Comparing `types-aiobotocore-schemas-2.5.2.post2/types_aiobotocore_schemas/__init__.py` & `types-aiobotocore-schemas-2.5.4/types_aiobotocore_schemas/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-schemas-2.5.2.post2/types_aiobotocore_schemas/__init__.pyi` & `types-aiobotocore-schemas-2.5.4/types_aiobotocore_schemas/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-schemas-2.5.2.post2/types_aiobotocore_schemas/__main__.py` & `types-aiobotocore-schemas-2.5.4/types_aiobotocore_schemas/__main__.py`

 * *Files 7% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.Schemas 2.5.2\nVersion:         2.5.2.post2\nBuilder"
-        " version: 7.17.2\nDocs:           "
+        "Type annotations for aiobotocore.Schemas 2.5.4\nVersion:         2.5.4\nBuilder version:"
+        " 7.17.2\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_schemas//\nBoto3 docs:"
         "     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/schemas.html#Schemas\nOther"
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

### Comparing `types-aiobotocore-schemas-2.5.2.post2/types_aiobotocore_schemas/client.py` & `types-aiobotocore-schemas-2.5.4/types_aiobotocore_schemas/client.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-schemas-2.5.2.post2/types_aiobotocore_schemas/client.pyi` & `types-aiobotocore-schemas-2.5.4/types_aiobotocore_schemas/client.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-schemas-2.5.2.post2/types_aiobotocore_schemas/literals.py` & `types-aiobotocore-schemas-2.5.4/types_aiobotocore_schemas/literals.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-schemas-2.5.2.post2/types_aiobotocore_schemas/literals.pyi` & `types-aiobotocore-schemas-2.5.4/types_aiobotocore_schemas/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-schemas-2.5.2.post2/types_aiobotocore_schemas/paginator.py` & `types-aiobotocore-schemas-2.5.4/types_aiobotocore_schemas/paginator.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-schemas-2.5.2.post2/types_aiobotocore_schemas/paginator.pyi` & `types-aiobotocore-schemas-2.5.4/types_aiobotocore_schemas/paginator.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-schemas-2.5.2.post2/types_aiobotocore_schemas/type_defs.py` & `types-aiobotocore-schemas-2.5.4/types_aiobotocore_schemas/type_defs.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-schemas-2.5.2.post2/types_aiobotocore_schemas/type_defs.pyi` & `types-aiobotocore-schemas-2.5.4/types_aiobotocore_schemas/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-schemas-2.5.2.post2/types_aiobotocore_schemas/waiter.py` & `types-aiobotocore-schemas-2.5.4/types_aiobotocore_schemas/waiter.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-schemas-2.5.2.post2/types_aiobotocore_schemas/waiter.pyi` & `types-aiobotocore-schemas-2.5.4/types_aiobotocore_schemas/waiter.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-schemas-2.5.2.post2/types_aiobotocore_schemas.egg-info/PKG-INFO` & `types-aiobotocore-schemas-2.5.4/types_aiobotocore_schemas.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-schemas
-Version: 2.5.2.post2
-Summary: Type annotations for aiobotocore.Schemas 2.5.2 service generated with mypy-boto3-builder 7.17.2
+Version: 2.5.4
+Summary: Type annotations for aiobotocore.Schemas 2.5.4 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_schemas/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-schemas.svg?color=blue)](https://pypi.org/project/types-aiobotocore-schemas)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_schemas/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-schemas)](https://pepy.tech/project/types-aiobotocore-schemas)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.Schemas 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/schemas.html#Schemas)
+[aiobotocore.Schemas 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/schemas.html#Schemas)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-schemas-2.5.2.post2/types_aiobotocore_schemas.egg-info/SOURCES.txt` & `types-aiobotocore-schemas-2.5.4/types_aiobotocore_schemas.egg-info/SOURCES.txt`

 * *Files identical despite different names*


# Comparing `tmp/types-aiobotocore-lakeformation-2.5.2.post2.tar.gz` & `tmp/types-aiobotocore-lakeformation-2.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-lakeformation-2.5.2.post2.tar", last modified: Fri Aug  4 13:59:15 2023, max compression
+gzip compressed data, was "types-aiobotocore-lakeformation-2.5.4.tar", last modified: Tue Aug  8 01:23:59 2023, max compression
```

## Comparing `types-aiobotocore-lakeformation-2.5.2.post2.tar` & `types-aiobotocore-lakeformation-2.5.4.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:15.036643 types-aiobotocore-lakeformation-2.5.2.post2/
--rw-r--r--   0 vlad      (1000) vlad      (1000)     1070 2023-08-04 13:42:20.000000 types-aiobotocore-lakeformation-2.5.2.post2/LICENSE
--rw-r--r--   0 vlad      (1000) vlad      (1000)    13882 2023-08-04 13:59:15.036643 types-aiobotocore-lakeformation-2.5.2.post2/PKG-INFO
--rw-r--r--   0 vlad      (1000) vlad      (1000)    12340 2023-08-04 13:42:20.000000 types-aiobotocore-lakeformation-2.5.2.post2/README.md
--rw-r--r--   0 vlad      (1000) vlad      (1000)       38 2023-08-04 13:59:15.036643 types-aiobotocore-lakeformation-2.5.2.post2/setup.cfg
--rw-r--r--   0 vlad      (1000) vlad      (1000)     2114 2023-08-04 13:42:19.000000 types-aiobotocore-lakeformation-2.5.2.post2/setup.py
-drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:15.036643 types-aiobotocore-lakeformation-2.5.2.post2/types_aiobotocore_lakeformation/
--rw-r--r--   0 vlad      (1000) vlad      (1000)     1583 2023-08-04 13:42:20.000000 types-aiobotocore-lakeformation-2.5.2.post2/types_aiobotocore_lakeformation/__init__.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)     1582 2023-08-04 13:42:20.000000 types-aiobotocore-lakeformation-2.5.2.post2/types_aiobotocore_lakeformation/__init__.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)      967 2023-08-04 13:42:20.000000 types-aiobotocore-lakeformation-2.5.2.post2/types_aiobotocore_lakeformation/__main__.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)    39384 2023-08-04 13:42:20.000000 types-aiobotocore-lakeformation-2.5.2.post2/types_aiobotocore_lakeformation/client.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)    39323 2023-08-04 13:42:20.000000 types-aiobotocore-lakeformation-2.5.2.post2/types_aiobotocore_lakeformation/client.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)    10579 2023-08-04 13:42:21.000000 types-aiobotocore-lakeformation-2.5.2.post2/types_aiobotocore_lakeformation/literals.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)    10577 2023-08-04 13:42:21.000000 types-aiobotocore-lakeformation-2.5.2.post2/types_aiobotocore_lakeformation/literals.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)     7069 2023-08-04 13:42:20.000000 types-aiobotocore-lakeformation-2.5.2.post2/types_aiobotocore_lakeformation/paginator.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)     7062 2023-08-04 13:42:20.000000 types-aiobotocore-lakeformation-2.5.2.post2/types_aiobotocore_lakeformation/paginator.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:42:20.000000 types-aiobotocore-lakeformation-2.5.2.post2/types_aiobotocore_lakeformation/py.typed
--rw-r--r--   0 vlad      (1000) vlad      (1000)    48362 2023-08-04 13:42:22.000000 types-aiobotocore-lakeformation-2.5.2.post2/types_aiobotocore_lakeformation/type_defs.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)    48277 2023-08-04 13:42:21.000000 types-aiobotocore-lakeformation-2.5.2.post2/types_aiobotocore_lakeformation/type_defs.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)       65 2023-08-04 13:42:20.000000 types-aiobotocore-lakeformation-2.5.2.post2/types_aiobotocore_lakeformation/version.py
-drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:15.036643 types-aiobotocore-lakeformation-2.5.2.post2/types_aiobotocore_lakeformation.egg-info/
--rw-r--r--   0 vlad      (1000) vlad      (1000)    13882 2023-08-04 13:59:14.000000 types-aiobotocore-lakeformation-2.5.2.post2/types_aiobotocore_lakeformation.egg-info/PKG-INFO
--rw-r--r--   0 vlad      (1000) vlad      (1000)      927 2023-08-04 13:59:14.000000 types-aiobotocore-lakeformation-2.5.2.post2/types_aiobotocore_lakeformation.egg-info/SOURCES.txt
--rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:14.000000 types-aiobotocore-lakeformation-2.5.2.post2/types_aiobotocore_lakeformation.egg-info/dependency_links.txt
--rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:14.000000 types-aiobotocore-lakeformation-2.5.2.post2/types_aiobotocore_lakeformation.egg-info/not-zip-safe
--rw-r--r--   0 vlad      (1000) vlad      (1000)       52 2023-08-04 13:59:14.000000 types-aiobotocore-lakeformation-2.5.2.post2/types_aiobotocore_lakeformation.egg-info/requires.txt
--rw-r--r--   0 vlad      (1000) vlad      (1000)       32 2023-08-04 13:59:14.000000 types-aiobotocore-lakeformation-2.5.2.post2/types_aiobotocore_lakeformation.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:23:59.382722 types-aiobotocore-lakeformation-2.5.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-08 01:13:46.000000 types-aiobotocore-lakeformation-2.5.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    13876 2023-08-08 01:23:59.370722 types-aiobotocore-lakeformation-2.5.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    12340 2023-08-08 01:13:46.000000 types-aiobotocore-lakeformation-2.5.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-08 01:23:59.382722 types-aiobotocore-lakeformation-2.5.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2108 2023-08-08 01:13:45.000000 types-aiobotocore-lakeformation-2.5.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:23:59.366722 types-aiobotocore-lakeformation-2.5.4/types_aiobotocore_lakeformation/
+-rw-r--r--   0 runner    (1001) docker     (123)     1583 2023-08-08 01:13:46.000000 types-aiobotocore-lakeformation-2.5.4/types_aiobotocore_lakeformation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1582 2023-08-08 01:13:46.000000 types-aiobotocore-lakeformation-2.5.4/types_aiobotocore_lakeformation/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      955 2023-08-08 01:13:46.000000 types-aiobotocore-lakeformation-2.5.4/types_aiobotocore_lakeformation/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39384 2023-08-08 01:13:46.000000 types-aiobotocore-lakeformation-2.5.4/types_aiobotocore_lakeformation/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39323 2023-08-08 01:13:46.000000 types-aiobotocore-lakeformation-2.5.4/types_aiobotocore_lakeformation/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    10519 2023-08-08 01:13:48.000000 types-aiobotocore-lakeformation-2.5.4/types_aiobotocore_lakeformation/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10517 2023-08-08 01:13:46.000000 types-aiobotocore-lakeformation-2.5.4/types_aiobotocore_lakeformation/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     7069 2023-08-08 01:13:46.000000 types-aiobotocore-lakeformation-2.5.4/types_aiobotocore_lakeformation/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7062 2023-08-08 01:13:46.000000 types-aiobotocore-lakeformation-2.5.4/types_aiobotocore_lakeformation/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 01:13:46.000000 types-aiobotocore-lakeformation-2.5.4/types_aiobotocore_lakeformation/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    48362 2023-08-08 01:13:49.000000 types-aiobotocore-lakeformation-2.5.4/types_aiobotocore_lakeformation/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    48277 2023-08-08 01:13:48.000000 types-aiobotocore-lakeformation-2.5.4/types_aiobotocore_lakeformation/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-08-08 01:13:46.000000 types-aiobotocore-lakeformation-2.5.4/types_aiobotocore_lakeformation/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:23:59.370722 types-aiobotocore-lakeformation-2.5.4/types_aiobotocore_lakeformation.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    13876 2023-08-08 01:23:59.000000 types-aiobotocore-lakeformation-2.5.4/types_aiobotocore_lakeformation.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      927 2023-08-08 01:23:59.000000 types-aiobotocore-lakeformation-2.5.4/types_aiobotocore_lakeformation.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 01:23:59.000000 types-aiobotocore-lakeformation-2.5.4/types_aiobotocore_lakeformation.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 01:23:59.000000 types-aiobotocore-lakeformation-2.5.4/types_aiobotocore_lakeformation.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-08 01:23:59.000000 types-aiobotocore-lakeformation-2.5.4/types_aiobotocore_lakeformation.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-08-08 01:23:59.000000 types-aiobotocore-lakeformation-2.5.4/types_aiobotocore_lakeformation.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-lakeformation-2.5.2.post2/LICENSE` & `types-aiobotocore-lakeformation-2.5.4/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-lakeformation-2.5.2.post2/PKG-INFO` & `types-aiobotocore-lakeformation-2.5.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-lakeformation
-Version: 2.5.2.post2
-Summary: Type annotations for aiobotocore.LakeFormation 2.5.2 service generated with mypy-boto3-builder 7.17.2
+Version: 2.5.4
+Summary: Type annotations for aiobotocore.LakeFormation 2.5.4 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lakeformation/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-lakeformation.svg?color=blue)](https://pypi.org/project/types-aiobotocore-lakeformation)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lakeformation/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-lakeformation)](https://pepy.tech/project/types-aiobotocore-lakeformation)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.LakeFormation 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lakeformation.html#LakeFormation)
+[aiobotocore.LakeFormation 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lakeformation.html#LakeFormation)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-lakeformation-2.5.2.post2/README.md` & `types-aiobotocore-lakeformation-2.5.4/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-lakeformation.svg?color=blue)](https://pypi.org/project/types-aiobotocore-lakeformation)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lakeformation/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-lakeformation)](https://pepy.tech/project/types-aiobotocore-lakeformation)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.LakeFormation 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lakeformation.html#LakeFormation)
+[aiobotocore.LakeFormation 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lakeformation.html#LakeFormation)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-lakeformation-2.5.2.post2/setup.py` & `types-aiobotocore-lakeformation-2.5.4/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-lakeformation",
-    version="2.5.2.post2",
+    version="2.5.4",
     packages=["types_aiobotocore_lakeformation"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.LakeFormation 2.5.2 service generated with"
+        "Type annotations for aiobotocore.LakeFormation 2.5.4 service generated with"
         " mypy-boto3-builder 7.17.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
```

### Comparing `types-aiobotocore-lakeformation-2.5.2.post2/types_aiobotocore_lakeformation/__init__.py` & `types-aiobotocore-lakeformation-2.5.4/types_aiobotocore_lakeformation/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-lakeformation-2.5.2.post2/types_aiobotocore_lakeformation/__init__.pyi` & `types-aiobotocore-lakeformation-2.5.4/types_aiobotocore_lakeformation/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-lakeformation-2.5.2.post2/types_aiobotocore_lakeformation/__main__.py` & `types-aiobotocore-lakeformation-2.5.4/types_aiobotocore_lakeformation/__main__.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.LakeFormation 2.5.2\nVersion:        "
-        " 2.5.2.post2\nBuilder version: 7.17.2\nDocs:           "
+        "Type annotations for aiobotocore.LakeFormation 2.5.4\nVersion:         2.5.4\nBuilder"
+        " version: 7.17.2\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lakeformation//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lakeformation.html#LakeFormation\nOther"
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

### Comparing `types-aiobotocore-lakeformation-2.5.2.post2/types_aiobotocore_lakeformation/client.py` & `types-aiobotocore-lakeformation-2.5.4/types_aiobotocore_lakeformation/client.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-lakeformation-2.5.2.post2/types_aiobotocore_lakeformation/client.pyi` & `types-aiobotocore-lakeformation-2.5.4/types_aiobotocore_lakeformation/client.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-lakeformation-2.5.2.post2/types_aiobotocore_lakeformation/literals.py` & `types-aiobotocore-lakeformation-2.5.4/types_aiobotocore_lakeformation/literals.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -14,15 +14,14 @@
 import sys
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = (
     "ComparisonOperatorType",
     "DataLakeResourceTypeType",
     "FieldNameStringType",
     "GetWorkUnitsPaginatorName",
     "ListDataCellsFilterPaginatorName",
     "ListLFTagsPaginatorName",
@@ -40,15 +39,14 @@
     "LakeFormationServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "RegionName",
 )
 
-
 ComparisonOperatorType = Literal[
     "BEGINS_WITH", "BETWEEN", "CONTAINS", "EQ", "GE", "GT", "IN", "LE", "LT", "NE", "NOT_CONTAINS"
 ]
 DataLakeResourceTypeType = Literal[
     "CATALOG",
     "DATABASE",
     "DATA_LOCATION",
@@ -467,29 +465,26 @@
 RegionName = Literal[
     "af-south-1",
     "ap-east-1",
     "ap-northeast-1",
     "ap-northeast-2",
     "ap-northeast-3",
     "ap-south-1",
-    "ap-south-2",
     "ap-southeast-1",
     "ap-southeast-2",
     "ap-southeast-3",
-    "ap-southeast-4",
     "ca-central-1",
     "eu-central-1",
     "eu-central-2",
     "eu-north-1",
     "eu-south-1",
     "eu-south-2",
     "eu-west-1",
     "eu-west-2",
     "eu-west-3",
-    "il-central-1",
     "me-central-1",
     "me-south-1",
     "sa-east-1",
     "us-east-1",
     "us-east-2",
     "us-west-1",
     "us-west-2",
```

### Comparing `types-aiobotocore-lakeformation-2.5.2.post2/types_aiobotocore_lakeformation/literals.pyi` & `types-aiobotocore-lakeformation-2.5.4/types_aiobotocore_lakeformation/literals.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 import sys
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
+
 __all__ = (
     "ComparisonOperatorType",
     "DataLakeResourceTypeType",
     "FieldNameStringType",
     "GetWorkUnitsPaginatorName",
     "ListDataCellsFilterPaginatorName",
     "ListLFTagsPaginatorName",
@@ -39,14 +40,15 @@
     "LakeFormationServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "RegionName",
 )
 
+
 ComparisonOperatorType = Literal[
     "BEGINS_WITH", "BETWEEN", "CONTAINS", "EQ", "GE", "GT", "IN", "LE", "LT", "NE", "NOT_CONTAINS"
 ]
 DataLakeResourceTypeType = Literal[
     "CATALOG",
     "DATABASE",
     "DATA_LOCATION",
@@ -465,29 +467,26 @@
 RegionName = Literal[
     "af-south-1",
     "ap-east-1",
     "ap-northeast-1",
     "ap-northeast-2",
     "ap-northeast-3",
     "ap-south-1",
-    "ap-south-2",
     "ap-southeast-1",
     "ap-southeast-2",
     "ap-southeast-3",
-    "ap-southeast-4",
     "ca-central-1",
     "eu-central-1",
     "eu-central-2",
     "eu-north-1",
     "eu-south-1",
     "eu-south-2",
     "eu-west-1",
     "eu-west-2",
     "eu-west-3",
-    "il-central-1",
     "me-central-1",
     "me-south-1",
     "sa-east-1",
     "us-east-1",
     "us-east-2",
     "us-west-1",
     "us-west-2",
```

### Comparing `types-aiobotocore-lakeformation-2.5.2.post2/types_aiobotocore_lakeformation/paginator.py` & `types-aiobotocore-lakeformation-2.5.4/types_aiobotocore_lakeformation/paginator.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-lakeformation-2.5.2.post2/types_aiobotocore_lakeformation/paginator.pyi` & `types-aiobotocore-lakeformation-2.5.4/types_aiobotocore_lakeformation/paginator.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-lakeformation-2.5.2.post2/types_aiobotocore_lakeformation/type_defs.py` & `types-aiobotocore-lakeformation-2.5.4/types_aiobotocore_lakeformation/type_defs.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-lakeformation-2.5.2.post2/types_aiobotocore_lakeformation/type_defs.pyi` & `types-aiobotocore-lakeformation-2.5.4/types_aiobotocore_lakeformation/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-lakeformation-2.5.2.post2/types_aiobotocore_lakeformation.egg-info/PKG-INFO` & `types-aiobotocore-lakeformation-2.5.4/types_aiobotocore_lakeformation.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-lakeformation
-Version: 2.5.2.post2
-Summary: Type annotations for aiobotocore.LakeFormation 2.5.2 service generated with mypy-boto3-builder 7.17.2
+Version: 2.5.4
+Summary: Type annotations for aiobotocore.LakeFormation 2.5.4 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lakeformation/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-lakeformation.svg?color=blue)](https://pypi.org/project/types-aiobotocore-lakeformation)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lakeformation/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-lakeformation)](https://pepy.tech/project/types-aiobotocore-lakeformation)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.LakeFormation 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lakeformation.html#LakeFormation)
+[aiobotocore.LakeFormation 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lakeformation.html#LakeFormation)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-lakeformation-2.5.2.post2/types_aiobotocore_lakeformation.egg-info/SOURCES.txt` & `types-aiobotocore-lakeformation-2.5.4/types_aiobotocore_lakeformation.egg-info/SOURCES.txt`

 * *Files identical despite different names*


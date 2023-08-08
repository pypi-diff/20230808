# Comparing `tmp/types-aiobotocore-athena-2.5.2.post3.tar.gz` & `tmp/types-aiobotocore-athena-2.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-athena-2.5.2.post3.tar", last modified: Fri Aug  4 12:37:19 2023, max compression
+gzip compressed data, was "types-aiobotocore-athena-2.5.4.tar", last modified: Tue Aug  8 01:23:19 2023, max compression
```

## Comparing `types-aiobotocore-athena-2.5.2.post3.tar` & `types-aiobotocore-athena-2.5.4.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:37:19.003228 types-aiobotocore-athena-2.5.2.post3/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-04 12:18:41.000000 types-aiobotocore-athena-2.5.2.post3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    13797 2023-08-04 12:37:19.003228 types-aiobotocore-athena-2.5.2.post3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    12283 2023-08-04 12:18:41.000000 types-aiobotocore-athena-2.5.2.post3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-04 12:37:19.003228 types-aiobotocore-athena-2.5.2.post3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2065 2023-08-04 12:18:41.000000 types-aiobotocore-athena-2.5.2.post3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:37:18.995227 types-aiobotocore-athena-2.5.2.post3/types_aiobotocore_athena/
--rw-r--r--   0 runner    (1001) docker     (123)     1919 2023-08-04 12:18:41.000000 types-aiobotocore-athena-2.5.2.post3/types_aiobotocore_athena/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1918 2023-08-04 12:18:41.000000 types-aiobotocore-athena-2.5.2.post3/types_aiobotocore_athena/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      928 2023-08-04 12:18:41.000000 types-aiobotocore-athena-2.5.2.post3/types_aiobotocore_athena/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    48904 2023-08-04 12:18:41.000000 types-aiobotocore-athena-2.5.2.post3/types_aiobotocore_athena/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    48820 2023-08-04 12:18:41.000000 types-aiobotocore-athena-2.5.2.post3/types_aiobotocore_athena/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    10421 2023-08-04 12:18:41.000000 types-aiobotocore-athena-2.5.2.post3/types_aiobotocore_athena/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    10419 2023-08-04 12:18:41.000000 types-aiobotocore-athena-2.5.2.post3/types_aiobotocore_athena/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8690 2023-08-04 12:18:41.000000 types-aiobotocore-athena-2.5.2.post3/types_aiobotocore_athena/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     8681 2023-08-04 12:18:41.000000 types-aiobotocore-athena-2.5.2.post3/types_aiobotocore_athena/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 12:18:41.000000 types-aiobotocore-athena-2.5.2.post3/types_aiobotocore_athena/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    62716 2023-08-04 12:18:43.000000 types-aiobotocore-athena-2.5.2.post3/types_aiobotocore_athena/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    62627 2023-08-04 12:18:42.000000 types-aiobotocore-athena-2.5.2.post3/types_aiobotocore_athena/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-04 12:18:41.000000 types-aiobotocore-athena-2.5.2.post3/types_aiobotocore_athena/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:37:19.003228 types-aiobotocore-athena-2.5.2.post3/types_aiobotocore_athena.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    13797 2023-08-04 12:37:18.000000 types-aiobotocore-athena-2.5.2.post3/types_aiobotocore_athena.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      794 2023-08-04 12:37:18.000000 types-aiobotocore-athena-2.5.2.post3/types_aiobotocore_athena.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 12:37:18.000000 types-aiobotocore-athena-2.5.2.post3/types_aiobotocore_athena.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 12:37:18.000000 types-aiobotocore-athena-2.5.2.post3/types_aiobotocore_athena.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-04 12:37:18.000000 types-aiobotocore-athena-2.5.2.post3/types_aiobotocore_athena.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-08-04 12:37:18.000000 types-aiobotocore-athena-2.5.2.post3/types_aiobotocore_athena.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:23:19.938553 types-aiobotocore-athena-2.5.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-08 01:06:27.000000 types-aiobotocore-athena-2.5.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    13791 2023-08-08 01:23:19.926552 types-aiobotocore-athena-2.5.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    12283 2023-08-08 01:06:27.000000 types-aiobotocore-athena-2.5.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-08 01:23:19.938553 types-aiobotocore-athena-2.5.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2059 2023-08-08 01:06:27.000000 types-aiobotocore-athena-2.5.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:23:19.926552 types-aiobotocore-athena-2.5.4/types_aiobotocore_athena/
+-rw-r--r--   0 runner    (1001) docker     (123)     1919 2023-08-08 01:06:27.000000 types-aiobotocore-athena-2.5.4/types_aiobotocore_athena/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1918 2023-08-08 01:06:27.000000 types-aiobotocore-athena-2.5.4/types_aiobotocore_athena/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      916 2023-08-08 01:06:27.000000 types-aiobotocore-athena-2.5.4/types_aiobotocore_athena/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    48904 2023-08-08 01:06:28.000000 types-aiobotocore-athena-2.5.4/types_aiobotocore_athena/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    48820 2023-08-08 01:06:28.000000 types-aiobotocore-athena-2.5.4/types_aiobotocore_athena/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    10614 2023-08-08 01:06:28.000000 types-aiobotocore-athena-2.5.4/types_aiobotocore_athena/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10612 2023-08-08 01:06:28.000000 types-aiobotocore-athena-2.5.4/types_aiobotocore_athena/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8690 2023-08-08 01:06:28.000000 types-aiobotocore-athena-2.5.4/types_aiobotocore_athena/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8681 2023-08-08 01:06:28.000000 types-aiobotocore-athena-2.5.4/types_aiobotocore_athena/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 01:06:27.000000 types-aiobotocore-athena-2.5.4/types_aiobotocore_athena/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    62716 2023-08-08 01:06:29.000000 types-aiobotocore-athena-2.5.4/types_aiobotocore_athena/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    62627 2023-08-08 01:06:29.000000 types-aiobotocore-athena-2.5.4/types_aiobotocore_athena/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-08-08 01:06:27.000000 types-aiobotocore-athena-2.5.4/types_aiobotocore_athena/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:23:19.926552 types-aiobotocore-athena-2.5.4/types_aiobotocore_athena.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    13791 2023-08-08 01:23:19.000000 types-aiobotocore-athena-2.5.4/types_aiobotocore_athena.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      794 2023-08-08 01:23:19.000000 types-aiobotocore-athena-2.5.4/types_aiobotocore_athena.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 01:23:19.000000 types-aiobotocore-athena-2.5.4/types_aiobotocore_athena.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 01:23:19.000000 types-aiobotocore-athena-2.5.4/types_aiobotocore_athena.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-08 01:23:19.000000 types-aiobotocore-athena-2.5.4/types_aiobotocore_athena.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-08-08 01:23:19.000000 types-aiobotocore-athena-2.5.4/types_aiobotocore_athena.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-athena-2.5.2.post3/LICENSE` & `types-aiobotocore-athena-2.5.4/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-athena-2.5.2.post3/PKG-INFO` & `types-aiobotocore-athena-2.5.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-athena
-Version: 2.5.2.post3
-Summary: Type annotations for aiobotocore.Athena 2.5.2 service generated with mypy-boto3-builder 7.17.2
+Version: 2.5.4
+Summary: Type annotations for aiobotocore.Athena 2.5.4 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_athena/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-athena.svg?color=blue)](https://pypi.org/project/types-aiobotocore-athena)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_athena/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-athena)](https://pepy.tech/project/types-aiobotocore-athena)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.Athena 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/athena.html#Athena)
+[aiobotocore.Athena 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/athena.html#Athena)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-athena-2.5.2.post3/README.md` & `types-aiobotocore-athena-2.5.4/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-athena.svg?color=blue)](https://pypi.org/project/types-aiobotocore-athena)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_athena/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-athena)](https://pepy.tech/project/types-aiobotocore-athena)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.Athena 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/athena.html#Athena)
+[aiobotocore.Athena 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/athena.html#Athena)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-athena-2.5.2.post3/setup.py` & `types-aiobotocore-athena-2.5.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-athena",
-    version="2.5.2.post3",
+    version="2.5.4",
     packages=["types_aiobotocore_athena"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.Athena 2.5.2 service generated with mypy-boto3-builder"
+        "Type annotations for aiobotocore.Athena 2.5.4 service generated with mypy-boto3-builder"
         " 7.17.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
```

### Comparing `types-aiobotocore-athena-2.5.2.post3/types_aiobotocore_athena/__init__.py` & `types-aiobotocore-athena-2.5.4/types_aiobotocore_athena/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-athena-2.5.2.post3/types_aiobotocore_athena/__init__.pyi` & `types-aiobotocore-athena-2.5.4/types_aiobotocore_athena/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-athena-2.5.2.post3/types_aiobotocore_athena/__main__.py` & `types-aiobotocore-athena-2.5.4/types_aiobotocore_athena/__main__.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.Athena 2.5.2\nVersion:         2.5.2.post3\nBuilder"
-        " version: 7.17.2\nDocs:           "
+        "Type annotations for aiobotocore.Athena 2.5.4\nVersion:         2.5.4\nBuilder version:"
+        " 7.17.2\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_athena//\nBoto3 docs: "
         "     https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/athena.html#Athena\nOther"
         " services:  https://pypi.org/project/boto3-stubs/\nChangelog:      "
         " https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("2.5.2.post3")
+    print("2.5.4")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `types-aiobotocore-athena-2.5.2.post3/types_aiobotocore_athena/client.py` & `types-aiobotocore-athena-2.5.4/types_aiobotocore_athena/client.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-athena-2.5.2.post3/types_aiobotocore_athena/client.pyi` & `types-aiobotocore-athena-2.5.4/types_aiobotocore_athena/client.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-athena-2.5.2.post3/types_aiobotocore_athena/literals.py` & `types-aiobotocore-athena-2.5.4/types_aiobotocore_athena/literals.pyi`

 * *Files 3% similar despite different names*

```diff
@@ -14,15 +14,14 @@
 import sys
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = (
     "CalculationExecutionStateType",
     "CapacityAllocationStatusType",
     "CapacityReservationStatusType",
     "ColumnNullableType",
     "DataCatalogTypeType",
     "EncryptionOptionType",
@@ -44,15 +43,14 @@
     "AthenaServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "RegionName",
 )
 
-
 CalculationExecutionStateType = Literal[
     "CANCELED", "CANCELING", "COMPLETED", "CREATED", "CREATING", "FAILED", "QUEUED", "RUNNING"
 ]
 CapacityAllocationStatusType = Literal["FAILED", "PENDING", "SUCCEEDED"]
 CapacityReservationStatusType = Literal[
     "ACTIVE", "CANCELLED", "CANCELLING", "FAILED", "PENDING", "UPDATE_PENDING"
 ]
@@ -90,14 +88,15 @@
     "amplifybackend",
     "amplifyuibuilder",
     "apigateway",
     "apigatewaymanagementapi",
     "apigatewayv2",
     "appconfig",
     "appconfigdata",
+    "appfabric",
     "appflow",
     "appintegrations",
     "application-autoscaling",
     "application-insights",
     "applicationcostprofiler",
     "appmesh",
     "apprunner",
@@ -193,14 +192,15 @@
     "elasticbeanstalk",
     "elastictranscoder",
     "elb",
     "elbv2",
     "emr",
     "emr-containers",
     "emr-serverless",
+    "entityresolution",
     "es",
     "events",
     "evidently",
     "finspace",
     "finspace-data",
     "firehose",
     "fis",
@@ -279,26 +279,28 @@
     "lookoutmetrics",
     "lookoutvision",
     "m2",
     "machinelearning",
     "macie",
     "macie2",
     "managedblockchain",
+    "managedblockchain-query",
     "marketplace-catalog",
     "marketplace-entitlement",
     "marketplacecommerceanalytics",
     "mediaconnect",
     "mediaconvert",
     "medialive",
     "mediapackage",
     "mediapackage-vod",
     "mediapackagev2",
     "mediastore",
     "mediastore-data",
     "mediatailor",
+    "medical-imaging",
     "memorydb",
     "meteringmarketplace",
     "mgh",
     "mgn",
     "migration-hub-refactor-spaces",
     "migrationhub-config",
     "migrationhuborchestrator",
@@ -454,24 +456,29 @@
 RegionName = Literal[
     "af-south-1",
     "ap-east-1",
     "ap-northeast-1",
     "ap-northeast-2",
     "ap-northeast-3",
     "ap-south-1",
+    "ap-south-2",
     "ap-southeast-1",
     "ap-southeast-2",
     "ap-southeast-3",
+    "ap-southeast-4",
     "ca-central-1",
     "eu-central-1",
+    "eu-central-2",
     "eu-north-1",
     "eu-south-1",
+    "eu-south-2",
     "eu-west-1",
     "eu-west-2",
     "eu-west-3",
+    "me-central-1",
     "me-south-1",
     "sa-east-1",
     "us-east-1",
     "us-east-2",
     "us-west-1",
     "us-west-2",
 ]
```

### Comparing `types-aiobotocore-athena-2.5.2.post3/types_aiobotocore_athena/literals.pyi` & `types-aiobotocore-athena-2.5.4/types_aiobotocore_athena/literals.py`

 * *Files 7% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 import sys
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
+
 __all__ = (
     "CalculationExecutionStateType",
     "CapacityAllocationStatusType",
     "CapacityReservationStatusType",
     "ColumnNullableType",
     "DataCatalogTypeType",
     "EncryptionOptionType",
@@ -43,14 +44,15 @@
     "AthenaServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "RegionName",
 )
 
+
 CalculationExecutionStateType = Literal[
     "CANCELED", "CANCELING", "COMPLETED", "CREATED", "CREATING", "FAILED", "QUEUED", "RUNNING"
 ]
 CapacityAllocationStatusType = Literal["FAILED", "PENDING", "SUCCEEDED"]
 CapacityReservationStatusType = Literal[
     "ACTIVE", "CANCELLED", "CANCELLING", "FAILED", "PENDING", "UPDATE_PENDING"
 ]
@@ -88,14 +90,15 @@
     "amplifybackend",
     "amplifyuibuilder",
     "apigateway",
     "apigatewaymanagementapi",
     "apigatewayv2",
     "appconfig",
     "appconfigdata",
+    "appfabric",
     "appflow",
     "appintegrations",
     "application-autoscaling",
     "application-insights",
     "applicationcostprofiler",
     "appmesh",
     "apprunner",
@@ -191,14 +194,15 @@
     "elasticbeanstalk",
     "elastictranscoder",
     "elb",
     "elbv2",
     "emr",
     "emr-containers",
     "emr-serverless",
+    "entityresolution",
     "es",
     "events",
     "evidently",
     "finspace",
     "finspace-data",
     "firehose",
     "fis",
@@ -277,26 +281,28 @@
     "lookoutmetrics",
     "lookoutvision",
     "m2",
     "machinelearning",
     "macie",
     "macie2",
     "managedblockchain",
+    "managedblockchain-query",
     "marketplace-catalog",
     "marketplace-entitlement",
     "marketplacecommerceanalytics",
     "mediaconnect",
     "mediaconvert",
     "medialive",
     "mediapackage",
     "mediapackage-vod",
     "mediapackagev2",
     "mediastore",
     "mediastore-data",
     "mediatailor",
+    "medical-imaging",
     "memorydb",
     "meteringmarketplace",
     "mgh",
     "mgn",
     "migration-hub-refactor-spaces",
     "migrationhub-config",
     "migrationhuborchestrator",
@@ -452,24 +458,29 @@
 RegionName = Literal[
     "af-south-1",
     "ap-east-1",
     "ap-northeast-1",
     "ap-northeast-2",
     "ap-northeast-3",
     "ap-south-1",
+    "ap-south-2",
     "ap-southeast-1",
     "ap-southeast-2",
     "ap-southeast-3",
+    "ap-southeast-4",
     "ca-central-1",
     "eu-central-1",
+    "eu-central-2",
     "eu-north-1",
     "eu-south-1",
+    "eu-south-2",
     "eu-west-1",
     "eu-west-2",
     "eu-west-3",
+    "me-central-1",
     "me-south-1",
     "sa-east-1",
     "us-east-1",
     "us-east-2",
     "us-west-1",
     "us-west-2",
 ]
```

### Comparing `types-aiobotocore-athena-2.5.2.post3/types_aiobotocore_athena/paginator.py` & `types-aiobotocore-athena-2.5.4/types_aiobotocore_athena/paginator.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-athena-2.5.2.post3/types_aiobotocore_athena/paginator.pyi` & `types-aiobotocore-athena-2.5.4/types_aiobotocore_athena/paginator.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-athena-2.5.2.post3/types_aiobotocore_athena/type_defs.py` & `types-aiobotocore-athena-2.5.4/types_aiobotocore_athena/type_defs.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-athena-2.5.2.post3/types_aiobotocore_athena/type_defs.pyi` & `types-aiobotocore-athena-2.5.4/types_aiobotocore_athena/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-athena-2.5.2.post3/types_aiobotocore_athena.egg-info/PKG-INFO` & `types-aiobotocore-athena-2.5.4/types_aiobotocore_athena.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-athena
-Version: 2.5.2.post3
-Summary: Type annotations for aiobotocore.Athena 2.5.2 service generated with mypy-boto3-builder 7.17.2
+Version: 2.5.4
+Summary: Type annotations for aiobotocore.Athena 2.5.4 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_athena/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-athena.svg?color=blue)](https://pypi.org/project/types-aiobotocore-athena)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_athena/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-athena)](https://pepy.tech/project/types-aiobotocore-athena)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.Athena 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/athena.html#Athena)
+[aiobotocore.Athena 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/athena.html#Athena)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-athena-2.5.2.post3/types_aiobotocore_athena.egg-info/SOURCES.txt` & `types-aiobotocore-athena-2.5.4/types_aiobotocore_athena.egg-info/SOURCES.txt`

 * *Files identical despite different names*


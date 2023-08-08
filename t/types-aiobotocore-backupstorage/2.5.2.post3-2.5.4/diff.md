# Comparing `tmp/types-aiobotocore-backupstorage-2.5.2.post3.tar.gz` & `tmp/types-aiobotocore-backupstorage-2.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-backupstorage-2.5.2.post3.tar", last modified: Fri Aug  4 12:37:21 2023, max compression
+gzip compressed data, was "types-aiobotocore-backupstorage-2.5.4.tar", last modified: Tue Aug  8 01:23:21 2023, max compression
```

## Comparing `types-aiobotocore-backupstorage-2.5.2.post3.tar` & `types-aiobotocore-backupstorage-2.5.4.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:37:21.519280 types-aiobotocore-backupstorage-2.5.2.post3/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-04 12:18:56.000000 types-aiobotocore-backupstorage-2.5.2.post3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    12516 2023-08-04 12:37:21.515279 types-aiobotocore-backupstorage-2.5.2.post3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    10974 2023-08-04 12:18:56.000000 types-aiobotocore-backupstorage-2.5.2.post3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-04 12:37:21.519280 types-aiobotocore-backupstorage-2.5.2.post3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2114 2023-08-04 12:18:56.000000 types-aiobotocore-backupstorage-2.5.2.post3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:37:21.511279 types-aiobotocore-backupstorage-2.5.2.post3/types_aiobotocore_backupstorage/
--rw-r--r--   0 runner    (1001) docker     (123)      490 2023-08-04 12:18:56.000000 types-aiobotocore-backupstorage-2.5.2.post3/types_aiobotocore_backupstorage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      489 2023-08-04 12:18:56.000000 types-aiobotocore-backupstorage-2.5.2.post3/types_aiobotocore_backupstorage/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      967 2023-08-04 12:18:56.000000 types-aiobotocore-backupstorage-2.5.2.post3/types_aiobotocore_backupstorage/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10956 2023-08-04 12:18:57.000000 types-aiobotocore-backupstorage-2.5.2.post3/types_aiobotocore_backupstorage/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    10938 2023-08-04 12:18:56.000000 types-aiobotocore-backupstorage-2.5.2.post3/types_aiobotocore_backupstorage/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     7825 2023-08-04 12:18:57.000000 types-aiobotocore-backupstorage-2.5.2.post3/types_aiobotocore_backupstorage/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     7823 2023-08-04 12:18:57.000000 types-aiobotocore-backupstorage-2.5.2.post3/types_aiobotocore_backupstorage/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 12:18:56.000000 types-aiobotocore-backupstorage-2.5.2.post3/types_aiobotocore_backupstorage/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     8502 2023-08-04 12:18:57.000000 types-aiobotocore-backupstorage-2.5.2.post3/types_aiobotocore_backupstorage/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)     8490 2023-08-04 12:18:57.000000 types-aiobotocore-backupstorage-2.5.2.post3/types_aiobotocore_backupstorage/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-04 12:18:56.000000 types-aiobotocore-backupstorage-2.5.2.post3/types_aiobotocore_backupstorage/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:37:21.515279 types-aiobotocore-backupstorage-2.5.2.post3/types_aiobotocore_backupstorage.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    12516 2023-08-04 12:37:21.000000 types-aiobotocore-backupstorage-2.5.2.post3/types_aiobotocore_backupstorage.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      836 2023-08-04 12:37:21.000000 types-aiobotocore-backupstorage-2.5.2.post3/types_aiobotocore_backupstorage.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 12:37:21.000000 types-aiobotocore-backupstorage-2.5.2.post3/types_aiobotocore_backupstorage.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 12:37:21.000000 types-aiobotocore-backupstorage-2.5.2.post3/types_aiobotocore_backupstorage.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-04 12:37:21.000000 types-aiobotocore-backupstorage-2.5.2.post3/types_aiobotocore_backupstorage.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-08-04 12:37:21.000000 types-aiobotocore-backupstorage-2.5.2.post3/types_aiobotocore_backupstorage.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:23:21.706620 types-aiobotocore-backupstorage-2.5.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-08 01:06:42.000000 types-aiobotocore-backupstorage-2.5.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    12510 2023-08-08 01:23:21.706620 types-aiobotocore-backupstorage-2.5.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10974 2023-08-08 01:06:42.000000 types-aiobotocore-backupstorage-2.5.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-08 01:23:21.706620 types-aiobotocore-backupstorage-2.5.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2108 2023-08-08 01:06:42.000000 types-aiobotocore-backupstorage-2.5.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:23:21.706620 types-aiobotocore-backupstorage-2.5.4/types_aiobotocore_backupstorage/
+-rw-r--r--   0 runner    (1001) docker     (123)      490 2023-08-08 01:06:42.000000 types-aiobotocore-backupstorage-2.5.4/types_aiobotocore_backupstorage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      489 2023-08-08 01:06:42.000000 types-aiobotocore-backupstorage-2.5.4/types_aiobotocore_backupstorage/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      955 2023-08-08 01:06:42.000000 types-aiobotocore-backupstorage-2.5.4/types_aiobotocore_backupstorage/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10956 2023-08-08 01:06:42.000000 types-aiobotocore-backupstorage-2.5.4/types_aiobotocore_backupstorage/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10938 2023-08-08 01:06:42.000000 types-aiobotocore-backupstorage-2.5.4/types_aiobotocore_backupstorage/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8384 2023-08-08 01:06:42.000000 types-aiobotocore-backupstorage-2.5.4/types_aiobotocore_backupstorage/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8382 2023-08-08 01:06:42.000000 types-aiobotocore-backupstorage-2.5.4/types_aiobotocore_backupstorage/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 01:06:42.000000 types-aiobotocore-backupstorage-2.5.4/types_aiobotocore_backupstorage/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     8502 2023-08-08 01:06:42.000000 types-aiobotocore-backupstorage-2.5.4/types_aiobotocore_backupstorage/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8490 2023-08-08 01:06:42.000000 types-aiobotocore-backupstorage-2.5.4/types_aiobotocore_backupstorage/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-08-08 01:06:42.000000 types-aiobotocore-backupstorage-2.5.4/types_aiobotocore_backupstorage/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:23:21.706620 types-aiobotocore-backupstorage-2.5.4/types_aiobotocore_backupstorage.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    12510 2023-08-08 01:23:21.000000 types-aiobotocore-backupstorage-2.5.4/types_aiobotocore_backupstorage.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      836 2023-08-08 01:23:21.000000 types-aiobotocore-backupstorage-2.5.4/types_aiobotocore_backupstorage.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 01:23:21.000000 types-aiobotocore-backupstorage-2.5.4/types_aiobotocore_backupstorage.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 01:23:21.000000 types-aiobotocore-backupstorage-2.5.4/types_aiobotocore_backupstorage.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-08 01:23:21.000000 types-aiobotocore-backupstorage-2.5.4/types_aiobotocore_backupstorage.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-08-08 01:23:21.000000 types-aiobotocore-backupstorage-2.5.4/types_aiobotocore_backupstorage.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-backupstorage-2.5.2.post3/LICENSE` & `types-aiobotocore-backupstorage-2.5.4/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-backupstorage-2.5.2.post3/PKG-INFO` & `types-aiobotocore-backupstorage-2.5.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-backupstorage
-Version: 2.5.2.post3
-Summary: Type annotations for aiobotocore.BackupStorage 2.5.2 service generated with mypy-boto3-builder 7.17.2
+Version: 2.5.4
+Summary: Type annotations for aiobotocore.BackupStorage 2.5.4 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_backupstorage/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-backupstorage.svg?color=blue)](https://pypi.org/project/types-aiobotocore-backupstorage)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_backupstorage/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-backupstorage)](https://pepy.tech/project/types-aiobotocore-backupstorage)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.BackupStorage 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backupstorage.html#BackupStorage)
+[aiobotocore.BackupStorage 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backupstorage.html#BackupStorage)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-backupstorage-2.5.2.post3/README.md` & `types-aiobotocore-backupstorage-2.5.4/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-backupstorage.svg?color=blue)](https://pypi.org/project/types-aiobotocore-backupstorage)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_backupstorage/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-backupstorage)](https://pepy.tech/project/types-aiobotocore-backupstorage)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.BackupStorage 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backupstorage.html#BackupStorage)
+[aiobotocore.BackupStorage 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backupstorage.html#BackupStorage)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-backupstorage-2.5.2.post3/setup.py` & `types-aiobotocore-backupstorage-2.5.4/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-backupstorage",
-    version="2.5.2.post3",
+    version="2.5.4",
     packages=["types_aiobotocore_backupstorage"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.BackupStorage 2.5.2 service generated with"
+        "Type annotations for aiobotocore.BackupStorage 2.5.4 service generated with"
         " mypy-boto3-builder 7.17.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
```

### Comparing `types-aiobotocore-backupstorage-2.5.2.post3/types_aiobotocore_backupstorage/__main__.py` & `types-aiobotocore-backupstorage-2.5.4/types_aiobotocore_backupstorage/__main__.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.BackupStorage 2.5.2\nVersion:        "
-        " 2.5.2.post3\nBuilder version: 7.17.2\nDocs:           "
+        "Type annotations for aiobotocore.BackupStorage 2.5.4\nVersion:         2.5.4\nBuilder"
+        " version: 7.17.2\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_backupstorage//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backupstorage.html#BackupStorage\nOther"
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

### Comparing `types-aiobotocore-backupstorage-2.5.2.post3/types_aiobotocore_backupstorage/client.py` & `types-aiobotocore-backupstorage-2.5.4/types_aiobotocore_backupstorage/client.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-backupstorage-2.5.2.post3/types_aiobotocore_backupstorage/client.pyi` & `types-aiobotocore-backupstorage-2.5.4/types_aiobotocore_backupstorage/client.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-backupstorage-2.5.2.post3/types_aiobotocore_backupstorage/literals.py` & `types-aiobotocore-backupstorage-2.5.4/types_aiobotocore_backupstorage/literals.pyi`

 * *Files 6% similar despite different names*

```diff
@@ -14,25 +14,23 @@
 import sys
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = (
     "DataChecksumAlgorithmType",
     "SummaryChecksumAlgorithmType",
     "BackupStorageServiceName",
     "ServiceName",
     "ResourceServiceName",
     "RegionName",
 )
 
-
 DataChecksumAlgorithmType = Literal["SHA256"]
 SummaryChecksumAlgorithmType = Literal["SUMMARY"]
 BackupStorageServiceName = Literal["backupstorage"]
 ServiceName = Literal[
     "accessanalyzer",
     "account",
     "acm",
@@ -43,14 +41,15 @@
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
@@ -146,14 +145,15 @@
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
@@ -232,26 +232,28 @@
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
@@ -391,8 +393,36 @@
     "glacier",
     "iam",
     "opsworks",
     "s3",
     "sns",
     "sqs",
 ]
-RegionName = Literal["eu-west-1", "us-east-1", "us-east-2", "us-west-2"]
+RegionName = Literal[
+    "af-south-1",
+    "ap-east-1",
+    "ap-northeast-1",
+    "ap-northeast-2",
+    "ap-northeast-3",
+    "ap-south-1",
+    "ap-south-2",
+    "ap-southeast-1",
+    "ap-southeast-2",
+    "ap-southeast-3",
+    "ap-southeast-4",
+    "ca-central-1",
+    "eu-central-1",
+    "eu-central-2",
+    "eu-north-1",
+    "eu-south-1",
+    "eu-south-2",
+    "eu-west-1",
+    "eu-west-2",
+    "eu-west-3",
+    "me-central-1",
+    "me-south-1",
+    "sa-east-1",
+    "us-east-1",
+    "us-east-2",
+    "us-west-1",
+    "us-west-2",
+]
```

### Comparing `types-aiobotocore-backupstorage-2.5.2.post3/types_aiobotocore_backupstorage/literals.pyi` & `types-aiobotocore-backupstorage-2.5.4/types_aiobotocore_backupstorage/literals.py`

 * *Files 9% similar despite different names*

```diff
@@ -14,23 +14,25 @@
 import sys
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
+
 __all__ = (
     "DataChecksumAlgorithmType",
     "SummaryChecksumAlgorithmType",
     "BackupStorageServiceName",
     "ServiceName",
     "ResourceServiceName",
     "RegionName",
 )
 
+
 DataChecksumAlgorithmType = Literal["SHA256"]
 SummaryChecksumAlgorithmType = Literal["SUMMARY"]
 BackupStorageServiceName = Literal["backupstorage"]
 ServiceName = Literal[
     "accessanalyzer",
     "account",
     "acm",
@@ -41,14 +43,15 @@
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
@@ -144,14 +147,15 @@
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
@@ -230,26 +234,28 @@
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
@@ -389,8 +395,36 @@
     "glacier",
     "iam",
     "opsworks",
     "s3",
     "sns",
     "sqs",
 ]
-RegionName = Literal["eu-west-1", "us-east-1", "us-east-2", "us-west-2"]
+RegionName = Literal[
+    "af-south-1",
+    "ap-east-1",
+    "ap-northeast-1",
+    "ap-northeast-2",
+    "ap-northeast-3",
+    "ap-south-1",
+    "ap-south-2",
+    "ap-southeast-1",
+    "ap-southeast-2",
+    "ap-southeast-3",
+    "ap-southeast-4",
+    "ca-central-1",
+    "eu-central-1",
+    "eu-central-2",
+    "eu-north-1",
+    "eu-south-1",
+    "eu-south-2",
+    "eu-west-1",
+    "eu-west-2",
+    "eu-west-3",
+    "me-central-1",
+    "me-south-1",
+    "sa-east-1",
+    "us-east-1",
+    "us-east-2",
+    "us-west-1",
+    "us-west-2",
+]
```

### Comparing `types-aiobotocore-backupstorage-2.5.2.post3/types_aiobotocore_backupstorage/type_defs.py` & `types-aiobotocore-backupstorage-2.5.4/types_aiobotocore_backupstorage/type_defs.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-backupstorage-2.5.2.post3/types_aiobotocore_backupstorage/type_defs.pyi` & `types-aiobotocore-backupstorage-2.5.4/types_aiobotocore_backupstorage/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-backupstorage-2.5.2.post3/types_aiobotocore_backupstorage.egg-info/PKG-INFO` & `types-aiobotocore-backupstorage-2.5.4/types_aiobotocore_backupstorage.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-backupstorage
-Version: 2.5.2.post3
-Summary: Type annotations for aiobotocore.BackupStorage 2.5.2 service generated with mypy-boto3-builder 7.17.2
+Version: 2.5.4
+Summary: Type annotations for aiobotocore.BackupStorage 2.5.4 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_backupstorage/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-backupstorage.svg?color=blue)](https://pypi.org/project/types-aiobotocore-backupstorage)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_backupstorage/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-backupstorage)](https://pepy.tech/project/types-aiobotocore-backupstorage)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.BackupStorage 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backupstorage.html#BackupStorage)
+[aiobotocore.BackupStorage 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backupstorage.html#BackupStorage)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-backupstorage-2.5.2.post3/types_aiobotocore_backupstorage.egg-info/SOURCES.txt` & `types-aiobotocore-backupstorage-2.5.4/types_aiobotocore_backupstorage.egg-info/SOURCES.txt`

 * *Files identical despite different names*


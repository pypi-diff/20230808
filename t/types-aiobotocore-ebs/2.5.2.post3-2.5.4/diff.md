# Comparing `tmp/types-aiobotocore-ebs-2.5.2.post3.tar.gz` & `tmp/types-aiobotocore-ebs-2.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-ebs-2.5.2.post3.tar", last modified: Fri Aug  4 12:37:38 2023, max compression
+gzip compressed data, was "types-aiobotocore-ebs-2.5.4.tar", last modified: Tue Aug  8 01:23:38 2023, max compression
```

## Comparing `types-aiobotocore-ebs-2.5.2.post3.tar` & `types-aiobotocore-ebs-2.5.4.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:37:38.899698 types-aiobotocore-ebs-2.5.2.post3/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-04 12:21:58.000000 types-aiobotocore-ebs-2.5.2.post3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    11976 2023-08-04 12:37:38.899698 types-aiobotocore-ebs-2.5.2.post3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    10474 2023-08-04 12:21:58.000000 types-aiobotocore-ebs-2.5.2.post3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-04 12:37:38.899698 types-aiobotocore-ebs-2.5.2.post3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2020 2023-08-04 12:21:58.000000 types-aiobotocore-ebs-2.5.2.post3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:37:38.895698 types-aiobotocore-ebs-2.5.2.post3/types_aiobotocore_ebs/
--rw-r--r--   0 runner    (1001) docker     (123)      410 2023-08-04 12:21:58.000000 types-aiobotocore-ebs-2.5.2.post3/types_aiobotocore_ebs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      409 2023-08-04 12:21:58.000000 types-aiobotocore-ebs-2.5.2.post3/types_aiobotocore_ebs/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      916 2023-08-04 12:21:58.000000 types-aiobotocore-ebs-2.5.2.post3/types_aiobotocore_ebs/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8555 2023-08-04 12:21:58.000000 types-aiobotocore-ebs-2.5.2.post3/types_aiobotocore_ebs/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     8540 2023-08-04 12:21:58.000000 types-aiobotocore-ebs-2.5.2.post3/types_aiobotocore_ebs/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8302 2023-08-04 12:21:58.000000 types-aiobotocore-ebs-2.5.2.post3/types_aiobotocore_ebs/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     8300 2023-08-04 12:21:58.000000 types-aiobotocore-ebs-2.5.2.post3/types_aiobotocore_ebs/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 12:21:58.000000 types-aiobotocore-ebs-2.5.2.post3/types_aiobotocore_ebs/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     7079 2023-08-04 12:21:58.000000 types-aiobotocore-ebs-2.5.2.post3/types_aiobotocore_ebs/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)     7068 2023-08-04 12:21:58.000000 types-aiobotocore-ebs-2.5.2.post3/types_aiobotocore_ebs/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-04 12:21:58.000000 types-aiobotocore-ebs-2.5.2.post3/types_aiobotocore_ebs/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:37:38.895698 types-aiobotocore-ebs-2.5.2.post3/types_aiobotocore_ebs.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    11976 2023-08-04 12:37:38.000000 types-aiobotocore-ebs-2.5.2.post3/types_aiobotocore_ebs.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      666 2023-08-04 12:37:38.000000 types-aiobotocore-ebs-2.5.2.post3/types_aiobotocore_ebs.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 12:37:38.000000 types-aiobotocore-ebs-2.5.2.post3/types_aiobotocore_ebs.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 12:37:38.000000 types-aiobotocore-ebs-2.5.2.post3/types_aiobotocore_ebs.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-04 12:37:38.000000 types-aiobotocore-ebs-2.5.2.post3/types_aiobotocore_ebs.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-08-04 12:37:38.000000 types-aiobotocore-ebs-2.5.2.post3/types_aiobotocore_ebs.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:23:38.518694 types-aiobotocore-ebs-2.5.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-08 01:09:32.000000 types-aiobotocore-ebs-2.5.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    11970 2023-08-08 01:23:38.514694 types-aiobotocore-ebs-2.5.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10474 2023-08-08 01:09:32.000000 types-aiobotocore-ebs-2.5.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-08 01:23:38.518694 types-aiobotocore-ebs-2.5.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2014 2023-08-08 01:09:32.000000 types-aiobotocore-ebs-2.5.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:23:38.506694 types-aiobotocore-ebs-2.5.4/types_aiobotocore_ebs/
+-rw-r--r--   0 runner    (1001) docker     (123)      410 2023-08-08 01:09:32.000000 types-aiobotocore-ebs-2.5.4/types_aiobotocore_ebs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      409 2023-08-08 01:09:32.000000 types-aiobotocore-ebs-2.5.4/types_aiobotocore_ebs/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      904 2023-08-08 01:09:32.000000 types-aiobotocore-ebs-2.5.4/types_aiobotocore_ebs/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8555 2023-08-08 01:09:32.000000 types-aiobotocore-ebs-2.5.4/types_aiobotocore_ebs/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8540 2023-08-08 01:09:32.000000 types-aiobotocore-ebs-2.5.4/types_aiobotocore_ebs/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8488 2023-08-08 01:09:32.000000 types-aiobotocore-ebs-2.5.4/types_aiobotocore_ebs/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8486 2023-08-08 01:09:32.000000 types-aiobotocore-ebs-2.5.4/types_aiobotocore_ebs/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 01:09:32.000000 types-aiobotocore-ebs-2.5.4/types_aiobotocore_ebs/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     7124 2023-08-08 01:09:32.000000 types-aiobotocore-ebs-2.5.4/types_aiobotocore_ebs/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7113 2023-08-08 01:09:32.000000 types-aiobotocore-ebs-2.5.4/types_aiobotocore_ebs/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-08-08 01:09:32.000000 types-aiobotocore-ebs-2.5.4/types_aiobotocore_ebs/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:23:38.514694 types-aiobotocore-ebs-2.5.4/types_aiobotocore_ebs.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    11970 2023-08-08 01:23:38.000000 types-aiobotocore-ebs-2.5.4/types_aiobotocore_ebs.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      666 2023-08-08 01:23:38.000000 types-aiobotocore-ebs-2.5.4/types_aiobotocore_ebs.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 01:23:38.000000 types-aiobotocore-ebs-2.5.4/types_aiobotocore_ebs.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 01:23:38.000000 types-aiobotocore-ebs-2.5.4/types_aiobotocore_ebs.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-08 01:23:38.000000 types-aiobotocore-ebs-2.5.4/types_aiobotocore_ebs.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-08-08 01:23:38.000000 types-aiobotocore-ebs-2.5.4/types_aiobotocore_ebs.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-ebs-2.5.2.post3/LICENSE` & `types-aiobotocore-ebs-2.5.4/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-ebs-2.5.2.post3/PKG-INFO` & `types-aiobotocore-ebs-2.5.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-ebs
-Version: 2.5.2.post3
-Summary: Type annotations for aiobotocore.EBS 2.5.2 service generated with mypy-boto3-builder 7.17.2
+Version: 2.5.4
+Summary: Type annotations for aiobotocore.EBS 2.5.4 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ebs/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-ebs.svg?color=blue)](https://pypi.org/project/types-aiobotocore-ebs)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ebs/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-ebs)](https://pepy.tech/project/types-aiobotocore-ebs)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.EBS 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ebs.html#EBS)
+[aiobotocore.EBS 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ebs.html#EBS)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-ebs-2.5.2.post3/README.md` & `types-aiobotocore-ebs-2.5.4/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-ebs.svg?color=blue)](https://pypi.org/project/types-aiobotocore-ebs)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ebs/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-ebs)](https://pepy.tech/project/types-aiobotocore-ebs)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.EBS 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ebs.html#EBS)
+[aiobotocore.EBS 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ebs.html#EBS)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-ebs-2.5.2.post3/setup.py` & `types-aiobotocore-ebs-2.5.4/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-ebs",
-    version="2.5.2.post3",
+    version="2.5.4",
     packages=["types_aiobotocore_ebs"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.EBS 2.5.2 service generated with mypy-boto3-builder"
+        "Type annotations for aiobotocore.EBS 2.5.4 service generated with mypy-boto3-builder"
         " 7.17.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
```

### Comparing `types-aiobotocore-ebs-2.5.2.post3/types_aiobotocore_ebs/__main__.py` & `types-aiobotocore-ebs-2.5.4/types_aiobotocore_ebs/__main__.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.EBS 2.5.2\nVersion:         2.5.2.post3\nBuilder version:"
+        "Type annotations for aiobotocore.EBS 2.5.4\nVersion:         2.5.4\nBuilder version:"
         " 7.17.2\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ebs//\nBoto3 docs:    "
         "  https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ebs.html#EBS\nOther"
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

### Comparing `types-aiobotocore-ebs-2.5.2.post3/types_aiobotocore_ebs/client.py` & `types-aiobotocore-ebs-2.5.4/types_aiobotocore_ebs/client.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-ebs-2.5.2.post3/types_aiobotocore_ebs/client.pyi` & `types-aiobotocore-ebs-2.5.4/types_aiobotocore_ebs/client.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-ebs-2.5.2.post3/types_aiobotocore_ebs/literals.py` & `types-aiobotocore-ebs-2.5.4/types_aiobotocore_ebs/literals.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -14,28 +14,28 @@
 import sys
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = (
     "ChecksumAggregationMethodType",
     "ChecksumAlgorithmType",
+    "SSETypeType",
     "StatusType",
     "EBSServiceName",
     "ServiceName",
     "ResourceServiceName",
     "RegionName",
 )
 
-
 ChecksumAggregationMethodType = Literal["LINEAR"]
 ChecksumAlgorithmType = Literal["SHA256"]
+SSETypeType = Literal["none", "sse-ebs", "sse-kms"]
 StatusType = Literal["completed", "error", "pending"]
 EBSServiceName = Literal["ebs"]
 ServiceName = Literal[
     "accessanalyzer",
     "account",
     "acm",
     "acm-pca",
@@ -45,14 +45,15 @@
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
@@ -148,14 +149,15 @@
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
@@ -234,26 +236,28 @@
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
@@ -414,14 +418,15 @@
     "eu-central-2",
     "eu-north-1",
     "eu-south-1",
     "eu-south-2",
     "eu-west-1",
     "eu-west-2",
     "eu-west-3",
+    "il-central-1",
     "me-central-1",
     "me-south-1",
     "sa-east-1",
     "us-east-1",
     "us-east-2",
     "us-west-1",
     "us-west-2",
```

### Comparing `types-aiobotocore-ebs-2.5.2.post3/types_aiobotocore_ebs/literals.pyi` & `types-aiobotocore-ebs-2.5.4/types_aiobotocore_ebs/literals.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,26 +14,30 @@
 import sys
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
+
 __all__ = (
     "ChecksumAggregationMethodType",
     "ChecksumAlgorithmType",
+    "SSETypeType",
     "StatusType",
     "EBSServiceName",
     "ServiceName",
     "ResourceServiceName",
     "RegionName",
 )
 
+
 ChecksumAggregationMethodType = Literal["LINEAR"]
 ChecksumAlgorithmType = Literal["SHA256"]
+SSETypeType = Literal["none", "sse-ebs", "sse-kms"]
 StatusType = Literal["completed", "error", "pending"]
 EBSServiceName = Literal["ebs"]
 ServiceName = Literal[
     "accessanalyzer",
     "account",
     "acm",
     "acm-pca",
@@ -43,14 +47,15 @@
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
@@ -146,14 +151,15 @@
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
@@ -232,26 +238,28 @@
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
@@ -412,14 +420,15 @@
     "eu-central-2",
     "eu-north-1",
     "eu-south-1",
     "eu-south-2",
     "eu-west-1",
     "eu-west-2",
     "eu-west-3",
+    "il-central-1",
     "me-central-1",
     "me-south-1",
     "sa-east-1",
     "us-east-1",
     "us-east-2",
     "us-west-1",
     "us-west-2",
```

### Comparing `types-aiobotocore-ebs-2.5.2.post3/types_aiobotocore_ebs/type_defs.py` & `types-aiobotocore-ebs-2.5.4/types_aiobotocore_ebs/type_defs.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 """
 import sys
 from datetime import datetime
 from typing import IO, Any, Dict, List, Sequence, Union
 
 from aiobotocore.response import StreamingBody
 
-from .literals import StatusType
+from .literals import SSETypeType, StatusType
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
@@ -284,10 +284,11 @@
         "Status": StatusType,
         "StartTime": datetime,
         "VolumeSize": int,
         "BlockSize": int,
         "Tags": List[TagTypeDef],
         "ParentSnapshotId": str,
         "KmsKeyArn": str,
+        "SseType": SSETypeType,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `types-aiobotocore-ebs-2.5.2.post3/types_aiobotocore_ebs/type_defs.pyi` & `types-aiobotocore-ebs-2.5.4/types_aiobotocore_ebs/type_defs.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 """
 import sys
 from datetime import datetime
 from typing import IO, Any, Dict, List, Sequence, Union
 
 from aiobotocore.response import StreamingBody
 
-from .literals import StatusType
+from .literals import SSETypeType, StatusType
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
@@ -273,10 +273,11 @@
         "Status": StatusType,
         "StartTime": datetime,
         "VolumeSize": int,
         "BlockSize": int,
         "Tags": List[TagTypeDef],
         "ParentSnapshotId": str,
         "KmsKeyArn": str,
+        "SseType": SSETypeType,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `types-aiobotocore-ebs-2.5.2.post3/types_aiobotocore_ebs.egg-info/PKG-INFO` & `types-aiobotocore-ebs-2.5.4/types_aiobotocore_ebs.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-ebs
-Version: 2.5.2.post3
-Summary: Type annotations for aiobotocore.EBS 2.5.2 service generated with mypy-boto3-builder 7.17.2
+Version: 2.5.4
+Summary: Type annotations for aiobotocore.EBS 2.5.4 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ebs/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-ebs.svg?color=blue)](https://pypi.org/project/types-aiobotocore-ebs)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ebs/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-ebs)](https://pepy.tech/project/types-aiobotocore-ebs)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.EBS 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ebs.html#EBS)
+[aiobotocore.EBS 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ebs.html#EBS)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-ebs-2.5.2.post3/types_aiobotocore_ebs.egg-info/SOURCES.txt` & `types-aiobotocore-ebs-2.5.4/types_aiobotocore_ebs.egg-info/SOURCES.txt`

 * *Files identical despite different names*


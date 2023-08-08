# Comparing `tmp/types-aiobotocore-cognito-sync-2.5.2.post3.tar.gz` & `tmp/types-aiobotocore-cognito-sync-2.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-cognito-sync-2.5.2.post3.tar", last modified: Fri Aug  4 12:37:31 2023, max compression
+gzip compressed data, was "types-aiobotocore-cognito-sync-2.5.4.tar", last modified: Tue Aug  8 01:23:31 2023, max compression
```

## Comparing `types-aiobotocore-cognito-sync-2.5.2.post3.tar` & `types-aiobotocore-cognito-sync-2.5.4.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:37:31.359517 types-aiobotocore-cognito-sync-2.5.2.post3/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-04 12:20:31.000000 types-aiobotocore-cognito-sync-2.5.2.post3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    12472 2023-08-04 12:37:31.359517 types-aiobotocore-cognito-sync-2.5.2.post3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    10935 2023-08-04 12:20:31.000000 types-aiobotocore-cognito-sync-2.5.2.post3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-04 12:37:31.359517 types-aiobotocore-cognito-sync-2.5.2.post3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2106 2023-08-04 12:20:30.000000 types-aiobotocore-cognito-sync-2.5.2.post3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:37:31.351517 types-aiobotocore-cognito-sync-2.5.2.post3/types_aiobotocore_cognito_sync/
--rw-r--r--   0 runner    (1001) docker     (123)      477 2023-08-04 12:20:31.000000 types-aiobotocore-cognito-sync-2.5.2.post3/types_aiobotocore_cognito_sync/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      476 2023-08-04 12:20:31.000000 types-aiobotocore-cognito-sync-2.5.2.post3/types_aiobotocore_cognito_sync/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      961 2023-08-04 12:20:31.000000 types-aiobotocore-cognito-sync-2.5.2.post3/types_aiobotocore_cognito_sync/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15515 2023-08-04 12:20:31.000000 types-aiobotocore-cognito-sync-2.5.2.post3/types_aiobotocore_cognito_sync/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    15490 2023-08-04 12:20:31.000000 types-aiobotocore-cognito-sync-2.5.2.post3/types_aiobotocore_cognito_sync/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8147 2023-08-04 12:20:31.000000 types-aiobotocore-cognito-sync-2.5.2.post3/types_aiobotocore_cognito_sync/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     8145 2023-08-04 12:20:31.000000 types-aiobotocore-cognito-sync-2.5.2.post3/types_aiobotocore_cognito_sync/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 12:20:31.000000 types-aiobotocore-cognito-sync-2.5.2.post3/types_aiobotocore_cognito_sync/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    12818 2023-08-04 12:20:31.000000 types-aiobotocore-cognito-sync-2.5.2.post3/types_aiobotocore_cognito_sync/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    12808 2023-08-04 12:20:31.000000 types-aiobotocore-cognito-sync-2.5.2.post3/types_aiobotocore_cognito_sync/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-04 12:20:31.000000 types-aiobotocore-cognito-sync-2.5.2.post3/types_aiobotocore_cognito_sync/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:37:31.359517 types-aiobotocore-cognito-sync-2.5.2.post3/types_aiobotocore_cognito_sync.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    12472 2023-08-04 12:37:31.000000 types-aiobotocore-cognito-sync-2.5.2.post3/types_aiobotocore_cognito_sync.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      819 2023-08-04 12:37:31.000000 types-aiobotocore-cognito-sync-2.5.2.post3/types_aiobotocore_cognito_sync.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 12:37:31.000000 types-aiobotocore-cognito-sync-2.5.2.post3/types_aiobotocore_cognito_sync.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 12:37:31.000000 types-aiobotocore-cognito-sync-2.5.2.post3/types_aiobotocore_cognito_sync.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-04 12:37:31.000000 types-aiobotocore-cognito-sync-2.5.2.post3/types_aiobotocore_cognito_sync.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-08-04 12:37:31.000000 types-aiobotocore-cognito-sync-2.5.2.post3/types_aiobotocore_cognito_sync.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:23:31.294668 types-aiobotocore-cognito-sync-2.5.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-08 01:08:09.000000 types-aiobotocore-cognito-sync-2.5.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    12466 2023-08-08 01:23:31.294668 types-aiobotocore-cognito-sync-2.5.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10935 2023-08-08 01:08:09.000000 types-aiobotocore-cognito-sync-2.5.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-08 01:23:31.294668 types-aiobotocore-cognito-sync-2.5.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2100 2023-08-08 01:08:09.000000 types-aiobotocore-cognito-sync-2.5.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:23:31.290668 types-aiobotocore-cognito-sync-2.5.4/types_aiobotocore_cognito_sync/
+-rw-r--r--   0 runner    (1001) docker     (123)      477 2023-08-08 01:08:09.000000 types-aiobotocore-cognito-sync-2.5.4/types_aiobotocore_cognito_sync/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      476 2023-08-08 01:08:09.000000 types-aiobotocore-cognito-sync-2.5.4/types_aiobotocore_cognito_sync/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      949 2023-08-08 01:08:09.000000 types-aiobotocore-cognito-sync-2.5.4/types_aiobotocore_cognito_sync/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15515 2023-08-08 01:08:10.000000 types-aiobotocore-cognito-sync-2.5.4/types_aiobotocore_cognito_sync/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15490 2023-08-08 01:08:09.000000 types-aiobotocore-cognito-sync-2.5.4/types_aiobotocore_cognito_sync/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8242 2023-08-08 01:08:10.000000 types-aiobotocore-cognito-sync-2.5.4/types_aiobotocore_cognito_sync/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8240 2023-08-08 01:08:10.000000 types-aiobotocore-cognito-sync-2.5.4/types_aiobotocore_cognito_sync/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 01:08:09.000000 types-aiobotocore-cognito-sync-2.5.4/types_aiobotocore_cognito_sync/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    12818 2023-08-08 01:08:10.000000 types-aiobotocore-cognito-sync-2.5.4/types_aiobotocore_cognito_sync/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12808 2023-08-08 01:08:10.000000 types-aiobotocore-cognito-sync-2.5.4/types_aiobotocore_cognito_sync/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-08-08 01:08:09.000000 types-aiobotocore-cognito-sync-2.5.4/types_aiobotocore_cognito_sync/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:23:31.294668 types-aiobotocore-cognito-sync-2.5.4/types_aiobotocore_cognito_sync.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    12466 2023-08-08 01:23:31.000000 types-aiobotocore-cognito-sync-2.5.4/types_aiobotocore_cognito_sync.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      819 2023-08-08 01:23:31.000000 types-aiobotocore-cognito-sync-2.5.4/types_aiobotocore_cognito_sync.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 01:23:31.000000 types-aiobotocore-cognito-sync-2.5.4/types_aiobotocore_cognito_sync.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 01:23:31.000000 types-aiobotocore-cognito-sync-2.5.4/types_aiobotocore_cognito_sync.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-08 01:23:31.000000 types-aiobotocore-cognito-sync-2.5.4/types_aiobotocore_cognito_sync.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-08-08 01:23:31.000000 types-aiobotocore-cognito-sync-2.5.4/types_aiobotocore_cognito_sync.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-cognito-sync-2.5.2.post3/LICENSE` & `types-aiobotocore-cognito-sync-2.5.4/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-cognito-sync-2.5.2.post3/PKG-INFO` & `types-aiobotocore-cognito-sync-2.5.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-cognito-sync
-Version: 2.5.2.post3
-Summary: Type annotations for aiobotocore.CognitoSync 2.5.2 service generated with mypy-boto3-builder 7.17.2
+Version: 2.5.4
+Summary: Type annotations for aiobotocore.CognitoSync 2.5.4 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cognito_sync/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-cognito-sync.svg?color=blue)](https://pypi.org/project/types-aiobotocore-cognito-sync)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cognito_sync/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-cognito-sync)](https://pepy.tech/project/types-aiobotocore-cognito-sync)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.CognitoSync 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-sync.html#CognitoSync)
+[aiobotocore.CognitoSync 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-sync.html#CognitoSync)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-cognito-sync-2.5.2.post3/README.md` & `types-aiobotocore-cognito-sync-2.5.4/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-cognito-sync.svg?color=blue)](https://pypi.org/project/types-aiobotocore-cognito-sync)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cognito_sync/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-cognito-sync)](https://pepy.tech/project/types-aiobotocore-cognito-sync)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.CognitoSync 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-sync.html#CognitoSync)
+[aiobotocore.CognitoSync 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-sync.html#CognitoSync)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-cognito-sync-2.5.2.post3/setup.py` & `types-aiobotocore-cognito-sync-2.5.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-cognito-sync",
-    version="2.5.2.post3",
+    version="2.5.4",
     packages=["types_aiobotocore_cognito_sync"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.CognitoSync 2.5.2 service generated with"
+        "Type annotations for aiobotocore.CognitoSync 2.5.4 service generated with"
         " mypy-boto3-builder 7.17.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
```

### Comparing `types-aiobotocore-cognito-sync-2.5.2.post3/types_aiobotocore_cognito_sync/__main__.py` & `types-aiobotocore-cognito-sync-2.5.4/types_aiobotocore_cognito_sync/__main__.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.CognitoSync 2.5.2\nVersion:         2.5.2.post3\nBuilder"
+        "Type annotations for aiobotocore.CognitoSync 2.5.4\nVersion:         2.5.4\nBuilder"
         " version: 7.17.2\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cognito_sync//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-sync.html#CognitoSync\nOther"
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

### Comparing `types-aiobotocore-cognito-sync-2.5.2.post3/types_aiobotocore_cognito_sync/client.py` & `types-aiobotocore-cognito-sync-2.5.4/types_aiobotocore_cognito_sync/client.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-cognito-sync-2.5.2.post3/types_aiobotocore_cognito_sync/client.pyi` & `types-aiobotocore-cognito-sync-2.5.4/types_aiobotocore_cognito_sync/client.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-cognito-sync-2.5.2.post3/types_aiobotocore_cognito_sync/literals.py` & `types-aiobotocore-cognito-sync-2.5.4/types_aiobotocore_cognito_sync/literals.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -14,27 +14,25 @@
 import sys
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = (
     "BulkPublishStatusType",
     "OperationType",
     "PlatformType",
     "StreamingStatusType",
     "CognitoSyncServiceName",
     "ServiceName",
     "ResourceServiceName",
     "RegionName",
 )
 
-
 BulkPublishStatusType = Literal["FAILED", "IN_PROGRESS", "NOT_STARTED", "SUCCEEDED"]
 OperationType = Literal["remove", "replace"]
 PlatformType = Literal["ADM", "APNS", "APNS_SANDBOX", "GCM"]
 StreamingStatusType = Literal["DISABLED", "ENABLED"]
 CognitoSyncServiceName = Literal["cognito-sync"]
 ServiceName = Literal[
     "accessanalyzer",
@@ -47,14 +45,15 @@
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
@@ -150,14 +149,15 @@
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
@@ -236,26 +236,28 @@
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
```

### Comparing `types-aiobotocore-cognito-sync-2.5.2.post3/types_aiobotocore_cognito_sync/literals.pyi` & `types-aiobotocore-cognito-sync-2.5.4/types_aiobotocore_cognito_sync/literals.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,25 +14,27 @@
 import sys
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
+
 __all__ = (
     "BulkPublishStatusType",
     "OperationType",
     "PlatformType",
     "StreamingStatusType",
     "CognitoSyncServiceName",
     "ServiceName",
     "ResourceServiceName",
     "RegionName",
 )
 
+
 BulkPublishStatusType = Literal["FAILED", "IN_PROGRESS", "NOT_STARTED", "SUCCEEDED"]
 OperationType = Literal["remove", "replace"]
 PlatformType = Literal["ADM", "APNS", "APNS_SANDBOX", "GCM"]
 StreamingStatusType = Literal["DISABLED", "ENABLED"]
 CognitoSyncServiceName = Literal["cognito-sync"]
 ServiceName = Literal[
     "accessanalyzer",
@@ -45,14 +47,15 @@
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
@@ -148,14 +151,15 @@
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
@@ -234,26 +238,28 @@
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
```

### Comparing `types-aiobotocore-cognito-sync-2.5.2.post3/types_aiobotocore_cognito_sync/type_defs.py` & `types-aiobotocore-cognito-sync-2.5.4/types_aiobotocore_cognito_sync/type_defs.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-cognito-sync-2.5.2.post3/types_aiobotocore_cognito_sync/type_defs.pyi` & `types-aiobotocore-cognito-sync-2.5.4/types_aiobotocore_cognito_sync/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-cognito-sync-2.5.2.post3/types_aiobotocore_cognito_sync.egg-info/PKG-INFO` & `types-aiobotocore-cognito-sync-2.5.4/types_aiobotocore_cognito_sync.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-cognito-sync
-Version: 2.5.2.post3
-Summary: Type annotations for aiobotocore.CognitoSync 2.5.2 service generated with mypy-boto3-builder 7.17.2
+Version: 2.5.4
+Summary: Type annotations for aiobotocore.CognitoSync 2.5.4 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cognito_sync/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-cognito-sync.svg?color=blue)](https://pypi.org/project/types-aiobotocore-cognito-sync)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cognito_sync/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-cognito-sync)](https://pepy.tech/project/types-aiobotocore-cognito-sync)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.CognitoSync 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-sync.html#CognitoSync)
+[aiobotocore.CognitoSync 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-sync.html#CognitoSync)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-cognito-sync-2.5.2.post3/types_aiobotocore_cognito_sync.egg-info/SOURCES.txt` & `types-aiobotocore-cognito-sync-2.5.4/types_aiobotocore_cognito_sync.egg-info/SOURCES.txt`

 * *Files identical despite different names*


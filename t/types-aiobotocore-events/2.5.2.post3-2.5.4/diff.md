# Comparing `tmp/types-aiobotocore-events-2.5.2.post3.tar.gz` & `tmp/types-aiobotocore-events-2.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-events-2.5.2.post3.tar", last modified: Fri Aug  4 12:37:42 2023, max compression
+gzip compressed data, was "types-aiobotocore-events-2.5.4.tar", last modified: Tue Aug  8 01:23:43 2023, max compression
```

## Comparing `types-aiobotocore-events-2.5.2.post3.tar` & `types-aiobotocore-events-2.5.4.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:37:42.951793 types-aiobotocore-events-2.5.2.post3/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-04 12:23:37.000000 types-aiobotocore-events-2.5.2.post3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    13272 2023-08-04 12:37:42.951793 types-aiobotocore-events-2.5.2.post3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    11753 2023-08-04 12:23:37.000000 types-aiobotocore-events-2.5.2.post3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-04 12:37:42.951793 types-aiobotocore-events-2.5.2.post3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2070 2023-08-04 12:23:37.000000 types-aiobotocore-events-2.5.2.post3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:37:42.951793 types-aiobotocore-events-2.5.2.post3/types_aiobotocore_events/
--rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-08-04 12:23:37.000000 types-aiobotocore-events-2.5.2.post3/types_aiobotocore_events/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1107 2023-08-04 12:23:37.000000 types-aiobotocore-events-2.5.2.post3/types_aiobotocore_events/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      938 2023-08-04 12:23:37.000000 types-aiobotocore-events-2.5.2.post3/types_aiobotocore_events/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    40210 2023-08-04 12:23:37.000000 types-aiobotocore-events-2.5.2.post3/types_aiobotocore_events/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    40142 2023-08-04 12:23:37.000000 types-aiobotocore-events-2.5.2.post3/types_aiobotocore_events/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    10206 2023-08-04 12:23:37.000000 types-aiobotocore-events-2.5.2.post3/types_aiobotocore_events/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    10204 2023-08-04 12:23:37.000000 types-aiobotocore-events-2.5.2.post3/types_aiobotocore_events/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     4373 2023-08-04 12:23:37.000000 types-aiobotocore-events-2.5.2.post3/types_aiobotocore_events/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     4368 2023-08-04 12:23:37.000000 types-aiobotocore-events-2.5.2.post3/types_aiobotocore_events/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 12:23:37.000000 types-aiobotocore-events-2.5.2.post3/types_aiobotocore_events/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    59024 2023-08-04 12:23:39.000000 types-aiobotocore-events-2.5.2.post3/types_aiobotocore_events/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    58955 2023-08-04 12:23:38.000000 types-aiobotocore-events-2.5.2.post3/types_aiobotocore_events/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-04 12:23:37.000000 types-aiobotocore-events-2.5.2.post3/types_aiobotocore_events/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:37:42.951793 types-aiobotocore-events-2.5.2.post3/types_aiobotocore_events.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    13272 2023-08-04 12:37:42.000000 types-aiobotocore-events-2.5.2.post3/types_aiobotocore_events.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      794 2023-08-04 12:37:42.000000 types-aiobotocore-events-2.5.2.post3/types_aiobotocore_events.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 12:37:42.000000 types-aiobotocore-events-2.5.2.post3/types_aiobotocore_events.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 12:37:42.000000 types-aiobotocore-events-2.5.2.post3/types_aiobotocore_events.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-04 12:37:42.000000 types-aiobotocore-events-2.5.2.post3/types_aiobotocore_events.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-08-04 12:37:42.000000 types-aiobotocore-events-2.5.2.post3/types_aiobotocore_events.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:23:43.330714 types-aiobotocore-events-2.5.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-08 01:11:02.000000 types-aiobotocore-events-2.5.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    13266 2023-08-08 01:23:43.330714 types-aiobotocore-events-2.5.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    11753 2023-08-08 01:11:02.000000 types-aiobotocore-events-2.5.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-08 01:23:43.330714 types-aiobotocore-events-2.5.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2064 2023-08-08 01:11:02.000000 types-aiobotocore-events-2.5.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:23:43.330714 types-aiobotocore-events-2.5.4/types_aiobotocore_events/
+-rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-08-08 01:11:02.000000 types-aiobotocore-events-2.5.4/types_aiobotocore_events/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1107 2023-08-08 01:11:02.000000 types-aiobotocore-events-2.5.4/types_aiobotocore_events/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      926 2023-08-08 01:11:02.000000 types-aiobotocore-events-2.5.4/types_aiobotocore_events/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40210 2023-08-08 01:11:03.000000 types-aiobotocore-events-2.5.4/types_aiobotocore_events/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40142 2023-08-08 01:11:03.000000 types-aiobotocore-events-2.5.4/types_aiobotocore_events/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    10321 2023-08-08 01:11:03.000000 types-aiobotocore-events-2.5.4/types_aiobotocore_events/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10319 2023-08-08 01:11:03.000000 types-aiobotocore-events-2.5.4/types_aiobotocore_events/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     4373 2023-08-08 01:11:03.000000 types-aiobotocore-events-2.5.4/types_aiobotocore_events/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4368 2023-08-08 01:11:03.000000 types-aiobotocore-events-2.5.4/types_aiobotocore_events/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 01:11:02.000000 types-aiobotocore-events-2.5.4/types_aiobotocore_events/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    59024 2023-08-08 01:11:04.000000 types-aiobotocore-events-2.5.4/types_aiobotocore_events/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    58955 2023-08-08 01:11:04.000000 types-aiobotocore-events-2.5.4/types_aiobotocore_events/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-08-08 01:11:02.000000 types-aiobotocore-events-2.5.4/types_aiobotocore_events/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:23:43.330714 types-aiobotocore-events-2.5.4/types_aiobotocore_events.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    13266 2023-08-08 01:23:43.000000 types-aiobotocore-events-2.5.4/types_aiobotocore_events.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      794 2023-08-08 01:23:43.000000 types-aiobotocore-events-2.5.4/types_aiobotocore_events.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 01:23:43.000000 types-aiobotocore-events-2.5.4/types_aiobotocore_events.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 01:23:43.000000 types-aiobotocore-events-2.5.4/types_aiobotocore_events.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-08 01:23:43.000000 types-aiobotocore-events-2.5.4/types_aiobotocore_events.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-08-08 01:23:43.000000 types-aiobotocore-events-2.5.4/types_aiobotocore_events.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-events-2.5.2.post3/LICENSE` & `types-aiobotocore-events-2.5.4/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-events-2.5.2.post3/PKG-INFO` & `types-aiobotocore-events-2.5.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-events
-Version: 2.5.2.post3
-Summary: Type annotations for aiobotocore.EventBridge 2.5.2 service generated with mypy-boto3-builder 7.17.2
+Version: 2.5.4
+Summary: Type annotations for aiobotocore.EventBridge 2.5.4 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_events/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-events.svg?color=blue)](https://pypi.org/project/types-aiobotocore-events)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_events/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-events)](https://pepy.tech/project/types-aiobotocore-events)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.EventBridge 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/events.html#EventBridge)
+[aiobotocore.EventBridge 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/events.html#EventBridge)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-events-2.5.2.post3/README.md` & `types-aiobotocore-events-2.5.4/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-events.svg?color=blue)](https://pypi.org/project/types-aiobotocore-events)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_events/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-events)](https://pepy.tech/project/types-aiobotocore-events)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.EventBridge 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/events.html#EventBridge)
+[aiobotocore.EventBridge 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/events.html#EventBridge)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-events-2.5.2.post3/setup.py` & `types-aiobotocore-events-2.5.4/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-events",
-    version="2.5.2.post3",
+    version="2.5.4",
     packages=["types_aiobotocore_events"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.EventBridge 2.5.2 service generated with"
+        "Type annotations for aiobotocore.EventBridge 2.5.4 service generated with"
         " mypy-boto3-builder 7.17.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
```

### Comparing `types-aiobotocore-events-2.5.2.post3/types_aiobotocore_events/__init__.py` & `types-aiobotocore-events-2.5.4/types_aiobotocore_events/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-events-2.5.2.post3/types_aiobotocore_events/__init__.pyi` & `types-aiobotocore-events-2.5.4/types_aiobotocore_events/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-events-2.5.2.post3/types_aiobotocore_events/__main__.py` & `types-aiobotocore-events-2.5.4/types_aiobotocore_events/__main__.py`

 * *Files 13% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.EventBridge 2.5.2\nVersion:         2.5.2.post3\nBuilder"
+        "Type annotations for aiobotocore.EventBridge 2.5.4\nVersion:         2.5.4\nBuilder"
         " version: 7.17.2\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_events//\nBoto3 docs: "
         "     https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/events.html#EventBridge\nOther"
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

### Comparing `types-aiobotocore-events-2.5.2.post3/types_aiobotocore_events/client.py` & `types-aiobotocore-events-2.5.4/types_aiobotocore_events/client.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-events-2.5.2.post3/types_aiobotocore_events/client.pyi` & `types-aiobotocore-events-2.5.4/types_aiobotocore_events/client.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-events-2.5.2.post3/types_aiobotocore_events/literals.py` & `types-aiobotocore-events-2.5.4/types_aiobotocore_events/literals.pyi`

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
     "ApiDestinationHttpMethodType",
     "ApiDestinationStateType",
     "ArchiveStateType",
     "AssignPublicIpType",
     "ConnectionAuthorizationTypeType",
     "ConnectionOAuthHttpMethodType",
@@ -42,15 +41,14 @@
     "EventBridgeServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "RegionName",
 )
 
-
 ApiDestinationHttpMethodType = Literal["DELETE", "GET", "HEAD", "OPTIONS", "PATCH", "POST", "PUT"]
 ApiDestinationStateType = Literal["ACTIVE", "INACTIVE"]
 ArchiveStateType = Literal[
     "CREATE_FAILED", "CREATING", "DISABLED", "ENABLED", "UPDATE_FAILED", "UPDATING"
 ]
 AssignPublicIpType = Literal["DISABLED", "ENABLED"]
 ConnectionAuthorizationTypeType = Literal["API_KEY", "BASIC", "OAUTH_CLIENT_CREDENTIALS"]
@@ -84,14 +82,15 @@
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
@@ -187,14 +186,15 @@
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
@@ -273,26 +273,28 @@
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
@@ -454,14 +456,15 @@
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

### Comparing `types-aiobotocore-events-2.5.2.post3/types_aiobotocore_events/literals.pyi` & `types-aiobotocore-events-2.5.4/types_aiobotocore_events/literals.py`

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
     "ApiDestinationHttpMethodType",
     "ApiDestinationStateType",
     "ArchiveStateType",
     "AssignPublicIpType",
     "ConnectionAuthorizationTypeType",
     "ConnectionOAuthHttpMethodType",
@@ -41,14 +42,15 @@
     "EventBridgeServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "RegionName",
 )
 
+
 ApiDestinationHttpMethodType = Literal["DELETE", "GET", "HEAD", "OPTIONS", "PATCH", "POST", "PUT"]
 ApiDestinationStateType = Literal["ACTIVE", "INACTIVE"]
 ArchiveStateType = Literal[
     "CREATE_FAILED", "CREATING", "DISABLED", "ENABLED", "UPDATE_FAILED", "UPDATING"
 ]
 AssignPublicIpType = Literal["DISABLED", "ENABLED"]
 ConnectionAuthorizationTypeType = Literal["API_KEY", "BASIC", "OAUTH_CLIENT_CREDENTIALS"]
@@ -82,14 +84,15 @@
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
@@ -185,14 +188,15 @@
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
@@ -271,26 +275,28 @@
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
@@ -452,14 +458,15 @@
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

### Comparing `types-aiobotocore-events-2.5.2.post3/types_aiobotocore_events/paginator.py` & `types-aiobotocore-events-2.5.4/types_aiobotocore_events/paginator.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-events-2.5.2.post3/types_aiobotocore_events/paginator.pyi` & `types-aiobotocore-events-2.5.4/types_aiobotocore_events/paginator.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-events-2.5.2.post3/types_aiobotocore_events/type_defs.py` & `types-aiobotocore-events-2.5.4/types_aiobotocore_events/type_defs.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-events-2.5.2.post3/types_aiobotocore_events/type_defs.pyi` & `types-aiobotocore-events-2.5.4/types_aiobotocore_events/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-events-2.5.2.post3/types_aiobotocore_events.egg-info/PKG-INFO` & `types-aiobotocore-events-2.5.4/types_aiobotocore_events.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-events
-Version: 2.5.2.post3
-Summary: Type annotations for aiobotocore.EventBridge 2.5.2 service generated with mypy-boto3-builder 7.17.2
+Version: 2.5.4
+Summary: Type annotations for aiobotocore.EventBridge 2.5.4 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_events/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-events.svg?color=blue)](https://pypi.org/project/types-aiobotocore-events)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_events/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-events)](https://pepy.tech/project/types-aiobotocore-events)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.EventBridge 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/events.html#EventBridge)
+[aiobotocore.EventBridge 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/events.html#EventBridge)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-events-2.5.2.post3/types_aiobotocore_events.egg-info/SOURCES.txt` & `types-aiobotocore-events-2.5.4/types_aiobotocore_events.egg-info/SOURCES.txt`

 * *Files identical despite different names*


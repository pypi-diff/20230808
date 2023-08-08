# Comparing `tmp/types-aiobotocore-appconfig-2.5.2.post3.tar.gz` & `tmp/types-aiobotocore-appconfig-2.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-appconfig-2.5.2.post3.tar", last modified: Fri Aug  4 12:37:16 2023, max compression
+gzip compressed data, was "types-aiobotocore-appconfig-2.5.4.tar", last modified: Tue Aug  8 01:23:14 2023, max compression
```

## Comparing `types-aiobotocore-appconfig-2.5.2.post3.tar` & `types-aiobotocore-appconfig-2.5.4.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:37:16.315167 types-aiobotocore-appconfig-2.5.2.post3/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-04 12:18:16.000000 types-aiobotocore-appconfig-2.5.2.post3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    12292 2023-08-04 12:37:16.307166 types-aiobotocore-appconfig-2.5.2.post3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    10766 2023-08-04 12:18:16.000000 types-aiobotocore-appconfig-2.5.2.post3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-04 12:37:16.315167 types-aiobotocore-appconfig-2.5.2.post3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2086 2023-08-04 12:18:16.000000 types-aiobotocore-appconfig-2.5.2.post3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:37:16.303166 types-aiobotocore-appconfig-2.5.2.post3/types_aiobotocore_appconfig/
--rw-r--r--   0 runner    (1001) docker     (123)      458 2023-08-04 12:18:16.000000 types-aiobotocore-appconfig-2.5.2.post3/types_aiobotocore_appconfig/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      457 2023-08-04 12:18:16.000000 types-aiobotocore-appconfig-2.5.2.post3/types_aiobotocore_appconfig/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      951 2023-08-04 12:18:16.000000 types-aiobotocore-appconfig-2.5.2.post3/types_aiobotocore_appconfig/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    30927 2023-08-04 12:18:16.000000 types-aiobotocore-appconfig-2.5.2.post3/types_aiobotocore_appconfig/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    30876 2023-08-04 12:18:16.000000 types-aiobotocore-appconfig-2.5.2.post3/types_aiobotocore_appconfig/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9189 2023-08-04 12:18:16.000000 types-aiobotocore-appconfig-2.5.2.post3/types_aiobotocore_appconfig/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     9187 2023-08-04 12:18:16.000000 types-aiobotocore-appconfig-2.5.2.post3/types_aiobotocore_appconfig/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 12:18:16.000000 types-aiobotocore-appconfig-2.5.2.post3/types_aiobotocore_appconfig/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    31152 2023-08-04 12:18:18.000000 types-aiobotocore-appconfig-2.5.2.post3/types_aiobotocore_appconfig/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    31107 2023-08-04 12:18:17.000000 types-aiobotocore-appconfig-2.5.2.post3/types_aiobotocore_appconfig/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-04 12:18:16.000000 types-aiobotocore-appconfig-2.5.2.post3/types_aiobotocore_appconfig/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:37:16.307166 types-aiobotocore-appconfig-2.5.2.post3/types_aiobotocore_appconfig.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    12292 2023-08-04 12:37:16.000000 types-aiobotocore-appconfig-2.5.2.post3/types_aiobotocore_appconfig.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      768 2023-08-04 12:37:16.000000 types-aiobotocore-appconfig-2.5.2.post3/types_aiobotocore_appconfig.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 12:37:16.000000 types-aiobotocore-appconfig-2.5.2.post3/types_aiobotocore_appconfig.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 12:37:16.000000 types-aiobotocore-appconfig-2.5.2.post3/types_aiobotocore_appconfig.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-04 12:37:16.000000 types-aiobotocore-appconfig-2.5.2.post3/types_aiobotocore_appconfig.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-08-04 12:37:16.000000 types-aiobotocore-appconfig-2.5.2.post3/types_aiobotocore_appconfig.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:23:14.594491 types-aiobotocore-appconfig-2.5.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-08 01:06:02.000000 types-aiobotocore-appconfig-2.5.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    12286 2023-08-08 01:23:14.590491 types-aiobotocore-appconfig-2.5.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10766 2023-08-08 01:06:02.000000 types-aiobotocore-appconfig-2.5.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-08 01:23:14.594491 types-aiobotocore-appconfig-2.5.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2080 2023-08-08 01:06:02.000000 types-aiobotocore-appconfig-2.5.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:23:14.590491 types-aiobotocore-appconfig-2.5.4/types_aiobotocore_appconfig/
+-rw-r--r--   0 runner    (1001) docker     (123)      458 2023-08-08 01:06:02.000000 types-aiobotocore-appconfig-2.5.4/types_aiobotocore_appconfig/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      457 2023-08-08 01:06:02.000000 types-aiobotocore-appconfig-2.5.4/types_aiobotocore_appconfig/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      939 2023-08-08 01:06:02.000000 types-aiobotocore-appconfig-2.5.4/types_aiobotocore_appconfig/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30927 2023-08-08 01:06:03.000000 types-aiobotocore-appconfig-2.5.4/types_aiobotocore_appconfig/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30876 2023-08-08 01:06:02.000000 types-aiobotocore-appconfig-2.5.4/types_aiobotocore_appconfig/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9304 2023-08-08 01:06:03.000000 types-aiobotocore-appconfig-2.5.4/types_aiobotocore_appconfig/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9302 2023-08-08 01:06:03.000000 types-aiobotocore-appconfig-2.5.4/types_aiobotocore_appconfig/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 01:06:02.000000 types-aiobotocore-appconfig-2.5.4/types_aiobotocore_appconfig/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    31152 2023-08-08 01:06:04.000000 types-aiobotocore-appconfig-2.5.4/types_aiobotocore_appconfig/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31107 2023-08-08 01:06:04.000000 types-aiobotocore-appconfig-2.5.4/types_aiobotocore_appconfig/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-08-08 01:06:02.000000 types-aiobotocore-appconfig-2.5.4/types_aiobotocore_appconfig/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:23:14.590491 types-aiobotocore-appconfig-2.5.4/types_aiobotocore_appconfig.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    12286 2023-08-08 01:23:14.000000 types-aiobotocore-appconfig-2.5.4/types_aiobotocore_appconfig.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      768 2023-08-08 01:23:14.000000 types-aiobotocore-appconfig-2.5.4/types_aiobotocore_appconfig.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 01:23:14.000000 types-aiobotocore-appconfig-2.5.4/types_aiobotocore_appconfig.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 01:23:14.000000 types-aiobotocore-appconfig-2.5.4/types_aiobotocore_appconfig.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-08 01:23:14.000000 types-aiobotocore-appconfig-2.5.4/types_aiobotocore_appconfig.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-08-08 01:23:14.000000 types-aiobotocore-appconfig-2.5.4/types_aiobotocore_appconfig.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-appconfig-2.5.2.post3/LICENSE` & `types-aiobotocore-appconfig-2.5.4/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-appconfig-2.5.2.post3/PKG-INFO` & `types-aiobotocore-appconfig-2.5.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-appconfig
-Version: 2.5.2.post3
-Summary: Type annotations for aiobotocore.AppConfig 2.5.2 service generated with mypy-boto3-builder 7.17.2
+Version: 2.5.4
+Summary: Type annotations for aiobotocore.AppConfig 2.5.4 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appconfig/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-appconfig.svg?color=blue)](https://pypi.org/project/types-aiobotocore-appconfig)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appconfig/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-appconfig)](https://pepy.tech/project/types-aiobotocore-appconfig)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.AppConfig 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appconfig.html#AppConfig)
+[aiobotocore.AppConfig 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appconfig.html#AppConfig)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-appconfig-2.5.2.post3/README.md` & `types-aiobotocore-appconfig-2.5.4/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-appconfig.svg?color=blue)](https://pypi.org/project/types-aiobotocore-appconfig)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appconfig/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-appconfig)](https://pepy.tech/project/types-aiobotocore-appconfig)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.AppConfig 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appconfig.html#AppConfig)
+[aiobotocore.AppConfig 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appconfig.html#AppConfig)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-appconfig-2.5.2.post3/setup.py` & `types-aiobotocore-appconfig-2.5.4/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-appconfig",
-    version="2.5.2.post3",
+    version="2.5.4",
     packages=["types_aiobotocore_appconfig"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.AppConfig 2.5.2 service generated with mypy-boto3-builder"
+        "Type annotations for aiobotocore.AppConfig 2.5.4 service generated with mypy-boto3-builder"
         " 7.17.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
```

### Comparing `types-aiobotocore-appconfig-2.5.2.post3/types_aiobotocore_appconfig/__main__.py` & `types-aiobotocore-appconfig-2.5.4/types_aiobotocore_appconfig/__main__.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.AppConfig 2.5.2\nVersion:         2.5.2.post3\nBuilder"
-        " version: 7.17.2\nDocs:           "
+        "Type annotations for aiobotocore.AppConfig 2.5.4\nVersion:         2.5.4\nBuilder version:"
+        " 7.17.2\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appconfig//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appconfig.html#AppConfig\nOther"
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

### Comparing `types-aiobotocore-appconfig-2.5.2.post3/types_aiobotocore_appconfig/client.py` & `types-aiobotocore-appconfig-2.5.4/types_aiobotocore_appconfig/client.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-appconfig-2.5.2.post3/types_aiobotocore_appconfig/client.pyi` & `types-aiobotocore-appconfig-2.5.4/types_aiobotocore_appconfig/client.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-appconfig-2.5.2.post3/types_aiobotocore_appconfig/literals.py` & `types-aiobotocore-appconfig-2.5.4/types_aiobotocore_appconfig/literals.pyi`

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
     "ActionPointType",
     "DeploymentEventTypeType",
     "DeploymentStateType",
     "EnvironmentStateType",
     "GrowthTypeType",
     "ReplicateToType",
@@ -30,15 +29,14 @@
     "ValidatorTypeType",
     "AppConfigServiceName",
     "ServiceName",
     "ResourceServiceName",
     "RegionName",
 )
 
-
 ActionPointType = Literal[
     "ON_DEPLOYMENT_BAKING",
     "ON_DEPLOYMENT_COMPLETE",
     "ON_DEPLOYMENT_ROLLED_BACK",
     "ON_DEPLOYMENT_START",
     "ON_DEPLOYMENT_STEP",
     "PRE_CREATE_HOSTED_CONFIGURATION_VERSION",
@@ -72,14 +70,15 @@
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
@@ -175,14 +174,15 @@
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
@@ -261,26 +261,28 @@
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
@@ -441,14 +443,15 @@
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

### Comparing `types-aiobotocore-appconfig-2.5.2.post3/types_aiobotocore_appconfig/literals.pyi` & `types-aiobotocore-appconfig-2.5.4/types_aiobotocore_appconfig/literals.py`

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
     "ActionPointType",
     "DeploymentEventTypeType",
     "DeploymentStateType",
     "EnvironmentStateType",
     "GrowthTypeType",
     "ReplicateToType",
@@ -29,14 +30,15 @@
     "ValidatorTypeType",
     "AppConfigServiceName",
     "ServiceName",
     "ResourceServiceName",
     "RegionName",
 )
 
+
 ActionPointType = Literal[
     "ON_DEPLOYMENT_BAKING",
     "ON_DEPLOYMENT_COMPLETE",
     "ON_DEPLOYMENT_ROLLED_BACK",
     "ON_DEPLOYMENT_START",
     "ON_DEPLOYMENT_STEP",
     "PRE_CREATE_HOSTED_CONFIGURATION_VERSION",
@@ -70,14 +72,15 @@
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
@@ -173,14 +176,15 @@
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
@@ -259,26 +263,28 @@
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
@@ -439,14 +445,15 @@
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

### Comparing `types-aiobotocore-appconfig-2.5.2.post3/types_aiobotocore_appconfig/type_defs.py` & `types-aiobotocore-appconfig-2.5.4/types_aiobotocore_appconfig/type_defs.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-appconfig-2.5.2.post3/types_aiobotocore_appconfig/type_defs.pyi` & `types-aiobotocore-appconfig-2.5.4/types_aiobotocore_appconfig/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-appconfig-2.5.2.post3/types_aiobotocore_appconfig.egg-info/PKG-INFO` & `types-aiobotocore-appconfig-2.5.4/types_aiobotocore_appconfig.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-appconfig
-Version: 2.5.2.post3
-Summary: Type annotations for aiobotocore.AppConfig 2.5.2 service generated with mypy-boto3-builder 7.17.2
+Version: 2.5.4
+Summary: Type annotations for aiobotocore.AppConfig 2.5.4 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appconfig/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-appconfig.svg?color=blue)](https://pypi.org/project/types-aiobotocore-appconfig)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appconfig/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-appconfig)](https://pepy.tech/project/types-aiobotocore-appconfig)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.AppConfig 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appconfig.html#AppConfig)
+[aiobotocore.AppConfig 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appconfig.html#AppConfig)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-appconfig-2.5.2.post3/types_aiobotocore_appconfig.egg-info/SOURCES.txt` & `types-aiobotocore-appconfig-2.5.4/types_aiobotocore_appconfig.egg-info/SOURCES.txt`

 * *Files identical despite different names*


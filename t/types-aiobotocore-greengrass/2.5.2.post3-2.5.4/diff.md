# Comparing `tmp/types-aiobotocore-greengrass-2.5.2.post3.tar.gz` & `tmp/types-aiobotocore-greengrass-2.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-greengrass-2.5.2.post3.tar", last modified: Fri Aug  4 12:37:46 2023, max compression
+gzip compressed data, was "types-aiobotocore-greengrass-2.5.4.tar", last modified: Tue Aug  8 01:23:47 2023, max compression
```

## Comparing `types-aiobotocore-greengrass-2.5.2.post3.tar` & `types-aiobotocore-greengrass-2.5.4.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:37:46.967887 types-aiobotocore-greengrass-2.5.2.post3/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-04 12:24:39.000000 types-aiobotocore-greengrass-2.5.2.post3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    16485 2023-08-04 12:37:46.967887 types-aiobotocore-greengrass-2.5.2.post3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    14955 2023-08-04 12:24:39.000000 types-aiobotocore-greengrass-2.5.2.post3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-04 12:37:46.967887 types-aiobotocore-greengrass-2.5.2.post3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2093 2023-08-04 12:24:39.000000 types-aiobotocore-greengrass-2.5.2.post3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:37:46.951887 types-aiobotocore-greengrass-2.5.2.post3/types_aiobotocore_greengrass/
--rw-r--r--   0 runner    (1001) docker     (123)     5325 2023-08-04 12:24:39.000000 types-aiobotocore-greengrass-2.5.2.post3/types_aiobotocore_greengrass/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5324 2023-08-04 12:24:39.000000 types-aiobotocore-greengrass-2.5.2.post3/types_aiobotocore_greengrass/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      955 2023-08-04 12:24:39.000000 types-aiobotocore-greengrass-2.5.2.post3/types_aiobotocore_greengrass/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    72384 2023-08-04 12:24:40.000000 types-aiobotocore-greengrass-2.5.2.post3/types_aiobotocore_greengrass/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    72264 2023-08-04 12:24:40.000000 types-aiobotocore-greengrass-2.5.2.post3/types_aiobotocore_greengrass/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    12283 2023-08-04 12:24:40.000000 types-aiobotocore-greengrass-2.5.2.post3/types_aiobotocore_greengrass/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    12281 2023-08-04 12:24:40.000000 types-aiobotocore-greengrass-2.5.2.post3/types_aiobotocore_greengrass/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    24010 2023-08-04 12:24:40.000000 types-aiobotocore-greengrass-2.5.2.post3/types_aiobotocore_greengrass/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)    23989 2023-08-04 12:24:40.000000 types-aiobotocore-greengrass-2.5.2.post3/types_aiobotocore_greengrass/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 12:24:39.000000 types-aiobotocore-greengrass-2.5.2.post3/types_aiobotocore_greengrass/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    88853 2023-08-04 12:24:42.000000 types-aiobotocore-greengrass-2.5.2.post3/types_aiobotocore_greengrass/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    88736 2023-08-04 12:24:41.000000 types-aiobotocore-greengrass-2.5.2.post3/types_aiobotocore_greengrass/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-04 12:24:39.000000 types-aiobotocore-greengrass-2.5.2.post3/types_aiobotocore_greengrass/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:37:46.967887 types-aiobotocore-greengrass-2.5.2.post3/types_aiobotocore_greengrass.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    16485 2023-08-04 12:37:46.000000 types-aiobotocore-greengrass-2.5.2.post3/types_aiobotocore_greengrass.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      870 2023-08-04 12:37:46.000000 types-aiobotocore-greengrass-2.5.2.post3/types_aiobotocore_greengrass.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 12:37:46.000000 types-aiobotocore-greengrass-2.5.2.post3/types_aiobotocore_greengrass.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 12:37:46.000000 types-aiobotocore-greengrass-2.5.2.post3/types_aiobotocore_greengrass.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-04 12:37:46.000000 types-aiobotocore-greengrass-2.5.2.post3/types_aiobotocore_greengrass.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-08-04 12:37:46.000000 types-aiobotocore-greengrass-2.5.2.post3/types_aiobotocore_greengrass.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:23:47.694726 types-aiobotocore-greengrass-2.5.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-08 01:11:59.000000 types-aiobotocore-greengrass-2.5.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    16479 2023-08-08 01:23:47.690726 types-aiobotocore-greengrass-2.5.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    14955 2023-08-08 01:11:59.000000 types-aiobotocore-greengrass-2.5.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-08 01:23:47.694726 types-aiobotocore-greengrass-2.5.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2087 2023-08-08 01:11:59.000000 types-aiobotocore-greengrass-2.5.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:23:47.686726 types-aiobotocore-greengrass-2.5.4/types_aiobotocore_greengrass/
+-rw-r--r--   0 runner    (1001) docker     (123)     5325 2023-08-08 01:11:59.000000 types-aiobotocore-greengrass-2.5.4/types_aiobotocore_greengrass/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5324 2023-08-08 01:11:59.000000 types-aiobotocore-greengrass-2.5.4/types_aiobotocore_greengrass/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      943 2023-08-08 01:11:59.000000 types-aiobotocore-greengrass-2.5.4/types_aiobotocore_greengrass/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    72384 2023-08-08 01:11:59.000000 types-aiobotocore-greengrass-2.5.4/types_aiobotocore_greengrass/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    72264 2023-08-08 01:11:59.000000 types-aiobotocore-greengrass-2.5.4/types_aiobotocore_greengrass/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    12378 2023-08-08 01:12:00.000000 types-aiobotocore-greengrass-2.5.4/types_aiobotocore_greengrass/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12376 2023-08-08 01:12:00.000000 types-aiobotocore-greengrass-2.5.4/types_aiobotocore_greengrass/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    24010 2023-08-08 01:12:00.000000 types-aiobotocore-greengrass-2.5.4/types_aiobotocore_greengrass/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23989 2023-08-08 01:12:00.000000 types-aiobotocore-greengrass-2.5.4/types_aiobotocore_greengrass/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 01:11:59.000000 types-aiobotocore-greengrass-2.5.4/types_aiobotocore_greengrass/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    88853 2023-08-08 01:12:01.000000 types-aiobotocore-greengrass-2.5.4/types_aiobotocore_greengrass/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    88736 2023-08-08 01:12:01.000000 types-aiobotocore-greengrass-2.5.4/types_aiobotocore_greengrass/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-08-08 01:11:59.000000 types-aiobotocore-greengrass-2.5.4/types_aiobotocore_greengrass/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:23:47.690726 types-aiobotocore-greengrass-2.5.4/types_aiobotocore_greengrass.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    16479 2023-08-08 01:23:47.000000 types-aiobotocore-greengrass-2.5.4/types_aiobotocore_greengrass.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      870 2023-08-08 01:23:47.000000 types-aiobotocore-greengrass-2.5.4/types_aiobotocore_greengrass.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 01:23:47.000000 types-aiobotocore-greengrass-2.5.4/types_aiobotocore_greengrass.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 01:23:47.000000 types-aiobotocore-greengrass-2.5.4/types_aiobotocore_greengrass.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-08 01:23:47.000000 types-aiobotocore-greengrass-2.5.4/types_aiobotocore_greengrass.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-08-08 01:23:47.000000 types-aiobotocore-greengrass-2.5.4/types_aiobotocore_greengrass.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-greengrass-2.5.2.post3/LICENSE` & `types-aiobotocore-greengrass-2.5.4/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-greengrass-2.5.2.post3/PKG-INFO` & `types-aiobotocore-greengrass-2.5.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-greengrass
-Version: 2.5.2.post3
-Summary: Type annotations for aiobotocore.Greengrass 2.5.2 service generated with mypy-boto3-builder 7.17.2
+Version: 2.5.4
+Summary: Type annotations for aiobotocore.Greengrass 2.5.4 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_greengrass/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-greengrass.svg?color=blue)](https://pypi.org/project/types-aiobotocore-greengrass)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_greengrass/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-greengrass)](https://pepy.tech/project/types-aiobotocore-greengrass)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.Greengrass 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/greengrass.html#Greengrass)
+[aiobotocore.Greengrass 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/greengrass.html#Greengrass)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-greengrass-2.5.2.post3/README.md` & `types-aiobotocore-greengrass-2.5.4/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-greengrass.svg?color=blue)](https://pypi.org/project/types-aiobotocore-greengrass)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_greengrass/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-greengrass)](https://pepy.tech/project/types-aiobotocore-greengrass)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.Greengrass 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/greengrass.html#Greengrass)
+[aiobotocore.Greengrass 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/greengrass.html#Greengrass)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-greengrass-2.5.2.post3/setup.py` & `types-aiobotocore-greengrass-2.5.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-greengrass",
-    version="2.5.2.post3",
+    version="2.5.4",
     packages=["types_aiobotocore_greengrass"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.Greengrass 2.5.2 service generated with"
+        "Type annotations for aiobotocore.Greengrass 2.5.4 service generated with"
         " mypy-boto3-builder 7.17.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
```

### Comparing `types-aiobotocore-greengrass-2.5.2.post3/types_aiobotocore_greengrass/__init__.py` & `types-aiobotocore-greengrass-2.5.4/types_aiobotocore_greengrass/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-greengrass-2.5.2.post3/types_aiobotocore_greengrass/__init__.pyi` & `types-aiobotocore-greengrass-2.5.4/types_aiobotocore_greengrass/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-greengrass-2.5.2.post3/types_aiobotocore_greengrass/__main__.py` & `types-aiobotocore-greengrass-2.5.4/types_aiobotocore_greengrass/__main__.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.Greengrass 2.5.2\nVersion:         2.5.2.post3\nBuilder"
+        "Type annotations for aiobotocore.Greengrass 2.5.4\nVersion:         2.5.4\nBuilder"
         " version: 7.17.2\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_greengrass//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/greengrass.html#Greengrass\nOther"
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

### Comparing `types-aiobotocore-greengrass-2.5.2.post3/types_aiobotocore_greengrass/client.py` & `types-aiobotocore-greengrass-2.5.4/types_aiobotocore_greengrass/client.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-greengrass-2.5.2.post3/types_aiobotocore_greengrass/client.pyi` & `types-aiobotocore-greengrass-2.5.4/types_aiobotocore_greengrass/client.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-greengrass-2.5.2.post3/types_aiobotocore_greengrass/literals.py` & `types-aiobotocore-greengrass-2.5.4/types_aiobotocore_greengrass/literals.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,14 @@
 import sys
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = (
     "BulkDeploymentStatusType",
     "ConfigurationSyncStatusType",
     "DeploymentTypeType",
     "EncodingTypeType",
     "FunctionIsolationModeType",
     "ListBulkDeploymentDetailedReportsPaginatorName",
@@ -56,15 +55,14 @@
     "GreengrassServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "RegionName",
 )
 
-
 BulkDeploymentStatusType = Literal[
     "Completed", "Failed", "Initializing", "Running", "Stopped", "Stopping"
 ]
 ConfigurationSyncStatusType = Literal["InSync", "OutOfSync"]
 DeploymentTypeType = Literal[
     "ForceResetDeployment", "NewDeployment", "Redeployment", "ResetDeployment"
 ]
@@ -112,14 +110,15 @@
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
@@ -215,14 +214,15 @@
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
@@ -301,26 +301,28 @@
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

### Comparing `types-aiobotocore-greengrass-2.5.2.post3/types_aiobotocore_greengrass/literals.pyi` & `types-aiobotocore-greengrass-2.5.4/types_aiobotocore_greengrass/literals.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 import sys
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
+
 __all__ = (
     "BulkDeploymentStatusType",
     "ConfigurationSyncStatusType",
     "DeploymentTypeType",
     "EncodingTypeType",
     "FunctionIsolationModeType",
     "ListBulkDeploymentDetailedReportsPaginatorName",
@@ -55,14 +56,15 @@
     "GreengrassServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "RegionName",
 )
 
+
 BulkDeploymentStatusType = Literal[
     "Completed", "Failed", "Initializing", "Running", "Stopped", "Stopping"
 ]
 ConfigurationSyncStatusType = Literal["InSync", "OutOfSync"]
 DeploymentTypeType = Literal[
     "ForceResetDeployment", "NewDeployment", "Redeployment", "ResetDeployment"
 ]
@@ -110,14 +112,15 @@
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
@@ -213,14 +216,15 @@
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
@@ -299,26 +303,28 @@
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

### Comparing `types-aiobotocore-greengrass-2.5.2.post3/types_aiobotocore_greengrass/paginator.py` & `types-aiobotocore-greengrass-2.5.4/types_aiobotocore_greengrass/paginator.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-greengrass-2.5.2.post3/types_aiobotocore_greengrass/paginator.pyi` & `types-aiobotocore-greengrass-2.5.4/types_aiobotocore_greengrass/paginator.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-greengrass-2.5.2.post3/types_aiobotocore_greengrass/type_defs.py` & `types-aiobotocore-greengrass-2.5.4/types_aiobotocore_greengrass/type_defs.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-greengrass-2.5.2.post3/types_aiobotocore_greengrass/type_defs.pyi` & `types-aiobotocore-greengrass-2.5.4/types_aiobotocore_greengrass/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-greengrass-2.5.2.post3/types_aiobotocore_greengrass.egg-info/PKG-INFO` & `types-aiobotocore-greengrass-2.5.4/types_aiobotocore_greengrass.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-greengrass
-Version: 2.5.2.post3
-Summary: Type annotations for aiobotocore.Greengrass 2.5.2 service generated with mypy-boto3-builder 7.17.2
+Version: 2.5.4
+Summary: Type annotations for aiobotocore.Greengrass 2.5.4 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_greengrass/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-greengrass.svg?color=blue)](https://pypi.org/project/types-aiobotocore-greengrass)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_greengrass/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-greengrass)](https://pepy.tech/project/types-aiobotocore-greengrass)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.Greengrass 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/greengrass.html#Greengrass)
+[aiobotocore.Greengrass 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/greengrass.html#Greengrass)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-greengrass-2.5.2.post3/types_aiobotocore_greengrass.egg-info/SOURCES.txt` & `types-aiobotocore-greengrass-2.5.4/types_aiobotocore_greengrass.egg-info/SOURCES.txt`

 * *Files identical despite different names*


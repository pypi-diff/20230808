# Comparing `tmp/types-aiobotocore-application-autoscaling-2.5.2.post3.tar.gz` & `tmp/types-aiobotocore-application-autoscaling-2.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-application-autoscaling-2.5.2.post3.tar", last modified: Fri Aug  4 12:37:16 2023, max compression
+gzip compressed data, was "types-aiobotocore-application-autoscaling-2.5.4.tar", last modified: Tue Aug  8 01:23:17 2023, max compression
```

## Comparing `types-aiobotocore-application-autoscaling-2.5.2.post3.tar` & `types-aiobotocore-application-autoscaling-2.5.4.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:37:16.431169 types-aiobotocore-application-autoscaling-2.5.2.post3/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-04 12:18:22.000000 types-aiobotocore-application-autoscaling-2.5.2.post3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    14423 2023-08-04 12:37:16.431169 types-aiobotocore-application-autoscaling-2.5.2.post3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    12842 2023-08-04 12:18:22.000000 types-aiobotocore-application-autoscaling-2.5.2.post3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-04 12:37:16.431169 types-aiobotocore-application-autoscaling-2.5.2.post3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2175 2023-08-04 12:18:22.000000 types-aiobotocore-application-autoscaling-2.5.2.post3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:37:16.431169 types-aiobotocore-application-autoscaling-2.5.2.post3/types_aiobotocore_application_autoscaling/
--rw-r--r--   0 runner    (1001) docker     (123)     1606 2023-08-04 12:18:22.000000 types-aiobotocore-application-autoscaling-2.5.2.post3/types_aiobotocore_application_autoscaling/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1605 2023-08-04 12:18:22.000000 types-aiobotocore-application-autoscaling-2.5.2.post3/types_aiobotocore_application_autoscaling/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1005 2023-08-04 12:18:22.000000 types-aiobotocore-application-autoscaling-2.5.2.post3/types_aiobotocore_application_autoscaling/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17822 2023-08-04 12:18:23.000000 types-aiobotocore-application-autoscaling-2.5.2.post3/types_aiobotocore_application_autoscaling/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    17796 2023-08-04 12:18:23.000000 types-aiobotocore-application-autoscaling-2.5.2.post3/types_aiobotocore_application_autoscaling/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    11802 2023-08-04 12:18:23.000000 types-aiobotocore-application-autoscaling-2.5.2.post3/types_aiobotocore_application_autoscaling/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    11800 2023-08-04 12:18:23.000000 types-aiobotocore-application-autoscaling-2.5.2.post3/types_aiobotocore_application_autoscaling/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     6966 2023-08-04 12:18:23.000000 types-aiobotocore-application-autoscaling-2.5.2.post3/types_aiobotocore_application_autoscaling/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     6960 2023-08-04 12:18:23.000000 types-aiobotocore-application-autoscaling-2.5.2.post3/types_aiobotocore_application_autoscaling/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 12:18:22.000000 types-aiobotocore-application-autoscaling-2.5.2.post3/types_aiobotocore_application_autoscaling/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    22793 2023-08-04 12:18:24.000000 types-aiobotocore-application-autoscaling-2.5.2.post3/types_aiobotocore_application_autoscaling/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    22750 2023-08-04 12:18:24.000000 types-aiobotocore-application-autoscaling-2.5.2.post3/types_aiobotocore_application_autoscaling/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-04 12:18:22.000000 types-aiobotocore-application-autoscaling-2.5.2.post3/types_aiobotocore_application_autoscaling/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:37:16.431169 types-aiobotocore-application-autoscaling-2.5.2.post3/types_aiobotocore_application_autoscaling.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    14423 2023-08-04 12:37:16.000000 types-aiobotocore-application-autoscaling-2.5.2.post3/types_aiobotocore_application_autoscaling.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1117 2023-08-04 12:37:16.000000 types-aiobotocore-application-autoscaling-2.5.2.post3/types_aiobotocore_application_autoscaling.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 12:37:16.000000 types-aiobotocore-application-autoscaling-2.5.2.post3/types_aiobotocore_application_autoscaling.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 12:37:16.000000 types-aiobotocore-application-autoscaling-2.5.2.post3/types_aiobotocore_application_autoscaling.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-04 12:37:16.000000 types-aiobotocore-application-autoscaling-2.5.2.post3/types_aiobotocore_application_autoscaling.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-08-04 12:37:16.000000 types-aiobotocore-application-autoscaling-2.5.2.post3/types_aiobotocore_application_autoscaling.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:23:17.046498 types-aiobotocore-application-autoscaling-2.5.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-08 01:06:10.000000 types-aiobotocore-application-autoscaling-2.5.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    14417 2023-08-08 01:23:17.046498 types-aiobotocore-application-autoscaling-2.5.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    12842 2023-08-08 01:06:10.000000 types-aiobotocore-application-autoscaling-2.5.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-08 01:23:17.046498 types-aiobotocore-application-autoscaling-2.5.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2169 2023-08-08 01:06:10.000000 types-aiobotocore-application-autoscaling-2.5.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:23:17.042498 types-aiobotocore-application-autoscaling-2.5.4/types_aiobotocore_application_autoscaling/
+-rw-r--r--   0 runner    (1001) docker     (123)     1606 2023-08-08 01:06:10.000000 types-aiobotocore-application-autoscaling-2.5.4/types_aiobotocore_application_autoscaling/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1605 2023-08-08 01:06:10.000000 types-aiobotocore-application-autoscaling-2.5.4/types_aiobotocore_application_autoscaling/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      993 2023-08-08 01:06:10.000000 types-aiobotocore-application-autoscaling-2.5.4/types_aiobotocore_application_autoscaling/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17822 2023-08-08 01:06:10.000000 types-aiobotocore-application-autoscaling-2.5.4/types_aiobotocore_application_autoscaling/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17796 2023-08-08 01:06:10.000000 types-aiobotocore-application-autoscaling-2.5.4/types_aiobotocore_application_autoscaling/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    11917 2023-08-08 01:06:10.000000 types-aiobotocore-application-autoscaling-2.5.4/types_aiobotocore_application_autoscaling/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11915 2023-08-08 01:06:10.000000 types-aiobotocore-application-autoscaling-2.5.4/types_aiobotocore_application_autoscaling/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     6966 2023-08-08 01:06:10.000000 types-aiobotocore-application-autoscaling-2.5.4/types_aiobotocore_application_autoscaling/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6960 2023-08-08 01:06:10.000000 types-aiobotocore-application-autoscaling-2.5.4/types_aiobotocore_application_autoscaling/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 01:06:10.000000 types-aiobotocore-application-autoscaling-2.5.4/types_aiobotocore_application_autoscaling/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    22793 2023-08-08 01:06:11.000000 types-aiobotocore-application-autoscaling-2.5.4/types_aiobotocore_application_autoscaling/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22750 2023-08-08 01:06:11.000000 types-aiobotocore-application-autoscaling-2.5.4/types_aiobotocore_application_autoscaling/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-08-08 01:06:10.000000 types-aiobotocore-application-autoscaling-2.5.4/types_aiobotocore_application_autoscaling/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:23:17.046498 types-aiobotocore-application-autoscaling-2.5.4/types_aiobotocore_application_autoscaling.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    14417 2023-08-08 01:23:16.000000 types-aiobotocore-application-autoscaling-2.5.4/types_aiobotocore_application_autoscaling.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1117 2023-08-08 01:23:16.000000 types-aiobotocore-application-autoscaling-2.5.4/types_aiobotocore_application_autoscaling.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 01:23:16.000000 types-aiobotocore-application-autoscaling-2.5.4/types_aiobotocore_application_autoscaling.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 01:23:16.000000 types-aiobotocore-application-autoscaling-2.5.4/types_aiobotocore_application_autoscaling.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-08 01:23:16.000000 types-aiobotocore-application-autoscaling-2.5.4/types_aiobotocore_application_autoscaling.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-08-08 01:23:16.000000 types-aiobotocore-application-autoscaling-2.5.4/types_aiobotocore_application_autoscaling.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-application-autoscaling-2.5.2.post3/LICENSE` & `types-aiobotocore-application-autoscaling-2.5.4/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-application-autoscaling-2.5.2.post3/PKG-INFO` & `types-aiobotocore-application-autoscaling-2.5.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-application-autoscaling
-Version: 2.5.2.post3
-Summary: Type annotations for aiobotocore.ApplicationAutoScaling 2.5.2 service generated with mypy-boto3-builder 7.17.2
+Version: 2.5.4
+Summary: Type annotations for aiobotocore.ApplicationAutoScaling 2.5.4 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_application_autoscaling/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-application-autoscaling.svg?color=blue)](https://pypi.org/project/types-aiobotocore-application-autoscaling)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_application_autoscaling/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-application-autoscaling)](https://pepy.tech/project/types-aiobotocore-application-autoscaling)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.ApplicationAutoScaling 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/application-autoscaling.html#ApplicationAutoScaling)
+[aiobotocore.ApplicationAutoScaling 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/application-autoscaling.html#ApplicationAutoScaling)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-application-autoscaling-2.5.2.post3/README.md` & `types-aiobotocore-application-autoscaling-2.5.4/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-application-autoscaling.svg?color=blue)](https://pypi.org/project/types-aiobotocore-application-autoscaling)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_application_autoscaling/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-application-autoscaling)](https://pepy.tech/project/types-aiobotocore-application-autoscaling)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.ApplicationAutoScaling 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/application-autoscaling.html#ApplicationAutoScaling)
+[aiobotocore.ApplicationAutoScaling 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/application-autoscaling.html#ApplicationAutoScaling)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-application-autoscaling-2.5.2.post3/setup.py` & `types-aiobotocore-application-autoscaling-2.5.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-application-autoscaling",
-    version="2.5.2.post3",
+    version="2.5.4",
     packages=["types_aiobotocore_application_autoscaling"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.ApplicationAutoScaling 2.5.2 service generated with"
+        "Type annotations for aiobotocore.ApplicationAutoScaling 2.5.4 service generated with"
         " mypy-boto3-builder 7.17.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
```

### Comparing `types-aiobotocore-application-autoscaling-2.5.2.post3/types_aiobotocore_application_autoscaling/__init__.py` & `types-aiobotocore-application-autoscaling-2.5.4/types_aiobotocore_application_autoscaling/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-application-autoscaling-2.5.2.post3/types_aiobotocore_application_autoscaling/__init__.pyi` & `types-aiobotocore-application-autoscaling-2.5.4/types_aiobotocore_application_autoscaling/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-application-autoscaling-2.5.2.post3/types_aiobotocore_application_autoscaling/__main__.py` & `types-aiobotocore-application-autoscaling-2.5.4/types_aiobotocore_application_autoscaling/__main__.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.ApplicationAutoScaling 2.5.2\nVersion:        "
-        " 2.5.2.post3\nBuilder version: 7.17.2\nDocs:           "
+        "Type annotations for aiobotocore.ApplicationAutoScaling 2.5.4\nVersion:        "
+        " 2.5.4\nBuilder version: 7.17.2\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_application_autoscaling//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/application-autoscaling.html#ApplicationAutoScaling\nOther"
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

### Comparing `types-aiobotocore-application-autoscaling-2.5.2.post3/types_aiobotocore_application_autoscaling/client.py` & `types-aiobotocore-application-autoscaling-2.5.4/types_aiobotocore_application_autoscaling/client.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-application-autoscaling-2.5.2.post3/types_aiobotocore_application_autoscaling/client.pyi` & `types-aiobotocore-application-autoscaling-2.5.4/types_aiobotocore_application_autoscaling/client.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-application-autoscaling-2.5.2.post3/types_aiobotocore_application_autoscaling/literals.py` & `types-aiobotocore-application-autoscaling-2.5.4/types_aiobotocore_application_autoscaling/literals.pyi`

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
     "AdjustmentTypeType",
     "DescribeScalableTargetsPaginatorName",
     "DescribeScalingActivitiesPaginatorName",
     "DescribeScalingPoliciesPaginatorName",
     "DescribeScheduledActionsPaginatorName",
     "MetricAggregationTypeType",
@@ -35,15 +34,14 @@
     "ApplicationAutoScalingServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "RegionName",
 )
 
-
 AdjustmentTypeType = Literal["ChangeInCapacity", "ExactCapacity", "PercentChangeInCapacity"]
 DescribeScalableTargetsPaginatorName = Literal["describe_scalable_targets"]
 DescribeScalingActivitiesPaginatorName = Literal["describe_scaling_activities"]
 DescribeScalingPoliciesPaginatorName = Literal["describe_scaling_policies"]
 DescribeScheduledActionsPaginatorName = Literal["describe_scheduled_actions"]
 MetricAggregationTypeType = Literal["Average", "Maximum", "Minimum"]
 MetricStatisticType = Literal["Average", "Maximum", "Minimum", "SampleCount", "Sum"]
@@ -127,14 +125,15 @@
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
@@ -230,14 +229,15 @@
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
@@ -316,26 +316,28 @@
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
@@ -502,14 +504,15 @@
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

### Comparing `types-aiobotocore-application-autoscaling-2.5.2.post3/types_aiobotocore_application_autoscaling/literals.pyi` & `types-aiobotocore-application-autoscaling-2.5.4/types_aiobotocore_application_autoscaling/literals.py`

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
     "AdjustmentTypeType",
     "DescribeScalableTargetsPaginatorName",
     "DescribeScalingActivitiesPaginatorName",
     "DescribeScalingPoliciesPaginatorName",
     "DescribeScheduledActionsPaginatorName",
     "MetricAggregationTypeType",
@@ -34,14 +35,15 @@
     "ApplicationAutoScalingServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "RegionName",
 )
 
+
 AdjustmentTypeType = Literal["ChangeInCapacity", "ExactCapacity", "PercentChangeInCapacity"]
 DescribeScalableTargetsPaginatorName = Literal["describe_scalable_targets"]
 DescribeScalingActivitiesPaginatorName = Literal["describe_scaling_activities"]
 DescribeScalingPoliciesPaginatorName = Literal["describe_scaling_policies"]
 DescribeScheduledActionsPaginatorName = Literal["describe_scheduled_actions"]
 MetricAggregationTypeType = Literal["Average", "Maximum", "Minimum"]
 MetricStatisticType = Literal["Average", "Maximum", "Minimum", "SampleCount", "Sum"]
@@ -125,14 +127,15 @@
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
@@ -228,14 +231,15 @@
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
@@ -314,26 +318,28 @@
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
@@ -500,14 +506,15 @@
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

### Comparing `types-aiobotocore-application-autoscaling-2.5.2.post3/types_aiobotocore_application_autoscaling/paginator.py` & `types-aiobotocore-application-autoscaling-2.5.4/types_aiobotocore_application_autoscaling/paginator.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-application-autoscaling-2.5.2.post3/types_aiobotocore_application_autoscaling/paginator.pyi` & `types-aiobotocore-application-autoscaling-2.5.4/types_aiobotocore_application_autoscaling/paginator.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-application-autoscaling-2.5.2.post3/types_aiobotocore_application_autoscaling/type_defs.py` & `types-aiobotocore-application-autoscaling-2.5.4/types_aiobotocore_application_autoscaling/type_defs.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-application-autoscaling-2.5.2.post3/types_aiobotocore_application_autoscaling/type_defs.pyi` & `types-aiobotocore-application-autoscaling-2.5.4/types_aiobotocore_application_autoscaling/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-application-autoscaling-2.5.2.post3/types_aiobotocore_application_autoscaling.egg-info/PKG-INFO` & `types-aiobotocore-application-autoscaling-2.5.4/types_aiobotocore_application_autoscaling.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-application-autoscaling
-Version: 2.5.2.post3
-Summary: Type annotations for aiobotocore.ApplicationAutoScaling 2.5.2 service generated with mypy-boto3-builder 7.17.2
+Version: 2.5.4
+Summary: Type annotations for aiobotocore.ApplicationAutoScaling 2.5.4 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_application_autoscaling/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-application-autoscaling.svg?color=blue)](https://pypi.org/project/types-aiobotocore-application-autoscaling)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_application_autoscaling/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-application-autoscaling)](https://pepy.tech/project/types-aiobotocore-application-autoscaling)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.ApplicationAutoScaling 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/application-autoscaling.html#ApplicationAutoScaling)
+[aiobotocore.ApplicationAutoScaling 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/application-autoscaling.html#ApplicationAutoScaling)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-application-autoscaling-2.5.2.post3/types_aiobotocore_application_autoscaling.egg-info/SOURCES.txt` & `types-aiobotocore-application-autoscaling-2.5.4/types_aiobotocore_application_autoscaling.egg-info/SOURCES.txt`

 * *Files identical despite different names*


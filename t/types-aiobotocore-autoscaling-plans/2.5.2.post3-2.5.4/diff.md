# Comparing `tmp/types-aiobotocore-autoscaling-plans-2.5.2.post3.tar.gz` & `tmp/types-aiobotocore-autoscaling-plans-2.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-autoscaling-plans-2.5.2.post3.tar", last modified: Fri Aug  4 12:37:19 2023, max compression
+gzip compressed data, was "types-aiobotocore-autoscaling-plans-2.5.4.tar", last modified: Tue Aug  8 01:23:21 2023, max compression
```

## Comparing `types-aiobotocore-autoscaling-plans-2.5.2.post3.tar` & `types-aiobotocore-autoscaling-plans-2.5.4.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:37:19.011228 types-aiobotocore-autoscaling-plans-2.5.2.post3/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-04 12:18:50.000000 types-aiobotocore-autoscaling-plans-2.5.2.post3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    13765 2023-08-04 12:37:19.003228 types-aiobotocore-autoscaling-plans-2.5.2.post3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    12208 2023-08-04 12:18:50.000000 types-aiobotocore-autoscaling-plans-2.5.2.post3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-04 12:37:19.011228 types-aiobotocore-autoscaling-plans-2.5.2.post3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2141 2023-08-04 12:18:50.000000 types-aiobotocore-autoscaling-plans-2.5.2.post3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:37:18.995227 types-aiobotocore-autoscaling-plans-2.5.2.post3/types_aiobotocore_autoscaling_plans/
--rw-r--r--   0 runner    (1001) docker     (123)     1049 2023-08-04 12:18:50.000000 types-aiobotocore-autoscaling-plans-2.5.2.post3/types_aiobotocore_autoscaling_plans/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1048 2023-08-04 12:18:50.000000 types-aiobotocore-autoscaling-plans-2.5.2.post3/types_aiobotocore_autoscaling_plans/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      981 2023-08-04 12:18:50.000000 types-aiobotocore-autoscaling-plans-2.5.2.post3/types_aiobotocore_autoscaling_plans/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10249 2023-08-04 12:18:50.000000 types-aiobotocore-autoscaling-plans-2.5.2.post3/types_aiobotocore_autoscaling_plans/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    10232 2023-08-04 12:18:50.000000 types-aiobotocore-autoscaling-plans-2.5.2.post3/types_aiobotocore_autoscaling_plans/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    10849 2023-08-04 12:18:51.000000 types-aiobotocore-autoscaling-plans-2.5.2.post3/types_aiobotocore_autoscaling_plans/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    10847 2023-08-04 12:18:51.000000 types-aiobotocore-autoscaling-plans-2.5.2.post3/types_aiobotocore_autoscaling_plans/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     3766 2023-08-04 12:18:50.000000 types-aiobotocore-autoscaling-plans-2.5.2.post3/types_aiobotocore_autoscaling_plans/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     3762 2023-08-04 12:18:50.000000 types-aiobotocore-autoscaling-plans-2.5.2.post3/types_aiobotocore_autoscaling_plans/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 12:18:50.000000 types-aiobotocore-autoscaling-plans-2.5.2.post3/types_aiobotocore_autoscaling_plans/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    14086 2023-08-04 12:18:51.000000 types-aiobotocore-autoscaling-plans-2.5.2.post3/types_aiobotocore_autoscaling_plans/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    14061 2023-08-04 12:18:51.000000 types-aiobotocore-autoscaling-plans-2.5.2.post3/types_aiobotocore_autoscaling_plans/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-04 12:18:50.000000 types-aiobotocore-autoscaling-plans-2.5.2.post3/types_aiobotocore_autoscaling_plans/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:37:19.003228 types-aiobotocore-autoscaling-plans-2.5.2.post3/types_aiobotocore_autoscaling_plans.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    13765 2023-08-04 12:37:18.000000 types-aiobotocore-autoscaling-plans-2.5.2.post3/types_aiobotocore_autoscaling_plans.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1003 2023-08-04 12:37:18.000000 types-aiobotocore-autoscaling-plans-2.5.2.post3/types_aiobotocore_autoscaling_plans.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 12:37:18.000000 types-aiobotocore-autoscaling-plans-2.5.2.post3/types_aiobotocore_autoscaling_plans.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 12:37:18.000000 types-aiobotocore-autoscaling-plans-2.5.2.post3/types_aiobotocore_autoscaling_plans.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-04 12:37:18.000000 types-aiobotocore-autoscaling-plans-2.5.2.post3/types_aiobotocore_autoscaling_plans.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-08-04 12:37:18.000000 types-aiobotocore-autoscaling-plans-2.5.2.post3/types_aiobotocore_autoscaling_plans.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:23:21.578620 types-aiobotocore-autoscaling-plans-2.5.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-08 01:06:37.000000 types-aiobotocore-autoscaling-plans-2.5.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    13759 2023-08-08 01:23:21.578620 types-aiobotocore-autoscaling-plans-2.5.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    12208 2023-08-08 01:06:37.000000 types-aiobotocore-autoscaling-plans-2.5.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-08 01:23:21.578620 types-aiobotocore-autoscaling-plans-2.5.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2135 2023-08-08 01:06:36.000000 types-aiobotocore-autoscaling-plans-2.5.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:23:21.570620 types-aiobotocore-autoscaling-plans-2.5.4/types_aiobotocore_autoscaling_plans/
+-rw-r--r--   0 runner    (1001) docker     (123)     1049 2023-08-08 01:06:37.000000 types-aiobotocore-autoscaling-plans-2.5.4/types_aiobotocore_autoscaling_plans/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1048 2023-08-08 01:06:37.000000 types-aiobotocore-autoscaling-plans-2.5.4/types_aiobotocore_autoscaling_plans/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      969 2023-08-08 01:06:37.000000 types-aiobotocore-autoscaling-plans-2.5.4/types_aiobotocore_autoscaling_plans/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10249 2023-08-08 01:06:37.000000 types-aiobotocore-autoscaling-plans-2.5.4/types_aiobotocore_autoscaling_plans/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10232 2023-08-08 01:06:37.000000 types-aiobotocore-autoscaling-plans-2.5.4/types_aiobotocore_autoscaling_plans/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    10944 2023-08-08 01:06:37.000000 types-aiobotocore-autoscaling-plans-2.5.4/types_aiobotocore_autoscaling_plans/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10942 2023-08-08 01:06:37.000000 types-aiobotocore-autoscaling-plans-2.5.4/types_aiobotocore_autoscaling_plans/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     3766 2023-08-08 01:06:37.000000 types-aiobotocore-autoscaling-plans-2.5.4/types_aiobotocore_autoscaling_plans/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3762 2023-08-08 01:06:37.000000 types-aiobotocore-autoscaling-plans-2.5.4/types_aiobotocore_autoscaling_plans/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 01:06:37.000000 types-aiobotocore-autoscaling-plans-2.5.4/types_aiobotocore_autoscaling_plans/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    14086 2023-08-08 01:06:37.000000 types-aiobotocore-autoscaling-plans-2.5.4/types_aiobotocore_autoscaling_plans/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14061 2023-08-08 01:06:37.000000 types-aiobotocore-autoscaling-plans-2.5.4/types_aiobotocore_autoscaling_plans/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-08-08 01:06:37.000000 types-aiobotocore-autoscaling-plans-2.5.4/types_aiobotocore_autoscaling_plans/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:23:21.578620 types-aiobotocore-autoscaling-plans-2.5.4/types_aiobotocore_autoscaling_plans.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    13759 2023-08-08 01:23:21.000000 types-aiobotocore-autoscaling-plans-2.5.4/types_aiobotocore_autoscaling_plans.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1003 2023-08-08 01:23:21.000000 types-aiobotocore-autoscaling-plans-2.5.4/types_aiobotocore_autoscaling_plans.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 01:23:21.000000 types-aiobotocore-autoscaling-plans-2.5.4/types_aiobotocore_autoscaling_plans.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 01:23:21.000000 types-aiobotocore-autoscaling-plans-2.5.4/types_aiobotocore_autoscaling_plans.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-08 01:23:21.000000 types-aiobotocore-autoscaling-plans-2.5.4/types_aiobotocore_autoscaling_plans.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-08-08 01:23:21.000000 types-aiobotocore-autoscaling-plans-2.5.4/types_aiobotocore_autoscaling_plans.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-autoscaling-plans-2.5.2.post3/LICENSE` & `types-aiobotocore-autoscaling-plans-2.5.4/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-autoscaling-plans-2.5.2.post3/PKG-INFO` & `types-aiobotocore-autoscaling-plans-2.5.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-autoscaling-plans
-Version: 2.5.2.post3
-Summary: Type annotations for aiobotocore.AutoScalingPlans 2.5.2 service generated with mypy-boto3-builder 7.17.2
+Version: 2.5.4
+Summary: Type annotations for aiobotocore.AutoScalingPlans 2.5.4 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_autoscaling_plans/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-autoscaling-plans.svg?color=blue)](https://pypi.org/project/types-aiobotocore-autoscaling-plans)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_autoscaling_plans/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-autoscaling-plans)](https://pepy.tech/project/types-aiobotocore-autoscaling-plans)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.AutoScalingPlans 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling-plans.html#AutoScalingPlans)
+[aiobotocore.AutoScalingPlans 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling-plans.html#AutoScalingPlans)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-autoscaling-plans-2.5.2.post3/README.md` & `types-aiobotocore-autoscaling-plans-2.5.4/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-autoscaling-plans.svg?color=blue)](https://pypi.org/project/types-aiobotocore-autoscaling-plans)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_autoscaling_plans/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-autoscaling-plans)](https://pepy.tech/project/types-aiobotocore-autoscaling-plans)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.AutoScalingPlans 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling-plans.html#AutoScalingPlans)
+[aiobotocore.AutoScalingPlans 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling-plans.html#AutoScalingPlans)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-autoscaling-plans-2.5.2.post3/setup.py` & `types-aiobotocore-autoscaling-plans-2.5.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-autoscaling-plans",
-    version="2.5.2.post3",
+    version="2.5.4",
     packages=["types_aiobotocore_autoscaling_plans"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.AutoScalingPlans 2.5.2 service generated with"
+        "Type annotations for aiobotocore.AutoScalingPlans 2.5.4 service generated with"
         " mypy-boto3-builder 7.17.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
```

### Comparing `types-aiobotocore-autoscaling-plans-2.5.2.post3/types_aiobotocore_autoscaling_plans/__init__.py` & `types-aiobotocore-autoscaling-plans-2.5.4/types_aiobotocore_autoscaling_plans/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-autoscaling-plans-2.5.2.post3/types_aiobotocore_autoscaling_plans/__init__.pyi` & `types-aiobotocore-autoscaling-plans-2.5.4/types_aiobotocore_autoscaling_plans/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-autoscaling-plans-2.5.2.post3/types_aiobotocore_autoscaling_plans/client.py` & `types-aiobotocore-autoscaling-plans-2.5.4/types_aiobotocore_autoscaling_plans/client.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-autoscaling-plans-2.5.2.post3/types_aiobotocore_autoscaling_plans/client.pyi` & `types-aiobotocore-autoscaling-plans-2.5.4/types_aiobotocore_autoscaling_plans/client.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-autoscaling-plans-2.5.2.post3/types_aiobotocore_autoscaling_plans/literals.py` & `types-aiobotocore-autoscaling-plans-2.5.4/types_aiobotocore_autoscaling_plans/literals.pyi`

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
     "DescribeScalingPlanResourcesPaginatorName",
     "DescribeScalingPlansPaginatorName",
     "ForecastDataTypeType",
     "LoadMetricTypeType",
     "MetricStatisticType",
     "PolicyTypeType",
@@ -37,15 +36,14 @@
     "AutoScalingPlansServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "RegionName",
 )
 
-
 DescribeScalingPlanResourcesPaginatorName = Literal["describe_scaling_plan_resources"]
 DescribeScalingPlansPaginatorName = Literal["describe_scaling_plans"]
 ForecastDataTypeType = Literal[
     "CapacityForecast", "LoadForecast", "ScheduledActionMaxCapacity", "ScheduledActionMinCapacity"
 ]
 LoadMetricTypeType = Literal[
     "ALBTargetGroupRequestCount",
@@ -111,14 +109,15 @@
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
@@ -214,14 +213,15 @@
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
@@ -300,26 +300,28 @@
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

### Comparing `types-aiobotocore-autoscaling-plans-2.5.2.post3/types_aiobotocore_autoscaling_plans/literals.pyi` & `types-aiobotocore-autoscaling-plans-2.5.4/types_aiobotocore_autoscaling_plans/literals.py`

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
     "DescribeScalingPlanResourcesPaginatorName",
     "DescribeScalingPlansPaginatorName",
     "ForecastDataTypeType",
     "LoadMetricTypeType",
     "MetricStatisticType",
     "PolicyTypeType",
@@ -36,14 +37,15 @@
     "AutoScalingPlansServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "RegionName",
 )
 
+
 DescribeScalingPlanResourcesPaginatorName = Literal["describe_scaling_plan_resources"]
 DescribeScalingPlansPaginatorName = Literal["describe_scaling_plans"]
 ForecastDataTypeType = Literal[
     "CapacityForecast", "LoadForecast", "ScheduledActionMaxCapacity", "ScheduledActionMinCapacity"
 ]
 LoadMetricTypeType = Literal[
     "ALBTargetGroupRequestCount",
@@ -109,14 +111,15 @@
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
@@ -212,14 +215,15 @@
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
@@ -298,26 +302,28 @@
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

### Comparing `types-aiobotocore-autoscaling-plans-2.5.2.post3/types_aiobotocore_autoscaling_plans/paginator.py` & `types-aiobotocore-autoscaling-plans-2.5.4/types_aiobotocore_autoscaling_plans/paginator.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-autoscaling-plans-2.5.2.post3/types_aiobotocore_autoscaling_plans/paginator.pyi` & `types-aiobotocore-autoscaling-plans-2.5.4/types_aiobotocore_autoscaling_plans/paginator.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-autoscaling-plans-2.5.2.post3/types_aiobotocore_autoscaling_plans/type_defs.py` & `types-aiobotocore-autoscaling-plans-2.5.4/types_aiobotocore_autoscaling_plans/type_defs.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-autoscaling-plans-2.5.2.post3/types_aiobotocore_autoscaling_plans/type_defs.pyi` & `types-aiobotocore-autoscaling-plans-2.5.4/types_aiobotocore_autoscaling_plans/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-autoscaling-plans-2.5.2.post3/types_aiobotocore_autoscaling_plans.egg-info/PKG-INFO` & `types-aiobotocore-autoscaling-plans-2.5.4/types_aiobotocore_autoscaling_plans.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-autoscaling-plans
-Version: 2.5.2.post3
-Summary: Type annotations for aiobotocore.AutoScalingPlans 2.5.2 service generated with mypy-boto3-builder 7.17.2
+Version: 2.5.4
+Summary: Type annotations for aiobotocore.AutoScalingPlans 2.5.4 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_autoscaling_plans/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-autoscaling-plans.svg?color=blue)](https://pypi.org/project/types-aiobotocore-autoscaling-plans)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_autoscaling_plans/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-autoscaling-plans)](https://pepy.tech/project/types-aiobotocore-autoscaling-plans)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.AutoScalingPlans 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling-plans.html#AutoScalingPlans)
+[aiobotocore.AutoScalingPlans 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling-plans.html#AutoScalingPlans)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-autoscaling-plans-2.5.2.post3/types_aiobotocore_autoscaling_plans.egg-info/SOURCES.txt` & `types-aiobotocore-autoscaling-plans-2.5.4/types_aiobotocore_autoscaling_plans.egg-info/SOURCES.txt`

 * *Files identical despite different names*


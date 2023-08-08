# Comparing `tmp/types-aiobotocore-ce-2.5.2.post3.tar.gz` & `tmp/types-aiobotocore-ce-2.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-ce-2.5.2.post3.tar", last modified: Fri Aug  4 12:37:21 2023, max compression
+gzip compressed data, was "types-aiobotocore-ce-2.5.4.tar", last modified: Tue Aug  8 01:23:23 2023, max compression
```

## Comparing `types-aiobotocore-ce-2.5.2.post3.tar` & `types-aiobotocore-ce-2.5.4.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:37:21.567281 types-aiobotocore-ce-2.5.2.post3/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-04 12:19:06.000000 types-aiobotocore-ce-2.5.2.post3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    12017 2023-08-04 12:37:21.563280 types-aiobotocore-ce-2.5.2.post3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    10509 2023-08-04 12:19:06.000000 types-aiobotocore-ce-2.5.2.post3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-04 12:37:21.567281 types-aiobotocore-ce-2.5.2.post3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2023 2023-08-04 12:19:06.000000 types-aiobotocore-ce-2.5.2.post3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:37:21.559280 types-aiobotocore-ce-2.5.2.post3/types_aiobotocore_ce/
--rw-r--r--   0 runner    (1001) docker     (123)      452 2023-08-04 12:19:06.000000 types-aiobotocore-ce-2.5.2.post3/types_aiobotocore_ce/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      451 2023-08-04 12:19:06.000000 types-aiobotocore-ce-2.5.2.post3/types_aiobotocore_ce/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      932 2023-08-04 12:19:06.000000 types-aiobotocore-ce-2.5.2.post3/types_aiobotocore_ce/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    33821 2023-08-04 12:19:07.000000 types-aiobotocore-ce-2.5.2.post3/types_aiobotocore_ce/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    33775 2023-08-04 12:19:06.000000 types-aiobotocore-ce-2.5.2.post3/types_aiobotocore_ce/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    12638 2023-08-04 12:19:07.000000 types-aiobotocore-ce-2.5.2.post3/types_aiobotocore_ce/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    12636 2023-08-04 12:19:07.000000 types-aiobotocore-ce-2.5.2.post3/types_aiobotocore_ce/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 12:19:06.000000 types-aiobotocore-ce-2.5.2.post3/types_aiobotocore_ce/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    63392 2023-08-04 12:19:08.000000 types-aiobotocore-ce-2.5.2.post3/types_aiobotocore_ce/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    63323 2023-08-04 12:19:07.000000 types-aiobotocore-ce-2.5.2.post3/types_aiobotocore_ce/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-04 12:19:06.000000 types-aiobotocore-ce-2.5.2.post3/types_aiobotocore_ce/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:37:21.559280 types-aiobotocore-ce-2.5.2.post3/types_aiobotocore_ce.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    12017 2023-08-04 12:37:21.000000 types-aiobotocore-ce-2.5.2.post3/types_aiobotocore_ce.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      649 2023-08-04 12:37:21.000000 types-aiobotocore-ce-2.5.2.post3/types_aiobotocore_ce.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 12:37:21.000000 types-aiobotocore-ce-2.5.2.post3/types_aiobotocore_ce.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 12:37:21.000000 types-aiobotocore-ce-2.5.2.post3/types_aiobotocore_ce.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-04 12:37:21.000000 types-aiobotocore-ce-2.5.2.post3/types_aiobotocore_ce.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-08-04 12:37:21.000000 types-aiobotocore-ce-2.5.2.post3/types_aiobotocore_ce.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:23:22.994622 types-aiobotocore-ce-2.5.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-08 01:06:51.000000 types-aiobotocore-ce-2.5.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    12011 2023-08-08 01:23:22.986622 types-aiobotocore-ce-2.5.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10509 2023-08-08 01:06:51.000000 types-aiobotocore-ce-2.5.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-08 01:23:22.994622 types-aiobotocore-ce-2.5.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2017 2023-08-08 01:06:51.000000 types-aiobotocore-ce-2.5.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:23:22.986622 types-aiobotocore-ce-2.5.4/types_aiobotocore_ce/
+-rw-r--r--   0 runner    (1001) docker     (123)      452 2023-08-08 01:06:51.000000 types-aiobotocore-ce-2.5.4/types_aiobotocore_ce/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      451 2023-08-08 01:06:51.000000 types-aiobotocore-ce-2.5.4/types_aiobotocore_ce/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      920 2023-08-08 01:06:51.000000 types-aiobotocore-ce-2.5.4/types_aiobotocore_ce/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34509 2023-08-08 01:06:51.000000 types-aiobotocore-ce-2.5.4/types_aiobotocore_ce/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34462 2023-08-08 01:06:51.000000 types-aiobotocore-ce-2.5.4/types_aiobotocore_ce/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    12733 2023-08-08 01:06:51.000000 types-aiobotocore-ce-2.5.4/types_aiobotocore_ce/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12731 2023-08-08 01:06:51.000000 types-aiobotocore-ce-2.5.4/types_aiobotocore_ce/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 01:06:51.000000 types-aiobotocore-ce-2.5.4/types_aiobotocore_ce/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    65817 2023-08-08 01:06:53.000000 types-aiobotocore-ce-2.5.4/types_aiobotocore_ce/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    65748 2023-08-08 01:06:53.000000 types-aiobotocore-ce-2.5.4/types_aiobotocore_ce/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-08-08 01:06:51.000000 types-aiobotocore-ce-2.5.4/types_aiobotocore_ce/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:23:22.986622 types-aiobotocore-ce-2.5.4/types_aiobotocore_ce.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    12011 2023-08-08 01:23:22.000000 types-aiobotocore-ce-2.5.4/types_aiobotocore_ce.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      649 2023-08-08 01:23:22.000000 types-aiobotocore-ce-2.5.4/types_aiobotocore_ce.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 01:23:22.000000 types-aiobotocore-ce-2.5.4/types_aiobotocore_ce.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 01:23:22.000000 types-aiobotocore-ce-2.5.4/types_aiobotocore_ce.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-08 01:23:22.000000 types-aiobotocore-ce-2.5.4/types_aiobotocore_ce.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-08-08 01:23:22.000000 types-aiobotocore-ce-2.5.4/types_aiobotocore_ce.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-ce-2.5.2.post3/LICENSE` & `types-aiobotocore-ce-2.5.4/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-ce-2.5.2.post3/PKG-INFO` & `types-aiobotocore-ce-2.5.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-ce
-Version: 2.5.2.post3
-Summary: Type annotations for aiobotocore.CostExplorer 2.5.2 service generated with mypy-boto3-builder 7.17.2
+Version: 2.5.4
+Summary: Type annotations for aiobotocore.CostExplorer 2.5.4 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ce/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-ce.svg?color=blue)](https://pypi.org/project/types-aiobotocore-ce)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ce/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-ce)](https://pepy.tech/project/types-aiobotocore-ce)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.CostExplorer 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ce.html#CostExplorer)
+[aiobotocore.CostExplorer 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ce.html#CostExplorer)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-ce-2.5.2.post3/README.md` & `types-aiobotocore-ce-2.5.4/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-ce.svg?color=blue)](https://pypi.org/project/types-aiobotocore-ce)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ce/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-ce)](https://pepy.tech/project/types-aiobotocore-ce)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.CostExplorer 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ce.html#CostExplorer)
+[aiobotocore.CostExplorer 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ce.html#CostExplorer)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-ce-2.5.2.post3/setup.py` & `types-aiobotocore-ce-2.5.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-ce",
-    version="2.5.2.post3",
+    version="2.5.4",
     packages=["types_aiobotocore_ce"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.CostExplorer 2.5.2 service generated with"
+        "Type annotations for aiobotocore.CostExplorer 2.5.4 service generated with"
         " mypy-boto3-builder 7.17.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
```

### Comparing `types-aiobotocore-ce-2.5.2.post3/types_aiobotocore_ce/__main__.py` & `types-aiobotocore-ce-2.5.4/types_aiobotocore_ce/__main__.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.CostExplorer 2.5.2\nVersion:         2.5.2.post3\nBuilder"
+        "Type annotations for aiobotocore.CostExplorer 2.5.4\nVersion:         2.5.4\nBuilder"
         " version: 7.17.2\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ce//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ce.html#CostExplorer\nOther"
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

### Comparing `types-aiobotocore-ce-2.5.2.post3/types_aiobotocore_ce/client.py` & `types-aiobotocore-ce-2.5.4/types_aiobotocore_ce/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -59,14 +59,15 @@
     GetCostCategoriesResponseTypeDef,
     GetCostForecastResponseTypeDef,
     GetDimensionValuesResponseTypeDef,
     GetReservationCoverageResponseTypeDef,
     GetReservationPurchaseRecommendationResponseTypeDef,
     GetReservationUtilizationResponseTypeDef,
     GetRightsizingRecommendationResponseTypeDef,
+    GetSavingsPlanPurchaseRecommendationDetailsResponseTypeDef,
     GetSavingsPlansCoverageResponseTypeDef,
     GetSavingsPlansPurchaseRecommendationResponseTypeDef,
     GetSavingsPlansUtilizationDetailsResponseTypeDef,
     GetSavingsPlansUtilizationResponseTypeDef,
     GetTagsResponseTypeDef,
     GetUsageForecastResponseTypeDef,
     GroupDefinitionTypeDef,
@@ -460,14 +461,24 @@
         Creates recommendations that help you save cost by identifying idle and
         underutilized Amazon EC2 instances.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ce.html#CostExplorer.Client.get_rightsizing_recommendation)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ce/client/#get_rightsizing_recommendation)
         """
 
+    async def get_savings_plan_purchase_recommendation_details(
+        self, *, RecommendationDetailId: str
+    ) -> GetSavingsPlanPurchaseRecommendationDetailsResponseTypeDef:
+        """
+        Retrieves the details for a Savings Plan recommendation.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ce.html#CostExplorer.Client.get_savings_plan_purchase_recommendation_details)
+        [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ce/client/#get_savings_plan_purchase_recommendation_details)
+        """
+
     async def get_savings_plans_coverage(
         self,
         *,
         TimePeriod: DateIntervalTypeDef,
         GroupBy: Sequence[GroupDefinitionTypeDef] = ...,
         Granularity: GranularityType = ...,
         Filter: "ExpressionTypeDef" = ...,
@@ -683,15 +694,15 @@
         Frequency: AnomalySubscriptionFrequencyType = ...,
         MonitorArnList: Sequence[str] = ...,
         Subscribers: Sequence[SubscriberTypeDef] = ...,
         SubscriptionName: str = ...,
         ThresholdExpression: "ExpressionTypeDef" = ...
     ) -> UpdateAnomalySubscriptionResponseTypeDef:
         """
-        Updates an existing cost anomaly monitor subscription.
+        Updates an existing cost anomaly subscription.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ce.html#CostExplorer.Client.update_anomaly_subscription)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ce/client/#update_anomaly_subscription)
         """
 
     async def update_cost_allocation_tags_status(
         self, *, CostAllocationTagsStatus: Sequence[CostAllocationTagStatusEntryTypeDef]
```

### Comparing `types-aiobotocore-ce-2.5.2.post3/types_aiobotocore_ce/client.pyi` & `types-aiobotocore-ce-2.5.4/types_aiobotocore_ce/client.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -59,14 +59,15 @@
     GetCostCategoriesResponseTypeDef,
     GetCostForecastResponseTypeDef,
     GetDimensionValuesResponseTypeDef,
     GetReservationCoverageResponseTypeDef,
     GetReservationPurchaseRecommendationResponseTypeDef,
     GetReservationUtilizationResponseTypeDef,
     GetRightsizingRecommendationResponseTypeDef,
+    GetSavingsPlanPurchaseRecommendationDetailsResponseTypeDef,
     GetSavingsPlansCoverageResponseTypeDef,
     GetSavingsPlansPurchaseRecommendationResponseTypeDef,
     GetSavingsPlansUtilizationDetailsResponseTypeDef,
     GetSavingsPlansUtilizationResponseTypeDef,
     GetTagsResponseTypeDef,
     GetUsageForecastResponseTypeDef,
     GroupDefinitionTypeDef,
@@ -433,14 +434,23 @@
         """
         Creates recommendations that help you save cost by identifying idle and
         underutilized Amazon EC2 instances.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ce.html#CostExplorer.Client.get_rightsizing_recommendation)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ce/client/#get_rightsizing_recommendation)
         """
+    async def get_savings_plan_purchase_recommendation_details(
+        self, *, RecommendationDetailId: str
+    ) -> GetSavingsPlanPurchaseRecommendationDetailsResponseTypeDef:
+        """
+        Retrieves the details for a Savings Plan recommendation.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ce.html#CostExplorer.Client.get_savings_plan_purchase_recommendation_details)
+        [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ce/client/#get_savings_plan_purchase_recommendation_details)
+        """
     async def get_savings_plans_coverage(
         self,
         *,
         TimePeriod: DateIntervalTypeDef,
         GroupBy: Sequence[GroupDefinitionTypeDef] = ...,
         Granularity: GranularityType = ...,
         Filter: "ExpressionTypeDef" = ...,
@@ -641,15 +651,15 @@
         Frequency: AnomalySubscriptionFrequencyType = ...,
         MonitorArnList: Sequence[str] = ...,
         Subscribers: Sequence[SubscriberTypeDef] = ...,
         SubscriptionName: str = ...,
         ThresholdExpression: "ExpressionTypeDef" = ...
     ) -> UpdateAnomalySubscriptionResponseTypeDef:
         """
-        Updates an existing cost anomaly monitor subscription.
+        Updates an existing cost anomaly subscription.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ce.html#CostExplorer.Client.update_anomaly_subscription)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ce/client/#update_anomaly_subscription)
         """
     async def update_cost_allocation_tags_status(
         self, *, CostAllocationTagsStatus: Sequence[CostAllocationTagStatusEntryTypeDef]
     ) -> UpdateCostAllocationTagsStatusResponseTypeDef:
```

### Comparing `types-aiobotocore-ce-2.5.2.post3/types_aiobotocore_ce/literals.py` & `types-aiobotocore-ce-2.5.4/types_aiobotocore_ce/literals.py`

 * *Files 1% similar despite different names*

```diff
@@ -192,14 +192,15 @@
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
@@ -295,14 +296,15 @@
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
@@ -381,26 +383,28 @@
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

### Comparing `types-aiobotocore-ce-2.5.2.post3/types_aiobotocore_ce/literals.pyi` & `types-aiobotocore-ce-2.5.4/types_aiobotocore_ce/literals.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -190,14 +190,15 @@
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
@@ -293,14 +294,15 @@
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
@@ -379,26 +381,28 @@
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

### Comparing `types-aiobotocore-ce-2.5.2.post3/types_aiobotocore_ce/type_defs.py` & `types-aiobotocore-ce-2.5.4/types_aiobotocore_ce/type_defs.py`

 * *Files 1% similar despite different names*

```diff
@@ -100,23 +100,25 @@
     "SortDefinitionTypeDef",
     "MetricValueTypeDef",
     "ReservationPurchaseRecommendationMetadataTypeDef",
     "ReservationAggregatesTypeDef",
     "RightsizingRecommendationConfigurationTypeDef",
     "RightsizingRecommendationMetadataTypeDef",
     "RightsizingRecommendationSummaryTypeDef",
+    "GetSavingsPlanPurchaseRecommendationDetailsRequestRequestTypeDef",
     "GetSavingsPlansPurchaseRecommendationRequestRequestTypeDef",
     "SavingsPlansPurchaseRecommendationMetadataTypeDef",
     "RDSInstanceDetailsTypeDef",
     "RedshiftInstanceDetailsTypeDef",
     "ListCostAllocationTagsRequestRequestTypeDef",
     "ListCostCategoryDefinitionsRequestRequestTypeDef",
     "ListSavingsPlansPurchaseRecommendationGenerationRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
     "ProvideAnomalyFeedbackRequestRequestTypeDef",
+    "RecommendationDetailHourlyMetricsTypeDef",
     "ReservationPurchaseRecommendationSummaryTypeDef",
     "TerminateRecommendationDetailTypeDef",
     "SavingsPlansAmortizedCommitmentTypeDef",
     "SavingsPlansCoverageDataTypeDef",
     "SavingsPlansDetailsTypeDef",
     "SavingsPlansPurchaseRecommendationSummaryTypeDef",
     "SavingsPlansSavingsTypeDef",
@@ -168,14 +170,15 @@
     "GetSavingsPlansUtilizationDetailsRequestRequestTypeDef",
     "GetSavingsPlansUtilizationRequestRequestTypeDef",
     "GetTagsRequestRequestTypeDef",
     "GroupTypeDef",
     "ReservationUtilizationGroupTypeDef",
     "GetRightsizingRecommendationRequestRequestTypeDef",
     "InstanceDetailsTypeDef",
+    "RecommendationDetailDataTypeDef",
     "SavingsPlansCoverageTypeDef",
     "SavingsPlansPurchaseRecommendationDetailTypeDef",
     "SavingsPlansUtilizationAggregatesTypeDef",
     "SavingsPlansUtilizationByTimeTypeDef",
     "SavingsPlansUtilizationDetailTypeDef",
     "UpdateCostAllocationTagsStatusResponseTypeDef",
     "CreateAnomalySubscriptionRequestRequestTypeDef",
@@ -189,14 +192,15 @@
     "GetUsageForecastResponseTypeDef",
     "ReservationCoverageGroupTypeDef",
     "ResourceUtilizationTypeDef",
     "GetReservationPurchaseRecommendationRequestRequestTypeDef",
     "ResultByTimeTypeDef",
     "UtilizationByTimeTypeDef",
     "ReservationPurchaseRecommendationDetailTypeDef",
+    "GetSavingsPlanPurchaseRecommendationDetailsResponseTypeDef",
     "GetSavingsPlansCoverageResponseTypeDef",
     "SavingsPlansPurchaseRecommendationTypeDef",
     "GetSavingsPlansUtilizationResponseTypeDef",
     "GetSavingsPlansUtilizationDetailsResponseTypeDef",
     "DescribeCostCategoryDefinitionResponseTypeDef",
     "CoverageByTimeTypeDef",
     "CurrentInstanceTypeDef",
@@ -742,14 +746,21 @@
         "EstimatedTotalMonthlySavingsAmount": str,
         "SavingsCurrencyCode": str,
         "SavingsPercentage": str,
     },
     total=False,
 )
 
+GetSavingsPlanPurchaseRecommendationDetailsRequestRequestTypeDef = TypedDict(
+    "GetSavingsPlanPurchaseRecommendationDetailsRequestRequestTypeDef",
+    {
+        "RecommendationDetailId": str,
+    },
+)
+
 _RequiredGetSavingsPlansPurchaseRecommendationRequestRequestTypeDef = TypedDict(
     "_RequiredGetSavingsPlansPurchaseRecommendationRequestRequestTypeDef",
     {
         "SavingsPlansType": SupportedSavingsPlansTypeType,
         "TermInYears": TermInYearsType,
         "PaymentOption": PaymentOptionType,
         "LookbackPeriodInDays": LookbackPeriodInDaysType,
@@ -856,14 +867,26 @@
     "ProvideAnomalyFeedbackRequestRequestTypeDef",
     {
         "AnomalyId": str,
         "Feedback": AnomalyFeedbackTypeType,
     },
 )
 
+RecommendationDetailHourlyMetricsTypeDef = TypedDict(
+    "RecommendationDetailHourlyMetricsTypeDef",
+    {
+        "StartTime": str,
+        "EstimatedOnDemandCost": str,
+        "CurrentCoverage": str,
+        "EstimatedCoverage": str,
+        "EstimatedNewCommitmentUtilization": str,
+    },
+    total=False,
+)
+
 ReservationPurchaseRecommendationSummaryTypeDef = TypedDict(
     "ReservationPurchaseRecommendationSummaryTypeDef",
     {
         "TotalEstimatedMonthlySavingsAmount": str,
         "TotalEstimatedMonthlySavingsPercentage": str,
         "CurrencyCode": str,
     },
@@ -1753,14 +1776,50 @@
         "RedshiftInstanceDetails": RedshiftInstanceDetailsTypeDef,
         "ElastiCacheInstanceDetails": ElastiCacheInstanceDetailsTypeDef,
         "ESInstanceDetails": ESInstanceDetailsTypeDef,
     },
     total=False,
 )
 
+RecommendationDetailDataTypeDef = TypedDict(
+    "RecommendationDetailDataTypeDef",
+    {
+        "AccountScope": AccountScopeType,
+        "LookbackPeriodInDays": LookbackPeriodInDaysType,
+        "SavingsPlansType": SupportedSavingsPlansTypeType,
+        "TermInYears": TermInYearsType,
+        "PaymentOption": PaymentOptionType,
+        "AccountId": str,
+        "CurrencyCode": str,
+        "InstanceFamily": str,
+        "Region": str,
+        "OfferingId": str,
+        "GenerationTimestamp": str,
+        "LatestUsageTimestamp": str,
+        "CurrentAverageHourlyOnDemandSpend": str,
+        "CurrentMaximumHourlyOnDemandSpend": str,
+        "CurrentMinimumHourlyOnDemandSpend": str,
+        "EstimatedAverageUtilization": str,
+        "EstimatedMonthlySavingsAmount": str,
+        "EstimatedOnDemandCost": str,
+        "EstimatedOnDemandCostWithCurrentCommitment": str,
+        "EstimatedROI": str,
+        "EstimatedSPCost": str,
+        "EstimatedSavingsAmount": str,
+        "EstimatedSavingsPercentage": str,
+        "ExistingHourlyCommitment": str,
+        "HourlyCommitmentToPurchase": str,
+        "UpfrontCost": str,
+        "CurrentAverageCoverage": str,
+        "EstimatedAverageCoverage": str,
+        "MetricsOverLookbackPeriod": List[RecommendationDetailHourlyMetricsTypeDef],
+    },
+    total=False,
+)
+
 SavingsPlansCoverageTypeDef = TypedDict(
     "SavingsPlansCoverageTypeDef",
     {
         "Attributes": Dict[str, str],
         "Coverage": SavingsPlansCoverageDataTypeDef,
         "TimePeriod": DateIntervalTypeDef,
     },
@@ -1782,14 +1841,15 @@
         "EstimatedSavingsPercentage": str,
         "HourlyCommitmentToPurchase": str,
         "EstimatedAverageUtilization": str,
         "EstimatedMonthlySavingsAmount": str,
         "CurrentMinimumHourlyOnDemandSpend": str,
         "CurrentMaximumHourlyOnDemandSpend": str,
         "CurrentAverageHourlyOnDemandSpend": str,
+        "RecommendationDetailId": str,
     },
     total=False,
 )
 
 _RequiredSavingsPlansUtilizationAggregatesTypeDef = TypedDict(
     "_RequiredSavingsPlansUtilizationAggregatesTypeDef",
     {
@@ -2092,14 +2152,23 @@
         "EstimatedReservationCostForLookbackPeriod": str,
         "UpfrontCost": str,
         "RecurringStandardMonthlyCost": str,
     },
     total=False,
 )
 
+GetSavingsPlanPurchaseRecommendationDetailsResponseTypeDef = TypedDict(
+    "GetSavingsPlanPurchaseRecommendationDetailsResponseTypeDef",
+    {
+        "RecommendationDetailId": str,
+        "RecommendationDetailData": RecommendationDetailDataTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 GetSavingsPlansCoverageResponseTypeDef = TypedDict(
     "GetSavingsPlansCoverageResponseTypeDef",
     {
         "SavingsPlansCoverages": List[SavingsPlansCoverageTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
```

### Comparing `types-aiobotocore-ce-2.5.2.post3/types_aiobotocore_ce/type_defs.pyi` & `types-aiobotocore-ce-2.5.4/types_aiobotocore_ce/type_defs.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -99,23 +99,25 @@
     "SortDefinitionTypeDef",
     "MetricValueTypeDef",
     "ReservationPurchaseRecommendationMetadataTypeDef",
     "ReservationAggregatesTypeDef",
     "RightsizingRecommendationConfigurationTypeDef",
     "RightsizingRecommendationMetadataTypeDef",
     "RightsizingRecommendationSummaryTypeDef",
+    "GetSavingsPlanPurchaseRecommendationDetailsRequestRequestTypeDef",
     "GetSavingsPlansPurchaseRecommendationRequestRequestTypeDef",
     "SavingsPlansPurchaseRecommendationMetadataTypeDef",
     "RDSInstanceDetailsTypeDef",
     "RedshiftInstanceDetailsTypeDef",
     "ListCostAllocationTagsRequestRequestTypeDef",
     "ListCostCategoryDefinitionsRequestRequestTypeDef",
     "ListSavingsPlansPurchaseRecommendationGenerationRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
     "ProvideAnomalyFeedbackRequestRequestTypeDef",
+    "RecommendationDetailHourlyMetricsTypeDef",
     "ReservationPurchaseRecommendationSummaryTypeDef",
     "TerminateRecommendationDetailTypeDef",
     "SavingsPlansAmortizedCommitmentTypeDef",
     "SavingsPlansCoverageDataTypeDef",
     "SavingsPlansDetailsTypeDef",
     "SavingsPlansPurchaseRecommendationSummaryTypeDef",
     "SavingsPlansSavingsTypeDef",
@@ -167,14 +169,15 @@
     "GetSavingsPlansUtilizationDetailsRequestRequestTypeDef",
     "GetSavingsPlansUtilizationRequestRequestTypeDef",
     "GetTagsRequestRequestTypeDef",
     "GroupTypeDef",
     "ReservationUtilizationGroupTypeDef",
     "GetRightsizingRecommendationRequestRequestTypeDef",
     "InstanceDetailsTypeDef",
+    "RecommendationDetailDataTypeDef",
     "SavingsPlansCoverageTypeDef",
     "SavingsPlansPurchaseRecommendationDetailTypeDef",
     "SavingsPlansUtilizationAggregatesTypeDef",
     "SavingsPlansUtilizationByTimeTypeDef",
     "SavingsPlansUtilizationDetailTypeDef",
     "UpdateCostAllocationTagsStatusResponseTypeDef",
     "CreateAnomalySubscriptionRequestRequestTypeDef",
@@ -188,14 +191,15 @@
     "GetUsageForecastResponseTypeDef",
     "ReservationCoverageGroupTypeDef",
     "ResourceUtilizationTypeDef",
     "GetReservationPurchaseRecommendationRequestRequestTypeDef",
     "ResultByTimeTypeDef",
     "UtilizationByTimeTypeDef",
     "ReservationPurchaseRecommendationDetailTypeDef",
+    "GetSavingsPlanPurchaseRecommendationDetailsResponseTypeDef",
     "GetSavingsPlansCoverageResponseTypeDef",
     "SavingsPlansPurchaseRecommendationTypeDef",
     "GetSavingsPlansUtilizationResponseTypeDef",
     "GetSavingsPlansUtilizationDetailsResponseTypeDef",
     "DescribeCostCategoryDefinitionResponseTypeDef",
     "CoverageByTimeTypeDef",
     "CurrentInstanceTypeDef",
@@ -729,14 +733,21 @@
         "EstimatedTotalMonthlySavingsAmount": str,
         "SavingsCurrencyCode": str,
         "SavingsPercentage": str,
     },
     total=False,
 )
 
+GetSavingsPlanPurchaseRecommendationDetailsRequestRequestTypeDef = TypedDict(
+    "GetSavingsPlanPurchaseRecommendationDetailsRequestRequestTypeDef",
+    {
+        "RecommendationDetailId": str,
+    },
+)
+
 _RequiredGetSavingsPlansPurchaseRecommendationRequestRequestTypeDef = TypedDict(
     "_RequiredGetSavingsPlansPurchaseRecommendationRequestRequestTypeDef",
     {
         "SavingsPlansType": SupportedSavingsPlansTypeType,
         "TermInYears": TermInYearsType,
         "PaymentOption": PaymentOptionType,
         "LookbackPeriodInDays": LookbackPeriodInDaysType,
@@ -841,14 +852,26 @@
     "ProvideAnomalyFeedbackRequestRequestTypeDef",
     {
         "AnomalyId": str,
         "Feedback": AnomalyFeedbackTypeType,
     },
 )
 
+RecommendationDetailHourlyMetricsTypeDef = TypedDict(
+    "RecommendationDetailHourlyMetricsTypeDef",
+    {
+        "StartTime": str,
+        "EstimatedOnDemandCost": str,
+        "CurrentCoverage": str,
+        "EstimatedCoverage": str,
+        "EstimatedNewCommitmentUtilization": str,
+    },
+    total=False,
+)
+
 ReservationPurchaseRecommendationSummaryTypeDef = TypedDict(
     "ReservationPurchaseRecommendationSummaryTypeDef",
     {
         "TotalEstimatedMonthlySavingsAmount": str,
         "TotalEstimatedMonthlySavingsPercentage": str,
         "CurrencyCode": str,
     },
@@ -1698,14 +1721,50 @@
         "RedshiftInstanceDetails": RedshiftInstanceDetailsTypeDef,
         "ElastiCacheInstanceDetails": ElastiCacheInstanceDetailsTypeDef,
         "ESInstanceDetails": ESInstanceDetailsTypeDef,
     },
     total=False,
 )
 
+RecommendationDetailDataTypeDef = TypedDict(
+    "RecommendationDetailDataTypeDef",
+    {
+        "AccountScope": AccountScopeType,
+        "LookbackPeriodInDays": LookbackPeriodInDaysType,
+        "SavingsPlansType": SupportedSavingsPlansTypeType,
+        "TermInYears": TermInYearsType,
+        "PaymentOption": PaymentOptionType,
+        "AccountId": str,
+        "CurrencyCode": str,
+        "InstanceFamily": str,
+        "Region": str,
+        "OfferingId": str,
+        "GenerationTimestamp": str,
+        "LatestUsageTimestamp": str,
+        "CurrentAverageHourlyOnDemandSpend": str,
+        "CurrentMaximumHourlyOnDemandSpend": str,
+        "CurrentMinimumHourlyOnDemandSpend": str,
+        "EstimatedAverageUtilization": str,
+        "EstimatedMonthlySavingsAmount": str,
+        "EstimatedOnDemandCost": str,
+        "EstimatedOnDemandCostWithCurrentCommitment": str,
+        "EstimatedROI": str,
+        "EstimatedSPCost": str,
+        "EstimatedSavingsAmount": str,
+        "EstimatedSavingsPercentage": str,
+        "ExistingHourlyCommitment": str,
+        "HourlyCommitmentToPurchase": str,
+        "UpfrontCost": str,
+        "CurrentAverageCoverage": str,
+        "EstimatedAverageCoverage": str,
+        "MetricsOverLookbackPeriod": List[RecommendationDetailHourlyMetricsTypeDef],
+    },
+    total=False,
+)
+
 SavingsPlansCoverageTypeDef = TypedDict(
     "SavingsPlansCoverageTypeDef",
     {
         "Attributes": Dict[str, str],
         "Coverage": SavingsPlansCoverageDataTypeDef,
         "TimePeriod": DateIntervalTypeDef,
     },
@@ -1727,14 +1786,15 @@
         "EstimatedSavingsPercentage": str,
         "HourlyCommitmentToPurchase": str,
         "EstimatedAverageUtilization": str,
         "EstimatedMonthlySavingsAmount": str,
         "CurrentMinimumHourlyOnDemandSpend": str,
         "CurrentMaximumHourlyOnDemandSpend": str,
         "CurrentAverageHourlyOnDemandSpend": str,
+        "RecommendationDetailId": str,
     },
     total=False,
 )
 
 _RequiredSavingsPlansUtilizationAggregatesTypeDef = TypedDict(
     "_RequiredSavingsPlansUtilizationAggregatesTypeDef",
     {
@@ -2023,14 +2083,23 @@
         "EstimatedReservationCostForLookbackPeriod": str,
         "UpfrontCost": str,
         "RecurringStandardMonthlyCost": str,
     },
     total=False,
 )
 
+GetSavingsPlanPurchaseRecommendationDetailsResponseTypeDef = TypedDict(
+    "GetSavingsPlanPurchaseRecommendationDetailsResponseTypeDef",
+    {
+        "RecommendationDetailId": str,
+        "RecommendationDetailData": RecommendationDetailDataTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 GetSavingsPlansCoverageResponseTypeDef = TypedDict(
     "GetSavingsPlansCoverageResponseTypeDef",
     {
         "SavingsPlansCoverages": List[SavingsPlansCoverageTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
```

### Comparing `types-aiobotocore-ce-2.5.2.post3/types_aiobotocore_ce.egg-info/PKG-INFO` & `types-aiobotocore-ce-2.5.4/types_aiobotocore_ce.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-ce
-Version: 2.5.2.post3
-Summary: Type annotations for aiobotocore.CostExplorer 2.5.2 service generated with mypy-boto3-builder 7.17.2
+Version: 2.5.4
+Summary: Type annotations for aiobotocore.CostExplorer 2.5.4 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ce/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-ce.svg?color=blue)](https://pypi.org/project/types-aiobotocore-ce)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ce/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-ce)](https://pepy.tech/project/types-aiobotocore-ce)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.CostExplorer 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ce.html#CostExplorer)
+[aiobotocore.CostExplorer 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ce.html#CostExplorer)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-ce-2.5.2.post3/types_aiobotocore_ce.egg-info/SOURCES.txt` & `types-aiobotocore-ce-2.5.4/types_aiobotocore_ce.egg-info/SOURCES.txt`

 * *Files identical despite different names*


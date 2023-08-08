# Comparing `tmp/types-aiobotocore-sagemaker-2.5.2.post2.tar.gz` & `tmp/types-aiobotocore-sagemaker-2.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-sagemaker-2.5.2.post2.tar", last modified: Fri Aug  4 13:59:25 2023, max compression
+gzip compressed data, was "types-aiobotocore-sagemaker-2.5.4.tar", last modified: Tue Aug  8 01:24:23 2023, max compression
```

## Comparing `types-aiobotocore-sagemaker-2.5.2.post2.tar` & `types-aiobotocore-sagemaker-2.5.4.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:25.086643 types-aiobotocore-sagemaker-2.5.2.post2/
--rw-r--r--   0 vlad      (1000) vlad      (1000)     1070 2023-08-04 13:51:56.000000 types-aiobotocore-sagemaker-2.5.2.post2/LICENSE
--rw-r--r--   0 vlad      (1000) vlad      (1000)    26500 2023-08-04 13:59:25.086643 types-aiobotocore-sagemaker-2.5.2.post2/PKG-INFO
--rw-r--r--   0 vlad      (1000) vlad      (1000)    24974 2023-08-04 13:51:56.000000 types-aiobotocore-sagemaker-2.5.2.post2/README.md
--rw-r--r--   0 vlad      (1000) vlad      (1000)       38 2023-08-04 13:59:25.086643 types-aiobotocore-sagemaker-2.5.2.post2/setup.cfg
--rw-r--r--   0 vlad      (1000) vlad      (1000)     2086 2023-08-04 13:51:56.000000 types-aiobotocore-sagemaker-2.5.2.post2/setup.py
-drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:25.076643 types-aiobotocore-sagemaker-2.5.2.post2/types_aiobotocore_sagemaker/
--rw-r--r--   0 vlad      (1000) vlad      (1000)    18810 2023-08-04 13:51:56.000000 types-aiobotocore-sagemaker-2.5.2.post2/types_aiobotocore_sagemaker/__init__.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)    18809 2023-08-04 13:51:56.000000 types-aiobotocore-sagemaker-2.5.2.post2/types_aiobotocore_sagemaker/__init__.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)      951 2023-08-04 13:51:56.000000 types-aiobotocore-sagemaker-2.5.2.post2/types_aiobotocore_sagemaker/__main__.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)   274298 2023-08-04 13:52:02.000000 types-aiobotocore-sagemaker-2.5.2.post2/types_aiobotocore_sagemaker/client.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)   273903 2023-08-04 13:52:01.000000 types-aiobotocore-sagemaker-2.5.2.post2/types_aiobotocore_sagemaker/client.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)    58126 2023-08-04 13:52:05.000000 types-aiobotocore-sagemaker-2.5.2.post2/types_aiobotocore_sagemaker/literals.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)    58124 2023-08-04 13:52:04.000000 types-aiobotocore-sagemaker-2.5.2.post2/types_aiobotocore_sagemaker/literals.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)   101540 2023-08-04 13:52:03.000000 types-aiobotocore-sagemaker-2.5.2.post2/types_aiobotocore_sagemaker/paginator.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)   101468 2023-08-04 13:52:03.000000 types-aiobotocore-sagemaker-2.5.2.post2/types_aiobotocore_sagemaker/paginator.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:51:56.000000 types-aiobotocore-sagemaker-2.5.2.post2/types_aiobotocore_sagemaker/py.typed
--rw-r--r--   0 vlad      (1000) vlad      (1000)   500242 2023-08-04 13:52:22.000000 types-aiobotocore-sagemaker-2.5.2.post2/types_aiobotocore_sagemaker/type_defs.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)   499609 2023-08-04 13:52:13.000000 types-aiobotocore-sagemaker-2.5.2.post2/types_aiobotocore_sagemaker/type_defs.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)       65 2023-08-04 13:51:56.000000 types-aiobotocore-sagemaker-2.5.2.post2/types_aiobotocore_sagemaker/version.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)    14121 2023-08-04 13:52:03.000000 types-aiobotocore-sagemaker-2.5.2.post2/types_aiobotocore_sagemaker/waiter.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)    14108 2023-08-04 13:52:03.000000 types-aiobotocore-sagemaker-2.5.2.post2/types_aiobotocore_sagemaker/waiter.pyi
-drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:25.086643 types-aiobotocore-sagemaker-2.5.2.post2/types_aiobotocore_sagemaker.egg-info/
--rw-r--r--   0 vlad      (1000) vlad      (1000)    26500 2023-08-04 13:59:24.000000 types-aiobotocore-sagemaker-2.5.2.post2/types_aiobotocore_sagemaker.egg-info/PKG-INFO
--rw-r--r--   0 vlad      (1000) vlad      (1000)      928 2023-08-04 13:59:25.000000 types-aiobotocore-sagemaker-2.5.2.post2/types_aiobotocore_sagemaker.egg-info/SOURCES.txt
--rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:24.000000 types-aiobotocore-sagemaker-2.5.2.post2/types_aiobotocore_sagemaker.egg-info/dependency_links.txt
--rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:24.000000 types-aiobotocore-sagemaker-2.5.2.post2/types_aiobotocore_sagemaker.egg-info/not-zip-safe
--rw-r--r--   0 vlad      (1000) vlad      (1000)       52 2023-08-04 13:59:24.000000 types-aiobotocore-sagemaker-2.5.2.post2/types_aiobotocore_sagemaker.egg-info/requires.txt
--rw-r--r--   0 vlad      (1000) vlad      (1000)       28 2023-08-04 13:59:24.000000 types-aiobotocore-sagemaker-2.5.2.post2/types_aiobotocore_sagemaker.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:24:23.286773 types-aiobotocore-sagemaker-2.5.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-08 01:20:10.000000 types-aiobotocore-sagemaker-2.5.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    26494 2023-08-08 01:24:23.282773 types-aiobotocore-sagemaker-2.5.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    24974 2023-08-08 01:20:10.000000 types-aiobotocore-sagemaker-2.5.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-08 01:24:23.286773 types-aiobotocore-sagemaker-2.5.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2080 2023-08-08 01:20:10.000000 types-aiobotocore-sagemaker-2.5.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:24:23.282773 types-aiobotocore-sagemaker-2.5.4/types_aiobotocore_sagemaker/
+-rw-r--r--   0 runner    (1001) docker     (123)    18810 2023-08-08 01:20:10.000000 types-aiobotocore-sagemaker-2.5.4/types_aiobotocore_sagemaker/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18809 2023-08-08 01:20:10.000000 types-aiobotocore-sagemaker-2.5.4/types_aiobotocore_sagemaker/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      939 2023-08-08 01:20:10.000000 types-aiobotocore-sagemaker-2.5.4/types_aiobotocore_sagemaker/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   273356 2023-08-08 01:20:12.000000 types-aiobotocore-sagemaker-2.5.4/types_aiobotocore_sagemaker/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)   272962 2023-08-08 01:20:11.000000 types-aiobotocore-sagemaker-2.5.4/types_aiobotocore_sagemaker/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    58004 2023-08-08 01:20:13.000000 types-aiobotocore-sagemaker-2.5.4/types_aiobotocore_sagemaker/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    58002 2023-08-08 01:20:13.000000 types-aiobotocore-sagemaker-2.5.4/types_aiobotocore_sagemaker/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)   101540 2023-08-08 01:20:12.000000 types-aiobotocore-sagemaker-2.5.4/types_aiobotocore_sagemaker/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)   101468 2023-08-08 01:20:12.000000 types-aiobotocore-sagemaker-2.5.4/types_aiobotocore_sagemaker/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 01:20:10.000000 types-aiobotocore-sagemaker-2.5.4/types_aiobotocore_sagemaker/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)   496756 2023-08-08 01:20:25.000000 types-aiobotocore-sagemaker-2.5.4/types_aiobotocore_sagemaker/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)   496125 2023-08-08 01:20:20.000000 types-aiobotocore-sagemaker-2.5.4/types_aiobotocore_sagemaker/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-08-08 01:20:10.000000 types-aiobotocore-sagemaker-2.5.4/types_aiobotocore_sagemaker/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14121 2023-08-08 01:20:13.000000 types-aiobotocore-sagemaker-2.5.4/types_aiobotocore_sagemaker/waiter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14108 2023-08-08 01:20:12.000000 types-aiobotocore-sagemaker-2.5.4/types_aiobotocore_sagemaker/waiter.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:24:23.282773 types-aiobotocore-sagemaker-2.5.4/types_aiobotocore_sagemaker.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    26494 2023-08-08 01:24:23.000000 types-aiobotocore-sagemaker-2.5.4/types_aiobotocore_sagemaker.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      928 2023-08-08 01:24:23.000000 types-aiobotocore-sagemaker-2.5.4/types_aiobotocore_sagemaker.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 01:24:23.000000 types-aiobotocore-sagemaker-2.5.4/types_aiobotocore_sagemaker.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 01:24:23.000000 types-aiobotocore-sagemaker-2.5.4/types_aiobotocore_sagemaker.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-08 01:24:23.000000 types-aiobotocore-sagemaker-2.5.4/types_aiobotocore_sagemaker.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-08-08 01:24:23.000000 types-aiobotocore-sagemaker-2.5.4/types_aiobotocore_sagemaker.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-sagemaker-2.5.2.post2/LICENSE` & `types-aiobotocore-sagemaker-2.5.4/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-sagemaker-2.5.2.post2/PKG-INFO` & `types-aiobotocore-sagemaker-2.5.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-sagemaker
-Version: 2.5.2.post2
-Summary: Type annotations for aiobotocore.SageMaker 2.5.2 service generated with mypy-boto3-builder 7.17.2
+Version: 2.5.4
+Summary: Type annotations for aiobotocore.SageMaker 2.5.4 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-sagemaker.svg?color=blue)](https://pypi.org/project/types-aiobotocore-sagemaker)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-sagemaker)](https://pepy.tech/project/types-aiobotocore-sagemaker)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.SageMaker 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker)
+[aiobotocore.SageMaker 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-sagemaker-2.5.2.post2/README.md` & `types-aiobotocore-sagemaker-2.5.4/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-sagemaker.svg?color=blue)](https://pypi.org/project/types-aiobotocore-sagemaker)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-sagemaker)](https://pepy.tech/project/types-aiobotocore-sagemaker)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.SageMaker 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker)
+[aiobotocore.SageMaker 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-sagemaker-2.5.2.post2/setup.py` & `types-aiobotocore-sagemaker-2.5.4/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-sagemaker",
-    version="2.5.2.post2",
+    version="2.5.4",
     packages=["types_aiobotocore_sagemaker"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.SageMaker 2.5.2 service generated with mypy-boto3-builder"
+        "Type annotations for aiobotocore.SageMaker 2.5.4 service generated with mypy-boto3-builder"
         " 7.17.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
```

### Comparing `types-aiobotocore-sagemaker-2.5.2.post2/types_aiobotocore_sagemaker/__init__.py` & `types-aiobotocore-sagemaker-2.5.4/types_aiobotocore_sagemaker/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-sagemaker-2.5.2.post2/types_aiobotocore_sagemaker/__init__.pyi` & `types-aiobotocore-sagemaker-2.5.4/types_aiobotocore_sagemaker/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-sagemaker-2.5.2.post2/types_aiobotocore_sagemaker/__main__.py` & `types-aiobotocore-sagemaker-2.5.4/types_aiobotocore_sagemaker/__main__.py`

 * *Files 15% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.SageMaker 2.5.2\nVersion:         2.5.2.post2\nBuilder"
-        " version: 7.17.2\nDocs:           "
+        "Type annotations for aiobotocore.SageMaker 2.5.4\nVersion:         2.5.4\nBuilder version:"
+        " 7.17.2\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker\nOther"
         " services:  https://pypi.org/project/boto3-stubs/\nChangelog:      "
         " https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("2.5.2.post2")
+    print("2.5.4")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `types-aiobotocore-sagemaker-2.5.2.post2/types_aiobotocore_sagemaker/client.py` & `types-aiobotocore-sagemaker-2.5.4/types_aiobotocore_sagemaker/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -371,15 +371,14 @@
     FeatureDefinitionTypeDef,
     FeatureParameterTypeDef,
     FlowDefinitionOutputConfigTypeDef,
     GetDeviceFleetReportResponseTypeDef,
     GetLineageGroupPolicyResponseTypeDef,
     GetModelPackageGroupPolicyOutputTypeDef,
     GetSagemakerServicecatalogPortfolioStatusOutputTypeDef,
-    GetScalingConfigurationRecommendationResponseTypeDef,
     GetSearchSuggestionsResponseTypeDef,
     GitConfigForUpdateTypeDef,
     GitConfigTypeDef,
     HubS3StorageConfigTypeDef,
     HumanLoopActivationConfigTypeDef,
     HumanLoopConfigTypeDef,
     HumanLoopRequestSourceTypeDef,
@@ -527,15 +526,14 @@
     RenderUiTemplateResponseTypeDef,
     ResourceConfigForUpdateTypeDef,
     ResourceConfigTypeDef,
     ResourceSpecTypeDef,
     RetentionPolicyTypeDef,
     RetryPipelineExecutionResponseTypeDef,
     RetryStrategyTypeDef,
-    ScalingPolicyObjectiveTypeDef,
     SearchExpressionTypeDef,
     SearchResponseTypeDef,
     SelectiveExecutionConfigTypeDef,
     SendPipelineExecutionStepFailureResponseTypeDef,
     SendPipelineExecutionStepSuccessResponseTypeDef,
     ServiceCatalogProvisioningDetailsTypeDef,
     ServiceCatalogProvisioningUpdateDetailsTypeDef,
@@ -2793,30 +2791,14 @@
         """
         Gets the status of Service Catalog in SageMaker.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.get_sagemaker_servicecatalog_portfolio_status)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker/client/#get_sagemaker_servicecatalog_portfolio_status)
         """
 
-    async def get_scaling_configuration_recommendation(
-        self,
-        *,
-        InferenceRecommendationsJobName: str,
-        RecommendationId: str = ...,
-        EndpointName: str = ...,
-        TargetCpuUtilizationPerCore: int = ...,
-        ScalingPolicyObjective: ScalingPolicyObjectiveTypeDef = ...
-    ) -> GetScalingConfigurationRecommendationResponseTypeDef:
-        """
-        Starts an Amazon SageMaker Inference Recommender autoscaling recommendation job.
-
-        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.get_scaling_configuration_recommendation)
-        [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker/client/#get_scaling_configuration_recommendation)
-        """
-
     async def get_search_suggestions(
         self, *, Resource: ResourceTypeType, SuggestionQuery: SuggestionQueryTypeDef = ...
     ) -> GetSearchSuggestionsResponseTypeDef:
         """
         An auto-complete API for the search functionality in the SageMaker console.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.get_search_suggestions)
```

### Comparing `types-aiobotocore-sagemaker-2.5.2.post2/types_aiobotocore_sagemaker/client.pyi` & `types-aiobotocore-sagemaker-2.5.4/types_aiobotocore_sagemaker/client.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -371,15 +371,14 @@
     FeatureDefinitionTypeDef,
     FeatureParameterTypeDef,
     FlowDefinitionOutputConfigTypeDef,
     GetDeviceFleetReportResponseTypeDef,
     GetLineageGroupPolicyResponseTypeDef,
     GetModelPackageGroupPolicyOutputTypeDef,
     GetSagemakerServicecatalogPortfolioStatusOutputTypeDef,
-    GetScalingConfigurationRecommendationResponseTypeDef,
     GetSearchSuggestionsResponseTypeDef,
     GitConfigForUpdateTypeDef,
     GitConfigTypeDef,
     HubS3StorageConfigTypeDef,
     HumanLoopActivationConfigTypeDef,
     HumanLoopConfigTypeDef,
     HumanLoopRequestSourceTypeDef,
@@ -527,15 +526,14 @@
     RenderUiTemplateResponseTypeDef,
     ResourceConfigForUpdateTypeDef,
     ResourceConfigTypeDef,
     ResourceSpecTypeDef,
     RetentionPolicyTypeDef,
     RetryPipelineExecutionResponseTypeDef,
     RetryStrategyTypeDef,
-    ScalingPolicyObjectiveTypeDef,
     SearchExpressionTypeDef,
     SearchResponseTypeDef,
     SelectiveExecutionConfigTypeDef,
     SendPipelineExecutionStepFailureResponseTypeDef,
     SendPipelineExecutionStepSuccessResponseTypeDef,
     ServiceCatalogProvisioningDetailsTypeDef,
     ServiceCatalogProvisioningUpdateDetailsTypeDef,
@@ -2616,29 +2614,14 @@
     ) -> GetSagemakerServicecatalogPortfolioStatusOutputTypeDef:
         """
         Gets the status of Service Catalog in SageMaker.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.get_sagemaker_servicecatalog_portfolio_status)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker/client/#get_sagemaker_servicecatalog_portfolio_status)
         """
-    async def get_scaling_configuration_recommendation(
-        self,
-        *,
-        InferenceRecommendationsJobName: str,
-        RecommendationId: str = ...,
-        EndpointName: str = ...,
-        TargetCpuUtilizationPerCore: int = ...,
-        ScalingPolicyObjective: ScalingPolicyObjectiveTypeDef = ...
-    ) -> GetScalingConfigurationRecommendationResponseTypeDef:
-        """
-        Starts an Amazon SageMaker Inference Recommender autoscaling recommendation job.
-
-        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.get_scaling_configuration_recommendation)
-        [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker/client/#get_scaling_configuration_recommendation)
-        """
     async def get_search_suggestions(
         self, *, Resource: ResourceTypeType, SuggestionQuery: SuggestionQueryTypeDef = ...
     ) -> GetSearchSuggestionsResponseTypeDef:
         """
         An auto-complete API for the search functionality in the SageMaker console.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.get_search_suggestions)
```

### Comparing `types-aiobotocore-sagemaker-2.5.2.post2/types_aiobotocore_sagemaker/literals.py` & `types-aiobotocore-sagemaker-2.5.4/types_aiobotocore_sagemaker/literals.py`

 * *Files 0% similar despite different names*

```diff
@@ -315,15 +315,14 @@
     "SortPipelinesByType",
     "SortTrialComponentsByType",
     "SortTrialsByType",
     "SpaceSortKeyType",
     "SpaceStatusType",
     "SplitTypeType",
     "StageStatusType",
-    "StatisticType",
     "StepStatusType",
     "StudioLifecycleConfigAppTypeType",
     "StudioLifecycleConfigSortKeyType",
     "TableFormatType",
     "TargetDeviceType",
     "TargetPlatformAcceleratorType",
     "TargetPlatformArchType",
@@ -1274,15 +1273,14 @@
     "FAILED",
     "INPROGRESS",
     "READYTODEPLOY",
     "STARTING",
     "STOPPED",
     "STOPPING",
 ]
-StatisticType = Literal["Average", "Maximum", "Minimum", "SampleCount", "Sum"]
 StepStatusType = Literal["Executing", "Failed", "Starting", "Stopped", "Stopping", "Succeeded"]
 StudioLifecycleConfigAppTypeType = Literal["JupyterServer", "KernelGateway"]
 StudioLifecycleConfigSortKeyType = Literal["CreationTime", "LastModifiedTime", "Name"]
 TableFormatType = Literal["Glue", "Iceberg"]
 TargetDeviceType = Literal[
     "aisage",
     "amba_cv2",
@@ -1369,15 +1367,14 @@
     "ml.p2.8xlarge",
     "ml.p2.xlarge",
     "ml.p3.16xlarge",
     "ml.p3.2xlarge",
     "ml.p3.8xlarge",
     "ml.p3dn.24xlarge",
     "ml.p4d.24xlarge",
-    "ml.p5.48xlarge",
     "ml.trn1.2xlarge",
     "ml.trn1.32xlarge",
     "ml.trn1n.32xlarge",
 ]
 TrainingJobCompletedOrStoppedWaiterName = Literal["training_job_completed_or_stopped"]
 TrainingJobEarlyStoppingTypeType = Literal["Auto", "Off"]
 TrainingJobSortByOptionsType = Literal[
```

### Comparing `types-aiobotocore-sagemaker-2.5.2.post2/types_aiobotocore_sagemaker/literals.pyi` & `types-aiobotocore-sagemaker-2.5.4/types_aiobotocore_sagemaker/literals.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -314,15 +314,14 @@
     "SortPipelinesByType",
     "SortTrialComponentsByType",
     "SortTrialsByType",
     "SpaceSortKeyType",
     "SpaceStatusType",
     "SplitTypeType",
     "StageStatusType",
-    "StatisticType",
     "StepStatusType",
     "StudioLifecycleConfigAppTypeType",
     "StudioLifecycleConfigSortKeyType",
     "TableFormatType",
     "TargetDeviceType",
     "TargetPlatformAcceleratorType",
     "TargetPlatformArchType",
@@ -1272,15 +1271,14 @@
     "FAILED",
     "INPROGRESS",
     "READYTODEPLOY",
     "STARTING",
     "STOPPED",
     "STOPPING",
 ]
-StatisticType = Literal["Average", "Maximum", "Minimum", "SampleCount", "Sum"]
 StepStatusType = Literal["Executing", "Failed", "Starting", "Stopped", "Stopping", "Succeeded"]
 StudioLifecycleConfigAppTypeType = Literal["JupyterServer", "KernelGateway"]
 StudioLifecycleConfigSortKeyType = Literal["CreationTime", "LastModifiedTime", "Name"]
 TableFormatType = Literal["Glue", "Iceberg"]
 TargetDeviceType = Literal[
     "aisage",
     "amba_cv2",
@@ -1367,15 +1365,14 @@
     "ml.p2.8xlarge",
     "ml.p2.xlarge",
     "ml.p3.16xlarge",
     "ml.p3.2xlarge",
     "ml.p3.8xlarge",
     "ml.p3dn.24xlarge",
     "ml.p4d.24xlarge",
-    "ml.p5.48xlarge",
     "ml.trn1.2xlarge",
     "ml.trn1.32xlarge",
     "ml.trn1n.32xlarge",
 ]
 TrainingJobCompletedOrStoppedWaiterName = Literal["training_job_completed_or_stopped"]
 TrainingJobEarlyStoppingTypeType = Literal["Auto", "Off"]
 TrainingJobSortByOptionsType = Literal[
```

### Comparing `types-aiobotocore-sagemaker-2.5.2.post2/types_aiobotocore_sagemaker/paginator.py` & `types-aiobotocore-sagemaker-2.5.4/types_aiobotocore_sagemaker/paginator.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-sagemaker-2.5.2.post2/types_aiobotocore_sagemaker/paginator.pyi` & `types-aiobotocore-sagemaker-2.5.4/types_aiobotocore_sagemaker/paginator.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-sagemaker-2.5.2.post2/types_aiobotocore_sagemaker/type_defs.py` & `types-aiobotocore-sagemaker-2.5.4/types_aiobotocore_sagemaker/type_defs.py`

 * *Files 1% similar despite different names*

```diff
@@ -219,15 +219,14 @@
     SortPipelinesByType,
     SortTrialComponentsByType,
     SortTrialsByType,
     SpaceSortKeyType,
     SpaceStatusType,
     SplitTypeType,
     StageStatusType,
-    StatisticType,
     StepStatusType,
     StudioLifecycleConfigAppTypeType,
     StudioLifecycleConfigSortKeyType,
     TableFormatType,
     TargetDeviceType,
     TargetPlatformAcceleratorType,
     TargetPlatformArchType,
@@ -381,15 +380,14 @@
     "TrialComponentParameterValueTypeDef",
     "TrialComponentStatusTypeDef",
     "OidcConfigTypeDef",
     "SourceIpConfigTypeDef",
     "WorkforceVpcConfigRequestTypeDef",
     "NotificationConfigurationTypeDef",
     "CustomImageTypeDef",
-    "CustomizedMetricSpecificationTypeDef",
     "DataCaptureConfigSummaryTypeDef",
     "DataCatalogConfigTypeDef",
     "MonitoringConstraintsResourceTypeDef",
     "MonitoringStatisticsResourceTypeDef",
     "EndpointInputTypeDef",
     "FileSystemDataSourceTypeDef",
     "S3DataSourceTypeDef",
@@ -558,16 +556,14 @@
     "FileSystemConfigTypeDef",
     "FilterTypeDef",
     "FinalHyperParameterTuningJobObjectiveMetricTypeDef",
     "FlowDefinitionSummaryTypeDef",
     "GetDeviceFleetReportRequestRequestTypeDef",
     "GetLineageGroupPolicyRequestRequestTypeDef",
     "GetModelPackageGroupPolicyInputRequestTypeDef",
-    "ScalingPolicyObjectiveTypeDef",
-    "ScalingPolicyMetricTypeDef",
     "PropertyNameSuggestionTypeDef",
     "GitConfigForUpdateTypeDef",
     "HubContentInfoTypeDef",
     "HubInfoTypeDef",
     "HumanLoopActivationConditionsConfigTypeDef",
     "UiConfigTypeDef",
     "HumanTaskUiSummaryTypeDef",
@@ -627,15 +623,14 @@
     "ListTrainingJobsForHyperParameterTuningJobRequestRequestTypeDef",
     "TransformJobSummaryTypeDef",
     "ListUserProfilesRequestRequestTypeDef",
     "UserProfileDetailsTypeDef",
     "ListWorkforcesRequestRequestTypeDef",
     "ListWorkteamsRequestRequestTypeDef",
     "OidcMemberDefinitionTypeDef",
-    "PredefinedMetricSpecificationTypeDef",
     "MonitoringGroundTruthS3InputTypeDef",
     "ModelDashboardEndpointTypeDef",
     "ModelDashboardIndicatorActionTypeDef",
     "S3ModelDataSourceTypeDef",
     "RealTimeInferenceConfigTypeDef",
     "ModelInputTypeDef",
     "ModelLatencyThresholdTypeDef",
@@ -1028,15 +1023,14 @@
     "EndpointOutputConfigurationTypeDef",
     "EndpointPerformanceTypeDef",
     "ListEndpointsOutputTypeDef",
     "ModelConfigurationTypeDef",
     "NestedFiltersTypeDef",
     "HyperParameterTrainingJobSummaryTypeDef",
     "ListFlowDefinitionsResponseTypeDef",
-    "GetScalingConfigurationRecommendationRequestRequestTypeDef",
     "GetSearchSuggestionsResponseTypeDef",
     "UpdateCodeRepositoryInputRequestTypeDef",
     "ListHubContentVersionsResponseTypeDef",
     "ListHubContentsResponseTypeDef",
     "ListHubsResponseTypeDef",
     "HumanLoopActivationConfigTypeDef",
     "ListHumanTaskUisResponseTypeDef",
@@ -1146,15 +1140,14 @@
     "ListProjectsOutputTypeDef",
     "ListResourceCatalogsResponseTypeDef",
     "ListSpacesResponseTypeDef",
     "ListStudioLifecycleConfigsResponseTypeDef",
     "ListTransformJobsResponseTypeDef",
     "ListUserProfilesResponseTypeDef",
     "MemberDefinitionTypeDef",
-    "MetricSpecificationTypeDef",
     "MonitoringAlertActionsTypeDef",
     "ModelDataSourceTypeDef",
     "ModelInfrastructureConfigTypeDef",
     "ModelPackageContainerDefinitionTypeDef",
     "RecommendationJobStoppingConditionsTypeDef",
     "ModelMetadataSearchExpressionTypeDef",
     "ModelPackageStatusDetailsTypeDef",
@@ -1257,15 +1250,14 @@
     "DescribeAppImageConfigResponseTypeDef",
     "UpdateAppImageConfigRequestRequestTypeDef",
     "ListLabelingJobsForWorkteamResponseTypeDef",
     "LabelingJobInputConfigTypeDef",
     "CreateWorkteamRequestRequestTypeDef",
     "UpdateWorkteamRequestRequestTypeDef",
     "WorkteamTypeDef",
-    "TargetTrackingScalingPolicyConfigurationTypeDef",
     "MonitoringAlertSummaryTypeDef",
     "ContainerDefinitionTypeDef",
     "ModelVariantConfigSummaryTypeDef",
     "ModelVariantConfigTypeDef",
     "AdditionalInferenceSpecificationDefinitionTypeDef",
     "InferenceSpecificationTypeDef",
     "ListModelMetadataRequestListModelMetadataPaginateTypeDef",
@@ -1322,15 +1314,14 @@
     "ListTrialComponentsResponseTypeDef",
     "TrainingSpecificationTypeDef",
     "ListAppImageConfigsResponseTypeDef",
     "LabelingJobSummaryTypeDef",
     "DescribeWorkteamResponseTypeDef",
     "ListWorkteamsResponseTypeDef",
     "UpdateWorkteamResponseTypeDef",
-    "ScalingPolicyTypeDef",
     "ListMonitoringAlertsResponseTypeDef",
     "CreateModelInputRequestTypeDef",
     "DescribeModelOutputTypeDef",
     "ModelTypeDef",
     "DescribeInferenceExperimentResponseTypeDef",
     "CreateInferenceExperimentRequestRequestTypeDef",
     "StopInferenceExperimentRequestRequestTypeDef",
@@ -1367,29 +1358,27 @@
     "DescribeEndpointConfigOutputTypeDef",
     "DescribeEndpointOutputTypeDef",
     "CreateHyperParameterTuningJobRequestRequestTypeDef",
     "DescribeHyperParameterTuningJobResponseTypeDef",
     "HyperParameterTuningJobSearchEntityTypeDef",
     "ListInferenceRecommendationsJobStepsResponseTypeDef",
     "ListLabelingJobsResponseTypeDef",
-    "DynamicScalingConfigurationTypeDef",
     "BatchDescribeModelPackageOutputTypeDef",
     "CreateDataQualityJobDefinitionRequestRequestTypeDef",
     "DescribeDataQualityJobDefinitionResponseTypeDef",
     "CreateModelBiasJobDefinitionRequestRequestTypeDef",
     "DescribeModelBiasJobDefinitionResponseTypeDef",
     "CreateModelExplainabilityJobDefinitionRequestRequestTypeDef",
     "DescribeModelExplainabilityJobDefinitionResponseTypeDef",
     "CreateModelQualityJobDefinitionRequestRequestTypeDef",
     "DescribeModelQualityJobDefinitionResponseTypeDef",
     "MonitoringJobDefinitionTypeDef",
     "AlgorithmValidationProfileTypeDef",
     "ModelPackageValidationProfileTypeDef",
     "TrialComponentSourceDetailTypeDef",
-    "GetScalingConfigurationRecommendationResponseTypeDef",
     "MonitoringScheduleConfigTypeDef",
     "AlgorithmValidationSpecificationTypeDef",
     "ModelPackageValidationSpecificationTypeDef",
     "TrialComponentTypeDef",
     "CreateMonitoringScheduleRequestRequestTypeDef",
     "DescribeMonitoringScheduleResponseTypeDef",
     "ModelDashboardMonitoringScheduleTypeDef",
@@ -2970,24 +2959,14 @@
 )
 
 
 class CustomImageTypeDef(_RequiredCustomImageTypeDef, _OptionalCustomImageTypeDef):
     pass
 
 
-CustomizedMetricSpecificationTypeDef = TypedDict(
-    "CustomizedMetricSpecificationTypeDef",
-    {
-        "MetricName": str,
-        "Namespace": str,
-        "Statistic": StatisticType,
-    },
-    total=False,
-)
-
 DataCaptureConfigSummaryTypeDef = TypedDict(
     "DataCaptureConfigSummaryTypeDef",
     {
         "EnableCapture": bool,
         "CaptureStatus": CaptureStatusType,
         "CurrentSamplingPercentage": int,
         "DestinationS3Uri": str,
@@ -4934,32 +4913,14 @@
 GetModelPackageGroupPolicyInputRequestTypeDef = TypedDict(
     "GetModelPackageGroupPolicyInputRequestTypeDef",
     {
         "ModelPackageGroupName": str,
     },
 )
 
-ScalingPolicyObjectiveTypeDef = TypedDict(
-    "ScalingPolicyObjectiveTypeDef",
-    {
-        "MinInvocationsPerMinute": int,
-        "MaxInvocationsPerMinute": int,
-    },
-    total=False,
-)
-
-ScalingPolicyMetricTypeDef = TypedDict(
-    "ScalingPolicyMetricTypeDef",
-    {
-        "InvocationsPerInstance": int,
-        "ModelLatency": int,
-    },
-    total=False,
-)
-
 PropertyNameSuggestionTypeDef = TypedDict(
     "PropertyNameSuggestionTypeDef",
     {
         "PropertyName": str,
     },
     total=False,
 )
@@ -6020,22 +5981,14 @@
 OidcMemberDefinitionTypeDef = TypedDict(
     "OidcMemberDefinitionTypeDef",
     {
         "Groups": Sequence[str],
     },
 )
 
-PredefinedMetricSpecificationTypeDef = TypedDict(
-    "PredefinedMetricSpecificationTypeDef",
-    {
-        "PredefinedMetricType": str,
-    },
-    total=False,
-)
-
 MonitoringGroundTruthS3InputTypeDef = TypedDict(
     "MonitoringGroundTruthS3InputTypeDef",
     {
         "S3Uri": str,
     },
     total=False,
 )
@@ -11479,39 +11432,14 @@
     {
         "FlowDefinitionSummaries": List[FlowDefinitionSummaryTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredGetScalingConfigurationRecommendationRequestRequestTypeDef = TypedDict(
-    "_RequiredGetScalingConfigurationRecommendationRequestRequestTypeDef",
-    {
-        "InferenceRecommendationsJobName": str,
-    },
-)
-_OptionalGetScalingConfigurationRecommendationRequestRequestTypeDef = TypedDict(
-    "_OptionalGetScalingConfigurationRecommendationRequestRequestTypeDef",
-    {
-        "RecommendationId": str,
-        "EndpointName": str,
-        "TargetCpuUtilizationPerCore": int,
-        "ScalingPolicyObjective": ScalingPolicyObjectiveTypeDef,
-    },
-    total=False,
-)
-
-
-class GetScalingConfigurationRecommendationRequestRequestTypeDef(
-    _RequiredGetScalingConfigurationRecommendationRequestRequestTypeDef,
-    _OptionalGetScalingConfigurationRecommendationRequestRequestTypeDef,
-):
-    pass
-
-
 GetSearchSuggestionsResponseTypeDef = TypedDict(
     "GetSearchSuggestionsResponseTypeDef",
     {
         "PropertyNameSuggestions": List[PropertyNameSuggestionTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -13156,23 +13084,14 @@
     {
         "CognitoMemberDefinition": CognitoMemberDefinitionTypeDef,
         "OidcMemberDefinition": OidcMemberDefinitionTypeDef,
     },
     total=False,
 )
 
-MetricSpecificationTypeDef = TypedDict(
-    "MetricSpecificationTypeDef",
-    {
-        "Predefined": PredefinedMetricSpecificationTypeDef,
-        "Customized": CustomizedMetricSpecificationTypeDef,
-    },
-    total=False,
-)
-
 MonitoringAlertActionsTypeDef = TypedDict(
     "MonitoringAlertActionsTypeDef",
     {
         "ModelDashboardIndicator": ModelDashboardIndicatorActionTypeDef,
     },
     total=False,
 )
@@ -14923,23 +14842,14 @@
 )
 
 
 class WorkteamTypeDef(_RequiredWorkteamTypeDef, _OptionalWorkteamTypeDef):
     pass
 
 
-TargetTrackingScalingPolicyConfigurationTypeDef = TypedDict(
-    "TargetTrackingScalingPolicyConfigurationTypeDef",
-    {
-        "MetricSpecification": MetricSpecificationTypeDef,
-        "TargetValue": float,
-    },
-    total=False,
-)
-
 MonitoringAlertSummaryTypeDef = TypedDict(
     "MonitoringAlertSummaryTypeDef",
     {
         "MonitoringAlertName": str,
         "CreationTime": datetime,
         "LastModifiedTime": datetime,
         "AlertStatus": MonitoringAlertStatusType,
@@ -16170,22 +16080,14 @@
     "UpdateWorkteamResponseTypeDef",
     {
         "Workteam": WorkteamTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-ScalingPolicyTypeDef = TypedDict(
-    "ScalingPolicyTypeDef",
-    {
-        "TargetTracking": TargetTrackingScalingPolicyConfigurationTypeDef,
-    },
-    total=False,
-)
-
 ListMonitoringAlertsResponseTypeDef = TypedDict(
     "ListMonitoringAlertsResponseTypeDef",
     {
         "MonitoringAlertSummaries": List[MonitoringAlertSummaryTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -17240,26 +17142,14 @@
     {
         "LabelingJobSummaryList": List[LabelingJobSummaryTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-DynamicScalingConfigurationTypeDef = TypedDict(
-    "DynamicScalingConfigurationTypeDef",
-    {
-        "MinCapacity": int,
-        "MaxCapacity": int,
-        "ScaleInCooldown": int,
-        "ScaleOutCooldown": int,
-        "ScalingPolicies": List[ScalingPolicyTypeDef],
-    },
-    total=False,
-)
-
 BatchDescribeModelPackageOutputTypeDef = TypedDict(
     "BatchDescribeModelPackageOutputTypeDef",
     {
         "ModelPackageSummaries": Dict[str, BatchDescribeModelPackageSummaryTypeDef],
         "BatchDescribeModelPackageErrorMap": Dict[str, BatchDescribeModelPackageErrorTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -17522,28 +17412,14 @@
         "TrainingJob": TrainingJobTypeDef,
         "ProcessingJob": ProcessingJobTypeDef,
         "TransformJob": TransformJobTypeDef,
     },
     total=False,
 )
 
-GetScalingConfigurationRecommendationResponseTypeDef = TypedDict(
-    "GetScalingConfigurationRecommendationResponseTypeDef",
-    {
-        "InferenceRecommendationsJobName": str,
-        "RecommendationId": str,
-        "EndpointName": str,
-        "TargetCpuUtilizationPerCore": int,
-        "ScalingPolicyObjective": ScalingPolicyObjectiveTypeDef,
-        "Metric": ScalingPolicyMetricTypeDef,
-        "DynamicScalingConfiguration": DynamicScalingConfigurationTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 MonitoringScheduleConfigTypeDef = TypedDict(
     "MonitoringScheduleConfigTypeDef",
     {
         "ScheduleConfig": ScheduleConfigTypeDef,
         "MonitoringJobDefinition": MonitoringJobDefinitionTypeDef,
         "MonitoringJobDefinitionName": str,
         "MonitoringType": MonitoringTypeType,
```

### Comparing `types-aiobotocore-sagemaker-2.5.2.post2/types_aiobotocore_sagemaker/type_defs.pyi` & `types-aiobotocore-sagemaker-2.5.4/types_aiobotocore_sagemaker/type_defs.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -219,15 +219,14 @@
     SortPipelinesByType,
     SortTrialComponentsByType,
     SortTrialsByType,
     SpaceSortKeyType,
     SpaceStatusType,
     SplitTypeType,
     StageStatusType,
-    StatisticType,
     StepStatusType,
     StudioLifecycleConfigAppTypeType,
     StudioLifecycleConfigSortKeyType,
     TableFormatType,
     TargetDeviceType,
     TargetPlatformAcceleratorType,
     TargetPlatformArchType,
@@ -380,15 +379,14 @@
     "TrialComponentParameterValueTypeDef",
     "TrialComponentStatusTypeDef",
     "OidcConfigTypeDef",
     "SourceIpConfigTypeDef",
     "WorkforceVpcConfigRequestTypeDef",
     "NotificationConfigurationTypeDef",
     "CustomImageTypeDef",
-    "CustomizedMetricSpecificationTypeDef",
     "DataCaptureConfigSummaryTypeDef",
     "DataCatalogConfigTypeDef",
     "MonitoringConstraintsResourceTypeDef",
     "MonitoringStatisticsResourceTypeDef",
     "EndpointInputTypeDef",
     "FileSystemDataSourceTypeDef",
     "S3DataSourceTypeDef",
@@ -557,16 +555,14 @@
     "FileSystemConfigTypeDef",
     "FilterTypeDef",
     "FinalHyperParameterTuningJobObjectiveMetricTypeDef",
     "FlowDefinitionSummaryTypeDef",
     "GetDeviceFleetReportRequestRequestTypeDef",
     "GetLineageGroupPolicyRequestRequestTypeDef",
     "GetModelPackageGroupPolicyInputRequestTypeDef",
-    "ScalingPolicyObjectiveTypeDef",
-    "ScalingPolicyMetricTypeDef",
     "PropertyNameSuggestionTypeDef",
     "GitConfigForUpdateTypeDef",
     "HubContentInfoTypeDef",
     "HubInfoTypeDef",
     "HumanLoopActivationConditionsConfigTypeDef",
     "UiConfigTypeDef",
     "HumanTaskUiSummaryTypeDef",
@@ -626,15 +622,14 @@
     "ListTrainingJobsForHyperParameterTuningJobRequestRequestTypeDef",
     "TransformJobSummaryTypeDef",
     "ListUserProfilesRequestRequestTypeDef",
     "UserProfileDetailsTypeDef",
     "ListWorkforcesRequestRequestTypeDef",
     "ListWorkteamsRequestRequestTypeDef",
     "OidcMemberDefinitionTypeDef",
-    "PredefinedMetricSpecificationTypeDef",
     "MonitoringGroundTruthS3InputTypeDef",
     "ModelDashboardEndpointTypeDef",
     "ModelDashboardIndicatorActionTypeDef",
     "S3ModelDataSourceTypeDef",
     "RealTimeInferenceConfigTypeDef",
     "ModelInputTypeDef",
     "ModelLatencyThresholdTypeDef",
@@ -1027,15 +1022,14 @@
     "EndpointOutputConfigurationTypeDef",
     "EndpointPerformanceTypeDef",
     "ListEndpointsOutputTypeDef",
     "ModelConfigurationTypeDef",
     "NestedFiltersTypeDef",
     "HyperParameterTrainingJobSummaryTypeDef",
     "ListFlowDefinitionsResponseTypeDef",
-    "GetScalingConfigurationRecommendationRequestRequestTypeDef",
     "GetSearchSuggestionsResponseTypeDef",
     "UpdateCodeRepositoryInputRequestTypeDef",
     "ListHubContentVersionsResponseTypeDef",
     "ListHubContentsResponseTypeDef",
     "ListHubsResponseTypeDef",
     "HumanLoopActivationConfigTypeDef",
     "ListHumanTaskUisResponseTypeDef",
@@ -1145,15 +1139,14 @@
     "ListProjectsOutputTypeDef",
     "ListResourceCatalogsResponseTypeDef",
     "ListSpacesResponseTypeDef",
     "ListStudioLifecycleConfigsResponseTypeDef",
     "ListTransformJobsResponseTypeDef",
     "ListUserProfilesResponseTypeDef",
     "MemberDefinitionTypeDef",
-    "MetricSpecificationTypeDef",
     "MonitoringAlertActionsTypeDef",
     "ModelDataSourceTypeDef",
     "ModelInfrastructureConfigTypeDef",
     "ModelPackageContainerDefinitionTypeDef",
     "RecommendationJobStoppingConditionsTypeDef",
     "ModelMetadataSearchExpressionTypeDef",
     "ModelPackageStatusDetailsTypeDef",
@@ -1256,15 +1249,14 @@
     "DescribeAppImageConfigResponseTypeDef",
     "UpdateAppImageConfigRequestRequestTypeDef",
     "ListLabelingJobsForWorkteamResponseTypeDef",
     "LabelingJobInputConfigTypeDef",
     "CreateWorkteamRequestRequestTypeDef",
     "UpdateWorkteamRequestRequestTypeDef",
     "WorkteamTypeDef",
-    "TargetTrackingScalingPolicyConfigurationTypeDef",
     "MonitoringAlertSummaryTypeDef",
     "ContainerDefinitionTypeDef",
     "ModelVariantConfigSummaryTypeDef",
     "ModelVariantConfigTypeDef",
     "AdditionalInferenceSpecificationDefinitionTypeDef",
     "InferenceSpecificationTypeDef",
     "ListModelMetadataRequestListModelMetadataPaginateTypeDef",
@@ -1321,15 +1313,14 @@
     "ListTrialComponentsResponseTypeDef",
     "TrainingSpecificationTypeDef",
     "ListAppImageConfigsResponseTypeDef",
     "LabelingJobSummaryTypeDef",
     "DescribeWorkteamResponseTypeDef",
     "ListWorkteamsResponseTypeDef",
     "UpdateWorkteamResponseTypeDef",
-    "ScalingPolicyTypeDef",
     "ListMonitoringAlertsResponseTypeDef",
     "CreateModelInputRequestTypeDef",
     "DescribeModelOutputTypeDef",
     "ModelTypeDef",
     "DescribeInferenceExperimentResponseTypeDef",
     "CreateInferenceExperimentRequestRequestTypeDef",
     "StopInferenceExperimentRequestRequestTypeDef",
@@ -1366,29 +1357,27 @@
     "DescribeEndpointConfigOutputTypeDef",
     "DescribeEndpointOutputTypeDef",
     "CreateHyperParameterTuningJobRequestRequestTypeDef",
     "DescribeHyperParameterTuningJobResponseTypeDef",
     "HyperParameterTuningJobSearchEntityTypeDef",
     "ListInferenceRecommendationsJobStepsResponseTypeDef",
     "ListLabelingJobsResponseTypeDef",
-    "DynamicScalingConfigurationTypeDef",
     "BatchDescribeModelPackageOutputTypeDef",
     "CreateDataQualityJobDefinitionRequestRequestTypeDef",
     "DescribeDataQualityJobDefinitionResponseTypeDef",
     "CreateModelBiasJobDefinitionRequestRequestTypeDef",
     "DescribeModelBiasJobDefinitionResponseTypeDef",
     "CreateModelExplainabilityJobDefinitionRequestRequestTypeDef",
     "DescribeModelExplainabilityJobDefinitionResponseTypeDef",
     "CreateModelQualityJobDefinitionRequestRequestTypeDef",
     "DescribeModelQualityJobDefinitionResponseTypeDef",
     "MonitoringJobDefinitionTypeDef",
     "AlgorithmValidationProfileTypeDef",
     "ModelPackageValidationProfileTypeDef",
     "TrialComponentSourceDetailTypeDef",
-    "GetScalingConfigurationRecommendationResponseTypeDef",
     "MonitoringScheduleConfigTypeDef",
     "AlgorithmValidationSpecificationTypeDef",
     "ModelPackageValidationSpecificationTypeDef",
     "TrialComponentTypeDef",
     "CreateMonitoringScheduleRequestRequestTypeDef",
     "DescribeMonitoringScheduleResponseTypeDef",
     "ModelDashboardMonitoringScheduleTypeDef",
@@ -2893,24 +2882,14 @@
     },
     total=False,
 )
 
 class CustomImageTypeDef(_RequiredCustomImageTypeDef, _OptionalCustomImageTypeDef):
     pass
 
-CustomizedMetricSpecificationTypeDef = TypedDict(
-    "CustomizedMetricSpecificationTypeDef",
-    {
-        "MetricName": str,
-        "Namespace": str,
-        "Statistic": StatisticType,
-    },
-    total=False,
-)
-
 DataCaptureConfigSummaryTypeDef = TypedDict(
     "DataCaptureConfigSummaryTypeDef",
     {
         "EnableCapture": bool,
         "CaptureStatus": CaptureStatusType,
         "CurrentSamplingPercentage": int,
         "DestinationS3Uri": str,
@@ -4781,32 +4760,14 @@
 GetModelPackageGroupPolicyInputRequestTypeDef = TypedDict(
     "GetModelPackageGroupPolicyInputRequestTypeDef",
     {
         "ModelPackageGroupName": str,
     },
 )
 
-ScalingPolicyObjectiveTypeDef = TypedDict(
-    "ScalingPolicyObjectiveTypeDef",
-    {
-        "MinInvocationsPerMinute": int,
-        "MaxInvocationsPerMinute": int,
-    },
-    total=False,
-)
-
-ScalingPolicyMetricTypeDef = TypedDict(
-    "ScalingPolicyMetricTypeDef",
-    {
-        "InvocationsPerInstance": int,
-        "ModelLatency": int,
-    },
-    total=False,
-)
-
 PropertyNameSuggestionTypeDef = TypedDict(
     "PropertyNameSuggestionTypeDef",
     {
         "PropertyName": str,
     },
     total=False,
 )
@@ -5813,22 +5774,14 @@
 OidcMemberDefinitionTypeDef = TypedDict(
     "OidcMemberDefinitionTypeDef",
     {
         "Groups": Sequence[str],
     },
 )
 
-PredefinedMetricSpecificationTypeDef = TypedDict(
-    "PredefinedMetricSpecificationTypeDef",
-    {
-        "PredefinedMetricType": str,
-    },
-    total=False,
-)
-
 MonitoringGroundTruthS3InputTypeDef = TypedDict(
     "MonitoringGroundTruthS3InputTypeDef",
     {
         "S3Uri": str,
     },
     total=False,
 )
@@ -11076,37 +11029,14 @@
     {
         "FlowDefinitionSummaries": List[FlowDefinitionSummaryTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredGetScalingConfigurationRecommendationRequestRequestTypeDef = TypedDict(
-    "_RequiredGetScalingConfigurationRecommendationRequestRequestTypeDef",
-    {
-        "InferenceRecommendationsJobName": str,
-    },
-)
-_OptionalGetScalingConfigurationRecommendationRequestRequestTypeDef = TypedDict(
-    "_OptionalGetScalingConfigurationRecommendationRequestRequestTypeDef",
-    {
-        "RecommendationId": str,
-        "EndpointName": str,
-        "TargetCpuUtilizationPerCore": int,
-        "ScalingPolicyObjective": ScalingPolicyObjectiveTypeDef,
-    },
-    total=False,
-)
-
-class GetScalingConfigurationRecommendationRequestRequestTypeDef(
-    _RequiredGetScalingConfigurationRecommendationRequestRequestTypeDef,
-    _OptionalGetScalingConfigurationRecommendationRequestRequestTypeDef,
-):
-    pass
-
 GetSearchSuggestionsResponseTypeDef = TypedDict(
     "GetSearchSuggestionsResponseTypeDef",
     {
         "PropertyNameSuggestions": List[PropertyNameSuggestionTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -12711,23 +12641,14 @@
     {
         "CognitoMemberDefinition": CognitoMemberDefinitionTypeDef,
         "OidcMemberDefinition": OidcMemberDefinitionTypeDef,
     },
     total=False,
 )
 
-MetricSpecificationTypeDef = TypedDict(
-    "MetricSpecificationTypeDef",
-    {
-        "Predefined": PredefinedMetricSpecificationTypeDef,
-        "Customized": CustomizedMetricSpecificationTypeDef,
-    },
-    total=False,
-)
-
 MonitoringAlertActionsTypeDef = TypedDict(
     "MonitoringAlertActionsTypeDef",
     {
         "ModelDashboardIndicator": ModelDashboardIndicatorActionTypeDef,
     },
     total=False,
 )
@@ -14406,23 +14327,14 @@
     },
     total=False,
 )
 
 class WorkteamTypeDef(_RequiredWorkteamTypeDef, _OptionalWorkteamTypeDef):
     pass
 
-TargetTrackingScalingPolicyConfigurationTypeDef = TypedDict(
-    "TargetTrackingScalingPolicyConfigurationTypeDef",
-    {
-        "MetricSpecification": MetricSpecificationTypeDef,
-        "TargetValue": float,
-    },
-    total=False,
-)
-
 MonitoringAlertSummaryTypeDef = TypedDict(
     "MonitoringAlertSummaryTypeDef",
     {
         "MonitoringAlertName": str,
         "CreationTime": datetime,
         "LastModifiedTime": datetime,
         "AlertStatus": MonitoringAlertStatusType,
@@ -15595,22 +15507,14 @@
     "UpdateWorkteamResponseTypeDef",
     {
         "Workteam": WorkteamTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-ScalingPolicyTypeDef = TypedDict(
-    "ScalingPolicyTypeDef",
-    {
-        "TargetTracking": TargetTrackingScalingPolicyConfigurationTypeDef,
-    },
-    total=False,
-)
-
 ListMonitoringAlertsResponseTypeDef = TypedDict(
     "ListMonitoringAlertsResponseTypeDef",
     {
         "MonitoringAlertSummaries": List[MonitoringAlertSummaryTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -16625,26 +16529,14 @@
     {
         "LabelingJobSummaryList": List[LabelingJobSummaryTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-DynamicScalingConfigurationTypeDef = TypedDict(
-    "DynamicScalingConfigurationTypeDef",
-    {
-        "MinCapacity": int,
-        "MaxCapacity": int,
-        "ScaleInCooldown": int,
-        "ScaleOutCooldown": int,
-        "ScalingPolicies": List[ScalingPolicyTypeDef],
-    },
-    total=False,
-)
-
 BatchDescribeModelPackageOutputTypeDef = TypedDict(
     "BatchDescribeModelPackageOutputTypeDef",
     {
         "ModelPackageSummaries": Dict[str, BatchDescribeModelPackageSummaryTypeDef],
         "BatchDescribeModelPackageErrorMap": Dict[str, BatchDescribeModelPackageErrorTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -16895,28 +16787,14 @@
         "TrainingJob": TrainingJobTypeDef,
         "ProcessingJob": ProcessingJobTypeDef,
         "TransformJob": TransformJobTypeDef,
     },
     total=False,
 )
 
-GetScalingConfigurationRecommendationResponseTypeDef = TypedDict(
-    "GetScalingConfigurationRecommendationResponseTypeDef",
-    {
-        "InferenceRecommendationsJobName": str,
-        "RecommendationId": str,
-        "EndpointName": str,
-        "TargetCpuUtilizationPerCore": int,
-        "ScalingPolicyObjective": ScalingPolicyObjectiveTypeDef,
-        "Metric": ScalingPolicyMetricTypeDef,
-        "DynamicScalingConfiguration": DynamicScalingConfigurationTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 MonitoringScheduleConfigTypeDef = TypedDict(
     "MonitoringScheduleConfigTypeDef",
     {
         "ScheduleConfig": ScheduleConfigTypeDef,
         "MonitoringJobDefinition": MonitoringJobDefinitionTypeDef,
         "MonitoringJobDefinitionName": str,
         "MonitoringType": MonitoringTypeType,
```

### Comparing `types-aiobotocore-sagemaker-2.5.2.post2/types_aiobotocore_sagemaker/waiter.py` & `types-aiobotocore-sagemaker-2.5.4/types_aiobotocore_sagemaker/waiter.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-sagemaker-2.5.2.post2/types_aiobotocore_sagemaker/waiter.pyi` & `types-aiobotocore-sagemaker-2.5.4/types_aiobotocore_sagemaker/waiter.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-sagemaker-2.5.2.post2/types_aiobotocore_sagemaker.egg-info/PKG-INFO` & `types-aiobotocore-sagemaker-2.5.4/types_aiobotocore_sagemaker.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-sagemaker
-Version: 2.5.2.post2
-Summary: Type annotations for aiobotocore.SageMaker 2.5.2 service generated with mypy-boto3-builder 7.17.2
+Version: 2.5.4
+Summary: Type annotations for aiobotocore.SageMaker 2.5.4 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-sagemaker.svg?color=blue)](https://pypi.org/project/types-aiobotocore-sagemaker)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-sagemaker)](https://pepy.tech/project/types-aiobotocore-sagemaker)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.SageMaker 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker)
+[aiobotocore.SageMaker 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-sagemaker-2.5.2.post2/types_aiobotocore_sagemaker.egg-info/SOURCES.txt` & `types-aiobotocore-sagemaker-2.5.4/types_aiobotocore_sagemaker.egg-info/SOURCES.txt`

 * *Files identical despite different names*


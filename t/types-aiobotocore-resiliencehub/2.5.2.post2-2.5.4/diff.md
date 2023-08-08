# Comparing `tmp/types-aiobotocore-resiliencehub-2.5.2.post2.tar.gz` & `tmp/types-aiobotocore-resiliencehub-2.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-resiliencehub-2.5.2.post2.tar", last modified: Fri Aug  4 13:59:23 2023, max compression
+gzip compressed data, was "types-aiobotocore-resiliencehub-2.5.4.tar", last modified: Tue Aug  8 01:24:18 2023, max compression
```

## Comparing `types-aiobotocore-resiliencehub-2.5.2.post2.tar` & `types-aiobotocore-resiliencehub-2.5.4.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:23.106643 types-aiobotocore-resiliencehub-2.5.2.post2/
--rw-r--r--   0 vlad      (1000) vlad      (1000)     1070 2023-08-04 13:50:42.000000 types-aiobotocore-resiliencehub-2.5.2.post2/LICENSE
--rw-r--r--   0 vlad      (1000) vlad      (1000)    12500 2023-08-04 13:59:23.106643 types-aiobotocore-resiliencehub-2.5.2.post2/PKG-INFO
--rw-r--r--   0 vlad      (1000) vlad      (1000)    10958 2023-08-04 13:50:42.000000 types-aiobotocore-resiliencehub-2.5.2.post2/README.md
--rw-r--r--   0 vlad      (1000) vlad      (1000)       38 2023-08-04 13:59:23.106643 types-aiobotocore-resiliencehub-2.5.2.post2/setup.cfg
--rw-r--r--   0 vlad      (1000) vlad      (1000)     2114 2023-08-04 13:50:41.000000 types-aiobotocore-resiliencehub-2.5.2.post2/setup.py
-drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:23.106643 types-aiobotocore-resiliencehub-2.5.2.post2/types_aiobotocore_resiliencehub/
--rw-r--r--   0 vlad      (1000) vlad      (1000)      490 2023-08-04 13:50:42.000000 types-aiobotocore-resiliencehub-2.5.2.post2/types_aiobotocore_resiliencehub/__init__.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)      489 2023-08-04 13:50:42.000000 types-aiobotocore-resiliencehub-2.5.2.post2/types_aiobotocore_resiliencehub/__init__.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)      967 2023-08-04 13:50:42.000000 types-aiobotocore-resiliencehub-2.5.2.post2/types_aiobotocore_resiliencehub/__main__.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)    43867 2023-08-04 13:50:42.000000 types-aiobotocore-resiliencehub-2.5.2.post2/types_aiobotocore_resiliencehub/client.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)    43805 2023-08-04 13:50:42.000000 types-aiobotocore-resiliencehub-2.5.2.post2/types_aiobotocore_resiliencehub/client.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)    11692 2023-08-04 13:50:42.000000 types-aiobotocore-resiliencehub-2.5.2.post2/types_aiobotocore_resiliencehub/literals.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)    11690 2023-08-04 13:50:42.000000 types-aiobotocore-resiliencehub-2.5.2.post2/types_aiobotocore_resiliencehub/literals.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:50:42.000000 types-aiobotocore-resiliencehub-2.5.2.post2/types_aiobotocore_resiliencehub/py.typed
--rw-r--r--   0 vlad      (1000) vlad      (1000)    67894 2023-08-04 13:50:44.000000 types-aiobotocore-resiliencehub-2.5.2.post2/types_aiobotocore_resiliencehub/type_defs.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)    67775 2023-08-04 13:50:43.000000 types-aiobotocore-resiliencehub-2.5.2.post2/types_aiobotocore_resiliencehub/type_defs.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)       65 2023-08-04 13:50:42.000000 types-aiobotocore-resiliencehub-2.5.2.post2/types_aiobotocore_resiliencehub/version.py
-drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:23.106643 types-aiobotocore-resiliencehub-2.5.2.post2/types_aiobotocore_resiliencehub.egg-info/
--rw-r--r--   0 vlad      (1000) vlad      (1000)    12500 2023-08-04 13:59:22.000000 types-aiobotocore-resiliencehub-2.5.2.post2/types_aiobotocore_resiliencehub.egg-info/PKG-INFO
--rw-r--r--   0 vlad      (1000) vlad      (1000)      836 2023-08-04 13:59:22.000000 types-aiobotocore-resiliencehub-2.5.2.post2/types_aiobotocore_resiliencehub.egg-info/SOURCES.txt
--rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:22.000000 types-aiobotocore-resiliencehub-2.5.2.post2/types_aiobotocore_resiliencehub.egg-info/dependency_links.txt
--rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:22.000000 types-aiobotocore-resiliencehub-2.5.2.post2/types_aiobotocore_resiliencehub.egg-info/not-zip-safe
--rw-r--r--   0 vlad      (1000) vlad      (1000)       52 2023-08-04 13:59:22.000000 types-aiobotocore-resiliencehub-2.5.2.post2/types_aiobotocore_resiliencehub.egg-info/requires.txt
--rw-r--r--   0 vlad      (1000) vlad      (1000)       32 2023-08-04 13:59:22.000000 types-aiobotocore-resiliencehub-2.5.2.post2/types_aiobotocore_resiliencehub.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:24:18.398761 types-aiobotocore-resiliencehub-2.5.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-08 01:19:21.000000 types-aiobotocore-resiliencehub-2.5.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    12494 2023-08-08 01:24:18.398761 types-aiobotocore-resiliencehub-2.5.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10958 2023-08-08 01:19:21.000000 types-aiobotocore-resiliencehub-2.5.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-08 01:24:18.398761 types-aiobotocore-resiliencehub-2.5.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2108 2023-08-08 01:19:21.000000 types-aiobotocore-resiliencehub-2.5.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:24:18.394761 types-aiobotocore-resiliencehub-2.5.4/types_aiobotocore_resiliencehub/
+-rw-r--r--   0 runner    (1001) docker     (123)      490 2023-08-08 01:19:21.000000 types-aiobotocore-resiliencehub-2.5.4/types_aiobotocore_resiliencehub/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      489 2023-08-08 01:19:21.000000 types-aiobotocore-resiliencehub-2.5.4/types_aiobotocore_resiliencehub/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      955 2023-08-08 01:19:21.000000 types-aiobotocore-resiliencehub-2.5.4/types_aiobotocore_resiliencehub/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41861 2023-08-08 01:19:21.000000 types-aiobotocore-resiliencehub-2.5.4/types_aiobotocore_resiliencehub/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41801 2023-08-08 01:19:21.000000 types-aiobotocore-resiliencehub-2.5.4/types_aiobotocore_resiliencehub/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    11003 2023-08-08 01:19:21.000000 types-aiobotocore-resiliencehub-2.5.4/types_aiobotocore_resiliencehub/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11001 2023-08-08 01:19:21.000000 types-aiobotocore-resiliencehub-2.5.4/types_aiobotocore_resiliencehub/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 01:19:21.000000 types-aiobotocore-resiliencehub-2.5.4/types_aiobotocore_resiliencehub/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    60797 2023-08-08 01:19:22.000000 types-aiobotocore-resiliencehub-2.5.4/types_aiobotocore_resiliencehub/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    60692 2023-08-08 01:19:22.000000 types-aiobotocore-resiliencehub-2.5.4/types_aiobotocore_resiliencehub/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-08-08 01:19:21.000000 types-aiobotocore-resiliencehub-2.5.4/types_aiobotocore_resiliencehub/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:24:18.398761 types-aiobotocore-resiliencehub-2.5.4/types_aiobotocore_resiliencehub.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    12494 2023-08-08 01:24:18.000000 types-aiobotocore-resiliencehub-2.5.4/types_aiobotocore_resiliencehub.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      836 2023-08-08 01:24:18.000000 types-aiobotocore-resiliencehub-2.5.4/types_aiobotocore_resiliencehub.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 01:24:18.000000 types-aiobotocore-resiliencehub-2.5.4/types_aiobotocore_resiliencehub.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 01:24:18.000000 types-aiobotocore-resiliencehub-2.5.4/types_aiobotocore_resiliencehub.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-08 01:24:18.000000 types-aiobotocore-resiliencehub-2.5.4/types_aiobotocore_resiliencehub.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-08-08 01:24:18.000000 types-aiobotocore-resiliencehub-2.5.4/types_aiobotocore_resiliencehub.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-resiliencehub-2.5.2.post2/LICENSE` & `types-aiobotocore-resiliencehub-2.5.4/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-resiliencehub-2.5.2.post2/PKG-INFO` & `types-aiobotocore-resiliencehub-2.5.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-resiliencehub
-Version: 2.5.2.post2
-Summary: Type annotations for aiobotocore.ResilienceHub 2.5.2 service generated with mypy-boto3-builder 7.17.2
+Version: 2.5.4
+Summary: Type annotations for aiobotocore.ResilienceHub 2.5.4 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_resiliencehub/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-resiliencehub.svg?color=blue)](https://pypi.org/project/types-aiobotocore-resiliencehub)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_resiliencehub/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-resiliencehub)](https://pepy.tech/project/types-aiobotocore-resiliencehub)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.ResilienceHub 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resiliencehub.html#ResilienceHub)
+[aiobotocore.ResilienceHub 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resiliencehub.html#ResilienceHub)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-resiliencehub-2.5.2.post2/README.md` & `types-aiobotocore-resiliencehub-2.5.4/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-resiliencehub.svg?color=blue)](https://pypi.org/project/types-aiobotocore-resiliencehub)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_resiliencehub/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-resiliencehub)](https://pepy.tech/project/types-aiobotocore-resiliencehub)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.ResilienceHub 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resiliencehub.html#ResilienceHub)
+[aiobotocore.ResilienceHub 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resiliencehub.html#ResilienceHub)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-resiliencehub-2.5.2.post2/setup.py` & `types-aiobotocore-resiliencehub-2.5.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-resiliencehub",
-    version="2.5.2.post2",
+    version="2.5.4",
     packages=["types_aiobotocore_resiliencehub"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.ResilienceHub 2.5.2 service generated with"
+        "Type annotations for aiobotocore.ResilienceHub 2.5.4 service generated with"
         " mypy-boto3-builder 7.17.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
```

### Comparing `types-aiobotocore-resiliencehub-2.5.2.post2/types_aiobotocore_resiliencehub/__main__.py` & `types-aiobotocore-resiliencehub-2.5.4/types_aiobotocore_resiliencehub/__main__.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.ResilienceHub 2.5.2\nVersion:        "
-        " 2.5.2.post2\nBuilder version: 7.17.2\nDocs:           "
+        "Type annotations for aiobotocore.ResilienceHub 2.5.4\nVersion:         2.5.4\nBuilder"
+        " version: 7.17.2\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_resiliencehub//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resiliencehub.html#ResilienceHub\nOther"
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

### Comparing `types-aiobotocore-resiliencehub-2.5.2.post2/types_aiobotocore_resiliencehub/client.py` & `types-aiobotocore-resiliencehub-2.5.4/types_aiobotocore_resiliencehub/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -30,15 +30,14 @@
     RenderRecommendationTypeType,
     ResiliencyPolicyTierType,
     ResourceImportStrategyTypeType,
     TemplateFormatType,
 )
 from .type_defs import (
     AddDraftAppVersionResourceMappingsResponseTypeDef,
-    BatchUpdateRecommendationStatusResponseTypeDef,
     CreateAppResponseTypeDef,
     CreateAppVersionAppComponentResponseTypeDef,
     CreateAppVersionResourceResponseTypeDef,
     CreateRecommendationTemplateResponseTypeDef,
     CreateResiliencyPolicyResponseTypeDef,
     DeleteAppAssessmentResponseTypeDef,
     DeleteAppInputSourceResponseTypeDef,
@@ -54,19 +53,17 @@
     DescribeAppVersionResourcesResolutionStatusResponseTypeDef,
     DescribeAppVersionResponseTypeDef,
     DescribeAppVersionTemplateResponseTypeDef,
     DescribeDraftAppVersionResourcesImportStatusResponseTypeDef,
     DescribeResiliencyPolicyResponseTypeDef,
     EksSourceClusterNamespaceTypeDef,
     EksSourceTypeDef,
-    EventSubscriptionTypeDef,
     FailurePolicyTypeDef,
     ImportResourcesToDraftAppVersionResponseTypeDef,
     ListAlarmRecommendationsResponseTypeDef,
-    ListAppAssessmentComplianceDriftsResponseTypeDef,
     ListAppAssessmentsResponseTypeDef,
     ListAppComponentCompliancesResponseTypeDef,
     ListAppComponentRecommendationsResponseTypeDef,
     ListAppInputSourcesResponseTypeDef,
     ListAppsResponseTypeDef,
     ListAppVersionAppComponentsResponseTypeDef,
     ListAppVersionResourceMappingsResponseTypeDef,
@@ -76,28 +73,25 @@
     ListResiliencyPoliciesResponseTypeDef,
     ListSopRecommendationsResponseTypeDef,
     ListSuggestedResiliencyPoliciesResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     ListTestRecommendationsResponseTypeDef,
     ListUnsupportedAppVersionResourcesResponseTypeDef,
     LogicalResourceIdTypeDef,
-    PermissionModelTypeDef,
     PublishAppVersionResponseTypeDef,
     PutDraftAppVersionTemplateResponseTypeDef,
     RemoveDraftAppVersionResourceMappingsResponseTypeDef,
     ResolveAppVersionResourcesResponseTypeDef,
     ResourceMappingTypeDef,
     StartAppAssessmentResponseTypeDef,
     TerraformSourceTypeDef,
-    TimestampTypeDef,
     UpdateAppResponseTypeDef,
     UpdateAppVersionAppComponentResponseTypeDef,
     UpdateAppVersionResourceResponseTypeDef,
     UpdateAppVersionResponseTypeDef,
-    UpdateRecommendationStatusRequestEntryTypeDef,
     UpdateResiliencyPolicyResponseTypeDef,
 )
 
 __all__ = ("ResilienceHubClient",)
 
 
 class BotocoreClientError(BaseException):
@@ -142,27 +136,14 @@
         """
         Adds the resource mapping for the draft application version.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resiliencehub.html#ResilienceHub.Client.add_draft_app_version_resource_mappings)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_resiliencehub/client/#add_draft_app_version_resource_mappings)
         """
 
-    async def batch_update_recommendation_status(
-        self,
-        *,
-        appArn: str,
-        requestEntries: Sequence[UpdateRecommendationStatusRequestEntryTypeDef]
-    ) -> BatchUpdateRecommendationStatusResponseTypeDef:
-        """
-        Enables you to include or exclude one or more operational recommendations.
-
-        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resiliencehub.html#ResilienceHub.Client.batch_update_recommendation_status)
-        [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_resiliencehub/client/#batch_update_recommendation_status)
-        """
-
     def can_paginate(self, operation_name: str) -> bool:
         """
         Check if an operation can be paginated.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resiliencehub.html#ResilienceHub.Client.can_paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_resiliencehub/client/#can_paginate)
         """
@@ -178,16 +159,14 @@
     async def create_app(
         self,
         *,
         name: str,
         assessmentSchedule: AppAssessmentScheduleTypeType = ...,
         clientToken: str = ...,
         description: str = ...,
-        eventSubscriptions: Sequence[EventSubscriptionTypeDef] = ...,
-        permissionModel: PermissionModelTypeDef = ...,
         policyArn: str = ...,
         tags: Mapping[str, str] = ...
     ) -> CreateAppResponseTypeDef:
         """
         Creates an Resilience Hub application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resiliencehub.html#ResilienceHub.Client.create_app)
@@ -489,24 +468,14 @@
         """
         Lists the alarm recommendations for an Resilience Hub application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resiliencehub.html#ResilienceHub.Client.list_alarm_recommendations)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_resiliencehub/client/#list_alarm_recommendations)
         """
 
-    async def list_app_assessment_compliance_drifts(
-        self, *, assessmentArn: str, maxResults: int = ..., nextToken: str = ...
-    ) -> ListAppAssessmentComplianceDriftsResponseTypeDef:
-        """
-        List of compliance drifts that were detected while running an assessment.
-
-        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resiliencehub.html#ResilienceHub.Client.list_app_assessment_compliance_drifts)
-        [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_resiliencehub/client/#list_app_assessment_compliance_drifts)
-        """
-
     async def list_app_assessments(
         self,
         *,
         appArn: str = ...,
         assessmentName: str = ...,
         assessmentStatus: Sequence[AssessmentStatusType] = ...,
         complianceStatus: ComplianceStatusType = ...,
@@ -585,21 +554,15 @@
         Lists all the resources in an Resilience Hub application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resiliencehub.html#ResilienceHub.Client.list_app_version_resources)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_resiliencehub/client/#list_app_version_resources)
         """
 
     async def list_app_versions(
-        self,
-        *,
-        appArn: str,
-        endTime: TimestampTypeDef = ...,
-        maxResults: int = ...,
-        nextToken: str = ...,
-        startTime: TimestampTypeDef = ...
+        self, *, appArn: str, maxResults: int = ..., nextToken: str = ...
     ) -> ListAppVersionsResponseTypeDef:
         """
         Lists the different versions for the Resilience Hub applications.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resiliencehub.html#ResilienceHub.Client.list_app_versions)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_resiliencehub/client/#list_app_versions)
         """
@@ -695,17 +658,15 @@
         """
         Lists the resources that are not currently supported in Resilience Hub.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resiliencehub.html#ResilienceHub.Client.list_unsupported_app_version_resources)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_resiliencehub/client/#list_unsupported_app_version_resources)
         """
 
-    async def publish_app_version(
-        self, *, appArn: str, versionName: str = ...
-    ) -> PublishAppVersionResponseTypeDef:
+    async def publish_app_version(self, *, appArn: str) -> PublishAppVersionResponseTypeDef:
         """
         Publishes a new version of a specific Resilience Hub application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resiliencehub.html#ResilienceHub.Client.publish_app_version)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_resiliencehub/client/#publish_app_version)
         """
 
@@ -783,16 +744,14 @@
     async def update_app(
         self,
         *,
         appArn: str,
         assessmentSchedule: AppAssessmentScheduleTypeType = ...,
         clearResiliencyPolicyArn: bool = ...,
         description: str = ...,
-        eventSubscriptions: Sequence[EventSubscriptionTypeDef] = ...,
-        permissionModel: PermissionModelTypeDef = ...,
         policyArn: str = ...
     ) -> UpdateAppResponseTypeDef:
         """
         Updates an application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resiliencehub.html#ResilienceHub.Client.update_app)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_resiliencehub/client/#update_app)
```

### Comparing `types-aiobotocore-resiliencehub-2.5.2.post2/types_aiobotocore_resiliencehub/client.pyi` & `types-aiobotocore-resiliencehub-2.5.4/types_aiobotocore_resiliencehub/client.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -30,15 +30,14 @@
     RenderRecommendationTypeType,
     ResiliencyPolicyTierType,
     ResourceImportStrategyTypeType,
     TemplateFormatType,
 )
 from .type_defs import (
     AddDraftAppVersionResourceMappingsResponseTypeDef,
-    BatchUpdateRecommendationStatusResponseTypeDef,
     CreateAppResponseTypeDef,
     CreateAppVersionAppComponentResponseTypeDef,
     CreateAppVersionResourceResponseTypeDef,
     CreateRecommendationTemplateResponseTypeDef,
     CreateResiliencyPolicyResponseTypeDef,
     DeleteAppAssessmentResponseTypeDef,
     DeleteAppInputSourceResponseTypeDef,
@@ -54,19 +53,17 @@
     DescribeAppVersionResourcesResolutionStatusResponseTypeDef,
     DescribeAppVersionResponseTypeDef,
     DescribeAppVersionTemplateResponseTypeDef,
     DescribeDraftAppVersionResourcesImportStatusResponseTypeDef,
     DescribeResiliencyPolicyResponseTypeDef,
     EksSourceClusterNamespaceTypeDef,
     EksSourceTypeDef,
-    EventSubscriptionTypeDef,
     FailurePolicyTypeDef,
     ImportResourcesToDraftAppVersionResponseTypeDef,
     ListAlarmRecommendationsResponseTypeDef,
-    ListAppAssessmentComplianceDriftsResponseTypeDef,
     ListAppAssessmentsResponseTypeDef,
     ListAppComponentCompliancesResponseTypeDef,
     ListAppComponentRecommendationsResponseTypeDef,
     ListAppInputSourcesResponseTypeDef,
     ListAppsResponseTypeDef,
     ListAppVersionAppComponentsResponseTypeDef,
     ListAppVersionResourceMappingsResponseTypeDef,
@@ -76,28 +73,25 @@
     ListResiliencyPoliciesResponseTypeDef,
     ListSopRecommendationsResponseTypeDef,
     ListSuggestedResiliencyPoliciesResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     ListTestRecommendationsResponseTypeDef,
     ListUnsupportedAppVersionResourcesResponseTypeDef,
     LogicalResourceIdTypeDef,
-    PermissionModelTypeDef,
     PublishAppVersionResponseTypeDef,
     PutDraftAppVersionTemplateResponseTypeDef,
     RemoveDraftAppVersionResourceMappingsResponseTypeDef,
     ResolveAppVersionResourcesResponseTypeDef,
     ResourceMappingTypeDef,
     StartAppAssessmentResponseTypeDef,
     TerraformSourceTypeDef,
-    TimestampTypeDef,
     UpdateAppResponseTypeDef,
     UpdateAppVersionAppComponentResponseTypeDef,
     UpdateAppVersionResourceResponseTypeDef,
     UpdateAppVersionResponseTypeDef,
-    UpdateRecommendationStatusRequestEntryTypeDef,
     UpdateResiliencyPolicyResponseTypeDef,
 )
 
 __all__ = ("ResilienceHubClient",)
 
 class BotocoreClientError(BaseException):
     MSG_TEMPLATE: str
@@ -137,26 +131,14 @@
     ) -> AddDraftAppVersionResourceMappingsResponseTypeDef:
         """
         Adds the resource mapping for the draft application version.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resiliencehub.html#ResilienceHub.Client.add_draft_app_version_resource_mappings)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_resiliencehub/client/#add_draft_app_version_resource_mappings)
         """
-    async def batch_update_recommendation_status(
-        self,
-        *,
-        appArn: str,
-        requestEntries: Sequence[UpdateRecommendationStatusRequestEntryTypeDef]
-    ) -> BatchUpdateRecommendationStatusResponseTypeDef:
-        """
-        Enables you to include or exclude one or more operational recommendations.
-
-        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resiliencehub.html#ResilienceHub.Client.batch_update_recommendation_status)
-        [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_resiliencehub/client/#batch_update_recommendation_status)
-        """
     def can_paginate(self, operation_name: str) -> bool:
         """
         Check if an operation can be paginated.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resiliencehub.html#ResilienceHub.Client.can_paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_resiliencehub/client/#can_paginate)
         """
@@ -170,16 +152,14 @@
     async def create_app(
         self,
         *,
         name: str,
         assessmentSchedule: AppAssessmentScheduleTypeType = ...,
         clientToken: str = ...,
         description: str = ...,
-        eventSubscriptions: Sequence[EventSubscriptionTypeDef] = ...,
-        permissionModel: PermissionModelTypeDef = ...,
         policyArn: str = ...,
         tags: Mapping[str, str] = ...
     ) -> CreateAppResponseTypeDef:
         """
         Creates an Resilience Hub application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resiliencehub.html#ResilienceHub.Client.create_app)
@@ -457,23 +437,14 @@
     ) -> ListAlarmRecommendationsResponseTypeDef:
         """
         Lists the alarm recommendations for an Resilience Hub application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resiliencehub.html#ResilienceHub.Client.list_alarm_recommendations)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_resiliencehub/client/#list_alarm_recommendations)
         """
-    async def list_app_assessment_compliance_drifts(
-        self, *, assessmentArn: str, maxResults: int = ..., nextToken: str = ...
-    ) -> ListAppAssessmentComplianceDriftsResponseTypeDef:
-        """
-        List of compliance drifts that were detected while running an assessment.
-
-        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resiliencehub.html#ResilienceHub.Client.list_app_assessment_compliance_drifts)
-        [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_resiliencehub/client/#list_app_assessment_compliance_drifts)
-        """
     async def list_app_assessments(
         self,
         *,
         appArn: str = ...,
         assessmentName: str = ...,
         assessmentStatus: Sequence[AssessmentStatusType] = ...,
         complianceStatus: ComplianceStatusType = ...,
@@ -545,21 +516,15 @@
         """
         Lists all the resources in an Resilience Hub application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resiliencehub.html#ResilienceHub.Client.list_app_version_resources)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_resiliencehub/client/#list_app_version_resources)
         """
     async def list_app_versions(
-        self,
-        *,
-        appArn: str,
-        endTime: TimestampTypeDef = ...,
-        maxResults: int = ...,
-        nextToken: str = ...,
-        startTime: TimestampTypeDef = ...
+        self, *, appArn: str, maxResults: int = ..., nextToken: str = ...
     ) -> ListAppVersionsResponseTypeDef:
         """
         Lists the different versions for the Resilience Hub applications.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resiliencehub.html#ResilienceHub.Client.list_app_versions)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_resiliencehub/client/#list_app_versions)
         """
@@ -646,17 +611,15 @@
     ) -> ListUnsupportedAppVersionResourcesResponseTypeDef:
         """
         Lists the resources that are not currently supported in Resilience Hub.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resiliencehub.html#ResilienceHub.Client.list_unsupported_app_version_resources)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_resiliencehub/client/#list_unsupported_app_version_resources)
         """
-    async def publish_app_version(
-        self, *, appArn: str, versionName: str = ...
-    ) -> PublishAppVersionResponseTypeDef:
+    async def publish_app_version(self, *, appArn: str) -> PublishAppVersionResponseTypeDef:
         """
         Publishes a new version of a specific Resilience Hub application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resiliencehub.html#ResilienceHub.Client.publish_app_version)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_resiliencehub/client/#publish_app_version)
         """
     async def put_draft_app_version_template(
@@ -727,16 +690,14 @@
     async def update_app(
         self,
         *,
         appArn: str,
         assessmentSchedule: AppAssessmentScheduleTypeType = ...,
         clearResiliencyPolicyArn: bool = ...,
         description: str = ...,
-        eventSubscriptions: Sequence[EventSubscriptionTypeDef] = ...,
-        permissionModel: PermissionModelTypeDef = ...,
         policyArn: str = ...
     ) -> UpdateAppResponseTypeDef:
         """
         Updates an application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resiliencehub.html#ResilienceHub.Client.update_app)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_resiliencehub/client/#update_app)
```

### Comparing `types-aiobotocore-resiliencehub-2.5.2.post2/types_aiobotocore_resiliencehub/literals.py` & `types-aiobotocore-resiliencehub-2.5.4/types_aiobotocore_resiliencehub/literals.py`

 * *Files 18% similar despite different names*

```diff
@@ -19,31 +19,24 @@
     from typing_extensions import Literal
 
 
 __all__ = (
     "AlarmTypeType",
     "AppAssessmentScheduleTypeType",
     "AppComplianceStatusTypeType",
-    "AppDriftStatusTypeType",
     "AppStatusTypeType",
     "AssessmentInvokerType",
     "AssessmentStatusType",
     "ComplianceStatusType",
     "ConfigRecommendationOptimizationTypeType",
     "CostFrequencyType",
     "DataLocationConstraintType",
-    "DifferenceTypeType",
     "DisruptionTypeType",
-    "DriftStatusType",
-    "DriftTypeType",
     "EstimatedCostTierType",
-    "EventTypeType",
-    "ExcludeRecommendationReasonType",
     "HaArchitectureType",
-    "PermissionModelTypeType",
     "PhysicalIdentifierTypeType",
     "RecommendationComplianceStatusType",
     "RecommendationTemplateStatusType",
     "RenderRecommendationTypeType",
     "ResiliencyPolicyTierType",
     "ResourceImportStatusTypeType",
     "ResourceImportStrategyTypeType",
@@ -62,50 +55,41 @@
 
 
 AlarmTypeType = Literal["Canary", "Composite", "Event", "Logs", "Metric"]
 AppAssessmentScheduleTypeType = Literal["Daily", "Disabled"]
 AppComplianceStatusTypeType = Literal[
     "ChangesDetected", "NotAssessed", "PolicyBreached", "PolicyMet"
 ]
-AppDriftStatusTypeType = Literal["Detected", "NotChecked", "NotDetected"]
 AppStatusTypeType = Literal["Active", "Deleting"]
 AssessmentInvokerType = Literal["System", "User"]
 AssessmentStatusType = Literal["Failed", "InProgress", "Pending", "Success"]
 ComplianceStatusType = Literal["PolicyBreached", "PolicyMet"]
 ConfigRecommendationOptimizationTypeType = Literal[
     "BestAZRecovery",
     "BestAttainable",
     "BestRegionRecovery",
     "LeastChange",
     "LeastCost",
     "LeastErrors",
 ]
 CostFrequencyType = Literal["Daily", "Hourly", "Monthly", "Yearly"]
 DataLocationConstraintType = Literal["AnyLocation", "SameContinent", "SameCountry"]
-DifferenceTypeType = Literal["NotEqual"]
 DisruptionTypeType = Literal["AZ", "Hardware", "Region", "Software"]
-DriftStatusType = Literal["Detected", "NotChecked", "NotDetected"]
-DriftTypeType = Literal["ApplicationCompliance"]
 EstimatedCostTierType = Literal["L1", "L2", "L3", "L4"]
-EventTypeType = Literal["DriftDetected", "ScheduledAssessmentFailure"]
-ExcludeRecommendationReasonType = Literal[
-    "AlreadyImplemented", "ComplexityOfImplementation", "NotRelevant"
-]
 HaArchitectureType = Literal[
     "BackupAndRestore", "MultiSite", "NoRecoveryPlan", "PilotLight", "WarmStandby"
 ]
-PermissionModelTypeType = Literal["LegacyIAMUser", "RoleBased"]
 PhysicalIdentifierTypeType = Literal["Arn", "Native"]
 RecommendationComplianceStatusType = Literal[
     "BreachedCanMeet", "BreachedUnattainable", "MetCanImprove"
 ]
 RecommendationTemplateStatusType = Literal["Failed", "InProgress", "Pending", "Success"]
 RenderRecommendationTypeType = Literal["Alarm", "Sop", "Test"]
 ResiliencyPolicyTierType = Literal[
-    "CoreServices", "Critical", "Important", "MissionCritical", "NonCritical", "NotApplicable"
+    "CoreServices", "Critical", "Important", "MissionCritical", "NonCritical"
 ]
 ResourceImportStatusTypeType = Literal["Failed", "InProgress", "Pending", "Success"]
 ResourceImportStrategyTypeType = Literal["AddOnly", "ReplaceAll"]
 ResourceMappingTypeType = Literal[
     "AppRegistryApp", "CfnStack", "EKS", "Resource", "ResourceGroup", "Terraform"
 ]
 ResourceResolutionStatusTypeType = Literal["Failed", "InProgress", "Pending", "Success"]
```

### Comparing `types-aiobotocore-resiliencehub-2.5.2.post2/types_aiobotocore_resiliencehub/literals.pyi` & `types-aiobotocore-resiliencehub-2.5.4/types_aiobotocore_resiliencehub/literals.pyi`

 * *Files 18% similar despite different names*

```diff
@@ -18,31 +18,24 @@
 else:
     from typing_extensions import Literal
 
 __all__ = (
     "AlarmTypeType",
     "AppAssessmentScheduleTypeType",
     "AppComplianceStatusTypeType",
-    "AppDriftStatusTypeType",
     "AppStatusTypeType",
     "AssessmentInvokerType",
     "AssessmentStatusType",
     "ComplianceStatusType",
     "ConfigRecommendationOptimizationTypeType",
     "CostFrequencyType",
     "DataLocationConstraintType",
-    "DifferenceTypeType",
     "DisruptionTypeType",
-    "DriftStatusType",
-    "DriftTypeType",
     "EstimatedCostTierType",
-    "EventTypeType",
-    "ExcludeRecommendationReasonType",
     "HaArchitectureType",
-    "PermissionModelTypeType",
     "PhysicalIdentifierTypeType",
     "RecommendationComplianceStatusType",
     "RecommendationTemplateStatusType",
     "RenderRecommendationTypeType",
     "ResiliencyPolicyTierType",
     "ResourceImportStatusTypeType",
     "ResourceImportStrategyTypeType",
@@ -60,50 +53,41 @@
 )
 
 AlarmTypeType = Literal["Canary", "Composite", "Event", "Logs", "Metric"]
 AppAssessmentScheduleTypeType = Literal["Daily", "Disabled"]
 AppComplianceStatusTypeType = Literal[
     "ChangesDetected", "NotAssessed", "PolicyBreached", "PolicyMet"
 ]
-AppDriftStatusTypeType = Literal["Detected", "NotChecked", "NotDetected"]
 AppStatusTypeType = Literal["Active", "Deleting"]
 AssessmentInvokerType = Literal["System", "User"]
 AssessmentStatusType = Literal["Failed", "InProgress", "Pending", "Success"]
 ComplianceStatusType = Literal["PolicyBreached", "PolicyMet"]
 ConfigRecommendationOptimizationTypeType = Literal[
     "BestAZRecovery",
     "BestAttainable",
     "BestRegionRecovery",
     "LeastChange",
     "LeastCost",
     "LeastErrors",
 ]
 CostFrequencyType = Literal["Daily", "Hourly", "Monthly", "Yearly"]
 DataLocationConstraintType = Literal["AnyLocation", "SameContinent", "SameCountry"]
-DifferenceTypeType = Literal["NotEqual"]
 DisruptionTypeType = Literal["AZ", "Hardware", "Region", "Software"]
-DriftStatusType = Literal["Detected", "NotChecked", "NotDetected"]
-DriftTypeType = Literal["ApplicationCompliance"]
 EstimatedCostTierType = Literal["L1", "L2", "L3", "L4"]
-EventTypeType = Literal["DriftDetected", "ScheduledAssessmentFailure"]
-ExcludeRecommendationReasonType = Literal[
-    "AlreadyImplemented", "ComplexityOfImplementation", "NotRelevant"
-]
 HaArchitectureType = Literal[
     "BackupAndRestore", "MultiSite", "NoRecoveryPlan", "PilotLight", "WarmStandby"
 ]
-PermissionModelTypeType = Literal["LegacyIAMUser", "RoleBased"]
 PhysicalIdentifierTypeType = Literal["Arn", "Native"]
 RecommendationComplianceStatusType = Literal[
     "BreachedCanMeet", "BreachedUnattainable", "MetCanImprove"
 ]
 RecommendationTemplateStatusType = Literal["Failed", "InProgress", "Pending", "Success"]
 RenderRecommendationTypeType = Literal["Alarm", "Sop", "Test"]
 ResiliencyPolicyTierType = Literal[
-    "CoreServices", "Critical", "Important", "MissionCritical", "NonCritical", "NotApplicable"
+    "CoreServices", "Critical", "Important", "MissionCritical", "NonCritical"
 ]
 ResourceImportStatusTypeType = Literal["Failed", "InProgress", "Pending", "Success"]
 ResourceImportStrategyTypeType = Literal["AddOnly", "ReplaceAll"]
 ResourceMappingTypeType = Literal[
     "AppRegistryApp", "CfnStack", "EKS", "Resource", "ResourceGroup", "Terraform"
 ]
 ResourceResolutionStatusTypeType = Literal["Failed", "InProgress", "Pending", "Success"]
```

### Comparing `types-aiobotocore-resiliencehub-2.5.2.post2/types_aiobotocore_resiliencehub/type_defs.py` & `types-aiobotocore-resiliencehub-2.5.4/types_aiobotocore_resiliencehub/type_defs.py`

 * *Files 5% similar despite different names*

```diff
@@ -9,35 +9,30 @@
     from types_aiobotocore_resiliencehub.type_defs import ResponseMetadataTypeDef
 
     data: ResponseMetadataTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
-from typing import Dict, List, Mapping, Sequence, Union
+from typing import Dict, List, Mapping, Sequence
 
 from .literals import (
     AlarmTypeType,
     AppAssessmentScheduleTypeType,
     AppComplianceStatusTypeType,
-    AppDriftStatusTypeType,
     AppStatusTypeType,
     AssessmentInvokerType,
     AssessmentStatusType,
     ComplianceStatusType,
     ConfigRecommendationOptimizationTypeType,
     CostFrequencyType,
     DataLocationConstraintType,
     DisruptionTypeType,
-    DriftStatusType,
     EstimatedCostTierType,
-    EventTypeType,
-    ExcludeRecommendationReasonType,
     HaArchitectureType,
-    PermissionModelTypeType,
     PhysicalIdentifierTypeType,
     RecommendationComplianceStatusType,
     RecommendationTemplateStatusType,
     RenderRecommendationTypeType,
     ResiliencyPolicyTierType,
     ResourceImportStatusTypeType,
     ResourceImportStrategyTypeType,
@@ -65,20 +60,18 @@
     "CostTypeDef",
     "DisruptionComplianceTypeDef",
     "ResiliencyScoreTypeDef",
     "AppComponentTypeDef",
     "EksSourceClusterNamespaceTypeDef",
     "TerraformSourceTypeDef",
     "AppSummaryTypeDef",
-    "EventSubscriptionTypeDef",
-    "PermissionModelTypeDef",
+    "AppTypeDef",
     "AppVersionSummaryTypeDef",
-    "BatchUpdateRecommendationStatusFailedEntryTypeDef",
-    "UpdateRecommendationStatusItemTypeDef",
     "RecommendationDisruptionComplianceTypeDef",
+    "CreateAppRequestRequestTypeDef",
     "CreateAppVersionAppComponentRequestRequestTypeDef",
     "LogicalResourceIdTypeDef",
     "CreateRecommendationTemplateRequestRequestTypeDef",
     "FailurePolicyTypeDef",
     "DeleteAppAssessmentRequestRequestTypeDef",
     "DeleteAppRequestRequestTypeDef",
     "DeleteAppVersionAppComponentRequestRequestTypeDef",
@@ -90,23 +83,22 @@
     "DescribeAppVersionRequestRequestTypeDef",
     "DescribeAppVersionResourcesResolutionStatusRequestRequestTypeDef",
     "DescribeAppVersionTemplateRequestRequestTypeDef",
     "DescribeDraftAppVersionResourcesImportStatusRequestRequestTypeDef",
     "DescribeResiliencyPolicyRequestRequestTypeDef",
     "EksSourceTypeDef",
     "ListAlarmRecommendationsRequestRequestTypeDef",
-    "ListAppAssessmentComplianceDriftsRequestRequestTypeDef",
     "ListAppAssessmentsRequestRequestTypeDef",
     "ListAppComponentCompliancesRequestRequestTypeDef",
     "ListAppComponentRecommendationsRequestRequestTypeDef",
     "ListAppInputSourcesRequestRequestTypeDef",
     "ListAppVersionAppComponentsRequestRequestTypeDef",
     "ListAppVersionResourceMappingsRequestRequestTypeDef",
     "ListAppVersionResourcesRequestRequestTypeDef",
-    "TimestampTypeDef",
+    "ListAppVersionsRequestRequestTypeDef",
     "ListAppsRequestRequestTypeDef",
     "ListRecommendationTemplatesRequestRequestTypeDef",
     "ListResiliencyPoliciesRequestRequestTypeDef",
     "ListSopRecommendationsRequestRequestTypeDef",
     "ListSuggestedResiliencyPoliciesRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
     "ListTestRecommendationsRequestRequestTypeDef",
@@ -117,14 +109,15 @@
     "S3LocationTypeDef",
     "RemoveDraftAppVersionResourceMappingsRequestRequestTypeDef",
     "ResolveAppVersionResourcesRequestRequestTypeDef",
     "ResourceErrorTypeDef",
     "StartAppAssessmentRequestRequestTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
+    "UpdateAppRequestRequestTypeDef",
     "UpdateAppVersionAppComponentRequestRequestTypeDef",
     "UpdateAppVersionRequestRequestTypeDef",
     "DeleteAppAssessmentResponseTypeDef",
     "DeleteAppResponseTypeDef",
     "DeleteRecommendationTemplateResponseTypeDef",
     "DeleteResiliencyPolicyResponseTypeDef",
     "DescribeAppVersionResourcesResolutionStatusResponseTypeDef",
@@ -137,59 +130,49 @@
     "RemoveDraftAppVersionResourceMappingsResponseTypeDef",
     "ResolveAppVersionResourcesResponseTypeDef",
     "UpdateAppVersionResponseTypeDef",
     "AlarmRecommendationTypeDef",
     "SopRecommendationTypeDef",
     "TestRecommendationTypeDef",
     "AppAssessmentSummaryTypeDef",
-    "ComplianceDriftTypeDef",
     "AppComponentComplianceTypeDef",
     "CreateAppVersionAppComponentResponseTypeDef",
     "DeleteAppVersionAppComponentResponseTypeDef",
     "DescribeAppVersionAppComponentResponseTypeDef",
     "ListAppVersionAppComponentsResponseTypeDef",
     "UpdateAppVersionAppComponentResponseTypeDef",
     "AppInputSourceTypeDef",
     "DeleteAppInputSourceRequestRequestTypeDef",
     "ListAppsResponseTypeDef",
-    "AppTypeDef",
-    "CreateAppRequestRequestTypeDef",
-    "UpdateAppRequestRequestTypeDef",
+    "CreateAppResponseTypeDef",
+    "DescribeAppResponseTypeDef",
+    "UpdateAppResponseTypeDef",
     "ListAppVersionsResponseTypeDef",
-    "BatchUpdateRecommendationStatusSuccessfulEntryTypeDef",
-    "UpdateRecommendationStatusRequestEntryTypeDef",
     "ConfigRecommendationTypeDef",
     "CreateAppVersionResourceRequestRequestTypeDef",
     "DeleteAppVersionResourceRequestRequestTypeDef",
     "DescribeAppVersionResourceRequestRequestTypeDef",
     "UpdateAppVersionResourceRequestRequestTypeDef",
     "CreateResiliencyPolicyRequestRequestTypeDef",
     "ResiliencyPolicyTypeDef",
     "UpdateResiliencyPolicyRequestRequestTypeDef",
     "ImportResourcesToDraftAppVersionRequestRequestTypeDef",
     "ImportResourcesToDraftAppVersionResponseTypeDef",
-    "ListAppVersionsRequestRequestTypeDef",
     "PhysicalResourceTypeDef",
     "ResourceMappingTypeDef",
     "UnsupportedResourceTypeDef",
     "RecommendationTemplateTypeDef",
     "ResourceErrorsDetailsTypeDef",
     "ListAlarmRecommendationsResponseTypeDef",
     "ListSopRecommendationsResponseTypeDef",
     "ListTestRecommendationsResponseTypeDef",
     "ListAppAssessmentsResponseTypeDef",
-    "ListAppAssessmentComplianceDriftsResponseTypeDef",
     "ListAppComponentCompliancesResponseTypeDef",
     "DeleteAppInputSourceResponseTypeDef",
     "ListAppInputSourcesResponseTypeDef",
-    "CreateAppResponseTypeDef",
-    "DescribeAppResponseTypeDef",
-    "UpdateAppResponseTypeDef",
-    "BatchUpdateRecommendationStatusResponseTypeDef",
-    "BatchUpdateRecommendationStatusRequestRequestTypeDef",
     "ComponentRecommendationTypeDef",
     "CreateResiliencyPolicyResponseTypeDef",
     "DescribeResiliencyPolicyResponseTypeDef",
     "ListResiliencyPoliciesResponseTypeDef",
     "ListSuggestedResiliencyPoliciesResponseTypeDef",
     "UpdateResiliencyPolicyResponseTypeDef",
     "CreateAppVersionResourceResponseTypeDef",
@@ -220,16 +203,14 @@
     },
 )
 
 RecommendationItemTypeDef = TypedDict(
     "RecommendationItemTypeDef",
     {
         "alreadyImplemented": bool,
-        "excludeReason": ExcludeRecommendationReasonType,
-        "excluded": bool,
         "resourceId": str,
         "targetAccountId": str,
         "targetRegion": str,
     },
     total=False,
 )
 
@@ -325,108 +306,60 @@
 )
 _OptionalAppSummaryTypeDef = TypedDict(
     "_OptionalAppSummaryTypeDef",
     {
         "assessmentSchedule": AppAssessmentScheduleTypeType,
         "complianceStatus": AppComplianceStatusTypeType,
         "description": str,
-        "driftStatus": AppDriftStatusTypeType,
         "resiliencyScore": float,
         "status": AppStatusTypeType,
     },
     total=False,
 )
 
 
 class AppSummaryTypeDef(_RequiredAppSummaryTypeDef, _OptionalAppSummaryTypeDef):
     pass
 
 
-_RequiredEventSubscriptionTypeDef = TypedDict(
-    "_RequiredEventSubscriptionTypeDef",
+_RequiredAppTypeDef = TypedDict(
+    "_RequiredAppTypeDef",
     {
-        "eventType": EventTypeType,
+        "appArn": str,
+        "creationTime": datetime,
         "name": str,
     },
 )
-_OptionalEventSubscriptionTypeDef = TypedDict(
-    "_OptionalEventSubscriptionTypeDef",
-    {
-        "snsTopicArn": str,
-    },
-    total=False,
-)
-
-
-class EventSubscriptionTypeDef(
-    _RequiredEventSubscriptionTypeDef, _OptionalEventSubscriptionTypeDef
-):
-    pass
-
-
-_RequiredPermissionModelTypeDef = TypedDict(
-    "_RequiredPermissionModelTypeDef",
-    {
-        "type": PermissionModelTypeType,
-    },
-)
-_OptionalPermissionModelTypeDef = TypedDict(
-    "_OptionalPermissionModelTypeDef",
+_OptionalAppTypeDef = TypedDict(
+    "_OptionalAppTypeDef",
     {
-        "crossAccountRoleArns": Sequence[str],
-        "invokerRoleName": str,
+        "assessmentSchedule": AppAssessmentScheduleTypeType,
+        "complianceStatus": AppComplianceStatusTypeType,
+        "description": str,
+        "lastAppComplianceEvaluationTime": datetime,
+        "lastResiliencyScoreEvaluationTime": datetime,
+        "policyArn": str,
+        "resiliencyScore": float,
+        "status": AppStatusTypeType,
+        "tags": Dict[str, str],
     },
     total=False,
 )
 
 
-class PermissionModelTypeDef(_RequiredPermissionModelTypeDef, _OptionalPermissionModelTypeDef):
+class AppTypeDef(_RequiredAppTypeDef, _OptionalAppTypeDef):
     pass
 
 
-_RequiredAppVersionSummaryTypeDef = TypedDict(
-    "_RequiredAppVersionSummaryTypeDef",
+AppVersionSummaryTypeDef = TypedDict(
+    "AppVersionSummaryTypeDef",
     {
         "appVersion": str,
     },
 )
-_OptionalAppVersionSummaryTypeDef = TypedDict(
-    "_OptionalAppVersionSummaryTypeDef",
-    {
-        "creationTime": datetime,
-        "identifier": int,
-        "versionName": str,
-    },
-    total=False,
-)
-
-
-class AppVersionSummaryTypeDef(
-    _RequiredAppVersionSummaryTypeDef, _OptionalAppVersionSummaryTypeDef
-):
-    pass
-
-
-BatchUpdateRecommendationStatusFailedEntryTypeDef = TypedDict(
-    "BatchUpdateRecommendationStatusFailedEntryTypeDef",
-    {
-        "entryId": str,
-        "errorMessage": str,
-    },
-)
-
-UpdateRecommendationStatusItemTypeDef = TypedDict(
-    "UpdateRecommendationStatusItemTypeDef",
-    {
-        "resourceId": str,
-        "targetAccountId": str,
-        "targetRegion": str,
-    },
-    total=False,
-)
 
 _RequiredRecommendationDisruptionComplianceTypeDef = TypedDict(
     "_RequiredRecommendationDisruptionComplianceTypeDef",
     {
         "expectedComplianceStatus": ComplianceStatusType,
     },
 )
@@ -445,14 +378,39 @@
 class RecommendationDisruptionComplianceTypeDef(
     _RequiredRecommendationDisruptionComplianceTypeDef,
     _OptionalRecommendationDisruptionComplianceTypeDef,
 ):
     pass
 
 
+_RequiredCreateAppRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateAppRequestRequestTypeDef",
+    {
+        "name": str,
+    },
+)
+_OptionalCreateAppRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateAppRequestRequestTypeDef",
+    {
+        "assessmentSchedule": AppAssessmentScheduleTypeType,
+        "clientToken": str,
+        "description": str,
+        "policyArn": str,
+        "tags": Mapping[str, str],
+    },
+    total=False,
+)
+
+
+class CreateAppRequestRequestTypeDef(
+    _RequiredCreateAppRequestRequestTypeDef, _OptionalCreateAppRequestRequestTypeDef
+):
+    pass
+
+
 _RequiredCreateAppVersionAppComponentRequestRequestTypeDef = TypedDict(
     "_RequiredCreateAppVersionAppComponentRequestRequestTypeDef",
     {
         "appArn": str,
         "name": str,
         "type": str,
     },
@@ -749,37 +707,14 @@
 class ListAlarmRecommendationsRequestRequestTypeDef(
     _RequiredListAlarmRecommendationsRequestRequestTypeDef,
     _OptionalListAlarmRecommendationsRequestRequestTypeDef,
 ):
     pass
 
 
-_RequiredListAppAssessmentComplianceDriftsRequestRequestTypeDef = TypedDict(
-    "_RequiredListAppAssessmentComplianceDriftsRequestRequestTypeDef",
-    {
-        "assessmentArn": str,
-    },
-)
-_OptionalListAppAssessmentComplianceDriftsRequestRequestTypeDef = TypedDict(
-    "_OptionalListAppAssessmentComplianceDriftsRequestRequestTypeDef",
-    {
-        "maxResults": int,
-        "nextToken": str,
-    },
-    total=False,
-)
-
-
-class ListAppAssessmentComplianceDriftsRequestRequestTypeDef(
-    _RequiredListAppAssessmentComplianceDriftsRequestRequestTypeDef,
-    _OptionalListAppAssessmentComplianceDriftsRequestRequestTypeDef,
-):
-    pass
-
-
 ListAppAssessmentsRequestRequestTypeDef = TypedDict(
     "ListAppAssessmentsRequestRequestTypeDef",
     {
         "appArn": str,
         "assessmentName": str,
         "assessmentStatus": Sequence[AssessmentStatusType],
         "complianceStatus": ComplianceStatusType,
@@ -930,15 +865,36 @@
 class ListAppVersionResourcesRequestRequestTypeDef(
     _RequiredListAppVersionResourcesRequestRequestTypeDef,
     _OptionalListAppVersionResourcesRequestRequestTypeDef,
 ):
     pass
 
 
-TimestampTypeDef = Union[datetime, str]
+_RequiredListAppVersionsRequestRequestTypeDef = TypedDict(
+    "_RequiredListAppVersionsRequestRequestTypeDef",
+    {
+        "appArn": str,
+    },
+)
+_OptionalListAppVersionsRequestRequestTypeDef = TypedDict(
+    "_OptionalListAppVersionsRequestRequestTypeDef",
+    {
+        "maxResults": int,
+        "nextToken": str,
+    },
+    total=False,
+)
+
+
+class ListAppVersionsRequestRequestTypeDef(
+    _RequiredListAppVersionsRequestRequestTypeDef, _OptionalListAppVersionsRequestRequestTypeDef
+):
+    pass
+
+
 ListAppsRequestRequestTypeDef = TypedDict(
     "ListAppsRequestRequestTypeDef",
     {
         "appArn": str,
         "maxResults": int,
         "name": str,
         "nextToken": str,
@@ -1089,34 +1045,20 @@
 
 class PhysicalResourceIdTypeDef(
     _RequiredPhysicalResourceIdTypeDef, _OptionalPhysicalResourceIdTypeDef
 ):
     pass
 
 
-_RequiredPublishAppVersionRequestRequestTypeDef = TypedDict(
-    "_RequiredPublishAppVersionRequestRequestTypeDef",
+PublishAppVersionRequestRequestTypeDef = TypedDict(
+    "PublishAppVersionRequestRequestTypeDef",
     {
         "appArn": str,
     },
 )
-_OptionalPublishAppVersionRequestRequestTypeDef = TypedDict(
-    "_OptionalPublishAppVersionRequestRequestTypeDef",
-    {
-        "versionName": str,
-    },
-    total=False,
-)
-
-
-class PublishAppVersionRequestRequestTypeDef(
-    _RequiredPublishAppVersionRequestRequestTypeDef, _OptionalPublishAppVersionRequestRequestTypeDef
-):
-    pass
-
 
 PutDraftAppVersionTemplateRequestRequestTypeDef = TypedDict(
     "PutDraftAppVersionTemplateRequestRequestTypeDef",
     {
         "appArn": str,
         "appTemplateBody": str,
     },
@@ -1213,14 +1155,38 @@
     "UntagResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
         "tagKeys": Sequence[str],
     },
 )
 
+_RequiredUpdateAppRequestRequestTypeDef = TypedDict(
+    "_RequiredUpdateAppRequestRequestTypeDef",
+    {
+        "appArn": str,
+    },
+)
+_OptionalUpdateAppRequestRequestTypeDef = TypedDict(
+    "_OptionalUpdateAppRequestRequestTypeDef",
+    {
+        "assessmentSchedule": AppAssessmentScheduleTypeType,
+        "clearResiliencyPolicyArn": bool,
+        "description": str,
+        "policyArn": str,
+    },
+    total=False,
+)
+
+
+class UpdateAppRequestRequestTypeDef(
+    _RequiredUpdateAppRequestRequestTypeDef, _OptionalUpdateAppRequestRequestTypeDef
+):
+    pass
+
+
 _RequiredUpdateAppVersionAppComponentRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateAppVersionAppComponentRequestRequestTypeDef",
     {
         "appArn": str,
         "id": str,
     },
 )
@@ -1350,16 +1316,14 @@
 )
 
 PublishAppVersionResponseTypeDef = TypedDict(
     "PublishAppVersionResponseTypeDef",
     {
         "appArn": str,
         "appVersion": str,
-        "identifier": int,
-        "versionName": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 PutDraftAppVersionTemplateResponseTypeDef = TypedDict(
     "PutDraftAppVersionTemplateResponseTypeDef",
     {
@@ -1408,15 +1372,14 @@
         "type": AlarmTypeType,
     },
 )
 _OptionalAlarmRecommendationTypeDef = TypedDict(
     "_OptionalAlarmRecommendationTypeDef",
     {
         "appComponentName": str,
-        "appComponentNames": List[str],
         "description": str,
         "items": List[RecommendationItemTypeDef],
         "prerequisite": str,
     },
     total=False,
 )
 
@@ -1495,49 +1458,30 @@
     "_OptionalAppAssessmentSummaryTypeDef",
     {
         "appArn": str,
         "appVersion": str,
         "assessmentName": str,
         "complianceStatus": ComplianceStatusType,
         "cost": CostTypeDef,
-        "driftStatus": DriftStatusType,
         "endTime": datetime,
         "invoker": AssessmentInvokerType,
         "message": str,
         "resiliencyScore": float,
         "startTime": datetime,
-        "versionName": str,
     },
     total=False,
 )
 
 
 class AppAssessmentSummaryTypeDef(
     _RequiredAppAssessmentSummaryTypeDef, _OptionalAppAssessmentSummaryTypeDef
 ):
     pass
 
 
-ComplianceDriftTypeDef = TypedDict(
-    "ComplianceDriftTypeDef",
-    {
-        "actualReferenceId": str,
-        "actualValue": Dict[DisruptionTypeType, DisruptionComplianceTypeDef],
-        "appId": str,
-        "appVersion": str,
-        "diffType": Literal["NotEqual"],
-        "driftType": Literal["ApplicationCompliance"],
-        "entityId": str,
-        "entityType": str,
-        "expectedReferenceId": str,
-        "expectedValue": Dict[DisruptionTypeType, DisruptionComplianceTypeDef],
-    },
-    total=False,
-)
-
 AppComponentComplianceTypeDef = TypedDict(
     "AppComponentComplianceTypeDef",
     {
         "appComponentName": str,
         "compliance": Dict[DisruptionTypeType, DisruptionComplianceTypeDef],
         "cost": CostTypeDef,
         "message": str,
@@ -1651,159 +1595,47 @@
     {
         "appSummaries": List[AppSummaryTypeDef],
         "nextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredAppTypeDef = TypedDict(
-    "_RequiredAppTypeDef",
+CreateAppResponseTypeDef = TypedDict(
+    "CreateAppResponseTypeDef",
     {
-        "appArn": str,
-        "creationTime": datetime,
-        "name": str,
+        "app": AppTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
-_OptionalAppTypeDef = TypedDict(
-    "_OptionalAppTypeDef",
-    {
-        "assessmentSchedule": AppAssessmentScheduleTypeType,
-        "complianceStatus": AppComplianceStatusTypeType,
-        "description": str,
-        "driftStatus": AppDriftStatusTypeType,
-        "eventSubscriptions": List[EventSubscriptionTypeDef],
-        "lastAppComplianceEvaluationTime": datetime,
-        "lastDriftEvaluationTime": datetime,
-        "lastResiliencyScoreEvaluationTime": datetime,
-        "permissionModel": PermissionModelTypeDef,
-        "policyArn": str,
-        "resiliencyScore": float,
-        "status": AppStatusTypeType,
-        "tags": Dict[str, str],
-    },
-    total=False,
-)
-
-
-class AppTypeDef(_RequiredAppTypeDef, _OptionalAppTypeDef):
-    pass
-
 
-_RequiredCreateAppRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateAppRequestRequestTypeDef",
-    {
-        "name": str,
-    },
-)
-_OptionalCreateAppRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateAppRequestRequestTypeDef",
+DescribeAppResponseTypeDef = TypedDict(
+    "DescribeAppResponseTypeDef",
     {
-        "assessmentSchedule": AppAssessmentScheduleTypeType,
-        "clientToken": str,
-        "description": str,
-        "eventSubscriptions": Sequence[EventSubscriptionTypeDef],
-        "permissionModel": PermissionModelTypeDef,
-        "policyArn": str,
-        "tags": Mapping[str, str],
+        "app": AppTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
-
-class CreateAppRequestRequestTypeDef(
-    _RequiredCreateAppRequestRequestTypeDef, _OptionalCreateAppRequestRequestTypeDef
-):
-    pass
-
-
-_RequiredUpdateAppRequestRequestTypeDef = TypedDict(
-    "_RequiredUpdateAppRequestRequestTypeDef",
-    {
-        "appArn": str,
-    },
-)
-_OptionalUpdateAppRequestRequestTypeDef = TypedDict(
-    "_OptionalUpdateAppRequestRequestTypeDef",
+UpdateAppResponseTypeDef = TypedDict(
+    "UpdateAppResponseTypeDef",
     {
-        "assessmentSchedule": AppAssessmentScheduleTypeType,
-        "clearResiliencyPolicyArn": bool,
-        "description": str,
-        "eventSubscriptions": Sequence[EventSubscriptionTypeDef],
-        "permissionModel": PermissionModelTypeDef,
-        "policyArn": str,
+        "app": AppTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
-
-class UpdateAppRequestRequestTypeDef(
-    _RequiredUpdateAppRequestRequestTypeDef, _OptionalUpdateAppRequestRequestTypeDef
-):
-    pass
-
-
 ListAppVersionsResponseTypeDef = TypedDict(
     "ListAppVersionsResponseTypeDef",
     {
         "appVersions": List[AppVersionSummaryTypeDef],
         "nextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredBatchUpdateRecommendationStatusSuccessfulEntryTypeDef = TypedDict(
-    "_RequiredBatchUpdateRecommendationStatusSuccessfulEntryTypeDef",
-    {
-        "entryId": str,
-        "excluded": bool,
-        "item": UpdateRecommendationStatusItemTypeDef,
-        "referenceId": str,
-    },
-)
-_OptionalBatchUpdateRecommendationStatusSuccessfulEntryTypeDef = TypedDict(
-    "_OptionalBatchUpdateRecommendationStatusSuccessfulEntryTypeDef",
-    {
-        "excludeReason": ExcludeRecommendationReasonType,
-    },
-    total=False,
-)
-
-
-class BatchUpdateRecommendationStatusSuccessfulEntryTypeDef(
-    _RequiredBatchUpdateRecommendationStatusSuccessfulEntryTypeDef,
-    _OptionalBatchUpdateRecommendationStatusSuccessfulEntryTypeDef,
-):
-    pass
-
-
-_RequiredUpdateRecommendationStatusRequestEntryTypeDef = TypedDict(
-    "_RequiredUpdateRecommendationStatusRequestEntryTypeDef",
-    {
-        "entryId": str,
-        "excluded": bool,
-        "item": UpdateRecommendationStatusItemTypeDef,
-        "referenceId": str,
-    },
-)
-_OptionalUpdateRecommendationStatusRequestEntryTypeDef = TypedDict(
-    "_OptionalUpdateRecommendationStatusRequestEntryTypeDef",
-    {
-        "excludeReason": ExcludeRecommendationReasonType,
-    },
-    total=False,
-)
-
-
-class UpdateRecommendationStatusRequestEntryTypeDef(
-    _RequiredUpdateRecommendationStatusRequestEntryTypeDef,
-    _OptionalUpdateRecommendationStatusRequestEntryTypeDef,
-):
-    pass
-
-
 _RequiredConfigRecommendationTypeDef = TypedDict(
     "_RequiredConfigRecommendationTypeDef",
     {
         "name": str,
         "optimizationType": ConfigRecommendationOptimizationTypeType,
         "referenceId": str,
     },
@@ -2048,38 +1880,14 @@
         "sourceArns": List[str],
         "status": ResourceImportStatusTypeType,
         "terraformSources": List[TerraformSourceTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredListAppVersionsRequestRequestTypeDef = TypedDict(
-    "_RequiredListAppVersionsRequestRequestTypeDef",
-    {
-        "appArn": str,
-    },
-)
-_OptionalListAppVersionsRequestRequestTypeDef = TypedDict(
-    "_OptionalListAppVersionsRequestRequestTypeDef",
-    {
-        "endTime": TimestampTypeDef,
-        "maxResults": int,
-        "nextToken": str,
-        "startTime": TimestampTypeDef,
-    },
-    total=False,
-)
-
-
-class ListAppVersionsRequestRequestTypeDef(
-    _RequiredListAppVersionsRequestRequestTypeDef, _OptionalListAppVersionsRequestRequestTypeDef
-):
-    pass
-
-
 _RequiredPhysicalResourceTypeDef = TypedDict(
     "_RequiredPhysicalResourceTypeDef",
     {
         "logicalResourceId": LogicalResourceIdTypeDef,
         "physicalResourceId": PhysicalResourceIdTypeDef,
         "resourceType": str,
     },
@@ -2224,23 +2032,14 @@
     {
         "assessmentSummaries": List[AppAssessmentSummaryTypeDef],
         "nextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-ListAppAssessmentComplianceDriftsResponseTypeDef = TypedDict(
-    "ListAppAssessmentComplianceDriftsResponseTypeDef",
-    {
-        "complianceDrifts": List[ComplianceDriftTypeDef],
-        "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 ListAppComponentCompliancesResponseTypeDef = TypedDict(
     "ListAppComponentCompliancesResponseTypeDef",
     {
         "componentCompliances": List[AppComponentComplianceTypeDef],
         "nextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -2260,56 +2059,14 @@
     {
         "appInputSources": List[AppInputSourceTypeDef],
         "nextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-CreateAppResponseTypeDef = TypedDict(
-    "CreateAppResponseTypeDef",
-    {
-        "app": AppTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DescribeAppResponseTypeDef = TypedDict(
-    "DescribeAppResponseTypeDef",
-    {
-        "app": AppTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-UpdateAppResponseTypeDef = TypedDict(
-    "UpdateAppResponseTypeDef",
-    {
-        "app": AppTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-BatchUpdateRecommendationStatusResponseTypeDef = TypedDict(
-    "BatchUpdateRecommendationStatusResponseTypeDef",
-    {
-        "appArn": str,
-        "failedEntries": List[BatchUpdateRecommendationStatusFailedEntryTypeDef],
-        "successfulEntries": List[BatchUpdateRecommendationStatusSuccessfulEntryTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-BatchUpdateRecommendationStatusRequestRequestTypeDef = TypedDict(
-    "BatchUpdateRecommendationStatusRequestRequestTypeDef",
-    {
-        "appArn": str,
-        "requestEntries": Sequence[UpdateRecommendationStatusRequestEntryTypeDef],
-    },
-)
-
 ComponentRecommendationTypeDef = TypedDict(
     "ComponentRecommendationTypeDef",
     {
         "appComponentName": str,
         "configRecommendations": List[ConfigRecommendationTypeDef],
         "recommendationStatus": RecommendationComplianceStatusType,
     },
@@ -2474,23 +2231,21 @@
     {
         "appArn": str,
         "appVersion": str,
         "assessmentName": str,
         "compliance": Dict[DisruptionTypeType, DisruptionComplianceTypeDef],
         "complianceStatus": ComplianceStatusType,
         "cost": CostTypeDef,
-        "driftStatus": DriftStatusType,
         "endTime": datetime,
         "message": str,
         "policy": ResiliencyPolicyTypeDef,
         "resiliencyScore": ResiliencyScoreTypeDef,
         "resourceErrorsDetails": ResourceErrorsDetailsTypeDef,
         "startTime": datetime,
         "tags": Dict[str, str],
-        "versionName": str,
     },
     total=False,
 )
 
 
 class AppAssessmentTypeDef(_RequiredAppAssessmentTypeDef, _OptionalAppAssessmentTypeDef):
     pass
```

### Comparing `types-aiobotocore-resiliencehub-2.5.2.post2/types_aiobotocore_resiliencehub/type_defs.pyi` & `types-aiobotocore-resiliencehub-2.5.4/types_aiobotocore_resiliencehub/type_defs.pyi`

 * *Files 6% similar despite different names*

```diff
@@ -9,35 +9,30 @@
     from types_aiobotocore_resiliencehub.type_defs import ResponseMetadataTypeDef
 
     data: ResponseMetadataTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
-from typing import Dict, List, Mapping, Sequence, Union
+from typing import Dict, List, Mapping, Sequence
 
 from .literals import (
     AlarmTypeType,
     AppAssessmentScheduleTypeType,
     AppComplianceStatusTypeType,
-    AppDriftStatusTypeType,
     AppStatusTypeType,
     AssessmentInvokerType,
     AssessmentStatusType,
     ComplianceStatusType,
     ConfigRecommendationOptimizationTypeType,
     CostFrequencyType,
     DataLocationConstraintType,
     DisruptionTypeType,
-    DriftStatusType,
     EstimatedCostTierType,
-    EventTypeType,
-    ExcludeRecommendationReasonType,
     HaArchitectureType,
-    PermissionModelTypeType,
     PhysicalIdentifierTypeType,
     RecommendationComplianceStatusType,
     RecommendationTemplateStatusType,
     RenderRecommendationTypeType,
     ResiliencyPolicyTierType,
     ResourceImportStatusTypeType,
     ResourceImportStrategyTypeType,
@@ -64,20 +59,18 @@
     "CostTypeDef",
     "DisruptionComplianceTypeDef",
     "ResiliencyScoreTypeDef",
     "AppComponentTypeDef",
     "EksSourceClusterNamespaceTypeDef",
     "TerraformSourceTypeDef",
     "AppSummaryTypeDef",
-    "EventSubscriptionTypeDef",
-    "PermissionModelTypeDef",
+    "AppTypeDef",
     "AppVersionSummaryTypeDef",
-    "BatchUpdateRecommendationStatusFailedEntryTypeDef",
-    "UpdateRecommendationStatusItemTypeDef",
     "RecommendationDisruptionComplianceTypeDef",
+    "CreateAppRequestRequestTypeDef",
     "CreateAppVersionAppComponentRequestRequestTypeDef",
     "LogicalResourceIdTypeDef",
     "CreateRecommendationTemplateRequestRequestTypeDef",
     "FailurePolicyTypeDef",
     "DeleteAppAssessmentRequestRequestTypeDef",
     "DeleteAppRequestRequestTypeDef",
     "DeleteAppVersionAppComponentRequestRequestTypeDef",
@@ -89,23 +82,22 @@
     "DescribeAppVersionRequestRequestTypeDef",
     "DescribeAppVersionResourcesResolutionStatusRequestRequestTypeDef",
     "DescribeAppVersionTemplateRequestRequestTypeDef",
     "DescribeDraftAppVersionResourcesImportStatusRequestRequestTypeDef",
     "DescribeResiliencyPolicyRequestRequestTypeDef",
     "EksSourceTypeDef",
     "ListAlarmRecommendationsRequestRequestTypeDef",
-    "ListAppAssessmentComplianceDriftsRequestRequestTypeDef",
     "ListAppAssessmentsRequestRequestTypeDef",
     "ListAppComponentCompliancesRequestRequestTypeDef",
     "ListAppComponentRecommendationsRequestRequestTypeDef",
     "ListAppInputSourcesRequestRequestTypeDef",
     "ListAppVersionAppComponentsRequestRequestTypeDef",
     "ListAppVersionResourceMappingsRequestRequestTypeDef",
     "ListAppVersionResourcesRequestRequestTypeDef",
-    "TimestampTypeDef",
+    "ListAppVersionsRequestRequestTypeDef",
     "ListAppsRequestRequestTypeDef",
     "ListRecommendationTemplatesRequestRequestTypeDef",
     "ListResiliencyPoliciesRequestRequestTypeDef",
     "ListSopRecommendationsRequestRequestTypeDef",
     "ListSuggestedResiliencyPoliciesRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
     "ListTestRecommendationsRequestRequestTypeDef",
@@ -116,14 +108,15 @@
     "S3LocationTypeDef",
     "RemoveDraftAppVersionResourceMappingsRequestRequestTypeDef",
     "ResolveAppVersionResourcesRequestRequestTypeDef",
     "ResourceErrorTypeDef",
     "StartAppAssessmentRequestRequestTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
+    "UpdateAppRequestRequestTypeDef",
     "UpdateAppVersionAppComponentRequestRequestTypeDef",
     "UpdateAppVersionRequestRequestTypeDef",
     "DeleteAppAssessmentResponseTypeDef",
     "DeleteAppResponseTypeDef",
     "DeleteRecommendationTemplateResponseTypeDef",
     "DeleteResiliencyPolicyResponseTypeDef",
     "DescribeAppVersionResourcesResolutionStatusResponseTypeDef",
@@ -136,59 +129,49 @@
     "RemoveDraftAppVersionResourceMappingsResponseTypeDef",
     "ResolveAppVersionResourcesResponseTypeDef",
     "UpdateAppVersionResponseTypeDef",
     "AlarmRecommendationTypeDef",
     "SopRecommendationTypeDef",
     "TestRecommendationTypeDef",
     "AppAssessmentSummaryTypeDef",
-    "ComplianceDriftTypeDef",
     "AppComponentComplianceTypeDef",
     "CreateAppVersionAppComponentResponseTypeDef",
     "DeleteAppVersionAppComponentResponseTypeDef",
     "DescribeAppVersionAppComponentResponseTypeDef",
     "ListAppVersionAppComponentsResponseTypeDef",
     "UpdateAppVersionAppComponentResponseTypeDef",
     "AppInputSourceTypeDef",
     "DeleteAppInputSourceRequestRequestTypeDef",
     "ListAppsResponseTypeDef",
-    "AppTypeDef",
-    "CreateAppRequestRequestTypeDef",
-    "UpdateAppRequestRequestTypeDef",
+    "CreateAppResponseTypeDef",
+    "DescribeAppResponseTypeDef",
+    "UpdateAppResponseTypeDef",
     "ListAppVersionsResponseTypeDef",
-    "BatchUpdateRecommendationStatusSuccessfulEntryTypeDef",
-    "UpdateRecommendationStatusRequestEntryTypeDef",
     "ConfigRecommendationTypeDef",
     "CreateAppVersionResourceRequestRequestTypeDef",
     "DeleteAppVersionResourceRequestRequestTypeDef",
     "DescribeAppVersionResourceRequestRequestTypeDef",
     "UpdateAppVersionResourceRequestRequestTypeDef",
     "CreateResiliencyPolicyRequestRequestTypeDef",
     "ResiliencyPolicyTypeDef",
     "UpdateResiliencyPolicyRequestRequestTypeDef",
     "ImportResourcesToDraftAppVersionRequestRequestTypeDef",
     "ImportResourcesToDraftAppVersionResponseTypeDef",
-    "ListAppVersionsRequestRequestTypeDef",
     "PhysicalResourceTypeDef",
     "ResourceMappingTypeDef",
     "UnsupportedResourceTypeDef",
     "RecommendationTemplateTypeDef",
     "ResourceErrorsDetailsTypeDef",
     "ListAlarmRecommendationsResponseTypeDef",
     "ListSopRecommendationsResponseTypeDef",
     "ListTestRecommendationsResponseTypeDef",
     "ListAppAssessmentsResponseTypeDef",
-    "ListAppAssessmentComplianceDriftsResponseTypeDef",
     "ListAppComponentCompliancesResponseTypeDef",
     "DeleteAppInputSourceResponseTypeDef",
     "ListAppInputSourcesResponseTypeDef",
-    "CreateAppResponseTypeDef",
-    "DescribeAppResponseTypeDef",
-    "UpdateAppResponseTypeDef",
-    "BatchUpdateRecommendationStatusResponseTypeDef",
-    "BatchUpdateRecommendationStatusRequestRequestTypeDef",
     "ComponentRecommendationTypeDef",
     "CreateResiliencyPolicyResponseTypeDef",
     "DescribeResiliencyPolicyResponseTypeDef",
     "ListResiliencyPoliciesResponseTypeDef",
     "ListSuggestedResiliencyPoliciesResponseTypeDef",
     "UpdateResiliencyPolicyResponseTypeDef",
     "CreateAppVersionResourceResponseTypeDef",
@@ -219,16 +202,14 @@
     },
 )
 
 RecommendationItemTypeDef = TypedDict(
     "RecommendationItemTypeDef",
     {
         "alreadyImplemented": bool,
-        "excludeReason": ExcludeRecommendationReasonType,
-        "excluded": bool,
         "resourceId": str,
         "targetAccountId": str,
         "targetRegion": str,
     },
     total=False,
 )
 
@@ -320,100 +301,56 @@
 )
 _OptionalAppSummaryTypeDef = TypedDict(
     "_OptionalAppSummaryTypeDef",
     {
         "assessmentSchedule": AppAssessmentScheduleTypeType,
         "complianceStatus": AppComplianceStatusTypeType,
         "description": str,
-        "driftStatus": AppDriftStatusTypeType,
         "resiliencyScore": float,
         "status": AppStatusTypeType,
     },
     total=False,
 )
 
 class AppSummaryTypeDef(_RequiredAppSummaryTypeDef, _OptionalAppSummaryTypeDef):
     pass
 
-_RequiredEventSubscriptionTypeDef = TypedDict(
-    "_RequiredEventSubscriptionTypeDef",
+_RequiredAppTypeDef = TypedDict(
+    "_RequiredAppTypeDef",
     {
-        "eventType": EventTypeType,
+        "appArn": str,
+        "creationTime": datetime,
         "name": str,
     },
 )
-_OptionalEventSubscriptionTypeDef = TypedDict(
-    "_OptionalEventSubscriptionTypeDef",
-    {
-        "snsTopicArn": str,
-    },
-    total=False,
-)
-
-class EventSubscriptionTypeDef(
-    _RequiredEventSubscriptionTypeDef, _OptionalEventSubscriptionTypeDef
-):
-    pass
-
-_RequiredPermissionModelTypeDef = TypedDict(
-    "_RequiredPermissionModelTypeDef",
-    {
-        "type": PermissionModelTypeType,
-    },
-)
-_OptionalPermissionModelTypeDef = TypedDict(
-    "_OptionalPermissionModelTypeDef",
+_OptionalAppTypeDef = TypedDict(
+    "_OptionalAppTypeDef",
     {
-        "crossAccountRoleArns": Sequence[str],
-        "invokerRoleName": str,
+        "assessmentSchedule": AppAssessmentScheduleTypeType,
+        "complianceStatus": AppComplianceStatusTypeType,
+        "description": str,
+        "lastAppComplianceEvaluationTime": datetime,
+        "lastResiliencyScoreEvaluationTime": datetime,
+        "policyArn": str,
+        "resiliencyScore": float,
+        "status": AppStatusTypeType,
+        "tags": Dict[str, str],
     },
     total=False,
 )
 
-class PermissionModelTypeDef(_RequiredPermissionModelTypeDef, _OptionalPermissionModelTypeDef):
+class AppTypeDef(_RequiredAppTypeDef, _OptionalAppTypeDef):
     pass
 
-_RequiredAppVersionSummaryTypeDef = TypedDict(
-    "_RequiredAppVersionSummaryTypeDef",
+AppVersionSummaryTypeDef = TypedDict(
+    "AppVersionSummaryTypeDef",
     {
         "appVersion": str,
     },
 )
-_OptionalAppVersionSummaryTypeDef = TypedDict(
-    "_OptionalAppVersionSummaryTypeDef",
-    {
-        "creationTime": datetime,
-        "identifier": int,
-        "versionName": str,
-    },
-    total=False,
-)
-
-class AppVersionSummaryTypeDef(
-    _RequiredAppVersionSummaryTypeDef, _OptionalAppVersionSummaryTypeDef
-):
-    pass
-
-BatchUpdateRecommendationStatusFailedEntryTypeDef = TypedDict(
-    "BatchUpdateRecommendationStatusFailedEntryTypeDef",
-    {
-        "entryId": str,
-        "errorMessage": str,
-    },
-)
-
-UpdateRecommendationStatusItemTypeDef = TypedDict(
-    "UpdateRecommendationStatusItemTypeDef",
-    {
-        "resourceId": str,
-        "targetAccountId": str,
-        "targetRegion": str,
-    },
-    total=False,
-)
 
 _RequiredRecommendationDisruptionComplianceTypeDef = TypedDict(
     "_RequiredRecommendationDisruptionComplianceTypeDef",
     {
         "expectedComplianceStatus": ComplianceStatusType,
     },
 )
@@ -430,14 +367,37 @@
 
 class RecommendationDisruptionComplianceTypeDef(
     _RequiredRecommendationDisruptionComplianceTypeDef,
     _OptionalRecommendationDisruptionComplianceTypeDef,
 ):
     pass
 
+_RequiredCreateAppRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateAppRequestRequestTypeDef",
+    {
+        "name": str,
+    },
+)
+_OptionalCreateAppRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateAppRequestRequestTypeDef",
+    {
+        "assessmentSchedule": AppAssessmentScheduleTypeType,
+        "clientToken": str,
+        "description": str,
+        "policyArn": str,
+        "tags": Mapping[str, str],
+    },
+    total=False,
+)
+
+class CreateAppRequestRequestTypeDef(
+    _RequiredCreateAppRequestRequestTypeDef, _OptionalCreateAppRequestRequestTypeDef
+):
+    pass
+
 _RequiredCreateAppVersionAppComponentRequestRequestTypeDef = TypedDict(
     "_RequiredCreateAppVersionAppComponentRequestRequestTypeDef",
     {
         "appArn": str,
         "name": str,
         "type": str,
     },
@@ -714,35 +674,14 @@
 
 class ListAlarmRecommendationsRequestRequestTypeDef(
     _RequiredListAlarmRecommendationsRequestRequestTypeDef,
     _OptionalListAlarmRecommendationsRequestRequestTypeDef,
 ):
     pass
 
-_RequiredListAppAssessmentComplianceDriftsRequestRequestTypeDef = TypedDict(
-    "_RequiredListAppAssessmentComplianceDriftsRequestRequestTypeDef",
-    {
-        "assessmentArn": str,
-    },
-)
-_OptionalListAppAssessmentComplianceDriftsRequestRequestTypeDef = TypedDict(
-    "_OptionalListAppAssessmentComplianceDriftsRequestRequestTypeDef",
-    {
-        "maxResults": int,
-        "nextToken": str,
-    },
-    total=False,
-)
-
-class ListAppAssessmentComplianceDriftsRequestRequestTypeDef(
-    _RequiredListAppAssessmentComplianceDriftsRequestRequestTypeDef,
-    _OptionalListAppAssessmentComplianceDriftsRequestRequestTypeDef,
-):
-    pass
-
 ListAppAssessmentsRequestRequestTypeDef = TypedDict(
     "ListAppAssessmentsRequestRequestTypeDef",
     {
         "appArn": str,
         "assessmentName": str,
         "assessmentStatus": Sequence[AssessmentStatusType],
         "complianceStatus": ComplianceStatusType,
@@ -881,15 +820,34 @@
 
 class ListAppVersionResourcesRequestRequestTypeDef(
     _RequiredListAppVersionResourcesRequestRequestTypeDef,
     _OptionalListAppVersionResourcesRequestRequestTypeDef,
 ):
     pass
 
-TimestampTypeDef = Union[datetime, str]
+_RequiredListAppVersionsRequestRequestTypeDef = TypedDict(
+    "_RequiredListAppVersionsRequestRequestTypeDef",
+    {
+        "appArn": str,
+    },
+)
+_OptionalListAppVersionsRequestRequestTypeDef = TypedDict(
+    "_OptionalListAppVersionsRequestRequestTypeDef",
+    {
+        "maxResults": int,
+        "nextToken": str,
+    },
+    total=False,
+)
+
+class ListAppVersionsRequestRequestTypeDef(
+    _RequiredListAppVersionsRequestRequestTypeDef, _OptionalListAppVersionsRequestRequestTypeDef
+):
+    pass
+
 ListAppsRequestRequestTypeDef = TypedDict(
     "ListAppsRequestRequestTypeDef",
     {
         "appArn": str,
         "maxResults": int,
         "name": str,
         "nextToken": str,
@@ -1030,32 +988,20 @@
 )
 
 class PhysicalResourceIdTypeDef(
     _RequiredPhysicalResourceIdTypeDef, _OptionalPhysicalResourceIdTypeDef
 ):
     pass
 
-_RequiredPublishAppVersionRequestRequestTypeDef = TypedDict(
-    "_RequiredPublishAppVersionRequestRequestTypeDef",
+PublishAppVersionRequestRequestTypeDef = TypedDict(
+    "PublishAppVersionRequestRequestTypeDef",
     {
         "appArn": str,
     },
 )
-_OptionalPublishAppVersionRequestRequestTypeDef = TypedDict(
-    "_OptionalPublishAppVersionRequestRequestTypeDef",
-    {
-        "versionName": str,
-    },
-    total=False,
-)
-
-class PublishAppVersionRequestRequestTypeDef(
-    _RequiredPublishAppVersionRequestRequestTypeDef, _OptionalPublishAppVersionRequestRequestTypeDef
-):
-    pass
 
 PutDraftAppVersionTemplateRequestRequestTypeDef = TypedDict(
     "PutDraftAppVersionTemplateRequestRequestTypeDef",
     {
         "appArn": str,
         "appTemplateBody": str,
     },
@@ -1148,14 +1094,36 @@
     "UntagResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
         "tagKeys": Sequence[str],
     },
 )
 
+_RequiredUpdateAppRequestRequestTypeDef = TypedDict(
+    "_RequiredUpdateAppRequestRequestTypeDef",
+    {
+        "appArn": str,
+    },
+)
+_OptionalUpdateAppRequestRequestTypeDef = TypedDict(
+    "_OptionalUpdateAppRequestRequestTypeDef",
+    {
+        "assessmentSchedule": AppAssessmentScheduleTypeType,
+        "clearResiliencyPolicyArn": bool,
+        "description": str,
+        "policyArn": str,
+    },
+    total=False,
+)
+
+class UpdateAppRequestRequestTypeDef(
+    _RequiredUpdateAppRequestRequestTypeDef, _OptionalUpdateAppRequestRequestTypeDef
+):
+    pass
+
 _RequiredUpdateAppVersionAppComponentRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateAppVersionAppComponentRequestRequestTypeDef",
     {
         "appArn": str,
         "id": str,
     },
 )
@@ -1281,16 +1249,14 @@
 )
 
 PublishAppVersionResponseTypeDef = TypedDict(
     "PublishAppVersionResponseTypeDef",
     {
         "appArn": str,
         "appVersion": str,
-        "identifier": int,
-        "versionName": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 PutDraftAppVersionTemplateResponseTypeDef = TypedDict(
     "PutDraftAppVersionTemplateResponseTypeDef",
     {
@@ -1339,15 +1305,14 @@
         "type": AlarmTypeType,
     },
 )
 _OptionalAlarmRecommendationTypeDef = TypedDict(
     "_OptionalAlarmRecommendationTypeDef",
     {
         "appComponentName": str,
-        "appComponentNames": List[str],
         "description": str,
         "items": List[RecommendationItemTypeDef],
         "prerequisite": str,
     },
     total=False,
 )
 
@@ -1420,47 +1385,28 @@
     "_OptionalAppAssessmentSummaryTypeDef",
     {
         "appArn": str,
         "appVersion": str,
         "assessmentName": str,
         "complianceStatus": ComplianceStatusType,
         "cost": CostTypeDef,
-        "driftStatus": DriftStatusType,
         "endTime": datetime,
         "invoker": AssessmentInvokerType,
         "message": str,
         "resiliencyScore": float,
         "startTime": datetime,
-        "versionName": str,
     },
     total=False,
 )
 
 class AppAssessmentSummaryTypeDef(
     _RequiredAppAssessmentSummaryTypeDef, _OptionalAppAssessmentSummaryTypeDef
 ):
     pass
 
-ComplianceDriftTypeDef = TypedDict(
-    "ComplianceDriftTypeDef",
-    {
-        "actualReferenceId": str,
-        "actualValue": Dict[DisruptionTypeType, DisruptionComplianceTypeDef],
-        "appId": str,
-        "appVersion": str,
-        "diffType": Literal["NotEqual"],
-        "driftType": Literal["ApplicationCompliance"],
-        "entityId": str,
-        "entityType": str,
-        "expectedReferenceId": str,
-        "expectedValue": Dict[DisruptionTypeType, DisruptionComplianceTypeDef],
-    },
-    total=False,
-)
-
 AppComponentComplianceTypeDef = TypedDict(
     "AppComponentComplianceTypeDef",
     {
         "appComponentName": str,
         "compliance": Dict[DisruptionTypeType, DisruptionComplianceTypeDef],
         "cost": CostTypeDef,
         "message": str,
@@ -1570,149 +1516,47 @@
     {
         "appSummaries": List[AppSummaryTypeDef],
         "nextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredAppTypeDef = TypedDict(
-    "_RequiredAppTypeDef",
-    {
-        "appArn": str,
-        "creationTime": datetime,
-        "name": str,
-    },
-)
-_OptionalAppTypeDef = TypedDict(
-    "_OptionalAppTypeDef",
+CreateAppResponseTypeDef = TypedDict(
+    "CreateAppResponseTypeDef",
     {
-        "assessmentSchedule": AppAssessmentScheduleTypeType,
-        "complianceStatus": AppComplianceStatusTypeType,
-        "description": str,
-        "driftStatus": AppDriftStatusTypeType,
-        "eventSubscriptions": List[EventSubscriptionTypeDef],
-        "lastAppComplianceEvaluationTime": datetime,
-        "lastDriftEvaluationTime": datetime,
-        "lastResiliencyScoreEvaluationTime": datetime,
-        "permissionModel": PermissionModelTypeDef,
-        "policyArn": str,
-        "resiliencyScore": float,
-        "status": AppStatusTypeType,
-        "tags": Dict[str, str],
+        "app": AppTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
-class AppTypeDef(_RequiredAppTypeDef, _OptionalAppTypeDef):
-    pass
-
-_RequiredCreateAppRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateAppRequestRequestTypeDef",
-    {
-        "name": str,
-    },
-)
-_OptionalCreateAppRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateAppRequestRequestTypeDef",
+DescribeAppResponseTypeDef = TypedDict(
+    "DescribeAppResponseTypeDef",
     {
-        "assessmentSchedule": AppAssessmentScheduleTypeType,
-        "clientToken": str,
-        "description": str,
-        "eventSubscriptions": Sequence[EventSubscriptionTypeDef],
-        "permissionModel": PermissionModelTypeDef,
-        "policyArn": str,
-        "tags": Mapping[str, str],
+        "app": AppTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
-class CreateAppRequestRequestTypeDef(
-    _RequiredCreateAppRequestRequestTypeDef, _OptionalCreateAppRequestRequestTypeDef
-):
-    pass
-
-_RequiredUpdateAppRequestRequestTypeDef = TypedDict(
-    "_RequiredUpdateAppRequestRequestTypeDef",
-    {
-        "appArn": str,
-    },
-)
-_OptionalUpdateAppRequestRequestTypeDef = TypedDict(
-    "_OptionalUpdateAppRequestRequestTypeDef",
+UpdateAppResponseTypeDef = TypedDict(
+    "UpdateAppResponseTypeDef",
     {
-        "assessmentSchedule": AppAssessmentScheduleTypeType,
-        "clearResiliencyPolicyArn": bool,
-        "description": str,
-        "eventSubscriptions": Sequence[EventSubscriptionTypeDef],
-        "permissionModel": PermissionModelTypeDef,
-        "policyArn": str,
+        "app": AppTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
-class UpdateAppRequestRequestTypeDef(
-    _RequiredUpdateAppRequestRequestTypeDef, _OptionalUpdateAppRequestRequestTypeDef
-):
-    pass
-
 ListAppVersionsResponseTypeDef = TypedDict(
     "ListAppVersionsResponseTypeDef",
     {
         "appVersions": List[AppVersionSummaryTypeDef],
         "nextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredBatchUpdateRecommendationStatusSuccessfulEntryTypeDef = TypedDict(
-    "_RequiredBatchUpdateRecommendationStatusSuccessfulEntryTypeDef",
-    {
-        "entryId": str,
-        "excluded": bool,
-        "item": UpdateRecommendationStatusItemTypeDef,
-        "referenceId": str,
-    },
-)
-_OptionalBatchUpdateRecommendationStatusSuccessfulEntryTypeDef = TypedDict(
-    "_OptionalBatchUpdateRecommendationStatusSuccessfulEntryTypeDef",
-    {
-        "excludeReason": ExcludeRecommendationReasonType,
-    },
-    total=False,
-)
-
-class BatchUpdateRecommendationStatusSuccessfulEntryTypeDef(
-    _RequiredBatchUpdateRecommendationStatusSuccessfulEntryTypeDef,
-    _OptionalBatchUpdateRecommendationStatusSuccessfulEntryTypeDef,
-):
-    pass
-
-_RequiredUpdateRecommendationStatusRequestEntryTypeDef = TypedDict(
-    "_RequiredUpdateRecommendationStatusRequestEntryTypeDef",
-    {
-        "entryId": str,
-        "excluded": bool,
-        "item": UpdateRecommendationStatusItemTypeDef,
-        "referenceId": str,
-    },
-)
-_OptionalUpdateRecommendationStatusRequestEntryTypeDef = TypedDict(
-    "_OptionalUpdateRecommendationStatusRequestEntryTypeDef",
-    {
-        "excludeReason": ExcludeRecommendationReasonType,
-    },
-    total=False,
-)
-
-class UpdateRecommendationStatusRequestEntryTypeDef(
-    _RequiredUpdateRecommendationStatusRequestEntryTypeDef,
-    _OptionalUpdateRecommendationStatusRequestEntryTypeDef,
-):
-    pass
-
 _RequiredConfigRecommendationTypeDef = TypedDict(
     "_RequiredConfigRecommendationTypeDef",
     {
         "name": str,
         "optimizationType": ConfigRecommendationOptimizationTypeType,
         "referenceId": str,
     },
@@ -1941,36 +1785,14 @@
         "sourceArns": List[str],
         "status": ResourceImportStatusTypeType,
         "terraformSources": List[TerraformSourceTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredListAppVersionsRequestRequestTypeDef = TypedDict(
-    "_RequiredListAppVersionsRequestRequestTypeDef",
-    {
-        "appArn": str,
-    },
-)
-_OptionalListAppVersionsRequestRequestTypeDef = TypedDict(
-    "_OptionalListAppVersionsRequestRequestTypeDef",
-    {
-        "endTime": TimestampTypeDef,
-        "maxResults": int,
-        "nextToken": str,
-        "startTime": TimestampTypeDef,
-    },
-    total=False,
-)
-
-class ListAppVersionsRequestRequestTypeDef(
-    _RequiredListAppVersionsRequestRequestTypeDef, _OptionalListAppVersionsRequestRequestTypeDef
-):
-    pass
-
 _RequiredPhysicalResourceTypeDef = TypedDict(
     "_RequiredPhysicalResourceTypeDef",
     {
         "logicalResourceId": LogicalResourceIdTypeDef,
         "physicalResourceId": PhysicalResourceIdTypeDef,
         "resourceType": str,
     },
@@ -2107,23 +1929,14 @@
     {
         "assessmentSummaries": List[AppAssessmentSummaryTypeDef],
         "nextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-ListAppAssessmentComplianceDriftsResponseTypeDef = TypedDict(
-    "ListAppAssessmentComplianceDriftsResponseTypeDef",
-    {
-        "complianceDrifts": List[ComplianceDriftTypeDef],
-        "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 ListAppComponentCompliancesResponseTypeDef = TypedDict(
     "ListAppComponentCompliancesResponseTypeDef",
     {
         "componentCompliances": List[AppComponentComplianceTypeDef],
         "nextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -2143,56 +1956,14 @@
     {
         "appInputSources": List[AppInputSourceTypeDef],
         "nextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-CreateAppResponseTypeDef = TypedDict(
-    "CreateAppResponseTypeDef",
-    {
-        "app": AppTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DescribeAppResponseTypeDef = TypedDict(
-    "DescribeAppResponseTypeDef",
-    {
-        "app": AppTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-UpdateAppResponseTypeDef = TypedDict(
-    "UpdateAppResponseTypeDef",
-    {
-        "app": AppTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-BatchUpdateRecommendationStatusResponseTypeDef = TypedDict(
-    "BatchUpdateRecommendationStatusResponseTypeDef",
-    {
-        "appArn": str,
-        "failedEntries": List[BatchUpdateRecommendationStatusFailedEntryTypeDef],
-        "successfulEntries": List[BatchUpdateRecommendationStatusSuccessfulEntryTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-BatchUpdateRecommendationStatusRequestRequestTypeDef = TypedDict(
-    "BatchUpdateRecommendationStatusRequestRequestTypeDef",
-    {
-        "appArn": str,
-        "requestEntries": Sequence[UpdateRecommendationStatusRequestEntryTypeDef],
-    },
-)
-
 ComponentRecommendationTypeDef = TypedDict(
     "ComponentRecommendationTypeDef",
     {
         "appComponentName": str,
         "configRecommendations": List[ConfigRecommendationTypeDef],
         "recommendationStatus": RecommendationComplianceStatusType,
     },
@@ -2357,23 +2128,21 @@
     {
         "appArn": str,
         "appVersion": str,
         "assessmentName": str,
         "compliance": Dict[DisruptionTypeType, DisruptionComplianceTypeDef],
         "complianceStatus": ComplianceStatusType,
         "cost": CostTypeDef,
-        "driftStatus": DriftStatusType,
         "endTime": datetime,
         "message": str,
         "policy": ResiliencyPolicyTypeDef,
         "resiliencyScore": ResiliencyScoreTypeDef,
         "resourceErrorsDetails": ResourceErrorsDetailsTypeDef,
         "startTime": datetime,
         "tags": Dict[str, str],
-        "versionName": str,
     },
     total=False,
 )
 
 class AppAssessmentTypeDef(_RequiredAppAssessmentTypeDef, _OptionalAppAssessmentTypeDef):
     pass
```

### Comparing `types-aiobotocore-resiliencehub-2.5.2.post2/types_aiobotocore_resiliencehub.egg-info/PKG-INFO` & `types-aiobotocore-resiliencehub-2.5.4/types_aiobotocore_resiliencehub.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-resiliencehub
-Version: 2.5.2.post2
-Summary: Type annotations for aiobotocore.ResilienceHub 2.5.2 service generated with mypy-boto3-builder 7.17.2
+Version: 2.5.4
+Summary: Type annotations for aiobotocore.ResilienceHub 2.5.4 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_resiliencehub/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-resiliencehub.svg?color=blue)](https://pypi.org/project/types-aiobotocore-resiliencehub)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_resiliencehub/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-resiliencehub)](https://pepy.tech/project/types-aiobotocore-resiliencehub)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.ResilienceHub 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resiliencehub.html#ResilienceHub)
+[aiobotocore.ResilienceHub 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resiliencehub.html#ResilienceHub)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-resiliencehub-2.5.2.post2/types_aiobotocore_resiliencehub.egg-info/SOURCES.txt` & `types-aiobotocore-resiliencehub-2.5.4/types_aiobotocore_resiliencehub.egg-info/SOURCES.txt`

 * *Files identical despite different names*


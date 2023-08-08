# Comparing `tmp/types-aiobotocore-application-insights-2.5.2.post3.tar.gz` & `tmp/types-aiobotocore-application-insights-2.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-application-insights-2.5.2.post3.tar", last modified: Fri Aug  4 12:37:16 2023, max compression
+gzip compressed data, was "types-aiobotocore-application-insights-2.5.4.tar", last modified: Tue Aug  8 01:23:18 2023, max compression
```

## Comparing `types-aiobotocore-application-insights-2.5.2.post3.tar` & `types-aiobotocore-application-insights-2.5.4.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:37:16.347167 types-aiobotocore-application-insights-2.5.2.post3/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-04 12:18:24.000000 types-aiobotocore-application-insights-2.5.2.post3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    12894 2023-08-04 12:37:16.347167 types-aiobotocore-application-insights-2.5.2.post3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    11325 2023-08-04 12:18:24.000000 types-aiobotocore-application-insights-2.5.2.post3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-04 12:37:16.347167 types-aiobotocore-application-insights-2.5.2.post3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2154 2023-08-04 12:18:24.000000 types-aiobotocore-application-insights-2.5.2.post3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:37:16.339167 types-aiobotocore-application-insights-2.5.2.post3/types_aiobotocore_application_insights/
--rw-r--r--   0 runner    (1001) docker     (123)      541 2023-08-04 12:18:24.000000 types-aiobotocore-application-insights-2.5.2.post3/types_aiobotocore_application_insights/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      540 2023-08-04 12:18:24.000000 types-aiobotocore-application-insights-2.5.2.post3/types_aiobotocore_application_insights/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      993 2023-08-04 12:18:24.000000 types-aiobotocore-application-insights-2.5.2.post3/types_aiobotocore_application_insights/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    22655 2023-08-04 12:18:24.000000 types-aiobotocore-application-insights-2.5.2.post3/types_aiobotocore_application_insights/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    22619 2023-08-04 12:18:24.000000 types-aiobotocore-application-insights-2.5.2.post3/types_aiobotocore_application_insights/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9532 2023-08-04 12:18:24.000000 types-aiobotocore-application-insights-2.5.2.post3/types_aiobotocore_application_insights/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     9530 2023-08-04 12:18:24.000000 types-aiobotocore-application-insights-2.5.2.post3/types_aiobotocore_application_insights/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 12:18:24.000000 types-aiobotocore-application-insights-2.5.2.post3/types_aiobotocore_application_insights/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    19824 2023-08-04 12:18:25.000000 types-aiobotocore-application-insights-2.5.2.post3/types_aiobotocore_application_insights/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    19809 2023-08-04 12:18:25.000000 types-aiobotocore-application-insights-2.5.2.post3/types_aiobotocore_application_insights/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-04 12:18:24.000000 types-aiobotocore-application-insights-2.5.2.post3/types_aiobotocore_application_insights/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:37:16.347167 types-aiobotocore-application-insights-2.5.2.post3/types_aiobotocore_application_insights.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    12894 2023-08-04 12:37:16.000000 types-aiobotocore-application-insights-2.5.2.post3/types_aiobotocore_application_insights.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      955 2023-08-04 12:37:16.000000 types-aiobotocore-application-insights-2.5.2.post3/types_aiobotocore_application_insights.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 12:37:16.000000 types-aiobotocore-application-insights-2.5.2.post3/types_aiobotocore_application_insights.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 12:37:16.000000 types-aiobotocore-application-insights-2.5.2.post3/types_aiobotocore_application_insights.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-04 12:37:16.000000 types-aiobotocore-application-insights-2.5.2.post3/types_aiobotocore_application_insights.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-08-04 12:37:16.000000 types-aiobotocore-application-insights-2.5.2.post3/types_aiobotocore_application_insights.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:23:18.306502 types-aiobotocore-application-insights-2.5.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-08 01:06:12.000000 types-aiobotocore-application-insights-2.5.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    12890 2023-08-08 01:23:18.306502 types-aiobotocore-application-insights-2.5.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    11327 2023-08-08 01:06:12.000000 types-aiobotocore-application-insights-2.5.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-08 01:23:18.306502 types-aiobotocore-application-insights-2.5.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2148 2023-08-08 01:06:12.000000 types-aiobotocore-application-insights-2.5.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:23:18.306502 types-aiobotocore-application-insights-2.5.4/types_aiobotocore_application_insights/
+-rw-r--r--   0 runner    (1001) docker     (123)      541 2023-08-08 01:06:12.000000 types-aiobotocore-application-insights-2.5.4/types_aiobotocore_application_insights/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      540 2023-08-08 01:06:12.000000 types-aiobotocore-application-insights-2.5.4/types_aiobotocore_application_insights/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      981 2023-08-08 01:06:12.000000 types-aiobotocore-application-insights-2.5.4/types_aiobotocore_application_insights/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27125 2023-08-08 01:06:12.000000 types-aiobotocore-application-insights-2.5.4/types_aiobotocore_application_insights/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27083 2023-08-08 01:06:12.000000 types-aiobotocore-application-insights-2.5.4/types_aiobotocore_application_insights/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    10148 2023-08-08 01:06:12.000000 types-aiobotocore-application-insights-2.5.4/types_aiobotocore_application_insights/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10146 2023-08-08 01:06:12.000000 types-aiobotocore-application-insights-2.5.4/types_aiobotocore_application_insights/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 01:06:12.000000 types-aiobotocore-application-insights-2.5.4/types_aiobotocore_application_insights/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    28040 2023-08-08 01:06:13.000000 types-aiobotocore-application-insights-2.5.4/types_aiobotocore_application_insights/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28001 2023-08-08 01:06:12.000000 types-aiobotocore-application-insights-2.5.4/types_aiobotocore_application_insights/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-08-08 01:06:12.000000 types-aiobotocore-application-insights-2.5.4/types_aiobotocore_application_insights/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:23:18.306502 types-aiobotocore-application-insights-2.5.4/types_aiobotocore_application_insights.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    12890 2023-08-08 01:23:18.000000 types-aiobotocore-application-insights-2.5.4/types_aiobotocore_application_insights.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      955 2023-08-08 01:23:18.000000 types-aiobotocore-application-insights-2.5.4/types_aiobotocore_application_insights.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 01:23:18.000000 types-aiobotocore-application-insights-2.5.4/types_aiobotocore_application_insights.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 01:23:18.000000 types-aiobotocore-application-insights-2.5.4/types_aiobotocore_application_insights.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-08 01:23:18.000000 types-aiobotocore-application-insights-2.5.4/types_aiobotocore_application_insights.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-08-08 01:23:18.000000 types-aiobotocore-application-insights-2.5.4/types_aiobotocore_application_insights.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-application-insights-2.5.2.post3/LICENSE` & `types-aiobotocore-application-insights-2.5.4/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-application-insights-2.5.2.post3/PKG-INFO` & `types-aiobotocore-application-insights-2.5.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-application-insights
-Version: 2.5.2.post3
-Summary: Type annotations for aiobotocore.ApplicationInsights 2.5.2 service generated with mypy-boto3-builder 7.17.2
+Version: 2.5.4
+Summary: Type annotations for aiobotocore.ApplicationInsights 2.5.4 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_application_insights/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-application-insights.svg?color=blue)](https://pypi.org/project/types-aiobotocore-application-insights)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_application_insights/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-application-insights)](https://pepy.tech/project/types-aiobotocore-application-insights)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.ApplicationInsights 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/application-insights.html#ApplicationInsights)
+[aiobotocore.ApplicationInsights 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/application-insights.html#ApplicationInsights)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
@@ -289,18 +289,18 @@
 and shapes assembled to typed dictionaries and unions for additional type
 checking.
 
 Full list of `ApplicationInsights` TypeDefs can be found in
 [docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_application_insights/type_defs/).
 
 ```python
-from types_aiobotocore_application_insights.type_defs import ApplicationComponentTypeDef
+from types_aiobotocore_application_insights.type_defs import WorkloadConfigurationTypeDef
 
 
-def get_value() -> ApplicationComponentTypeDef:
+def get_value() -> WorkloadConfigurationTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-application-insights-2.5.2.post3/README.md` & `types-aiobotocore-application-insights-2.5.4/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-application-insights.svg?color=blue)](https://pypi.org/project/types-aiobotocore-application-insights)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_application_insights/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-application-insights)](https://pepy.tech/project/types-aiobotocore-application-insights)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.ApplicationInsights 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/application-insights.html#ApplicationInsights)
+[aiobotocore.ApplicationInsights 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/application-insights.html#ApplicationInsights)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
@@ -257,18 +257,18 @@
 and shapes assembled to typed dictionaries and unions for additional type
 checking.
 
 Full list of `ApplicationInsights` TypeDefs can be found in
 [docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_application_insights/type_defs/).
 
 ```python
-from types_aiobotocore_application_insights.type_defs import ApplicationComponentTypeDef
+from types_aiobotocore_application_insights.type_defs import WorkloadConfigurationTypeDef
 
 
-def get_value() -> ApplicationComponentTypeDef:
+def get_value() -> WorkloadConfigurationTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-application-insights-2.5.2.post3/setup.py` & `types-aiobotocore-application-insights-2.5.4/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-application-insights",
-    version="2.5.2.post3",
+    version="2.5.4",
     packages=["types_aiobotocore_application_insights"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.ApplicationInsights 2.5.2 service generated with"
+        "Type annotations for aiobotocore.ApplicationInsights 2.5.4 service generated with"
         " mypy-boto3-builder 7.17.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
```

### Comparing `types-aiobotocore-application-insights-2.5.2.post3/types_aiobotocore_application_insights/__init__.py` & `types-aiobotocore-application-insights-2.5.4/types_aiobotocore_application_insights/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-application-insights-2.5.2.post3/types_aiobotocore_application_insights/__init__.pyi` & `types-aiobotocore-application-insights-2.5.4/types_aiobotocore_application_insights/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-application-insights-2.5.2.post3/types_aiobotocore_application_insights/__main__.py` & `types-aiobotocore-application-insights-2.5.4/types_aiobotocore_application_insights/__main__.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.ApplicationInsights 2.5.2\nVersion:        "
-        " 2.5.2.post3\nBuilder version: 7.17.2\nDocs:           "
+        "Type annotations for aiobotocore.ApplicationInsights 2.5.4\nVersion:        "
+        " 2.5.4\nBuilder version: 7.17.2\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_application_insights//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/application-insights.html#ApplicationInsights\nOther"
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

### Comparing `types-aiobotocore-application-insights-2.5.2.post3/types_aiobotocore_application_insights/client.py` & `types-aiobotocore-application-insights-2.5.4/types_aiobotocore_application_insights/client.py`

 * *Files 9% similar despite different names*

```diff
@@ -16,37 +16,42 @@
 """
 import sys
 from typing import Any, Dict, Mapping, Sequence, Type
 
 from aiobotocore.client import AioBaseClient
 from botocore.client import ClientMeta
 
-from .literals import ConfigurationEventStatusType, TierType
+from .literals import ConfigurationEventStatusType, RecommendationTypeType, TierType, VisibilityType
 from .type_defs import (
+    AddWorkloadResponseTypeDef,
     CreateApplicationResponseTypeDef,
     CreateLogPatternResponseTypeDef,
     DescribeApplicationResponseTypeDef,
     DescribeComponentConfigurationRecommendationResponseTypeDef,
     DescribeComponentConfigurationResponseTypeDef,
     DescribeComponentResponseTypeDef,
     DescribeLogPatternResponseTypeDef,
     DescribeObservationResponseTypeDef,
     DescribeProblemObservationsResponseTypeDef,
     DescribeProblemResponseTypeDef,
+    DescribeWorkloadResponseTypeDef,
     ListApplicationsResponseTypeDef,
     ListComponentsResponseTypeDef,
     ListConfigurationHistoryResponseTypeDef,
     ListLogPatternSetsResponseTypeDef,
     ListLogPatternsResponseTypeDef,
     ListProblemsResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
+    ListWorkloadsResponseTypeDef,
     TagTypeDef,
     TimestampTypeDef,
     UpdateApplicationResponseTypeDef,
     UpdateLogPatternResponseTypeDef,
+    UpdateWorkloadResponseTypeDef,
+    WorkloadConfigurationTypeDef,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
@@ -87,14 +92,28 @@
         """
         ApplicationInsightsClient exceptions.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/application-insights.html#ApplicationInsights.Client.exceptions)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_application_insights/client/#exceptions)
         """
 
+    async def add_workload(
+        self,
+        *,
+        ResourceGroupName: str,
+        ComponentName: str,
+        WorkloadConfiguration: WorkloadConfigurationTypeDef
+    ) -> AddWorkloadResponseTypeDef:
+        """
+        Adds a workload to a component.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/application-insights.html#ApplicationInsights.Client.add_workload)
+        [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_application_insights/client/#add_workload)
+        """
+
     def can_paginate(self, operation_name: str) -> bool:
         """
         Check if an operation can be paginated.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/application-insights.html#ApplicationInsights.Client.can_paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_application_insights/client/#can_paginate)
         """
@@ -177,92 +196,109 @@
         Removes the specified log pattern from a `LogPatternSet`.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/application-insights.html#ApplicationInsights.Client.delete_log_pattern)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_application_insights/client/#delete_log_pattern)
         """
 
     async def describe_application(
-        self, *, ResourceGroupName: str
+        self, *, ResourceGroupName: str, AccountId: str = ...
     ) -> DescribeApplicationResponseTypeDef:
         """
         Describes the application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/application-insights.html#ApplicationInsights.Client.describe_application)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_application_insights/client/#describe_application)
         """
 
     async def describe_component(
-        self, *, ResourceGroupName: str, ComponentName: str
+        self, *, ResourceGroupName: str, ComponentName: str, AccountId: str = ...
     ) -> DescribeComponentResponseTypeDef:
         """
         Describes a component and lists the resources that are grouped together in a
         component.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/application-insights.html#ApplicationInsights.Client.describe_component)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_application_insights/client/#describe_component)
         """
 
     async def describe_component_configuration(
-        self, *, ResourceGroupName: str, ComponentName: str
+        self, *, ResourceGroupName: str, ComponentName: str, AccountId: str = ...
     ) -> DescribeComponentConfigurationResponseTypeDef:
         """
         Describes the monitoring configuration of the component.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/application-insights.html#ApplicationInsights.Client.describe_component_configuration)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_application_insights/client/#describe_component_configuration)
         """
 
     async def describe_component_configuration_recommendation(
-        self, *, ResourceGroupName: str, ComponentName: str, Tier: TierType
+        self,
+        *,
+        ResourceGroupName: str,
+        ComponentName: str,
+        Tier: TierType,
+        RecommendationType: RecommendationTypeType = ...
     ) -> DescribeComponentConfigurationRecommendationResponseTypeDef:
         """
         Describes the recommended monitoring configuration of the component.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/application-insights.html#ApplicationInsights.Client.describe_component_configuration_recommendation)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_application_insights/client/#describe_component_configuration_recommendation)
         """
 
     async def describe_log_pattern(
-        self, *, ResourceGroupName: str, PatternSetName: str, PatternName: str
+        self, *, ResourceGroupName: str, PatternSetName: str, PatternName: str, AccountId: str = ...
     ) -> DescribeLogPatternResponseTypeDef:
         """
         Describe a specific log pattern from a `LogPatternSet`.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/application-insights.html#ApplicationInsights.Client.describe_log_pattern)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_application_insights/client/#describe_log_pattern)
         """
 
     async def describe_observation(
-        self, *, ObservationId: str
+        self, *, ObservationId: str, AccountId: str = ...
     ) -> DescribeObservationResponseTypeDef:
         """
         Describes an anomaly or error with the application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/application-insights.html#ApplicationInsights.Client.describe_observation)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_application_insights/client/#describe_observation)
         """
 
-    async def describe_problem(self, *, ProblemId: str) -> DescribeProblemResponseTypeDef:
+    async def describe_problem(
+        self, *, ProblemId: str, AccountId: str = ...
+    ) -> DescribeProblemResponseTypeDef:
         """
         Describes an application problem.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/application-insights.html#ApplicationInsights.Client.describe_problem)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_application_insights/client/#describe_problem)
         """
 
     async def describe_problem_observations(
-        self, *, ProblemId: str
+        self, *, ProblemId: str, AccountId: str = ...
     ) -> DescribeProblemObservationsResponseTypeDef:
         """
         Describes the anomalies or errors associated with the problem.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/application-insights.html#ApplicationInsights.Client.describe_problem_observations)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_application_insights/client/#describe_problem_observations)
         """
 
+    async def describe_workload(
+        self, *, ResourceGroupName: str, ComponentName: str, WorkloadId: str, AccountId: str = ...
+    ) -> DescribeWorkloadResponseTypeDef:
+        """
+        Describes a workload and its configuration.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/application-insights.html#ApplicationInsights.Client.describe_workload)
+        [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_application_insights/client/#describe_workload)
+        """
+
     async def generate_presigned_url(
         self,
         ClientMethod: str,
         Params: Mapping[str, Any] = ...,
         ExpiresIn: int = 3600,
         HttpMethod: str = ...,
     ) -> str:
@@ -270,25 +306,30 @@
         Generate a presigned url given a client, its method, and arguments.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/application-insights.html#ApplicationInsights.Client.generate_presigned_url)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_application_insights/client/#generate_presigned_url)
         """
 
     async def list_applications(
-        self, *, MaxResults: int = ..., NextToken: str = ...
+        self, *, MaxResults: int = ..., NextToken: str = ..., AccountId: str = ...
     ) -> ListApplicationsResponseTypeDef:
         """
         Lists the IDs of the applications that you are monitoring.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/application-insights.html#ApplicationInsights.Client.list_applications)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_application_insights/client/#list_applications)
         """
 
     async def list_components(
-        self, *, ResourceGroupName: str, MaxResults: int = ..., NextToken: str = ...
+        self,
+        *,
+        ResourceGroupName: str,
+        MaxResults: int = ...,
+        NextToken: str = ...,
+        AccountId: str = ...
     ) -> ListComponentsResponseTypeDef:
         """
         Lists the auto-grouped, standalone, and custom components of the application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/application-insights.html#ApplicationInsights.Client.list_components)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_application_insights/client/#list_components)
         """
@@ -297,58 +338,67 @@
         self,
         *,
         ResourceGroupName: str = ...,
         StartTime: TimestampTypeDef = ...,
         EndTime: TimestampTypeDef = ...,
         EventStatus: ConfigurationEventStatusType = ...,
         MaxResults: int = ...,
-        NextToken: str = ...
+        NextToken: str = ...,
+        AccountId: str = ...
     ) -> ListConfigurationHistoryResponseTypeDef:
         """
         Lists the INFO, WARN, and ERROR events for periodic configuration updates
         performed by Application Insights.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/application-insights.html#ApplicationInsights.Client.list_configuration_history)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_application_insights/client/#list_configuration_history)
         """
 
     async def list_log_pattern_sets(
-        self, *, ResourceGroupName: str, MaxResults: int = ..., NextToken: str = ...
+        self,
+        *,
+        ResourceGroupName: str,
+        MaxResults: int = ...,
+        NextToken: str = ...,
+        AccountId: str = ...
     ) -> ListLogPatternSetsResponseTypeDef:
         """
         Lists the log pattern sets in the specific application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/application-insights.html#ApplicationInsights.Client.list_log_pattern_sets)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_application_insights/client/#list_log_pattern_sets)
         """
 
     async def list_log_patterns(
         self,
         *,
         ResourceGroupName: str,
         PatternSetName: str = ...,
         MaxResults: int = ...,
-        NextToken: str = ...
+        NextToken: str = ...,
+        AccountId: str = ...
     ) -> ListLogPatternsResponseTypeDef:
         """
         Lists the log patterns in the specific log `LogPatternSet`.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/application-insights.html#ApplicationInsights.Client.list_log_patterns)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_application_insights/client/#list_log_patterns)
         """
 
     async def list_problems(
         self,
         *,
+        AccountId: str = ...,
         ResourceGroupName: str = ...,
         StartTime: TimestampTypeDef = ...,
         EndTime: TimestampTypeDef = ...,
         MaxResults: int = ...,
         NextToken: str = ...,
-        ComponentName: str = ...
+        ComponentName: str = ...,
+        Visibility: VisibilityType = ...
     ) -> ListProblemsResponseTypeDef:
         """
         Lists the problems with your application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/application-insights.html#ApplicationInsights.Client.list_problems)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_application_insights/client/#list_problems)
         """
@@ -360,14 +410,40 @@
         Retrieve a list of the tags (keys and values) that are associated with a
         specified application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/application-insights.html#ApplicationInsights.Client.list_tags_for_resource)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_application_insights/client/#list_tags_for_resource)
         """
 
+    async def list_workloads(
+        self,
+        *,
+        ResourceGroupName: str,
+        ComponentName: str,
+        MaxResults: int = ...,
+        NextToken: str = ...,
+        AccountId: str = ...
+    ) -> ListWorkloadsResponseTypeDef:
+        """
+        Lists the workloads that are configured on a given component.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/application-insights.html#ApplicationInsights.Client.list_workloads)
+        [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_application_insights/client/#list_workloads)
+        """
+
+    async def remove_workload(
+        self, *, ResourceGroupName: str, ComponentName: str, WorkloadId: str
+    ) -> Dict[str, Any]:
+        """
+        Remove workload from a component.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/application-insights.html#ApplicationInsights.Client.remove_workload)
+        [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_application_insights/client/#remove_workload)
+        """
+
     async def tag_resource(self, *, ResourceARN: str, Tags: Sequence[TagTypeDef]) -> Dict[str, Any]:
         """
         Add one or more tags (keys and values) to a specified application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/application-insights.html#ApplicationInsights.Client.tag_resource)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_application_insights/client/#tag_resource)
         """
@@ -442,14 +518,43 @@
         """
         Adds a log pattern to a `LogPatternSet`.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/application-insights.html#ApplicationInsights.Client.update_log_pattern)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_application_insights/client/#update_log_pattern)
         """
 
+    async def update_problem(
+        self,
+        *,
+        ProblemId: str,
+        UpdateStatus: Literal["RESOLVED"] = ...,
+        Visibility: VisibilityType = ...
+    ) -> Dict[str, Any]:
+        """
+        Updates the visibility of the problem or specifies the problem as `RESOLVED`.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/application-insights.html#ApplicationInsights.Client.update_problem)
+        [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_application_insights/client/#update_problem)
+        """
+
+    async def update_workload(
+        self,
+        *,
+        ResourceGroupName: str,
+        ComponentName: str,
+        WorkloadConfiguration: WorkloadConfigurationTypeDef,
+        WorkloadId: str = ...
+    ) -> UpdateWorkloadResponseTypeDef:
+        """
+        Adds a workload to a component.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/application-insights.html#ApplicationInsights.Client.update_workload)
+        [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_application_insights/client/#update_workload)
+        """
+
     async def __aenter__(self) -> "ApplicationInsightsClient":
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/application-insights.html#ApplicationInsights.Client)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_application_insights/client/)
         """
 
     async def __aexit__(self, exc_type: Any, exc_val: Any, exc_tb: Any) -> Any:
```

### Comparing `types-aiobotocore-application-insights-2.5.2.post3/types_aiobotocore_application_insights/client.pyi` & `types-aiobotocore-application-insights-2.5.4/types_aiobotocore_application_insights/client.pyi`

 * *Files 12% similar despite different names*

```diff
@@ -16,37 +16,42 @@
 """
 import sys
 from typing import Any, Dict, Mapping, Sequence, Type
 
 from aiobotocore.client import AioBaseClient
 from botocore.client import ClientMeta
 
-from .literals import ConfigurationEventStatusType, TierType
+from .literals import ConfigurationEventStatusType, RecommendationTypeType, TierType, VisibilityType
 from .type_defs import (
+    AddWorkloadResponseTypeDef,
     CreateApplicationResponseTypeDef,
     CreateLogPatternResponseTypeDef,
     DescribeApplicationResponseTypeDef,
     DescribeComponentConfigurationRecommendationResponseTypeDef,
     DescribeComponentConfigurationResponseTypeDef,
     DescribeComponentResponseTypeDef,
     DescribeLogPatternResponseTypeDef,
     DescribeObservationResponseTypeDef,
     DescribeProblemObservationsResponseTypeDef,
     DescribeProblemResponseTypeDef,
+    DescribeWorkloadResponseTypeDef,
     ListApplicationsResponseTypeDef,
     ListComponentsResponseTypeDef,
     ListConfigurationHistoryResponseTypeDef,
     ListLogPatternSetsResponseTypeDef,
     ListLogPatternsResponseTypeDef,
     ListProblemsResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
+    ListWorkloadsResponseTypeDef,
     TagTypeDef,
     TimestampTypeDef,
     UpdateApplicationResponseTypeDef,
     UpdateLogPatternResponseTypeDef,
+    UpdateWorkloadResponseTypeDef,
+    WorkloadConfigurationTypeDef,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
@@ -82,14 +87,27 @@
     def exceptions(self) -> Exceptions:
         """
         ApplicationInsightsClient exceptions.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/application-insights.html#ApplicationInsights.Client.exceptions)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_application_insights/client/#exceptions)
         """
+    async def add_workload(
+        self,
+        *,
+        ResourceGroupName: str,
+        ComponentName: str,
+        WorkloadConfiguration: WorkloadConfigurationTypeDef
+    ) -> AddWorkloadResponseTypeDef:
+        """
+        Adds a workload to a component.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/application-insights.html#ApplicationInsights.Client.add_workload)
+        [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_application_insights/client/#add_workload)
+        """
     def can_paginate(self, operation_name: str) -> bool:
         """
         Check if an operation can be paginated.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/application-insights.html#ApplicationInsights.Client.can_paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_application_insights/client/#can_paginate)
         """
@@ -164,108 +182,129 @@
         """
         Removes the specified log pattern from a `LogPatternSet`.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/application-insights.html#ApplicationInsights.Client.delete_log_pattern)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_application_insights/client/#delete_log_pattern)
         """
     async def describe_application(
-        self, *, ResourceGroupName: str
+        self, *, ResourceGroupName: str, AccountId: str = ...
     ) -> DescribeApplicationResponseTypeDef:
         """
         Describes the application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/application-insights.html#ApplicationInsights.Client.describe_application)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_application_insights/client/#describe_application)
         """
     async def describe_component(
-        self, *, ResourceGroupName: str, ComponentName: str
+        self, *, ResourceGroupName: str, ComponentName: str, AccountId: str = ...
     ) -> DescribeComponentResponseTypeDef:
         """
         Describes a component and lists the resources that are grouped together in a
         component.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/application-insights.html#ApplicationInsights.Client.describe_component)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_application_insights/client/#describe_component)
         """
     async def describe_component_configuration(
-        self, *, ResourceGroupName: str, ComponentName: str
+        self, *, ResourceGroupName: str, ComponentName: str, AccountId: str = ...
     ) -> DescribeComponentConfigurationResponseTypeDef:
         """
         Describes the monitoring configuration of the component.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/application-insights.html#ApplicationInsights.Client.describe_component_configuration)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_application_insights/client/#describe_component_configuration)
         """
     async def describe_component_configuration_recommendation(
-        self, *, ResourceGroupName: str, ComponentName: str, Tier: TierType
+        self,
+        *,
+        ResourceGroupName: str,
+        ComponentName: str,
+        Tier: TierType,
+        RecommendationType: RecommendationTypeType = ...
     ) -> DescribeComponentConfigurationRecommendationResponseTypeDef:
         """
         Describes the recommended monitoring configuration of the component.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/application-insights.html#ApplicationInsights.Client.describe_component_configuration_recommendation)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_application_insights/client/#describe_component_configuration_recommendation)
         """
     async def describe_log_pattern(
-        self, *, ResourceGroupName: str, PatternSetName: str, PatternName: str
+        self, *, ResourceGroupName: str, PatternSetName: str, PatternName: str, AccountId: str = ...
     ) -> DescribeLogPatternResponseTypeDef:
         """
         Describe a specific log pattern from a `LogPatternSet`.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/application-insights.html#ApplicationInsights.Client.describe_log_pattern)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_application_insights/client/#describe_log_pattern)
         """
     async def describe_observation(
-        self, *, ObservationId: str
+        self, *, ObservationId: str, AccountId: str = ...
     ) -> DescribeObservationResponseTypeDef:
         """
         Describes an anomaly or error with the application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/application-insights.html#ApplicationInsights.Client.describe_observation)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_application_insights/client/#describe_observation)
         """
-    async def describe_problem(self, *, ProblemId: str) -> DescribeProblemResponseTypeDef:
+    async def describe_problem(
+        self, *, ProblemId: str, AccountId: str = ...
+    ) -> DescribeProblemResponseTypeDef:
         """
         Describes an application problem.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/application-insights.html#ApplicationInsights.Client.describe_problem)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_application_insights/client/#describe_problem)
         """
     async def describe_problem_observations(
-        self, *, ProblemId: str
+        self, *, ProblemId: str, AccountId: str = ...
     ) -> DescribeProblemObservationsResponseTypeDef:
         """
         Describes the anomalies or errors associated with the problem.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/application-insights.html#ApplicationInsights.Client.describe_problem_observations)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_application_insights/client/#describe_problem_observations)
         """
+    async def describe_workload(
+        self, *, ResourceGroupName: str, ComponentName: str, WorkloadId: str, AccountId: str = ...
+    ) -> DescribeWorkloadResponseTypeDef:
+        """
+        Describes a workload and its configuration.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/application-insights.html#ApplicationInsights.Client.describe_workload)
+        [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_application_insights/client/#describe_workload)
+        """
     async def generate_presigned_url(
         self,
         ClientMethod: str,
         Params: Mapping[str, Any] = ...,
         ExpiresIn: int = 3600,
         HttpMethod: str = ...,
     ) -> str:
         """
         Generate a presigned url given a client, its method, and arguments.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/application-insights.html#ApplicationInsights.Client.generate_presigned_url)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_application_insights/client/#generate_presigned_url)
         """
     async def list_applications(
-        self, *, MaxResults: int = ..., NextToken: str = ...
+        self, *, MaxResults: int = ..., NextToken: str = ..., AccountId: str = ...
     ) -> ListApplicationsResponseTypeDef:
         """
         Lists the IDs of the applications that you are monitoring.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/application-insights.html#ApplicationInsights.Client.list_applications)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_application_insights/client/#list_applications)
         """
     async def list_components(
-        self, *, ResourceGroupName: str, MaxResults: int = ..., NextToken: str = ...
+        self,
+        *,
+        ResourceGroupName: str,
+        MaxResults: int = ...,
+        NextToken: str = ...,
+        AccountId: str = ...
     ) -> ListComponentsResponseTypeDef:
         """
         Lists the auto-grouped, standalone, and custom components of the application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/application-insights.html#ApplicationInsights.Client.list_components)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_application_insights/client/#list_components)
         """
@@ -273,55 +312,64 @@
         self,
         *,
         ResourceGroupName: str = ...,
         StartTime: TimestampTypeDef = ...,
         EndTime: TimestampTypeDef = ...,
         EventStatus: ConfigurationEventStatusType = ...,
         MaxResults: int = ...,
-        NextToken: str = ...
+        NextToken: str = ...,
+        AccountId: str = ...
     ) -> ListConfigurationHistoryResponseTypeDef:
         """
         Lists the INFO, WARN, and ERROR events for periodic configuration updates
         performed by Application Insights.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/application-insights.html#ApplicationInsights.Client.list_configuration_history)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_application_insights/client/#list_configuration_history)
         """
     async def list_log_pattern_sets(
-        self, *, ResourceGroupName: str, MaxResults: int = ..., NextToken: str = ...
+        self,
+        *,
+        ResourceGroupName: str,
+        MaxResults: int = ...,
+        NextToken: str = ...,
+        AccountId: str = ...
     ) -> ListLogPatternSetsResponseTypeDef:
         """
         Lists the log pattern sets in the specific application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/application-insights.html#ApplicationInsights.Client.list_log_pattern_sets)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_application_insights/client/#list_log_pattern_sets)
         """
     async def list_log_patterns(
         self,
         *,
         ResourceGroupName: str,
         PatternSetName: str = ...,
         MaxResults: int = ...,
-        NextToken: str = ...
+        NextToken: str = ...,
+        AccountId: str = ...
     ) -> ListLogPatternsResponseTypeDef:
         """
         Lists the log patterns in the specific log `LogPatternSet`.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/application-insights.html#ApplicationInsights.Client.list_log_patterns)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_application_insights/client/#list_log_patterns)
         """
     async def list_problems(
         self,
         *,
+        AccountId: str = ...,
         ResourceGroupName: str = ...,
         StartTime: TimestampTypeDef = ...,
         EndTime: TimestampTypeDef = ...,
         MaxResults: int = ...,
         NextToken: str = ...,
-        ComponentName: str = ...
+        ComponentName: str = ...,
+        Visibility: VisibilityType = ...
     ) -> ListProblemsResponseTypeDef:
         """
         Lists the problems with your application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/application-insights.html#ApplicationInsights.Client.list_problems)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_application_insights/client/#list_problems)
         """
@@ -331,14 +379,38 @@
         """
         Retrieve a list of the tags (keys and values) that are associated with a
         specified application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/application-insights.html#ApplicationInsights.Client.list_tags_for_resource)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_application_insights/client/#list_tags_for_resource)
         """
+    async def list_workloads(
+        self,
+        *,
+        ResourceGroupName: str,
+        ComponentName: str,
+        MaxResults: int = ...,
+        NextToken: str = ...,
+        AccountId: str = ...
+    ) -> ListWorkloadsResponseTypeDef:
+        """
+        Lists the workloads that are configured on a given component.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/application-insights.html#ApplicationInsights.Client.list_workloads)
+        [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_application_insights/client/#list_workloads)
+        """
+    async def remove_workload(
+        self, *, ResourceGroupName: str, ComponentName: str, WorkloadId: str
+    ) -> Dict[str, Any]:
+        """
+        Remove workload from a component.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/application-insights.html#ApplicationInsights.Client.remove_workload)
+        [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_application_insights/client/#remove_workload)
+        """
     async def tag_resource(self, *, ResourceARN: str, Tags: Sequence[TagTypeDef]) -> Dict[str, Any]:
         """
         Add one or more tags (keys and values) to a specified application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/application-insights.html#ApplicationInsights.Client.tag_resource)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_application_insights/client/#tag_resource)
         """
@@ -407,14 +479,41 @@
     ) -> UpdateLogPatternResponseTypeDef:
         """
         Adds a log pattern to a `LogPatternSet`.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/application-insights.html#ApplicationInsights.Client.update_log_pattern)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_application_insights/client/#update_log_pattern)
         """
+    async def update_problem(
+        self,
+        *,
+        ProblemId: str,
+        UpdateStatus: Literal["RESOLVED"] = ...,
+        Visibility: VisibilityType = ...
+    ) -> Dict[str, Any]:
+        """
+        Updates the visibility of the problem or specifies the problem as `RESOLVED`.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/application-insights.html#ApplicationInsights.Client.update_problem)
+        [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_application_insights/client/#update_problem)
+        """
+    async def update_workload(
+        self,
+        *,
+        ResourceGroupName: str,
+        ComponentName: str,
+        WorkloadConfiguration: WorkloadConfigurationTypeDef,
+        WorkloadId: str = ...
+    ) -> UpdateWorkloadResponseTypeDef:
+        """
+        Adds a workload to a component.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/application-insights.html#ApplicationInsights.Client.update_workload)
+        [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_application_insights/client/#update_workload)
+        """
     async def __aenter__(self) -> "ApplicationInsightsClient":
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/application-insights.html#ApplicationInsights.Client)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_application_insights/client/)
         """
     async def __aexit__(self, exc_type: Any, exc_val: Any, exc_tb: Any) -> Any:
         """
```

### Comparing `types-aiobotocore-application-insights-2.5.2.post3/types_aiobotocore_application_insights/literals.py` & `types-aiobotocore-application-insights-2.5.4/types_aiobotocore_application_insights/literals.py`

 * *Files 3% similar despite different names*

```diff
@@ -25,17 +25,21 @@
     "ConfigurationEventStatusType",
     "DiscoveryTypeType",
     "FeedbackKeyType",
     "FeedbackValueType",
     "GroupingTypeType",
     "LogFilterType",
     "OsTypeType",
+    "RecommendationTypeType",
+    "ResolutionMethodType",
     "SeverityLevelType",
     "StatusType",
     "TierType",
+    "UpdateStatusType",
+    "VisibilityType",
     "ApplicationInsightsServiceName",
     "ServiceName",
     "ResourceServiceName",
     "RegionName",
 )
 
 
@@ -46,16 +50,18 @@
 ConfigurationEventStatusType = Literal["ERROR", "INFO", "WARN"]
 DiscoveryTypeType = Literal["ACCOUNT_BASED", "RESOURCE_GROUP_BASED"]
 FeedbackKeyType = Literal["INSIGHTS_FEEDBACK"]
 FeedbackValueType = Literal["NOT_SPECIFIED", "NOT_USEFUL", "USEFUL"]
 GroupingTypeType = Literal["ACCOUNT_BASED"]
 LogFilterType = Literal["ERROR", "INFO", "WARN"]
 OsTypeType = Literal["LINUX", "WINDOWS"]
+RecommendationTypeType = Literal["ALL", "INFRA_ONLY", "WORKLOAD_ONLY"]
+ResolutionMethodType = Literal["AUTOMATIC", "MANUAL", "UNRESOLVED"]
 SeverityLevelType = Literal["High", "Informative", "Low", "Medium"]
-StatusType = Literal["IGNORE", "PENDING", "RECURRING", "RESOLVED"]
+StatusType = Literal["IGNORE", "PENDING", "RECOVERING", "RECURRING", "RESOLVED"]
 TierType = Literal[
     "ACTIVE_DIRECTORY",
     "CUSTOM",
     "DEFAULT",
     "DOT_NET_CORE",
     "DOT_NET_WEB",
     "DOT_NET_WEB_TIER",
@@ -63,19 +69,24 @@
     "JAVA_JMX",
     "MYSQL",
     "ORACLE",
     "POSTGRESQL",
     "SAP_HANA_HIGH_AVAILABILITY",
     "SAP_HANA_MULTI_NODE",
     "SAP_HANA_SINGLE_NODE",
+    "SAP_NETWEAVER_DISTRIBUTED",
+    "SAP_NETWEAVER_HIGH_AVAILABILITY",
+    "SAP_NETWEAVER_STANDARD",
     "SHAREPOINT",
     "SQL_SERVER",
     "SQL_SERVER_ALWAYSON_AVAILABILITY_GROUP",
     "SQL_SERVER_FAILOVER_CLUSTER_INSTANCE",
 ]
+UpdateStatusType = Literal["RESOLVED"]
+VisibilityType = Literal["IGNORED", "VISIBLE"]
 ApplicationInsightsServiceName = Literal["application-insights"]
 ServiceName = Literal[
     "accessanalyzer",
     "account",
     "acm",
     "acm-pca",
     "alexaforbusiness",
@@ -84,14 +95,15 @@
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
@@ -187,14 +199,15 @@
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
@@ -273,26 +286,28 @@
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
@@ -439,24 +454,28 @@
 RegionName = Literal[
     "af-south-1",
     "ap-east-1",
     "ap-northeast-1",
     "ap-northeast-2",
     "ap-northeast-3",
     "ap-south-1",
+    "ap-south-2",
     "ap-southeast-1",
     "ap-southeast-2",
     "ap-southeast-3",
     "ca-central-1",
     "eu-central-1",
+    "eu-central-2",
     "eu-north-1",
     "eu-south-1",
+    "eu-south-2",
     "eu-west-1",
     "eu-west-2",
     "eu-west-3",
+    "me-central-1",
     "me-south-1",
     "sa-east-1",
     "us-east-1",
     "us-east-2",
     "us-west-1",
     "us-west-2",
 ]
```

### Comparing `types-aiobotocore-application-insights-2.5.2.post3/types_aiobotocore_application_insights/literals.pyi` & `types-aiobotocore-application-insights-2.5.4/types_aiobotocore_application_insights/literals.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -24,17 +24,21 @@
     "ConfigurationEventStatusType",
     "DiscoveryTypeType",
     "FeedbackKeyType",
     "FeedbackValueType",
     "GroupingTypeType",
     "LogFilterType",
     "OsTypeType",
+    "RecommendationTypeType",
+    "ResolutionMethodType",
     "SeverityLevelType",
     "StatusType",
     "TierType",
+    "UpdateStatusType",
+    "VisibilityType",
     "ApplicationInsightsServiceName",
     "ServiceName",
     "ResourceServiceName",
     "RegionName",
 )
 
 CloudWatchEventSourceType = Literal["CODE_DEPLOY", "EC2", "HEALTH", "RDS"]
@@ -44,16 +48,18 @@
 ConfigurationEventStatusType = Literal["ERROR", "INFO", "WARN"]
 DiscoveryTypeType = Literal["ACCOUNT_BASED", "RESOURCE_GROUP_BASED"]
 FeedbackKeyType = Literal["INSIGHTS_FEEDBACK"]
 FeedbackValueType = Literal["NOT_SPECIFIED", "NOT_USEFUL", "USEFUL"]
 GroupingTypeType = Literal["ACCOUNT_BASED"]
 LogFilterType = Literal["ERROR", "INFO", "WARN"]
 OsTypeType = Literal["LINUX", "WINDOWS"]
+RecommendationTypeType = Literal["ALL", "INFRA_ONLY", "WORKLOAD_ONLY"]
+ResolutionMethodType = Literal["AUTOMATIC", "MANUAL", "UNRESOLVED"]
 SeverityLevelType = Literal["High", "Informative", "Low", "Medium"]
-StatusType = Literal["IGNORE", "PENDING", "RECURRING", "RESOLVED"]
+StatusType = Literal["IGNORE", "PENDING", "RECOVERING", "RECURRING", "RESOLVED"]
 TierType = Literal[
     "ACTIVE_DIRECTORY",
     "CUSTOM",
     "DEFAULT",
     "DOT_NET_CORE",
     "DOT_NET_WEB",
     "DOT_NET_WEB_TIER",
@@ -61,19 +67,24 @@
     "JAVA_JMX",
     "MYSQL",
     "ORACLE",
     "POSTGRESQL",
     "SAP_HANA_HIGH_AVAILABILITY",
     "SAP_HANA_MULTI_NODE",
     "SAP_HANA_SINGLE_NODE",
+    "SAP_NETWEAVER_DISTRIBUTED",
+    "SAP_NETWEAVER_HIGH_AVAILABILITY",
+    "SAP_NETWEAVER_STANDARD",
     "SHAREPOINT",
     "SQL_SERVER",
     "SQL_SERVER_ALWAYSON_AVAILABILITY_GROUP",
     "SQL_SERVER_FAILOVER_CLUSTER_INSTANCE",
 ]
+UpdateStatusType = Literal["RESOLVED"]
+VisibilityType = Literal["IGNORED", "VISIBLE"]
 ApplicationInsightsServiceName = Literal["application-insights"]
 ServiceName = Literal[
     "accessanalyzer",
     "account",
     "acm",
     "acm-pca",
     "alexaforbusiness",
@@ -82,14 +93,15 @@
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
@@ -185,14 +197,15 @@
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
@@ -271,26 +284,28 @@
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
@@ -437,24 +452,28 @@
 RegionName = Literal[
     "af-south-1",
     "ap-east-1",
     "ap-northeast-1",
     "ap-northeast-2",
     "ap-northeast-3",
     "ap-south-1",
+    "ap-south-2",
     "ap-southeast-1",
     "ap-southeast-2",
     "ap-southeast-3",
     "ca-central-1",
     "eu-central-1",
+    "eu-central-2",
     "eu-north-1",
     "eu-south-1",
+    "eu-south-2",
     "eu-west-1",
     "eu-west-2",
     "eu-west-3",
+    "me-central-1",
     "me-south-1",
     "sa-east-1",
     "us-east-1",
     "us-east-2",
     "us-west-1",
     "us-west-2",
 ]
```

### Comparing `types-aiobotocore-application-insights-2.5.2.post3/types_aiobotocore_application_insights/type_defs.py` & `types-aiobotocore-application-insights-2.5.4/types_aiobotocore_application_insights/type_defs.py`

 * *Files 18% similar despite different names*

```diff
@@ -2,52 +2,56 @@
 Type annotations for application-insights service type definitions.
 
 [Open documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_application_insights/type_defs/)
 
 Usage::
 
     ```python
-    from types_aiobotocore_application_insights.type_defs import ApplicationComponentTypeDef
+    from types_aiobotocore_application_insights.type_defs import WorkloadConfigurationTypeDef
 
-    data: ApplicationComponentTypeDef = ...
+    data: WorkloadConfigurationTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, List, Sequence, Union
 
 from .literals import (
     CloudWatchEventSourceType,
     ConfigurationEventResourceTypeType,
     ConfigurationEventStatusType,
     DiscoveryTypeType,
     FeedbackValueType,
     LogFilterType,
     OsTypeType,
+    RecommendationTypeType,
+    ResolutionMethodType,
     SeverityLevelType,
     StatusType,
     TierType,
+    VisibilityType,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 
 __all__ = (
+    "WorkloadConfigurationTypeDef",
+    "ResponseMetadataTypeDef",
     "ApplicationComponentTypeDef",
     "ApplicationInfoTypeDef",
     "ConfigurationEventTypeDef",
     "TagTypeDef",
-    "ResponseMetadataTypeDef",
     "CreateComponentRequestRequestTypeDef",
     "CreateLogPatternRequestRequestTypeDef",
     "LogPatternTypeDef",
     "DeleteApplicationRequestRequestTypeDef",
     "DeleteComponentRequestRequestTypeDef",
     "DeleteLogPatternRequestRequestTypeDef",
     "DescribeApplicationRequestRequestTypeDef",
@@ -56,51 +60,83 @@
     "DescribeComponentRequestRequestTypeDef",
     "DescribeLogPatternRequestRequestTypeDef",
     "DescribeObservationRequestRequestTypeDef",
     "ObservationTypeDef",
     "DescribeProblemObservationsRequestRequestTypeDef",
     "DescribeProblemRequestRequestTypeDef",
     "ProblemTypeDef",
+    "DescribeWorkloadRequestRequestTypeDef",
     "ListApplicationsRequestRequestTypeDef",
     "ListComponentsRequestRequestTypeDef",
     "TimestampTypeDef",
     "ListLogPatternSetsRequestRequestTypeDef",
     "ListLogPatternsRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
+    "ListWorkloadsRequestRequestTypeDef",
+    "WorkloadTypeDef",
+    "RemoveWorkloadRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateApplicationRequestRequestTypeDef",
     "UpdateComponentConfigurationRequestRequestTypeDef",
     "UpdateComponentRequestRequestTypeDef",
     "UpdateLogPatternRequestRequestTypeDef",
-    "CreateApplicationRequestRequestTypeDef",
-    "TagResourceRequestRequestTypeDef",
-    "CreateApplicationResponseTypeDef",
-    "DescribeApplicationResponseTypeDef",
+    "UpdateProblemRequestRequestTypeDef",
+    "AddWorkloadRequestRequestTypeDef",
+    "UpdateWorkloadRequestRequestTypeDef",
+    "AddWorkloadResponseTypeDef",
     "DescribeComponentConfigurationRecommendationResponseTypeDef",
     "DescribeComponentConfigurationResponseTypeDef",
+    "DescribeWorkloadResponseTypeDef",
+    "ListLogPatternSetsResponseTypeDef",
+    "UpdateWorkloadResponseTypeDef",
     "DescribeComponentResponseTypeDef",
-    "ListApplicationsResponseTypeDef",
     "ListComponentsResponseTypeDef",
+    "CreateApplicationResponseTypeDef",
+    "DescribeApplicationResponseTypeDef",
+    "ListApplicationsResponseTypeDef",
+    "UpdateApplicationResponseTypeDef",
     "ListConfigurationHistoryResponseTypeDef",
-    "ListLogPatternSetsResponseTypeDef",
+    "CreateApplicationRequestRequestTypeDef",
     "ListTagsForResourceResponseTypeDef",
-    "UpdateApplicationResponseTypeDef",
+    "TagResourceRequestRequestTypeDef",
     "CreateLogPatternResponseTypeDef",
     "DescribeLogPatternResponseTypeDef",
     "ListLogPatternsResponseTypeDef",
     "UpdateLogPatternResponseTypeDef",
     "DescribeObservationResponseTypeDef",
     "RelatedObservationsTypeDef",
     "DescribeProblemResponseTypeDef",
     "ListProblemsResponseTypeDef",
     "ListConfigurationHistoryRequestRequestTypeDef",
     "ListProblemsRequestRequestTypeDef",
+    "ListWorkloadsResponseTypeDef",
     "DescribeProblemObservationsResponseTypeDef",
 )
 
+WorkloadConfigurationTypeDef = TypedDict(
+    "WorkloadConfigurationTypeDef",
+    {
+        "WorkloadName": str,
+        "Tier": TierType,
+        "Configuration": str,
+    },
+    total=False,
+)
+
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
+    {
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
+    },
+)
+
 ApplicationComponentTypeDef = TypedDict(
     "ApplicationComponentTypeDef",
     {
         "ComponentName": str,
         "ComponentRemarks": str,
         "ResourceType": str,
         "OsType": OsTypeType,
@@ -110,14 +146,15 @@
     },
     total=False,
 )
 
 ApplicationInfoTypeDef = TypedDict(
     "ApplicationInfoTypeDef",
     {
+        "AccountId": str,
         "ResourceGroupName": str,
         "LifeCycle": str,
         "OpsItemSNSTopicArn": str,
         "OpsCenterEnabled": bool,
         "CWEMonitorEnabled": bool,
         "Remarks": str,
         "AutoConfigEnabled": bool,
@@ -125,14 +162,16 @@
     },
     total=False,
 )
 
 ConfigurationEventTypeDef = TypedDict(
     "ConfigurationEventTypeDef",
     {
+        "ResourceGroupName": str,
+        "AccountId": str,
         "MonitoredResourceARN": str,
         "EventStatus": ConfigurationEventStatusType,
         "EventResourceType": ConfigurationEventResourceTypeType,
         "EventTime": datetime,
         "EventDetail": str,
         "EventResourceName": str,
     },
@@ -143,25 +182,14 @@
     "TagTypeDef",
     {
         "Key": str,
         "Value": str,
     },
 )
 
-ResponseMetadataTypeDef = TypedDict(
-    "ResponseMetadataTypeDef",
-    {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
-    },
-)
-
 CreateComponentRequestRequestTypeDef = TypedDict(
     "CreateComponentRequestRequestTypeDef",
     {
         "ResourceGroupName": str,
         "ComponentName": str,
         "ResourceList": Sequence[str],
     },
@@ -209,61 +237,150 @@
     {
         "ResourceGroupName": str,
         "PatternSetName": str,
         "PatternName": str,
     },
 )
 
-DescribeApplicationRequestRequestTypeDef = TypedDict(
-    "DescribeApplicationRequestRequestTypeDef",
+_RequiredDescribeApplicationRequestRequestTypeDef = TypedDict(
+    "_RequiredDescribeApplicationRequestRequestTypeDef",
     {
         "ResourceGroupName": str,
     },
 )
+_OptionalDescribeApplicationRequestRequestTypeDef = TypedDict(
+    "_OptionalDescribeApplicationRequestRequestTypeDef",
+    {
+        "AccountId": str,
+    },
+    total=False,
+)
 
-DescribeComponentConfigurationRecommendationRequestRequestTypeDef = TypedDict(
-    "DescribeComponentConfigurationRecommendationRequestRequestTypeDef",
+
+class DescribeApplicationRequestRequestTypeDef(
+    _RequiredDescribeApplicationRequestRequestTypeDef,
+    _OptionalDescribeApplicationRequestRequestTypeDef,
+):
+    pass
+
+
+_RequiredDescribeComponentConfigurationRecommendationRequestRequestTypeDef = TypedDict(
+    "_RequiredDescribeComponentConfigurationRecommendationRequestRequestTypeDef",
     {
         "ResourceGroupName": str,
         "ComponentName": str,
         "Tier": TierType,
     },
 )
+_OptionalDescribeComponentConfigurationRecommendationRequestRequestTypeDef = TypedDict(
+    "_OptionalDescribeComponentConfigurationRecommendationRequestRequestTypeDef",
+    {
+        "RecommendationType": RecommendationTypeType,
+    },
+    total=False,
+)
 
-DescribeComponentConfigurationRequestRequestTypeDef = TypedDict(
-    "DescribeComponentConfigurationRequestRequestTypeDef",
+
+class DescribeComponentConfigurationRecommendationRequestRequestTypeDef(
+    _RequiredDescribeComponentConfigurationRecommendationRequestRequestTypeDef,
+    _OptionalDescribeComponentConfigurationRecommendationRequestRequestTypeDef,
+):
+    pass
+
+
+_RequiredDescribeComponentConfigurationRequestRequestTypeDef = TypedDict(
+    "_RequiredDescribeComponentConfigurationRequestRequestTypeDef",
     {
         "ResourceGroupName": str,
         "ComponentName": str,
     },
 )
+_OptionalDescribeComponentConfigurationRequestRequestTypeDef = TypedDict(
+    "_OptionalDescribeComponentConfigurationRequestRequestTypeDef",
+    {
+        "AccountId": str,
+    },
+    total=False,
+)
 
-DescribeComponentRequestRequestTypeDef = TypedDict(
-    "DescribeComponentRequestRequestTypeDef",
+
+class DescribeComponentConfigurationRequestRequestTypeDef(
+    _RequiredDescribeComponentConfigurationRequestRequestTypeDef,
+    _OptionalDescribeComponentConfigurationRequestRequestTypeDef,
+):
+    pass
+
+
+_RequiredDescribeComponentRequestRequestTypeDef = TypedDict(
+    "_RequiredDescribeComponentRequestRequestTypeDef",
     {
         "ResourceGroupName": str,
         "ComponentName": str,
     },
 )
+_OptionalDescribeComponentRequestRequestTypeDef = TypedDict(
+    "_OptionalDescribeComponentRequestRequestTypeDef",
+    {
+        "AccountId": str,
+    },
+    total=False,
+)
 
-DescribeLogPatternRequestRequestTypeDef = TypedDict(
-    "DescribeLogPatternRequestRequestTypeDef",
+
+class DescribeComponentRequestRequestTypeDef(
+    _RequiredDescribeComponentRequestRequestTypeDef, _OptionalDescribeComponentRequestRequestTypeDef
+):
+    pass
+
+
+_RequiredDescribeLogPatternRequestRequestTypeDef = TypedDict(
+    "_RequiredDescribeLogPatternRequestRequestTypeDef",
     {
         "ResourceGroupName": str,
         "PatternSetName": str,
         "PatternName": str,
     },
 )
+_OptionalDescribeLogPatternRequestRequestTypeDef = TypedDict(
+    "_OptionalDescribeLogPatternRequestRequestTypeDef",
+    {
+        "AccountId": str,
+    },
+    total=False,
+)
 
-DescribeObservationRequestRequestTypeDef = TypedDict(
-    "DescribeObservationRequestRequestTypeDef",
+
+class DescribeLogPatternRequestRequestTypeDef(
+    _RequiredDescribeLogPatternRequestRequestTypeDef,
+    _OptionalDescribeLogPatternRequestRequestTypeDef,
+):
+    pass
+
+
+_RequiredDescribeObservationRequestRequestTypeDef = TypedDict(
+    "_RequiredDescribeObservationRequestRequestTypeDef",
     {
         "ObservationId": str,
     },
 )
+_OptionalDescribeObservationRequestRequestTypeDef = TypedDict(
+    "_OptionalDescribeObservationRequestRequestTypeDef",
+    {
+        "AccountId": str,
+    },
+    total=False,
+)
+
+
+class DescribeObservationRequestRequestTypeDef(
+    _RequiredDescribeObservationRequestRequestTypeDef,
+    _OptionalDescribeObservationRequestRequestTypeDef,
+):
+    pass
+
 
 ObservationTypeDef = TypedDict(
     "ObservationTypeDef",
     {
         "Id": str,
         "StartTime": datetime,
         "EndTime": datetime,
@@ -309,52 +426,108 @@
         "XRayRequestAverageLatency": int,
         "XRayNodeName": str,
         "XRayNodeType": str,
     },
     total=False,
 )
 
-DescribeProblemObservationsRequestRequestTypeDef = TypedDict(
-    "DescribeProblemObservationsRequestRequestTypeDef",
+_RequiredDescribeProblemObservationsRequestRequestTypeDef = TypedDict(
+    "_RequiredDescribeProblemObservationsRequestRequestTypeDef",
     {
         "ProblemId": str,
     },
 )
+_OptionalDescribeProblemObservationsRequestRequestTypeDef = TypedDict(
+    "_OptionalDescribeProblemObservationsRequestRequestTypeDef",
+    {
+        "AccountId": str,
+    },
+    total=False,
+)
 
-DescribeProblemRequestRequestTypeDef = TypedDict(
-    "DescribeProblemRequestRequestTypeDef",
+
+class DescribeProblemObservationsRequestRequestTypeDef(
+    _RequiredDescribeProblemObservationsRequestRequestTypeDef,
+    _OptionalDescribeProblemObservationsRequestRequestTypeDef,
+):
+    pass
+
+
+_RequiredDescribeProblemRequestRequestTypeDef = TypedDict(
+    "_RequiredDescribeProblemRequestRequestTypeDef",
     {
         "ProblemId": str,
     },
 )
+_OptionalDescribeProblemRequestRequestTypeDef = TypedDict(
+    "_OptionalDescribeProblemRequestRequestTypeDef",
+    {
+        "AccountId": str,
+    },
+    total=False,
+)
+
+
+class DescribeProblemRequestRequestTypeDef(
+    _RequiredDescribeProblemRequestRequestTypeDef, _OptionalDescribeProblemRequestRequestTypeDef
+):
+    pass
+
 
 ProblemTypeDef = TypedDict(
     "ProblemTypeDef",
     {
         "Id": str,
         "Title": str,
         "Insights": str,
         "Status": StatusType,
         "AffectedResource": str,
         "StartTime": datetime,
         "EndTime": datetime,
         "SeverityLevel": SeverityLevelType,
+        "AccountId": str,
         "ResourceGroupName": str,
         "Feedback": Dict[Literal["INSIGHTS_FEEDBACK"], FeedbackValueType],
         "RecurringCount": int,
         "LastRecurrenceTime": datetime,
+        "Visibility": VisibilityType,
+        "ResolutionMethod": ResolutionMethodType,
+    },
+    total=False,
+)
+
+_RequiredDescribeWorkloadRequestRequestTypeDef = TypedDict(
+    "_RequiredDescribeWorkloadRequestRequestTypeDef",
+    {
+        "ResourceGroupName": str,
+        "ComponentName": str,
+        "WorkloadId": str,
+    },
+)
+_OptionalDescribeWorkloadRequestRequestTypeDef = TypedDict(
+    "_OptionalDescribeWorkloadRequestRequestTypeDef",
+    {
+        "AccountId": str,
     },
     total=False,
 )
 
+
+class DescribeWorkloadRequestRequestTypeDef(
+    _RequiredDescribeWorkloadRequestRequestTypeDef, _OptionalDescribeWorkloadRequestRequestTypeDef
+):
+    pass
+
+
 ListApplicationsRequestRequestTypeDef = TypedDict(
     "ListApplicationsRequestRequestTypeDef",
     {
         "MaxResults": int,
         "NextToken": str,
+        "AccountId": str,
     },
     total=False,
 )
 
 _RequiredListComponentsRequestRequestTypeDef = TypedDict(
     "_RequiredListComponentsRequestRequestTypeDef",
     {
@@ -362,14 +535,15 @@
     },
 )
 _OptionalListComponentsRequestRequestTypeDef = TypedDict(
     "_OptionalListComponentsRequestRequestTypeDef",
     {
         "MaxResults": int,
         "NextToken": str,
+        "AccountId": str,
     },
     total=False,
 )
 
 
 class ListComponentsRequestRequestTypeDef(
     _RequiredListComponentsRequestRequestTypeDef, _OptionalListComponentsRequestRequestTypeDef
@@ -385,14 +559,15 @@
     },
 )
 _OptionalListLogPatternSetsRequestRequestTypeDef = TypedDict(
     "_OptionalListLogPatternSetsRequestRequestTypeDef",
     {
         "MaxResults": int,
         "NextToken": str,
+        "AccountId": str,
     },
     total=False,
 )
 
 
 class ListLogPatternSetsRequestRequestTypeDef(
     _RequiredListLogPatternSetsRequestRequestTypeDef,
@@ -409,14 +584,15 @@
 )
 _OptionalListLogPatternsRequestRequestTypeDef = TypedDict(
     "_OptionalListLogPatternsRequestRequestTypeDef",
     {
         "PatternSetName": str,
         "MaxResults": int,
         "NextToken": str,
+        "AccountId": str,
     },
     total=False,
 )
 
 
 class ListLogPatternsRequestRequestTypeDef(
     _RequiredListLogPatternsRequestRequestTypeDef, _OptionalListLogPatternsRequestRequestTypeDef
@@ -427,14 +603,59 @@
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "ResourceARN": str,
     },
 )
 
+_RequiredListWorkloadsRequestRequestTypeDef = TypedDict(
+    "_RequiredListWorkloadsRequestRequestTypeDef",
+    {
+        "ResourceGroupName": str,
+        "ComponentName": str,
+    },
+)
+_OptionalListWorkloadsRequestRequestTypeDef = TypedDict(
+    "_OptionalListWorkloadsRequestRequestTypeDef",
+    {
+        "MaxResults": int,
+        "NextToken": str,
+        "AccountId": str,
+    },
+    total=False,
+)
+
+
+class ListWorkloadsRequestRequestTypeDef(
+    _RequiredListWorkloadsRequestRequestTypeDef, _OptionalListWorkloadsRequestRequestTypeDef
+):
+    pass
+
+
+WorkloadTypeDef = TypedDict(
+    "WorkloadTypeDef",
+    {
+        "WorkloadId": str,
+        "ComponentName": str,
+        "WorkloadName": str,
+        "Tier": TierType,
+        "WorkloadRemarks": str,
+    },
+    total=False,
+)
+
+RemoveWorkloadRequestRequestTypeDef = TypedDict(
+    "RemoveWorkloadRequestRequestTypeDef",
+    {
+        "ResourceGroupName": str,
+        "ComponentName": str,
+        "WorkloadId": str,
+    },
+)
+
 UntagResourceRequestRequestTypeDef = TypedDict(
     "UntagResourceRequestRequestTypeDef",
     {
         "ResourceARN": str,
         "TagKeys": Sequence[str],
     },
 )
@@ -533,49 +754,73 @@
 
 class UpdateLogPatternRequestRequestTypeDef(
     _RequiredUpdateLogPatternRequestRequestTypeDef, _OptionalUpdateLogPatternRequestRequestTypeDef
 ):
     pass
 
 
-CreateApplicationRequestRequestTypeDef = TypedDict(
-    "CreateApplicationRequestRequestTypeDef",
+_RequiredUpdateProblemRequestRequestTypeDef = TypedDict(
+    "_RequiredUpdateProblemRequestRequestTypeDef",
     {
-        "ResourceGroupName": str,
-        "OpsCenterEnabled": bool,
-        "CWEMonitorEnabled": bool,
-        "OpsItemSNSTopicArn": str,
-        "Tags": Sequence[TagTypeDef],
-        "AutoConfigEnabled": bool,
-        "AutoCreate": bool,
-        "GroupingType": Literal["ACCOUNT_BASED"],
+        "ProblemId": str,
+    },
+)
+_OptionalUpdateProblemRequestRequestTypeDef = TypedDict(
+    "_OptionalUpdateProblemRequestRequestTypeDef",
+    {
+        "UpdateStatus": Literal["RESOLVED"],
+        "Visibility": VisibilityType,
     },
     total=False,
 )
 
-TagResourceRequestRequestTypeDef = TypedDict(
-    "TagResourceRequestRequestTypeDef",
+
+class UpdateProblemRequestRequestTypeDef(
+    _RequiredUpdateProblemRequestRequestTypeDef, _OptionalUpdateProblemRequestRequestTypeDef
+):
+    pass
+
+
+AddWorkloadRequestRequestTypeDef = TypedDict(
+    "AddWorkloadRequestRequestTypeDef",
     {
-        "ResourceARN": str,
-        "Tags": Sequence[TagTypeDef],
+        "ResourceGroupName": str,
+        "ComponentName": str,
+        "WorkloadConfiguration": WorkloadConfigurationTypeDef,
     },
 )
 
-CreateApplicationResponseTypeDef = TypedDict(
-    "CreateApplicationResponseTypeDef",
+_RequiredUpdateWorkloadRequestRequestTypeDef = TypedDict(
+    "_RequiredUpdateWorkloadRequestRequestTypeDef",
     {
-        "ApplicationInfo": ApplicationInfoTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResourceGroupName": str,
+        "ComponentName": str,
+        "WorkloadConfiguration": WorkloadConfigurationTypeDef,
     },
 )
+_OptionalUpdateWorkloadRequestRequestTypeDef = TypedDict(
+    "_OptionalUpdateWorkloadRequestRequestTypeDef",
+    {
+        "WorkloadId": str,
+    },
+    total=False,
+)
 
-DescribeApplicationResponseTypeDef = TypedDict(
-    "DescribeApplicationResponseTypeDef",
+
+class UpdateWorkloadRequestRequestTypeDef(
+    _RequiredUpdateWorkloadRequestRequestTypeDef, _OptionalUpdateWorkloadRequestRequestTypeDef
+):
+    pass
+
+
+AddWorkloadResponseTypeDef = TypedDict(
+    "AddWorkloadResponseTypeDef",
     {
-        "ApplicationInfo": ApplicationInfoTypeDef,
+        "WorkloadId": str,
+        "WorkloadConfiguration": WorkloadConfigurationTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeComponentConfigurationRecommendationResponseTypeDef = TypedDict(
     "DescribeComponentConfigurationRecommendationResponseTypeDef",
     {
@@ -590,73 +835,132 @@
         "Monitor": bool,
         "Tier": TierType,
         "ComponentConfiguration": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+DescribeWorkloadResponseTypeDef = TypedDict(
+    "DescribeWorkloadResponseTypeDef",
+    {
+        "WorkloadId": str,
+        "WorkloadRemarks": str,
+        "WorkloadConfiguration": WorkloadConfigurationTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListLogPatternSetsResponseTypeDef = TypedDict(
+    "ListLogPatternSetsResponseTypeDef",
+    {
+        "ResourceGroupName": str,
+        "AccountId": str,
+        "LogPatternSets": List[str],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateWorkloadResponseTypeDef = TypedDict(
+    "UpdateWorkloadResponseTypeDef",
+    {
+        "WorkloadId": str,
+        "WorkloadConfiguration": WorkloadConfigurationTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 DescribeComponentResponseTypeDef = TypedDict(
     "DescribeComponentResponseTypeDef",
     {
         "ApplicationComponent": ApplicationComponentTypeDef,
         "ResourceList": List[str],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+ListComponentsResponseTypeDef = TypedDict(
+    "ListComponentsResponseTypeDef",
+    {
+        "ApplicationComponentList": List[ApplicationComponentTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateApplicationResponseTypeDef = TypedDict(
+    "CreateApplicationResponseTypeDef",
+    {
+        "ApplicationInfo": ApplicationInfoTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeApplicationResponseTypeDef = TypedDict(
+    "DescribeApplicationResponseTypeDef",
+    {
+        "ApplicationInfo": ApplicationInfoTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 ListApplicationsResponseTypeDef = TypedDict(
     "ListApplicationsResponseTypeDef",
     {
         "ApplicationInfoList": List[ApplicationInfoTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-ListComponentsResponseTypeDef = TypedDict(
-    "ListComponentsResponseTypeDef",
+UpdateApplicationResponseTypeDef = TypedDict(
+    "UpdateApplicationResponseTypeDef",
     {
-        "ApplicationComponentList": List[ApplicationComponentTypeDef],
-        "NextToken": str,
+        "ApplicationInfo": ApplicationInfoTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListConfigurationHistoryResponseTypeDef = TypedDict(
     "ListConfigurationHistoryResponseTypeDef",
     {
         "EventList": List[ConfigurationEventTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-ListLogPatternSetsResponseTypeDef = TypedDict(
-    "ListLogPatternSetsResponseTypeDef",
+CreateApplicationRequestRequestTypeDef = TypedDict(
+    "CreateApplicationRequestRequestTypeDef",
     {
         "ResourceGroupName": str,
-        "LogPatternSets": List[str],
-        "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "OpsCenterEnabled": bool,
+        "CWEMonitorEnabled": bool,
+        "OpsItemSNSTopicArn": str,
+        "Tags": Sequence[TagTypeDef],
+        "AutoConfigEnabled": bool,
+        "AutoCreate": bool,
+        "GroupingType": Literal["ACCOUNT_BASED"],
     },
+    total=False,
 )
 
 ListTagsForResourceResponseTypeDef = TypedDict(
     "ListTagsForResourceResponseTypeDef",
     {
         "Tags": List[TagTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-UpdateApplicationResponseTypeDef = TypedDict(
-    "UpdateApplicationResponseTypeDef",
+TagResourceRequestRequestTypeDef = TypedDict(
+    "TagResourceRequestRequestTypeDef",
     {
-        "ApplicationInfo": ApplicationInfoTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResourceARN": str,
+        "Tags": Sequence[TagTypeDef],
     },
 )
 
 CreateLogPatternResponseTypeDef = TypedDict(
     "CreateLogPatternResponseTypeDef",
     {
         "LogPattern": LogPatternTypeDef,
@@ -665,23 +969,25 @@
     },
 )
 
 DescribeLogPatternResponseTypeDef = TypedDict(
     "DescribeLogPatternResponseTypeDef",
     {
         "ResourceGroupName": str,
+        "AccountId": str,
         "LogPattern": LogPatternTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListLogPatternsResponseTypeDef = TypedDict(
     "ListLogPatternsResponseTypeDef",
     {
         "ResourceGroupName": str,
+        "AccountId": str,
         "LogPatterns": List[LogPatternTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateLogPatternResponseTypeDef = TypedDict(
@@ -719,44 +1025,57 @@
 
 ListProblemsResponseTypeDef = TypedDict(
     "ListProblemsResponseTypeDef",
     {
         "ProblemList": List[ProblemTypeDef],
         "NextToken": str,
         "ResourceGroupName": str,
+        "AccountId": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListConfigurationHistoryRequestRequestTypeDef = TypedDict(
     "ListConfigurationHistoryRequestRequestTypeDef",
     {
         "ResourceGroupName": str,
         "StartTime": TimestampTypeDef,
         "EndTime": TimestampTypeDef,
         "EventStatus": ConfigurationEventStatusType,
         "MaxResults": int,
         "NextToken": str,
+        "AccountId": str,
     },
     total=False,
 )
 
 ListProblemsRequestRequestTypeDef = TypedDict(
     "ListProblemsRequestRequestTypeDef",
     {
+        "AccountId": str,
         "ResourceGroupName": str,
         "StartTime": TimestampTypeDef,
         "EndTime": TimestampTypeDef,
         "MaxResults": int,
         "NextToken": str,
         "ComponentName": str,
+        "Visibility": VisibilityType,
     },
     total=False,
 )
 
+ListWorkloadsResponseTypeDef = TypedDict(
+    "ListWorkloadsResponseTypeDef",
+    {
+        "WorkloadList": List[WorkloadTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 DescribeProblemObservationsResponseTypeDef = TypedDict(
     "DescribeProblemObservationsResponseTypeDef",
     {
         "RelatedObservations": RelatedObservationsTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `types-aiobotocore-application-insights-2.5.2.post3/types_aiobotocore_application_insights/type_defs.pyi` & `types-aiobotocore-application-insights-2.5.4/types_aiobotocore_application_insights/type_defs.pyi`

 * *Files 20% similar despite different names*

```diff
@@ -2,51 +2,55 @@
 Type annotations for application-insights service type definitions.
 
 [Open documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_application_insights/type_defs/)
 
 Usage::
 
     ```python
-    from types_aiobotocore_application_insights.type_defs import ApplicationComponentTypeDef
+    from types_aiobotocore_application_insights.type_defs import WorkloadConfigurationTypeDef
 
-    data: ApplicationComponentTypeDef = ...
+    data: WorkloadConfigurationTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, List, Sequence, Union
 
 from .literals import (
     CloudWatchEventSourceType,
     ConfigurationEventResourceTypeType,
     ConfigurationEventStatusType,
     DiscoveryTypeType,
     FeedbackValueType,
     LogFilterType,
     OsTypeType,
+    RecommendationTypeType,
+    ResolutionMethodType,
     SeverityLevelType,
     StatusType,
     TierType,
+    VisibilityType,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
+    "WorkloadConfigurationTypeDef",
+    "ResponseMetadataTypeDef",
     "ApplicationComponentTypeDef",
     "ApplicationInfoTypeDef",
     "ConfigurationEventTypeDef",
     "TagTypeDef",
-    "ResponseMetadataTypeDef",
     "CreateComponentRequestRequestTypeDef",
     "CreateLogPatternRequestRequestTypeDef",
     "LogPatternTypeDef",
     "DeleteApplicationRequestRequestTypeDef",
     "DeleteComponentRequestRequestTypeDef",
     "DeleteLogPatternRequestRequestTypeDef",
     "DescribeApplicationRequestRequestTypeDef",
@@ -55,51 +59,83 @@
     "DescribeComponentRequestRequestTypeDef",
     "DescribeLogPatternRequestRequestTypeDef",
     "DescribeObservationRequestRequestTypeDef",
     "ObservationTypeDef",
     "DescribeProblemObservationsRequestRequestTypeDef",
     "DescribeProblemRequestRequestTypeDef",
     "ProblemTypeDef",
+    "DescribeWorkloadRequestRequestTypeDef",
     "ListApplicationsRequestRequestTypeDef",
     "ListComponentsRequestRequestTypeDef",
     "TimestampTypeDef",
     "ListLogPatternSetsRequestRequestTypeDef",
     "ListLogPatternsRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
+    "ListWorkloadsRequestRequestTypeDef",
+    "WorkloadTypeDef",
+    "RemoveWorkloadRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateApplicationRequestRequestTypeDef",
     "UpdateComponentConfigurationRequestRequestTypeDef",
     "UpdateComponentRequestRequestTypeDef",
     "UpdateLogPatternRequestRequestTypeDef",
-    "CreateApplicationRequestRequestTypeDef",
-    "TagResourceRequestRequestTypeDef",
-    "CreateApplicationResponseTypeDef",
-    "DescribeApplicationResponseTypeDef",
+    "UpdateProblemRequestRequestTypeDef",
+    "AddWorkloadRequestRequestTypeDef",
+    "UpdateWorkloadRequestRequestTypeDef",
+    "AddWorkloadResponseTypeDef",
     "DescribeComponentConfigurationRecommendationResponseTypeDef",
     "DescribeComponentConfigurationResponseTypeDef",
+    "DescribeWorkloadResponseTypeDef",
+    "ListLogPatternSetsResponseTypeDef",
+    "UpdateWorkloadResponseTypeDef",
     "DescribeComponentResponseTypeDef",
-    "ListApplicationsResponseTypeDef",
     "ListComponentsResponseTypeDef",
+    "CreateApplicationResponseTypeDef",
+    "DescribeApplicationResponseTypeDef",
+    "ListApplicationsResponseTypeDef",
+    "UpdateApplicationResponseTypeDef",
     "ListConfigurationHistoryResponseTypeDef",
-    "ListLogPatternSetsResponseTypeDef",
+    "CreateApplicationRequestRequestTypeDef",
     "ListTagsForResourceResponseTypeDef",
-    "UpdateApplicationResponseTypeDef",
+    "TagResourceRequestRequestTypeDef",
     "CreateLogPatternResponseTypeDef",
     "DescribeLogPatternResponseTypeDef",
     "ListLogPatternsResponseTypeDef",
     "UpdateLogPatternResponseTypeDef",
     "DescribeObservationResponseTypeDef",
     "RelatedObservationsTypeDef",
     "DescribeProblemResponseTypeDef",
     "ListProblemsResponseTypeDef",
     "ListConfigurationHistoryRequestRequestTypeDef",
     "ListProblemsRequestRequestTypeDef",
+    "ListWorkloadsResponseTypeDef",
     "DescribeProblemObservationsResponseTypeDef",
 )
 
+WorkloadConfigurationTypeDef = TypedDict(
+    "WorkloadConfigurationTypeDef",
+    {
+        "WorkloadName": str,
+        "Tier": TierType,
+        "Configuration": str,
+    },
+    total=False,
+)
+
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
+    {
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
+    },
+)
+
 ApplicationComponentTypeDef = TypedDict(
     "ApplicationComponentTypeDef",
     {
         "ComponentName": str,
         "ComponentRemarks": str,
         "ResourceType": str,
         "OsType": OsTypeType,
@@ -109,14 +145,15 @@
     },
     total=False,
 )
 
 ApplicationInfoTypeDef = TypedDict(
     "ApplicationInfoTypeDef",
     {
+        "AccountId": str,
         "ResourceGroupName": str,
         "LifeCycle": str,
         "OpsItemSNSTopicArn": str,
         "OpsCenterEnabled": bool,
         "CWEMonitorEnabled": bool,
         "Remarks": str,
         "AutoConfigEnabled": bool,
@@ -124,14 +161,16 @@
     },
     total=False,
 )
 
 ConfigurationEventTypeDef = TypedDict(
     "ConfigurationEventTypeDef",
     {
+        "ResourceGroupName": str,
+        "AccountId": str,
         "MonitoredResourceARN": str,
         "EventStatus": ConfigurationEventStatusType,
         "EventResourceType": ConfigurationEventResourceTypeType,
         "EventTime": datetime,
         "EventDetail": str,
         "EventResourceName": str,
     },
@@ -142,25 +181,14 @@
     "TagTypeDef",
     {
         "Key": str,
         "Value": str,
     },
 )
 
-ResponseMetadataTypeDef = TypedDict(
-    "ResponseMetadataTypeDef",
-    {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
-    },
-)
-
 CreateComponentRequestRequestTypeDef = TypedDict(
     "CreateComponentRequestRequestTypeDef",
     {
         "ResourceGroupName": str,
         "ComponentName": str,
         "ResourceList": Sequence[str],
     },
@@ -208,61 +236,138 @@
     {
         "ResourceGroupName": str,
         "PatternSetName": str,
         "PatternName": str,
     },
 )
 
-DescribeApplicationRequestRequestTypeDef = TypedDict(
-    "DescribeApplicationRequestRequestTypeDef",
+_RequiredDescribeApplicationRequestRequestTypeDef = TypedDict(
+    "_RequiredDescribeApplicationRequestRequestTypeDef",
     {
         "ResourceGroupName": str,
     },
 )
+_OptionalDescribeApplicationRequestRequestTypeDef = TypedDict(
+    "_OptionalDescribeApplicationRequestRequestTypeDef",
+    {
+        "AccountId": str,
+    },
+    total=False,
+)
 
-DescribeComponentConfigurationRecommendationRequestRequestTypeDef = TypedDict(
-    "DescribeComponentConfigurationRecommendationRequestRequestTypeDef",
+class DescribeApplicationRequestRequestTypeDef(
+    _RequiredDescribeApplicationRequestRequestTypeDef,
+    _OptionalDescribeApplicationRequestRequestTypeDef,
+):
+    pass
+
+_RequiredDescribeComponentConfigurationRecommendationRequestRequestTypeDef = TypedDict(
+    "_RequiredDescribeComponentConfigurationRecommendationRequestRequestTypeDef",
     {
         "ResourceGroupName": str,
         "ComponentName": str,
         "Tier": TierType,
     },
 )
+_OptionalDescribeComponentConfigurationRecommendationRequestRequestTypeDef = TypedDict(
+    "_OptionalDescribeComponentConfigurationRecommendationRequestRequestTypeDef",
+    {
+        "RecommendationType": RecommendationTypeType,
+    },
+    total=False,
+)
 
-DescribeComponentConfigurationRequestRequestTypeDef = TypedDict(
-    "DescribeComponentConfigurationRequestRequestTypeDef",
+class DescribeComponentConfigurationRecommendationRequestRequestTypeDef(
+    _RequiredDescribeComponentConfigurationRecommendationRequestRequestTypeDef,
+    _OptionalDescribeComponentConfigurationRecommendationRequestRequestTypeDef,
+):
+    pass
+
+_RequiredDescribeComponentConfigurationRequestRequestTypeDef = TypedDict(
+    "_RequiredDescribeComponentConfigurationRequestRequestTypeDef",
     {
         "ResourceGroupName": str,
         "ComponentName": str,
     },
 )
+_OptionalDescribeComponentConfigurationRequestRequestTypeDef = TypedDict(
+    "_OptionalDescribeComponentConfigurationRequestRequestTypeDef",
+    {
+        "AccountId": str,
+    },
+    total=False,
+)
 
-DescribeComponentRequestRequestTypeDef = TypedDict(
-    "DescribeComponentRequestRequestTypeDef",
+class DescribeComponentConfigurationRequestRequestTypeDef(
+    _RequiredDescribeComponentConfigurationRequestRequestTypeDef,
+    _OptionalDescribeComponentConfigurationRequestRequestTypeDef,
+):
+    pass
+
+_RequiredDescribeComponentRequestRequestTypeDef = TypedDict(
+    "_RequiredDescribeComponentRequestRequestTypeDef",
     {
         "ResourceGroupName": str,
         "ComponentName": str,
     },
 )
+_OptionalDescribeComponentRequestRequestTypeDef = TypedDict(
+    "_OptionalDescribeComponentRequestRequestTypeDef",
+    {
+        "AccountId": str,
+    },
+    total=False,
+)
 
-DescribeLogPatternRequestRequestTypeDef = TypedDict(
-    "DescribeLogPatternRequestRequestTypeDef",
+class DescribeComponentRequestRequestTypeDef(
+    _RequiredDescribeComponentRequestRequestTypeDef, _OptionalDescribeComponentRequestRequestTypeDef
+):
+    pass
+
+_RequiredDescribeLogPatternRequestRequestTypeDef = TypedDict(
+    "_RequiredDescribeLogPatternRequestRequestTypeDef",
     {
         "ResourceGroupName": str,
         "PatternSetName": str,
         "PatternName": str,
     },
 )
+_OptionalDescribeLogPatternRequestRequestTypeDef = TypedDict(
+    "_OptionalDescribeLogPatternRequestRequestTypeDef",
+    {
+        "AccountId": str,
+    },
+    total=False,
+)
 
-DescribeObservationRequestRequestTypeDef = TypedDict(
-    "DescribeObservationRequestRequestTypeDef",
+class DescribeLogPatternRequestRequestTypeDef(
+    _RequiredDescribeLogPatternRequestRequestTypeDef,
+    _OptionalDescribeLogPatternRequestRequestTypeDef,
+):
+    pass
+
+_RequiredDescribeObservationRequestRequestTypeDef = TypedDict(
+    "_RequiredDescribeObservationRequestRequestTypeDef",
     {
         "ObservationId": str,
     },
 )
+_OptionalDescribeObservationRequestRequestTypeDef = TypedDict(
+    "_OptionalDescribeObservationRequestRequestTypeDef",
+    {
+        "AccountId": str,
+    },
+    total=False,
+)
+
+class DescribeObservationRequestRequestTypeDef(
+    _RequiredDescribeObservationRequestRequestTypeDef,
+    _OptionalDescribeObservationRequestRequestTypeDef,
+):
+    pass
 
 ObservationTypeDef = TypedDict(
     "ObservationTypeDef",
     {
         "Id": str,
         "StartTime": datetime,
         "EndTime": datetime,
@@ -308,52 +413,102 @@
         "XRayRequestAverageLatency": int,
         "XRayNodeName": str,
         "XRayNodeType": str,
     },
     total=False,
 )
 
-DescribeProblemObservationsRequestRequestTypeDef = TypedDict(
-    "DescribeProblemObservationsRequestRequestTypeDef",
+_RequiredDescribeProblemObservationsRequestRequestTypeDef = TypedDict(
+    "_RequiredDescribeProblemObservationsRequestRequestTypeDef",
     {
         "ProblemId": str,
     },
 )
+_OptionalDescribeProblemObservationsRequestRequestTypeDef = TypedDict(
+    "_OptionalDescribeProblemObservationsRequestRequestTypeDef",
+    {
+        "AccountId": str,
+    },
+    total=False,
+)
 
-DescribeProblemRequestRequestTypeDef = TypedDict(
-    "DescribeProblemRequestRequestTypeDef",
+class DescribeProblemObservationsRequestRequestTypeDef(
+    _RequiredDescribeProblemObservationsRequestRequestTypeDef,
+    _OptionalDescribeProblemObservationsRequestRequestTypeDef,
+):
+    pass
+
+_RequiredDescribeProblemRequestRequestTypeDef = TypedDict(
+    "_RequiredDescribeProblemRequestRequestTypeDef",
     {
         "ProblemId": str,
     },
 )
+_OptionalDescribeProblemRequestRequestTypeDef = TypedDict(
+    "_OptionalDescribeProblemRequestRequestTypeDef",
+    {
+        "AccountId": str,
+    },
+    total=False,
+)
+
+class DescribeProblemRequestRequestTypeDef(
+    _RequiredDescribeProblemRequestRequestTypeDef, _OptionalDescribeProblemRequestRequestTypeDef
+):
+    pass
 
 ProblemTypeDef = TypedDict(
     "ProblemTypeDef",
     {
         "Id": str,
         "Title": str,
         "Insights": str,
         "Status": StatusType,
         "AffectedResource": str,
         "StartTime": datetime,
         "EndTime": datetime,
         "SeverityLevel": SeverityLevelType,
+        "AccountId": str,
         "ResourceGroupName": str,
         "Feedback": Dict[Literal["INSIGHTS_FEEDBACK"], FeedbackValueType],
         "RecurringCount": int,
         "LastRecurrenceTime": datetime,
+        "Visibility": VisibilityType,
+        "ResolutionMethod": ResolutionMethodType,
+    },
+    total=False,
+)
+
+_RequiredDescribeWorkloadRequestRequestTypeDef = TypedDict(
+    "_RequiredDescribeWorkloadRequestRequestTypeDef",
+    {
+        "ResourceGroupName": str,
+        "ComponentName": str,
+        "WorkloadId": str,
+    },
+)
+_OptionalDescribeWorkloadRequestRequestTypeDef = TypedDict(
+    "_OptionalDescribeWorkloadRequestRequestTypeDef",
+    {
+        "AccountId": str,
     },
     total=False,
 )
 
+class DescribeWorkloadRequestRequestTypeDef(
+    _RequiredDescribeWorkloadRequestRequestTypeDef, _OptionalDescribeWorkloadRequestRequestTypeDef
+):
+    pass
+
 ListApplicationsRequestRequestTypeDef = TypedDict(
     "ListApplicationsRequestRequestTypeDef",
     {
         "MaxResults": int,
         "NextToken": str,
+        "AccountId": str,
     },
     total=False,
 )
 
 _RequiredListComponentsRequestRequestTypeDef = TypedDict(
     "_RequiredListComponentsRequestRequestTypeDef",
     {
@@ -361,14 +516,15 @@
     },
 )
 _OptionalListComponentsRequestRequestTypeDef = TypedDict(
     "_OptionalListComponentsRequestRequestTypeDef",
     {
         "MaxResults": int,
         "NextToken": str,
+        "AccountId": str,
     },
     total=False,
 )
 
 class ListComponentsRequestRequestTypeDef(
     _RequiredListComponentsRequestRequestTypeDef, _OptionalListComponentsRequestRequestTypeDef
 ):
@@ -382,14 +538,15 @@
     },
 )
 _OptionalListLogPatternSetsRequestRequestTypeDef = TypedDict(
     "_OptionalListLogPatternSetsRequestRequestTypeDef",
     {
         "MaxResults": int,
         "NextToken": str,
+        "AccountId": str,
     },
     total=False,
 )
 
 class ListLogPatternSetsRequestRequestTypeDef(
     _RequiredListLogPatternSetsRequestRequestTypeDef,
     _OptionalListLogPatternSetsRequestRequestTypeDef,
@@ -404,14 +561,15 @@
 )
 _OptionalListLogPatternsRequestRequestTypeDef = TypedDict(
     "_OptionalListLogPatternsRequestRequestTypeDef",
     {
         "PatternSetName": str,
         "MaxResults": int,
         "NextToken": str,
+        "AccountId": str,
     },
     total=False,
 )
 
 class ListLogPatternsRequestRequestTypeDef(
     _RequiredListLogPatternsRequestRequestTypeDef, _OptionalListLogPatternsRequestRequestTypeDef
 ):
@@ -420,14 +578,57 @@
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "ResourceARN": str,
     },
 )
 
+_RequiredListWorkloadsRequestRequestTypeDef = TypedDict(
+    "_RequiredListWorkloadsRequestRequestTypeDef",
+    {
+        "ResourceGroupName": str,
+        "ComponentName": str,
+    },
+)
+_OptionalListWorkloadsRequestRequestTypeDef = TypedDict(
+    "_OptionalListWorkloadsRequestRequestTypeDef",
+    {
+        "MaxResults": int,
+        "NextToken": str,
+        "AccountId": str,
+    },
+    total=False,
+)
+
+class ListWorkloadsRequestRequestTypeDef(
+    _RequiredListWorkloadsRequestRequestTypeDef, _OptionalListWorkloadsRequestRequestTypeDef
+):
+    pass
+
+WorkloadTypeDef = TypedDict(
+    "WorkloadTypeDef",
+    {
+        "WorkloadId": str,
+        "ComponentName": str,
+        "WorkloadName": str,
+        "Tier": TierType,
+        "WorkloadRemarks": str,
+    },
+    total=False,
+)
+
+RemoveWorkloadRequestRequestTypeDef = TypedDict(
+    "RemoveWorkloadRequestRequestTypeDef",
+    {
+        "ResourceGroupName": str,
+        "ComponentName": str,
+        "WorkloadId": str,
+    },
+)
+
 UntagResourceRequestRequestTypeDef = TypedDict(
     "UntagResourceRequestRequestTypeDef",
     {
         "ResourceARN": str,
         "TagKeys": Sequence[str],
     },
 )
@@ -518,49 +719,69 @@
 )
 
 class UpdateLogPatternRequestRequestTypeDef(
     _RequiredUpdateLogPatternRequestRequestTypeDef, _OptionalUpdateLogPatternRequestRequestTypeDef
 ):
     pass
 
-CreateApplicationRequestRequestTypeDef = TypedDict(
-    "CreateApplicationRequestRequestTypeDef",
+_RequiredUpdateProblemRequestRequestTypeDef = TypedDict(
+    "_RequiredUpdateProblemRequestRequestTypeDef",
     {
-        "ResourceGroupName": str,
-        "OpsCenterEnabled": bool,
-        "CWEMonitorEnabled": bool,
-        "OpsItemSNSTopicArn": str,
-        "Tags": Sequence[TagTypeDef],
-        "AutoConfigEnabled": bool,
-        "AutoCreate": bool,
-        "GroupingType": Literal["ACCOUNT_BASED"],
+        "ProblemId": str,
+    },
+)
+_OptionalUpdateProblemRequestRequestTypeDef = TypedDict(
+    "_OptionalUpdateProblemRequestRequestTypeDef",
+    {
+        "UpdateStatus": Literal["RESOLVED"],
+        "Visibility": VisibilityType,
     },
     total=False,
 )
 
-TagResourceRequestRequestTypeDef = TypedDict(
-    "TagResourceRequestRequestTypeDef",
+class UpdateProblemRequestRequestTypeDef(
+    _RequiredUpdateProblemRequestRequestTypeDef, _OptionalUpdateProblemRequestRequestTypeDef
+):
+    pass
+
+AddWorkloadRequestRequestTypeDef = TypedDict(
+    "AddWorkloadRequestRequestTypeDef",
     {
-        "ResourceARN": str,
-        "Tags": Sequence[TagTypeDef],
+        "ResourceGroupName": str,
+        "ComponentName": str,
+        "WorkloadConfiguration": WorkloadConfigurationTypeDef,
     },
 )
 
-CreateApplicationResponseTypeDef = TypedDict(
-    "CreateApplicationResponseTypeDef",
+_RequiredUpdateWorkloadRequestRequestTypeDef = TypedDict(
+    "_RequiredUpdateWorkloadRequestRequestTypeDef",
     {
-        "ApplicationInfo": ApplicationInfoTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResourceGroupName": str,
+        "ComponentName": str,
+        "WorkloadConfiguration": WorkloadConfigurationTypeDef,
+    },
+)
+_OptionalUpdateWorkloadRequestRequestTypeDef = TypedDict(
+    "_OptionalUpdateWorkloadRequestRequestTypeDef",
+    {
+        "WorkloadId": str,
     },
+    total=False,
 )
 
-DescribeApplicationResponseTypeDef = TypedDict(
-    "DescribeApplicationResponseTypeDef",
+class UpdateWorkloadRequestRequestTypeDef(
+    _RequiredUpdateWorkloadRequestRequestTypeDef, _OptionalUpdateWorkloadRequestRequestTypeDef
+):
+    pass
+
+AddWorkloadResponseTypeDef = TypedDict(
+    "AddWorkloadResponseTypeDef",
     {
-        "ApplicationInfo": ApplicationInfoTypeDef,
+        "WorkloadId": str,
+        "WorkloadConfiguration": WorkloadConfigurationTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeComponentConfigurationRecommendationResponseTypeDef = TypedDict(
     "DescribeComponentConfigurationRecommendationResponseTypeDef",
     {
@@ -575,73 +796,132 @@
         "Monitor": bool,
         "Tier": TierType,
         "ComponentConfiguration": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+DescribeWorkloadResponseTypeDef = TypedDict(
+    "DescribeWorkloadResponseTypeDef",
+    {
+        "WorkloadId": str,
+        "WorkloadRemarks": str,
+        "WorkloadConfiguration": WorkloadConfigurationTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListLogPatternSetsResponseTypeDef = TypedDict(
+    "ListLogPatternSetsResponseTypeDef",
+    {
+        "ResourceGroupName": str,
+        "AccountId": str,
+        "LogPatternSets": List[str],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateWorkloadResponseTypeDef = TypedDict(
+    "UpdateWorkloadResponseTypeDef",
+    {
+        "WorkloadId": str,
+        "WorkloadConfiguration": WorkloadConfigurationTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 DescribeComponentResponseTypeDef = TypedDict(
     "DescribeComponentResponseTypeDef",
     {
         "ApplicationComponent": ApplicationComponentTypeDef,
         "ResourceList": List[str],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+ListComponentsResponseTypeDef = TypedDict(
+    "ListComponentsResponseTypeDef",
+    {
+        "ApplicationComponentList": List[ApplicationComponentTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateApplicationResponseTypeDef = TypedDict(
+    "CreateApplicationResponseTypeDef",
+    {
+        "ApplicationInfo": ApplicationInfoTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeApplicationResponseTypeDef = TypedDict(
+    "DescribeApplicationResponseTypeDef",
+    {
+        "ApplicationInfo": ApplicationInfoTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 ListApplicationsResponseTypeDef = TypedDict(
     "ListApplicationsResponseTypeDef",
     {
         "ApplicationInfoList": List[ApplicationInfoTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-ListComponentsResponseTypeDef = TypedDict(
-    "ListComponentsResponseTypeDef",
+UpdateApplicationResponseTypeDef = TypedDict(
+    "UpdateApplicationResponseTypeDef",
     {
-        "ApplicationComponentList": List[ApplicationComponentTypeDef],
-        "NextToken": str,
+        "ApplicationInfo": ApplicationInfoTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListConfigurationHistoryResponseTypeDef = TypedDict(
     "ListConfigurationHistoryResponseTypeDef",
     {
         "EventList": List[ConfigurationEventTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-ListLogPatternSetsResponseTypeDef = TypedDict(
-    "ListLogPatternSetsResponseTypeDef",
+CreateApplicationRequestRequestTypeDef = TypedDict(
+    "CreateApplicationRequestRequestTypeDef",
     {
         "ResourceGroupName": str,
-        "LogPatternSets": List[str],
-        "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "OpsCenterEnabled": bool,
+        "CWEMonitorEnabled": bool,
+        "OpsItemSNSTopicArn": str,
+        "Tags": Sequence[TagTypeDef],
+        "AutoConfigEnabled": bool,
+        "AutoCreate": bool,
+        "GroupingType": Literal["ACCOUNT_BASED"],
     },
+    total=False,
 )
 
 ListTagsForResourceResponseTypeDef = TypedDict(
     "ListTagsForResourceResponseTypeDef",
     {
         "Tags": List[TagTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-UpdateApplicationResponseTypeDef = TypedDict(
-    "UpdateApplicationResponseTypeDef",
+TagResourceRequestRequestTypeDef = TypedDict(
+    "TagResourceRequestRequestTypeDef",
     {
-        "ApplicationInfo": ApplicationInfoTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResourceARN": str,
+        "Tags": Sequence[TagTypeDef],
     },
 )
 
 CreateLogPatternResponseTypeDef = TypedDict(
     "CreateLogPatternResponseTypeDef",
     {
         "LogPattern": LogPatternTypeDef,
@@ -650,23 +930,25 @@
     },
 )
 
 DescribeLogPatternResponseTypeDef = TypedDict(
     "DescribeLogPatternResponseTypeDef",
     {
         "ResourceGroupName": str,
+        "AccountId": str,
         "LogPattern": LogPatternTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListLogPatternsResponseTypeDef = TypedDict(
     "ListLogPatternsResponseTypeDef",
     {
         "ResourceGroupName": str,
+        "AccountId": str,
         "LogPatterns": List[LogPatternTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateLogPatternResponseTypeDef = TypedDict(
@@ -704,44 +986,57 @@
 
 ListProblemsResponseTypeDef = TypedDict(
     "ListProblemsResponseTypeDef",
     {
         "ProblemList": List[ProblemTypeDef],
         "NextToken": str,
         "ResourceGroupName": str,
+        "AccountId": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListConfigurationHistoryRequestRequestTypeDef = TypedDict(
     "ListConfigurationHistoryRequestRequestTypeDef",
     {
         "ResourceGroupName": str,
         "StartTime": TimestampTypeDef,
         "EndTime": TimestampTypeDef,
         "EventStatus": ConfigurationEventStatusType,
         "MaxResults": int,
         "NextToken": str,
+        "AccountId": str,
     },
     total=False,
 )
 
 ListProblemsRequestRequestTypeDef = TypedDict(
     "ListProblemsRequestRequestTypeDef",
     {
+        "AccountId": str,
         "ResourceGroupName": str,
         "StartTime": TimestampTypeDef,
         "EndTime": TimestampTypeDef,
         "MaxResults": int,
         "NextToken": str,
         "ComponentName": str,
+        "Visibility": VisibilityType,
     },
     total=False,
 )
 
+ListWorkloadsResponseTypeDef = TypedDict(
+    "ListWorkloadsResponseTypeDef",
+    {
+        "WorkloadList": List[WorkloadTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 DescribeProblemObservationsResponseTypeDef = TypedDict(
     "DescribeProblemObservationsResponseTypeDef",
     {
         "RelatedObservations": RelatedObservationsTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `types-aiobotocore-application-insights-2.5.2.post3/types_aiobotocore_application_insights.egg-info/PKG-INFO` & `types-aiobotocore-application-insights-2.5.4/types_aiobotocore_application_insights.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-application-insights
-Version: 2.5.2.post3
-Summary: Type annotations for aiobotocore.ApplicationInsights 2.5.2 service generated with mypy-boto3-builder 7.17.2
+Version: 2.5.4
+Summary: Type annotations for aiobotocore.ApplicationInsights 2.5.4 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_application_insights/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-application-insights.svg?color=blue)](https://pypi.org/project/types-aiobotocore-application-insights)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_application_insights/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-application-insights)](https://pepy.tech/project/types-aiobotocore-application-insights)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.ApplicationInsights 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/application-insights.html#ApplicationInsights)
+[aiobotocore.ApplicationInsights 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/application-insights.html#ApplicationInsights)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
@@ -289,18 +289,18 @@
 and shapes assembled to typed dictionaries and unions for additional type
 checking.
 
 Full list of `ApplicationInsights` TypeDefs can be found in
 [docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_application_insights/type_defs/).
 
 ```python
-from types_aiobotocore_application_insights.type_defs import ApplicationComponentTypeDef
+from types_aiobotocore_application_insights.type_defs import WorkloadConfigurationTypeDef
 
 
-def get_value() -> ApplicationComponentTypeDef:
+def get_value() -> WorkloadConfigurationTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-application-insights-2.5.2.post3/types_aiobotocore_application_insights.egg-info/SOURCES.txt` & `types-aiobotocore-application-insights-2.5.4/types_aiobotocore_application_insights.egg-info/SOURCES.txt`

 * *Files identical despite different names*


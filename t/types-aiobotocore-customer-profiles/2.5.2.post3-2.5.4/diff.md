# Comparing `tmp/types-aiobotocore-customer-profiles-2.5.2.post3.tar.gz` & `tmp/types-aiobotocore-customer-profiles-2.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-customer-profiles-2.5.2.post3.tar", last modified: Fri Aug  4 12:37:34 2023, max compression
+gzip compressed data, was "types-aiobotocore-customer-profiles-2.5.4.tar", last modified: Tue Aug  8 01:23:33 2023, max compression
```

## Comparing `types-aiobotocore-customer-profiles-2.5.2.post3.tar` & `types-aiobotocore-customer-profiles-2.5.4.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:37:34.099585 types-aiobotocore-customer-profiles-2.5.2.post3/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-04 12:21:04.000000 types-aiobotocore-customer-profiles-2.5.2.post3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    13544 2023-08-04 12:37:34.091585 types-aiobotocore-customer-profiles-2.5.2.post3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    11987 2023-08-04 12:21:04.000000 types-aiobotocore-customer-profiles-2.5.2.post3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-04 12:37:34.099585 types-aiobotocore-customer-profiles-2.5.2.post3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2141 2023-08-04 12:21:04.000000 types-aiobotocore-customer-profiles-2.5.2.post3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:37:34.087585 types-aiobotocore-customer-profiles-2.5.2.post3/types_aiobotocore_customer_profiles/
--rw-r--r--   0 runner    (1001) docker     (123)      736 2023-08-04 12:21:04.000000 types-aiobotocore-customer-profiles-2.5.2.post3/types_aiobotocore_customer_profiles/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      735 2023-08-04 12:21:04.000000 types-aiobotocore-customer-profiles-2.5.2.post3/types_aiobotocore_customer_profiles/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      981 2023-08-04 12:21:04.000000 types-aiobotocore-customer-profiles-2.5.2.post3/types_aiobotocore_customer_profiles/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    41017 2023-08-04 12:21:04.000000 types-aiobotocore-customer-profiles-2.5.2.post3/types_aiobotocore_customer_profiles/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    40958 2023-08-04 12:21:04.000000 types-aiobotocore-customer-profiles-2.5.2.post3/types_aiobotocore_customer_profiles/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    12679 2023-08-04 12:21:04.000000 types-aiobotocore-customer-profiles-2.5.2.post3/types_aiobotocore_customer_profiles/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    12677 2023-08-04 12:21:04.000000 types-aiobotocore-customer-profiles-2.5.2.post3/types_aiobotocore_customer_profiles/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2148 2023-08-04 12:21:04.000000 types-aiobotocore-customer-profiles-2.5.2.post3/types_aiobotocore_customer_profiles/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     2145 2023-08-04 12:21:04.000000 types-aiobotocore-customer-profiles-2.5.2.post3/types_aiobotocore_customer_profiles/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 12:21:04.000000 types-aiobotocore-customer-profiles-2.5.2.post3/types_aiobotocore_customer_profiles/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    62983 2023-08-04 12:21:07.000000 types-aiobotocore-customer-profiles-2.5.2.post3/types_aiobotocore_customer_profiles/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    62895 2023-08-04 12:21:05.000000 types-aiobotocore-customer-profiles-2.5.2.post3/types_aiobotocore_customer_profiles/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-04 12:21:04.000000 types-aiobotocore-customer-profiles-2.5.2.post3/types_aiobotocore_customer_profiles/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:37:34.091585 types-aiobotocore-customer-profiles-2.5.2.post3/types_aiobotocore_customer_profiles.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    13544 2023-08-04 12:37:33.000000 types-aiobotocore-customer-profiles-2.5.2.post3/types_aiobotocore_customer_profiles.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1003 2023-08-04 12:37:33.000000 types-aiobotocore-customer-profiles-2.5.2.post3/types_aiobotocore_customer_profiles.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 12:37:33.000000 types-aiobotocore-customer-profiles-2.5.2.post3/types_aiobotocore_customer_profiles.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 12:37:33.000000 types-aiobotocore-customer-profiles-2.5.2.post3/types_aiobotocore_customer_profiles.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-04 12:37:33.000000 types-aiobotocore-customer-profiles-2.5.2.post3/types_aiobotocore_customer_profiles.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-08-04 12:37:33.000000 types-aiobotocore-customer-profiles-2.5.2.post3/types_aiobotocore_customer_profiles.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:23:33.818677 types-aiobotocore-customer-profiles-2.5.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-08 01:08:41.000000 types-aiobotocore-customer-profiles-2.5.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    13538 2023-08-08 01:23:33.814677 types-aiobotocore-customer-profiles-2.5.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    11987 2023-08-08 01:08:41.000000 types-aiobotocore-customer-profiles-2.5.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-08 01:23:33.818677 types-aiobotocore-customer-profiles-2.5.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2135 2023-08-08 01:08:41.000000 types-aiobotocore-customer-profiles-2.5.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:23:33.814677 types-aiobotocore-customer-profiles-2.5.4/types_aiobotocore_customer_profiles/
+-rw-r--r--   0 runner    (1001) docker     (123)      736 2023-08-08 01:08:41.000000 types-aiobotocore-customer-profiles-2.5.4/types_aiobotocore_customer_profiles/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      735 2023-08-08 01:08:41.000000 types-aiobotocore-customer-profiles-2.5.4/types_aiobotocore_customer_profiles/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      969 2023-08-08 01:08:41.000000 types-aiobotocore-customer-profiles-2.5.4/types_aiobotocore_customer_profiles/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42673 2023-08-08 01:08:41.000000 types-aiobotocore-customer-profiles-2.5.4/types_aiobotocore_customer_profiles/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42612 2023-08-08 01:08:41.000000 types-aiobotocore-customer-profiles-2.5.4/types_aiobotocore_customer_profiles/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    13078 2023-08-08 01:08:41.000000 types-aiobotocore-customer-profiles-2.5.4/types_aiobotocore_customer_profiles/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13076 2023-08-08 01:08:41.000000 types-aiobotocore-customer-profiles-2.5.4/types_aiobotocore_customer_profiles/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2148 2023-08-08 01:08:41.000000 types-aiobotocore-customer-profiles-2.5.4/types_aiobotocore_customer_profiles/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2145 2023-08-08 01:08:41.000000 types-aiobotocore-customer-profiles-2.5.4/types_aiobotocore_customer_profiles/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 01:08:41.000000 types-aiobotocore-customer-profiles-2.5.4/types_aiobotocore_customer_profiles/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    67337 2023-08-08 01:08:43.000000 types-aiobotocore-customer-profiles-2.5.4/types_aiobotocore_customer_profiles/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    67241 2023-08-08 01:08:42.000000 types-aiobotocore-customer-profiles-2.5.4/types_aiobotocore_customer_profiles/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-08-08 01:08:41.000000 types-aiobotocore-customer-profiles-2.5.4/types_aiobotocore_customer_profiles/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:23:33.814677 types-aiobotocore-customer-profiles-2.5.4/types_aiobotocore_customer_profiles.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    13538 2023-08-08 01:23:33.000000 types-aiobotocore-customer-profiles-2.5.4/types_aiobotocore_customer_profiles.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1003 2023-08-08 01:23:33.000000 types-aiobotocore-customer-profiles-2.5.4/types_aiobotocore_customer_profiles.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 01:23:33.000000 types-aiobotocore-customer-profiles-2.5.4/types_aiobotocore_customer_profiles.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 01:23:33.000000 types-aiobotocore-customer-profiles-2.5.4/types_aiobotocore_customer_profiles.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-08 01:23:33.000000 types-aiobotocore-customer-profiles-2.5.4/types_aiobotocore_customer_profiles.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-08-08 01:23:33.000000 types-aiobotocore-customer-profiles-2.5.4/types_aiobotocore_customer_profiles.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-customer-profiles-2.5.2.post3/LICENSE` & `types-aiobotocore-customer-profiles-2.5.4/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-customer-profiles-2.5.2.post3/PKG-INFO` & `types-aiobotocore-customer-profiles-2.5.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-customer-profiles
-Version: 2.5.2.post3
-Summary: Type annotations for aiobotocore.CustomerProfiles 2.5.2 service generated with mypy-boto3-builder 7.17.2
+Version: 2.5.4
+Summary: Type annotations for aiobotocore.CustomerProfiles 2.5.4 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_customer_profiles/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-customer-profiles.svg?color=blue)](https://pypi.org/project/types-aiobotocore-customer-profiles)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_customer_profiles/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-customer-profiles)](https://pepy.tech/project/types-aiobotocore-customer-profiles)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.CustomerProfiles 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/customer-profiles.html#CustomerProfiles)
+[aiobotocore.CustomerProfiles 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/customer-profiles.html#CustomerProfiles)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
@@ -295,18 +295,18 @@
 `types_aiobotocore_customer_profiles.literals` module contains literals
 extracted from shapes that can be used in user code for type checking.
 
 Full list of `CustomerProfiles` Literals can be found in
 [docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_customer_profiles/literals/).
 
 ```python
-from types_aiobotocore_customer_profiles.literals import ConflictResolvingModelType
+from types_aiobotocore_customer_profiles.literals import AttributeMatchingModelType
 
 
-def check_value(value: ConflictResolvingModelType) -> bool:
+def check_value(value: AttributeMatchingModelType) -> bool:
     ...
 ```
 
 <a id="type-definitions"></a>
 
 ### Type definitions
```

### Comparing `types-aiobotocore-customer-profiles-2.5.2.post3/README.md` & `types-aiobotocore-customer-profiles-2.5.4/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-customer-profiles.svg?color=blue)](https://pypi.org/project/types-aiobotocore-customer-profiles)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_customer_profiles/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-customer-profiles)](https://pepy.tech/project/types-aiobotocore-customer-profiles)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.CustomerProfiles 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/customer-profiles.html#CustomerProfiles)
+[aiobotocore.CustomerProfiles 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/customer-profiles.html#CustomerProfiles)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
@@ -263,18 +263,18 @@
 `types_aiobotocore_customer_profiles.literals` module contains literals
 extracted from shapes that can be used in user code for type checking.
 
 Full list of `CustomerProfiles` Literals can be found in
 [docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_customer_profiles/literals/).
 
 ```python
-from types_aiobotocore_customer_profiles.literals import ConflictResolvingModelType
+from types_aiobotocore_customer_profiles.literals import AttributeMatchingModelType
 
 
-def check_value(value: ConflictResolvingModelType) -> bool:
+def check_value(value: AttributeMatchingModelType) -> bool:
     ...
 ```
 
 <a id="type-definitions"></a>
 
 ### Type definitions
```

### Comparing `types-aiobotocore-customer-profiles-2.5.2.post3/setup.py` & `types-aiobotocore-customer-profiles-2.5.4/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-customer-profiles",
-    version="2.5.2.post3",
+    version="2.5.4",
     packages=["types_aiobotocore_customer_profiles"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.CustomerProfiles 2.5.2 service generated with"
+        "Type annotations for aiobotocore.CustomerProfiles 2.5.4 service generated with"
         " mypy-boto3-builder 7.17.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
```

### Comparing `types-aiobotocore-customer-profiles-2.5.2.post3/types_aiobotocore_customer_profiles/__init__.py` & `types-aiobotocore-customer-profiles-2.5.4/types_aiobotocore_customer_profiles/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-customer-profiles-2.5.2.post3/types_aiobotocore_customer_profiles/__init__.pyi` & `types-aiobotocore-customer-profiles-2.5.4/types_aiobotocore_customer_profiles/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-customer-profiles-2.5.2.post3/types_aiobotocore_customer_profiles/__main__.py` & `types-aiobotocore-customer-profiles-2.5.4/types_aiobotocore_customer_profiles/__main__.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.CustomerProfiles 2.5.2\nVersion:        "
-        " 2.5.2.post3\nBuilder version: 7.17.2\nDocs:           "
+        "Type annotations for aiobotocore.CustomerProfiles 2.5.4\nVersion:         2.5.4\nBuilder"
+        " version: 7.17.2\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_customer_profiles//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/customer-profiles.html#CustomerProfiles\nOther"
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

### Comparing `types-aiobotocore-customer-profiles-2.5.2.post3/types_aiobotocore_customer_profiles/client.py` & `types-aiobotocore-customer-profiles-2.5.4/types_aiobotocore_customer_profiles/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,22 @@
 """
 import sys
 from typing import Any, Dict, Mapping, Sequence, Type
 
 from aiobotocore.client import AioBaseClient
 from botocore.client import ClientMeta
 
-from .literals import GenderType, PartyTypeType, StatisticType, StatusType, logicalOperatorType
+from .literals import (
+    GenderType,
+    MatchTypeType,
+    PartyTypeType,
+    StatisticType,
+    StatusType,
+    logicalOperatorType,
+)
 from .paginator import ListEventStreamsPaginator
 from .type_defs import (
     AdditionalSearchKeyTypeDef,
     AddProfileKeyResponseTypeDef,
     AddressTypeDef,
     AttributeDetailsTypeDef,
     ConditionsTypeDef,
@@ -49,37 +56,40 @@
     GetDomainResponseTypeDef,
     GetEventStreamResponseTypeDef,
     GetIdentityResolutionJobResponseTypeDef,
     GetIntegrationResponseTypeDef,
     GetMatchesResponseTypeDef,
     GetProfileObjectTypeResponseTypeDef,
     GetProfileObjectTypeTemplateResponseTypeDef,
+    GetSimilarProfilesResponseTypeDef,
     GetWorkflowResponseTypeDef,
     GetWorkflowStepsResponseTypeDef,
     IntegrationConfigTypeDef,
     ListAccountIntegrationsResponseTypeDef,
     ListCalculatedAttributeDefinitionsResponseTypeDef,
     ListCalculatedAttributesForProfileResponseTypeDef,
     ListDomainsResponseTypeDef,
     ListEventStreamsResponseTypeDef,
     ListIdentityResolutionJobsResponseTypeDef,
     ListIntegrationsResponseTypeDef,
     ListProfileObjectsResponseTypeDef,
     ListProfileObjectTypesResponseTypeDef,
     ListProfileObjectTypeTemplatesResponseTypeDef,
+    ListRuleBasedMatchesResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     ListWorkflowsResponseTypeDef,
     MatchingRequestTypeDef,
     MergeProfilesResponseTypeDef,
     ObjectFilterTypeDef,
     ObjectTypeFieldTypeDef,
     ObjectTypeKeyTypeDef,
     PutIntegrationResponseTypeDef,
     PutProfileObjectResponseTypeDef,
     PutProfileObjectTypeResponseTypeDef,
+    RuleBasedMatchingRequestTypeDef,
     SearchProfilesResponseTypeDef,
     TimestampTypeDef,
     UpdateAddressTypeDef,
     UpdateCalculatedAttributeDefinitionResponseTypeDef,
     UpdateDomainResponseTypeDef,
     UpdateProfileResponseTypeDef,
 )
@@ -177,14 +187,15 @@
         self,
         *,
         DomainName: str,
         DefaultExpirationDays: int,
         DefaultEncryptionKey: str = ...,
         DeadLetterQueueUrl: str = ...,
         Matching: MatchingRequestTypeDef = ...,
+        RuleBasedMatching: RuleBasedMatchingRequestTypeDef = ...,
         Tags: Mapping[str, str] = ...
     ) -> CreateDomainResponseTypeDef:
         """
         Creates a domain, which is a container for all customer data, such as customer
         profile attributes, object types, profile keys, and encryption keys.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/customer-profiles.html#CustomerProfiles.Client.create_domain)
@@ -457,14 +468,32 @@
         """
         Returns the template information for a specific object type.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/customer-profiles.html#CustomerProfiles.Client.get_profile_object_type_template)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_customer_profiles/client/#get_profile_object_type_template)
         """
 
+    async def get_similar_profiles(
+        self,
+        *,
+        DomainName: str,
+        MatchType: MatchTypeType,
+        SearchKey: str,
+        SearchValue: str,
+        NextToken: str = ...,
+        MaxResults: int = ...
+    ) -> GetSimilarProfilesResponseTypeDef:
+        """
+        Returns a set of profiles that belong to the same matching group using the
+        `matchId` or `profileId`.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/customer-profiles.html#CustomerProfiles.Client.get_similar_profiles)
+        [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_customer_profiles/client/#get_similar_profiles)
+        """
+
     async def get_workflow(self, *, DomainName: str, WorkflowId: str) -> GetWorkflowResponseTypeDef:
         """
         Get details of specified workflow.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/customer-profiles.html#CustomerProfiles.Client.get_workflow)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_customer_profiles/client/#get_workflow)
         """
@@ -590,14 +619,24 @@
         Returns a list of objects associated with a profile of a given
         ProfileObjectType.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/customer-profiles.html#CustomerProfiles.Client.list_profile_objects)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_customer_profiles/client/#list_profile_objects)
         """
 
+    async def list_rule_based_matches(
+        self, *, DomainName: str, NextToken: str = ..., MaxResults: int = ...
+    ) -> ListRuleBasedMatchesResponseTypeDef:
+        """
+        Returns a set of `MatchIds` that belong to the given domain.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/customer-profiles.html#CustomerProfiles.Client.list_rule_based_matches)
+        [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_customer_profiles/client/#list_rule_based_matches)
+        """
+
     async def list_tags_for_resource(
         self, *, resourceArn: str
     ) -> ListTagsForResourceResponseTypeDef:
         """
         Displays the tags associated with an Amazon Connect Customer Profiles resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/customer-profiles.html#CustomerProfiles.Client.list_tags_for_resource)
@@ -746,14 +785,15 @@
         self,
         *,
         DomainName: str,
         DefaultExpirationDays: int = ...,
         DefaultEncryptionKey: str = ...,
         DeadLetterQueueUrl: str = ...,
         Matching: MatchingRequestTypeDef = ...,
+        RuleBasedMatching: RuleBasedMatchingRequestTypeDef = ...,
         Tags: Mapping[str, str] = ...
     ) -> UpdateDomainResponseTypeDef:
         """
         Updates the properties of a domain, including creating or selecting a dead
         letter queue or an encryption key.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/customer-profiles.html#CustomerProfiles.Client.update_domain)
```

### Comparing `types-aiobotocore-customer-profiles-2.5.2.post3/types_aiobotocore_customer_profiles/client.pyi` & `types-aiobotocore-customer-profiles-2.5.4/types_aiobotocore_customer_profiles/client.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -16,15 +16,22 @@
 """
 import sys
 from typing import Any, Dict, Mapping, Sequence, Type
 
 from aiobotocore.client import AioBaseClient
 from botocore.client import ClientMeta
 
-from .literals import GenderType, PartyTypeType, StatisticType, StatusType, logicalOperatorType
+from .literals import (
+    GenderType,
+    MatchTypeType,
+    PartyTypeType,
+    StatisticType,
+    StatusType,
+    logicalOperatorType,
+)
 from .paginator import ListEventStreamsPaginator
 from .type_defs import (
     AdditionalSearchKeyTypeDef,
     AddProfileKeyResponseTypeDef,
     AddressTypeDef,
     AttributeDetailsTypeDef,
     ConditionsTypeDef,
@@ -49,37 +56,40 @@
     GetDomainResponseTypeDef,
     GetEventStreamResponseTypeDef,
     GetIdentityResolutionJobResponseTypeDef,
     GetIntegrationResponseTypeDef,
     GetMatchesResponseTypeDef,
     GetProfileObjectTypeResponseTypeDef,
     GetProfileObjectTypeTemplateResponseTypeDef,
+    GetSimilarProfilesResponseTypeDef,
     GetWorkflowResponseTypeDef,
     GetWorkflowStepsResponseTypeDef,
     IntegrationConfigTypeDef,
     ListAccountIntegrationsResponseTypeDef,
     ListCalculatedAttributeDefinitionsResponseTypeDef,
     ListCalculatedAttributesForProfileResponseTypeDef,
     ListDomainsResponseTypeDef,
     ListEventStreamsResponseTypeDef,
     ListIdentityResolutionJobsResponseTypeDef,
     ListIntegrationsResponseTypeDef,
     ListProfileObjectsResponseTypeDef,
     ListProfileObjectTypesResponseTypeDef,
     ListProfileObjectTypeTemplatesResponseTypeDef,
+    ListRuleBasedMatchesResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     ListWorkflowsResponseTypeDef,
     MatchingRequestTypeDef,
     MergeProfilesResponseTypeDef,
     ObjectFilterTypeDef,
     ObjectTypeFieldTypeDef,
     ObjectTypeKeyTypeDef,
     PutIntegrationResponseTypeDef,
     PutProfileObjectResponseTypeDef,
     PutProfileObjectTypeResponseTypeDef,
+    RuleBasedMatchingRequestTypeDef,
     SearchProfilesResponseTypeDef,
     TimestampTypeDef,
     UpdateAddressTypeDef,
     UpdateCalculatedAttributeDefinitionResponseTypeDef,
     UpdateDomainResponseTypeDef,
     UpdateProfileResponseTypeDef,
 )
@@ -168,14 +178,15 @@
         self,
         *,
         DomainName: str,
         DefaultExpirationDays: int,
         DefaultEncryptionKey: str = ...,
         DeadLetterQueueUrl: str = ...,
         Matching: MatchingRequestTypeDef = ...,
+        RuleBasedMatching: RuleBasedMatchingRequestTypeDef = ...,
         Tags: Mapping[str, str] = ...
     ) -> CreateDomainResponseTypeDef:
         """
         Creates a domain, which is a container for all customer data, such as customer
         profile attributes, object types, profile keys, and encryption keys.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/customer-profiles.html#CustomerProfiles.Client.create_domain)
@@ -424,14 +435,31 @@
     ) -> GetProfileObjectTypeTemplateResponseTypeDef:
         """
         Returns the template information for a specific object type.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/customer-profiles.html#CustomerProfiles.Client.get_profile_object_type_template)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_customer_profiles/client/#get_profile_object_type_template)
         """
+    async def get_similar_profiles(
+        self,
+        *,
+        DomainName: str,
+        MatchType: MatchTypeType,
+        SearchKey: str,
+        SearchValue: str,
+        NextToken: str = ...,
+        MaxResults: int = ...
+    ) -> GetSimilarProfilesResponseTypeDef:
+        """
+        Returns a set of profiles that belong to the same matching group using the
+        `matchId` or `profileId`.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/customer-profiles.html#CustomerProfiles.Client.get_similar_profiles)
+        [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_customer_profiles/client/#get_similar_profiles)
+        """
     async def get_workflow(self, *, DomainName: str, WorkflowId: str) -> GetWorkflowResponseTypeDef:
         """
         Get details of specified workflow.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/customer-profiles.html#CustomerProfiles.Client.get_workflow)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_customer_profiles/client/#get_workflow)
         """
@@ -545,14 +573,23 @@
         """
         Returns a list of objects associated with a profile of a given
         ProfileObjectType.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/customer-profiles.html#CustomerProfiles.Client.list_profile_objects)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_customer_profiles/client/#list_profile_objects)
         """
+    async def list_rule_based_matches(
+        self, *, DomainName: str, NextToken: str = ..., MaxResults: int = ...
+    ) -> ListRuleBasedMatchesResponseTypeDef:
+        """
+        Returns a set of `MatchIds` that belong to the given domain.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/customer-profiles.html#CustomerProfiles.Client.list_rule_based_matches)
+        [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_customer_profiles/client/#list_rule_based_matches)
+        """
     async def list_tags_for_resource(
         self, *, resourceArn: str
     ) -> ListTagsForResourceResponseTypeDef:
         """
         Displays the tags associated with an Amazon Connect Customer Profiles resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/customer-profiles.html#CustomerProfiles.Client.list_tags_for_resource)
@@ -691,14 +728,15 @@
         self,
         *,
         DomainName: str,
         DefaultExpirationDays: int = ...,
         DefaultEncryptionKey: str = ...,
         DeadLetterQueueUrl: str = ...,
         Matching: MatchingRequestTypeDef = ...,
+        RuleBasedMatching: RuleBasedMatchingRequestTypeDef = ...,
         Tags: Mapping[str, str] = ...
     ) -> UpdateDomainResponseTypeDef:
         """
         Updates the properties of a domain, including creating or selecting a dead
         letter queue or an encryption key.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/customer-profiles.html#CustomerProfiles.Client.update_domain)
```

### Comparing `types-aiobotocore-customer-profiles-2.5.2.post3/types_aiobotocore_customer_profiles/literals.py` & `types-aiobotocore-customer-profiles-2.5.4/types_aiobotocore_customer_profiles/literals.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,41 +2,44 @@
 Type annotations for customer-profiles service literal definitions.
 
 [Open documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_customer_profiles/literals/)
 
 Usage::
 
     ```python
-    from types_aiobotocore_customer_profiles.literals import ConflictResolvingModelType
+    from types_aiobotocore_customer_profiles.literals import AttributeMatchingModelType
 
-    data: ConflictResolvingModelType = "RECENCY"
+    data: AttributeMatchingModelType = "MANY_TO_MANY"
     ```
 """
 import sys
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
 
 __all__ = (
+    "AttributeMatchingModelType",
     "ConflictResolvingModelType",
     "DataPullModeType",
     "EventStreamDestinationStatusType",
     "EventStreamStateType",
     "FieldContentTypeType",
     "GenderType",
     "IdentityResolutionJobStatusType",
     "JobScheduleDayOfTheWeekType",
     "ListEventStreamsPaginatorName",
     "MarketoConnectorOperatorType",
+    "MatchTypeType",
     "OperatorPropertiesKeysType",
     "OperatorType",
     "PartyTypeType",
+    "RuleBasedMatchingStatusType",
     "S3ConnectorOperatorType",
     "SalesforceConnectorOperatorType",
     "ServiceNowConnectorOperatorType",
     "SourceConnectorTypeType",
     "StandardIdentifierType",
     "StatisticType",
     "StatusType",
@@ -50,14 +53,15 @@
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "RegionName",
 )
 
 
+AttributeMatchingModelType = Literal["MANY_TO_MANY", "ONE_TO_ONE"]
 ConflictResolvingModelType = Literal["RECENCY", "SOURCE"]
 DataPullModeType = Literal["Complete", "Incremental"]
 EventStreamDestinationStatusType = Literal["HEALTHY", "UNHEALTHY"]
 EventStreamStateType = Literal["RUNNING", "STOPPED"]
 FieldContentTypeType = Literal["EMAIL_ADDRESS", "NAME", "NUMBER", "PHONE_NUMBER", "STRING"]
 GenderType = Literal["FEMALE", "MALE", "UNSPECIFIED"]
 IdentityResolutionJobStatusType = Literal[
@@ -81,14 +85,15 @@
     "PROJECTION",
     "SUBTRACTION",
     "VALIDATE_NON_NEGATIVE",
     "VALIDATE_NON_NULL",
     "VALIDATE_NON_ZERO",
     "VALIDATE_NUMERIC",
 ]
+MatchTypeType = Literal["ML_BASED_MATCHING", "RULE_BASED_MATCHING"]
 OperatorPropertiesKeysType = Literal[
     "CONCAT_FORMAT",
     "DATA_TYPE",
     "DESTINATION_DATA_TYPE",
     "LOWER_BOUND",
     "MASK_LENGTH",
     "MASK_VALUE",
@@ -99,14 +104,15 @@
     "UPPER_BOUND",
     "VALIDATION_ACTION",
     "VALUE",
     "VALUES",
 ]
 OperatorType = Literal["EQUAL_TO", "GREATER_THAN", "LESS_THAN", "NOT_EQUAL_TO"]
 PartyTypeType = Literal["BUSINESS", "INDIVIDUAL", "OTHER"]
+RuleBasedMatchingStatusType = Literal["ACTIVE", "IN_PROGRESS", "PENDING"]
 S3ConnectorOperatorType = Literal[
     "ADDITION",
     "BETWEEN",
     "DIVISION",
     "EQUAL_TO",
     "GREATER_THAN",
     "GREATER_THAN_OR_EQUAL_TO",
@@ -221,14 +227,15 @@
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
@@ -324,14 +331,15 @@
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
@@ -410,26 +418,28 @@
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

### Comparing `types-aiobotocore-customer-profiles-2.5.2.post3/types_aiobotocore_customer_profiles/literals.pyi` & `types-aiobotocore-customer-profiles-2.5.4/types_aiobotocore_customer_profiles/literals.pyi`

 * *Files 6% similar despite different names*

```diff
@@ -2,40 +2,43 @@
 Type annotations for customer-profiles service literal definitions.
 
 [Open documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_customer_profiles/literals/)
 
 Usage::
 
     ```python
-    from types_aiobotocore_customer_profiles.literals import ConflictResolvingModelType
+    from types_aiobotocore_customer_profiles.literals import AttributeMatchingModelType
 
-    data: ConflictResolvingModelType = "RECENCY"
+    data: AttributeMatchingModelType = "MANY_TO_MANY"
     ```
 """
 import sys
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
 __all__ = (
+    "AttributeMatchingModelType",
     "ConflictResolvingModelType",
     "DataPullModeType",
     "EventStreamDestinationStatusType",
     "EventStreamStateType",
     "FieldContentTypeType",
     "GenderType",
     "IdentityResolutionJobStatusType",
     "JobScheduleDayOfTheWeekType",
     "ListEventStreamsPaginatorName",
     "MarketoConnectorOperatorType",
+    "MatchTypeType",
     "OperatorPropertiesKeysType",
     "OperatorType",
     "PartyTypeType",
+    "RuleBasedMatchingStatusType",
     "S3ConnectorOperatorType",
     "SalesforceConnectorOperatorType",
     "ServiceNowConnectorOperatorType",
     "SourceConnectorTypeType",
     "StandardIdentifierType",
     "StatisticType",
     "StatusType",
@@ -48,14 +51,15 @@
     "CustomerProfilesServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "RegionName",
 )
 
+AttributeMatchingModelType = Literal["MANY_TO_MANY", "ONE_TO_ONE"]
 ConflictResolvingModelType = Literal["RECENCY", "SOURCE"]
 DataPullModeType = Literal["Complete", "Incremental"]
 EventStreamDestinationStatusType = Literal["HEALTHY", "UNHEALTHY"]
 EventStreamStateType = Literal["RUNNING", "STOPPED"]
 FieldContentTypeType = Literal["EMAIL_ADDRESS", "NAME", "NUMBER", "PHONE_NUMBER", "STRING"]
 GenderType = Literal["FEMALE", "MALE", "UNSPECIFIED"]
 IdentityResolutionJobStatusType = Literal[
@@ -79,14 +83,15 @@
     "PROJECTION",
     "SUBTRACTION",
     "VALIDATE_NON_NEGATIVE",
     "VALIDATE_NON_NULL",
     "VALIDATE_NON_ZERO",
     "VALIDATE_NUMERIC",
 ]
+MatchTypeType = Literal["ML_BASED_MATCHING", "RULE_BASED_MATCHING"]
 OperatorPropertiesKeysType = Literal[
     "CONCAT_FORMAT",
     "DATA_TYPE",
     "DESTINATION_DATA_TYPE",
     "LOWER_BOUND",
     "MASK_LENGTH",
     "MASK_VALUE",
@@ -97,14 +102,15 @@
     "UPPER_BOUND",
     "VALIDATION_ACTION",
     "VALUE",
     "VALUES",
 ]
 OperatorType = Literal["EQUAL_TO", "GREATER_THAN", "LESS_THAN", "NOT_EQUAL_TO"]
 PartyTypeType = Literal["BUSINESS", "INDIVIDUAL", "OTHER"]
+RuleBasedMatchingStatusType = Literal["ACTIVE", "IN_PROGRESS", "PENDING"]
 S3ConnectorOperatorType = Literal[
     "ADDITION",
     "BETWEEN",
     "DIVISION",
     "EQUAL_TO",
     "GREATER_THAN",
     "GREATER_THAN_OR_EQUAL_TO",
@@ -219,14 +225,15 @@
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
@@ -322,14 +329,15 @@
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
@@ -408,26 +416,28 @@
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

### Comparing `types-aiobotocore-customer-profiles-2.5.2.post3/types_aiobotocore_customer_profiles/paginator.py` & `types-aiobotocore-customer-profiles-2.5.4/types_aiobotocore_customer_profiles/paginator.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-customer-profiles-2.5.2.post3/types_aiobotocore_customer_profiles/paginator.pyi` & `types-aiobotocore-customer-profiles-2.5.4/types_aiobotocore_customer_profiles/paginator.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-customer-profiles-2.5.2.post3/types_aiobotocore_customer_profiles/type_defs.py` & `types-aiobotocore-customer-profiles-2.5.4/types_aiobotocore_customer_profiles/type_defs.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,26 +12,29 @@
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, List, Mapping, Sequence, Union
 
 from .literals import (
+    AttributeMatchingModelType,
     ConflictResolvingModelType,
     DataPullModeType,
     EventStreamDestinationStatusType,
     EventStreamStateType,
     FieldContentTypeType,
     GenderType,
     IdentityResolutionJobStatusType,
     JobScheduleDayOfTheWeekType,
     MarketoConnectorOperatorType,
+    MatchTypeType,
     OperatorPropertiesKeysType,
     OperatorType,
     PartyTypeType,
+    RuleBasedMatchingStatusType,
     S3ConnectorOperatorType,
     SalesforceConnectorOperatorType,
     ServiceNowConnectorOperatorType,
     SourceConnectorTypeType,
     StandardIdentifierType,
     StatisticType,
     StatusType,
@@ -56,14 +59,15 @@
     "ResponseMetadataTypeDef",
     "AdditionalSearchKeyTypeDef",
     "AddressTypeDef",
     "AppflowIntegrationWorkflowAttributesTypeDef",
     "AppflowIntegrationWorkflowMetricsTypeDef",
     "AppflowIntegrationWorkflowStepTypeDef",
     "AttributeItemTypeDef",
+    "AttributeTypesSelectorTypeDef",
     "ConflictResolutionTypeDef",
     "ConsolidationTypeDef",
     "TimestampTypeDef",
     "RangeTypeDef",
     "ThresholdTypeDef",
     "ConnectorOperatorTypeDef",
     "CreateEventStreamRequestRequestTypeDef",
@@ -92,14 +96,15 @@
     "GetIntegrationRequestRequestTypeDef",
     "GetMatchesRequestRequestTypeDef",
     "MatchItemTypeDef",
     "GetProfileObjectTypeRequestRequestTypeDef",
     "ObjectTypeFieldTypeDef",
     "ObjectTypeKeyTypeDef",
     "GetProfileObjectTypeTemplateRequestRequestTypeDef",
+    "GetSimilarProfilesRequestRequestTypeDef",
     "GetWorkflowRequestRequestTypeDef",
     "GetWorkflowStepsRequestRequestTypeDef",
     "IncrementalPullConfigTypeDef",
     "JobScheduleTypeDef",
     "ListAccountIntegrationsRequestRequestTypeDef",
     "ListIntegrationItemTypeDef",
     "ListCalculatedAttributeDefinitionItemTypeDef",
@@ -114,17 +119,19 @@
     "ListIntegrationsRequestRequestTypeDef",
     "ListProfileObjectTypeItemTypeDef",
     "ListProfileObjectTypeTemplateItemTypeDef",
     "ListProfileObjectTypeTemplatesRequestRequestTypeDef",
     "ListProfileObjectTypesRequestRequestTypeDef",
     "ListProfileObjectsItemTypeDef",
     "ObjectFilterTypeDef",
+    "ListRuleBasedMatchesRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
     "ListWorkflowsItemTypeDef",
     "MarketoSourcePropertiesTypeDef",
+    "MatchingRuleTypeDef",
     "PutProfileObjectRequestRequestTypeDef",
     "S3SourcePropertiesTypeDef",
     "SalesforceSourcePropertiesTypeDef",
     "ServiceNowSourcePropertiesTypeDef",
     "ZendeskSourcePropertiesTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
@@ -138,14 +145,16 @@
     "DeleteProfileKeyResponseTypeDef",
     "DeleteProfileObjectResponseTypeDef",
     "DeleteProfileObjectTypeResponseTypeDef",
     "DeleteProfileResponseTypeDef",
     "GetAutoMergingPreviewResponseTypeDef",
     "GetCalculatedAttributeForProfileResponseTypeDef",
     "GetIntegrationResponseTypeDef",
+    "GetSimilarProfilesResponseTypeDef",
+    "ListRuleBasedMatchesResponseTypeDef",
     "ListTagsForResourceResponseTypeDef",
     "MergeProfilesResponseTypeDef",
     "PutIntegrationResponseTypeDef",
     "PutProfileObjectResponseTypeDef",
     "UpdateProfileResponseTypeDef",
     "SearchProfilesRequestRequestTypeDef",
     "CreateProfileRequestRequestTypeDef",
@@ -191,14 +200,16 @@
     "CreateCalculatedAttributeDefinitionResponseTypeDef",
     "GetCalculatedAttributeDefinitionResponseTypeDef",
     "UpdateCalculatedAttributeDefinitionRequestRequestTypeDef",
     "UpdateCalculatedAttributeDefinitionResponseTypeDef",
     "ListEventStreamsResponseTypeDef",
     "MatchingRequestTypeDef",
     "MatchingResponseTypeDef",
+    "RuleBasedMatchingRequestTypeDef",
+    "RuleBasedMatchingResponseTypeDef",
     "GetIdentityResolutionJobResponseTypeDef",
     "IdentityResolutionJobTypeDef",
     "SearchProfilesResponseTypeDef",
     "SourceFlowConfigTypeDef",
     "TriggerConfigTypeDef",
     "CreateDomainRequestRequestTypeDef",
     "UpdateDomainRequestRequestTypeDef",
@@ -308,14 +319,37 @@
 AttributeItemTypeDef = TypedDict(
     "AttributeItemTypeDef",
     {
         "Name": str,
     },
 )
 
+_RequiredAttributeTypesSelectorTypeDef = TypedDict(
+    "_RequiredAttributeTypesSelectorTypeDef",
+    {
+        "AttributeMatchingModel": AttributeMatchingModelType,
+    },
+)
+_OptionalAttributeTypesSelectorTypeDef = TypedDict(
+    "_OptionalAttributeTypesSelectorTypeDef",
+    {
+        "Address": Sequence[str],
+        "PhoneNumber": Sequence[str],
+        "EmailAddress": Sequence[str],
+    },
+    total=False,
+)
+
+
+class AttributeTypesSelectorTypeDef(
+    _RequiredAttributeTypesSelectorTypeDef, _OptionalAttributeTypesSelectorTypeDef
+):
+    pass
+
+
 _RequiredConflictResolutionTypeDef = TypedDict(
     "_RequiredConflictResolutionTypeDef",
     {
         "ConflictResolvingModel": ConflictResolvingModelType,
     },
 )
 _OptionalConflictResolutionTypeDef = TypedDict(
@@ -710,14 +744,40 @@
 GetProfileObjectTypeTemplateRequestRequestTypeDef = TypedDict(
     "GetProfileObjectTypeTemplateRequestRequestTypeDef",
     {
         "TemplateId": str,
     },
 )
 
+_RequiredGetSimilarProfilesRequestRequestTypeDef = TypedDict(
+    "_RequiredGetSimilarProfilesRequestRequestTypeDef",
+    {
+        "DomainName": str,
+        "MatchType": MatchTypeType,
+        "SearchKey": str,
+        "SearchValue": str,
+    },
+)
+_OptionalGetSimilarProfilesRequestRequestTypeDef = TypedDict(
+    "_OptionalGetSimilarProfilesRequestRequestTypeDef",
+    {
+        "NextToken": str,
+        "MaxResults": int,
+    },
+    total=False,
+)
+
+
+class GetSimilarProfilesRequestRequestTypeDef(
+    _RequiredGetSimilarProfilesRequestRequestTypeDef,
+    _OptionalGetSimilarProfilesRequestRequestTypeDef,
+):
+    pass
+
+
 GetWorkflowRequestRequestTypeDef = TypedDict(
     "GetWorkflowRequestRequestTypeDef",
     {
         "DomainName": str,
         "WorkflowId": str,
     },
 )
@@ -1072,14 +1132,37 @@
     "ObjectFilterTypeDef",
     {
         "KeyName": str,
         "Values": Sequence[str],
     },
 )
 
+_RequiredListRuleBasedMatchesRequestRequestTypeDef = TypedDict(
+    "_RequiredListRuleBasedMatchesRequestRequestTypeDef",
+    {
+        "DomainName": str,
+    },
+)
+_OptionalListRuleBasedMatchesRequestRequestTypeDef = TypedDict(
+    "_OptionalListRuleBasedMatchesRequestRequestTypeDef",
+    {
+        "NextToken": str,
+        "MaxResults": int,
+    },
+    total=False,
+)
+
+
+class ListRuleBasedMatchesRequestRequestTypeDef(
+    _RequiredListRuleBasedMatchesRequestRequestTypeDef,
+    _OptionalListRuleBasedMatchesRequestRequestTypeDef,
+):
+    pass
+
+
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
     },
 )
 
@@ -1098,14 +1181,21 @@
 MarketoSourcePropertiesTypeDef = TypedDict(
     "MarketoSourcePropertiesTypeDef",
     {
         "Object": str,
     },
 )
 
+MatchingRuleTypeDef = TypedDict(
+    "MatchingRuleTypeDef",
+    {
+        "Rule": Sequence[str],
+    },
+)
+
 PutProfileObjectRequestRequestTypeDef = TypedDict(
     "PutProfileObjectRequestRequestTypeDef",
     {
         "ObjectTypeName": str,
         "Object": str,
         "DomainName": str,
     },
@@ -1318,14 +1408,36 @@
         "ObjectTypeNames": Dict[str, str],
         "WorkflowId": str,
         "IsUnstructured": bool,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+GetSimilarProfilesResponseTypeDef = TypedDict(
+    "GetSimilarProfilesResponseTypeDef",
+    {
+        "ProfileIds": List[str],
+        "MatchId": str,
+        "MatchType": MatchTypeType,
+        "RuleLevel": int,
+        "ConfidenceScore": float,
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListRuleBasedMatchesResponseTypeDef = TypedDict(
+    "ListRuleBasedMatchesResponseTypeDef",
+    {
+        "MatchIds": List[str],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 ListTagsForResourceResponseTypeDef = TypedDict(
     "ListTagsForResourceResponseTypeDef",
     {
         "tags": Dict[str, str],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -2170,14 +2282,55 @@
         "JobSchedule": JobScheduleTypeDef,
         "AutoMerging": AutoMergingTypeDef,
         "ExportingConfig": ExportingConfigTypeDef,
     },
     total=False,
 )
 
+_RequiredRuleBasedMatchingRequestTypeDef = TypedDict(
+    "_RequiredRuleBasedMatchingRequestTypeDef",
+    {
+        "Enabled": bool,
+    },
+)
+_OptionalRuleBasedMatchingRequestTypeDef = TypedDict(
+    "_OptionalRuleBasedMatchingRequestTypeDef",
+    {
+        "MatchingRules": Sequence[MatchingRuleTypeDef],
+        "MaxAllowedRuleLevelForMerging": int,
+        "MaxAllowedRuleLevelForMatching": int,
+        "AttributeTypesSelector": AttributeTypesSelectorTypeDef,
+        "ConflictResolution": ConflictResolutionTypeDef,
+        "ExportingConfig": ExportingConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class RuleBasedMatchingRequestTypeDef(
+    _RequiredRuleBasedMatchingRequestTypeDef, _OptionalRuleBasedMatchingRequestTypeDef
+):
+    pass
+
+
+RuleBasedMatchingResponseTypeDef = TypedDict(
+    "RuleBasedMatchingResponseTypeDef",
+    {
+        "Enabled": bool,
+        "MatchingRules": List[MatchingRuleTypeDef],
+        "Status": RuleBasedMatchingStatusType,
+        "MaxAllowedRuleLevelForMerging": int,
+        "MaxAllowedRuleLevelForMatching": int,
+        "AttributeTypesSelector": AttributeTypesSelectorTypeDef,
+        "ConflictResolution": ConflictResolutionTypeDef,
+        "ExportingConfig": ExportingConfigTypeDef,
+    },
+    total=False,
+)
+
 GetIdentityResolutionJobResponseTypeDef = TypedDict(
     "GetIdentityResolutionJobResponseTypeDef",
     {
         "DomainName": str,
         "JobId": str,
         "Status": IdentityResolutionJobStatusType,
         "Message": str,
@@ -2265,14 +2418,15 @@
 )
 _OptionalCreateDomainRequestRequestTypeDef = TypedDict(
     "_OptionalCreateDomainRequestRequestTypeDef",
     {
         "DefaultEncryptionKey": str,
         "DeadLetterQueueUrl": str,
         "Matching": MatchingRequestTypeDef,
+        "RuleBasedMatching": RuleBasedMatchingRequestTypeDef,
         "Tags": Mapping[str, str],
     },
     total=False,
 )
 
 
 class CreateDomainRequestRequestTypeDef(
@@ -2290,14 +2444,15 @@
 _OptionalUpdateDomainRequestRequestTypeDef = TypedDict(
     "_OptionalUpdateDomainRequestRequestTypeDef",
     {
         "DefaultExpirationDays": int,
         "DefaultEncryptionKey": str,
         "DeadLetterQueueUrl": str,
         "Matching": MatchingRequestTypeDef,
+        "RuleBasedMatching": RuleBasedMatchingRequestTypeDef,
         "Tags": Mapping[str, str],
     },
     total=False,
 )
 
 
 class UpdateDomainRequestRequestTypeDef(
@@ -2310,14 +2465,15 @@
     "CreateDomainResponseTypeDef",
     {
         "DomainName": str,
         "DefaultExpirationDays": int,
         "DefaultEncryptionKey": str,
         "DeadLetterQueueUrl": str,
         "Matching": MatchingResponseTypeDef,
+        "RuleBasedMatching": RuleBasedMatchingResponseTypeDef,
         "CreatedAt": datetime,
         "LastUpdatedAt": datetime,
         "Tags": Dict[str, str],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
@@ -2326,14 +2482,15 @@
     {
         "DomainName": str,
         "DefaultExpirationDays": int,
         "DefaultEncryptionKey": str,
         "DeadLetterQueueUrl": str,
         "Stats": DomainStatsTypeDef,
         "Matching": MatchingResponseTypeDef,
+        "RuleBasedMatching": RuleBasedMatchingResponseTypeDef,
         "CreatedAt": datetime,
         "LastUpdatedAt": datetime,
         "Tags": Dict[str, str],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
@@ -2341,14 +2498,15 @@
     "UpdateDomainResponseTypeDef",
     {
         "DomainName": str,
         "DefaultExpirationDays": int,
         "DefaultEncryptionKey": str,
         "DeadLetterQueueUrl": str,
         "Matching": MatchingResponseTypeDef,
+        "RuleBasedMatching": RuleBasedMatchingResponseTypeDef,
         "CreatedAt": datetime,
         "LastUpdatedAt": datetime,
         "Tags": Dict[str, str],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `types-aiobotocore-customer-profiles-2.5.2.post3/types_aiobotocore_customer_profiles/type_defs.pyi` & `types-aiobotocore-customer-profiles-2.5.4/types_aiobotocore_customer_profiles/type_defs.pyi`

 * *Files 3% similar despite different names*

```diff
@@ -12,26 +12,29 @@
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, List, Mapping, Sequence, Union
 
 from .literals import (
+    AttributeMatchingModelType,
     ConflictResolvingModelType,
     DataPullModeType,
     EventStreamDestinationStatusType,
     EventStreamStateType,
     FieldContentTypeType,
     GenderType,
     IdentityResolutionJobStatusType,
     JobScheduleDayOfTheWeekType,
     MarketoConnectorOperatorType,
+    MatchTypeType,
     OperatorPropertiesKeysType,
     OperatorType,
     PartyTypeType,
+    RuleBasedMatchingStatusType,
     S3ConnectorOperatorType,
     SalesforceConnectorOperatorType,
     ServiceNowConnectorOperatorType,
     SourceConnectorTypeType,
     StandardIdentifierType,
     StatisticType,
     StatusType,
@@ -55,14 +58,15 @@
     "ResponseMetadataTypeDef",
     "AdditionalSearchKeyTypeDef",
     "AddressTypeDef",
     "AppflowIntegrationWorkflowAttributesTypeDef",
     "AppflowIntegrationWorkflowMetricsTypeDef",
     "AppflowIntegrationWorkflowStepTypeDef",
     "AttributeItemTypeDef",
+    "AttributeTypesSelectorTypeDef",
     "ConflictResolutionTypeDef",
     "ConsolidationTypeDef",
     "TimestampTypeDef",
     "RangeTypeDef",
     "ThresholdTypeDef",
     "ConnectorOperatorTypeDef",
     "CreateEventStreamRequestRequestTypeDef",
@@ -91,14 +95,15 @@
     "GetIntegrationRequestRequestTypeDef",
     "GetMatchesRequestRequestTypeDef",
     "MatchItemTypeDef",
     "GetProfileObjectTypeRequestRequestTypeDef",
     "ObjectTypeFieldTypeDef",
     "ObjectTypeKeyTypeDef",
     "GetProfileObjectTypeTemplateRequestRequestTypeDef",
+    "GetSimilarProfilesRequestRequestTypeDef",
     "GetWorkflowRequestRequestTypeDef",
     "GetWorkflowStepsRequestRequestTypeDef",
     "IncrementalPullConfigTypeDef",
     "JobScheduleTypeDef",
     "ListAccountIntegrationsRequestRequestTypeDef",
     "ListIntegrationItemTypeDef",
     "ListCalculatedAttributeDefinitionItemTypeDef",
@@ -113,17 +118,19 @@
     "ListIntegrationsRequestRequestTypeDef",
     "ListProfileObjectTypeItemTypeDef",
     "ListProfileObjectTypeTemplateItemTypeDef",
     "ListProfileObjectTypeTemplatesRequestRequestTypeDef",
     "ListProfileObjectTypesRequestRequestTypeDef",
     "ListProfileObjectsItemTypeDef",
     "ObjectFilterTypeDef",
+    "ListRuleBasedMatchesRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
     "ListWorkflowsItemTypeDef",
     "MarketoSourcePropertiesTypeDef",
+    "MatchingRuleTypeDef",
     "PutProfileObjectRequestRequestTypeDef",
     "S3SourcePropertiesTypeDef",
     "SalesforceSourcePropertiesTypeDef",
     "ServiceNowSourcePropertiesTypeDef",
     "ZendeskSourcePropertiesTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
@@ -137,14 +144,16 @@
     "DeleteProfileKeyResponseTypeDef",
     "DeleteProfileObjectResponseTypeDef",
     "DeleteProfileObjectTypeResponseTypeDef",
     "DeleteProfileResponseTypeDef",
     "GetAutoMergingPreviewResponseTypeDef",
     "GetCalculatedAttributeForProfileResponseTypeDef",
     "GetIntegrationResponseTypeDef",
+    "GetSimilarProfilesResponseTypeDef",
+    "ListRuleBasedMatchesResponseTypeDef",
     "ListTagsForResourceResponseTypeDef",
     "MergeProfilesResponseTypeDef",
     "PutIntegrationResponseTypeDef",
     "PutProfileObjectResponseTypeDef",
     "UpdateProfileResponseTypeDef",
     "SearchProfilesRequestRequestTypeDef",
     "CreateProfileRequestRequestTypeDef",
@@ -190,14 +199,16 @@
     "CreateCalculatedAttributeDefinitionResponseTypeDef",
     "GetCalculatedAttributeDefinitionResponseTypeDef",
     "UpdateCalculatedAttributeDefinitionRequestRequestTypeDef",
     "UpdateCalculatedAttributeDefinitionResponseTypeDef",
     "ListEventStreamsResponseTypeDef",
     "MatchingRequestTypeDef",
     "MatchingResponseTypeDef",
+    "RuleBasedMatchingRequestTypeDef",
+    "RuleBasedMatchingResponseTypeDef",
     "GetIdentityResolutionJobResponseTypeDef",
     "IdentityResolutionJobTypeDef",
     "SearchProfilesResponseTypeDef",
     "SourceFlowConfigTypeDef",
     "TriggerConfigTypeDef",
     "CreateDomainRequestRequestTypeDef",
     "UpdateDomainRequestRequestTypeDef",
@@ -305,14 +316,35 @@
 AttributeItemTypeDef = TypedDict(
     "AttributeItemTypeDef",
     {
         "Name": str,
     },
 )
 
+_RequiredAttributeTypesSelectorTypeDef = TypedDict(
+    "_RequiredAttributeTypesSelectorTypeDef",
+    {
+        "AttributeMatchingModel": AttributeMatchingModelType,
+    },
+)
+_OptionalAttributeTypesSelectorTypeDef = TypedDict(
+    "_OptionalAttributeTypesSelectorTypeDef",
+    {
+        "Address": Sequence[str],
+        "PhoneNumber": Sequence[str],
+        "EmailAddress": Sequence[str],
+    },
+    total=False,
+)
+
+class AttributeTypesSelectorTypeDef(
+    _RequiredAttributeTypesSelectorTypeDef, _OptionalAttributeTypesSelectorTypeDef
+):
+    pass
+
 _RequiredConflictResolutionTypeDef = TypedDict(
     "_RequiredConflictResolutionTypeDef",
     {
         "ConflictResolvingModel": ConflictResolvingModelType,
     },
 )
 _OptionalConflictResolutionTypeDef = TypedDict(
@@ -695,14 +727,38 @@
 GetProfileObjectTypeTemplateRequestRequestTypeDef = TypedDict(
     "GetProfileObjectTypeTemplateRequestRequestTypeDef",
     {
         "TemplateId": str,
     },
 )
 
+_RequiredGetSimilarProfilesRequestRequestTypeDef = TypedDict(
+    "_RequiredGetSimilarProfilesRequestRequestTypeDef",
+    {
+        "DomainName": str,
+        "MatchType": MatchTypeType,
+        "SearchKey": str,
+        "SearchValue": str,
+    },
+)
+_OptionalGetSimilarProfilesRequestRequestTypeDef = TypedDict(
+    "_OptionalGetSimilarProfilesRequestRequestTypeDef",
+    {
+        "NextToken": str,
+        "MaxResults": int,
+    },
+    total=False,
+)
+
+class GetSimilarProfilesRequestRequestTypeDef(
+    _RequiredGetSimilarProfilesRequestRequestTypeDef,
+    _OptionalGetSimilarProfilesRequestRequestTypeDef,
+):
+    pass
+
 GetWorkflowRequestRequestTypeDef = TypedDict(
     "GetWorkflowRequestRequestTypeDef",
     {
         "DomainName": str,
         "WorkflowId": str,
     },
 )
@@ -1035,14 +1091,35 @@
     "ObjectFilterTypeDef",
     {
         "KeyName": str,
         "Values": Sequence[str],
     },
 )
 
+_RequiredListRuleBasedMatchesRequestRequestTypeDef = TypedDict(
+    "_RequiredListRuleBasedMatchesRequestRequestTypeDef",
+    {
+        "DomainName": str,
+    },
+)
+_OptionalListRuleBasedMatchesRequestRequestTypeDef = TypedDict(
+    "_OptionalListRuleBasedMatchesRequestRequestTypeDef",
+    {
+        "NextToken": str,
+        "MaxResults": int,
+    },
+    total=False,
+)
+
+class ListRuleBasedMatchesRequestRequestTypeDef(
+    _RequiredListRuleBasedMatchesRequestRequestTypeDef,
+    _OptionalListRuleBasedMatchesRequestRequestTypeDef,
+):
+    pass
+
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
     },
 )
 
@@ -1061,14 +1138,21 @@
 MarketoSourcePropertiesTypeDef = TypedDict(
     "MarketoSourcePropertiesTypeDef",
     {
         "Object": str,
     },
 )
 
+MatchingRuleTypeDef = TypedDict(
+    "MatchingRuleTypeDef",
+    {
+        "Rule": Sequence[str],
+    },
+)
+
 PutProfileObjectRequestRequestTypeDef = TypedDict(
     "PutProfileObjectRequestRequestTypeDef",
     {
         "ObjectTypeName": str,
         "Object": str,
         "DomainName": str,
     },
@@ -1277,14 +1361,36 @@
         "ObjectTypeNames": Dict[str, str],
         "WorkflowId": str,
         "IsUnstructured": bool,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+GetSimilarProfilesResponseTypeDef = TypedDict(
+    "GetSimilarProfilesResponseTypeDef",
+    {
+        "ProfileIds": List[str],
+        "MatchId": str,
+        "MatchType": MatchTypeType,
+        "RuleLevel": int,
+        "ConfidenceScore": float,
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListRuleBasedMatchesResponseTypeDef = TypedDict(
+    "ListRuleBasedMatchesResponseTypeDef",
+    {
+        "MatchIds": List[str],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 ListTagsForResourceResponseTypeDef = TypedDict(
     "ListTagsForResourceResponseTypeDef",
     {
         "tags": Dict[str, str],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -2097,14 +2203,53 @@
         "JobSchedule": JobScheduleTypeDef,
         "AutoMerging": AutoMergingTypeDef,
         "ExportingConfig": ExportingConfigTypeDef,
     },
     total=False,
 )
 
+_RequiredRuleBasedMatchingRequestTypeDef = TypedDict(
+    "_RequiredRuleBasedMatchingRequestTypeDef",
+    {
+        "Enabled": bool,
+    },
+)
+_OptionalRuleBasedMatchingRequestTypeDef = TypedDict(
+    "_OptionalRuleBasedMatchingRequestTypeDef",
+    {
+        "MatchingRules": Sequence[MatchingRuleTypeDef],
+        "MaxAllowedRuleLevelForMerging": int,
+        "MaxAllowedRuleLevelForMatching": int,
+        "AttributeTypesSelector": AttributeTypesSelectorTypeDef,
+        "ConflictResolution": ConflictResolutionTypeDef,
+        "ExportingConfig": ExportingConfigTypeDef,
+    },
+    total=False,
+)
+
+class RuleBasedMatchingRequestTypeDef(
+    _RequiredRuleBasedMatchingRequestTypeDef, _OptionalRuleBasedMatchingRequestTypeDef
+):
+    pass
+
+RuleBasedMatchingResponseTypeDef = TypedDict(
+    "RuleBasedMatchingResponseTypeDef",
+    {
+        "Enabled": bool,
+        "MatchingRules": List[MatchingRuleTypeDef],
+        "Status": RuleBasedMatchingStatusType,
+        "MaxAllowedRuleLevelForMerging": int,
+        "MaxAllowedRuleLevelForMatching": int,
+        "AttributeTypesSelector": AttributeTypesSelectorTypeDef,
+        "ConflictResolution": ConflictResolutionTypeDef,
+        "ExportingConfig": ExportingConfigTypeDef,
+    },
+    total=False,
+)
+
 GetIdentityResolutionJobResponseTypeDef = TypedDict(
     "GetIdentityResolutionJobResponseTypeDef",
     {
         "DomainName": str,
         "JobId": str,
         "Status": IdentityResolutionJobStatusType,
         "Message": str,
@@ -2188,14 +2333,15 @@
 )
 _OptionalCreateDomainRequestRequestTypeDef = TypedDict(
     "_OptionalCreateDomainRequestRequestTypeDef",
     {
         "DefaultEncryptionKey": str,
         "DeadLetterQueueUrl": str,
         "Matching": MatchingRequestTypeDef,
+        "RuleBasedMatching": RuleBasedMatchingRequestTypeDef,
         "Tags": Mapping[str, str],
     },
     total=False,
 )
 
 class CreateDomainRequestRequestTypeDef(
     _RequiredCreateDomainRequestRequestTypeDef, _OptionalCreateDomainRequestRequestTypeDef
@@ -2211,14 +2357,15 @@
 _OptionalUpdateDomainRequestRequestTypeDef = TypedDict(
     "_OptionalUpdateDomainRequestRequestTypeDef",
     {
         "DefaultExpirationDays": int,
         "DefaultEncryptionKey": str,
         "DeadLetterQueueUrl": str,
         "Matching": MatchingRequestTypeDef,
+        "RuleBasedMatching": RuleBasedMatchingRequestTypeDef,
         "Tags": Mapping[str, str],
     },
     total=False,
 )
 
 class UpdateDomainRequestRequestTypeDef(
     _RequiredUpdateDomainRequestRequestTypeDef, _OptionalUpdateDomainRequestRequestTypeDef
@@ -2229,14 +2376,15 @@
     "CreateDomainResponseTypeDef",
     {
         "DomainName": str,
         "DefaultExpirationDays": int,
         "DefaultEncryptionKey": str,
         "DeadLetterQueueUrl": str,
         "Matching": MatchingResponseTypeDef,
+        "RuleBasedMatching": RuleBasedMatchingResponseTypeDef,
         "CreatedAt": datetime,
         "LastUpdatedAt": datetime,
         "Tags": Dict[str, str],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
@@ -2245,14 +2393,15 @@
     {
         "DomainName": str,
         "DefaultExpirationDays": int,
         "DefaultEncryptionKey": str,
         "DeadLetterQueueUrl": str,
         "Stats": DomainStatsTypeDef,
         "Matching": MatchingResponseTypeDef,
+        "RuleBasedMatching": RuleBasedMatchingResponseTypeDef,
         "CreatedAt": datetime,
         "LastUpdatedAt": datetime,
         "Tags": Dict[str, str],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
@@ -2260,14 +2409,15 @@
     "UpdateDomainResponseTypeDef",
     {
         "DomainName": str,
         "DefaultExpirationDays": int,
         "DefaultEncryptionKey": str,
         "DeadLetterQueueUrl": str,
         "Matching": MatchingResponseTypeDef,
+        "RuleBasedMatching": RuleBasedMatchingResponseTypeDef,
         "CreatedAt": datetime,
         "LastUpdatedAt": datetime,
         "Tags": Dict[str, str],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `types-aiobotocore-customer-profiles-2.5.2.post3/types_aiobotocore_customer_profiles.egg-info/PKG-INFO` & `types-aiobotocore-customer-profiles-2.5.4/types_aiobotocore_customer_profiles.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-customer-profiles
-Version: 2.5.2.post3
-Summary: Type annotations for aiobotocore.CustomerProfiles 2.5.2 service generated with mypy-boto3-builder 7.17.2
+Version: 2.5.4
+Summary: Type annotations for aiobotocore.CustomerProfiles 2.5.4 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_customer_profiles/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-customer-profiles.svg?color=blue)](https://pypi.org/project/types-aiobotocore-customer-profiles)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_customer_profiles/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-customer-profiles)](https://pepy.tech/project/types-aiobotocore-customer-profiles)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.CustomerProfiles 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/customer-profiles.html#CustomerProfiles)
+[aiobotocore.CustomerProfiles 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/customer-profiles.html#CustomerProfiles)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
@@ -295,18 +295,18 @@
 `types_aiobotocore_customer_profiles.literals` module contains literals
 extracted from shapes that can be used in user code for type checking.
 
 Full list of `CustomerProfiles` Literals can be found in
 [docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_customer_profiles/literals/).
 
 ```python
-from types_aiobotocore_customer_profiles.literals import ConflictResolvingModelType
+from types_aiobotocore_customer_profiles.literals import AttributeMatchingModelType
 
 
-def check_value(value: ConflictResolvingModelType) -> bool:
+def check_value(value: AttributeMatchingModelType) -> bool:
     ...
 ```
 
 <a id="type-definitions"></a>
 
 ### Type definitions
```

### Comparing `types-aiobotocore-customer-profiles-2.5.2.post3/types_aiobotocore_customer_profiles.egg-info/SOURCES.txt` & `types-aiobotocore-customer-profiles-2.5.4/types_aiobotocore_customer_profiles.egg-info/SOURCES.txt`

 * *Files identical despite different names*


# Comparing `tmp/types-aiobotocore-cloudformation-2.5.2.post3.tar.gz` & `tmp/types-aiobotocore-cloudformation-2.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-cloudformation-2.5.2.post3.tar", last modified: Fri Aug  4 12:37:24 2023, max compression
+gzip compressed data, was "types-aiobotocore-cloudformation-2.5.4.tar", last modified: Tue Aug  8 01:23:26 2023, max compression
```

## Comparing `types-aiobotocore-cloudformation-2.5.2.post3.tar` & `types-aiobotocore-cloudformation-2.5.4.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:37:24.139338 types-aiobotocore-cloudformation-2.5.2.post3/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-04 12:19:35.000000 types-aiobotocore-cloudformation-2.5.2.post3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    19432 2023-08-04 12:37:24.139338 types-aiobotocore-cloudformation-2.5.2.post3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    17886 2023-08-04 12:19:35.000000 types-aiobotocore-cloudformation-2.5.2.post3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-04 12:37:24.139338 types-aiobotocore-cloudformation-2.5.2.post3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2121 2023-08-04 12:19:35.000000 types-aiobotocore-cloudformation-2.5.2.post3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:37:24.135338 types-aiobotocore-cloudformation-2.5.2.post3/types_aiobotocore_cloudformation/
--rw-r--r--   0 runner    (1001) docker     (123)     5304 2023-08-04 12:19:35.000000 types-aiobotocore-cloudformation-2.5.2.post3/types_aiobotocore_cloudformation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5302 2023-08-04 12:19:35.000000 types-aiobotocore-cloudformation-2.5.2.post3/types_aiobotocore_cloudformation/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      971 2023-08-04 12:19:35.000000 types-aiobotocore-cloudformation-2.5.2.post3/types_aiobotocore_cloudformation/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    68293 2023-08-04 12:19:36.000000 types-aiobotocore-cloudformation-2.5.2.post3/types_aiobotocore_cloudformation/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    68193 2023-08-04 12:19:35.000000 types-aiobotocore-cloudformation-2.5.2.post3/types_aiobotocore_cloudformation/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    18426 2023-08-04 12:19:37.000000 types-aiobotocore-cloudformation-2.5.2.post3/types_aiobotocore_cloudformation/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    18424 2023-08-04 12:19:37.000000 types-aiobotocore-cloudformation-2.5.2.post3/types_aiobotocore_cloudformation/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    18150 2023-08-04 12:19:37.000000 types-aiobotocore-cloudformation-2.5.2.post3/types_aiobotocore_cloudformation/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)    18134 2023-08-04 12:19:36.000000 types-aiobotocore-cloudformation-2.5.2.post3/types_aiobotocore_cloudformation/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 12:19:35.000000 types-aiobotocore-cloudformation-2.5.2.post3/types_aiobotocore_cloudformation/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    25491 2023-08-04 12:19:36.000000 types-aiobotocore-cloudformation-2.5.2.post3/types_aiobotocore_cloudformation/service_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)    25444 2023-08-04 12:19:36.000000 types-aiobotocore-cloudformation-2.5.2.post3/types_aiobotocore_cloudformation/service_resource.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    94484 2023-08-04 12:19:40.000000 types-aiobotocore-cloudformation-2.5.2.post3/types_aiobotocore_cloudformation/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    94369 2023-08-04 12:19:38.000000 types-aiobotocore-cloudformation-2.5.2.post3/types_aiobotocore_cloudformation/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-04 12:19:35.000000 types-aiobotocore-cloudformation-2.5.2.post3/types_aiobotocore_cloudformation/version.py
--rw-r--r--   0 runner    (1001) docker     (123)     9291 2023-08-04 12:19:37.000000 types-aiobotocore-cloudformation-2.5.2.post3/types_aiobotocore_cloudformation/waiter.py
--rw-r--r--   0 runner    (1001) docker     (123)     9283 2023-08-04 12:19:37.000000 types-aiobotocore-cloudformation-2.5.2.post3/types_aiobotocore_cloudformation/waiter.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:37:24.139338 types-aiobotocore-cloudformation-2.5.2.post3/types_aiobotocore_cloudformation.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    19432 2023-08-04 12:37:23.000000 types-aiobotocore-cloudformation-2.5.2.post3/types_aiobotocore_cloudformation.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1140 2023-08-04 12:37:23.000000 types-aiobotocore-cloudformation-2.5.2.post3/types_aiobotocore_cloudformation.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 12:37:23.000000 types-aiobotocore-cloudformation-2.5.2.post3/types_aiobotocore_cloudformation.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 12:37:23.000000 types-aiobotocore-cloudformation-2.5.2.post3/types_aiobotocore_cloudformation.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-04 12:37:23.000000 types-aiobotocore-cloudformation-2.5.2.post3/types_aiobotocore_cloudformation.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-08-04 12:37:23.000000 types-aiobotocore-cloudformation-2.5.2.post3/types_aiobotocore_cloudformation.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:23:26.342626 types-aiobotocore-cloudformation-2.5.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-08 01:07:18.000000 types-aiobotocore-cloudformation-2.5.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    19426 2023-08-08 01:23:26.342626 types-aiobotocore-cloudformation-2.5.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    17886 2023-08-08 01:07:18.000000 types-aiobotocore-cloudformation-2.5.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-08 01:23:26.342626 types-aiobotocore-cloudformation-2.5.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2115 2023-08-08 01:07:18.000000 types-aiobotocore-cloudformation-2.5.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:23:26.338626 types-aiobotocore-cloudformation-2.5.4/types_aiobotocore_cloudformation/
+-rw-r--r--   0 runner    (1001) docker     (123)     5304 2023-08-08 01:07:18.000000 types-aiobotocore-cloudformation-2.5.4/types_aiobotocore_cloudformation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5302 2023-08-08 01:07:18.000000 types-aiobotocore-cloudformation-2.5.4/types_aiobotocore_cloudformation/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      959 2023-08-08 01:07:18.000000 types-aiobotocore-cloudformation-2.5.4/types_aiobotocore_cloudformation/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    69539 2023-08-08 01:07:18.000000 types-aiobotocore-cloudformation-2.5.4/types_aiobotocore_cloudformation/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    69438 2023-08-08 01:07:18.000000 types-aiobotocore-cloudformation-2.5.4/types_aiobotocore_cloudformation/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    18557 2023-08-08 01:07:20.000000 types-aiobotocore-cloudformation-2.5.4/types_aiobotocore_cloudformation/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18555 2023-08-08 01:07:20.000000 types-aiobotocore-cloudformation-2.5.4/types_aiobotocore_cloudformation/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    18150 2023-08-08 01:07:20.000000 types-aiobotocore-cloudformation-2.5.4/types_aiobotocore_cloudformation/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18134 2023-08-08 01:07:19.000000 types-aiobotocore-cloudformation-2.5.4/types_aiobotocore_cloudformation/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 01:07:18.000000 types-aiobotocore-cloudformation-2.5.4/types_aiobotocore_cloudformation/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    25620 2023-08-08 01:07:19.000000 types-aiobotocore-cloudformation-2.5.4/types_aiobotocore_cloudformation/service_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25573 2023-08-08 01:07:19.000000 types-aiobotocore-cloudformation-2.5.4/types_aiobotocore_cloudformation/service_resource.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    97353 2023-08-08 01:07:22.000000 types-aiobotocore-cloudformation-2.5.4/types_aiobotocore_cloudformation/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    97234 2023-08-08 01:07:21.000000 types-aiobotocore-cloudformation-2.5.4/types_aiobotocore_cloudformation/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-08-08 01:07:18.000000 types-aiobotocore-cloudformation-2.5.4/types_aiobotocore_cloudformation/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9291 2023-08-08 01:07:20.000000 types-aiobotocore-cloudformation-2.5.4/types_aiobotocore_cloudformation/waiter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9283 2023-08-08 01:07:20.000000 types-aiobotocore-cloudformation-2.5.4/types_aiobotocore_cloudformation/waiter.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:23:26.342626 types-aiobotocore-cloudformation-2.5.4/types_aiobotocore_cloudformation.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    19426 2023-08-08 01:23:26.000000 types-aiobotocore-cloudformation-2.5.4/types_aiobotocore_cloudformation.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1140 2023-08-08 01:23:26.000000 types-aiobotocore-cloudformation-2.5.4/types_aiobotocore_cloudformation.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 01:23:26.000000 types-aiobotocore-cloudformation-2.5.4/types_aiobotocore_cloudformation.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 01:23:26.000000 types-aiobotocore-cloudformation-2.5.4/types_aiobotocore_cloudformation.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-08 01:23:26.000000 types-aiobotocore-cloudformation-2.5.4/types_aiobotocore_cloudformation.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-08-08 01:23:26.000000 types-aiobotocore-cloudformation-2.5.4/types_aiobotocore_cloudformation.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-cloudformation-2.5.2.post3/LICENSE` & `types-aiobotocore-cloudformation-2.5.4/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-cloudformation-2.5.2.post3/PKG-INFO` & `types-aiobotocore-cloudformation-2.5.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-cloudformation
-Version: 2.5.2.post3
-Summary: Type annotations for aiobotocore.CloudFormation 2.5.2 service generated with mypy-boto3-builder 7.17.2
+Version: 2.5.4
+Summary: Type annotations for aiobotocore.CloudFormation 2.5.4 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudformation/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-cloudformation.svg?color=blue)](https://pypi.org/project/types-aiobotocore-cloudformation)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudformation/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-cloudformation)](https://pepy.tech/project/types-aiobotocore-cloudformation)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.CloudFormation 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudformation.html#CloudFormation)
+[aiobotocore.CloudFormation 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudformation.html#CloudFormation)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-cloudformation-2.5.2.post3/README.md` & `types-aiobotocore-cloudformation-2.5.4/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-cloudformation.svg?color=blue)](https://pypi.org/project/types-aiobotocore-cloudformation)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudformation/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-cloudformation)](https://pepy.tech/project/types-aiobotocore-cloudformation)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.CloudFormation 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudformation.html#CloudFormation)
+[aiobotocore.CloudFormation 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudformation.html#CloudFormation)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-cloudformation-2.5.2.post3/setup.py` & `types-aiobotocore-cloudformation-2.5.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-cloudformation",
-    version="2.5.2.post3",
+    version="2.5.4",
     packages=["types_aiobotocore_cloudformation"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.CloudFormation 2.5.2 service generated with"
+        "Type annotations for aiobotocore.CloudFormation 2.5.4 service generated with"
         " mypy-boto3-builder 7.17.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
```

### Comparing `types-aiobotocore-cloudformation-2.5.2.post3/types_aiobotocore_cloudformation/__init__.py` & `types-aiobotocore-cloudformation-2.5.4/types_aiobotocore_cloudformation/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-cloudformation-2.5.2.post3/types_aiobotocore_cloudformation/__init__.pyi` & `types-aiobotocore-cloudformation-2.5.4/types_aiobotocore_cloudformation/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-cloudformation-2.5.2.post3/types_aiobotocore_cloudformation/__main__.py` & `types-aiobotocore-cloudformation-2.5.4/types_aiobotocore_cloudformation/__main__.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.CloudFormation 2.5.2\nVersion:        "
-        " 2.5.2.post3\nBuilder version: 7.17.2\nDocs:           "
+        "Type annotations for aiobotocore.CloudFormation 2.5.4\nVersion:         2.5.4\nBuilder"
+        " version: 7.17.2\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudformation//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudformation.html#CloudFormation\nOther"
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

### Comparing `types-aiobotocore-cloudformation-2.5.2.post3/types_aiobotocore_cloudformation/client.py` & `types-aiobotocore-cloudformation-2.5.4/types_aiobotocore_cloudformation/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -92,14 +92,15 @@
     GetStackPolicyOutputTypeDef,
     GetTemplateOutputTypeDef,
     GetTemplateSummaryOutputTypeDef,
     ImportStacksToStackSetOutputTypeDef,
     ListChangeSetsOutputTypeDef,
     ListExportsOutputTypeDef,
     ListImportsOutputTypeDef,
+    ListStackInstanceResourceDriftsOutputTypeDef,
     ListStackInstancesOutputTypeDef,
     ListStackResourcesOutputTypeDef,
     ListStackSetOperationResultsOutputTypeDef,
     ListStackSetOperationsOutputTypeDef,
     ListStackSetsOutputTypeDef,
     ListStacksOutputTypeDef,
     ListTypeRegistrationsOutputTypeDef,
@@ -115,14 +116,15 @@
     ResourceToImportTypeDef,
     RollbackConfigurationTypeDef,
     RollbackStackOutputTypeDef,
     SetTypeConfigurationOutputTypeDef,
     StackInstanceFilterTypeDef,
     StackSetOperationPreferencesTypeDef,
     TagTypeDef,
+    TemplateSummaryConfigTypeDef,
     TestTypeOutputTypeDef,
     TypeConfigurationIdentifierTypeDef,
     TypeFiltersTypeDef,
     UpdateStackInstancesOutputTypeDef,
     UpdateStackOutputTypeDef,
     UpdateStackSetOutputTypeDef,
     UpdateTerminationProtectionOutputTypeDef,
@@ -327,15 +329,16 @@
         ResourceTypes: Sequence[str] = ...,
         RoleARN: str = ...,
         OnFailure: OnFailureType = ...,
         StackPolicyBody: str = ...,
         StackPolicyURL: str = ...,
         Tags: Sequence[TagTypeDef] = ...,
         ClientRequestToken: str = ...,
-        EnableTerminationProtection: bool = ...
+        EnableTerminationProtection: bool = ...,
+        RetainExceptOnCreate: bool = ...
     ) -> CreateStackOutputTypeDef:
         """
         Creates a stack as specified in the template.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudformation.html#CloudFormation.Client.create_stack)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudformation/client/#create_stack)
         """
@@ -720,15 +723,16 @@
 
     async def execute_change_set(
         self,
         *,
         ChangeSetName: str,
         StackName: str = ...,
         ClientRequestToken: str = ...,
-        DisableRollback: bool = ...
+        DisableRollback: bool = ...,
+        RetainExceptOnCreate: bool = ...
     ) -> Dict[str, Any]:
         """
         Updates a stack using the input information that was provided when the specified
         change set was created.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudformation.html#CloudFormation.Client.execute_change_set)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudformation/client/#execute_change_set)
@@ -773,15 +777,16 @@
     async def get_template_summary(
         self,
         *,
         TemplateBody: str = ...,
         TemplateURL: str = ...,
         StackName: str = ...,
         StackSetName: str = ...,
-        CallAs: CallAsType = ...
+        CallAs: CallAsType = ...,
+        TemplateSummaryConfig: TemplateSummaryConfigTypeDef = ...
     ) -> GetTemplateSummaryOutputTypeDef:
         """
         Returns information about a new or existing template.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudformation.html#CloudFormation.Client.get_template_summary)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudformation/client/#get_template_summary)
         """
@@ -829,14 +834,33 @@
         """
         Lists all stacks that are importing an exported output value.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudformation.html#CloudFormation.Client.list_imports)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudformation/client/#list_imports)
         """
 
+    async def list_stack_instance_resource_drifts(
+        self,
+        *,
+        StackSetName: str,
+        StackInstanceAccount: str,
+        StackInstanceRegion: str,
+        OperationId: str,
+        NextToken: str = ...,
+        MaxResults: int = ...,
+        StackInstanceResourceDriftStatuses: Sequence[StackResourceDriftStatusType] = ...,
+        CallAs: CallAsType = ...
+    ) -> ListStackInstanceResourceDriftsOutputTypeDef:
+        """
+        Returns drift information for resources in a stack instance.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudformation.html#CloudFormation.Client.list_stack_instance_resource_drifts)
+        [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudformation/client/#list_stack_instance_resource_drifts)
+        """
+
     async def list_stack_instances(
         self,
         *,
         StackSetName: str,
         NextToken: str = ...,
         MaxResults: int = ...,
         Filters: Sequence[StackInstanceFilterTypeDef] = ...,
@@ -1033,15 +1057,20 @@
         Registers an extension with the CloudFormation service.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudformation.html#CloudFormation.Client.register_type)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudformation/client/#register_type)
         """
 
     async def rollback_stack(
-        self, *, StackName: str, RoleARN: str = ..., ClientRequestToken: str = ...
+        self,
+        *,
+        StackName: str,
+        RoleARN: str = ...,
+        ClientRequestToken: str = ...,
+        RetainExceptOnCreate: bool = ...
     ) -> RollbackStackOutputTypeDef:
         """
         When specifying `RollbackStack`, you preserve the state of previously
         provisioned resources when an operation fails.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudformation.html#CloudFormation.Client.rollback_stack)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudformation/client/#rollback_stack)
@@ -1147,15 +1176,16 @@
         RoleARN: str = ...,
         RollbackConfiguration: RollbackConfigurationTypeDef = ...,
         StackPolicyBody: str = ...,
         StackPolicyURL: str = ...,
         NotificationARNs: Sequence[str] = ...,
         Tags: Sequence[TagTypeDef] = ...,
         DisableRollback: bool = ...,
-        ClientRequestToken: str = ...
+        ClientRequestToken: str = ...,
+        RetainExceptOnCreate: bool = ...
     ) -> UpdateStackOutputTypeDef:
         """
         Updates a stack as specified in the template.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudformation.html#CloudFormation.Client.update_stack)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudformation/client/#update_stack)
         """
```

### Comparing `types-aiobotocore-cloudformation-2.5.2.post3/types_aiobotocore_cloudformation/client.pyi` & `types-aiobotocore-cloudformation-2.5.4/types_aiobotocore_cloudformation/client.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -92,14 +92,15 @@
     GetStackPolicyOutputTypeDef,
     GetTemplateOutputTypeDef,
     GetTemplateSummaryOutputTypeDef,
     ImportStacksToStackSetOutputTypeDef,
     ListChangeSetsOutputTypeDef,
     ListExportsOutputTypeDef,
     ListImportsOutputTypeDef,
+    ListStackInstanceResourceDriftsOutputTypeDef,
     ListStackInstancesOutputTypeDef,
     ListStackResourcesOutputTypeDef,
     ListStackSetOperationResultsOutputTypeDef,
     ListStackSetOperationsOutputTypeDef,
     ListStackSetsOutputTypeDef,
     ListStacksOutputTypeDef,
     ListTypeRegistrationsOutputTypeDef,
@@ -115,14 +116,15 @@
     ResourceToImportTypeDef,
     RollbackConfigurationTypeDef,
     RollbackStackOutputTypeDef,
     SetTypeConfigurationOutputTypeDef,
     StackInstanceFilterTypeDef,
     StackSetOperationPreferencesTypeDef,
     TagTypeDef,
+    TemplateSummaryConfigTypeDef,
     TestTypeOutputTypeDef,
     TypeConfigurationIdentifierTypeDef,
     TypeFiltersTypeDef,
     UpdateStackInstancesOutputTypeDef,
     UpdateStackOutputTypeDef,
     UpdateStackSetOutputTypeDef,
     UpdateTerminationProtectionOutputTypeDef,
@@ -314,15 +316,16 @@
         ResourceTypes: Sequence[str] = ...,
         RoleARN: str = ...,
         OnFailure: OnFailureType = ...,
         StackPolicyBody: str = ...,
         StackPolicyURL: str = ...,
         Tags: Sequence[TagTypeDef] = ...,
         ClientRequestToken: str = ...,
-        EnableTerminationProtection: bool = ...
+        EnableTerminationProtection: bool = ...,
+        RetainExceptOnCreate: bool = ...
     ) -> CreateStackOutputTypeDef:
         """
         Creates a stack as specified in the template.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudformation.html#CloudFormation.Client.create_stack)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudformation/client/#create_stack)
         """
@@ -677,15 +680,16 @@
         """
     async def execute_change_set(
         self,
         *,
         ChangeSetName: str,
         StackName: str = ...,
         ClientRequestToken: str = ...,
-        DisableRollback: bool = ...
+        DisableRollback: bool = ...,
+        RetainExceptOnCreate: bool = ...
     ) -> Dict[str, Any]:
         """
         Updates a stack using the input information that was provided when the specified
         change set was created.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudformation.html#CloudFormation.Client.execute_change_set)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudformation/client/#execute_change_set)
@@ -726,15 +730,16 @@
     async def get_template_summary(
         self,
         *,
         TemplateBody: str = ...,
         TemplateURL: str = ...,
         StackName: str = ...,
         StackSetName: str = ...,
-        CallAs: CallAsType = ...
+        CallAs: CallAsType = ...,
+        TemplateSummaryConfig: TemplateSummaryConfigTypeDef = ...
     ) -> GetTemplateSummaryOutputTypeDef:
         """
         Returns information about a new or existing template.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudformation.html#CloudFormation.Client.get_template_summary)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudformation/client/#get_template_summary)
         """
@@ -777,14 +782,32 @@
     ) -> ListImportsOutputTypeDef:
         """
         Lists all stacks that are importing an exported output value.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudformation.html#CloudFormation.Client.list_imports)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudformation/client/#list_imports)
         """
+    async def list_stack_instance_resource_drifts(
+        self,
+        *,
+        StackSetName: str,
+        StackInstanceAccount: str,
+        StackInstanceRegion: str,
+        OperationId: str,
+        NextToken: str = ...,
+        MaxResults: int = ...,
+        StackInstanceResourceDriftStatuses: Sequence[StackResourceDriftStatusType] = ...,
+        CallAs: CallAsType = ...
+    ) -> ListStackInstanceResourceDriftsOutputTypeDef:
+        """
+        Returns drift information for resources in a stack instance.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudformation.html#CloudFormation.Client.list_stack_instance_resource_drifts)
+        [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudformation/client/#list_stack_instance_resource_drifts)
+        """
     async def list_stack_instances(
         self,
         *,
         StackSetName: str,
         NextToken: str = ...,
         MaxResults: int = ...,
         Filters: Sequence[StackInstanceFilterTypeDef] = ...,
@@ -968,15 +991,20 @@
         """
         Registers an extension with the CloudFormation service.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudformation.html#CloudFormation.Client.register_type)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudformation/client/#register_type)
         """
     async def rollback_stack(
-        self, *, StackName: str, RoleARN: str = ..., ClientRequestToken: str = ...
+        self,
+        *,
+        StackName: str,
+        RoleARN: str = ...,
+        ClientRequestToken: str = ...,
+        RetainExceptOnCreate: bool = ...
     ) -> RollbackStackOutputTypeDef:
         """
         When specifying `RollbackStack`, you preserve the state of previously
         provisioned resources when an operation fails.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudformation.html#CloudFormation.Client.rollback_stack)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudformation/client/#rollback_stack)
@@ -1075,15 +1103,16 @@
         RoleARN: str = ...,
         RollbackConfiguration: RollbackConfigurationTypeDef = ...,
         StackPolicyBody: str = ...,
         StackPolicyURL: str = ...,
         NotificationARNs: Sequence[str] = ...,
         Tags: Sequence[TagTypeDef] = ...,
         DisableRollback: bool = ...,
-        ClientRequestToken: str = ...
+        ClientRequestToken: str = ...,
+        RetainExceptOnCreate: bool = ...
     ) -> UpdateStackOutputTypeDef:
         """
         Updates a stack as specified in the template.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudformation.html#CloudFormation.Client.update_stack)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudformation/client/#update_stack)
         """
```

### Comparing `types-aiobotocore-cloudformation-2.5.2.post3/types_aiobotocore_cloudformation/literals.py` & `types-aiobotocore-cloudformation-2.5.4/types_aiobotocore_cloudformation/literals.py`

 * *Files 1% similar despite different names*

```diff
@@ -240,15 +240,15 @@
     "FAILED",
     "INOPERABLE",
     "PENDING",
     "RUNNING",
     "SKIPPED_SUSPENDED_ACCOUNT",
     "SUCCEEDED",
 ]
-StackInstanceFilterNameType = Literal["DETAILED_STATUS", "LAST_OPERATION_ID"]
+StackInstanceFilterNameType = Literal["DETAILED_STATUS", "DRIFT_STATUS", "LAST_OPERATION_ID"]
 StackInstanceStatusType = Literal["CURRENT", "INOPERABLE", "OUTDATED"]
 StackResourceDriftStatusType = Literal["DELETED", "IN_SYNC", "MODIFIED", "NOT_CHECKED"]
 StackRollbackCompleteWaiterName = Literal["stack_rollback_complete"]
 StackSetDriftDetectionStatusType = Literal[
     "COMPLETED", "FAILED", "IN_PROGRESS", "PARTIAL_SUCCESS", "STOPPED"
 ]
 StackSetDriftStatusType = Literal["DRIFTED", "IN_SYNC", "NOT_CHECKED"]
@@ -304,14 +304,15 @@
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
@@ -407,14 +408,15 @@
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
@@ -493,26 +495,28 @@
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
@@ -699,14 +703,15 @@
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

### Comparing `types-aiobotocore-cloudformation-2.5.2.post3/types_aiobotocore_cloudformation/literals.pyi` & `types-aiobotocore-cloudformation-2.5.4/types_aiobotocore_cloudformation/literals.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -238,15 +238,15 @@
     "FAILED",
     "INOPERABLE",
     "PENDING",
     "RUNNING",
     "SKIPPED_SUSPENDED_ACCOUNT",
     "SUCCEEDED",
 ]
-StackInstanceFilterNameType = Literal["DETAILED_STATUS", "LAST_OPERATION_ID"]
+StackInstanceFilterNameType = Literal["DETAILED_STATUS", "DRIFT_STATUS", "LAST_OPERATION_ID"]
 StackInstanceStatusType = Literal["CURRENT", "INOPERABLE", "OUTDATED"]
 StackResourceDriftStatusType = Literal["DELETED", "IN_SYNC", "MODIFIED", "NOT_CHECKED"]
 StackRollbackCompleteWaiterName = Literal["stack_rollback_complete"]
 StackSetDriftDetectionStatusType = Literal[
     "COMPLETED", "FAILED", "IN_PROGRESS", "PARTIAL_SUCCESS", "STOPPED"
 ]
 StackSetDriftStatusType = Literal["DRIFTED", "IN_SYNC", "NOT_CHECKED"]
@@ -302,14 +302,15 @@
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
@@ -405,14 +406,15 @@
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
@@ -491,26 +493,28 @@
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
@@ -697,14 +701,15 @@
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

### Comparing `types-aiobotocore-cloudformation-2.5.2.post3/types_aiobotocore_cloudformation/paginator.py` & `types-aiobotocore-cloudformation-2.5.4/types_aiobotocore_cloudformation/paginator.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-cloudformation-2.5.2.post3/types_aiobotocore_cloudformation/paginator.pyi` & `types-aiobotocore-cloudformation-2.5.4/types_aiobotocore_cloudformation/paginator.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-cloudformation-2.5.2.post3/types_aiobotocore_cloudformation/service_resource.py` & `types-aiobotocore-cloudformation-2.5.4/types_aiobotocore_cloudformation/service_resource.py`

 * *Files 2% similar despite different names*

```diff
@@ -279,14 +279,15 @@
     outputs: Awaitable[List[OutputTypeDef]]
     role_arn: Awaitable[str]
     tags: Awaitable[List[TagTypeDef]]
     enable_termination_protection: Awaitable[bool]
     parent_id: Awaitable[str]
     root_id: Awaitable[str]
     drift_information: Awaitable[StackDriftInformationResponseTypeDef]
+    retain_except_on_create: Awaitable[bool]
     name: str
     events: StackEventsCollection
     resource_summaries: StackResourceSummariesCollection
 
     async def Resource(self, logical_id: str) -> "_StackResource":
         """
         Creates a StackResource resource.
@@ -357,15 +358,16 @@
         RoleARN: str = ...,
         RollbackConfiguration: RollbackConfigurationTypeDef = ...,
         StackPolicyBody: str = ...,
         StackPolicyURL: str = ...,
         NotificationARNs: Sequence[str] = ...,
         Tags: Sequence[TagTypeDef] = ...,
         DisableRollback: bool = ...,
-        ClientRequestToken: str = ...
+        ClientRequestToken: str = ...,
+        RetainExceptOnCreate: bool = ...
     ) -> UpdateStackOutputTypeDef:
         """
         Updates a stack as specified in the template.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudformation.html#CloudFormation.Stack.update)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudformation/service_resource/#stackupdate-method)
         """
@@ -529,15 +531,16 @@
         ResourceTypes: Sequence[str] = ...,
         RoleARN: str = ...,
         OnFailure: OnFailureType = ...,
         StackPolicyBody: str = ...,
         StackPolicyURL: str = ...,
         Tags: Sequence[TagTypeDef] = ...,
         ClientRequestToken: str = ...,
-        EnableTerminationProtection: bool = ...
+        EnableTerminationProtection: bool = ...,
+        RetainExceptOnCreate: bool = ...
     ) -> _Stack:
         """
         Creates a stack as specified in the template.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudformation.html#CloudFormation.ServiceResource.create_stack)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudformation/service_resource/#cloudformationserviceresourcecreate_stack-method)
         """
```

### Comparing `types-aiobotocore-cloudformation-2.5.2.post3/types_aiobotocore_cloudformation/service_resource.pyi` & `types-aiobotocore-cloudformation-2.5.4/types_aiobotocore_cloudformation/service_resource.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -254,14 +254,15 @@
     outputs: Awaitable[List[OutputTypeDef]]
     role_arn: Awaitable[str]
     tags: Awaitable[List[TagTypeDef]]
     enable_termination_protection: Awaitable[bool]
     parent_id: Awaitable[str]
     root_id: Awaitable[str]
     drift_information: Awaitable[StackDriftInformationResponseTypeDef]
+    retain_except_on_create: Awaitable[bool]
     name: str
     events: StackEventsCollection
     resource_summaries: StackResourceSummariesCollection
 
     async def Resource(self, logical_id: str) -> "_StackResource":
         """
         Creates a StackResource resource.
@@ -326,15 +327,16 @@
         RoleARN: str = ...,
         RollbackConfiguration: RollbackConfigurationTypeDef = ...,
         StackPolicyBody: str = ...,
         StackPolicyURL: str = ...,
         NotificationARNs: Sequence[str] = ...,
         Tags: Sequence[TagTypeDef] = ...,
         DisableRollback: bool = ...,
-        ClientRequestToken: str = ...
+        ClientRequestToken: str = ...,
+        RetainExceptOnCreate: bool = ...
     ) -> UpdateStackOutputTypeDef:
         """
         Updates a stack as specified in the template.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudformation.html#CloudFormation.Stack.update)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudformation/service_resource/#stackupdate-method)
         """
@@ -483,15 +485,16 @@
         ResourceTypes: Sequence[str] = ...,
         RoleARN: str = ...,
         OnFailure: OnFailureType = ...,
         StackPolicyBody: str = ...,
         StackPolicyURL: str = ...,
         Tags: Sequence[TagTypeDef] = ...,
         ClientRequestToken: str = ...,
-        EnableTerminationProtection: bool = ...
+        EnableTerminationProtection: bool = ...,
+        RetainExceptOnCreate: bool = ...
     ) -> _Stack:
         """
         Creates a stack as specified in the template.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudformation.html#CloudFormation.ServiceResource.create_stack)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudformation/service_resource/#cloudformationserviceresourcecreate_stack-method)
         """
```

### Comparing `types-aiobotocore-cloudformation-2.5.2.post3/types_aiobotocore_cloudformation/type_defs.py` & `types-aiobotocore-cloudformation-2.5.4/types_aiobotocore_cloudformation/type_defs.py`

 * *Files 2% similar despite different names*

```diff
@@ -126,19 +126,21 @@
     "DescribeTypeRegistrationInputRequestTypeDef",
     "DetectStackDriftInputRequestTypeDef",
     "DetectStackResourceDriftInputRequestTypeDef",
     "ExecuteChangeSetInputRequestTypeDef",
     "ExportTypeDef",
     "GetStackPolicyInputRequestTypeDef",
     "GetTemplateInputRequestTypeDef",
-    "GetTemplateSummaryInputRequestTypeDef",
+    "TemplateSummaryConfigTypeDef",
     "ResourceIdentifierSummaryTypeDef",
+    "WarningsTypeDef",
     "ListChangeSetsInputRequestTypeDef",
     "ListExportsInputRequestTypeDef",
     "ListImportsInputRequestTypeDef",
+    "ListStackInstanceResourceDriftsInputRequestTypeDef",
     "StackInstanceFilterTypeDef",
     "ListStackResourcesInputRequestTypeDef",
     "OperationResultFilterTypeDef",
     "ListStackSetOperationsInputRequestTypeDef",
     "ListStackSetsInputRequestTypeDef",
     "ListStacksInputRequestTypeDef",
     "ListTypeRegistrationsInputRequestTypeDef",
@@ -242,23 +244,25 @@
     "DescribeStacksInputStackImportCompleteWaitTypeDef",
     "DescribeStacksInputStackRollbackCompleteWaitTypeDef",
     "DescribeStacksInputStackUpdateCompleteWaitTypeDef",
     "DescribeTypeRegistrationInputTypeRegistrationCompleteWaitTypeDef",
     "DescribeStackEventsOutputTypeDef",
     "DescribeTypeOutputTypeDef",
     "ListExportsOutputTypeDef",
+    "GetTemplateSummaryInputRequestTypeDef",
     "ListStackInstancesInputListStackInstancesPaginateTypeDef",
     "ListStackInstancesInputRequestTypeDef",
     "ListStackSetOperationResultsInputListStackSetOperationResultsPaginateTypeDef",
     "ListStackSetOperationResultsInputRequestTypeDef",
     "ListTypeVersionsOutputTypeDef",
     "ListTypesInputListTypesPaginateTypeDef",
     "ListTypesInputRequestTypeDef",
     "ListTypesOutputTypeDef",
     "ParameterDeclarationTypeDef",
+    "StackInstanceResourceDriftsSummaryTypeDef",
     "ResourceChangeDetailTypeDef",
     "RollbackConfigurationResponseTypeDef",
     "RollbackConfigurationStackResourceSummaryTypeDef",
     "RollbackConfigurationTypeDef",
     "StackSummaryTypeDef",
     "StackInstanceSummaryTypeDef",
     "StackInstanceTypeDef",
@@ -272,14 +276,15 @@
     "StackResourceDriftTypeDef",
     "StackResourceSummaryTypeDef",
     "StackResourceTypeDef",
     "BatchDescribeTypeConfigurationsOutputTypeDef",
     "ChangeSetHookTypeDef",
     "ListStackSetsOutputTypeDef",
     "GetTemplateSummaryOutputTypeDef",
+    "ListStackInstanceResourceDriftsOutputTypeDef",
     "ResourceChangeTypeDef",
     "StackStackResourceSummaryTypeDef",
     "CreateChangeSetInputRequestTypeDef",
     "CreateStackInputRequestTypeDef",
     "CreateStackInputServiceResourceCreateStackTypeDef",
     "StackTypeDef",
     "UpdateStackInputRequestTypeDef",
@@ -939,14 +944,15 @@
 )
 _OptionalExecuteChangeSetInputRequestTypeDef = TypedDict(
     "_OptionalExecuteChangeSetInputRequestTypeDef",
     {
         "StackName": str,
         "ClientRequestToken": str,
         "DisableRollback": bool,
+        "RetainExceptOnCreate": bool,
     },
     total=False,
 )
 
 
 class ExecuteChangeSetInputRequestTypeDef(
     _RequiredExecuteChangeSetInputRequestTypeDef, _OptionalExecuteChangeSetInputRequestTypeDef
@@ -977,36 +983,40 @@
         "StackName": str,
         "ChangeSetName": str,
         "TemplateStage": TemplateStageType,
     },
     total=False,
 )
 
-GetTemplateSummaryInputRequestTypeDef = TypedDict(
-    "GetTemplateSummaryInputRequestTypeDef",
+TemplateSummaryConfigTypeDef = TypedDict(
+    "TemplateSummaryConfigTypeDef",
     {
-        "TemplateBody": str,
-        "TemplateURL": str,
-        "StackName": str,
-        "StackSetName": str,
-        "CallAs": CallAsType,
+        "TreatUnrecognizedResourceTypesAsWarnings": bool,
     },
     total=False,
 )
 
 ResourceIdentifierSummaryTypeDef = TypedDict(
     "ResourceIdentifierSummaryTypeDef",
     {
         "ResourceType": str,
         "LogicalResourceIds": List[str],
         "ResourceIdentifiers": List[str],
     },
     total=False,
 )
 
+WarningsTypeDef = TypedDict(
+    "WarningsTypeDef",
+    {
+        "UnrecognizedResourceTypes": List[str],
+    },
+    total=False,
+)
+
 _RequiredListChangeSetsInputRequestTypeDef = TypedDict(
     "_RequiredListChangeSetsInputRequestTypeDef",
     {
         "StackName": str,
     },
 )
 _OptionalListChangeSetsInputRequestTypeDef = TypedDict(
@@ -1049,14 +1059,42 @@
 
 class ListImportsInputRequestTypeDef(
     _RequiredListImportsInputRequestTypeDef, _OptionalListImportsInputRequestTypeDef
 ):
     pass
 
 
+_RequiredListStackInstanceResourceDriftsInputRequestTypeDef = TypedDict(
+    "_RequiredListStackInstanceResourceDriftsInputRequestTypeDef",
+    {
+        "StackSetName": str,
+        "StackInstanceAccount": str,
+        "StackInstanceRegion": str,
+        "OperationId": str,
+    },
+)
+_OptionalListStackInstanceResourceDriftsInputRequestTypeDef = TypedDict(
+    "_OptionalListStackInstanceResourceDriftsInputRequestTypeDef",
+    {
+        "NextToken": str,
+        "MaxResults": int,
+        "StackInstanceResourceDriftStatuses": Sequence[StackResourceDriftStatusType],
+        "CallAs": CallAsType,
+    },
+    total=False,
+)
+
+
+class ListStackInstanceResourceDriftsInputRequestTypeDef(
+    _RequiredListStackInstanceResourceDriftsInputRequestTypeDef,
+    _OptionalListStackInstanceResourceDriftsInputRequestTypeDef,
+):
+    pass
+
+
 StackInstanceFilterTypeDef = TypedDict(
     "StackInstanceFilterTypeDef",
     {
         "Name": StackInstanceFilterNameType,
         "Values": str,
     },
     total=False,
@@ -1317,14 +1355,15 @@
     },
 )
 _OptionalRollbackStackInputRequestTypeDef = TypedDict(
     "_OptionalRollbackStackInputRequestTypeDef",
     {
         "RoleARN": str,
         "ClientRequestToken": str,
+        "RetainExceptOnCreate": bool,
     },
     total=False,
 )
 
 
 class RollbackStackInputRequestTypeDef(
     _RequiredRollbackStackInputRequestTypeDef, _OptionalRollbackStackInputRequestTypeDef
@@ -2534,14 +2573,27 @@
     {
         "Exports": List[ExportTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+GetTemplateSummaryInputRequestTypeDef = TypedDict(
+    "GetTemplateSummaryInputRequestTypeDef",
+    {
+        "TemplateBody": str,
+        "TemplateURL": str,
+        "StackName": str,
+        "StackSetName": str,
+        "CallAs": CallAsType,
+        "TemplateSummaryConfig": TemplateSummaryConfigTypeDef,
+    },
+    total=False,
+)
+
 _RequiredListStackInstancesInputListStackInstancesPaginateTypeDef = TypedDict(
     "_RequiredListStackInstancesInputListStackInstancesPaginateTypeDef",
     {
         "StackSetName": str,
     },
 )
 _OptionalListStackInstancesInputListStackInstancesPaginateTypeDef = TypedDict(
@@ -2695,14 +2747,42 @@
         "NoEcho": bool,
         "Description": str,
         "ParameterConstraints": ParameterConstraintsTypeDef,
     },
     total=False,
 )
 
+_RequiredStackInstanceResourceDriftsSummaryTypeDef = TypedDict(
+    "_RequiredStackInstanceResourceDriftsSummaryTypeDef",
+    {
+        "StackId": str,
+        "LogicalResourceId": str,
+        "ResourceType": str,
+        "StackResourceDriftStatus": StackResourceDriftStatusType,
+        "Timestamp": datetime,
+    },
+)
+_OptionalStackInstanceResourceDriftsSummaryTypeDef = TypedDict(
+    "_OptionalStackInstanceResourceDriftsSummaryTypeDef",
+    {
+        "PhysicalResourceId": str,
+        "PhysicalResourceIdContext": List[PhysicalResourceIdContextKeyValuePairTypeDef],
+        "PropertyDifferences": List[PropertyDifferenceTypeDef],
+    },
+    total=False,
+)
+
+
+class StackInstanceResourceDriftsSummaryTypeDef(
+    _RequiredStackInstanceResourceDriftsSummaryTypeDef,
+    _OptionalStackInstanceResourceDriftsSummaryTypeDef,
+):
+    pass
+
+
 ResourceChangeDetailTypeDef = TypedDict(
     "ResourceChangeDetailTypeDef",
     {
         "Target": ResourceTargetDefinitionTypeDef,
         "Evaluation": EvaluationTypeType,
         "ChangeSource": ChangeSourceType,
         "CausingEntity": str,
@@ -3054,14 +3134,24 @@
         "Capabilities": List[CapabilityType],
         "CapabilitiesReason": str,
         "ResourceTypes": List[str],
         "Version": str,
         "Metadata": str,
         "DeclaredTransforms": List[str],
         "ResourceIdentifierSummaries": List[ResourceIdentifierSummaryTypeDef],
+        "Warnings": WarningsTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListStackInstanceResourceDriftsOutputTypeDef = TypedDict(
+    "ListStackInstanceResourceDriftsOutputTypeDef",
+    {
+        "Summaries": List[StackInstanceResourceDriftsSummaryTypeDef],
+        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ResourceChangeTypeDef = TypedDict(
     "ResourceChangeTypeDef",
     {
@@ -3104,14 +3194,15 @@
         "Outputs": List[OutputTypeDef],
         "RoleARN": str,
         "Tags": List[TagTypeDef],
         "EnableTerminationProtection": bool,
         "ParentId": str,
         "RootId": str,
         "DriftInformation": StackDriftInformationTypeDef,
+        "RetainExceptOnCreate": bool,
     },
     total=False,
 )
 
 
 class StackStackResourceSummaryTypeDef(
     _RequiredStackStackResourceSummaryTypeDef, _OptionalStackStackResourceSummaryTypeDef
@@ -3177,14 +3268,15 @@
         "RoleARN": str,
         "OnFailure": OnFailureType,
         "StackPolicyBody": str,
         "StackPolicyURL": str,
         "Tags": Sequence[TagTypeDef],
         "ClientRequestToken": str,
         "EnableTerminationProtection": bool,
+        "RetainExceptOnCreate": bool,
     },
     total=False,
 )
 
 
 class CreateStackInputRequestTypeDef(
     _RequiredCreateStackInputRequestTypeDef, _OptionalCreateStackInputRequestTypeDef
@@ -3213,14 +3305,15 @@
         "RoleARN": str,
         "OnFailure": OnFailureType,
         "StackPolicyBody": str,
         "StackPolicyURL": str,
         "Tags": Sequence[TagTypeDef],
         "ClientRequestToken": str,
         "EnableTerminationProtection": bool,
+        "RetainExceptOnCreate": bool,
     },
     total=False,
 )
 
 
 class CreateStackInputServiceResourceCreateStackTypeDef(
     _RequiredCreateStackInputServiceResourceCreateStackTypeDef,
@@ -3255,14 +3348,15 @@
         "Outputs": List[OutputTypeDef],
         "RoleARN": str,
         "Tags": List[TagTypeDef],
         "EnableTerminationProtection": bool,
         "ParentId": str,
         "RootId": str,
         "DriftInformation": StackDriftInformationTypeDef,
+        "RetainExceptOnCreate": bool,
     },
     total=False,
 )
 
 
 class StackTypeDef(_RequiredStackTypeDef, _OptionalStackTypeDef):
     pass
@@ -3289,14 +3383,15 @@
         "RollbackConfiguration": RollbackConfigurationTypeDef,
         "StackPolicyBody": str,
         "StackPolicyURL": str,
         "NotificationARNs": Sequence[str],
         "Tags": Sequence[TagTypeDef],
         "DisableRollback": bool,
         "ClientRequestToken": str,
+        "RetainExceptOnCreate": bool,
     },
     total=False,
 )
 
 
 class UpdateStackInputRequestTypeDef(
     _RequiredUpdateStackInputRequestTypeDef, _OptionalUpdateStackInputRequestTypeDef
@@ -3319,14 +3414,15 @@
         "RollbackConfiguration": RollbackConfigurationTypeDef,
         "StackPolicyBody": str,
         "StackPolicyURL": str,
         "NotificationARNs": Sequence[str],
         "Tags": Sequence[TagTypeDef],
         "DisableRollback": bool,
         "ClientRequestToken": str,
+        "RetainExceptOnCreate": bool,
     },
     total=False,
 )
 
 ListStacksOutputTypeDef = TypedDict(
     "ListStacksOutputTypeDef",
     {
```

### Comparing `types-aiobotocore-cloudformation-2.5.2.post3/types_aiobotocore_cloudformation/type_defs.pyi` & `types-aiobotocore-cloudformation-2.5.4/types_aiobotocore_cloudformation/type_defs.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -125,19 +125,21 @@
     "DescribeTypeRegistrationInputRequestTypeDef",
     "DetectStackDriftInputRequestTypeDef",
     "DetectStackResourceDriftInputRequestTypeDef",
     "ExecuteChangeSetInputRequestTypeDef",
     "ExportTypeDef",
     "GetStackPolicyInputRequestTypeDef",
     "GetTemplateInputRequestTypeDef",
-    "GetTemplateSummaryInputRequestTypeDef",
+    "TemplateSummaryConfigTypeDef",
     "ResourceIdentifierSummaryTypeDef",
+    "WarningsTypeDef",
     "ListChangeSetsInputRequestTypeDef",
     "ListExportsInputRequestTypeDef",
     "ListImportsInputRequestTypeDef",
+    "ListStackInstanceResourceDriftsInputRequestTypeDef",
     "StackInstanceFilterTypeDef",
     "ListStackResourcesInputRequestTypeDef",
     "OperationResultFilterTypeDef",
     "ListStackSetOperationsInputRequestTypeDef",
     "ListStackSetsInputRequestTypeDef",
     "ListStacksInputRequestTypeDef",
     "ListTypeRegistrationsInputRequestTypeDef",
@@ -241,23 +243,25 @@
     "DescribeStacksInputStackImportCompleteWaitTypeDef",
     "DescribeStacksInputStackRollbackCompleteWaitTypeDef",
     "DescribeStacksInputStackUpdateCompleteWaitTypeDef",
     "DescribeTypeRegistrationInputTypeRegistrationCompleteWaitTypeDef",
     "DescribeStackEventsOutputTypeDef",
     "DescribeTypeOutputTypeDef",
     "ListExportsOutputTypeDef",
+    "GetTemplateSummaryInputRequestTypeDef",
     "ListStackInstancesInputListStackInstancesPaginateTypeDef",
     "ListStackInstancesInputRequestTypeDef",
     "ListStackSetOperationResultsInputListStackSetOperationResultsPaginateTypeDef",
     "ListStackSetOperationResultsInputRequestTypeDef",
     "ListTypeVersionsOutputTypeDef",
     "ListTypesInputListTypesPaginateTypeDef",
     "ListTypesInputRequestTypeDef",
     "ListTypesOutputTypeDef",
     "ParameterDeclarationTypeDef",
+    "StackInstanceResourceDriftsSummaryTypeDef",
     "ResourceChangeDetailTypeDef",
     "RollbackConfigurationResponseTypeDef",
     "RollbackConfigurationStackResourceSummaryTypeDef",
     "RollbackConfigurationTypeDef",
     "StackSummaryTypeDef",
     "StackInstanceSummaryTypeDef",
     "StackInstanceTypeDef",
@@ -271,14 +275,15 @@
     "StackResourceDriftTypeDef",
     "StackResourceSummaryTypeDef",
     "StackResourceTypeDef",
     "BatchDescribeTypeConfigurationsOutputTypeDef",
     "ChangeSetHookTypeDef",
     "ListStackSetsOutputTypeDef",
     "GetTemplateSummaryOutputTypeDef",
+    "ListStackInstanceResourceDriftsOutputTypeDef",
     "ResourceChangeTypeDef",
     "StackStackResourceSummaryTypeDef",
     "CreateChangeSetInputRequestTypeDef",
     "CreateStackInputRequestTypeDef",
     "CreateStackInputServiceResourceCreateStackTypeDef",
     "StackTypeDef",
     "UpdateStackInputRequestTypeDef",
@@ -912,14 +917,15 @@
 )
 _OptionalExecuteChangeSetInputRequestTypeDef = TypedDict(
     "_OptionalExecuteChangeSetInputRequestTypeDef",
     {
         "StackName": str,
         "ClientRequestToken": str,
         "DisableRollback": bool,
+        "RetainExceptOnCreate": bool,
     },
     total=False,
 )
 
 class ExecuteChangeSetInputRequestTypeDef(
     _RequiredExecuteChangeSetInputRequestTypeDef, _OptionalExecuteChangeSetInputRequestTypeDef
 ):
@@ -948,36 +954,40 @@
         "StackName": str,
         "ChangeSetName": str,
         "TemplateStage": TemplateStageType,
     },
     total=False,
 )
 
-GetTemplateSummaryInputRequestTypeDef = TypedDict(
-    "GetTemplateSummaryInputRequestTypeDef",
+TemplateSummaryConfigTypeDef = TypedDict(
+    "TemplateSummaryConfigTypeDef",
     {
-        "TemplateBody": str,
-        "TemplateURL": str,
-        "StackName": str,
-        "StackSetName": str,
-        "CallAs": CallAsType,
+        "TreatUnrecognizedResourceTypesAsWarnings": bool,
     },
     total=False,
 )
 
 ResourceIdentifierSummaryTypeDef = TypedDict(
     "ResourceIdentifierSummaryTypeDef",
     {
         "ResourceType": str,
         "LogicalResourceIds": List[str],
         "ResourceIdentifiers": List[str],
     },
     total=False,
 )
 
+WarningsTypeDef = TypedDict(
+    "WarningsTypeDef",
+    {
+        "UnrecognizedResourceTypes": List[str],
+    },
+    total=False,
+)
+
 _RequiredListChangeSetsInputRequestTypeDef = TypedDict(
     "_RequiredListChangeSetsInputRequestTypeDef",
     {
         "StackName": str,
     },
 )
 _OptionalListChangeSetsInputRequestTypeDef = TypedDict(
@@ -1016,14 +1026,40 @@
 )
 
 class ListImportsInputRequestTypeDef(
     _RequiredListImportsInputRequestTypeDef, _OptionalListImportsInputRequestTypeDef
 ):
     pass
 
+_RequiredListStackInstanceResourceDriftsInputRequestTypeDef = TypedDict(
+    "_RequiredListStackInstanceResourceDriftsInputRequestTypeDef",
+    {
+        "StackSetName": str,
+        "StackInstanceAccount": str,
+        "StackInstanceRegion": str,
+        "OperationId": str,
+    },
+)
+_OptionalListStackInstanceResourceDriftsInputRequestTypeDef = TypedDict(
+    "_OptionalListStackInstanceResourceDriftsInputRequestTypeDef",
+    {
+        "NextToken": str,
+        "MaxResults": int,
+        "StackInstanceResourceDriftStatuses": Sequence[StackResourceDriftStatusType],
+        "CallAs": CallAsType,
+    },
+    total=False,
+)
+
+class ListStackInstanceResourceDriftsInputRequestTypeDef(
+    _RequiredListStackInstanceResourceDriftsInputRequestTypeDef,
+    _OptionalListStackInstanceResourceDriftsInputRequestTypeDef,
+):
+    pass
+
 StackInstanceFilterTypeDef = TypedDict(
     "StackInstanceFilterTypeDef",
     {
         "Name": StackInstanceFilterNameType,
         "Values": str,
     },
     total=False,
@@ -1278,14 +1314,15 @@
     },
 )
 _OptionalRollbackStackInputRequestTypeDef = TypedDict(
     "_OptionalRollbackStackInputRequestTypeDef",
     {
         "RoleARN": str,
         "ClientRequestToken": str,
+        "RetainExceptOnCreate": bool,
     },
     total=False,
 )
 
 class RollbackStackInputRequestTypeDef(
     _RequiredRollbackStackInputRequestTypeDef, _OptionalRollbackStackInputRequestTypeDef
 ):
@@ -2449,14 +2486,27 @@
     {
         "Exports": List[ExportTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+GetTemplateSummaryInputRequestTypeDef = TypedDict(
+    "GetTemplateSummaryInputRequestTypeDef",
+    {
+        "TemplateBody": str,
+        "TemplateURL": str,
+        "StackName": str,
+        "StackSetName": str,
+        "CallAs": CallAsType,
+        "TemplateSummaryConfig": TemplateSummaryConfigTypeDef,
+    },
+    total=False,
+)
+
 _RequiredListStackInstancesInputListStackInstancesPaginateTypeDef = TypedDict(
     "_RequiredListStackInstancesInputListStackInstancesPaginateTypeDef",
     {
         "StackSetName": str,
     },
 )
 _OptionalListStackInstancesInputListStackInstancesPaginateTypeDef = TypedDict(
@@ -2602,14 +2652,40 @@
         "NoEcho": bool,
         "Description": str,
         "ParameterConstraints": ParameterConstraintsTypeDef,
     },
     total=False,
 )
 
+_RequiredStackInstanceResourceDriftsSummaryTypeDef = TypedDict(
+    "_RequiredStackInstanceResourceDriftsSummaryTypeDef",
+    {
+        "StackId": str,
+        "LogicalResourceId": str,
+        "ResourceType": str,
+        "StackResourceDriftStatus": StackResourceDriftStatusType,
+        "Timestamp": datetime,
+    },
+)
+_OptionalStackInstanceResourceDriftsSummaryTypeDef = TypedDict(
+    "_OptionalStackInstanceResourceDriftsSummaryTypeDef",
+    {
+        "PhysicalResourceId": str,
+        "PhysicalResourceIdContext": List[PhysicalResourceIdContextKeyValuePairTypeDef],
+        "PropertyDifferences": List[PropertyDifferenceTypeDef],
+    },
+    total=False,
+)
+
+class StackInstanceResourceDriftsSummaryTypeDef(
+    _RequiredStackInstanceResourceDriftsSummaryTypeDef,
+    _OptionalStackInstanceResourceDriftsSummaryTypeDef,
+):
+    pass
+
 ResourceChangeDetailTypeDef = TypedDict(
     "ResourceChangeDetailTypeDef",
     {
         "Target": ResourceTargetDefinitionTypeDef,
         "Evaluation": EvaluationTypeType,
         "ChangeSource": ChangeSourceType,
         "CausingEntity": str,
@@ -2951,14 +3027,24 @@
         "Capabilities": List[CapabilityType],
         "CapabilitiesReason": str,
         "ResourceTypes": List[str],
         "Version": str,
         "Metadata": str,
         "DeclaredTransforms": List[str],
         "ResourceIdentifierSummaries": List[ResourceIdentifierSummaryTypeDef],
+        "Warnings": WarningsTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListStackInstanceResourceDriftsOutputTypeDef = TypedDict(
+    "ListStackInstanceResourceDriftsOutputTypeDef",
+    {
+        "Summaries": List[StackInstanceResourceDriftsSummaryTypeDef],
+        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ResourceChangeTypeDef = TypedDict(
     "ResourceChangeTypeDef",
     {
@@ -3001,14 +3087,15 @@
         "Outputs": List[OutputTypeDef],
         "RoleARN": str,
         "Tags": List[TagTypeDef],
         "EnableTerminationProtection": bool,
         "ParentId": str,
         "RootId": str,
         "DriftInformation": StackDriftInformationTypeDef,
+        "RetainExceptOnCreate": bool,
     },
     total=False,
 )
 
 class StackStackResourceSummaryTypeDef(
     _RequiredStackStackResourceSummaryTypeDef, _OptionalStackStackResourceSummaryTypeDef
 ):
@@ -3070,14 +3157,15 @@
         "RoleARN": str,
         "OnFailure": OnFailureType,
         "StackPolicyBody": str,
         "StackPolicyURL": str,
         "Tags": Sequence[TagTypeDef],
         "ClientRequestToken": str,
         "EnableTerminationProtection": bool,
+        "RetainExceptOnCreate": bool,
     },
     total=False,
 )
 
 class CreateStackInputRequestTypeDef(
     _RequiredCreateStackInputRequestTypeDef, _OptionalCreateStackInputRequestTypeDef
 ):
@@ -3104,14 +3192,15 @@
         "RoleARN": str,
         "OnFailure": OnFailureType,
         "StackPolicyBody": str,
         "StackPolicyURL": str,
         "Tags": Sequence[TagTypeDef],
         "ClientRequestToken": str,
         "EnableTerminationProtection": bool,
+        "RetainExceptOnCreate": bool,
     },
     total=False,
 )
 
 class CreateStackInputServiceResourceCreateStackTypeDef(
     _RequiredCreateStackInputServiceResourceCreateStackTypeDef,
     _OptionalCreateStackInputServiceResourceCreateStackTypeDef,
@@ -3144,14 +3233,15 @@
         "Outputs": List[OutputTypeDef],
         "RoleARN": str,
         "Tags": List[TagTypeDef],
         "EnableTerminationProtection": bool,
         "ParentId": str,
         "RootId": str,
         "DriftInformation": StackDriftInformationTypeDef,
+        "RetainExceptOnCreate": bool,
     },
     total=False,
 )
 
 class StackTypeDef(_RequiredStackTypeDef, _OptionalStackTypeDef):
     pass
 
@@ -3176,14 +3266,15 @@
         "RollbackConfiguration": RollbackConfigurationTypeDef,
         "StackPolicyBody": str,
         "StackPolicyURL": str,
         "NotificationARNs": Sequence[str],
         "Tags": Sequence[TagTypeDef],
         "DisableRollback": bool,
         "ClientRequestToken": str,
+        "RetainExceptOnCreate": bool,
     },
     total=False,
 )
 
 class UpdateStackInputRequestTypeDef(
     _RequiredUpdateStackInputRequestTypeDef, _OptionalUpdateStackInputRequestTypeDef
 ):
@@ -3204,14 +3295,15 @@
         "RollbackConfiguration": RollbackConfigurationTypeDef,
         "StackPolicyBody": str,
         "StackPolicyURL": str,
         "NotificationARNs": Sequence[str],
         "Tags": Sequence[TagTypeDef],
         "DisableRollback": bool,
         "ClientRequestToken": str,
+        "RetainExceptOnCreate": bool,
     },
     total=False,
 )
 
 ListStacksOutputTypeDef = TypedDict(
     "ListStacksOutputTypeDef",
     {
```

### Comparing `types-aiobotocore-cloudformation-2.5.2.post3/types_aiobotocore_cloudformation/waiter.py` & `types-aiobotocore-cloudformation-2.5.4/types_aiobotocore_cloudformation/waiter.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-cloudformation-2.5.2.post3/types_aiobotocore_cloudformation/waiter.pyi` & `types-aiobotocore-cloudformation-2.5.4/types_aiobotocore_cloudformation/waiter.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-cloudformation-2.5.2.post3/types_aiobotocore_cloudformation.egg-info/PKG-INFO` & `types-aiobotocore-cloudformation-2.5.4/types_aiobotocore_cloudformation.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-cloudformation
-Version: 2.5.2.post3
-Summary: Type annotations for aiobotocore.CloudFormation 2.5.2 service generated with mypy-boto3-builder 7.17.2
+Version: 2.5.4
+Summary: Type annotations for aiobotocore.CloudFormation 2.5.4 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudformation/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-cloudformation.svg?color=blue)](https://pypi.org/project/types-aiobotocore-cloudformation)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudformation/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-cloudformation)](https://pepy.tech/project/types-aiobotocore-cloudformation)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.CloudFormation 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudformation.html#CloudFormation)
+[aiobotocore.CloudFormation 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudformation.html#CloudFormation)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-cloudformation-2.5.2.post3/types_aiobotocore_cloudformation.egg-info/SOURCES.txt` & `types-aiobotocore-cloudformation-2.5.4/types_aiobotocore_cloudformation.egg-info/SOURCES.txt`

 * *Files identical despite different names*


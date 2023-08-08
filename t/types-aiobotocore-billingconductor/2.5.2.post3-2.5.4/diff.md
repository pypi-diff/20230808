# Comparing `tmp/types-aiobotocore-billingconductor-2.5.2.post3.tar.gz` & `tmp/types-aiobotocore-billingconductor-2.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-billingconductor-2.5.2.post3.tar", last modified: Fri Aug  4 12:37:21 2023, max compression
+gzip compressed data, was "types-aiobotocore-billingconductor-2.5.4.tar", last modified: Tue Aug  8 01:23:22 2023, max compression
```

## Comparing `types-aiobotocore-billingconductor-2.5.2.post3.tar` & `types-aiobotocore-billingconductor-2.5.4.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:37:21.495279 types-aiobotocore-billingconductor-2.5.2.post3/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-04 12:19:00.000000 types-aiobotocore-billingconductor-2.5.2.post3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    15323 2023-08-04 12:37:21.491279 types-aiobotocore-billingconductor-2.5.2.post3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    13769 2023-08-04 12:19:00.000000 types-aiobotocore-billingconductor-2.5.2.post3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-04 12:37:21.495279 types-aiobotocore-billingconductor-2.5.2.post3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2135 2023-08-04 12:19:00.000000 types-aiobotocore-billingconductor-2.5.2.post3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:37:21.479279 types-aiobotocore-billingconductor-2.5.2.post3/types_aiobotocore_billingconductor/
--rw-r--r--   0 runner    (1001) docker     (123)     3245 2023-08-04 12:19:00.000000 types-aiobotocore-billingconductor-2.5.2.post3/types_aiobotocore_billingconductor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3244 2023-08-04 12:19:00.000000 types-aiobotocore-billingconductor-2.5.2.post3/types_aiobotocore_billingconductor/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      979 2023-08-04 12:19:00.000000 types-aiobotocore-billingconductor-2.5.2.post3/types_aiobotocore_billingconductor/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    33540 2023-08-04 12:19:00.000000 types-aiobotocore-billingconductor-2.5.2.post3/types_aiobotocore_billingconductor/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    33490 2023-08-04 12:19:00.000000 types-aiobotocore-billingconductor-2.5.2.post3/types_aiobotocore_billingconductor/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    10151 2023-08-04 12:19:01.000000 types-aiobotocore-billingconductor-2.5.2.post3/types_aiobotocore_billingconductor/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    10149 2023-08-04 12:19:01.000000 types-aiobotocore-billingconductor-2.5.2.post3/types_aiobotocore_billingconductor/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    14995 2023-08-04 12:19:00.000000 types-aiobotocore-billingconductor-2.5.2.post3/types_aiobotocore_billingconductor/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)    14983 2023-08-04 12:19:00.000000 types-aiobotocore-billingconductor-2.5.2.post3/types_aiobotocore_billingconductor/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 12:19:00.000000 types-aiobotocore-billingconductor-2.5.2.post3/types_aiobotocore_billingconductor/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    42732 2023-08-04 12:19:01.000000 types-aiobotocore-billingconductor-2.5.2.post3/types_aiobotocore_billingconductor/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    42685 2023-08-04 12:19:01.000000 types-aiobotocore-billingconductor-2.5.2.post3/types_aiobotocore_billingconductor/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-04 12:19:00.000000 types-aiobotocore-billingconductor-2.5.2.post3/types_aiobotocore_billingconductor/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:37:21.491279 types-aiobotocore-billingconductor-2.5.2.post3/types_aiobotocore_billingconductor.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    15323 2023-08-04 12:37:21.000000 types-aiobotocore-billingconductor-2.5.2.post3/types_aiobotocore_billingconductor.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      984 2023-08-04 12:37:21.000000 types-aiobotocore-billingconductor-2.5.2.post3/types_aiobotocore_billingconductor.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 12:37:21.000000 types-aiobotocore-billingconductor-2.5.2.post3/types_aiobotocore_billingconductor.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 12:37:21.000000 types-aiobotocore-billingconductor-2.5.2.post3/types_aiobotocore_billingconductor.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-04 12:37:21.000000 types-aiobotocore-billingconductor-2.5.2.post3/types_aiobotocore_billingconductor.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-08-04 12:37:21.000000 types-aiobotocore-billingconductor-2.5.2.post3/types_aiobotocore_billingconductor.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:23:22.214621 types-aiobotocore-billingconductor-2.5.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-08 01:06:45.000000 types-aiobotocore-billingconductor-2.5.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    15317 2023-08-08 01:23:22.214621 types-aiobotocore-billingconductor-2.5.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    13769 2023-08-08 01:06:45.000000 types-aiobotocore-billingconductor-2.5.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-08 01:23:22.214621 types-aiobotocore-billingconductor-2.5.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2129 2023-08-08 01:06:45.000000 types-aiobotocore-billingconductor-2.5.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:23:22.214621 types-aiobotocore-billingconductor-2.5.4/types_aiobotocore_billingconductor/
+-rw-r--r--   0 runner    (1001) docker     (123)     3245 2023-08-08 01:06:45.000000 types-aiobotocore-billingconductor-2.5.4/types_aiobotocore_billingconductor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3244 2023-08-08 01:06:45.000000 types-aiobotocore-billingconductor-2.5.4/types_aiobotocore_billingconductor/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      967 2023-08-08 01:06:45.000000 types-aiobotocore-billingconductor-2.5.4/types_aiobotocore_billingconductor/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33659 2023-08-08 01:06:46.000000 types-aiobotocore-billingconductor-2.5.4/types_aiobotocore_billingconductor/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33609 2023-08-08 01:06:45.000000 types-aiobotocore-billingconductor-2.5.4/types_aiobotocore_billingconductor/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    10246 2023-08-08 01:06:46.000000 types-aiobotocore-billingconductor-2.5.4/types_aiobotocore_billingconductor/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10244 2023-08-08 01:06:46.000000 types-aiobotocore-billingconductor-2.5.4/types_aiobotocore_billingconductor/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    14995 2023-08-08 01:06:46.000000 types-aiobotocore-billingconductor-2.5.4/types_aiobotocore_billingconductor/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14983 2023-08-08 01:06:46.000000 types-aiobotocore-billingconductor-2.5.4/types_aiobotocore_billingconductor/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 01:06:45.000000 types-aiobotocore-billingconductor-2.5.4/types_aiobotocore_billingconductor/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    43663 2023-08-08 01:06:47.000000 types-aiobotocore-billingconductor-2.5.4/types_aiobotocore_billingconductor/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    43614 2023-08-08 01:06:47.000000 types-aiobotocore-billingconductor-2.5.4/types_aiobotocore_billingconductor/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-08-08 01:06:45.000000 types-aiobotocore-billingconductor-2.5.4/types_aiobotocore_billingconductor/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:23:22.214621 types-aiobotocore-billingconductor-2.5.4/types_aiobotocore_billingconductor.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    15317 2023-08-08 01:23:22.000000 types-aiobotocore-billingconductor-2.5.4/types_aiobotocore_billingconductor.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      984 2023-08-08 01:23:22.000000 types-aiobotocore-billingconductor-2.5.4/types_aiobotocore_billingconductor.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 01:23:22.000000 types-aiobotocore-billingconductor-2.5.4/types_aiobotocore_billingconductor.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 01:23:22.000000 types-aiobotocore-billingconductor-2.5.4/types_aiobotocore_billingconductor.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-08 01:23:22.000000 types-aiobotocore-billingconductor-2.5.4/types_aiobotocore_billingconductor.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-08-08 01:23:22.000000 types-aiobotocore-billingconductor-2.5.4/types_aiobotocore_billingconductor.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-billingconductor-2.5.2.post3/LICENSE` & `types-aiobotocore-billingconductor-2.5.4/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-billingconductor-2.5.2.post3/PKG-INFO` & `types-aiobotocore-billingconductor-2.5.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-billingconductor
-Version: 2.5.2.post3
-Summary: Type annotations for aiobotocore.BillingConductor 2.5.2 service generated with mypy-boto3-builder 7.17.2
+Version: 2.5.4
+Summary: Type annotations for aiobotocore.BillingConductor 2.5.4 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_billingconductor/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-billingconductor.svg?color=blue)](https://pypi.org/project/types-aiobotocore-billingconductor)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_billingconductor/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-billingconductor)](https://pepy.tech/project/types-aiobotocore-billingconductor)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.BillingConductor 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/billingconductor.html#BillingConductor)
+[aiobotocore.BillingConductor 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/billingconductor.html#BillingConductor)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-billingconductor-2.5.2.post3/README.md` & `types-aiobotocore-billingconductor-2.5.4/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-billingconductor.svg?color=blue)](https://pypi.org/project/types-aiobotocore-billingconductor)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_billingconductor/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-billingconductor)](https://pepy.tech/project/types-aiobotocore-billingconductor)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.BillingConductor 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/billingconductor.html#BillingConductor)
+[aiobotocore.BillingConductor 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/billingconductor.html#BillingConductor)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-billingconductor-2.5.2.post3/setup.py` & `types-aiobotocore-billingconductor-2.5.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-billingconductor",
-    version="2.5.2.post3",
+    version="2.5.4",
     packages=["types_aiobotocore_billingconductor"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.BillingConductor 2.5.2 service generated with"
+        "Type annotations for aiobotocore.BillingConductor 2.5.4 service generated with"
         " mypy-boto3-builder 7.17.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
```

### Comparing `types-aiobotocore-billingconductor-2.5.2.post3/types_aiobotocore_billingconductor/__init__.py` & `types-aiobotocore-billingconductor-2.5.4/types_aiobotocore_billingconductor/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-billingconductor-2.5.2.post3/types_aiobotocore_billingconductor/__init__.pyi` & `types-aiobotocore-billingconductor-2.5.4/types_aiobotocore_billingconductor/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-billingconductor-2.5.2.post3/types_aiobotocore_billingconductor/__main__.py` & `types-aiobotocore-billingconductor-2.5.4/types_aiobotocore_billingconductor/__main__.py`

 * *Files 21% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.BillingConductor 2.5.2\nVersion:        "
-        " 2.5.2.post3\nBuilder version: 7.17.2\nDocs:           "
+        "Type annotations for aiobotocore.BillingConductor 2.5.4\nVersion:         2.5.4\nBuilder"
+        " version: 7.17.2\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_billingconductor//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/billingconductor.html#BillingConductor\nOther"
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

### Comparing `types-aiobotocore-billingconductor-2.5.2.post3/types_aiobotocore_billingconductor/client.py` & `types-aiobotocore-billingconductor-2.5.4/types_aiobotocore_billingconductor/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -68,14 +68,15 @@
     ListPricingPlansOutputTypeDef,
     ListPricingRulesAssociatedToPricingPlanOutputTypeDef,
     ListPricingRulesFilterTypeDef,
     ListPricingRulesOutputTypeDef,
     ListResourcesAssociatedToCustomLineItemFilterTypeDef,
     ListResourcesAssociatedToCustomLineItemOutputTypeDef,
     ListTagsForResourceResponseTypeDef,
+    UpdateBillingGroupAccountGroupingTypeDef,
     UpdateBillingGroupOutputTypeDef,
     UpdateCustomLineItemChargeDetailsTypeDef,
     UpdateCustomLineItemOutputTypeDef,
     UpdatePricingPlanOutputTypeDef,
     UpdatePricingRuleOutputTypeDef,
     UpdateTieringInputTypeDef,
 )
@@ -525,15 +526,16 @@
     async def update_billing_group(
         self,
         *,
         Arn: str,
         Name: str = ...,
         Status: BillingGroupStatusType = ...,
         ComputationPreference: ComputationPreferenceTypeDef = ...,
-        Description: str = ...
+        Description: str = ...,
+        AccountGrouping: UpdateBillingGroupAccountGroupingTypeDef = ...
     ) -> UpdateBillingGroupOutputTypeDef:
         """
         This updates an existing billing group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/billingconductor.html#BillingConductor.Client.update_billing_group)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_billingconductor/client/#update_billing_group)
         """
```

### Comparing `types-aiobotocore-billingconductor-2.5.2.post3/types_aiobotocore_billingconductor/client.pyi` & `types-aiobotocore-billingconductor-2.5.4/types_aiobotocore_billingconductor/client.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -68,14 +68,15 @@
     ListPricingPlansOutputTypeDef,
     ListPricingRulesAssociatedToPricingPlanOutputTypeDef,
     ListPricingRulesFilterTypeDef,
     ListPricingRulesOutputTypeDef,
     ListResourcesAssociatedToCustomLineItemFilterTypeDef,
     ListResourcesAssociatedToCustomLineItemOutputTypeDef,
     ListTagsForResourceResponseTypeDef,
+    UpdateBillingGroupAccountGroupingTypeDef,
     UpdateBillingGroupOutputTypeDef,
     UpdateCustomLineItemChargeDetailsTypeDef,
     UpdateCustomLineItemOutputTypeDef,
     UpdatePricingPlanOutputTypeDef,
     UpdatePricingRuleOutputTypeDef,
     UpdateTieringInputTypeDef,
 )
@@ -490,15 +491,16 @@
     async def update_billing_group(
         self,
         *,
         Arn: str,
         Name: str = ...,
         Status: BillingGroupStatusType = ...,
         ComputationPreference: ComputationPreferenceTypeDef = ...,
-        Description: str = ...
+        Description: str = ...,
+        AccountGrouping: UpdateBillingGroupAccountGroupingTypeDef = ...
     ) -> UpdateBillingGroupOutputTypeDef:
         """
         This updates an existing billing group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/billingconductor.html#BillingConductor.Client.update_billing_group)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_billingconductor/client/#update_billing_group)
         """
```

### Comparing `types-aiobotocore-billingconductor-2.5.2.post3/types_aiobotocore_billingconductor/literals.py` & `types-aiobotocore-billingconductor-2.5.4/types_aiobotocore_billingconductor/literals.py`

 * *Files 1% similar despite different names*

```diff
@@ -85,14 +85,15 @@
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
@@ -188,14 +189,15 @@
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
@@ -274,26 +276,28 @@
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

### Comparing `types-aiobotocore-billingconductor-2.5.2.post3/types_aiobotocore_billingconductor/literals.pyi` & `types-aiobotocore-billingconductor-2.5.4/types_aiobotocore_billingconductor/literals.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -83,14 +83,15 @@
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
@@ -186,14 +187,15 @@
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
@@ -272,26 +274,28 @@
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

### Comparing `types-aiobotocore-billingconductor-2.5.2.post3/types_aiobotocore_billingconductor/paginator.py` & `types-aiobotocore-billingconductor-2.5.4/types_aiobotocore_billingconductor/paginator.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-billingconductor-2.5.2.post3/types_aiobotocore_billingconductor/paginator.pyi` & `types-aiobotocore-billingconductor-2.5.4/types_aiobotocore_billingconductor/paginator.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-billingconductor-2.5.2.post3/types_aiobotocore_billingconductor/type_defs.py` & `types-aiobotocore-billingconductor-2.5.4/types_aiobotocore_billingconductor/type_defs.py`

 * *Files 2% similar despite different names*

```diff
@@ -36,14 +36,15 @@
     "AssociateAccountsInputRequestTypeDef",
     "ResponseMetadataTypeDef",
     "AssociatePricingRulesInputRequestTypeDef",
     "AssociateResourceErrorTypeDef",
     "CustomLineItemBillingPeriodRangeTypeDef",
     "BillingGroupCostReportElementTypeDef",
     "ComputationPreferenceTypeDef",
+    "ListBillingGroupAccountGroupingTypeDef",
     "CreateFreeTierConfigTypeDef",
     "CreatePricingPlanInputRequestTypeDef",
     "CustomLineItemFlatChargeDetailsTypeDef",
     "CustomLineItemPercentageChargeDetailsTypeDef",
     "DeleteBillingGroupInputRequestTypeDef",
     "DeletePricingPlanInputRequestTypeDef",
     "DeletePricingRuleInputRequestTypeDef",
@@ -64,14 +65,15 @@
     "ListPricingRulesAssociatedToPricingPlanInputRequestTypeDef",
     "ListPricingRulesFilterTypeDef",
     "ListResourcesAssociatedToCustomLineItemFilterTypeDef",
     "ListResourcesAssociatedToCustomLineItemResponseElementTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
+    "UpdateBillingGroupAccountGroupingTypeDef",
     "UpdateCustomLineItemFlatChargeDetailsTypeDef",
     "UpdateCustomLineItemPercentageChargeDetailsTypeDef",
     "UpdateFreeTierConfigTypeDef",
     "UpdatePricingPlanInputRequestTypeDef",
     "AssociateAccountsOutputTypeDef",
     "AssociatePricingRulesOutputTypeDef",
     "CreateBillingGroupOutputTypeDef",
@@ -84,25 +86,23 @@
     "DeletePricingRuleOutputTypeDef",
     "DisassociateAccountsOutputTypeDef",
     "DisassociatePricingRulesOutputTypeDef",
     "ListAccountAssociationsOutputTypeDef",
     "ListPricingPlansAssociatedWithPricingRuleOutputTypeDef",
     "ListPricingRulesAssociatedToPricingPlanOutputTypeDef",
     "ListTagsForResourceResponseTypeDef",
-    "UpdateBillingGroupOutputTypeDef",
     "UpdatePricingPlanOutputTypeDef",
     "AssociateResourceResponseElementTypeDef",
     "DisassociateResourceResponseElementTypeDef",
     "BatchAssociateResourcesToCustomLineItemInputRequestTypeDef",
     "BatchDisassociateResourcesFromCustomLineItemInputRequestTypeDef",
     "DeleteCustomLineItemInputRequestTypeDef",
     "ListBillingGroupCostReportsOutputTypeDef",
-    "BillingGroupListElementTypeDef",
     "CreateBillingGroupInputRequestTypeDef",
-    "UpdateBillingGroupInputRequestTypeDef",
+    "BillingGroupListElementTypeDef",
     "CreateTieringInputTypeDef",
     "CustomLineItemChargeDetailsTypeDef",
     "TieringTypeDef",
     "ListAccountAssociationsInputRequestTypeDef",
     "ListAccountAssociationsInputListAccountAssociationsPaginateTypeDef",
     "ListPricingPlansAssociatedWithPricingRuleInputListPricingPlansAssociatedWithPricingRulePaginateTypeDef",
     "ListPricingRulesAssociatedToPricingPlanInputListPricingRulesAssociatedToPricingPlanPaginateTypeDef",
@@ -118,14 +118,16 @@
     "ListPricingPlansInputRequestTypeDef",
     "ListPricingPlansOutputTypeDef",
     "ListPricingRulesInputListPricingRulesPaginateTypeDef",
     "ListPricingRulesInputRequestTypeDef",
     "ListResourcesAssociatedToCustomLineItemInputListResourcesAssociatedToCustomLineItemPaginateTypeDef",
     "ListResourcesAssociatedToCustomLineItemInputRequestTypeDef",
     "ListResourcesAssociatedToCustomLineItemOutputTypeDef",
+    "UpdateBillingGroupInputRequestTypeDef",
+    "UpdateBillingGroupOutputTypeDef",
     "UpdateCustomLineItemChargeDetailsTypeDef",
     "UpdateTieringInputTypeDef",
     "BatchAssociateResourcesToCustomLineItemOutputTypeDef",
     "BatchDisassociateResourcesFromCustomLineItemOutputTypeDef",
     "ListBillingGroupsOutputTypeDef",
     "CreatePricingRuleInputRequestTypeDef",
     "CreateCustomLineItemInputRequestTypeDef",
@@ -150,20 +152,32 @@
         "BillingGroupArn": str,
         "AccountName": str,
         "AccountEmail": str,
     },
     total=False,
 )
 
-AccountGroupingTypeDef = TypedDict(
-    "AccountGroupingTypeDef",
+_RequiredAccountGroupingTypeDef = TypedDict(
+    "_RequiredAccountGroupingTypeDef",
     {
         "LinkedAccountIds": Sequence[str],
     },
 )
+_OptionalAccountGroupingTypeDef = TypedDict(
+    "_OptionalAccountGroupingTypeDef",
+    {
+        "AutoAssociate": bool,
+    },
+    total=False,
+)
+
+
+class AccountGroupingTypeDef(_RequiredAccountGroupingTypeDef, _OptionalAccountGroupingTypeDef):
+    pass
+
 
 AssociateAccountsInputRequestTypeDef = TypedDict(
     "AssociateAccountsInputRequestTypeDef",
     {
         "Arn": str,
         "AccountIds": Sequence[str],
     },
@@ -235,14 +249,22 @@
 ComputationPreferenceTypeDef = TypedDict(
     "ComputationPreferenceTypeDef",
     {
         "PricingPlanArn": str,
     },
 )
 
+ListBillingGroupAccountGroupingTypeDef = TypedDict(
+    "ListBillingGroupAccountGroupingTypeDef",
+    {
+        "AutoAssociate": bool,
+    },
+    total=False,
+)
+
 CreateFreeTierConfigTypeDef = TypedDict(
     "CreateFreeTierConfigTypeDef",
     {
         "Activated": bool,
     },
 )
 
@@ -373,14 +395,15 @@
 
 ListBillingGroupsFilterTypeDef = TypedDict(
     "ListBillingGroupsFilterTypeDef",
     {
         "Arns": Sequence[str],
         "PricingPlan": str,
         "Statuses": Sequence[BillingGroupStatusType],
+        "AutoAssociate": bool,
     },
     total=False,
 )
 
 ListCustomLineItemFlatChargeDetailsTypeDef = TypedDict(
     "ListCustomLineItemFlatChargeDetailsTypeDef",
     {
@@ -528,14 +551,22 @@
     "UntagResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
         "TagKeys": Sequence[str],
     },
 )
 
+UpdateBillingGroupAccountGroupingTypeDef = TypedDict(
+    "UpdateBillingGroupAccountGroupingTypeDef",
+    {
+        "AutoAssociate": bool,
+    },
+    total=False,
+)
+
 UpdateCustomLineItemFlatChargeDetailsTypeDef = TypedDict(
     "UpdateCustomLineItemFlatChargeDetailsTypeDef",
     {
         "ChargeValue": float,
     },
 )
 
@@ -706,30 +737,14 @@
     "ListTagsForResourceResponseTypeDef",
     {
         "Tags": Dict[str, str],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-UpdateBillingGroupOutputTypeDef = TypedDict(
-    "UpdateBillingGroupOutputTypeDef",
-    {
-        "Arn": str,
-        "Name": str,
-        "Description": str,
-        "PrimaryAccountId": str,
-        "PricingPlanArn": str,
-        "Size": int,
-        "LastModifiedTime": int,
-        "Status": BillingGroupStatusType,
-        "StatusReason": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 UpdatePricingPlanOutputTypeDef = TypedDict(
     "UpdatePricingPlanOutputTypeDef",
     {
         "Arn": str,
         "Name": str,
         "Description": str,
         "Size": int,
@@ -829,31 +844,14 @@
     {
         "BillingGroupCostReports": List[BillingGroupCostReportElementTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-BillingGroupListElementTypeDef = TypedDict(
-    "BillingGroupListElementTypeDef",
-    {
-        "Name": str,
-        "Arn": str,
-        "Description": str,
-        "PrimaryAccountId": str,
-        "ComputationPreference": ComputationPreferenceTypeDef,
-        "Size": int,
-        "CreationTime": int,
-        "LastModifiedTime": int,
-        "Status": BillingGroupStatusType,
-        "StatusReason": str,
-    },
-    total=False,
-)
-
 _RequiredCreateBillingGroupInputRequestTypeDef = TypedDict(
     "_RequiredCreateBillingGroupInputRequestTypeDef",
     {
         "Name": str,
         "AccountGrouping": AccountGroupingTypeDef,
         "ComputationPreference": ComputationPreferenceTypeDef,
     },
@@ -872,38 +870,32 @@
 
 class CreateBillingGroupInputRequestTypeDef(
     _RequiredCreateBillingGroupInputRequestTypeDef, _OptionalCreateBillingGroupInputRequestTypeDef
 ):
     pass
 
 
-_RequiredUpdateBillingGroupInputRequestTypeDef = TypedDict(
-    "_RequiredUpdateBillingGroupInputRequestTypeDef",
-    {
-        "Arn": str,
-    },
-)
-_OptionalUpdateBillingGroupInputRequestTypeDef = TypedDict(
-    "_OptionalUpdateBillingGroupInputRequestTypeDef",
+BillingGroupListElementTypeDef = TypedDict(
+    "BillingGroupListElementTypeDef",
     {
         "Name": str,
-        "Status": BillingGroupStatusType,
-        "ComputationPreference": ComputationPreferenceTypeDef,
+        "Arn": str,
         "Description": str,
+        "PrimaryAccountId": str,
+        "ComputationPreference": ComputationPreferenceTypeDef,
+        "Size": int,
+        "CreationTime": int,
+        "LastModifiedTime": int,
+        "Status": BillingGroupStatusType,
+        "StatusReason": str,
+        "AccountGrouping": ListBillingGroupAccountGroupingTypeDef,
     },
     total=False,
 )
 
-
-class UpdateBillingGroupInputRequestTypeDef(
-    _RequiredUpdateBillingGroupInputRequestTypeDef, _OptionalUpdateBillingGroupInputRequestTypeDef
-):
-    pass
-
-
 CreateTieringInputTypeDef = TypedDict(
     "CreateTieringInputTypeDef",
     {
         "FreeTier": CreateFreeTierConfigTypeDef,
     },
 )
 
@@ -1202,14 +1194,56 @@
         "Arn": str,
         "AssociatedResources": List[ListResourcesAssociatedToCustomLineItemResponseElementTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+_RequiredUpdateBillingGroupInputRequestTypeDef = TypedDict(
+    "_RequiredUpdateBillingGroupInputRequestTypeDef",
+    {
+        "Arn": str,
+    },
+)
+_OptionalUpdateBillingGroupInputRequestTypeDef = TypedDict(
+    "_OptionalUpdateBillingGroupInputRequestTypeDef",
+    {
+        "Name": str,
+        "Status": BillingGroupStatusType,
+        "ComputationPreference": ComputationPreferenceTypeDef,
+        "Description": str,
+        "AccountGrouping": UpdateBillingGroupAccountGroupingTypeDef,
+    },
+    total=False,
+)
+
+
+class UpdateBillingGroupInputRequestTypeDef(
+    _RequiredUpdateBillingGroupInputRequestTypeDef, _OptionalUpdateBillingGroupInputRequestTypeDef
+):
+    pass
+
+
+UpdateBillingGroupOutputTypeDef = TypedDict(
+    "UpdateBillingGroupOutputTypeDef",
+    {
+        "Arn": str,
+        "Name": str,
+        "Description": str,
+        "PrimaryAccountId": str,
+        "PricingPlanArn": str,
+        "Size": int,
+        "LastModifiedTime": int,
+        "Status": BillingGroupStatusType,
+        "StatusReason": str,
+        "AccountGrouping": UpdateBillingGroupAccountGroupingTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 UpdateCustomLineItemChargeDetailsTypeDef = TypedDict(
     "UpdateCustomLineItemChargeDetailsTypeDef",
     {
         "Flat": UpdateCustomLineItemFlatChargeDetailsTypeDef,
         "Percentage": UpdateCustomLineItemPercentageChargeDetailsTypeDef,
     },
     total=False,
```

### Comparing `types-aiobotocore-billingconductor-2.5.2.post3/types_aiobotocore_billingconductor/type_defs.pyi` & `types-aiobotocore-billingconductor-2.5.4/types_aiobotocore_billingconductor/type_defs.pyi`

 * *Files 3% similar despite different names*

```diff
@@ -35,14 +35,15 @@
     "AssociateAccountsInputRequestTypeDef",
     "ResponseMetadataTypeDef",
     "AssociatePricingRulesInputRequestTypeDef",
     "AssociateResourceErrorTypeDef",
     "CustomLineItemBillingPeriodRangeTypeDef",
     "BillingGroupCostReportElementTypeDef",
     "ComputationPreferenceTypeDef",
+    "ListBillingGroupAccountGroupingTypeDef",
     "CreateFreeTierConfigTypeDef",
     "CreatePricingPlanInputRequestTypeDef",
     "CustomLineItemFlatChargeDetailsTypeDef",
     "CustomLineItemPercentageChargeDetailsTypeDef",
     "DeleteBillingGroupInputRequestTypeDef",
     "DeletePricingPlanInputRequestTypeDef",
     "DeletePricingRuleInputRequestTypeDef",
@@ -63,14 +64,15 @@
     "ListPricingRulesAssociatedToPricingPlanInputRequestTypeDef",
     "ListPricingRulesFilterTypeDef",
     "ListResourcesAssociatedToCustomLineItemFilterTypeDef",
     "ListResourcesAssociatedToCustomLineItemResponseElementTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
+    "UpdateBillingGroupAccountGroupingTypeDef",
     "UpdateCustomLineItemFlatChargeDetailsTypeDef",
     "UpdateCustomLineItemPercentageChargeDetailsTypeDef",
     "UpdateFreeTierConfigTypeDef",
     "UpdatePricingPlanInputRequestTypeDef",
     "AssociateAccountsOutputTypeDef",
     "AssociatePricingRulesOutputTypeDef",
     "CreateBillingGroupOutputTypeDef",
@@ -83,25 +85,23 @@
     "DeletePricingRuleOutputTypeDef",
     "DisassociateAccountsOutputTypeDef",
     "DisassociatePricingRulesOutputTypeDef",
     "ListAccountAssociationsOutputTypeDef",
     "ListPricingPlansAssociatedWithPricingRuleOutputTypeDef",
     "ListPricingRulesAssociatedToPricingPlanOutputTypeDef",
     "ListTagsForResourceResponseTypeDef",
-    "UpdateBillingGroupOutputTypeDef",
     "UpdatePricingPlanOutputTypeDef",
     "AssociateResourceResponseElementTypeDef",
     "DisassociateResourceResponseElementTypeDef",
     "BatchAssociateResourcesToCustomLineItemInputRequestTypeDef",
     "BatchDisassociateResourcesFromCustomLineItemInputRequestTypeDef",
     "DeleteCustomLineItemInputRequestTypeDef",
     "ListBillingGroupCostReportsOutputTypeDef",
-    "BillingGroupListElementTypeDef",
     "CreateBillingGroupInputRequestTypeDef",
-    "UpdateBillingGroupInputRequestTypeDef",
+    "BillingGroupListElementTypeDef",
     "CreateTieringInputTypeDef",
     "CustomLineItemChargeDetailsTypeDef",
     "TieringTypeDef",
     "ListAccountAssociationsInputRequestTypeDef",
     "ListAccountAssociationsInputListAccountAssociationsPaginateTypeDef",
     "ListPricingPlansAssociatedWithPricingRuleInputListPricingPlansAssociatedWithPricingRulePaginateTypeDef",
     "ListPricingRulesAssociatedToPricingPlanInputListPricingRulesAssociatedToPricingPlanPaginateTypeDef",
@@ -117,14 +117,16 @@
     "ListPricingPlansInputRequestTypeDef",
     "ListPricingPlansOutputTypeDef",
     "ListPricingRulesInputListPricingRulesPaginateTypeDef",
     "ListPricingRulesInputRequestTypeDef",
     "ListResourcesAssociatedToCustomLineItemInputListResourcesAssociatedToCustomLineItemPaginateTypeDef",
     "ListResourcesAssociatedToCustomLineItemInputRequestTypeDef",
     "ListResourcesAssociatedToCustomLineItemOutputTypeDef",
+    "UpdateBillingGroupInputRequestTypeDef",
+    "UpdateBillingGroupOutputTypeDef",
     "UpdateCustomLineItemChargeDetailsTypeDef",
     "UpdateTieringInputTypeDef",
     "BatchAssociateResourcesToCustomLineItemOutputTypeDef",
     "BatchDisassociateResourcesFromCustomLineItemOutputTypeDef",
     "ListBillingGroupsOutputTypeDef",
     "CreatePricingRuleInputRequestTypeDef",
     "CreateCustomLineItemInputRequestTypeDef",
@@ -149,20 +151,30 @@
         "BillingGroupArn": str,
         "AccountName": str,
         "AccountEmail": str,
     },
     total=False,
 )
 
-AccountGroupingTypeDef = TypedDict(
-    "AccountGroupingTypeDef",
+_RequiredAccountGroupingTypeDef = TypedDict(
+    "_RequiredAccountGroupingTypeDef",
     {
         "LinkedAccountIds": Sequence[str],
     },
 )
+_OptionalAccountGroupingTypeDef = TypedDict(
+    "_OptionalAccountGroupingTypeDef",
+    {
+        "AutoAssociate": bool,
+    },
+    total=False,
+)
+
+class AccountGroupingTypeDef(_RequiredAccountGroupingTypeDef, _OptionalAccountGroupingTypeDef):
+    pass
 
 AssociateAccountsInputRequestTypeDef = TypedDict(
     "AssociateAccountsInputRequestTypeDef",
     {
         "Arn": str,
         "AccountIds": Sequence[str],
     },
@@ -232,14 +244,22 @@
 ComputationPreferenceTypeDef = TypedDict(
     "ComputationPreferenceTypeDef",
     {
         "PricingPlanArn": str,
     },
 )
 
+ListBillingGroupAccountGroupingTypeDef = TypedDict(
+    "ListBillingGroupAccountGroupingTypeDef",
+    {
+        "AutoAssociate": bool,
+    },
+    total=False,
+)
+
 CreateFreeTierConfigTypeDef = TypedDict(
     "CreateFreeTierConfigTypeDef",
     {
         "Activated": bool,
     },
 )
 
@@ -366,14 +386,15 @@
 
 ListBillingGroupsFilterTypeDef = TypedDict(
     "ListBillingGroupsFilterTypeDef",
     {
         "Arns": Sequence[str],
         "PricingPlan": str,
         "Statuses": Sequence[BillingGroupStatusType],
+        "AutoAssociate": bool,
     },
     total=False,
 )
 
 ListCustomLineItemFlatChargeDetailsTypeDef = TypedDict(
     "ListCustomLineItemFlatChargeDetailsTypeDef",
     {
@@ -517,14 +538,22 @@
     "UntagResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
         "TagKeys": Sequence[str],
     },
 )
 
+UpdateBillingGroupAccountGroupingTypeDef = TypedDict(
+    "UpdateBillingGroupAccountGroupingTypeDef",
+    {
+        "AutoAssociate": bool,
+    },
+    total=False,
+)
+
 UpdateCustomLineItemFlatChargeDetailsTypeDef = TypedDict(
     "UpdateCustomLineItemFlatChargeDetailsTypeDef",
     {
         "ChargeValue": float,
     },
 )
 
@@ -693,30 +722,14 @@
     "ListTagsForResourceResponseTypeDef",
     {
         "Tags": Dict[str, str],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-UpdateBillingGroupOutputTypeDef = TypedDict(
-    "UpdateBillingGroupOutputTypeDef",
-    {
-        "Arn": str,
-        "Name": str,
-        "Description": str,
-        "PrimaryAccountId": str,
-        "PricingPlanArn": str,
-        "Size": int,
-        "LastModifiedTime": int,
-        "Status": BillingGroupStatusType,
-        "StatusReason": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 UpdatePricingPlanOutputTypeDef = TypedDict(
     "UpdatePricingPlanOutputTypeDef",
     {
         "Arn": str,
         "Name": str,
         "Description": str,
         "Size": int,
@@ -810,31 +823,14 @@
     {
         "BillingGroupCostReports": List[BillingGroupCostReportElementTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-BillingGroupListElementTypeDef = TypedDict(
-    "BillingGroupListElementTypeDef",
-    {
-        "Name": str,
-        "Arn": str,
-        "Description": str,
-        "PrimaryAccountId": str,
-        "ComputationPreference": ComputationPreferenceTypeDef,
-        "Size": int,
-        "CreationTime": int,
-        "LastModifiedTime": int,
-        "Status": BillingGroupStatusType,
-        "StatusReason": str,
-    },
-    total=False,
-)
-
 _RequiredCreateBillingGroupInputRequestTypeDef = TypedDict(
     "_RequiredCreateBillingGroupInputRequestTypeDef",
     {
         "Name": str,
         "AccountGrouping": AccountGroupingTypeDef,
         "ComputationPreference": ComputationPreferenceTypeDef,
     },
@@ -851,36 +847,32 @@
 )
 
 class CreateBillingGroupInputRequestTypeDef(
     _RequiredCreateBillingGroupInputRequestTypeDef, _OptionalCreateBillingGroupInputRequestTypeDef
 ):
     pass
 
-_RequiredUpdateBillingGroupInputRequestTypeDef = TypedDict(
-    "_RequiredUpdateBillingGroupInputRequestTypeDef",
-    {
-        "Arn": str,
-    },
-)
-_OptionalUpdateBillingGroupInputRequestTypeDef = TypedDict(
-    "_OptionalUpdateBillingGroupInputRequestTypeDef",
+BillingGroupListElementTypeDef = TypedDict(
+    "BillingGroupListElementTypeDef",
     {
         "Name": str,
-        "Status": BillingGroupStatusType,
-        "ComputationPreference": ComputationPreferenceTypeDef,
+        "Arn": str,
         "Description": str,
+        "PrimaryAccountId": str,
+        "ComputationPreference": ComputationPreferenceTypeDef,
+        "Size": int,
+        "CreationTime": int,
+        "LastModifiedTime": int,
+        "Status": BillingGroupStatusType,
+        "StatusReason": str,
+        "AccountGrouping": ListBillingGroupAccountGroupingTypeDef,
     },
     total=False,
 )
 
-class UpdateBillingGroupInputRequestTypeDef(
-    _RequiredUpdateBillingGroupInputRequestTypeDef, _OptionalUpdateBillingGroupInputRequestTypeDef
-):
-    pass
-
 CreateTieringInputTypeDef = TypedDict(
     "CreateTieringInputTypeDef",
     {
         "FreeTier": CreateFreeTierConfigTypeDef,
     },
 )
 
@@ -1167,14 +1159,54 @@
         "Arn": str,
         "AssociatedResources": List[ListResourcesAssociatedToCustomLineItemResponseElementTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+_RequiredUpdateBillingGroupInputRequestTypeDef = TypedDict(
+    "_RequiredUpdateBillingGroupInputRequestTypeDef",
+    {
+        "Arn": str,
+    },
+)
+_OptionalUpdateBillingGroupInputRequestTypeDef = TypedDict(
+    "_OptionalUpdateBillingGroupInputRequestTypeDef",
+    {
+        "Name": str,
+        "Status": BillingGroupStatusType,
+        "ComputationPreference": ComputationPreferenceTypeDef,
+        "Description": str,
+        "AccountGrouping": UpdateBillingGroupAccountGroupingTypeDef,
+    },
+    total=False,
+)
+
+class UpdateBillingGroupInputRequestTypeDef(
+    _RequiredUpdateBillingGroupInputRequestTypeDef, _OptionalUpdateBillingGroupInputRequestTypeDef
+):
+    pass
+
+UpdateBillingGroupOutputTypeDef = TypedDict(
+    "UpdateBillingGroupOutputTypeDef",
+    {
+        "Arn": str,
+        "Name": str,
+        "Description": str,
+        "PrimaryAccountId": str,
+        "PricingPlanArn": str,
+        "Size": int,
+        "LastModifiedTime": int,
+        "Status": BillingGroupStatusType,
+        "StatusReason": str,
+        "AccountGrouping": UpdateBillingGroupAccountGroupingTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 UpdateCustomLineItemChargeDetailsTypeDef = TypedDict(
     "UpdateCustomLineItemChargeDetailsTypeDef",
     {
         "Flat": UpdateCustomLineItemFlatChargeDetailsTypeDef,
         "Percentage": UpdateCustomLineItemPercentageChargeDetailsTypeDef,
     },
     total=False,
```

### Comparing `types-aiobotocore-billingconductor-2.5.2.post3/types_aiobotocore_billingconductor.egg-info/PKG-INFO` & `types-aiobotocore-billingconductor-2.5.4/types_aiobotocore_billingconductor.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-billingconductor
-Version: 2.5.2.post3
-Summary: Type annotations for aiobotocore.BillingConductor 2.5.2 service generated with mypy-boto3-builder 7.17.2
+Version: 2.5.4
+Summary: Type annotations for aiobotocore.BillingConductor 2.5.4 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_billingconductor/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-billingconductor.svg?color=blue)](https://pypi.org/project/types-aiobotocore-billingconductor)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_billingconductor/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-billingconductor)](https://pepy.tech/project/types-aiobotocore-billingconductor)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.BillingConductor 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/billingconductor.html#BillingConductor)
+[aiobotocore.BillingConductor 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/billingconductor.html#BillingConductor)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-billingconductor-2.5.2.post3/types_aiobotocore_billingconductor.egg-info/SOURCES.txt` & `types-aiobotocore-billingconductor-2.5.4/types_aiobotocore_billingconductor.egg-info/SOURCES.txt`

 * *Files identical despite different names*


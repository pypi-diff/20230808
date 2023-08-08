# Comparing `tmp/types-aiobotocore-glue-2.5.2.post3.tar.gz` & `tmp/types-aiobotocore-glue-2.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-glue-2.5.2.post3.tar", last modified: Fri Aug  4 12:37:46 2023, max compression
+gzip compressed data, was "types-aiobotocore-glue-2.5.4.tar", last modified: Tue Aug  8 01:23:47 2023, max compression
```

## Comparing `types-aiobotocore-glue-2.5.2.post3.tar` & `types-aiobotocore-glue-2.5.4.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:37:46.771883 types-aiobotocore-glue-2.5.2.post3/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-04 12:24:27.000000 types-aiobotocore-glue-2.5.2.post3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    15203 2023-08-04 12:37:46.771883 types-aiobotocore-glue-2.5.2.post3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    13697 2023-08-04 12:24:27.000000 types-aiobotocore-glue-2.5.2.post3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-04 12:37:46.771883 types-aiobotocore-glue-2.5.2.post3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2027 2023-08-04 12:24:27.000000 types-aiobotocore-glue-2.5.2.post3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:37:46.759882 types-aiobotocore-glue-2.5.2.post3/types_aiobotocore_glue/
--rw-r--r--   0 runner    (1001) docker     (123)     4159 2023-08-04 12:24:27.000000 types-aiobotocore-glue-2.5.2.post3/types_aiobotocore_glue/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4158 2023-08-04 12:24:27.000000 types-aiobotocore-glue-2.5.2.post3/types_aiobotocore_glue/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      920 2023-08-04 12:24:27.000000 types-aiobotocore-glue-2.5.2.post3/types_aiobotocore_glue/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)   143723 2023-08-04 12:24:28.000000 types-aiobotocore-glue-2.5.2.post3/types_aiobotocore_glue/client.py
--rw-r--r--   0 runner    (1001) docker     (123)   143493 2023-08-04 12:24:28.000000 types-aiobotocore-glue-2.5.2.post3/types_aiobotocore_glue/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    20771 2023-08-04 12:24:29.000000 types-aiobotocore-glue-2.5.2.post3/types_aiobotocore_glue/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    20769 2023-08-04 12:24:29.000000 types-aiobotocore-glue-2.5.2.post3/types_aiobotocore_glue/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    22187 2023-08-04 12:24:28.000000 types-aiobotocore-glue-2.5.2.post3/types_aiobotocore_glue/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)    22166 2023-08-04 12:24:28.000000 types-aiobotocore-glue-2.5.2.post3/types_aiobotocore_glue/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 12:24:27.000000 types-aiobotocore-glue-2.5.2.post3/types_aiobotocore_glue/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)   253061 2023-08-04 12:24:36.000000 types-aiobotocore-glue-2.5.2.post3/types_aiobotocore_glue/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)   252686 2023-08-04 12:24:33.000000 types-aiobotocore-glue-2.5.2.post3/types_aiobotocore_glue/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-04 12:24:27.000000 types-aiobotocore-glue-2.5.2.post3/types_aiobotocore_glue/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:37:46.771883 types-aiobotocore-glue-2.5.2.post3/types_aiobotocore_glue.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    15203 2023-08-04 12:37:46.000000 types-aiobotocore-glue-2.5.2.post3/types_aiobotocore_glue.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      756 2023-08-04 12:37:46.000000 types-aiobotocore-glue-2.5.2.post3/types_aiobotocore_glue.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 12:37:46.000000 types-aiobotocore-glue-2.5.2.post3/types_aiobotocore_glue.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 12:37:46.000000 types-aiobotocore-glue-2.5.2.post3/types_aiobotocore_glue.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-04 12:37:46.000000 types-aiobotocore-glue-2.5.2.post3/types_aiobotocore_glue.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-08-04 12:37:46.000000 types-aiobotocore-glue-2.5.2.post3/types_aiobotocore_glue.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:23:47.078724 types-aiobotocore-glue-2.5.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-08 01:11:48.000000 types-aiobotocore-glue-2.5.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    15197 2023-08-08 01:23:47.078724 types-aiobotocore-glue-2.5.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    13697 2023-08-08 01:11:48.000000 types-aiobotocore-glue-2.5.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-08 01:23:47.078724 types-aiobotocore-glue-2.5.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2021 2023-08-08 01:11:48.000000 types-aiobotocore-glue-2.5.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:23:47.078724 types-aiobotocore-glue-2.5.4/types_aiobotocore_glue/
+-rw-r--r--   0 runner    (1001) docker     (123)     4159 2023-08-08 01:11:48.000000 types-aiobotocore-glue-2.5.4/types_aiobotocore_glue/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4158 2023-08-08 01:11:48.000000 types-aiobotocore-glue-2.5.4/types_aiobotocore_glue/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      908 2023-08-08 01:11:48.000000 types-aiobotocore-glue-2.5.4/types_aiobotocore_glue/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   143821 2023-08-08 01:11:49.000000 types-aiobotocore-glue-2.5.4/types_aiobotocore_glue/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)   143591 2023-08-08 01:11:49.000000 types-aiobotocore-glue-2.5.4/types_aiobotocore_glue/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    21050 2023-08-08 01:11:50.000000 types-aiobotocore-glue-2.5.4/types_aiobotocore_glue/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21048 2023-08-08 01:11:50.000000 types-aiobotocore-glue-2.5.4/types_aiobotocore_glue/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    22187 2023-08-08 01:11:49.000000 types-aiobotocore-glue-2.5.4/types_aiobotocore_glue/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22166 2023-08-08 01:11:49.000000 types-aiobotocore-glue-2.5.4/types_aiobotocore_glue/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 01:11:48.000000 types-aiobotocore-glue-2.5.4/types_aiobotocore_glue/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)   256490 2023-08-08 01:11:56.000000 types-aiobotocore-glue-2.5.4/types_aiobotocore_glue/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)   256109 2023-08-08 01:11:54.000000 types-aiobotocore-glue-2.5.4/types_aiobotocore_glue/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-08-08 01:11:48.000000 types-aiobotocore-glue-2.5.4/types_aiobotocore_glue/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:23:47.078724 types-aiobotocore-glue-2.5.4/types_aiobotocore_glue.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    15197 2023-08-08 01:23:46.000000 types-aiobotocore-glue-2.5.4/types_aiobotocore_glue.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      756 2023-08-08 01:23:46.000000 types-aiobotocore-glue-2.5.4/types_aiobotocore_glue.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 01:23:46.000000 types-aiobotocore-glue-2.5.4/types_aiobotocore_glue.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 01:23:46.000000 types-aiobotocore-glue-2.5.4/types_aiobotocore_glue.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-08 01:23:46.000000 types-aiobotocore-glue-2.5.4/types_aiobotocore_glue.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-08-08 01:23:46.000000 types-aiobotocore-glue-2.5.4/types_aiobotocore_glue.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-glue-2.5.2.post3/LICENSE` & `types-aiobotocore-glue-2.5.4/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-glue-2.5.2.post3/PKG-INFO` & `types-aiobotocore-glue-2.5.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-glue
-Version: 2.5.2.post3
-Summary: Type annotations for aiobotocore.Glue 2.5.2 service generated with mypy-boto3-builder 7.17.2
+Version: 2.5.4
+Summary: Type annotations for aiobotocore.Glue 2.5.4 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_glue/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-glue.svg?color=blue)](https://pypi.org/project/types-aiobotocore-glue)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_glue/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-glue)](https://pepy.tech/project/types-aiobotocore-glue)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.Glue 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue)
+[aiobotocore.Glue 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-glue-2.5.2.post3/README.md` & `types-aiobotocore-glue-2.5.4/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-glue.svg?color=blue)](https://pypi.org/project/types-aiobotocore-glue)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_glue/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-glue)](https://pepy.tech/project/types-aiobotocore-glue)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.Glue 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue)
+[aiobotocore.Glue 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-glue-2.5.2.post3/setup.py` & `types-aiobotocore-glue-2.5.4/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-glue",
-    version="2.5.2.post3",
+    version="2.5.4",
     packages=["types_aiobotocore_glue"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.Glue 2.5.2 service generated with mypy-boto3-builder"
+        "Type annotations for aiobotocore.Glue 2.5.4 service generated with mypy-boto3-builder"
         " 7.17.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
```

### Comparing `types-aiobotocore-glue-2.5.2.post3/types_aiobotocore_glue/__init__.py` & `types-aiobotocore-glue-2.5.4/types_aiobotocore_glue/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-glue-2.5.2.post3/types_aiobotocore_glue/__init__.pyi` & `types-aiobotocore-glue-2.5.4/types_aiobotocore_glue/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-glue-2.5.2.post3/types_aiobotocore_glue/__main__.py` & `types-aiobotocore-glue-2.5.4/types_aiobotocore_glue/__main__.py`

 * *Files 18% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.Glue 2.5.2\nVersion:         2.5.2.post3\nBuilder"
-        " version: 7.17.2\nDocs:           "
+        "Type annotations for aiobotocore.Glue 2.5.4\nVersion:         2.5.4\nBuilder version:"
+        " 7.17.2\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_glue//\nBoto3 docs:   "
         "   https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue\nOther"
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

### Comparing `types-aiobotocore-glue-2.5.2.post3/types_aiobotocore_glue/client.py` & `types-aiobotocore-glue-2.5.4/types_aiobotocore_glue/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -215,14 +215,15 @@
     ListStatementsResponseTypeDef,
     ListTriggersResponseTypeDef,
     ListWorkflowsResponseTypeDef,
     LocationTypeDef,
     MappingEntryTypeDef,
     MetadataKeyValuePairTypeDef,
     NotificationPropertyTypeDef,
+    OpenTableFormatInputTypeDef,
     PartitionIndexTypeDef,
     PartitionInputTypeDef,
     PartitionValueListTypeDef,
     PredicateTypeDef,
     PropertyPredicateTypeDef,
     PutResourcePolicyResponseTypeDef,
     PutSchemaVersionMetadataResponseTypeDef,
@@ -915,15 +916,16 @@
     async def create_table(
         self,
         *,
         DatabaseName: str,
         TableInput: TableInputTypeDef,
         CatalogId: str = ...,
         PartitionIndexes: Sequence[PartitionIndexTypeDef] = ...,
-        TransactionId: str = ...
+        TransactionId: str = ...,
+        OpenTableFormatInput: OpenTableFormatInputTypeDef = ...
     ) -> Dict[str, Any]:
         """
         Creates a new table definition in the Data Catalog.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Client.create_table)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_glue/client/#create_table)
         """
```

### Comparing `types-aiobotocore-glue-2.5.2.post3/types_aiobotocore_glue/client.pyi` & `types-aiobotocore-glue-2.5.4/types_aiobotocore_glue/client.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -215,14 +215,15 @@
     ListStatementsResponseTypeDef,
     ListTriggersResponseTypeDef,
     ListWorkflowsResponseTypeDef,
     LocationTypeDef,
     MappingEntryTypeDef,
     MetadataKeyValuePairTypeDef,
     NotificationPropertyTypeDef,
+    OpenTableFormatInputTypeDef,
     PartitionIndexTypeDef,
     PartitionInputTypeDef,
     PartitionValueListTypeDef,
     PredicateTypeDef,
     PropertyPredicateTypeDef,
     PutResourcePolicyResponseTypeDef,
     PutSchemaVersionMetadataResponseTypeDef,
@@ -870,15 +871,16 @@
     async def create_table(
         self,
         *,
         DatabaseName: str,
         TableInput: TableInputTypeDef,
         CatalogId: str = ...,
         PartitionIndexes: Sequence[PartitionIndexTypeDef] = ...,
-        TransactionId: str = ...
+        TransactionId: str = ...,
+        OpenTableFormatInput: OpenTableFormatInputTypeDef = ...
     ) -> Dict[str, Any]:
         """
         Creates a new table definition in the Data Catalog.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Client.create_table)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_glue/client/#create_table)
         """
```

### Comparing `types-aiobotocore-glue-2.5.2.post3/types_aiobotocore_glue/literals.py` & `types-aiobotocore-glue-2.5.4/types_aiobotocore_glue/literals.pyi`

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
     "AdditionalOptionKeysType",
     "AggFunctionType",
     "BackfillErrorCodeType",
     "BlueprintRunStateType",
     "BlueprintStatusType",
     "CatalogEncryptionModeType",
@@ -80,14 +79,15 @@
     "LastCrawlStatusType",
     "ListRegistriesPaginatorName",
     "ListSchemaVersionsPaginatorName",
     "ListSchemasPaginatorName",
     "LogicalOperatorType",
     "LogicalType",
     "MLUserDataEncryptionModeStringType",
+    "MetadataOperationType",
     "NodeTypeType",
     "ParamTypeType",
     "ParquetCompressionTypeType",
     "PartitionIndexStatusType",
     "PermissionType",
     "PermissionTypeType",
     "PiiTypeType",
@@ -127,15 +127,14 @@
     "GlueServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "RegionName",
 )
 
-
 AdditionalOptionKeysType = Literal["performanceTuning.caching"]
 AggFunctionType = Literal[
     "avg",
     "count",
     "countDistinct",
     "first",
     "kurtosis",
@@ -303,14 +302,15 @@
 LastCrawlStatusType = Literal["CANCELLED", "FAILED", "SUCCEEDED"]
 ListRegistriesPaginatorName = Literal["list_registries"]
 ListSchemaVersionsPaginatorName = Literal["list_schema_versions"]
 ListSchemasPaginatorName = Literal["list_schemas"]
 LogicalOperatorType = Literal["EQUALS"]
 LogicalType = Literal["AND", "ANY"]
 MLUserDataEncryptionModeStringType = Literal["DISABLED", "SSE-KMS"]
+MetadataOperationType = Literal["CREATE"]
 NodeTypeType = Literal["CRAWLER", "JOB", "TRIGGER"]
 ParamTypeType = Literal["bool", "complex", "float", "int", "list", "null", "str"]
 ParquetCompressionTypeType = Literal["gzip", "lzo", "none", "snappy", "uncompressed"]
 PartitionIndexStatusType = Literal["ACTIVE", "CREATING", "DELETING", "FAILED"]
 PermissionType = Literal[
     "ALL",
     "ALTER",
@@ -318,15 +318,17 @@
     "CREATE_TABLE",
     "DATA_LOCATION_ACCESS",
     "DELETE",
     "DROP",
     "INSERT",
     "SELECT",
 ]
-PermissionTypeType = Literal["CELL_FILTER_PERMISSION", "COLUMN_PERMISSION"]
+PermissionTypeType = Literal[
+    "CELL_FILTER_PERMISSION", "COLUMN_PERMISSION", "NESTED_CELL_PERMISSION", "NESTED_PERMISSION"
+]
 PiiTypeType = Literal["ColumnAudit", "ColumnMasking", "RowAudit", "RowMasking"]
 PrincipalTypeType = Literal["GROUP", "ROLE", "USER"]
 QuoteCharType = Literal["disabled", "quillemet", "quote", "single_quote"]
 RecrawlBehaviorType = Literal["CRAWL_EVENT_MODE", "CRAWL_EVERYTHING", "CRAWL_NEW_FOLDERS_ONLY"]
 RegistryStatusType = Literal["AVAILABLE", "DELETING"]
 ResourceShareTypeType = Literal["ALL", "FEDERATED", "FOREIGN"]
 ResourceTypeType = Literal["ARCHIVE", "FILE", "JAR"]
@@ -384,14 +386,15 @@
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
@@ -487,14 +490,15 @@
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
@@ -573,26 +577,28 @@
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
@@ -760,26 +766,29 @@
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
+    "ap-southeast-4",
     "ca-central-1",
     "eu-central-1",
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

### Comparing `types-aiobotocore-glue-2.5.2.post3/types_aiobotocore_glue/literals.pyi` & `types-aiobotocore-glue-2.5.4/types_aiobotocore_glue/literals.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 import sys
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
+
 __all__ = (
     "AdditionalOptionKeysType",
     "AggFunctionType",
     "BackfillErrorCodeType",
     "BlueprintRunStateType",
     "BlueprintStatusType",
     "CatalogEncryptionModeType",
@@ -79,14 +80,15 @@
     "LastCrawlStatusType",
     "ListRegistriesPaginatorName",
     "ListSchemaVersionsPaginatorName",
     "ListSchemasPaginatorName",
     "LogicalOperatorType",
     "LogicalType",
     "MLUserDataEncryptionModeStringType",
+    "MetadataOperationType",
     "NodeTypeType",
     "ParamTypeType",
     "ParquetCompressionTypeType",
     "PartitionIndexStatusType",
     "PermissionType",
     "PermissionTypeType",
     "PiiTypeType",
@@ -126,14 +128,15 @@
     "GlueServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "RegionName",
 )
 
+
 AdditionalOptionKeysType = Literal["performanceTuning.caching"]
 AggFunctionType = Literal[
     "avg",
     "count",
     "countDistinct",
     "first",
     "kurtosis",
@@ -301,14 +304,15 @@
 LastCrawlStatusType = Literal["CANCELLED", "FAILED", "SUCCEEDED"]
 ListRegistriesPaginatorName = Literal["list_registries"]
 ListSchemaVersionsPaginatorName = Literal["list_schema_versions"]
 ListSchemasPaginatorName = Literal["list_schemas"]
 LogicalOperatorType = Literal["EQUALS"]
 LogicalType = Literal["AND", "ANY"]
 MLUserDataEncryptionModeStringType = Literal["DISABLED", "SSE-KMS"]
+MetadataOperationType = Literal["CREATE"]
 NodeTypeType = Literal["CRAWLER", "JOB", "TRIGGER"]
 ParamTypeType = Literal["bool", "complex", "float", "int", "list", "null", "str"]
 ParquetCompressionTypeType = Literal["gzip", "lzo", "none", "snappy", "uncompressed"]
 PartitionIndexStatusType = Literal["ACTIVE", "CREATING", "DELETING", "FAILED"]
 PermissionType = Literal[
     "ALL",
     "ALTER",
@@ -316,15 +320,17 @@
     "CREATE_TABLE",
     "DATA_LOCATION_ACCESS",
     "DELETE",
     "DROP",
     "INSERT",
     "SELECT",
 ]
-PermissionTypeType = Literal["CELL_FILTER_PERMISSION", "COLUMN_PERMISSION"]
+PermissionTypeType = Literal[
+    "CELL_FILTER_PERMISSION", "COLUMN_PERMISSION", "NESTED_CELL_PERMISSION", "NESTED_PERMISSION"
+]
 PiiTypeType = Literal["ColumnAudit", "ColumnMasking", "RowAudit", "RowMasking"]
 PrincipalTypeType = Literal["GROUP", "ROLE", "USER"]
 QuoteCharType = Literal["disabled", "quillemet", "quote", "single_quote"]
 RecrawlBehaviorType = Literal["CRAWL_EVENT_MODE", "CRAWL_EVERYTHING", "CRAWL_NEW_FOLDERS_ONLY"]
 RegistryStatusType = Literal["AVAILABLE", "DELETING"]
 ResourceShareTypeType = Literal["ALL", "FEDERATED", "FOREIGN"]
 ResourceTypeType = Literal["ARCHIVE", "FILE", "JAR"]
@@ -382,14 +388,15 @@
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
@@ -485,14 +492,15 @@
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
@@ -571,26 +579,28 @@
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
@@ -758,26 +768,29 @@
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
+    "ap-southeast-4",
     "ca-central-1",
     "eu-central-1",
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

### Comparing `types-aiobotocore-glue-2.5.2.post3/types_aiobotocore_glue/paginator.py` & `types-aiobotocore-glue-2.5.4/types_aiobotocore_glue/paginator.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-glue-2.5.2.post3/types_aiobotocore_glue/paginator.pyi` & `types-aiobotocore-glue-2.5.4/types_aiobotocore_glue/paginator.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-glue-2.5.2.post3/types_aiobotocore_glue/type_defs.py` & `types-aiobotocore-glue-2.5.4/types_aiobotocore_glue/type_defs.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -104,15 +104,14 @@
 else:
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "NotificationPropertyTypeDef",
     "AggregateOperationTypeDef",
     "AmazonRedshiftAdvancedOptionTypeDef",
     "OptionTypeDef",
     "ApplyMappingTypeDef",
     "AuditContextTypeDef",
@@ -196,14 +195,16 @@
     "ConnectionPasswordEncryptionTypeDef",
     "ConnectionsListTypeDef",
     "CrawlTypeDef",
     "CrawlerHistoryTypeDef",
     "CrawlerMetricsTypeDef",
     "DeltaTargetTypeDef",
     "DynamoDBTargetTypeDef",
+    "HudiTargetTypeDef",
+    "IcebergTargetTypeDef",
     "JdbcTargetTypeDef",
     "MongoDBTargetTypeDef",
     "S3TargetTypeDef",
     "LakeFormationConfigurationTypeDef",
     "LastCrawlInfoTypeDef",
     "LineageConfigurationTypeDef",
     "RecrawlPolicyTypeDef",
@@ -332,14 +333,15 @@
     "GetUserDefinedFunctionsRequestRequestTypeDef",
     "GetWorkflowRequestRequestTypeDef",
     "GetWorkflowRunPropertiesRequestRequestTypeDef",
     "GetWorkflowRunRequestRequestTypeDef",
     "GetWorkflowRunsRequestRequestTypeDef",
     "GlueStudioSchemaColumnTypeDef",
     "S3SourceAdditionalOptionsTypeDef",
+    "IcebergInputTypeDef",
     "ImportCatalogToGlueRequestRequestTypeDef",
     "ImportLabelsTaskRunPropertiesTypeDef",
     "JDBCConnectorOptionsTypeDef",
     "PredecessorTypeDef",
     "JoinColumnTypeDef",
     "KeySchemaElementTypeDef",
     "LabelingSetGenerationTaskRunPropertiesTypeDef",
@@ -360,14 +362,15 @@
     "MappingTypeDef",
     "OtherMetadataValueListItemTypeDef",
     "MetadataKeyValuePairTypeDef",
     "OrderTypeDef",
     "PropertyPredicateTypeDef",
     "PutResourcePolicyRequestRequestTypeDef",
     "PutWorkflowRunPropertiesRequestRequestTypeDef",
+    "RecipeReferenceTypeDef",
     "UpsertRedshiftTargetOptionsTypeDef",
     "ResetJobBookmarkRequestRequestTypeDef",
     "ResourceUriTypeDef",
     "ResumeWorkflowRunRequestRequestTypeDef",
     "RunStatementRequestRequestTypeDef",
     "S3DirectSourceAdditionalOptionsTypeDef",
     "SortCriterionTypeDef",
@@ -404,14 +407,15 @@
     "UpdateSourceControlFromJobRequestRequestTypeDef",
     "UpdateWorkflowRequestRequestTypeDef",
     "WorkflowRunStatisticsTypeDef",
     "ActionTypeDef",
     "StartJobRunRequestRequestTypeDef",
     "AggregateTypeDef",
     "AmazonRedshiftNodeDataTypeDef",
+    "SnowflakeNodeDataTypeDef",
     "GetUnfilteredPartitionMetadataRequestRequestTypeDef",
     "GetUnfilteredTableMetadataRequestRequestTypeDef",
     "BackfillErrorTypeDef",
     "BatchDeletePartitionRequestRequestTypeDef",
     "BatchGetPartitionRequestRequestTypeDef",
     "CancelMLTaskRunResponseTypeDef",
     "CheckSchemaVersionValidityResponseTypeDef",
@@ -584,33 +588,36 @@
     "GetResourcePoliciesResponseTypeDef",
     "GetSchemaVersionInputRequestTypeDef",
     "GetSchemaVersionsDiffInputRequestTypeDef",
     "UpdateSchemaInputRequestTypeDef",
     "GlueSchemaTypeDef",
     "GovernedCatalogSourceTypeDef",
     "S3CatalogSourceTypeDef",
+    "OpenTableFormatInputTypeDef",
     "JobRunTypeDef",
     "JoinTypeDef",
     "TaskRunPropertiesTypeDef",
     "ListRegistriesResponseTypeDef",
     "ListSchemaVersionsResponseTypeDef",
     "ListSchemasResponseTypeDef",
     "TransformEncryptionTypeDef",
     "MetadataInfoTypeDef",
     "PutSchemaVersionMetadataInputRequestTypeDef",
     "QuerySchemaVersionMetadataInputRequestTypeDef",
     "RemoveSchemaVersionMetadataInputRequestTypeDef",
+    "RecipeTypeDef",
     "RedshiftTargetTypeDef",
     "UserDefinedFunctionInputTypeDef",
     "UserDefinedFunctionTypeDef",
     "SearchTablesRequestRequestTypeDef",
     "StatementOutputTypeDef",
     "UpdateClassifierRequestRequestTypeDef",
     "AmazonRedshiftSourceTypeDef",
     "AmazonRedshiftTargetTypeDef",
+    "SnowflakeTargetTypeDef",
     "PartitionIndexDescriptorTypeDef",
     "BatchStopJobRunResponseTypeDef",
     "BatchUpdatePartitionResponseTypeDef",
     "BatchCreatePartitionResponseTypeDef",
     "BatchDeletePartitionResponseTypeDef",
     "BatchDeleteTableResponseTypeDef",
     "BatchDeleteTableVersionResponseTypeDef",
@@ -675,14 +682,15 @@
     "S3CatalogDeltaSourceTypeDef",
     "S3CatalogHudiSourceTypeDef",
     "S3CsvSourceTypeDef",
     "S3DeltaSourceTypeDef",
     "S3HudiSourceTypeDef",
     "S3JsonSourceTypeDef",
     "S3ParquetSourceTypeDef",
+    "SnowflakeSourceTypeDef",
     "SparkConnectorSourceTypeDef",
     "SparkConnectorTargetTypeDef",
     "SparkSQLTypeDef",
     "GetJobRunResponseTypeDef",
     "GetJobRunsResponseTypeDef",
     "JobNodeDetailsTypeDef",
     "GetMLTaskRunResponseTypeDef",
@@ -865,22 +873,20 @@
     "_OptionalBatchDeleteConnectionRequestRequestTypeDef",
     {
         "CatalogId": str,
     },
     total=False,
 )
 
-
 class BatchDeleteConnectionRequestRequestTypeDef(
     _RequiredBatchDeleteConnectionRequestRequestTypeDef,
     _OptionalBatchDeleteConnectionRequestRequestTypeDef,
 ):
     pass
 
-
 ErrorDetailTypeDef = TypedDict(
     "ErrorDetailTypeDef",
     {
         "ErrorCode": str,
         "ErrorMessage": str,
     },
     total=False,
@@ -898,21 +904,19 @@
     {
         "CatalogId": str,
         "TransactionId": str,
     },
     total=False,
 )
 
-
 class BatchDeleteTableRequestRequestTypeDef(
     _RequiredBatchDeleteTableRequestRequestTypeDef, _OptionalBatchDeleteTableRequestRequestTypeDef
 ):
     pass
 
-
 _RequiredBatchDeleteTableVersionRequestRequestTypeDef = TypedDict(
     "_RequiredBatchDeleteTableVersionRequestRequestTypeDef",
     {
         "DatabaseName": str,
         "TableName": str,
         "VersionIds": Sequence[str],
     },
@@ -921,22 +925,20 @@
     "_OptionalBatchDeleteTableVersionRequestRequestTypeDef",
     {
         "CatalogId": str,
     },
     total=False,
 )
 
-
 class BatchDeleteTableVersionRequestRequestTypeDef(
     _RequiredBatchDeleteTableVersionRequestRequestTypeDef,
     _OptionalBatchDeleteTableVersionRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredBatchGetBlueprintsRequestRequestTypeDef = TypedDict(
     "_RequiredBatchGetBlueprintsRequestRequestTypeDef",
     {
         "Names": Sequence[str],
     },
 )
 _OptionalBatchGetBlueprintsRequestRequestTypeDef = TypedDict(
@@ -944,22 +946,20 @@
     {
         "IncludeBlueprint": bool,
         "IncludeParameterSpec": bool,
     },
     total=False,
 )
 
-
 class BatchGetBlueprintsRequestRequestTypeDef(
     _RequiredBatchGetBlueprintsRequestRequestTypeDef,
     _OptionalBatchGetBlueprintsRequestRequestTypeDef,
 ):
     pass
 
-
 BatchGetCrawlersRequestRequestTypeDef = TypedDict(
     "BatchGetCrawlersRequestRequestTypeDef",
     {
         "CrawlerNames": Sequence[str],
     },
 )
 
@@ -981,19 +981,17 @@
     "_OptionalCustomEntityTypeTypeDef",
     {
         "ContextWords": List[str],
     },
     total=False,
 )
 
-
 class CustomEntityTypeTypeDef(_RequiredCustomEntityTypeTypeDef, _OptionalCustomEntityTypeTypeDef):
     pass
 
-
 BatchGetDataQualityResultRequestRequestTypeDef = TypedDict(
     "BatchGetDataQualityResultRequestRequestTypeDef",
     {
         "ResultIds": Sequence[str],
     },
 )
 
@@ -1060,21 +1058,19 @@
     "_OptionalBatchGetWorkflowsRequestRequestTypeDef",
     {
         "IncludeGraph": bool,
     },
     total=False,
 )
 
-
 class BatchGetWorkflowsRequestRequestTypeDef(
     _RequiredBatchGetWorkflowsRequestRequestTypeDef, _OptionalBatchGetWorkflowsRequestRequestTypeDef
 ):
     pass
 
-
 BatchStopJobRunRequestRequestTypeDef = TypedDict(
     "BatchStopJobRunRequestRequestTypeDef",
     {
         "JobName": str,
         "JobRunIds": Sequence[str],
     },
 )
@@ -1177,21 +1173,19 @@
     "_OptionalCancelStatementRequestRequestTypeDef",
     {
         "RequestOrigin": str,
     },
     total=False,
 )
 
-
 class CancelStatementRequestRequestTypeDef(
     _RequiredCancelStatementRequestRequestTypeDef, _OptionalCancelStatementRequestRequestTypeDef
 ):
     pass
 
-
 CatalogEntryTypeDef = TypedDict(
     "CatalogEntryTypeDef",
     {
         "DatabaseName": str,
         "TableName": str,
     },
 )
@@ -1300,19 +1294,17 @@
         "ConnectionName": str,
         "EventQueueArn": str,
         "DlqEventQueueArn": str,
     },
     total=False,
 )
 
-
 class CatalogTargetTypeDef(_RequiredCatalogTargetTypeDef, _OptionalCatalogTargetTypeDef):
     pass
 
-
 CheckSchemaVersionValidityInputRequestTypeDef = TypedDict(
     "CheckSchemaVersionValidityInputRequestTypeDef",
     {
         "DataFormat": DataFormatType,
         "SchemaDefinition": str,
     },
 )
@@ -1337,19 +1329,17 @@
         "AllowSingleColumn": bool,
         "CustomDatatypeConfigured": bool,
         "CustomDatatypes": List[str],
     },
     total=False,
 )
 
-
 class CsvClassifierTypeDef(_RequiredCsvClassifierTypeDef, _OptionalCsvClassifierTypeDef):
     pass
 
-
 _RequiredGrokClassifierTypeDef = TypedDict(
     "_RequiredGrokClassifierTypeDef",
     {
         "Name": str,
         "Classification": str,
         "GrokPattern": str,
     },
@@ -1361,19 +1351,17 @@
         "LastUpdated": datetime,
         "Version": int,
         "CustomPatterns": str,
     },
     total=False,
 )
 
-
 class GrokClassifierTypeDef(_RequiredGrokClassifierTypeDef, _OptionalGrokClassifierTypeDef):
     pass
 
-
 _RequiredJsonClassifierTypeDef = TypedDict(
     "_RequiredJsonClassifierTypeDef",
     {
         "Name": str,
         "JsonPath": str,
     },
 )
@@ -1383,19 +1371,17 @@
         "CreationTime": datetime,
         "LastUpdated": datetime,
         "Version": int,
     },
     total=False,
 )
 
-
 class JsonClassifierTypeDef(_RequiredJsonClassifierTypeDef, _OptionalJsonClassifierTypeDef):
     pass
 
-
 _RequiredXMLClassifierTypeDef = TypedDict(
     "_RequiredXMLClassifierTypeDef",
     {
         "Name": str,
         "Classification": str,
     },
 )
@@ -1406,19 +1392,17 @@
         "LastUpdated": datetime,
         "Version": int,
         "RowTag": str,
     },
     total=False,
 )
 
-
 class XMLClassifierTypeDef(_RequiredXMLClassifierTypeDef, _OptionalXMLClassifierTypeDef):
     pass
 
-
 CloudWatchEncryptionTypeDef = TypedDict(
     "CloudWatchEncryptionTypeDef",
     {
         "CloudWatchEncryptionMode": CloudWatchEncryptionModeType,
         "KmsKeyArn": str,
     },
     total=False,
@@ -1438,19 +1422,17 @@
     "_OptionalDirectJDBCSourceTypeDef",
     {
         "RedshiftTmpDir": str,
     },
     total=False,
 )
 
-
 class DirectJDBCSourceTypeDef(_RequiredDirectJDBCSourceTypeDef, _OptionalDirectJDBCSourceTypeDef):
     pass
 
-
 _RequiredDropDuplicatesTypeDef = TypedDict(
     "_RequiredDropDuplicatesTypeDef",
     {
         "Name": str,
         "Inputs": List[str],
     },
 )
@@ -1458,19 +1440,17 @@
     "_OptionalDropDuplicatesTypeDef",
     {
         "Columns": List[List[str]],
     },
     total=False,
 )
 
-
 class DropDuplicatesTypeDef(_RequiredDropDuplicatesTypeDef, _OptionalDropDuplicatesTypeDef):
     pass
 
-
 DropFieldsTypeDef = TypedDict(
     "DropFieldsTypeDef",
     {
         "Name": str,
         "Inputs": List[str],
         "Paths": List[List[str]],
     },
@@ -1497,21 +1477,19 @@
     "_OptionalFillMissingValuesTypeDef",
     {
         "FilledPath": str,
     },
     total=False,
 )
 
-
 class FillMissingValuesTypeDef(
     _RequiredFillMissingValuesTypeDef, _OptionalFillMissingValuesTypeDef
 ):
     pass
 
-
 MergeTypeDef = TypedDict(
     "MergeTypeDef",
     {
         "Name": str,
         "Inputs": List[str],
         "Source": str,
         "PrimaryKeys": List[List[str]],
@@ -1591,19 +1569,17 @@
         "SampleFraction": float,
         "ThresholdFraction": float,
         "MaskValue": str,
     },
     total=False,
 )
 
-
 class PIIDetectionTypeDef(_RequiredPIIDetectionTypeDef, _OptionalPIIDetectionTypeDef):
     pass
 
-
 PostgreSQLCatalogSourceTypeDef = TypedDict(
     "PostgreSQLCatalogSourceTypeDef",
     {
         "Name": str,
         "Database": str,
         "Table": str,
     },
@@ -1632,19 +1608,17 @@
     {
         "RedshiftTmpDir": str,
         "TmpDirIAMRole": str,
     },
     total=False,
 )
 
-
 class RedshiftSourceTypeDef(_RequiredRedshiftSourceTypeDef, _OptionalRedshiftSourceTypeDef):
     pass
 
-
 RelationalCatalogSourceTypeDef = TypedDict(
     "RelationalCatalogSourceTypeDef",
     {
         "Name": str,
         "Database": str,
         "Table": str,
     },
@@ -1691,19 +1665,17 @@
     {
         "Topk": int,
         "Prob": float,
     },
     total=False,
 )
 
-
 class SpigotTypeDef(_RequiredSpigotTypeDef, _OptionalSpigotTypeDef):
     pass
 
-
 SplitFieldsTypeDef = TypedDict(
     "SplitFieldsTypeDef",
     {
         "Name": str,
         "Inputs": List[str],
         "Paths": List[List[str]],
     },
@@ -1729,19 +1701,17 @@
     "_OptionalCodeGenEdgeTypeDef",
     {
         "TargetParameter": str,
     },
     total=False,
 )
 
-
 class CodeGenEdgeTypeDef(_RequiredCodeGenEdgeTypeDef, _OptionalCodeGenEdgeTypeDef):
     pass
 
-
 _RequiredCodeGenNodeArgTypeDef = TypedDict(
     "_RequiredCodeGenNodeArgTypeDef",
     {
         "Name": str,
         "Value": str,
     },
 )
@@ -1749,19 +1719,17 @@
     "_OptionalCodeGenNodeArgTypeDef",
     {
         "Param": bool,
     },
     total=False,
 )
 
-
 class CodeGenNodeArgTypeDef(_RequiredCodeGenNodeArgTypeDef, _OptionalCodeGenNodeArgTypeDef):
     pass
 
-
 ColumnImportanceTypeDef = TypedDict(
     "ColumnImportanceTypeDef",
     {
         "ColumnName": str,
         "Importance": float,
     },
     total=False,
@@ -1788,21 +1756,19 @@
     {
         "MinimumValue": datetime,
         "MaximumValue": datetime,
     },
     total=False,
 )
 
-
 class DateColumnStatisticsDataTypeDef(
     _RequiredDateColumnStatisticsDataTypeDef, _OptionalDateColumnStatisticsDataTypeDef
 ):
     pass
 
-
 _RequiredDoubleColumnStatisticsDataTypeDef = TypedDict(
     "_RequiredDoubleColumnStatisticsDataTypeDef",
     {
         "NumberOfNulls": int,
         "NumberOfDistinctValues": int,
     },
 )
@@ -1811,21 +1777,19 @@
     {
         "MinimumValue": float,
         "MaximumValue": float,
     },
     total=False,
 )
 
-
 class DoubleColumnStatisticsDataTypeDef(
     _RequiredDoubleColumnStatisticsDataTypeDef, _OptionalDoubleColumnStatisticsDataTypeDef
 ):
     pass
 
-
 _RequiredLongColumnStatisticsDataTypeDef = TypedDict(
     "_RequiredLongColumnStatisticsDataTypeDef",
     {
         "NumberOfNulls": int,
         "NumberOfDistinctValues": int,
     },
 )
@@ -1834,21 +1798,19 @@
     {
         "MinimumValue": int,
         "MaximumValue": int,
     },
     total=False,
 )
 
-
 class LongColumnStatisticsDataTypeDef(
     _RequiredLongColumnStatisticsDataTypeDef, _OptionalLongColumnStatisticsDataTypeDef
 ):
     pass
 
-
 StringColumnStatisticsDataTypeDef = TypedDict(
     "StringColumnStatisticsDataTypeDef",
     {
         "MaximumLength": int,
         "AverageLength": float,
         "NumberOfNulls": int,
         "NumberOfDistinctValues": int,
@@ -1867,19 +1829,17 @@
         "Type": str,
         "Comment": str,
         "Parameters": Mapping[str, str],
     },
     total=False,
 )
 
-
 class ColumnTypeDef(_RequiredColumnTypeDef, _OptionalColumnTypeDef):
     pass
 
-
 ConditionTypeDef = TypedDict(
     "ConditionTypeDef",
     {
         "LogicalOperator": Literal["EQUALS"],
         "JobName": str,
         "State": JobRunStateType,
         "CrawlerName": str,
@@ -1919,21 +1879,19 @@
     "_OptionalConnectionPasswordEncryptionTypeDef",
     {
         "AwsKmsKeyId": str,
     },
     total=False,
 )
 
-
 class ConnectionPasswordEncryptionTypeDef(
     _RequiredConnectionPasswordEncryptionTypeDef, _OptionalConnectionPasswordEncryptionTypeDef
 ):
     pass
 
-
 ConnectionsListTypeDef = TypedDict(
     "ConnectionsListTypeDef",
     {
         "Connections": List[str],
     },
     total=False,
 )
@@ -2000,14 +1958,36 @@
         "Path": str,
         "scanAll": bool,
         "scanRate": float,
     },
     total=False,
 )
 
+HudiTargetTypeDef = TypedDict(
+    "HudiTargetTypeDef",
+    {
+        "Paths": List[str],
+        "ConnectionName": str,
+        "Exclusions": List[str],
+        "MaximumTraversalDepth": int,
+    },
+    total=False,
+)
+
+IcebergTargetTypeDef = TypedDict(
+    "IcebergTargetTypeDef",
+    {
+        "Paths": List[str],
+        "ConnectionName": str,
+        "Exclusions": List[str],
+        "MaximumTraversalDepth": int,
+    },
+    total=False,
+)
+
 JdbcTargetTypeDef = TypedDict(
     "JdbcTargetTypeDef",
     {
         "ConnectionName": str,
         "Path": str,
         "Exclusions": List[str],
         "EnableAdditionalMetadata": List[JdbcMetadataEntryType],
@@ -2116,21 +2096,19 @@
     {
         "Description": str,
         "Tags": Mapping[str, str],
     },
     total=False,
 )
 
-
 class CreateBlueprintRequestRequestTypeDef(
     _RequiredCreateBlueprintRequestRequestTypeDef, _OptionalCreateBlueprintRequestRequestTypeDef
 ):
     pass
 
-
 _RequiredCreateCsvClassifierRequestTypeDef = TypedDict(
     "_RequiredCreateCsvClassifierRequestTypeDef",
     {
         "Name": str,
     },
 )
 _OptionalCreateCsvClassifierRequestTypeDef = TypedDict(
@@ -2144,21 +2122,19 @@
         "AllowSingleColumn": bool,
         "CustomDatatypeConfigured": bool,
         "CustomDatatypes": Sequence[str],
     },
     total=False,
 )
 
-
 class CreateCsvClassifierRequestTypeDef(
     _RequiredCreateCsvClassifierRequestTypeDef, _OptionalCreateCsvClassifierRequestTypeDef
 ):
     pass
 
-
 _RequiredCreateGrokClassifierRequestTypeDef = TypedDict(
     "_RequiredCreateGrokClassifierRequestTypeDef",
     {
         "Classification": str,
         "Name": str,
         "GrokPattern": str,
     },
@@ -2167,21 +2143,19 @@
     "_OptionalCreateGrokClassifierRequestTypeDef",
     {
         "CustomPatterns": str,
     },
     total=False,
 )
 
-
 class CreateGrokClassifierRequestTypeDef(
     _RequiredCreateGrokClassifierRequestTypeDef, _OptionalCreateGrokClassifierRequestTypeDef
 ):
     pass
 
-
 CreateJsonClassifierRequestTypeDef = TypedDict(
     "CreateJsonClassifierRequestTypeDef",
     {
         "Name": str,
         "JsonPath": str,
     },
 )
@@ -2197,21 +2171,19 @@
     "_OptionalCreateXMLClassifierRequestTypeDef",
     {
         "RowTag": str,
     },
     total=False,
 )
 
-
 class CreateXMLClassifierRequestTypeDef(
     _RequiredCreateXMLClassifierRequestTypeDef, _OptionalCreateXMLClassifierRequestTypeDef
 ):
     pass
 
-
 _RequiredCreateCustomEntityTypeRequestRequestTypeDef = TypedDict(
     "_RequiredCreateCustomEntityTypeRequestRequestTypeDef",
     {
         "Name": str,
         "RegexString": str,
     },
 )
@@ -2220,22 +2192,20 @@
     {
         "ContextWords": Sequence[str],
         "Tags": Mapping[str, str],
     },
     total=False,
 )
 
-
 class CreateCustomEntityTypeRequestRequestTypeDef(
     _RequiredCreateCustomEntityTypeRequestRequestTypeDef,
     _OptionalCreateCustomEntityTypeRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredDataQualityTargetTableTypeDef = TypedDict(
     "_RequiredDataQualityTargetTableTypeDef",
     {
         "TableName": str,
         "DatabaseName": str,
     },
 )
@@ -2243,21 +2213,19 @@
     "_OptionalDataQualityTargetTableTypeDef",
     {
         "CatalogId": str,
     },
     total=False,
 )
 
-
 class DataQualityTargetTableTypeDef(
     _RequiredDataQualityTargetTableTypeDef, _OptionalDataQualityTargetTableTypeDef
 ):
     pass
 
-
 _RequiredCreateDevEndpointRequestRequestTypeDef = TypedDict(
     "_RequiredCreateDevEndpointRequestRequestTypeDef",
     {
         "EndpointName": str,
         "RoleArn": str,
     },
 )
@@ -2277,21 +2245,19 @@
         "SecurityConfiguration": str,
         "Tags": Mapping[str, str],
         "Arguments": Mapping[str, str],
     },
     total=False,
 )
 
-
 class CreateDevEndpointRequestRequestTypeDef(
     _RequiredCreateDevEndpointRequestRequestTypeDef, _OptionalCreateDevEndpointRequestRequestTypeDef
 ):
     pass
 
-
 ExecutionPropertyTypeDef = TypedDict(
     "ExecutionPropertyTypeDef",
     {
         "MaxConcurrentRuns": int,
     },
     total=False,
 )
@@ -2335,19 +2301,17 @@
         "CatalogId": str,
         "ConnectionName": str,
         "AdditionalOptions": Dict[str, str],
     },
     total=False,
 )
 
-
 class GlueTableTypeDef(_RequiredGlueTableTypeDef, _OptionalGlueTableTypeDef):
     pass
 
-
 PartitionIndexTypeDef = TypedDict(
     "PartitionIndexTypeDef",
     {
         "Keys": Sequence[str],
         "IndexName": str,
     },
 )
@@ -2363,21 +2327,19 @@
     {
         "Description": str,
         "Tags": Mapping[str, str],
     },
     total=False,
 )
 
-
 class CreateRegistryInputRequestTypeDef(
     _RequiredCreateRegistryInputRequestTypeDef, _OptionalCreateRegistryInputRequestTypeDef
 ):
     pass
 
-
 RegistryIdTypeDef = TypedDict(
     "RegistryIdTypeDef",
     {
         "RegistryName": str,
         "RegistryArn": str,
     },
     total=False,
@@ -2402,21 +2364,19 @@
     "_OptionalEventBatchingConditionTypeDef",
     {
         "BatchWindow": int,
     },
     total=False,
 )
 
-
 class EventBatchingConditionTypeDef(
     _RequiredEventBatchingConditionTypeDef, _OptionalEventBatchingConditionTypeDef
 ):
     pass
 
-
 _RequiredCreateWorkflowRequestRequestTypeDef = TypedDict(
     "_RequiredCreateWorkflowRequestRequestTypeDef",
     {
         "Name": str,
     },
 )
 _OptionalCreateWorkflowRequestRequestTypeDef = TypedDict(
@@ -2426,21 +2386,19 @@
         "DefaultRunProperties": Mapping[str, str],
         "Tags": Mapping[str, str],
         "MaxConcurrentRuns": int,
     },
     total=False,
 )
 
-
 class CreateWorkflowRequestRequestTypeDef(
     _RequiredCreateWorkflowRequestRequestTypeDef, _OptionalCreateWorkflowRequestRequestTypeDef
 ):
     pass
 
-
 DQResultsPublishingOptionsTypeDef = TypedDict(
     "DQResultsPublishingOptionsTypeDef",
     {
         "EvaluationContext": str,
         "ResultsS3Prefix": str,
         "CloudWatchMetricsEnabled": bool,
         "ResultsPublishingEnabled": bool,
@@ -2466,19 +2424,17 @@
     "_OptionalEncryptionAtRestTypeDef",
     {
         "SseAwsKmsKeyId": str,
     },
     total=False,
 )
 
-
 class EncryptionAtRestTypeDef(_RequiredEncryptionAtRestTypeDef, _OptionalEncryptionAtRestTypeDef):
     pass
 
-
 DataLakePrincipalTypeDef = TypedDict(
     "DataLakePrincipalTypeDef",
     {
         "DataLakePrincipalIdentifier": str,
     },
     total=False,
 )
@@ -2567,22 +2523,20 @@
     "_OptionalDeleteColumnStatisticsForPartitionRequestRequestTypeDef",
     {
         "CatalogId": str,
     },
     total=False,
 )
 
-
 class DeleteColumnStatisticsForPartitionRequestRequestTypeDef(
     _RequiredDeleteColumnStatisticsForPartitionRequestRequestTypeDef,
     _OptionalDeleteColumnStatisticsForPartitionRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredDeleteColumnStatisticsForTableRequestRequestTypeDef = TypedDict(
     "_RequiredDeleteColumnStatisticsForTableRequestRequestTypeDef",
     {
         "DatabaseName": str,
         "TableName": str,
         "ColumnName": str,
     },
@@ -2591,43 +2545,39 @@
     "_OptionalDeleteColumnStatisticsForTableRequestRequestTypeDef",
     {
         "CatalogId": str,
     },
     total=False,
 )
 
-
 class DeleteColumnStatisticsForTableRequestRequestTypeDef(
     _RequiredDeleteColumnStatisticsForTableRequestRequestTypeDef,
     _OptionalDeleteColumnStatisticsForTableRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredDeleteConnectionRequestRequestTypeDef = TypedDict(
     "_RequiredDeleteConnectionRequestRequestTypeDef",
     {
         "ConnectionName": str,
     },
 )
 _OptionalDeleteConnectionRequestRequestTypeDef = TypedDict(
     "_OptionalDeleteConnectionRequestRequestTypeDef",
     {
         "CatalogId": str,
     },
     total=False,
 )
 
-
 class DeleteConnectionRequestRequestTypeDef(
     _RequiredDeleteConnectionRequestRequestTypeDef, _OptionalDeleteConnectionRequestRequestTypeDef
 ):
     pass
 
-
 DeleteCrawlerRequestRequestTypeDef = TypedDict(
     "DeleteCrawlerRequestRequestTypeDef",
     {
         "Name": str,
     },
 )
 
@@ -2655,21 +2605,19 @@
     "_OptionalDeleteDatabaseRequestRequestTypeDef",
     {
         "CatalogId": str,
     },
     total=False,
 )
 
-
 class DeleteDatabaseRequestRequestTypeDef(
     _RequiredDeleteDatabaseRequestRequestTypeDef, _OptionalDeleteDatabaseRequestRequestTypeDef
 ):
     pass
 
-
 DeleteDevEndpointRequestRequestTypeDef = TypedDict(
     "DeleteDevEndpointRequestRequestTypeDef",
     {
         "EndpointName": str,
     },
 )
 
@@ -2699,22 +2647,20 @@
     "_OptionalDeletePartitionIndexRequestRequestTypeDef",
     {
         "CatalogId": str,
     },
     total=False,
 )
 
-
 class DeletePartitionIndexRequestRequestTypeDef(
     _RequiredDeletePartitionIndexRequestRequestTypeDef,
     _OptionalDeletePartitionIndexRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredDeletePartitionRequestRequestTypeDef = TypedDict(
     "_RequiredDeletePartitionRequestRequestTypeDef",
     {
         "DatabaseName": str,
         "TableName": str,
         "PartitionValues": Sequence[str],
     },
@@ -2723,21 +2669,19 @@
     "_OptionalDeletePartitionRequestRequestTypeDef",
     {
         "CatalogId": str,
     },
     total=False,
 )
 
-
 class DeletePartitionRequestRequestTypeDef(
     _RequiredDeletePartitionRequestRequestTypeDef, _OptionalDeletePartitionRequestRequestTypeDef
 ):
     pass
 
-
 DeleteResourcePolicyRequestRequestTypeDef = TypedDict(
     "DeleteResourcePolicyRequestRequestTypeDef",
     {
         "PolicyHashCondition": str,
         "ResourceArn": str,
     },
     total=False,
@@ -2770,21 +2714,19 @@
     "_OptionalDeleteSessionRequestRequestTypeDef",
     {
         "RequestOrigin": str,
     },
     total=False,
 )
 
-
 class DeleteSessionRequestRequestTypeDef(
     _RequiredDeleteSessionRequestRequestTypeDef, _OptionalDeleteSessionRequestRequestTypeDef
 ):
     pass
 
-
 _RequiredDeleteTableRequestRequestTypeDef = TypedDict(
     "_RequiredDeleteTableRequestRequestTypeDef",
     {
         "DatabaseName": str,
         "Name": str,
     },
 )
@@ -2793,21 +2735,19 @@
     {
         "CatalogId": str,
         "TransactionId": str,
     },
     total=False,
 )
 
-
 class DeleteTableRequestRequestTypeDef(
     _RequiredDeleteTableRequestRequestTypeDef, _OptionalDeleteTableRequestRequestTypeDef
 ):
     pass
 
-
 _RequiredDeleteTableVersionRequestRequestTypeDef = TypedDict(
     "_RequiredDeleteTableVersionRequestRequestTypeDef",
     {
         "DatabaseName": str,
         "TableName": str,
         "VersionId": str,
     },
@@ -2816,22 +2756,20 @@
     "_OptionalDeleteTableVersionRequestRequestTypeDef",
     {
         "CatalogId": str,
     },
     total=False,
 )
 
-
 class DeleteTableVersionRequestRequestTypeDef(
     _RequiredDeleteTableVersionRequestRequestTypeDef,
     _OptionalDeleteTableVersionRequestRequestTypeDef,
 ):
     pass
 
-
 DeleteTriggerRequestRequestTypeDef = TypedDict(
     "DeleteTriggerRequestRequestTypeDef",
     {
         "Name": str,
     },
 )
 
@@ -2846,22 +2784,20 @@
     "_OptionalDeleteUserDefinedFunctionRequestRequestTypeDef",
     {
         "CatalogId": str,
     },
     total=False,
 )
 
-
 class DeleteUserDefinedFunctionRequestRequestTypeDef(
     _RequiredDeleteUserDefinedFunctionRequestRequestTypeDef,
     _OptionalDeleteUserDefinedFunctionRequestRequestTypeDef,
 ):
     pass
 
-
 DeleteWorkflowRequestRequestTypeDef = TypedDict(
     "DeleteWorkflowRequestRequestTypeDef",
     {
         "Name": str,
     },
 )
 
@@ -2910,21 +2846,19 @@
         "Value": List[str],
         "ListType": ParamTypeType,
         "IsOptional": bool,
     },
     total=False,
 )
 
-
 class TransformConfigParameterTypeDef(
     _RequiredTransformConfigParameterTypeDef, _OptionalTransformConfigParameterTypeDef
 ):
     pass
 
-
 EdgeTypeDef = TypedDict(
     "EdgeTypeDef",
     {
         "SourceId": str,
         "DestinationId": str,
     },
     total=False,
@@ -3015,21 +2949,19 @@
     {
         "IncludeBlueprint": bool,
         "IncludeParameterSpec": bool,
     },
     total=False,
 )
 
-
 class GetBlueprintRequestRequestTypeDef(
     _RequiredGetBlueprintRequestRequestTypeDef, _OptionalGetBlueprintRequestRequestTypeDef
 ):
     pass
 
-
 GetBlueprintRunRequestRequestTypeDef = TypedDict(
     "GetBlueprintRunRequestRequestTypeDef",
     {
         "BlueprintName": str,
         "RunId": str,
     },
 )
@@ -3045,21 +2977,19 @@
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
-
 class GetBlueprintRunsRequestRequestTypeDef(
     _RequiredGetBlueprintRunsRequestRequestTypeDef, _OptionalGetBlueprintRunsRequestRequestTypeDef
 ):
     pass
 
-
 GetCatalogImportStatusRequestRequestTypeDef = TypedDict(
     "GetCatalogImportStatusRequestRequestTypeDef",
     {
         "CatalogId": str,
     },
     total=False,
 )
@@ -3103,22 +3033,20 @@
     "_OptionalGetColumnStatisticsForPartitionRequestRequestTypeDef",
     {
         "CatalogId": str,
     },
     total=False,
 )
 
-
 class GetColumnStatisticsForPartitionRequestRequestTypeDef(
     _RequiredGetColumnStatisticsForPartitionRequestRequestTypeDef,
     _OptionalGetColumnStatisticsForPartitionRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredGetColumnStatisticsForTableRequestRequestTypeDef = TypedDict(
     "_RequiredGetColumnStatisticsForTableRequestRequestTypeDef",
     {
         "DatabaseName": str,
         "TableName": str,
         "ColumnNames": Sequence[str],
     },
@@ -3127,22 +3055,20 @@
     "_OptionalGetColumnStatisticsForTableRequestRequestTypeDef",
     {
         "CatalogId": str,
     },
     total=False,
 )
 
-
 class GetColumnStatisticsForTableRequestRequestTypeDef(
     _RequiredGetColumnStatisticsForTableRequestRequestTypeDef,
     _OptionalGetColumnStatisticsForTableRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredGetConnectionRequestRequestTypeDef = TypedDict(
     "_RequiredGetConnectionRequestRequestTypeDef",
     {
         "Name": str,
     },
 )
 _OptionalGetConnectionRequestRequestTypeDef = TypedDict(
@@ -3150,21 +3076,19 @@
     {
         "CatalogId": str,
         "HidePassword": bool,
     },
     total=False,
 )
 
-
 class GetConnectionRequestRequestTypeDef(
     _RequiredGetConnectionRequestRequestTypeDef, _OptionalGetConnectionRequestRequestTypeDef
 ):
     pass
 
-
 GetConnectionsFilterTypeDef = TypedDict(
     "GetConnectionsFilterTypeDef",
     {
         "MatchCriteria": Sequence[str],
         "ConnectionType": ConnectionTypeType,
     },
     total=False,
@@ -3249,21 +3173,19 @@
     "_OptionalGetDatabaseRequestRequestTypeDef",
     {
         "CatalogId": str,
     },
     total=False,
 )
 
-
 class GetDatabaseRequestRequestTypeDef(
     _RequiredGetDatabaseRequestRequestTypeDef, _OptionalGetDatabaseRequestRequestTypeDef
 ):
     pass
 
-
 GetDatabasesRequestRequestTypeDef = TypedDict(
     "GetDatabasesRequestRequestTypeDef",
     {
         "CatalogId": str,
         "NextToken": str,
         "MaxResults": int,
         "ResourceShareType": ResourceShareTypeType,
@@ -3305,21 +3227,19 @@
     "_OptionalGetJobBookmarkRequestRequestTypeDef",
     {
         "RunId": str,
     },
     total=False,
 )
 
-
 class GetJobBookmarkRequestRequestTypeDef(
     _RequiredGetJobBookmarkRequestRequestTypeDef, _OptionalGetJobBookmarkRequestRequestTypeDef
 ):
     pass
 
-
 JobBookmarkEntryTypeDef = TypedDict(
     "JobBookmarkEntryTypeDef",
     {
         "JobName": str,
         "Version": int,
         "Run": int,
         "Attempt": int,
@@ -3348,21 +3268,19 @@
     "_OptionalGetJobRunRequestRequestTypeDef",
     {
         "PredecessorsIncluded": bool,
     },
     total=False,
 )
 
-
 class GetJobRunRequestRequestTypeDef(
     _RequiredGetJobRunRequestRequestTypeDef, _OptionalGetJobRunRequestRequestTypeDef
 ):
     pass
 
-
 _RequiredGetJobRunsRequestRequestTypeDef = TypedDict(
     "_RequiredGetJobRunsRequestRequestTypeDef",
     {
         "JobName": str,
     },
 )
 _OptionalGetJobRunsRequestRequestTypeDef = TypedDict(
@@ -3370,21 +3288,19 @@
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
-
 class GetJobRunsRequestRequestTypeDef(
     _RequiredGetJobRunsRequestRequestTypeDef, _OptionalGetJobRunsRequestRequestTypeDef
 ):
     pass
 
-
 GetJobsRequestRequestTypeDef = TypedDict(
     "GetJobsRequestRequestTypeDef",
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
@@ -3455,22 +3371,20 @@
     {
         "CatalogId": str,
         "NextToken": str,
     },
     total=False,
 )
 
-
 class GetPartitionIndexesRequestRequestTypeDef(
     _RequiredGetPartitionIndexesRequestRequestTypeDef,
     _OptionalGetPartitionIndexesRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredGetPartitionRequestRequestTypeDef = TypedDict(
     "_RequiredGetPartitionRequestRequestTypeDef",
     {
         "DatabaseName": str,
         "TableName": str,
         "PartitionValues": Sequence[str],
     },
@@ -3479,21 +3393,19 @@
     "_OptionalGetPartitionRequestRequestTypeDef",
     {
         "CatalogId": str,
     },
     total=False,
 )
 
-
 class GetPartitionRequestRequestTypeDef(
     _RequiredGetPartitionRequestRequestTypeDef, _OptionalGetPartitionRequestRequestTypeDef
 ):
     pass
 
-
 SegmentTypeDef = TypedDict(
     "SegmentTypeDef",
     {
         "SegmentNumber": int,
         "TotalSegments": int,
     },
 )
@@ -3561,21 +3473,19 @@
     "_OptionalGetSessionRequestRequestTypeDef",
     {
         "RequestOrigin": str,
     },
     total=False,
 )
 
-
 class GetSessionRequestRequestTypeDef(
     _RequiredGetSessionRequestRequestTypeDef, _OptionalGetSessionRequestRequestTypeDef
 ):
     pass
 
-
 _RequiredGetStatementRequestRequestTypeDef = TypedDict(
     "_RequiredGetStatementRequestRequestTypeDef",
     {
         "SessionId": str,
         "Id": int,
     },
 )
@@ -3583,21 +3493,19 @@
     "_OptionalGetStatementRequestRequestTypeDef",
     {
         "RequestOrigin": str,
     },
     total=False,
 )
 
-
 class GetStatementRequestRequestTypeDef(
     _RequiredGetStatementRequestRequestTypeDef, _OptionalGetStatementRequestRequestTypeDef
 ):
     pass
 
-
 _RequiredGetTableVersionRequestRequestTypeDef = TypedDict(
     "_RequiredGetTableVersionRequestRequestTypeDef",
     {
         "DatabaseName": str,
         "TableName": str,
     },
 )
@@ -3606,21 +3514,19 @@
     {
         "CatalogId": str,
         "VersionId": str,
     },
     total=False,
 )
 
-
 class GetTableVersionRequestRequestTypeDef(
     _RequiredGetTableVersionRequestRequestTypeDef, _OptionalGetTableVersionRequestRequestTypeDef
 ):
     pass
 
-
 _RequiredGetTableVersionsRequestRequestTypeDef = TypedDict(
     "_RequiredGetTableVersionsRequestRequestTypeDef",
     {
         "DatabaseName": str,
         "TableName": str,
     },
 )
@@ -3630,21 +3536,19 @@
         "CatalogId": str,
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
-
 class GetTableVersionsRequestRequestTypeDef(
     _RequiredGetTableVersionsRequestRequestTypeDef, _OptionalGetTableVersionsRequestRequestTypeDef
 ):
     pass
 
-
 GetTagsRequestRequestTypeDef = TypedDict(
     "GetTagsRequestRequestTypeDef",
     {
         "ResourceArn": str,
     },
 )
 
@@ -3676,22 +3580,20 @@
     "_OptionalGetUserDefinedFunctionRequestRequestTypeDef",
     {
         "CatalogId": str,
     },
     total=False,
 )
 
-
 class GetUserDefinedFunctionRequestRequestTypeDef(
     _RequiredGetUserDefinedFunctionRequestRequestTypeDef,
     _OptionalGetUserDefinedFunctionRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredGetUserDefinedFunctionsRequestRequestTypeDef = TypedDict(
     "_RequiredGetUserDefinedFunctionsRequestRequestTypeDef",
     {
         "Pattern": str,
     },
 )
 _OptionalGetUserDefinedFunctionsRequestRequestTypeDef = TypedDict(
@@ -3701,43 +3603,39 @@
         "DatabaseName": str,
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
-
 class GetUserDefinedFunctionsRequestRequestTypeDef(
     _RequiredGetUserDefinedFunctionsRequestRequestTypeDef,
     _OptionalGetUserDefinedFunctionsRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredGetWorkflowRequestRequestTypeDef = TypedDict(
     "_RequiredGetWorkflowRequestRequestTypeDef",
     {
         "Name": str,
     },
 )
 _OptionalGetWorkflowRequestRequestTypeDef = TypedDict(
     "_OptionalGetWorkflowRequestRequestTypeDef",
     {
         "IncludeGraph": bool,
     },
     total=False,
 )
 
-
 class GetWorkflowRequestRequestTypeDef(
     _RequiredGetWorkflowRequestRequestTypeDef, _OptionalGetWorkflowRequestRequestTypeDef
 ):
     pass
 
-
 GetWorkflowRunPropertiesRequestRequestTypeDef = TypedDict(
     "GetWorkflowRunPropertiesRequestRequestTypeDef",
     {
         "Name": str,
         "RunId": str,
     },
 )
@@ -3753,21 +3651,19 @@
     "_OptionalGetWorkflowRunRequestRequestTypeDef",
     {
         "IncludeGraph": bool,
     },
     total=False,
 )
 
-
 class GetWorkflowRunRequestRequestTypeDef(
     _RequiredGetWorkflowRunRequestRequestTypeDef, _OptionalGetWorkflowRunRequestRequestTypeDef
 ):
     pass
 
-
 _RequiredGetWorkflowRunsRequestRequestTypeDef = TypedDict(
     "_RequiredGetWorkflowRunsRequestRequestTypeDef",
     {
         "Name": str,
     },
 )
 _OptionalGetWorkflowRunsRequestRequestTypeDef = TypedDict(
@@ -3776,51 +3672,64 @@
         "IncludeGraph": bool,
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
-
 class GetWorkflowRunsRequestRequestTypeDef(
     _RequiredGetWorkflowRunsRequestRequestTypeDef, _OptionalGetWorkflowRunsRequestRequestTypeDef
 ):
     pass
 
-
 _RequiredGlueStudioSchemaColumnTypeDef = TypedDict(
     "_RequiredGlueStudioSchemaColumnTypeDef",
     {
         "Name": str,
     },
 )
 _OptionalGlueStudioSchemaColumnTypeDef = TypedDict(
     "_OptionalGlueStudioSchemaColumnTypeDef",
     {
         "Type": str,
     },
     total=False,
 )
 
-
 class GlueStudioSchemaColumnTypeDef(
     _RequiredGlueStudioSchemaColumnTypeDef, _OptionalGlueStudioSchemaColumnTypeDef
 ):
     pass
 
-
 S3SourceAdditionalOptionsTypeDef = TypedDict(
     "S3SourceAdditionalOptionsTypeDef",
     {
         "BoundedSize": int,
         "BoundedFiles": int,
     },
     total=False,
 )
 
+_RequiredIcebergInputTypeDef = TypedDict(
+    "_RequiredIcebergInputTypeDef",
+    {
+        "MetadataOperation": Literal["CREATE"],
+    },
+)
+_OptionalIcebergInputTypeDef = TypedDict(
+    "_OptionalIcebergInputTypeDef",
+    {
+        "Version": str,
+    },
+    total=False,
+)
+
+class IcebergInputTypeDef(_RequiredIcebergInputTypeDef, _OptionalIcebergInputTypeDef):
+    pass
+
 ImportCatalogToGlueRequestRequestTypeDef = TypedDict(
     "ImportCatalogToGlueRequestRequestTypeDef",
     {
         "CatalogId": str,
     },
     total=False,
 )
@@ -4002,21 +3911,19 @@
     {
         "RequestOrigin": str,
         "NextToken": str,
     },
     total=False,
 )
 
-
 class ListStatementsRequestRequestTypeDef(
     _RequiredListStatementsRequestRequestTypeDef, _OptionalListStatementsRequestRequestTypeDef
 ):
     pass
 
-
 ListTriggersRequestRequestTypeDef = TypedDict(
     "ListTriggersRequestRequestTypeDef",
     {
         "NextToken": str,
         "DependentJobName": str,
         "MaxResults": int,
         "Tags": Mapping[str, str],
@@ -4043,21 +3950,19 @@
     "_OptionalMLUserDataEncryptionTypeDef",
     {
         "KmsKeyId": str,
     },
     total=False,
 )
 
-
 class MLUserDataEncryptionTypeDef(
     _RequiredMLUserDataEncryptionTypeDef, _OptionalMLUserDataEncryptionTypeDef
 ):
     pass
 
-
 MappingTypeDef = TypedDict(
     "MappingTypeDef",
     {
         "ToKey": str,
         "FromPath": List[str],
         "FromType": str,
         "ToType": str,
@@ -4116,30 +4021,36 @@
         "PolicyHashCondition": str,
         "PolicyExistsCondition": ExistConditionType,
         "EnableHybrid": EnableHybridValuesType,
     },
     total=False,
 )
 
-
 class PutResourcePolicyRequestRequestTypeDef(
     _RequiredPutResourcePolicyRequestRequestTypeDef, _OptionalPutResourcePolicyRequestRequestTypeDef
 ):
     pass
 
-
 PutWorkflowRunPropertiesRequestRequestTypeDef = TypedDict(
     "PutWorkflowRunPropertiesRequestRequestTypeDef",
     {
         "Name": str,
         "RunId": str,
         "RunProperties": Mapping[str, str],
     },
 )
 
+RecipeReferenceTypeDef = TypedDict(
+    "RecipeReferenceTypeDef",
+    {
+        "RecipeArn": str,
+        "RecipeVersion": str,
+    },
+)
+
 UpsertRedshiftTargetOptionsTypeDef = TypedDict(
     "UpsertRedshiftTargetOptionsTypeDef",
     {
         "TableLocation": str,
         "ConnectionName": str,
         "UpsertKeys": List[str],
     },
@@ -4156,21 +4067,19 @@
     "_OptionalResetJobBookmarkRequestRequestTypeDef",
     {
         "RunId": str,
     },
     total=False,
 )
 
-
 class ResetJobBookmarkRequestRequestTypeDef(
     _RequiredResetJobBookmarkRequestRequestTypeDef, _OptionalResetJobBookmarkRequestRequestTypeDef
 ):
     pass
 
-
 ResourceUriTypeDef = TypedDict(
     "ResourceUriTypeDef",
     {
         "ResourceType": ResourceTypeType,
         "Uri": str,
     },
     total=False,
@@ -4196,21 +4105,19 @@
     "_OptionalRunStatementRequestRequestTypeDef",
     {
         "RequestOrigin": str,
     },
     total=False,
 )
 
-
 class RunStatementRequestRequestTypeDef(
     _RequiredRunStatementRequestRequestTypeDef, _OptionalRunStatementRequestRequestTypeDef
 ):
     pass
 
-
 S3DirectSourceAdditionalOptionsTypeDef = TypedDict(
     "S3DirectSourceAdditionalOptionsTypeDef",
     {
         "BoundedSize": int,
         "BoundedFiles": int,
         "EnableSamplePath": bool,
         "SamplePath": str,
@@ -4266,21 +4173,19 @@
     "_OptionalStartBlueprintRunRequestRequestTypeDef",
     {
         "Parameters": str,
     },
     total=False,
 )
 
-
 class StartBlueprintRunRequestRequestTypeDef(
     _RequiredStartBlueprintRunRequestRequestTypeDef, _OptionalStartBlueprintRunRequestRequestTypeDef
 ):
     pass
 
-
 StartCrawlerRequestRequestTypeDef = TypedDict(
     "StartCrawlerRequestRequestTypeDef",
     {
         "Name": str,
     },
 )
 
@@ -4310,22 +4215,20 @@
     "_OptionalStartImportLabelsTaskRunRequestRequestTypeDef",
     {
         "ReplaceAllLabels": bool,
     },
     total=False,
 )
 
-
 class StartImportLabelsTaskRunRequestRequestTypeDef(
     _RequiredStartImportLabelsTaskRunRequestRequestTypeDef,
     _OptionalStartImportLabelsTaskRunRequestRequestTypeDef,
 ):
     pass
 
-
 StartMLEvaluationTaskRunRequestRequestTypeDef = TypedDict(
     "StartMLEvaluationTaskRunRequestRequestTypeDef",
     {
         "TransformId": str,
     },
 )
 
@@ -4354,21 +4257,19 @@
     "_OptionalStartWorkflowRunRequestRequestTypeDef",
     {
         "RunProperties": Mapping[str, str],
     },
     total=False,
 )
 
-
 class StartWorkflowRunRequestRequestTypeDef(
     _RequiredStartWorkflowRunRequestRequestTypeDef, _OptionalStartWorkflowRunRequestRequestTypeDef
 ):
     pass
 
-
 StartingEventBatchConditionTypeDef = TypedDict(
     "StartingEventBatchConditionTypeDef",
     {
         "BatchSize": int,
         "BatchWindow": int,
     },
     total=False,
@@ -4406,21 +4307,19 @@
     "_OptionalStopSessionRequestRequestTypeDef",
     {
         "RequestOrigin": str,
     },
     total=False,
 )
 
-
 class StopSessionRequestRequestTypeDef(
     _RequiredStopSessionRequestRequestTypeDef, _OptionalStopSessionRequestRequestTypeDef
 ):
     pass
 
-
 StopTriggerRequestRequestTypeDef = TypedDict(
     "StopTriggerRequestRequestTypeDef",
     {
         "Name": str,
     },
 )
 
@@ -4470,21 +4369,19 @@
     "_OptionalUpdateBlueprintRequestRequestTypeDef",
     {
         "Description": str,
     },
     total=False,
 )
 
-
 class UpdateBlueprintRequestRequestTypeDef(
     _RequiredUpdateBlueprintRequestRequestTypeDef, _OptionalUpdateBlueprintRequestRequestTypeDef
 ):
     pass
 
-
 _RequiredUpdateCsvClassifierRequestTypeDef = TypedDict(
     "_RequiredUpdateCsvClassifierRequestTypeDef",
     {
         "Name": str,
     },
 )
 _OptionalUpdateCsvClassifierRequestTypeDef = TypedDict(
@@ -4498,21 +4395,19 @@
         "AllowSingleColumn": bool,
         "CustomDatatypeConfigured": bool,
         "CustomDatatypes": Sequence[str],
     },
     total=False,
 )
 
-
 class UpdateCsvClassifierRequestTypeDef(
     _RequiredUpdateCsvClassifierRequestTypeDef, _OptionalUpdateCsvClassifierRequestTypeDef
 ):
     pass
 
-
 _RequiredUpdateGrokClassifierRequestTypeDef = TypedDict(
     "_RequiredUpdateGrokClassifierRequestTypeDef",
     {
         "Name": str,
     },
 )
 _OptionalUpdateGrokClassifierRequestTypeDef = TypedDict(
@@ -4521,42 +4416,38 @@
         "Classification": str,
         "GrokPattern": str,
         "CustomPatterns": str,
     },
     total=False,
 )
 
-
 class UpdateGrokClassifierRequestTypeDef(
     _RequiredUpdateGrokClassifierRequestTypeDef, _OptionalUpdateGrokClassifierRequestTypeDef
 ):
     pass
 
-
 _RequiredUpdateJsonClassifierRequestTypeDef = TypedDict(
     "_RequiredUpdateJsonClassifierRequestTypeDef",
     {
         "Name": str,
     },
 )
 _OptionalUpdateJsonClassifierRequestTypeDef = TypedDict(
     "_OptionalUpdateJsonClassifierRequestTypeDef",
     {
         "JsonPath": str,
     },
     total=False,
 )
 
-
 class UpdateJsonClassifierRequestTypeDef(
     _RequiredUpdateJsonClassifierRequestTypeDef, _OptionalUpdateJsonClassifierRequestTypeDef
 ):
     pass
 
-
 _RequiredUpdateXMLClassifierRequestTypeDef = TypedDict(
     "_RequiredUpdateXMLClassifierRequestTypeDef",
     {
         "Name": str,
     },
 )
 _OptionalUpdateXMLClassifierRequestTypeDef = TypedDict(
@@ -4564,43 +4455,39 @@
     {
         "Classification": str,
         "RowTag": str,
     },
     total=False,
 )
 
-
 class UpdateXMLClassifierRequestTypeDef(
     _RequiredUpdateXMLClassifierRequestTypeDef, _OptionalUpdateXMLClassifierRequestTypeDef
 ):
     pass
 
-
 _RequiredUpdateCrawlerScheduleRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateCrawlerScheduleRequestRequestTypeDef",
     {
         "CrawlerName": str,
     },
 )
 _OptionalUpdateCrawlerScheduleRequestRequestTypeDef = TypedDict(
     "_OptionalUpdateCrawlerScheduleRequestRequestTypeDef",
     {
         "Schedule": str,
     },
     total=False,
 )
 
-
 class UpdateCrawlerScheduleRequestRequestTypeDef(
     _RequiredUpdateCrawlerScheduleRequestRequestTypeDef,
     _OptionalUpdateCrawlerScheduleRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredUpdateDataQualityRulesetRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateDataQualityRulesetRequestRequestTypeDef",
     {
         "Name": str,
     },
 )
 _OptionalUpdateDataQualityRulesetRequestRequestTypeDef = TypedDict(
@@ -4608,22 +4495,20 @@
     {
         "Description": str,
         "Ruleset": str,
     },
     total=False,
 )
 
-
 class UpdateDataQualityRulesetRequestRequestTypeDef(
     _RequiredUpdateDataQualityRulesetRequestRequestTypeDef,
     _OptionalUpdateDataQualityRulesetRequestRequestTypeDef,
 ):
     pass
 
-
 UpdateJobFromSourceControlRequestRequestTypeDef = TypedDict(
     "UpdateJobFromSourceControlRequestRequestTypeDef",
     {
         "JobName": str,
         "Provider": SourceControlProviderType,
         "RepositoryName": str,
         "RepositoryOwner": str,
@@ -4664,21 +4549,19 @@
         "Description": str,
         "DefaultRunProperties": Mapping[str, str],
         "MaxConcurrentRuns": int,
     },
     total=False,
 )
 
-
 class UpdateWorkflowRequestRequestTypeDef(
     _RequiredUpdateWorkflowRequestRequestTypeDef, _OptionalUpdateWorkflowRequestRequestTypeDef
 ):
     pass
 
-
 WorkflowRunStatisticsTypeDef = TypedDict(
     "WorkflowRunStatisticsTypeDef",
     {
         "TotalActions": int,
         "TimeoutActions": int,
         "FailedActions": int,
         "StoppedActions": int,
@@ -4722,21 +4605,19 @@
         "WorkerType": WorkerTypeType,
         "NumberOfWorkers": int,
         "ExecutionClass": ExecutionClassType,
     },
     total=False,
 )
 
-
 class StartJobRunRequestRequestTypeDef(
     _RequiredStartJobRunRequestRequestTypeDef, _OptionalStartJobRunRequestRequestTypeDef
 ):
     pass
 
-
 AggregateTypeDef = TypedDict(
     "AggregateTypeDef",
     {
         "Name": str,
         "Inputs": List[str],
         "Groups": List[List[str]],
         "Aggs": List[AggregateOperationTypeDef],
@@ -4772,14 +4653,42 @@
         "TableSchema": List[OptionTypeDef],
         "StagingTable": str,
         "SelectedColumns": List[OptionTypeDef],
     },
     total=False,
 )
 
+SnowflakeNodeDataTypeDef = TypedDict(
+    "SnowflakeNodeDataTypeDef",
+    {
+        "SourceType": str,
+        "Connection": OptionTypeDef,
+        "Schema": str,
+        "Table": str,
+        "Database": str,
+        "TempDir": str,
+        "IamRole": OptionTypeDef,
+        "AdditionalOptions": Dict[str, str],
+        "SampleQuery": str,
+        "PreAction": str,
+        "PostAction": str,
+        "Action": str,
+        "Upsert": bool,
+        "MergeAction": str,
+        "MergeWhenMatched": str,
+        "MergeWhenNotMatched": str,
+        "MergeClause": str,
+        "StagingTable": str,
+        "SelectedColumns": List[OptionTypeDef],
+        "AutoPushdown": bool,
+        "TableSchema": List[OptionTypeDef],
+    },
+    total=False,
+)
+
 _RequiredGetUnfilteredPartitionMetadataRequestRequestTypeDef = TypedDict(
     "_RequiredGetUnfilteredPartitionMetadataRequestRequestTypeDef",
     {
         "CatalogId": str,
         "DatabaseName": str,
         "TableName": str,
         "PartitionValues": Sequence[str],
@@ -4790,22 +4699,20 @@
     "_OptionalGetUnfilteredPartitionMetadataRequestRequestTypeDef",
     {
         "AuditContext": AuditContextTypeDef,
     },
     total=False,
 )
 
-
 class GetUnfilteredPartitionMetadataRequestRequestTypeDef(
     _RequiredGetUnfilteredPartitionMetadataRequestRequestTypeDef,
     _OptionalGetUnfilteredPartitionMetadataRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredGetUnfilteredTableMetadataRequestRequestTypeDef = TypedDict(
     "_RequiredGetUnfilteredTableMetadataRequestRequestTypeDef",
     {
         "CatalogId": str,
         "DatabaseName": str,
         "Name": str,
         "SupportedPermissionTypes": Sequence[PermissionTypeType],
@@ -4815,22 +4722,20 @@
     "_OptionalGetUnfilteredTableMetadataRequestRequestTypeDef",
     {
         "AuditContext": AuditContextTypeDef,
     },
     total=False,
 )
 
-
 class GetUnfilteredTableMetadataRequestRequestTypeDef(
     _RequiredGetUnfilteredTableMetadataRequestRequestTypeDef,
     _OptionalGetUnfilteredTableMetadataRequestRequestTypeDef,
 ):
     pass
 
-
 BackfillErrorTypeDef = TypedDict(
     "BackfillErrorTypeDef",
     {
         "Code": BackfillErrorCodeType,
         "Partitions": List[PartitionValueListTypeDef],
     },
     total=False,
@@ -4848,22 +4753,20 @@
     "_OptionalBatchDeletePartitionRequestRequestTypeDef",
     {
         "CatalogId": str,
     },
     total=False,
 )
 
-
 class BatchDeletePartitionRequestRequestTypeDef(
     _RequiredBatchDeletePartitionRequestRequestTypeDef,
     _OptionalBatchDeletePartitionRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredBatchGetPartitionRequestRequestTypeDef = TypedDict(
     "_RequiredBatchGetPartitionRequestRequestTypeDef",
     {
         "DatabaseName": str,
         "TableName": str,
         "PartitionsToGet": Sequence[PartitionValueListTypeDef],
     },
@@ -4872,21 +4775,19 @@
     "_OptionalBatchGetPartitionRequestRequestTypeDef",
     {
         "CatalogId": str,
     },
     total=False,
 )
 
-
 class BatchGetPartitionRequestRequestTypeDef(
     _RequiredBatchGetPartitionRequestRequestTypeDef, _OptionalBatchGetPartitionRequestRequestTypeDef
 ):
     pass
 
-
 CancelMLTaskRunResponseTypeDef = TypedDict(
     "CancelMLTaskRunResponseTypeDef",
     {
         "TransformId": str,
         "TaskRunId": str,
         "Status": TaskStatusTypeType,
         "ResponseMetadata": ResponseMetadataTypeDef,
@@ -5690,21 +5591,19 @@
         "DetectSchema": bool,
         "StreamingOptions": KafkaStreamingSourceOptionsTypeDef,
         "DataPreviewOptions": StreamingDataPreviewOptionsTypeDef,
     },
     total=False,
 )
 
-
 class CatalogKafkaSourceTypeDef(
     _RequiredCatalogKafkaSourceTypeDef, _OptionalCatalogKafkaSourceTypeDef
 ):
     pass
 
-
 _RequiredDirectKafkaSourceTypeDef = TypedDict(
     "_RequiredDirectKafkaSourceTypeDef",
     {
         "Name": str,
     },
 )
 _OptionalDirectKafkaSourceTypeDef = TypedDict(
@@ -5714,21 +5613,19 @@
         "WindowSize": int,
         "DetectSchema": bool,
         "DataPreviewOptions": StreamingDataPreviewOptionsTypeDef,
     },
     total=False,
 )
 
-
 class DirectKafkaSourceTypeDef(
     _RequiredDirectKafkaSourceTypeDef, _OptionalDirectKafkaSourceTypeDef
 ):
     pass
 
-
 _RequiredCatalogKinesisSourceTypeDef = TypedDict(
     "_RequiredCatalogKinesisSourceTypeDef",
     {
         "Name": str,
         "Table": str,
         "Database": str,
     },
@@ -5740,21 +5637,19 @@
         "DetectSchema": bool,
         "StreamingOptions": KinesisStreamingSourceOptionsTypeDef,
         "DataPreviewOptions": StreamingDataPreviewOptionsTypeDef,
     },
     total=False,
 )
 
-
 class CatalogKinesisSourceTypeDef(
     _RequiredCatalogKinesisSourceTypeDef, _OptionalCatalogKinesisSourceTypeDef
 ):
     pass
 
-
 _RequiredDirectKinesisSourceTypeDef = TypedDict(
     "_RequiredDirectKinesisSourceTypeDef",
     {
         "Name": str,
     },
 )
 _OptionalDirectKinesisSourceTypeDef = TypedDict(
@@ -5764,21 +5659,19 @@
         "DetectSchema": bool,
         "StreamingOptions": KinesisStreamingSourceOptionsTypeDef,
         "DataPreviewOptions": StreamingDataPreviewOptionsTypeDef,
     },
     total=False,
 )
 
-
 class DirectKinesisSourceTypeDef(
     _RequiredDirectKinesisSourceTypeDef, _OptionalDirectKinesisSourceTypeDef
 ):
     pass
 
-
 _RequiredGovernedCatalogTargetTypeDef = TypedDict(
     "_RequiredGovernedCatalogTargetTypeDef",
     {
         "Name": str,
         "Inputs": List[str],
         "Table": str,
         "Database": str,
@@ -5789,21 +5682,19 @@
     {
         "PartitionKeys": List[List[str]],
         "SchemaChangePolicy": CatalogSchemaChangePolicyTypeDef,
     },
     total=False,
 )
 
-
 class GovernedCatalogTargetTypeDef(
     _RequiredGovernedCatalogTargetTypeDef, _OptionalGovernedCatalogTargetTypeDef
 ):
     pass
 
-
 _RequiredS3CatalogTargetTypeDef = TypedDict(
     "_RequiredS3CatalogTargetTypeDef",
     {
         "Name": str,
         "Inputs": List[str],
         "Table": str,
         "Database": str,
@@ -5814,19 +5705,17 @@
     {
         "PartitionKeys": List[List[str]],
         "SchemaChangePolicy": CatalogSchemaChangePolicyTypeDef,
     },
     total=False,
 )
 
-
 class S3CatalogTargetTypeDef(_RequiredS3CatalogTargetTypeDef, _OptionalS3CatalogTargetTypeDef):
     pass
 
-
 _RequiredS3DeltaCatalogTargetTypeDef = TypedDict(
     "_RequiredS3DeltaCatalogTargetTypeDef",
     {
         "Name": str,
         "Inputs": List[str],
         "Table": str,
         "Database": str,
@@ -5838,21 +5727,19 @@
         "PartitionKeys": List[List[str]],
         "AdditionalOptions": Dict[str, str],
         "SchemaChangePolicy": CatalogSchemaChangePolicyTypeDef,
     },
     total=False,
 )
 
-
 class S3DeltaCatalogTargetTypeDef(
     _RequiredS3DeltaCatalogTargetTypeDef, _OptionalS3DeltaCatalogTargetTypeDef
 ):
     pass
 
-
 _RequiredS3HudiCatalogTargetTypeDef = TypedDict(
     "_RequiredS3HudiCatalogTargetTypeDef",
     {
         "Name": str,
         "Inputs": List[str],
         "Table": str,
         "Database": str,
@@ -5864,21 +5751,19 @@
     {
         "PartitionKeys": List[List[str]],
         "SchemaChangePolicy": CatalogSchemaChangePolicyTypeDef,
     },
     total=False,
 )
 
-
 class S3HudiCatalogTargetTypeDef(
     _RequiredS3HudiCatalogTargetTypeDef, _OptionalS3HudiCatalogTargetTypeDef
 ):
     pass
 
-
 ClassifierTypeDef = TypedDict(
     "ClassifierTypeDef",
     {
         "GrokClassifier": GrokClassifierTypeDef,
         "XMLClassifier": XMLClassifierTypeDef,
         "JsonClassifier": JsonClassifierTypeDef,
         "CsvClassifier": CsvClassifierTypeDef,
@@ -5898,19 +5783,17 @@
     "_OptionalCodeGenNodeTypeDef",
     {
         "LineNumber": int,
     },
     total=False,
 )
 
-
 class CodeGenNodeTypeDef(_RequiredCodeGenNodeTypeDef, _OptionalCodeGenNodeTypeDef):
     pass
 
-
 LocationTypeDef = TypedDict(
     "LocationTypeDef",
     {
         "Jdbc": Sequence[CodeGenNodeArgTypeDef],
         "S3": Sequence[CodeGenNodeArgTypeDef],
         "DynamoDB": Sequence[CodeGenNodeArgTypeDef],
     },
@@ -5953,19 +5836,17 @@
         "Description": str,
         "MatchCriteria": Sequence[str],
         "PhysicalConnectionRequirements": PhysicalConnectionRequirementsTypeDef,
     },
     total=False,
 )
 
-
 class ConnectionInputTypeDef(_RequiredConnectionInputTypeDef, _OptionalConnectionInputTypeDef):
     pass
 
-
 ConnectionTypeDef = TypedDict(
     "ConnectionTypeDef",
     {
         "Name": str,
         "Description": str,
         "ConnectionType": ConnectionTypeType,
         "MatchCriteria": List[str],
@@ -6009,14 +5890,16 @@
     {
         "S3Targets": List[S3TargetTypeDef],
         "JdbcTargets": List[JdbcTargetTypeDef],
         "MongoDBTargets": List[MongoDBTargetTypeDef],
         "DynamoDBTargets": List[DynamoDBTargetTypeDef],
         "CatalogTargets": List[CatalogTargetTypeDef],
         "DeltaTargets": List[DeltaTargetTypeDef],
+        "IcebergTargets": List[IcebergTargetTypeDef],
+        "HudiTargets": List[HudiTargetTypeDef],
     },
     total=False,
 )
 
 _RequiredListCrawlsRequestRequestTypeDef = TypedDict(
     "_RequiredListCrawlsRequestRequestTypeDef",
     {
@@ -6029,21 +5912,19 @@
         "MaxResults": int,
         "Filters": Sequence[CrawlsFilterTypeDef],
         "NextToken": str,
     },
     total=False,
 )
 
-
 class ListCrawlsRequestRequestTypeDef(
     _RequiredListCrawlsRequestRequestTypeDef, _OptionalListCrawlsRequestRequestTypeDef
 ):
     pass
 
-
 CreateClassifierRequestRequestTypeDef = TypedDict(
     "CreateClassifierRequestRequestTypeDef",
     {
         "GrokClassifier": CreateGrokClassifierRequestTypeDef,
         "XMLClassifier": CreateXMLClassifierRequestTypeDef,
         "JsonClassifier": CreateJsonClassifierRequestTypeDef,
         "CsvClassifier": CreateCsvClassifierRequestTypeDef,
@@ -6065,22 +5946,20 @@
         "Tags": Mapping[str, str],
         "TargetTable": DataQualityTargetTableTypeDef,
         "ClientToken": str,
     },
     total=False,
 )
 
-
 class CreateDataQualityRulesetRequestRequestTypeDef(
     _RequiredCreateDataQualityRulesetRequestRequestTypeDef,
     _OptionalCreateDataQualityRulesetRequestRequestTypeDef,
 ):
     pass
 
-
 DataQualityRulesetListDetailsTypeDef = TypedDict(
     "DataQualityRulesetListDetailsTypeDef",
     {
         "Name": str,
         "Description": str,
         "CreatedOn": datetime,
         "LastModifiedOn": datetime,
@@ -6124,22 +6003,20 @@
     "_OptionalCreatePartitionIndexRequestRequestTypeDef",
     {
         "CatalogId": str,
     },
     total=False,
 )
 
-
 class CreatePartitionIndexRequestRequestTypeDef(
     _RequiredCreatePartitionIndexRequestRequestTypeDef,
     _OptionalCreatePartitionIndexRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredCreateSchemaInputRequestTypeDef = TypedDict(
     "_RequiredCreateSchemaInputRequestTypeDef",
     {
         "SchemaName": str,
         "DataFormat": DataFormatType,
     },
 )
@@ -6151,21 +6028,19 @@
         "Description": str,
         "Tags": Mapping[str, str],
         "SchemaDefinition": str,
     },
     total=False,
 )
 
-
 class CreateSchemaInputRequestTypeDef(
     _RequiredCreateSchemaInputRequestTypeDef, _OptionalCreateSchemaInputRequestTypeDef
 ):
     pass
 
-
 DeleteRegistryInputRequestTypeDef = TypedDict(
     "DeleteRegistryInputRequestTypeDef",
     {
         "RegistryId": RegistryIdTypeDef,
     },
 )
 
@@ -6217,21 +6092,19 @@
         "GlueVersion": str,
         "Tags": Mapping[str, str],
         "RequestOrigin": str,
     },
     total=False,
 )
 
-
 class CreateSessionRequestRequestTypeDef(
     _RequiredCreateSessionRequestRequestTypeDef, _OptionalCreateSessionRequestRequestTypeDef
 ):
     pass
 
-
 SessionTypeDef = TypedDict(
     "SessionTypeDef",
     {
         "Id": str,
         "CreatedOn": datetime,
         "Status": SessionStatusType,
         "ErrorMessage": str,
@@ -6263,21 +6136,19 @@
         "PublishingOptions": DQResultsPublishingOptionsTypeDef,
         "AdditionalOptions": Dict[Literal["performanceTuning.caching"], str],
         "StopJobOnFailureOptions": DQStopJobOnFailureOptionsTypeDef,
     },
     total=False,
 )
 
-
 class EvaluateDataQualityMultiFrameTypeDef(
     _RequiredEvaluateDataQualityMultiFrameTypeDef, _OptionalEvaluateDataQualityMultiFrameTypeDef
 ):
     pass
 
-
 _RequiredEvaluateDataQualityTypeDef = TypedDict(
     "_RequiredEvaluateDataQualityTypeDef",
     {
         "Name": str,
         "Inputs": List[str],
         "Ruleset": str,
     },
@@ -6288,21 +6159,19 @@
         "Output": DQTransformOutputType,
         "PublishingOptions": DQResultsPublishingOptionsTypeDef,
         "StopJobOnFailureOptions": DQStopJobOnFailureOptionsTypeDef,
     },
     total=False,
 )
 
-
 class EvaluateDataQualityTypeDef(
     _RequiredEvaluateDataQualityTypeDef, _OptionalEvaluateDataQualityTypeDef
 ):
     pass
 
-
 DataCatalogEncryptionSettingsTypeDef = TypedDict(
     "DataCatalogEncryptionSettingsTypeDef",
     {
         "EncryptionAtRest": EncryptionAtRestTypeDef,
         "ConnectionPasswordEncryption": ConnectionPasswordEncryptionTypeDef,
     },
     total=False,
@@ -6344,21 +6213,19 @@
         "CatalogId": str,
         "TransactionId": str,
         "QueryAsOfTime": TimestampTypeDef,
     },
     total=False,
 )
 
-
 class GetTableRequestRequestTypeDef(
     _RequiredGetTableRequestRequestTypeDef, _OptionalGetTableRequestRequestTypeDef
 ):
     pass
 
-
 _RequiredGetTablesRequestRequestTypeDef = TypedDict(
     "_RequiredGetTablesRequestRequestTypeDef",
     {
         "DatabaseName": str,
     },
 )
 _OptionalGetTablesRequestRequestTypeDef = TypedDict(
@@ -6370,21 +6237,19 @@
         "MaxResults": int,
         "TransactionId": str,
         "QueryAsOfTime": TimestampTypeDef,
     },
     total=False,
 )
 
-
 class GetTablesRequestRequestTypeDef(
     _RequiredGetTablesRequestRequestTypeDef, _OptionalGetTablesRequestRequestTypeDef
 ):
     pass
 
-
 TaskRunFilterCriteriaTypeDef = TypedDict(
     "TaskRunFilterCriteriaTypeDef",
     {
         "TaskRunType": TaskTypeType,
         "Status": TaskStatusTypeType,
         "StartedBefore": TimestampTypeDef,
         "StartedAfter": TimestampTypeDef,
@@ -6412,21 +6277,19 @@
     {
         "MinimumValue": DecimalNumberTypeDef,
         "MaximumValue": DecimalNumberTypeDef,
     },
     total=False,
 )
 
-
 class DecimalColumnStatisticsDataTypeDef(
     _RequiredDecimalColumnStatisticsDataTypeDef, _OptionalDecimalColumnStatisticsDataTypeDef
 ):
     pass
 
-
 DeleteSchemaInputRequestTypeDef = TypedDict(
     "DeleteSchemaInputRequestTypeDef",
     {
         "SchemaId": SchemaIdTypeDef,
     },
 )
 
@@ -6464,21 +6327,19 @@
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
-
 class ListSchemaVersionsInputRequestTypeDef(
     _RequiredListSchemaVersionsInputRequestTypeDef, _OptionalListSchemaVersionsInputRequestTypeDef
 ):
     pass
 
-
 RegisterSchemaVersionInputRequestTypeDef = TypedDict(
     "RegisterSchemaVersionInputRequestTypeDef",
     {
         "SchemaId": SchemaIdTypeDef,
         "SchemaDefinition": str,
     },
 )
@@ -6509,21 +6370,19 @@
         "UpdateEtlLibraries": bool,
         "DeleteArguments": Sequence[str],
         "AddArguments": Mapping[str, str],
     },
     total=False,
 )
 
-
 class UpdateDevEndpointRequestRequestTypeDef(
     _RequiredUpdateDevEndpointRequestRequestTypeDef, _OptionalUpdateDevEndpointRequestRequestTypeDef
 ):
     pass
 
-
 _RequiredS3DeltaDirectTargetTypeDef = TypedDict(
     "_RequiredS3DeltaDirectTargetTypeDef",
     {
         "Name": str,
         "Inputs": List[str],
         "Path": str,
         "Compression": DeltaTargetCompressionTypeType,
@@ -6536,21 +6395,19 @@
         "PartitionKeys": List[List[str]],
         "AdditionalOptions": Dict[str, str],
         "SchemaChangePolicy": DirectSchemaChangePolicyTypeDef,
     },
     total=False,
 )
 
-
 class S3DeltaDirectTargetTypeDef(
     _RequiredS3DeltaDirectTargetTypeDef, _OptionalS3DeltaDirectTargetTypeDef
 ):
     pass
 
-
 _RequiredS3DirectTargetTypeDef = TypedDict(
     "_RequiredS3DirectTargetTypeDef",
     {
         "Name": str,
         "Inputs": List[str],
         "Path": str,
         "Format": TargetFormatType,
@@ -6562,19 +6419,17 @@
         "PartitionKeys": List[List[str]],
         "Compression": str,
         "SchemaChangePolicy": DirectSchemaChangePolicyTypeDef,
     },
     total=False,
 )
 
-
 class S3DirectTargetTypeDef(_RequiredS3DirectTargetTypeDef, _OptionalS3DirectTargetTypeDef):
     pass
 
-
 _RequiredS3GlueParquetTargetTypeDef = TypedDict(
     "_RequiredS3GlueParquetTargetTypeDef",
     {
         "Name": str,
         "Inputs": List[str],
         "Path": str,
     },
@@ -6585,21 +6440,19 @@
         "PartitionKeys": List[List[str]],
         "Compression": ParquetCompressionTypeType,
         "SchemaChangePolicy": DirectSchemaChangePolicyTypeDef,
     },
     total=False,
 )
 
-
 class S3GlueParquetTargetTypeDef(
     _RequiredS3GlueParquetTargetTypeDef, _OptionalS3GlueParquetTargetTypeDef
 ):
     pass
 
-
 _RequiredS3HudiDirectTargetTypeDef = TypedDict(
     "_RequiredS3HudiDirectTargetTypeDef",
     {
         "Name": str,
         "Inputs": List[str],
         "Path": str,
         "Compression": HudiTargetCompressionTypeType,
@@ -6612,21 +6465,19 @@
     {
         "PartitionKeys": List[List[str]],
         "SchemaChangePolicy": DirectSchemaChangePolicyTypeDef,
     },
     total=False,
 )
 
-
 class S3HudiDirectTargetTypeDef(
     _RequiredS3HudiDirectTargetTypeDef, _OptionalS3HudiDirectTargetTypeDef
 ):
     pass
 
-
 EncryptionConfigurationTypeDef = TypedDict(
     "EncryptionConfigurationTypeDef",
     {
         "S3Encryption": Sequence[S3EncryptionTypeDef],
         "CloudWatchEncryption": CloudWatchEncryptionTypeDef,
         "JobBookmarksEncryption": JobBookmarksEncryptionTypeDef,
     },
@@ -6653,40 +6504,36 @@
     "_OptionalFilterExpressionTypeDef",
     {
         "Negated": bool,
     },
     total=False,
 )
 
-
 class FilterExpressionTypeDef(_RequiredFilterExpressionTypeDef, _OptionalFilterExpressionTypeDef):
     pass
 
-
 _RequiredTransformParametersTypeDef = TypedDict(
     "_RequiredTransformParametersTypeDef",
     {
         "TransformType": Literal["FIND_MATCHES"],
     },
 )
 _OptionalTransformParametersTypeDef = TypedDict(
     "_OptionalTransformParametersTypeDef",
     {
         "FindMatchesParameters": FindMatchesParametersTypeDef,
     },
     total=False,
 )
 
-
 class TransformParametersTypeDef(
     _RequiredTransformParametersTypeDef, _OptionalTransformParametersTypeDef
 ):
     pass
 
-
 GetClassifiersRequestGetClassifiersPaginateTypeDef = TypedDict(
     "GetClassifiersRequestGetClassifiersPaginateTypeDef",
     {
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
@@ -6736,22 +6583,20 @@
     "_OptionalGetJobRunsRequestGetJobRunsPaginateTypeDef",
     {
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-
 class GetJobRunsRequestGetJobRunsPaginateTypeDef(
     _RequiredGetJobRunsRequestGetJobRunsPaginateTypeDef,
     _OptionalGetJobRunsRequestGetJobRunsPaginateTypeDef,
 ):
     pass
 
-
 GetJobsRequestGetJobsPaginateTypeDef = TypedDict(
     "GetJobsRequestGetJobsPaginateTypeDef",
     {
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
@@ -6768,22 +6613,20 @@
     {
         "CatalogId": str,
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-
 class GetPartitionIndexesRequestGetPartitionIndexesPaginateTypeDef(
     _RequiredGetPartitionIndexesRequestGetPartitionIndexesPaginateTypeDef,
     _OptionalGetPartitionIndexesRequestGetPartitionIndexesPaginateTypeDef,
 ):
     pass
 
-
 GetResourcePoliciesRequestGetResourcePoliciesPaginateTypeDef = TypedDict(
     "GetResourcePoliciesRequestGetResourcePoliciesPaginateTypeDef",
     {
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
@@ -6808,22 +6651,20 @@
     {
         "CatalogId": str,
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-
 class GetTableVersionsRequestGetTableVersionsPaginateTypeDef(
     _RequiredGetTableVersionsRequestGetTableVersionsPaginateTypeDef,
     _OptionalGetTableVersionsRequestGetTableVersionsPaginateTypeDef,
 ):
     pass
 
-
 _RequiredGetTablesRequestGetTablesPaginateTypeDef = TypedDict(
     "_RequiredGetTablesRequestGetTablesPaginateTypeDef",
     {
         "DatabaseName": str,
     },
 )
 _OptionalGetTablesRequestGetTablesPaginateTypeDef = TypedDict(
@@ -6834,22 +6675,20 @@
         "TransactionId": str,
         "QueryAsOfTime": TimestampTypeDef,
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-
 class GetTablesRequestGetTablesPaginateTypeDef(
     _RequiredGetTablesRequestGetTablesPaginateTypeDef,
     _OptionalGetTablesRequestGetTablesPaginateTypeDef,
 ):
     pass
 
-
 GetTriggersRequestGetTriggersPaginateTypeDef = TypedDict(
     "GetTriggersRequestGetTriggersPaginateTypeDef",
     {
         "DependentJobName": str,
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
@@ -6867,22 +6706,20 @@
         "CatalogId": str,
         "DatabaseName": str,
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-
 class GetUserDefinedFunctionsRequestGetUserDefinedFunctionsPaginateTypeDef(
     _RequiredGetUserDefinedFunctionsRequestGetUserDefinedFunctionsPaginateTypeDef,
     _OptionalGetUserDefinedFunctionsRequestGetUserDefinedFunctionsPaginateTypeDef,
 ):
     pass
 
-
 ListRegistriesInputListRegistriesPaginateTypeDef = TypedDict(
     "ListRegistriesInputListRegistriesPaginateTypeDef",
     {
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
@@ -6897,22 +6734,20 @@
     "_OptionalListSchemaVersionsInputListSchemaVersionsPaginateTypeDef",
     {
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-
 class ListSchemaVersionsInputListSchemaVersionsPaginateTypeDef(
     _RequiredListSchemaVersionsInputListSchemaVersionsPaginateTypeDef,
     _OptionalListSchemaVersionsInputListSchemaVersionsPaginateTypeDef,
 ):
     pass
 
-
 ListSchemasInputListSchemasPaginateTypeDef = TypedDict(
     "ListSchemasInputListSchemasPaginateTypeDef",
     {
         "RegistryId": RegistryIdTypeDef,
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
@@ -6998,22 +6833,20 @@
         "TransactionId": str,
         "QueryAsOfTime": TimestampTypeDef,
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-
 class GetPartitionsRequestGetPartitionsPaginateTypeDef(
     _RequiredGetPartitionsRequestGetPartitionsPaginateTypeDef,
     _OptionalGetPartitionsRequestGetPartitionsPaginateTypeDef,
 ):
     pass
 
-
 _RequiredGetPartitionsRequestRequestTypeDef = TypedDict(
     "_RequiredGetPartitionsRequestRequestTypeDef",
     {
         "DatabaseName": str,
         "TableName": str,
     },
 )
@@ -7028,21 +6861,19 @@
         "ExcludeColumnSchema": bool,
         "TransactionId": str,
         "QueryAsOfTime": TimestampTypeDef,
     },
     total=False,
 )
 
-
 class GetPartitionsRequestRequestTypeDef(
     _RequiredGetPartitionsRequestRequestTypeDef, _OptionalGetPartitionsRequestRequestTypeDef
 ):
     pass
 
-
 _RequiredGetUnfilteredPartitionsMetadataRequestRequestTypeDef = TypedDict(
     "_RequiredGetUnfilteredPartitionsMetadataRequestRequestTypeDef",
     {
         "CatalogId": str,
         "DatabaseName": str,
         "TableName": str,
         "SupportedPermissionTypes": Sequence[PermissionTypeType],
@@ -7056,22 +6887,20 @@
         "NextToken": str,
         "Segment": SegmentTypeDef,
         "MaxResults": int,
     },
     total=False,
 )
 
-
 class GetUnfilteredPartitionsMetadataRequestRequestTypeDef(
     _RequiredGetUnfilteredPartitionsMetadataRequestRequestTypeDef,
     _OptionalGetUnfilteredPartitionsMetadataRequestRequestTypeDef,
 ):
     pass
 
-
 GetResourcePoliciesResponseTypeDef = TypedDict(
     "GetResourcePoliciesResponseTypeDef",
     {
         "GetResourcePoliciesResponseList": List[GluePolicyTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -7109,21 +6938,19 @@
         "SchemaVersionNumber": SchemaVersionNumberTypeDef,
         "Compatibility": CompatibilityType,
         "Description": str,
     },
     total=False,
 )
 
-
 class UpdateSchemaInputRequestTypeDef(
     _RequiredUpdateSchemaInputRequestTypeDef, _OptionalUpdateSchemaInputRequestTypeDef
 ):
     pass
 
-
 GlueSchemaTypeDef = TypedDict(
     "GlueSchemaTypeDef",
     {
         "Columns": List[GlueStudioSchemaColumnTypeDef],
     },
     total=False,
 )
@@ -7141,21 +6968,19 @@
     {
         "PartitionPredicate": str,
         "AdditionalOptions": S3SourceAdditionalOptionsTypeDef,
     },
     total=False,
 )
 
-
 class GovernedCatalogSourceTypeDef(
     _RequiredGovernedCatalogSourceTypeDef, _OptionalGovernedCatalogSourceTypeDef
 ):
     pass
 
-
 _RequiredS3CatalogSourceTypeDef = TypedDict(
     "_RequiredS3CatalogSourceTypeDef",
     {
         "Name": str,
         "Database": str,
         "Table": str,
     },
@@ -7165,18 +6990,24 @@
     {
         "PartitionPredicate": str,
         "AdditionalOptions": S3SourceAdditionalOptionsTypeDef,
     },
     total=False,
 )
 
-
 class S3CatalogSourceTypeDef(_RequiredS3CatalogSourceTypeDef, _OptionalS3CatalogSourceTypeDef):
     pass
 
+OpenTableFormatInputTypeDef = TypedDict(
+    "OpenTableFormatInputTypeDef",
+    {
+        "IcebergInput": IcebergInputTypeDef,
+    },
+    total=False,
+)
 
 JobRunTypeDef = TypedDict(
     "JobRunTypeDef",
     {
         "Id": str,
         "Attempt": int,
         "PreviousRunId": str,
@@ -7285,22 +7116,20 @@
         "SchemaId": SchemaIdTypeDef,
         "SchemaVersionNumber": SchemaVersionNumberTypeDef,
         "SchemaVersionId": str,
     },
     total=False,
 )
 
-
 class PutSchemaVersionMetadataInputRequestTypeDef(
     _RequiredPutSchemaVersionMetadataInputRequestTypeDef,
     _OptionalPutSchemaVersionMetadataInputRequestTypeDef,
 ):
     pass
 
-
 QuerySchemaVersionMetadataInputRequestTypeDef = TypedDict(
     "QuerySchemaVersionMetadataInputRequestTypeDef",
     {
         "SchemaId": SchemaIdTypeDef,
         "SchemaVersionNumber": SchemaVersionNumberTypeDef,
         "SchemaVersionId": str,
         "MetadataList": Sequence[MetadataKeyValuePairTypeDef],
@@ -7322,21 +7151,28 @@
         "SchemaId": SchemaIdTypeDef,
         "SchemaVersionNumber": SchemaVersionNumberTypeDef,
         "SchemaVersionId": str,
     },
     total=False,
 )
 
-
 class RemoveSchemaVersionMetadataInputRequestTypeDef(
     _RequiredRemoveSchemaVersionMetadataInputRequestTypeDef,
     _OptionalRemoveSchemaVersionMetadataInputRequestTypeDef,
 ):
     pass
 
+RecipeTypeDef = TypedDict(
+    "RecipeTypeDef",
+    {
+        "Name": str,
+        "Inputs": List[str],
+        "RecipeReference": RecipeReferenceTypeDef,
+    },
+)
 
 _RequiredRedshiftTargetTypeDef = TypedDict(
     "_RequiredRedshiftTargetTypeDef",
     {
         "Name": str,
         "Inputs": List[str],
         "Database": str,
@@ -7349,19 +7185,17 @@
         "RedshiftTmpDir": str,
         "TmpDirIAMRole": str,
         "UpsertRedshiftOptions": UpsertRedshiftTargetOptionsTypeDef,
     },
     total=False,
 )
 
-
 class RedshiftTargetTypeDef(_RequiredRedshiftTargetTypeDef, _OptionalRedshiftTargetTypeDef):
     pass
 
-
 UserDefinedFunctionInputTypeDef = TypedDict(
     "UserDefinedFunctionInputTypeDef",
     {
         "FunctionName": str,
         "ClassName": str,
         "OwnerName": str,
         "OwnerType": PrincipalTypeType,
@@ -7438,14 +7272,32 @@
         "Name": str,
         "Data": AmazonRedshiftNodeDataTypeDef,
         "Inputs": List[str],
     },
     total=False,
 )
 
+_RequiredSnowflakeTargetTypeDef = TypedDict(
+    "_RequiredSnowflakeTargetTypeDef",
+    {
+        "Name": str,
+        "Data": SnowflakeNodeDataTypeDef,
+    },
+)
+_OptionalSnowflakeTargetTypeDef = TypedDict(
+    "_OptionalSnowflakeTargetTypeDef",
+    {
+        "Inputs": List[str],
+    },
+    total=False,
+)
+
+class SnowflakeTargetTypeDef(_RequiredSnowflakeTargetTypeDef, _OptionalSnowflakeTargetTypeDef):
+    pass
+
 _RequiredPartitionIndexDescriptorTypeDef = TypedDict(
     "_RequiredPartitionIndexDescriptorTypeDef",
     {
         "IndexName": str,
         "Keys": List[KeySchemaElementTypeDef],
         "IndexStatus": PartitionIndexStatusType,
     },
@@ -7454,21 +7306,19 @@
     "_OptionalPartitionIndexDescriptorTypeDef",
     {
         "BackfillErrors": List[BackfillErrorTypeDef],
     },
     total=False,
 )
 
-
 class PartitionIndexDescriptorTypeDef(
     _RequiredPartitionIndexDescriptorTypeDef, _OptionalPartitionIndexDescriptorTypeDef
 ):
     pass
 
-
 BatchStopJobRunResponseTypeDef = TypedDict(
     "BatchStopJobRunResponseTypeDef",
     {
         "SuccessfulSubmissions": List[BatchStopJobRunSuccessfulSubmissionTypeDef],
         "Errors": List[BatchStopJobRunErrorTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -7578,21 +7428,19 @@
     {
         "Sinks": Sequence[CatalogEntryTypeDef],
         "Location": LocationTypeDef,
     },
     total=False,
 )
 
-
 class GetMappingRequestRequestTypeDef(
     _RequiredGetMappingRequestRequestTypeDef, _OptionalGetMappingRequestRequestTypeDef
 ):
     pass
 
-
 _RequiredGetPlanRequestRequestTypeDef = TypedDict(
     "_RequiredGetPlanRequestRequestTypeDef",
     {
         "Mapping": Sequence[MappingEntryTypeDef],
         "Source": CatalogEntryTypeDef,
     },
 )
@@ -7603,21 +7451,19 @@
         "Location": LocationTypeDef,
         "Language": LanguageType,
         "AdditionalPlanOptionsMap": Mapping[str, str],
     },
     total=False,
 )
 
-
 class GetPlanRequestRequestTypeDef(
     _RequiredGetPlanRequestRequestTypeDef, _OptionalGetPlanRequestRequestTypeDef
 ):
     pass
 
-
 _RequiredCreateTriggerRequestRequestTypeDef = TypedDict(
     "_RequiredCreateTriggerRequestRequestTypeDef",
     {
         "Name": str,
         "Type": TriggerTypeType,
         "Actions": Sequence[ActionTypeDef],
     },
@@ -7632,21 +7478,19 @@
         "StartOnCreation": bool,
         "Tags": Mapping[str, str],
         "EventBatchingCondition": EventBatchingConditionTypeDef,
     },
     total=False,
 )
 
-
 class CreateTriggerRequestRequestTypeDef(
     _RequiredCreateTriggerRequestRequestTypeDef, _OptionalCreateTriggerRequestRequestTypeDef
 ):
     pass
 
-
 TriggerTypeDef = TypedDict(
     "TriggerTypeDef",
     {
         "Name": str,
         "WorkflowName": str,
         "Id": str,
         "Type": TriggerTypeType,
@@ -7683,21 +7527,19 @@
     "_OptionalEvaluationMetricsTypeDef",
     {
         "FindMatchesMetrics": FindMatchesMetricsTypeDef,
     },
     total=False,
 )
 
-
 class EvaluationMetricsTypeDef(
     _RequiredEvaluationMetricsTypeDef, _OptionalEvaluationMetricsTypeDef
 ):
     pass
 
-
 _RequiredCreateConnectionRequestRequestTypeDef = TypedDict(
     "_RequiredCreateConnectionRequestRequestTypeDef",
     {
         "ConnectionInput": ConnectionInputTypeDef,
     },
 )
 _OptionalCreateConnectionRequestRequestTypeDef = TypedDict(
@@ -7705,21 +7547,19 @@
     {
         "CatalogId": str,
         "Tags": Mapping[str, str],
     },
     total=False,
 )
 
-
 class CreateConnectionRequestRequestTypeDef(
     _RequiredCreateConnectionRequestRequestTypeDef, _OptionalCreateConnectionRequestRequestTypeDef
 ):
     pass
 
-
 _RequiredUpdateConnectionRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateConnectionRequestRequestTypeDef",
     {
         "Name": str,
         "ConnectionInput": ConnectionInputTypeDef,
     },
 )
@@ -7727,21 +7567,19 @@
     "_OptionalUpdateConnectionRequestRequestTypeDef",
     {
         "CatalogId": str,
     },
     total=False,
 )
 
-
 class UpdateConnectionRequestRequestTypeDef(
     _RequiredUpdateConnectionRequestRequestTypeDef, _OptionalUpdateConnectionRequestRequestTypeDef
 ):
     pass
 
-
 GetConnectionResponseTypeDef = TypedDict(
     "GetConnectionResponseTypeDef",
     {
         "Connection": ConnectionTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -7805,21 +7643,19 @@
         "Configuration": str,
         "CrawlerSecurityConfiguration": str,
         "Tags": Mapping[str, str],
     },
     total=False,
 )
 
-
 class CreateCrawlerRequestRequestTypeDef(
     _RequiredCreateCrawlerRequestRequestTypeDef, _OptionalCreateCrawlerRequestRequestTypeDef
 ):
     pass
 
-
 _RequiredUpdateCrawlerRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateCrawlerRequestRequestTypeDef",
     {
         "Name": str,
     },
 )
 _OptionalUpdateCrawlerRequestRequestTypeDef = TypedDict(
@@ -7838,21 +7674,19 @@
         "LakeFormationConfiguration": LakeFormationConfigurationTypeDef,
         "Configuration": str,
         "CrawlerSecurityConfiguration": str,
     },
     total=False,
 )
 
-
 class UpdateCrawlerRequestRequestTypeDef(
     _RequiredUpdateCrawlerRequestRequestTypeDef, _OptionalUpdateCrawlerRequestRequestTypeDef
 ):
     pass
 
-
 ListDataQualityRulesetsResponseTypeDef = TypedDict(
     "ListDataQualityRulesetsResponseTypeDef",
     {
         "Rulesets": List[DataQualityRulesetListDetailsTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -7922,22 +7756,20 @@
     {
         "StartedBefore": TimestampTypeDef,
         "StartedAfter": TimestampTypeDef,
     },
     total=False,
 )
 
-
 class DataQualityRuleRecommendationRunFilterTypeDef(
     _RequiredDataQualityRuleRecommendationRunFilterTypeDef,
     _OptionalDataQualityRuleRecommendationRunFilterTypeDef,
 ):
     pass
 
-
 DataQualityRulesetEvaluationRunDescriptionTypeDef = TypedDict(
     "DataQualityRulesetEvaluationRunDescriptionTypeDef",
     {
         "RunId": str,
         "Status": TaskStatusTypeType,
         "StartedOn": datetime,
         "DataSource": DataSourceTypeDef,
@@ -7956,22 +7788,20 @@
     {
         "StartedBefore": TimestampTypeDef,
         "StartedAfter": TimestampTypeDef,
     },
     total=False,
 )
 
-
 class DataQualityRulesetEvaluationRunFilterTypeDef(
     _RequiredDataQualityRulesetEvaluationRunFilterTypeDef,
     _OptionalDataQualityRulesetEvaluationRunFilterTypeDef,
 ):
     pass
 
-
 GetDataQualityResultResponseTypeDef = TypedDict(
     "GetDataQualityResultResponseTypeDef",
     {
         "ResultId": str,
         "Score": float,
         "DataSource": DataSourceTypeDef,
         "RulesetName": str,
@@ -8042,22 +7872,20 @@
         "Timeout": int,
         "CreatedRulesetName": str,
         "ClientToken": str,
     },
     total=False,
 )
 
-
 class StartDataQualityRuleRecommendationRunRequestRequestTypeDef(
     _RequiredStartDataQualityRuleRecommendationRunRequestRequestTypeDef,
     _OptionalStartDataQualityRuleRecommendationRunRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredStartDataQualityRulesetEvaluationRunRequestRequestTypeDef = TypedDict(
     "_RequiredStartDataQualityRulesetEvaluationRunRequestRequestTypeDef",
     {
         "DataSource": DataSourceTypeDef,
         "Role": str,
         "RulesetNames": Sequence[str],
     },
@@ -8070,22 +7898,20 @@
         "ClientToken": str,
         "AdditionalRunOptions": DataQualityEvaluationRunAdditionalRunOptionsTypeDef,
         "AdditionalDataSources": Mapping[str, DataSourceTypeDef],
     },
     total=False,
 )
 
-
 class StartDataQualityRulesetEvaluationRunRequestRequestTypeDef(
     _RequiredStartDataQualityRulesetEvaluationRunRequestRequestTypeDef,
     _OptionalStartDataQualityRulesetEvaluationRunRequestRequestTypeDef,
 ):
     pass
 
-
 CreateSessionResponseTypeDef = TypedDict(
     "CreateSessionResponseTypeDef",
     {
         "Session": SessionTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -8126,22 +7952,20 @@
     "_OptionalPutDataCatalogEncryptionSettingsRequestRequestTypeDef",
     {
         "CatalogId": str,
     },
     total=False,
 )
 
-
 class PutDataCatalogEncryptionSettingsRequestRequestTypeDef(
     _RequiredPutDataCatalogEncryptionSettingsRequestRequestTypeDef,
     _OptionalPutDataCatalogEncryptionSettingsRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredDatabaseInputTypeDef = TypedDict(
     "_RequiredDatabaseInputTypeDef",
     {
         "Name": str,
     },
 )
 _OptionalDatabaseInputTypeDef = TypedDict(
@@ -8153,19 +7977,17 @@
         "CreateTableDefaultPermissions": Sequence[PrincipalPermissionsTypeDef],
         "TargetDatabase": DatabaseIdentifierTypeDef,
         "FederatedDatabase": FederatedDatabaseTypeDef,
     },
     total=False,
 )
 
-
 class DatabaseInputTypeDef(_RequiredDatabaseInputTypeDef, _OptionalDatabaseInputTypeDef):
     pass
 
-
 _RequiredDatabaseTypeDef = TypedDict(
     "_RequiredDatabaseTypeDef",
     {
         "Name": str,
     },
 )
 _OptionalDatabaseTypeDef = TypedDict(
@@ -8179,19 +8001,17 @@
         "TargetDatabase": DatabaseIdentifierTypeDef,
         "CatalogId": str,
         "FederatedDatabase": FederatedDatabaseTypeDef,
     },
     total=False,
 )
 
-
 class DatabaseTypeDef(_RequiredDatabaseTypeDef, _OptionalDatabaseTypeDef):
     pass
 
-
 ListDataQualityRulesetsRequestRequestTypeDef = TypedDict(
     "ListDataQualityRulesetsRequestRequestTypeDef",
     {
         "NextToken": str,
         "MaxResults": int,
         "Filter": DataQualityRulesetFilterCriteriaTypeDef,
         "Tags": Mapping[str, str],
@@ -8212,21 +8032,19 @@
         "MaxResults": int,
         "Filter": TaskRunFilterCriteriaTypeDef,
         "Sort": TaskRunSortCriteriaTypeDef,
     },
     total=False,
 )
 
-
 class GetMLTaskRunsRequestRequestTypeDef(
     _RequiredGetMLTaskRunsRequestRequestTypeDef, _OptionalGetMLTaskRunsRequestRequestTypeDef
 ):
     pass
 
-
 _RequiredDropNullFieldsTypeDef = TypedDict(
     "_RequiredDropNullFieldsTypeDef",
     {
         "Name": str,
         "Inputs": List[str],
     },
 )
@@ -8235,19 +8053,17 @@
     {
         "NullCheckBoxList": NullCheckBoxListTypeDef,
         "NullTextList": List[NullValueFieldTypeDef],
     },
     total=False,
 )
 
-
 class DropNullFieldsTypeDef(_RequiredDropNullFieldsTypeDef, _OptionalDropNullFieldsTypeDef):
     pass
 
-
 _RequiredColumnStatisticsDataTypeDef = TypedDict(
     "_RequiredColumnStatisticsDataTypeDef",
     {
         "Type": ColumnStatisticsTypeType,
     },
 )
 _OptionalColumnStatisticsDataTypeDef = TypedDict(
@@ -8260,21 +8076,19 @@
         "LongColumnStatisticsData": LongColumnStatisticsDataTypeDef,
         "StringColumnStatisticsData": StringColumnStatisticsDataTypeDef,
         "BinaryColumnStatisticsData": BinaryColumnStatisticsDataTypeDef,
     },
     total=False,
 )
 
-
 class ColumnStatisticsDataTypeDef(
     _RequiredColumnStatisticsDataTypeDef, _OptionalColumnStatisticsDataTypeDef
 ):
     pass
 
-
 StorageDescriptorTypeDef = TypedDict(
     "StorageDescriptorTypeDef",
     {
         "Columns": Sequence[ColumnTypeDef],
         "Location": str,
         "AdditionalLocations": Sequence[str],
         "InputFormat": str,
@@ -8347,21 +8161,19 @@
         "NumberOfWorkers": int,
         "Timeout": int,
         "MaxRetries": int,
     },
     total=False,
 )
 
-
 class UpdateMLTransformRequestRequestTypeDef(
     _RequiredUpdateMLTransformRequestRequestTypeDef, _OptionalUpdateMLTransformRequestRequestTypeDef
 ):
     pass
 
-
 GetMLTransformsRequestRequestTypeDef = TypedDict(
     "GetMLTransformsRequestRequestTypeDef",
     {
         "NextToken": str,
         "MaxResults": int,
         "Filter": TransformFilterCriteriaTypeDef,
         "Sort": TransformSortCriteriaTypeDef,
@@ -8396,21 +8208,19 @@
     {
         "ConnectionTable": str,
         "OutputSchemas": List[GlueSchemaTypeDef],
     },
     total=False,
 )
 
-
 class AthenaConnectorSourceTypeDef(
     _RequiredAthenaConnectorSourceTypeDef, _OptionalAthenaConnectorSourceTypeDef
 ):
     pass
 
-
 _RequiredCatalogDeltaSourceTypeDef = TypedDict(
     "_RequiredCatalogDeltaSourceTypeDef",
     {
         "Name": str,
         "Database": str,
         "Table": str,
     },
@@ -8420,21 +8230,19 @@
     {
         "AdditionalDeltaOptions": Dict[str, str],
         "OutputSchemas": List[GlueSchemaTypeDef],
     },
     total=False,
 )
 
-
 class CatalogDeltaSourceTypeDef(
     _RequiredCatalogDeltaSourceTypeDef, _OptionalCatalogDeltaSourceTypeDef
 ):
     pass
 
-
 _RequiredCatalogHudiSourceTypeDef = TypedDict(
     "_RequiredCatalogHudiSourceTypeDef",
     {
         "Name": str,
         "Database": str,
         "Table": str,
     },
@@ -8444,21 +8252,19 @@
     {
         "AdditionalHudiOptions": Dict[str, str],
         "OutputSchemas": List[GlueSchemaTypeDef],
     },
     total=False,
 )
 
-
 class CatalogHudiSourceTypeDef(
     _RequiredCatalogHudiSourceTypeDef, _OptionalCatalogHudiSourceTypeDef
 ):
     pass
 
-
 _RequiredCustomCodeTypeDef = TypedDict(
     "_RequiredCustomCodeTypeDef",
     {
         "Name": str,
         "Inputs": List[str],
         "Code": str,
         "ClassName": str,
@@ -8468,19 +8274,17 @@
     "_OptionalCustomCodeTypeDef",
     {
         "OutputSchemas": List[GlueSchemaTypeDef],
     },
     total=False,
 )
 
-
 class CustomCodeTypeDef(_RequiredCustomCodeTypeDef, _OptionalCustomCodeTypeDef):
     pass
 
-
 _RequiredDynamicTransformTypeDef = TypedDict(
     "_RequiredDynamicTransformTypeDef",
     {
         "Name": str,
         "TransformName": str,
         "Inputs": List[str],
         "FunctionName": str,
@@ -8493,19 +8297,17 @@
         "Parameters": List[TransformConfigParameterTypeDef],
         "Version": str,
         "OutputSchemas": List[GlueSchemaTypeDef],
     },
     total=False,
 )
 
-
 class DynamicTransformTypeDef(_RequiredDynamicTransformTypeDef, _OptionalDynamicTransformTypeDef):
     pass
 
-
 _RequiredJDBCConnectorSourceTypeDef = TypedDict(
     "_RequiredJDBCConnectorSourceTypeDef",
     {
         "Name": str,
         "ConnectionName": str,
         "ConnectorName": str,
         "ConnectionType": str,
@@ -8518,21 +8320,19 @@
         "ConnectionTable": str,
         "Query": str,
         "OutputSchemas": List[GlueSchemaTypeDef],
     },
     total=False,
 )
 
-
 class JDBCConnectorSourceTypeDef(
     _RequiredJDBCConnectorSourceTypeDef, _OptionalJDBCConnectorSourceTypeDef
 ):
     pass
 
-
 _RequiredJDBCConnectorTargetTypeDef = TypedDict(
     "_RequiredJDBCConnectorTargetTypeDef",
     {
         "Name": str,
         "Inputs": List[str],
         "ConnectionName": str,
         "ConnectionTable": str,
@@ -8545,21 +8345,19 @@
     {
         "AdditionalOptions": Dict[str, str],
         "OutputSchemas": List[GlueSchemaTypeDef],
     },
     total=False,
 )
 
-
 class JDBCConnectorTargetTypeDef(
     _RequiredJDBCConnectorTargetTypeDef, _OptionalJDBCConnectorTargetTypeDef
 ):
     pass
 
-
 _RequiredS3CatalogDeltaSourceTypeDef = TypedDict(
     "_RequiredS3CatalogDeltaSourceTypeDef",
     {
         "Name": str,
         "Database": str,
         "Table": str,
     },
@@ -8569,21 +8367,19 @@
     {
         "AdditionalDeltaOptions": Dict[str, str],
         "OutputSchemas": List[GlueSchemaTypeDef],
     },
     total=False,
 )
 
-
 class S3CatalogDeltaSourceTypeDef(
     _RequiredS3CatalogDeltaSourceTypeDef, _OptionalS3CatalogDeltaSourceTypeDef
 ):
     pass
 
-
 _RequiredS3CatalogHudiSourceTypeDef = TypedDict(
     "_RequiredS3CatalogHudiSourceTypeDef",
     {
         "Name": str,
         "Database": str,
         "Table": str,
     },
@@ -8593,21 +8389,19 @@
     {
         "AdditionalHudiOptions": Dict[str, str],
         "OutputSchemas": List[GlueSchemaTypeDef],
     },
     total=False,
 )
 
-
 class S3CatalogHudiSourceTypeDef(
     _RequiredS3CatalogHudiSourceTypeDef, _OptionalS3CatalogHudiSourceTypeDef
 ):
     pass
 
-
 _RequiredS3CsvSourceTypeDef = TypedDict(
     "_RequiredS3CsvSourceTypeDef",
     {
         "Name": str,
         "Paths": List[str],
         "Separator": SeparatorType,
         "QuoteChar": QuoteCharType,
@@ -8631,19 +8425,17 @@
         "SkipFirst": bool,
         "OptimizePerformance": bool,
         "OutputSchemas": List[GlueSchemaTypeDef],
     },
     total=False,
 )
 
-
 class S3CsvSourceTypeDef(_RequiredS3CsvSourceTypeDef, _OptionalS3CsvSourceTypeDef):
     pass
 
-
 _RequiredS3DeltaSourceTypeDef = TypedDict(
     "_RequiredS3DeltaSourceTypeDef",
     {
         "Name": str,
         "Paths": List[str],
     },
 )
@@ -8653,19 +8445,17 @@
         "AdditionalDeltaOptions": Dict[str, str],
         "AdditionalOptions": S3DirectSourceAdditionalOptionsTypeDef,
         "OutputSchemas": List[GlueSchemaTypeDef],
     },
     total=False,
 )
 
-
 class S3DeltaSourceTypeDef(_RequiredS3DeltaSourceTypeDef, _OptionalS3DeltaSourceTypeDef):
     pass
 
-
 _RequiredS3HudiSourceTypeDef = TypedDict(
     "_RequiredS3HudiSourceTypeDef",
     {
         "Name": str,
         "Paths": List[str],
     },
 )
@@ -8675,19 +8465,17 @@
         "AdditionalHudiOptions": Dict[str, str],
         "AdditionalOptions": S3DirectSourceAdditionalOptionsTypeDef,
         "OutputSchemas": List[GlueSchemaTypeDef],
     },
     total=False,
 )
 
-
 class S3HudiSourceTypeDef(_RequiredS3HudiSourceTypeDef, _OptionalS3HudiSourceTypeDef):
     pass
 
-
 _RequiredS3JsonSourceTypeDef = TypedDict(
     "_RequiredS3JsonSourceTypeDef",
     {
         "Name": str,
         "Paths": List[str],
     },
 )
@@ -8705,19 +8493,17 @@
         "JsonPath": str,
         "Multiline": bool,
         "OutputSchemas": List[GlueSchemaTypeDef],
     },
     total=False,
 )
 
-
 class S3JsonSourceTypeDef(_RequiredS3JsonSourceTypeDef, _OptionalS3JsonSourceTypeDef):
     pass
 
-
 _RequiredS3ParquetSourceTypeDef = TypedDict(
     "_RequiredS3ParquetSourceTypeDef",
     {
         "Name": str,
         "Paths": List[str],
     },
 )
@@ -8733,18 +8519,34 @@
         "MaxFilesInBand": int,
         "AdditionalOptions": S3DirectSourceAdditionalOptionsTypeDef,
         "OutputSchemas": List[GlueSchemaTypeDef],
     },
     total=False,
 )
 
-
 class S3ParquetSourceTypeDef(_RequiredS3ParquetSourceTypeDef, _OptionalS3ParquetSourceTypeDef):
     pass
 
+_RequiredSnowflakeSourceTypeDef = TypedDict(
+    "_RequiredSnowflakeSourceTypeDef",
+    {
+        "Name": str,
+        "Data": SnowflakeNodeDataTypeDef,
+    },
+)
+_OptionalSnowflakeSourceTypeDef = TypedDict(
+    "_OptionalSnowflakeSourceTypeDef",
+    {
+        "OutputSchemas": List[GlueSchemaTypeDef],
+    },
+    total=False,
+)
+
+class SnowflakeSourceTypeDef(_RequiredSnowflakeSourceTypeDef, _OptionalSnowflakeSourceTypeDef):
+    pass
 
 _RequiredSparkConnectorSourceTypeDef = TypedDict(
     "_RequiredSparkConnectorSourceTypeDef",
     {
         "Name": str,
         "ConnectionName": str,
         "ConnectorName": str,
@@ -8756,21 +8558,19 @@
     {
         "AdditionalOptions": Dict[str, str],
         "OutputSchemas": List[GlueSchemaTypeDef],
     },
     total=False,
 )
 
-
 class SparkConnectorSourceTypeDef(
     _RequiredSparkConnectorSourceTypeDef, _OptionalSparkConnectorSourceTypeDef
 ):
     pass
 
-
 _RequiredSparkConnectorTargetTypeDef = TypedDict(
     "_RequiredSparkConnectorTargetTypeDef",
     {
         "Name": str,
         "Inputs": List[str],
         "ConnectionName": str,
         "ConnectorName": str,
@@ -8782,21 +8582,19 @@
     {
         "AdditionalOptions": Dict[str, str],
         "OutputSchemas": List[GlueSchemaTypeDef],
     },
     total=False,
 )
 
-
 class SparkConnectorTargetTypeDef(
     _RequiredSparkConnectorTargetTypeDef, _OptionalSparkConnectorTargetTypeDef
 ):
     pass
 
-
 _RequiredSparkSQLTypeDef = TypedDict(
     "_RequiredSparkSQLTypeDef",
     {
         "Name": str,
         "Inputs": List[str],
         "SqlQuery": str,
         "SqlAliases": List[SqlAliasTypeDef],
@@ -8806,19 +8604,17 @@
     "_OptionalSparkSQLTypeDef",
     {
         "OutputSchemas": List[GlueSchemaTypeDef],
     },
     total=False,
 )
 
-
 class SparkSQLTypeDef(_RequiredSparkSQLTypeDef, _OptionalSparkSQLTypeDef):
     pass
 
-
 GetJobRunResponseTypeDef = TypedDict(
     "GetJobRunResponseTypeDef",
     {
         "JobRun": JobRunTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -8895,21 +8691,19 @@
         "MaxRetries": int,
         "Tags": Mapping[str, str],
         "TransformEncryption": TransformEncryptionTypeDef,
     },
     total=False,
 )
 
-
 class CreateMLTransformRequestRequestTypeDef(
     _RequiredCreateMLTransformRequestRequestTypeDef, _OptionalCreateMLTransformRequestRequestTypeDef
 ):
     pass
 
-
 QuerySchemaVersionMetadataResponseTypeDef = TypedDict(
     "QuerySchemaVersionMetadataResponseTypeDef",
     {
         "MetadataInfoMap": Dict[str, MetadataInfoTypeDef],
         "SchemaVersionId": str,
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
@@ -8927,22 +8721,20 @@
     "_OptionalCreateUserDefinedFunctionRequestRequestTypeDef",
     {
         "CatalogId": str,
     },
     total=False,
 )
 
-
 class CreateUserDefinedFunctionRequestRequestTypeDef(
     _RequiredCreateUserDefinedFunctionRequestRequestTypeDef,
     _OptionalCreateUserDefinedFunctionRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredUpdateUserDefinedFunctionRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateUserDefinedFunctionRequestRequestTypeDef",
     {
         "DatabaseName": str,
         "FunctionName": str,
         "FunctionInput": UserDefinedFunctionInputTypeDef,
     },
@@ -8951,22 +8743,20 @@
     "_OptionalUpdateUserDefinedFunctionRequestRequestTypeDef",
     {
         "CatalogId": str,
     },
     total=False,
 )
 
-
 class UpdateUserDefinedFunctionRequestRequestTypeDef(
     _RequiredUpdateUserDefinedFunctionRequestRequestTypeDef,
     _OptionalUpdateUserDefinedFunctionRequestRequestTypeDef,
 ):
     pass
 
-
 GetUserDefinedFunctionResponseTypeDef = TypedDict(
     "GetUserDefinedFunctionResponseTypeDef",
     {
         "UserDefinedFunction": UserDefinedFunctionTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -9208,21 +8998,19 @@
     {
         "CatalogId": str,
         "Tags": Mapping[str, str],
     },
     total=False,
 )
 
-
 class CreateDatabaseRequestRequestTypeDef(
     _RequiredCreateDatabaseRequestRequestTypeDef, _OptionalCreateDatabaseRequestRequestTypeDef
 ):
     pass
 
-
 _RequiredUpdateDatabaseRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateDatabaseRequestRequestTypeDef",
     {
         "Name": str,
         "DatabaseInput": DatabaseInputTypeDef,
     },
 )
@@ -9230,21 +9018,19 @@
     "_OptionalUpdateDatabaseRequestRequestTypeDef",
     {
         "CatalogId": str,
     },
     total=False,
 )
 
-
 class UpdateDatabaseRequestRequestTypeDef(
     _RequiredUpdateDatabaseRequestRequestTypeDef, _OptionalUpdateDatabaseRequestRequestTypeDef
 ):
     pass
 
-
 GetDatabaseResponseTypeDef = TypedDict(
     "GetDatabaseResponseTypeDef",
     {
         "Database": DatabaseTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -9317,19 +9103,17 @@
         "TableType": str,
         "Parameters": Mapping[str, str],
         "TargetTable": TableIdentifierTypeDef,
     },
     total=False,
 )
 
-
 class TableInputTypeDef(_RequiredTableInputTypeDef, _OptionalTableInputTypeDef):
     pass
 
-
 _RequiredTableTypeDef = TypedDict(
     "_RequiredTableTypeDef",
     {
         "Name": str,
     },
 )
 _OptionalTableTypeDef = TypedDict(
@@ -9355,19 +9139,17 @@
         "CatalogId": str,
         "VersionId": str,
         "FederatedTable": FederatedTableTypeDef,
     },
     total=False,
 )
 
-
 class TableTypeDef(_RequiredTableTypeDef, _OptionalTableTypeDef):
     pass
 
-
 GetSecurityConfigurationResponseTypeDef = TypedDict(
     "GetSecurityConfigurationResponseTypeDef",
     {
         "SecurityConfiguration": SecurityConfigurationTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -9446,14 +9228,17 @@
         "CatalogDeltaSource": CatalogDeltaSourceTypeDef,
         "S3DeltaSource": S3DeltaSourceTypeDef,
         "S3DeltaCatalogTarget": S3DeltaCatalogTargetTypeDef,
         "S3DeltaDirectTarget": S3DeltaDirectTargetTypeDef,
         "AmazonRedshiftSource": AmazonRedshiftSourceTypeDef,
         "AmazonRedshiftTarget": AmazonRedshiftTargetTypeDef,
         "EvaluateDataQualityMultiFrame": EvaluateDataQualityMultiFrameTypeDef,
+        "Recipe": RecipeTypeDef,
+        "SnowflakeSource": SnowflakeSourceTypeDef,
+        "SnowflakeTarget": SnowflakeTargetTypeDef,
     },
     total=False,
 )
 
 GetMLTaskRunsResponseTypeDef = TypedDict(
     "GetMLTaskRunsResponseTypeDef",
     {
@@ -9542,22 +9327,20 @@
     "_OptionalUpdateColumnStatisticsForPartitionRequestRequestTypeDef",
     {
         "CatalogId": str,
     },
     total=False,
 )
 
-
 class UpdateColumnStatisticsForPartitionRequestRequestTypeDef(
     _RequiredUpdateColumnStatisticsForPartitionRequestRequestTypeDef,
     _OptionalUpdateColumnStatisticsForPartitionRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredUpdateColumnStatisticsForTableRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateColumnStatisticsForTableRequestRequestTypeDef",
     {
         "DatabaseName": str,
         "TableName": str,
         "ColumnStatisticsList": Sequence[ColumnStatisticsTypeDef],
     },
@@ -9566,22 +9349,20 @@
     "_OptionalUpdateColumnStatisticsForTableRequestRequestTypeDef",
     {
         "CatalogId": str,
     },
     total=False,
 )
 
-
 class UpdateColumnStatisticsForTableRequestRequestTypeDef(
     _RequiredUpdateColumnStatisticsForTableRequestRequestTypeDef,
     _OptionalUpdateColumnStatisticsForTableRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredBatchCreatePartitionRequestRequestTypeDef = TypedDict(
     "_RequiredBatchCreatePartitionRequestRequestTypeDef",
     {
         "DatabaseName": str,
         "TableName": str,
         "PartitionInputList": Sequence[PartitionInputTypeDef],
     },
@@ -9590,22 +9371,20 @@
     "_OptionalBatchCreatePartitionRequestRequestTypeDef",
     {
         "CatalogId": str,
     },
     total=False,
 )
 
-
 class BatchCreatePartitionRequestRequestTypeDef(
     _RequiredBatchCreatePartitionRequestRequestTypeDef,
     _OptionalBatchCreatePartitionRequestRequestTypeDef,
 ):
     pass
 
-
 BatchUpdatePartitionRequestEntryTypeDef = TypedDict(
     "BatchUpdatePartitionRequestEntryTypeDef",
     {
         "PartitionValueList": Sequence[str],
         "PartitionInput": PartitionInputTypeDef,
     },
 )
@@ -9622,21 +9401,19 @@
     "_OptionalCreatePartitionRequestRequestTypeDef",
     {
         "CatalogId": str,
     },
     total=False,
 )
 
-
 class CreatePartitionRequestRequestTypeDef(
     _RequiredCreatePartitionRequestRequestTypeDef, _OptionalCreatePartitionRequestRequestTypeDef
 ):
     pass
 
-
 _RequiredUpdatePartitionRequestRequestTypeDef = TypedDict(
     "_RequiredUpdatePartitionRequestRequestTypeDef",
     {
         "DatabaseName": str,
         "TableName": str,
         "PartitionValueList": Sequence[str],
         "PartitionInput": PartitionInputTypeDef,
@@ -9646,21 +9423,19 @@
     "_OptionalUpdatePartitionRequestRequestTypeDef",
     {
         "CatalogId": str,
     },
     total=False,
 )
 
-
 class UpdatePartitionRequestRequestTypeDef(
     _RequiredUpdatePartitionRequestRequestTypeDef, _OptionalUpdatePartitionRequestRequestTypeDef
 ):
     pass
 
-
 BatchGetPartitionResponseTypeDef = TypedDict(
     "BatchGetPartitionResponseTypeDef",
     {
         "Partitions": List[PartitionTypeDef],
         "UnprocessedKeys": List[PartitionValueListTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -9712,25 +9487,24 @@
 )
 _OptionalCreateTableRequestRequestTypeDef = TypedDict(
     "_OptionalCreateTableRequestRequestTypeDef",
     {
         "CatalogId": str,
         "PartitionIndexes": Sequence[PartitionIndexTypeDef],
         "TransactionId": str,
+        "OpenTableFormatInput": OpenTableFormatInputTypeDef,
     },
     total=False,
 )
 
-
 class CreateTableRequestRequestTypeDef(
     _RequiredCreateTableRequestRequestTypeDef, _OptionalCreateTableRequestRequestTypeDef
 ):
     pass
 
-
 _RequiredUpdateTableRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateTableRequestRequestTypeDef",
     {
         "DatabaseName": str,
         "TableInput": TableInputTypeDef,
     },
 )
@@ -9741,21 +9515,19 @@
         "SkipArchive": bool,
         "TransactionId": str,
         "VersionId": str,
     },
     total=False,
 )
 
-
 class UpdateTableRequestRequestTypeDef(
     _RequiredUpdateTableRequestRequestTypeDef, _OptionalUpdateTableRequestRequestTypeDef
 ):
     pass
 
-
 GetTableResponseTypeDef = TypedDict(
     "GetTableResponseTypeDef",
     {
         "Table": TableTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -9828,21 +9600,19 @@
         "CodeGenConfigurationNodes": Mapping[str, CodeGenConfigurationNodeTypeDef],
         "ExecutionClass": ExecutionClassType,
         "SourceControlDetails": SourceControlDetailsTypeDef,
     },
     total=False,
 )
 
-
 class CreateJobRequestRequestTypeDef(
     _RequiredCreateJobRequestRequestTypeDef, _OptionalCreateJobRequestRequestTypeDef
 ):
     pass
 
-
 JobTypeDef = TypedDict(
     "JobTypeDef",
     {
         "Name": str,
         "Description": str,
         "LogUri": str,
         "Role": str,
@@ -9933,22 +9703,20 @@
     "_OptionalBatchUpdatePartitionRequestRequestTypeDef",
     {
         "CatalogId": str,
     },
     total=False,
 )
 
-
 class BatchUpdatePartitionRequestRequestTypeDef(
     _RequiredBatchUpdatePartitionRequestRequestTypeDef,
     _OptionalBatchUpdatePartitionRequestRequestTypeDef,
 ):
     pass
 
-
 GetUnfilteredPartitionsMetadataResponseTypeDef = TypedDict(
     "GetUnfilteredPartitionsMetadataResponseTypeDef",
     {
         "UnfilteredPartitions": List[UnfilteredPartitionTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
```

### Comparing `types-aiobotocore-glue-2.5.2.post3/types_aiobotocore_glue/type_defs.pyi` & `types-aiobotocore-glue-2.5.4/types_aiobotocore_glue/type_defs.py`

 * *Files 1% similar despite different names*

```diff
@@ -104,14 +104,15 @@
 else:
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
+
 __all__ = (
     "NotificationPropertyTypeDef",
     "AggregateOperationTypeDef",
     "AmazonRedshiftAdvancedOptionTypeDef",
     "OptionTypeDef",
     "ApplyMappingTypeDef",
     "AuditContextTypeDef",
@@ -195,14 +196,16 @@
     "ConnectionPasswordEncryptionTypeDef",
     "ConnectionsListTypeDef",
     "CrawlTypeDef",
     "CrawlerHistoryTypeDef",
     "CrawlerMetricsTypeDef",
     "DeltaTargetTypeDef",
     "DynamoDBTargetTypeDef",
+    "HudiTargetTypeDef",
+    "IcebergTargetTypeDef",
     "JdbcTargetTypeDef",
     "MongoDBTargetTypeDef",
     "S3TargetTypeDef",
     "LakeFormationConfigurationTypeDef",
     "LastCrawlInfoTypeDef",
     "LineageConfigurationTypeDef",
     "RecrawlPolicyTypeDef",
@@ -331,14 +334,15 @@
     "GetUserDefinedFunctionsRequestRequestTypeDef",
     "GetWorkflowRequestRequestTypeDef",
     "GetWorkflowRunPropertiesRequestRequestTypeDef",
     "GetWorkflowRunRequestRequestTypeDef",
     "GetWorkflowRunsRequestRequestTypeDef",
     "GlueStudioSchemaColumnTypeDef",
     "S3SourceAdditionalOptionsTypeDef",
+    "IcebergInputTypeDef",
     "ImportCatalogToGlueRequestRequestTypeDef",
     "ImportLabelsTaskRunPropertiesTypeDef",
     "JDBCConnectorOptionsTypeDef",
     "PredecessorTypeDef",
     "JoinColumnTypeDef",
     "KeySchemaElementTypeDef",
     "LabelingSetGenerationTaskRunPropertiesTypeDef",
@@ -359,14 +363,15 @@
     "MappingTypeDef",
     "OtherMetadataValueListItemTypeDef",
     "MetadataKeyValuePairTypeDef",
     "OrderTypeDef",
     "PropertyPredicateTypeDef",
     "PutResourcePolicyRequestRequestTypeDef",
     "PutWorkflowRunPropertiesRequestRequestTypeDef",
+    "RecipeReferenceTypeDef",
     "UpsertRedshiftTargetOptionsTypeDef",
     "ResetJobBookmarkRequestRequestTypeDef",
     "ResourceUriTypeDef",
     "ResumeWorkflowRunRequestRequestTypeDef",
     "RunStatementRequestRequestTypeDef",
     "S3DirectSourceAdditionalOptionsTypeDef",
     "SortCriterionTypeDef",
@@ -403,14 +408,15 @@
     "UpdateSourceControlFromJobRequestRequestTypeDef",
     "UpdateWorkflowRequestRequestTypeDef",
     "WorkflowRunStatisticsTypeDef",
     "ActionTypeDef",
     "StartJobRunRequestRequestTypeDef",
     "AggregateTypeDef",
     "AmazonRedshiftNodeDataTypeDef",
+    "SnowflakeNodeDataTypeDef",
     "GetUnfilteredPartitionMetadataRequestRequestTypeDef",
     "GetUnfilteredTableMetadataRequestRequestTypeDef",
     "BackfillErrorTypeDef",
     "BatchDeletePartitionRequestRequestTypeDef",
     "BatchGetPartitionRequestRequestTypeDef",
     "CancelMLTaskRunResponseTypeDef",
     "CheckSchemaVersionValidityResponseTypeDef",
@@ -583,33 +589,36 @@
     "GetResourcePoliciesResponseTypeDef",
     "GetSchemaVersionInputRequestTypeDef",
     "GetSchemaVersionsDiffInputRequestTypeDef",
     "UpdateSchemaInputRequestTypeDef",
     "GlueSchemaTypeDef",
     "GovernedCatalogSourceTypeDef",
     "S3CatalogSourceTypeDef",
+    "OpenTableFormatInputTypeDef",
     "JobRunTypeDef",
     "JoinTypeDef",
     "TaskRunPropertiesTypeDef",
     "ListRegistriesResponseTypeDef",
     "ListSchemaVersionsResponseTypeDef",
     "ListSchemasResponseTypeDef",
     "TransformEncryptionTypeDef",
     "MetadataInfoTypeDef",
     "PutSchemaVersionMetadataInputRequestTypeDef",
     "QuerySchemaVersionMetadataInputRequestTypeDef",
     "RemoveSchemaVersionMetadataInputRequestTypeDef",
+    "RecipeTypeDef",
     "RedshiftTargetTypeDef",
     "UserDefinedFunctionInputTypeDef",
     "UserDefinedFunctionTypeDef",
     "SearchTablesRequestRequestTypeDef",
     "StatementOutputTypeDef",
     "UpdateClassifierRequestRequestTypeDef",
     "AmazonRedshiftSourceTypeDef",
     "AmazonRedshiftTargetTypeDef",
+    "SnowflakeTargetTypeDef",
     "PartitionIndexDescriptorTypeDef",
     "BatchStopJobRunResponseTypeDef",
     "BatchUpdatePartitionResponseTypeDef",
     "BatchCreatePartitionResponseTypeDef",
     "BatchDeletePartitionResponseTypeDef",
     "BatchDeleteTableResponseTypeDef",
     "BatchDeleteTableVersionResponseTypeDef",
@@ -674,14 +683,15 @@
     "S3CatalogDeltaSourceTypeDef",
     "S3CatalogHudiSourceTypeDef",
     "S3CsvSourceTypeDef",
     "S3DeltaSourceTypeDef",
     "S3HudiSourceTypeDef",
     "S3JsonSourceTypeDef",
     "S3ParquetSourceTypeDef",
+    "SnowflakeSourceTypeDef",
     "SparkConnectorSourceTypeDef",
     "SparkConnectorTargetTypeDef",
     "SparkSQLTypeDef",
     "GetJobRunResponseTypeDef",
     "GetJobRunsResponseTypeDef",
     "JobNodeDetailsTypeDef",
     "GetMLTaskRunResponseTypeDef",
@@ -864,20 +874,22 @@
     "_OptionalBatchDeleteConnectionRequestRequestTypeDef",
     {
         "CatalogId": str,
     },
     total=False,
 )
 
+
 class BatchDeleteConnectionRequestRequestTypeDef(
     _RequiredBatchDeleteConnectionRequestRequestTypeDef,
     _OptionalBatchDeleteConnectionRequestRequestTypeDef,
 ):
     pass
 
+
 ErrorDetailTypeDef = TypedDict(
     "ErrorDetailTypeDef",
     {
         "ErrorCode": str,
         "ErrorMessage": str,
     },
     total=False,
@@ -895,19 +907,21 @@
     {
         "CatalogId": str,
         "TransactionId": str,
     },
     total=False,
 )
 
+
 class BatchDeleteTableRequestRequestTypeDef(
     _RequiredBatchDeleteTableRequestRequestTypeDef, _OptionalBatchDeleteTableRequestRequestTypeDef
 ):
     pass
 
+
 _RequiredBatchDeleteTableVersionRequestRequestTypeDef = TypedDict(
     "_RequiredBatchDeleteTableVersionRequestRequestTypeDef",
     {
         "DatabaseName": str,
         "TableName": str,
         "VersionIds": Sequence[str],
     },
@@ -916,20 +930,22 @@
     "_OptionalBatchDeleteTableVersionRequestRequestTypeDef",
     {
         "CatalogId": str,
     },
     total=False,
 )
 
+
 class BatchDeleteTableVersionRequestRequestTypeDef(
     _RequiredBatchDeleteTableVersionRequestRequestTypeDef,
     _OptionalBatchDeleteTableVersionRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredBatchGetBlueprintsRequestRequestTypeDef = TypedDict(
     "_RequiredBatchGetBlueprintsRequestRequestTypeDef",
     {
         "Names": Sequence[str],
     },
 )
 _OptionalBatchGetBlueprintsRequestRequestTypeDef = TypedDict(
@@ -937,20 +953,22 @@
     {
         "IncludeBlueprint": bool,
         "IncludeParameterSpec": bool,
     },
     total=False,
 )
 
+
 class BatchGetBlueprintsRequestRequestTypeDef(
     _RequiredBatchGetBlueprintsRequestRequestTypeDef,
     _OptionalBatchGetBlueprintsRequestRequestTypeDef,
 ):
     pass
 
+
 BatchGetCrawlersRequestRequestTypeDef = TypedDict(
     "BatchGetCrawlersRequestRequestTypeDef",
     {
         "CrawlerNames": Sequence[str],
     },
 )
 
@@ -972,17 +990,19 @@
     "_OptionalCustomEntityTypeTypeDef",
     {
         "ContextWords": List[str],
     },
     total=False,
 )
 
+
 class CustomEntityTypeTypeDef(_RequiredCustomEntityTypeTypeDef, _OptionalCustomEntityTypeTypeDef):
     pass
 
+
 BatchGetDataQualityResultRequestRequestTypeDef = TypedDict(
     "BatchGetDataQualityResultRequestRequestTypeDef",
     {
         "ResultIds": Sequence[str],
     },
 )
 
@@ -1049,19 +1069,21 @@
     "_OptionalBatchGetWorkflowsRequestRequestTypeDef",
     {
         "IncludeGraph": bool,
     },
     total=False,
 )
 
+
 class BatchGetWorkflowsRequestRequestTypeDef(
     _RequiredBatchGetWorkflowsRequestRequestTypeDef, _OptionalBatchGetWorkflowsRequestRequestTypeDef
 ):
     pass
 
+
 BatchStopJobRunRequestRequestTypeDef = TypedDict(
     "BatchStopJobRunRequestRequestTypeDef",
     {
         "JobName": str,
         "JobRunIds": Sequence[str],
     },
 )
@@ -1164,19 +1186,21 @@
     "_OptionalCancelStatementRequestRequestTypeDef",
     {
         "RequestOrigin": str,
     },
     total=False,
 )
 
+
 class CancelStatementRequestRequestTypeDef(
     _RequiredCancelStatementRequestRequestTypeDef, _OptionalCancelStatementRequestRequestTypeDef
 ):
     pass
 
+
 CatalogEntryTypeDef = TypedDict(
     "CatalogEntryTypeDef",
     {
         "DatabaseName": str,
         "TableName": str,
     },
 )
@@ -1285,17 +1309,19 @@
         "ConnectionName": str,
         "EventQueueArn": str,
         "DlqEventQueueArn": str,
     },
     total=False,
 )
 
+
 class CatalogTargetTypeDef(_RequiredCatalogTargetTypeDef, _OptionalCatalogTargetTypeDef):
     pass
 
+
 CheckSchemaVersionValidityInputRequestTypeDef = TypedDict(
     "CheckSchemaVersionValidityInputRequestTypeDef",
     {
         "DataFormat": DataFormatType,
         "SchemaDefinition": str,
     },
 )
@@ -1320,17 +1346,19 @@
         "AllowSingleColumn": bool,
         "CustomDatatypeConfigured": bool,
         "CustomDatatypes": List[str],
     },
     total=False,
 )
 
+
 class CsvClassifierTypeDef(_RequiredCsvClassifierTypeDef, _OptionalCsvClassifierTypeDef):
     pass
 
+
 _RequiredGrokClassifierTypeDef = TypedDict(
     "_RequiredGrokClassifierTypeDef",
     {
         "Name": str,
         "Classification": str,
         "GrokPattern": str,
     },
@@ -1342,17 +1370,19 @@
         "LastUpdated": datetime,
         "Version": int,
         "CustomPatterns": str,
     },
     total=False,
 )
 
+
 class GrokClassifierTypeDef(_RequiredGrokClassifierTypeDef, _OptionalGrokClassifierTypeDef):
     pass
 
+
 _RequiredJsonClassifierTypeDef = TypedDict(
     "_RequiredJsonClassifierTypeDef",
     {
         "Name": str,
         "JsonPath": str,
     },
 )
@@ -1362,17 +1392,19 @@
         "CreationTime": datetime,
         "LastUpdated": datetime,
         "Version": int,
     },
     total=False,
 )
 
+
 class JsonClassifierTypeDef(_RequiredJsonClassifierTypeDef, _OptionalJsonClassifierTypeDef):
     pass
 
+
 _RequiredXMLClassifierTypeDef = TypedDict(
     "_RequiredXMLClassifierTypeDef",
     {
         "Name": str,
         "Classification": str,
     },
 )
@@ -1383,17 +1415,19 @@
         "LastUpdated": datetime,
         "Version": int,
         "RowTag": str,
     },
     total=False,
 )
 
+
 class XMLClassifierTypeDef(_RequiredXMLClassifierTypeDef, _OptionalXMLClassifierTypeDef):
     pass
 
+
 CloudWatchEncryptionTypeDef = TypedDict(
     "CloudWatchEncryptionTypeDef",
     {
         "CloudWatchEncryptionMode": CloudWatchEncryptionModeType,
         "KmsKeyArn": str,
     },
     total=False,
@@ -1413,17 +1447,19 @@
     "_OptionalDirectJDBCSourceTypeDef",
     {
         "RedshiftTmpDir": str,
     },
     total=False,
 )
 
+
 class DirectJDBCSourceTypeDef(_RequiredDirectJDBCSourceTypeDef, _OptionalDirectJDBCSourceTypeDef):
     pass
 
+
 _RequiredDropDuplicatesTypeDef = TypedDict(
     "_RequiredDropDuplicatesTypeDef",
     {
         "Name": str,
         "Inputs": List[str],
     },
 )
@@ -1431,17 +1467,19 @@
     "_OptionalDropDuplicatesTypeDef",
     {
         "Columns": List[List[str]],
     },
     total=False,
 )
 
+
 class DropDuplicatesTypeDef(_RequiredDropDuplicatesTypeDef, _OptionalDropDuplicatesTypeDef):
     pass
 
+
 DropFieldsTypeDef = TypedDict(
     "DropFieldsTypeDef",
     {
         "Name": str,
         "Inputs": List[str],
         "Paths": List[List[str]],
     },
@@ -1468,19 +1506,21 @@
     "_OptionalFillMissingValuesTypeDef",
     {
         "FilledPath": str,
     },
     total=False,
 )
 
+
 class FillMissingValuesTypeDef(
     _RequiredFillMissingValuesTypeDef, _OptionalFillMissingValuesTypeDef
 ):
     pass
 
+
 MergeTypeDef = TypedDict(
     "MergeTypeDef",
     {
         "Name": str,
         "Inputs": List[str],
         "Source": str,
         "PrimaryKeys": List[List[str]],
@@ -1560,17 +1600,19 @@
         "SampleFraction": float,
         "ThresholdFraction": float,
         "MaskValue": str,
     },
     total=False,
 )
 
+
 class PIIDetectionTypeDef(_RequiredPIIDetectionTypeDef, _OptionalPIIDetectionTypeDef):
     pass
 
+
 PostgreSQLCatalogSourceTypeDef = TypedDict(
     "PostgreSQLCatalogSourceTypeDef",
     {
         "Name": str,
         "Database": str,
         "Table": str,
     },
@@ -1599,17 +1641,19 @@
     {
         "RedshiftTmpDir": str,
         "TmpDirIAMRole": str,
     },
     total=False,
 )
 
+
 class RedshiftSourceTypeDef(_RequiredRedshiftSourceTypeDef, _OptionalRedshiftSourceTypeDef):
     pass
 
+
 RelationalCatalogSourceTypeDef = TypedDict(
     "RelationalCatalogSourceTypeDef",
     {
         "Name": str,
         "Database": str,
         "Table": str,
     },
@@ -1656,17 +1700,19 @@
     {
         "Topk": int,
         "Prob": float,
     },
     total=False,
 )
 
+
 class SpigotTypeDef(_RequiredSpigotTypeDef, _OptionalSpigotTypeDef):
     pass
 
+
 SplitFieldsTypeDef = TypedDict(
     "SplitFieldsTypeDef",
     {
         "Name": str,
         "Inputs": List[str],
         "Paths": List[List[str]],
     },
@@ -1692,17 +1738,19 @@
     "_OptionalCodeGenEdgeTypeDef",
     {
         "TargetParameter": str,
     },
     total=False,
 )
 
+
 class CodeGenEdgeTypeDef(_RequiredCodeGenEdgeTypeDef, _OptionalCodeGenEdgeTypeDef):
     pass
 
+
 _RequiredCodeGenNodeArgTypeDef = TypedDict(
     "_RequiredCodeGenNodeArgTypeDef",
     {
         "Name": str,
         "Value": str,
     },
 )
@@ -1710,17 +1758,19 @@
     "_OptionalCodeGenNodeArgTypeDef",
     {
         "Param": bool,
     },
     total=False,
 )
 
+
 class CodeGenNodeArgTypeDef(_RequiredCodeGenNodeArgTypeDef, _OptionalCodeGenNodeArgTypeDef):
     pass
 
+
 ColumnImportanceTypeDef = TypedDict(
     "ColumnImportanceTypeDef",
     {
         "ColumnName": str,
         "Importance": float,
     },
     total=False,
@@ -1747,19 +1797,21 @@
     {
         "MinimumValue": datetime,
         "MaximumValue": datetime,
     },
     total=False,
 )
 
+
 class DateColumnStatisticsDataTypeDef(
     _RequiredDateColumnStatisticsDataTypeDef, _OptionalDateColumnStatisticsDataTypeDef
 ):
     pass
 
+
 _RequiredDoubleColumnStatisticsDataTypeDef = TypedDict(
     "_RequiredDoubleColumnStatisticsDataTypeDef",
     {
         "NumberOfNulls": int,
         "NumberOfDistinctValues": int,
     },
 )
@@ -1768,19 +1820,21 @@
     {
         "MinimumValue": float,
         "MaximumValue": float,
     },
     total=False,
 )
 
+
 class DoubleColumnStatisticsDataTypeDef(
     _RequiredDoubleColumnStatisticsDataTypeDef, _OptionalDoubleColumnStatisticsDataTypeDef
 ):
     pass
 
+
 _RequiredLongColumnStatisticsDataTypeDef = TypedDict(
     "_RequiredLongColumnStatisticsDataTypeDef",
     {
         "NumberOfNulls": int,
         "NumberOfDistinctValues": int,
     },
 )
@@ -1789,19 +1843,21 @@
     {
         "MinimumValue": int,
         "MaximumValue": int,
     },
     total=False,
 )
 
+
 class LongColumnStatisticsDataTypeDef(
     _RequiredLongColumnStatisticsDataTypeDef, _OptionalLongColumnStatisticsDataTypeDef
 ):
     pass
 
+
 StringColumnStatisticsDataTypeDef = TypedDict(
     "StringColumnStatisticsDataTypeDef",
     {
         "MaximumLength": int,
         "AverageLength": float,
         "NumberOfNulls": int,
         "NumberOfDistinctValues": int,
@@ -1820,17 +1876,19 @@
         "Type": str,
         "Comment": str,
         "Parameters": Mapping[str, str],
     },
     total=False,
 )
 
+
 class ColumnTypeDef(_RequiredColumnTypeDef, _OptionalColumnTypeDef):
     pass
 
+
 ConditionTypeDef = TypedDict(
     "ConditionTypeDef",
     {
         "LogicalOperator": Literal["EQUALS"],
         "JobName": str,
         "State": JobRunStateType,
         "CrawlerName": str,
@@ -1870,19 +1928,21 @@
     "_OptionalConnectionPasswordEncryptionTypeDef",
     {
         "AwsKmsKeyId": str,
     },
     total=False,
 )
 
+
 class ConnectionPasswordEncryptionTypeDef(
     _RequiredConnectionPasswordEncryptionTypeDef, _OptionalConnectionPasswordEncryptionTypeDef
 ):
     pass
 
+
 ConnectionsListTypeDef = TypedDict(
     "ConnectionsListTypeDef",
     {
         "Connections": List[str],
     },
     total=False,
 )
@@ -1949,14 +2009,36 @@
         "Path": str,
         "scanAll": bool,
         "scanRate": float,
     },
     total=False,
 )
 
+HudiTargetTypeDef = TypedDict(
+    "HudiTargetTypeDef",
+    {
+        "Paths": List[str],
+        "ConnectionName": str,
+        "Exclusions": List[str],
+        "MaximumTraversalDepth": int,
+    },
+    total=False,
+)
+
+IcebergTargetTypeDef = TypedDict(
+    "IcebergTargetTypeDef",
+    {
+        "Paths": List[str],
+        "ConnectionName": str,
+        "Exclusions": List[str],
+        "MaximumTraversalDepth": int,
+    },
+    total=False,
+)
+
 JdbcTargetTypeDef = TypedDict(
     "JdbcTargetTypeDef",
     {
         "ConnectionName": str,
         "Path": str,
         "Exclusions": List[str],
         "EnableAdditionalMetadata": List[JdbcMetadataEntryType],
@@ -2065,19 +2147,21 @@
     {
         "Description": str,
         "Tags": Mapping[str, str],
     },
     total=False,
 )
 
+
 class CreateBlueprintRequestRequestTypeDef(
     _RequiredCreateBlueprintRequestRequestTypeDef, _OptionalCreateBlueprintRequestRequestTypeDef
 ):
     pass
 
+
 _RequiredCreateCsvClassifierRequestTypeDef = TypedDict(
     "_RequiredCreateCsvClassifierRequestTypeDef",
     {
         "Name": str,
     },
 )
 _OptionalCreateCsvClassifierRequestTypeDef = TypedDict(
@@ -2091,19 +2175,21 @@
         "AllowSingleColumn": bool,
         "CustomDatatypeConfigured": bool,
         "CustomDatatypes": Sequence[str],
     },
     total=False,
 )
 
+
 class CreateCsvClassifierRequestTypeDef(
     _RequiredCreateCsvClassifierRequestTypeDef, _OptionalCreateCsvClassifierRequestTypeDef
 ):
     pass
 
+
 _RequiredCreateGrokClassifierRequestTypeDef = TypedDict(
     "_RequiredCreateGrokClassifierRequestTypeDef",
     {
         "Classification": str,
         "Name": str,
         "GrokPattern": str,
     },
@@ -2112,19 +2198,21 @@
     "_OptionalCreateGrokClassifierRequestTypeDef",
     {
         "CustomPatterns": str,
     },
     total=False,
 )
 
+
 class CreateGrokClassifierRequestTypeDef(
     _RequiredCreateGrokClassifierRequestTypeDef, _OptionalCreateGrokClassifierRequestTypeDef
 ):
     pass
 
+
 CreateJsonClassifierRequestTypeDef = TypedDict(
     "CreateJsonClassifierRequestTypeDef",
     {
         "Name": str,
         "JsonPath": str,
     },
 )
@@ -2140,19 +2228,21 @@
     "_OptionalCreateXMLClassifierRequestTypeDef",
     {
         "RowTag": str,
     },
     total=False,
 )
 
+
 class CreateXMLClassifierRequestTypeDef(
     _RequiredCreateXMLClassifierRequestTypeDef, _OptionalCreateXMLClassifierRequestTypeDef
 ):
     pass
 
+
 _RequiredCreateCustomEntityTypeRequestRequestTypeDef = TypedDict(
     "_RequiredCreateCustomEntityTypeRequestRequestTypeDef",
     {
         "Name": str,
         "RegexString": str,
     },
 )
@@ -2161,20 +2251,22 @@
     {
         "ContextWords": Sequence[str],
         "Tags": Mapping[str, str],
     },
     total=False,
 )
 
+
 class CreateCustomEntityTypeRequestRequestTypeDef(
     _RequiredCreateCustomEntityTypeRequestRequestTypeDef,
     _OptionalCreateCustomEntityTypeRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredDataQualityTargetTableTypeDef = TypedDict(
     "_RequiredDataQualityTargetTableTypeDef",
     {
         "TableName": str,
         "DatabaseName": str,
     },
 )
@@ -2182,19 +2274,21 @@
     "_OptionalDataQualityTargetTableTypeDef",
     {
         "CatalogId": str,
     },
     total=False,
 )
 
+
 class DataQualityTargetTableTypeDef(
     _RequiredDataQualityTargetTableTypeDef, _OptionalDataQualityTargetTableTypeDef
 ):
     pass
 
+
 _RequiredCreateDevEndpointRequestRequestTypeDef = TypedDict(
     "_RequiredCreateDevEndpointRequestRequestTypeDef",
     {
         "EndpointName": str,
         "RoleArn": str,
     },
 )
@@ -2214,19 +2308,21 @@
         "SecurityConfiguration": str,
         "Tags": Mapping[str, str],
         "Arguments": Mapping[str, str],
     },
     total=False,
 )
 
+
 class CreateDevEndpointRequestRequestTypeDef(
     _RequiredCreateDevEndpointRequestRequestTypeDef, _OptionalCreateDevEndpointRequestRequestTypeDef
 ):
     pass
 
+
 ExecutionPropertyTypeDef = TypedDict(
     "ExecutionPropertyTypeDef",
     {
         "MaxConcurrentRuns": int,
     },
     total=False,
 )
@@ -2270,17 +2366,19 @@
         "CatalogId": str,
         "ConnectionName": str,
         "AdditionalOptions": Dict[str, str],
     },
     total=False,
 )
 
+
 class GlueTableTypeDef(_RequiredGlueTableTypeDef, _OptionalGlueTableTypeDef):
     pass
 
+
 PartitionIndexTypeDef = TypedDict(
     "PartitionIndexTypeDef",
     {
         "Keys": Sequence[str],
         "IndexName": str,
     },
 )
@@ -2296,19 +2394,21 @@
     {
         "Description": str,
         "Tags": Mapping[str, str],
     },
     total=False,
 )
 
+
 class CreateRegistryInputRequestTypeDef(
     _RequiredCreateRegistryInputRequestTypeDef, _OptionalCreateRegistryInputRequestTypeDef
 ):
     pass
 
+
 RegistryIdTypeDef = TypedDict(
     "RegistryIdTypeDef",
     {
         "RegistryName": str,
         "RegistryArn": str,
     },
     total=False,
@@ -2333,19 +2433,21 @@
     "_OptionalEventBatchingConditionTypeDef",
     {
         "BatchWindow": int,
     },
     total=False,
 )
 
+
 class EventBatchingConditionTypeDef(
     _RequiredEventBatchingConditionTypeDef, _OptionalEventBatchingConditionTypeDef
 ):
     pass
 
+
 _RequiredCreateWorkflowRequestRequestTypeDef = TypedDict(
     "_RequiredCreateWorkflowRequestRequestTypeDef",
     {
         "Name": str,
     },
 )
 _OptionalCreateWorkflowRequestRequestTypeDef = TypedDict(
@@ -2355,19 +2457,21 @@
         "DefaultRunProperties": Mapping[str, str],
         "Tags": Mapping[str, str],
         "MaxConcurrentRuns": int,
     },
     total=False,
 )
 
+
 class CreateWorkflowRequestRequestTypeDef(
     _RequiredCreateWorkflowRequestRequestTypeDef, _OptionalCreateWorkflowRequestRequestTypeDef
 ):
     pass
 
+
 DQResultsPublishingOptionsTypeDef = TypedDict(
     "DQResultsPublishingOptionsTypeDef",
     {
         "EvaluationContext": str,
         "ResultsS3Prefix": str,
         "CloudWatchMetricsEnabled": bool,
         "ResultsPublishingEnabled": bool,
@@ -2393,17 +2497,19 @@
     "_OptionalEncryptionAtRestTypeDef",
     {
         "SseAwsKmsKeyId": str,
     },
     total=False,
 )
 
+
 class EncryptionAtRestTypeDef(_RequiredEncryptionAtRestTypeDef, _OptionalEncryptionAtRestTypeDef):
     pass
 
+
 DataLakePrincipalTypeDef = TypedDict(
     "DataLakePrincipalTypeDef",
     {
         "DataLakePrincipalIdentifier": str,
     },
     total=False,
 )
@@ -2492,20 +2598,22 @@
     "_OptionalDeleteColumnStatisticsForPartitionRequestRequestTypeDef",
     {
         "CatalogId": str,
     },
     total=False,
 )
 
+
 class DeleteColumnStatisticsForPartitionRequestRequestTypeDef(
     _RequiredDeleteColumnStatisticsForPartitionRequestRequestTypeDef,
     _OptionalDeleteColumnStatisticsForPartitionRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredDeleteColumnStatisticsForTableRequestRequestTypeDef = TypedDict(
     "_RequiredDeleteColumnStatisticsForTableRequestRequestTypeDef",
     {
         "DatabaseName": str,
         "TableName": str,
         "ColumnName": str,
     },
@@ -2514,39 +2622,43 @@
     "_OptionalDeleteColumnStatisticsForTableRequestRequestTypeDef",
     {
         "CatalogId": str,
     },
     total=False,
 )
 
+
 class DeleteColumnStatisticsForTableRequestRequestTypeDef(
     _RequiredDeleteColumnStatisticsForTableRequestRequestTypeDef,
     _OptionalDeleteColumnStatisticsForTableRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredDeleteConnectionRequestRequestTypeDef = TypedDict(
     "_RequiredDeleteConnectionRequestRequestTypeDef",
     {
         "ConnectionName": str,
     },
 )
 _OptionalDeleteConnectionRequestRequestTypeDef = TypedDict(
     "_OptionalDeleteConnectionRequestRequestTypeDef",
     {
         "CatalogId": str,
     },
     total=False,
 )
 
+
 class DeleteConnectionRequestRequestTypeDef(
     _RequiredDeleteConnectionRequestRequestTypeDef, _OptionalDeleteConnectionRequestRequestTypeDef
 ):
     pass
 
+
 DeleteCrawlerRequestRequestTypeDef = TypedDict(
     "DeleteCrawlerRequestRequestTypeDef",
     {
         "Name": str,
     },
 )
 
@@ -2574,19 +2686,21 @@
     "_OptionalDeleteDatabaseRequestRequestTypeDef",
     {
         "CatalogId": str,
     },
     total=False,
 )
 
+
 class DeleteDatabaseRequestRequestTypeDef(
     _RequiredDeleteDatabaseRequestRequestTypeDef, _OptionalDeleteDatabaseRequestRequestTypeDef
 ):
     pass
 
+
 DeleteDevEndpointRequestRequestTypeDef = TypedDict(
     "DeleteDevEndpointRequestRequestTypeDef",
     {
         "EndpointName": str,
     },
 )
 
@@ -2616,20 +2730,22 @@
     "_OptionalDeletePartitionIndexRequestRequestTypeDef",
     {
         "CatalogId": str,
     },
     total=False,
 )
 
+
 class DeletePartitionIndexRequestRequestTypeDef(
     _RequiredDeletePartitionIndexRequestRequestTypeDef,
     _OptionalDeletePartitionIndexRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredDeletePartitionRequestRequestTypeDef = TypedDict(
     "_RequiredDeletePartitionRequestRequestTypeDef",
     {
         "DatabaseName": str,
         "TableName": str,
         "PartitionValues": Sequence[str],
     },
@@ -2638,19 +2754,21 @@
     "_OptionalDeletePartitionRequestRequestTypeDef",
     {
         "CatalogId": str,
     },
     total=False,
 )
 
+
 class DeletePartitionRequestRequestTypeDef(
     _RequiredDeletePartitionRequestRequestTypeDef, _OptionalDeletePartitionRequestRequestTypeDef
 ):
     pass
 
+
 DeleteResourcePolicyRequestRequestTypeDef = TypedDict(
     "DeleteResourcePolicyRequestRequestTypeDef",
     {
         "PolicyHashCondition": str,
         "ResourceArn": str,
     },
     total=False,
@@ -2683,19 +2801,21 @@
     "_OptionalDeleteSessionRequestRequestTypeDef",
     {
         "RequestOrigin": str,
     },
     total=False,
 )
 
+
 class DeleteSessionRequestRequestTypeDef(
     _RequiredDeleteSessionRequestRequestTypeDef, _OptionalDeleteSessionRequestRequestTypeDef
 ):
     pass
 
+
 _RequiredDeleteTableRequestRequestTypeDef = TypedDict(
     "_RequiredDeleteTableRequestRequestTypeDef",
     {
         "DatabaseName": str,
         "Name": str,
     },
 )
@@ -2704,19 +2824,21 @@
     {
         "CatalogId": str,
         "TransactionId": str,
     },
     total=False,
 )
 
+
 class DeleteTableRequestRequestTypeDef(
     _RequiredDeleteTableRequestRequestTypeDef, _OptionalDeleteTableRequestRequestTypeDef
 ):
     pass
 
+
 _RequiredDeleteTableVersionRequestRequestTypeDef = TypedDict(
     "_RequiredDeleteTableVersionRequestRequestTypeDef",
     {
         "DatabaseName": str,
         "TableName": str,
         "VersionId": str,
     },
@@ -2725,20 +2847,22 @@
     "_OptionalDeleteTableVersionRequestRequestTypeDef",
     {
         "CatalogId": str,
     },
     total=False,
 )
 
+
 class DeleteTableVersionRequestRequestTypeDef(
     _RequiredDeleteTableVersionRequestRequestTypeDef,
     _OptionalDeleteTableVersionRequestRequestTypeDef,
 ):
     pass
 
+
 DeleteTriggerRequestRequestTypeDef = TypedDict(
     "DeleteTriggerRequestRequestTypeDef",
     {
         "Name": str,
     },
 )
 
@@ -2753,20 +2877,22 @@
     "_OptionalDeleteUserDefinedFunctionRequestRequestTypeDef",
     {
         "CatalogId": str,
     },
     total=False,
 )
 
+
 class DeleteUserDefinedFunctionRequestRequestTypeDef(
     _RequiredDeleteUserDefinedFunctionRequestRequestTypeDef,
     _OptionalDeleteUserDefinedFunctionRequestRequestTypeDef,
 ):
     pass
 
+
 DeleteWorkflowRequestRequestTypeDef = TypedDict(
     "DeleteWorkflowRequestRequestTypeDef",
     {
         "Name": str,
     },
 )
 
@@ -2815,19 +2941,21 @@
         "Value": List[str],
         "ListType": ParamTypeType,
         "IsOptional": bool,
     },
     total=False,
 )
 
+
 class TransformConfigParameterTypeDef(
     _RequiredTransformConfigParameterTypeDef, _OptionalTransformConfigParameterTypeDef
 ):
     pass
 
+
 EdgeTypeDef = TypedDict(
     "EdgeTypeDef",
     {
         "SourceId": str,
         "DestinationId": str,
     },
     total=False,
@@ -2918,19 +3046,21 @@
     {
         "IncludeBlueprint": bool,
         "IncludeParameterSpec": bool,
     },
     total=False,
 )
 
+
 class GetBlueprintRequestRequestTypeDef(
     _RequiredGetBlueprintRequestRequestTypeDef, _OptionalGetBlueprintRequestRequestTypeDef
 ):
     pass
 
+
 GetBlueprintRunRequestRequestTypeDef = TypedDict(
     "GetBlueprintRunRequestRequestTypeDef",
     {
         "BlueprintName": str,
         "RunId": str,
     },
 )
@@ -2946,19 +3076,21 @@
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
+
 class GetBlueprintRunsRequestRequestTypeDef(
     _RequiredGetBlueprintRunsRequestRequestTypeDef, _OptionalGetBlueprintRunsRequestRequestTypeDef
 ):
     pass
 
+
 GetCatalogImportStatusRequestRequestTypeDef = TypedDict(
     "GetCatalogImportStatusRequestRequestTypeDef",
     {
         "CatalogId": str,
     },
     total=False,
 )
@@ -3002,20 +3134,22 @@
     "_OptionalGetColumnStatisticsForPartitionRequestRequestTypeDef",
     {
         "CatalogId": str,
     },
     total=False,
 )
 
+
 class GetColumnStatisticsForPartitionRequestRequestTypeDef(
     _RequiredGetColumnStatisticsForPartitionRequestRequestTypeDef,
     _OptionalGetColumnStatisticsForPartitionRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredGetColumnStatisticsForTableRequestRequestTypeDef = TypedDict(
     "_RequiredGetColumnStatisticsForTableRequestRequestTypeDef",
     {
         "DatabaseName": str,
         "TableName": str,
         "ColumnNames": Sequence[str],
     },
@@ -3024,20 +3158,22 @@
     "_OptionalGetColumnStatisticsForTableRequestRequestTypeDef",
     {
         "CatalogId": str,
     },
     total=False,
 )
 
+
 class GetColumnStatisticsForTableRequestRequestTypeDef(
     _RequiredGetColumnStatisticsForTableRequestRequestTypeDef,
     _OptionalGetColumnStatisticsForTableRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredGetConnectionRequestRequestTypeDef = TypedDict(
     "_RequiredGetConnectionRequestRequestTypeDef",
     {
         "Name": str,
     },
 )
 _OptionalGetConnectionRequestRequestTypeDef = TypedDict(
@@ -3045,19 +3181,21 @@
     {
         "CatalogId": str,
         "HidePassword": bool,
     },
     total=False,
 )
 
+
 class GetConnectionRequestRequestTypeDef(
     _RequiredGetConnectionRequestRequestTypeDef, _OptionalGetConnectionRequestRequestTypeDef
 ):
     pass
 
+
 GetConnectionsFilterTypeDef = TypedDict(
     "GetConnectionsFilterTypeDef",
     {
         "MatchCriteria": Sequence[str],
         "ConnectionType": ConnectionTypeType,
     },
     total=False,
@@ -3142,19 +3280,21 @@
     "_OptionalGetDatabaseRequestRequestTypeDef",
     {
         "CatalogId": str,
     },
     total=False,
 )
 
+
 class GetDatabaseRequestRequestTypeDef(
     _RequiredGetDatabaseRequestRequestTypeDef, _OptionalGetDatabaseRequestRequestTypeDef
 ):
     pass
 
+
 GetDatabasesRequestRequestTypeDef = TypedDict(
     "GetDatabasesRequestRequestTypeDef",
     {
         "CatalogId": str,
         "NextToken": str,
         "MaxResults": int,
         "ResourceShareType": ResourceShareTypeType,
@@ -3196,19 +3336,21 @@
     "_OptionalGetJobBookmarkRequestRequestTypeDef",
     {
         "RunId": str,
     },
     total=False,
 )
 
+
 class GetJobBookmarkRequestRequestTypeDef(
     _RequiredGetJobBookmarkRequestRequestTypeDef, _OptionalGetJobBookmarkRequestRequestTypeDef
 ):
     pass
 
+
 JobBookmarkEntryTypeDef = TypedDict(
     "JobBookmarkEntryTypeDef",
     {
         "JobName": str,
         "Version": int,
         "Run": int,
         "Attempt": int,
@@ -3237,19 +3379,21 @@
     "_OptionalGetJobRunRequestRequestTypeDef",
     {
         "PredecessorsIncluded": bool,
     },
     total=False,
 )
 
+
 class GetJobRunRequestRequestTypeDef(
     _RequiredGetJobRunRequestRequestTypeDef, _OptionalGetJobRunRequestRequestTypeDef
 ):
     pass
 
+
 _RequiredGetJobRunsRequestRequestTypeDef = TypedDict(
     "_RequiredGetJobRunsRequestRequestTypeDef",
     {
         "JobName": str,
     },
 )
 _OptionalGetJobRunsRequestRequestTypeDef = TypedDict(
@@ -3257,19 +3401,21 @@
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
+
 class GetJobRunsRequestRequestTypeDef(
     _RequiredGetJobRunsRequestRequestTypeDef, _OptionalGetJobRunsRequestRequestTypeDef
 ):
     pass
 
+
 GetJobsRequestRequestTypeDef = TypedDict(
     "GetJobsRequestRequestTypeDef",
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
@@ -3340,20 +3486,22 @@
     {
         "CatalogId": str,
         "NextToken": str,
     },
     total=False,
 )
 
+
 class GetPartitionIndexesRequestRequestTypeDef(
     _RequiredGetPartitionIndexesRequestRequestTypeDef,
     _OptionalGetPartitionIndexesRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredGetPartitionRequestRequestTypeDef = TypedDict(
     "_RequiredGetPartitionRequestRequestTypeDef",
     {
         "DatabaseName": str,
         "TableName": str,
         "PartitionValues": Sequence[str],
     },
@@ -3362,19 +3510,21 @@
     "_OptionalGetPartitionRequestRequestTypeDef",
     {
         "CatalogId": str,
     },
     total=False,
 )
 
+
 class GetPartitionRequestRequestTypeDef(
     _RequiredGetPartitionRequestRequestTypeDef, _OptionalGetPartitionRequestRequestTypeDef
 ):
     pass
 
+
 SegmentTypeDef = TypedDict(
     "SegmentTypeDef",
     {
         "SegmentNumber": int,
         "TotalSegments": int,
     },
 )
@@ -3442,19 +3592,21 @@
     "_OptionalGetSessionRequestRequestTypeDef",
     {
         "RequestOrigin": str,
     },
     total=False,
 )
 
+
 class GetSessionRequestRequestTypeDef(
     _RequiredGetSessionRequestRequestTypeDef, _OptionalGetSessionRequestRequestTypeDef
 ):
     pass
 
+
 _RequiredGetStatementRequestRequestTypeDef = TypedDict(
     "_RequiredGetStatementRequestRequestTypeDef",
     {
         "SessionId": str,
         "Id": int,
     },
 )
@@ -3462,19 +3614,21 @@
     "_OptionalGetStatementRequestRequestTypeDef",
     {
         "RequestOrigin": str,
     },
     total=False,
 )
 
+
 class GetStatementRequestRequestTypeDef(
     _RequiredGetStatementRequestRequestTypeDef, _OptionalGetStatementRequestRequestTypeDef
 ):
     pass
 
+
 _RequiredGetTableVersionRequestRequestTypeDef = TypedDict(
     "_RequiredGetTableVersionRequestRequestTypeDef",
     {
         "DatabaseName": str,
         "TableName": str,
     },
 )
@@ -3483,19 +3637,21 @@
     {
         "CatalogId": str,
         "VersionId": str,
     },
     total=False,
 )
 
+
 class GetTableVersionRequestRequestTypeDef(
     _RequiredGetTableVersionRequestRequestTypeDef, _OptionalGetTableVersionRequestRequestTypeDef
 ):
     pass
 
+
 _RequiredGetTableVersionsRequestRequestTypeDef = TypedDict(
     "_RequiredGetTableVersionsRequestRequestTypeDef",
     {
         "DatabaseName": str,
         "TableName": str,
     },
 )
@@ -3505,19 +3661,21 @@
         "CatalogId": str,
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
+
 class GetTableVersionsRequestRequestTypeDef(
     _RequiredGetTableVersionsRequestRequestTypeDef, _OptionalGetTableVersionsRequestRequestTypeDef
 ):
     pass
 
+
 GetTagsRequestRequestTypeDef = TypedDict(
     "GetTagsRequestRequestTypeDef",
     {
         "ResourceArn": str,
     },
 )
 
@@ -3549,20 +3707,22 @@
     "_OptionalGetUserDefinedFunctionRequestRequestTypeDef",
     {
         "CatalogId": str,
     },
     total=False,
 )
 
+
 class GetUserDefinedFunctionRequestRequestTypeDef(
     _RequiredGetUserDefinedFunctionRequestRequestTypeDef,
     _OptionalGetUserDefinedFunctionRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredGetUserDefinedFunctionsRequestRequestTypeDef = TypedDict(
     "_RequiredGetUserDefinedFunctionsRequestRequestTypeDef",
     {
         "Pattern": str,
     },
 )
 _OptionalGetUserDefinedFunctionsRequestRequestTypeDef = TypedDict(
@@ -3572,39 +3732,43 @@
         "DatabaseName": str,
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
+
 class GetUserDefinedFunctionsRequestRequestTypeDef(
     _RequiredGetUserDefinedFunctionsRequestRequestTypeDef,
     _OptionalGetUserDefinedFunctionsRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredGetWorkflowRequestRequestTypeDef = TypedDict(
     "_RequiredGetWorkflowRequestRequestTypeDef",
     {
         "Name": str,
     },
 )
 _OptionalGetWorkflowRequestRequestTypeDef = TypedDict(
     "_OptionalGetWorkflowRequestRequestTypeDef",
     {
         "IncludeGraph": bool,
     },
     total=False,
 )
 
+
 class GetWorkflowRequestRequestTypeDef(
     _RequiredGetWorkflowRequestRequestTypeDef, _OptionalGetWorkflowRequestRequestTypeDef
 ):
     pass
 
+
 GetWorkflowRunPropertiesRequestRequestTypeDef = TypedDict(
     "GetWorkflowRunPropertiesRequestRequestTypeDef",
     {
         "Name": str,
         "RunId": str,
     },
 )
@@ -3620,19 +3784,21 @@
     "_OptionalGetWorkflowRunRequestRequestTypeDef",
     {
         "IncludeGraph": bool,
     },
     total=False,
 )
 
+
 class GetWorkflowRunRequestRequestTypeDef(
     _RequiredGetWorkflowRunRequestRequestTypeDef, _OptionalGetWorkflowRunRequestRequestTypeDef
 ):
     pass
 
+
 _RequiredGetWorkflowRunsRequestRequestTypeDef = TypedDict(
     "_RequiredGetWorkflowRunsRequestRequestTypeDef",
     {
         "Name": str,
     },
 )
 _OptionalGetWorkflowRunsRequestRequestTypeDef = TypedDict(
@@ -3641,47 +3807,70 @@
         "IncludeGraph": bool,
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
+
 class GetWorkflowRunsRequestRequestTypeDef(
     _RequiredGetWorkflowRunsRequestRequestTypeDef, _OptionalGetWorkflowRunsRequestRequestTypeDef
 ):
     pass
 
+
 _RequiredGlueStudioSchemaColumnTypeDef = TypedDict(
     "_RequiredGlueStudioSchemaColumnTypeDef",
     {
         "Name": str,
     },
 )
 _OptionalGlueStudioSchemaColumnTypeDef = TypedDict(
     "_OptionalGlueStudioSchemaColumnTypeDef",
     {
         "Type": str,
     },
     total=False,
 )
 
+
 class GlueStudioSchemaColumnTypeDef(
     _RequiredGlueStudioSchemaColumnTypeDef, _OptionalGlueStudioSchemaColumnTypeDef
 ):
     pass
 
+
 S3SourceAdditionalOptionsTypeDef = TypedDict(
     "S3SourceAdditionalOptionsTypeDef",
     {
         "BoundedSize": int,
         "BoundedFiles": int,
     },
     total=False,
 )
 
+_RequiredIcebergInputTypeDef = TypedDict(
+    "_RequiredIcebergInputTypeDef",
+    {
+        "MetadataOperation": Literal["CREATE"],
+    },
+)
+_OptionalIcebergInputTypeDef = TypedDict(
+    "_OptionalIcebergInputTypeDef",
+    {
+        "Version": str,
+    },
+    total=False,
+)
+
+
+class IcebergInputTypeDef(_RequiredIcebergInputTypeDef, _OptionalIcebergInputTypeDef):
+    pass
+
+
 ImportCatalogToGlueRequestRequestTypeDef = TypedDict(
     "ImportCatalogToGlueRequestRequestTypeDef",
     {
         "CatalogId": str,
     },
     total=False,
 )
@@ -3863,19 +4052,21 @@
     {
         "RequestOrigin": str,
         "NextToken": str,
     },
     total=False,
 )
 
+
 class ListStatementsRequestRequestTypeDef(
     _RequiredListStatementsRequestRequestTypeDef, _OptionalListStatementsRequestRequestTypeDef
 ):
     pass
 
+
 ListTriggersRequestRequestTypeDef = TypedDict(
     "ListTriggersRequestRequestTypeDef",
     {
         "NextToken": str,
         "DependentJobName": str,
         "MaxResults": int,
         "Tags": Mapping[str, str],
@@ -3902,19 +4093,21 @@
     "_OptionalMLUserDataEncryptionTypeDef",
     {
         "KmsKeyId": str,
     },
     total=False,
 )
 
+
 class MLUserDataEncryptionTypeDef(
     _RequiredMLUserDataEncryptionTypeDef, _OptionalMLUserDataEncryptionTypeDef
 ):
     pass
 
+
 MappingTypeDef = TypedDict(
     "MappingTypeDef",
     {
         "ToKey": str,
         "FromPath": List[str],
         "FromType": str,
         "ToType": str,
@@ -3973,28 +4166,38 @@
         "PolicyHashCondition": str,
         "PolicyExistsCondition": ExistConditionType,
         "EnableHybrid": EnableHybridValuesType,
     },
     total=False,
 )
 
+
 class PutResourcePolicyRequestRequestTypeDef(
     _RequiredPutResourcePolicyRequestRequestTypeDef, _OptionalPutResourcePolicyRequestRequestTypeDef
 ):
     pass
 
+
 PutWorkflowRunPropertiesRequestRequestTypeDef = TypedDict(
     "PutWorkflowRunPropertiesRequestRequestTypeDef",
     {
         "Name": str,
         "RunId": str,
         "RunProperties": Mapping[str, str],
     },
 )
 
+RecipeReferenceTypeDef = TypedDict(
+    "RecipeReferenceTypeDef",
+    {
+        "RecipeArn": str,
+        "RecipeVersion": str,
+    },
+)
+
 UpsertRedshiftTargetOptionsTypeDef = TypedDict(
     "UpsertRedshiftTargetOptionsTypeDef",
     {
         "TableLocation": str,
         "ConnectionName": str,
         "UpsertKeys": List[str],
     },
@@ -4011,19 +4214,21 @@
     "_OptionalResetJobBookmarkRequestRequestTypeDef",
     {
         "RunId": str,
     },
     total=False,
 )
 
+
 class ResetJobBookmarkRequestRequestTypeDef(
     _RequiredResetJobBookmarkRequestRequestTypeDef, _OptionalResetJobBookmarkRequestRequestTypeDef
 ):
     pass
 
+
 ResourceUriTypeDef = TypedDict(
     "ResourceUriTypeDef",
     {
         "ResourceType": ResourceTypeType,
         "Uri": str,
     },
     total=False,
@@ -4049,19 +4254,21 @@
     "_OptionalRunStatementRequestRequestTypeDef",
     {
         "RequestOrigin": str,
     },
     total=False,
 )
 
+
 class RunStatementRequestRequestTypeDef(
     _RequiredRunStatementRequestRequestTypeDef, _OptionalRunStatementRequestRequestTypeDef
 ):
     pass
 
+
 S3DirectSourceAdditionalOptionsTypeDef = TypedDict(
     "S3DirectSourceAdditionalOptionsTypeDef",
     {
         "BoundedSize": int,
         "BoundedFiles": int,
         "EnableSamplePath": bool,
         "SamplePath": str,
@@ -4117,19 +4324,21 @@
     "_OptionalStartBlueprintRunRequestRequestTypeDef",
     {
         "Parameters": str,
     },
     total=False,
 )
 
+
 class StartBlueprintRunRequestRequestTypeDef(
     _RequiredStartBlueprintRunRequestRequestTypeDef, _OptionalStartBlueprintRunRequestRequestTypeDef
 ):
     pass
 
+
 StartCrawlerRequestRequestTypeDef = TypedDict(
     "StartCrawlerRequestRequestTypeDef",
     {
         "Name": str,
     },
 )
 
@@ -4159,20 +4368,22 @@
     "_OptionalStartImportLabelsTaskRunRequestRequestTypeDef",
     {
         "ReplaceAllLabels": bool,
     },
     total=False,
 )
 
+
 class StartImportLabelsTaskRunRequestRequestTypeDef(
     _RequiredStartImportLabelsTaskRunRequestRequestTypeDef,
     _OptionalStartImportLabelsTaskRunRequestRequestTypeDef,
 ):
     pass
 
+
 StartMLEvaluationTaskRunRequestRequestTypeDef = TypedDict(
     "StartMLEvaluationTaskRunRequestRequestTypeDef",
     {
         "TransformId": str,
     },
 )
 
@@ -4201,19 +4412,21 @@
     "_OptionalStartWorkflowRunRequestRequestTypeDef",
     {
         "RunProperties": Mapping[str, str],
     },
     total=False,
 )
 
+
 class StartWorkflowRunRequestRequestTypeDef(
     _RequiredStartWorkflowRunRequestRequestTypeDef, _OptionalStartWorkflowRunRequestRequestTypeDef
 ):
     pass
 
+
 StartingEventBatchConditionTypeDef = TypedDict(
     "StartingEventBatchConditionTypeDef",
     {
         "BatchSize": int,
         "BatchWindow": int,
     },
     total=False,
@@ -4251,19 +4464,21 @@
     "_OptionalStopSessionRequestRequestTypeDef",
     {
         "RequestOrigin": str,
     },
     total=False,
 )
 
+
 class StopSessionRequestRequestTypeDef(
     _RequiredStopSessionRequestRequestTypeDef, _OptionalStopSessionRequestRequestTypeDef
 ):
     pass
 
+
 StopTriggerRequestRequestTypeDef = TypedDict(
     "StopTriggerRequestRequestTypeDef",
     {
         "Name": str,
     },
 )
 
@@ -4313,19 +4528,21 @@
     "_OptionalUpdateBlueprintRequestRequestTypeDef",
     {
         "Description": str,
     },
     total=False,
 )
 
+
 class UpdateBlueprintRequestRequestTypeDef(
     _RequiredUpdateBlueprintRequestRequestTypeDef, _OptionalUpdateBlueprintRequestRequestTypeDef
 ):
     pass
 
+
 _RequiredUpdateCsvClassifierRequestTypeDef = TypedDict(
     "_RequiredUpdateCsvClassifierRequestTypeDef",
     {
         "Name": str,
     },
 )
 _OptionalUpdateCsvClassifierRequestTypeDef = TypedDict(
@@ -4339,19 +4556,21 @@
         "AllowSingleColumn": bool,
         "CustomDatatypeConfigured": bool,
         "CustomDatatypes": Sequence[str],
     },
     total=False,
 )
 
+
 class UpdateCsvClassifierRequestTypeDef(
     _RequiredUpdateCsvClassifierRequestTypeDef, _OptionalUpdateCsvClassifierRequestTypeDef
 ):
     pass
 
+
 _RequiredUpdateGrokClassifierRequestTypeDef = TypedDict(
     "_RequiredUpdateGrokClassifierRequestTypeDef",
     {
         "Name": str,
     },
 )
 _OptionalUpdateGrokClassifierRequestTypeDef = TypedDict(
@@ -4360,38 +4579,42 @@
         "Classification": str,
         "GrokPattern": str,
         "CustomPatterns": str,
     },
     total=False,
 )
 
+
 class UpdateGrokClassifierRequestTypeDef(
     _RequiredUpdateGrokClassifierRequestTypeDef, _OptionalUpdateGrokClassifierRequestTypeDef
 ):
     pass
 
+
 _RequiredUpdateJsonClassifierRequestTypeDef = TypedDict(
     "_RequiredUpdateJsonClassifierRequestTypeDef",
     {
         "Name": str,
     },
 )
 _OptionalUpdateJsonClassifierRequestTypeDef = TypedDict(
     "_OptionalUpdateJsonClassifierRequestTypeDef",
     {
         "JsonPath": str,
     },
     total=False,
 )
 
+
 class UpdateJsonClassifierRequestTypeDef(
     _RequiredUpdateJsonClassifierRequestTypeDef, _OptionalUpdateJsonClassifierRequestTypeDef
 ):
     pass
 
+
 _RequiredUpdateXMLClassifierRequestTypeDef = TypedDict(
     "_RequiredUpdateXMLClassifierRequestTypeDef",
     {
         "Name": str,
     },
 )
 _OptionalUpdateXMLClassifierRequestTypeDef = TypedDict(
@@ -4399,39 +4622,43 @@
     {
         "Classification": str,
         "RowTag": str,
     },
     total=False,
 )
 
+
 class UpdateXMLClassifierRequestTypeDef(
     _RequiredUpdateXMLClassifierRequestTypeDef, _OptionalUpdateXMLClassifierRequestTypeDef
 ):
     pass
 
+
 _RequiredUpdateCrawlerScheduleRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateCrawlerScheduleRequestRequestTypeDef",
     {
         "CrawlerName": str,
     },
 )
 _OptionalUpdateCrawlerScheduleRequestRequestTypeDef = TypedDict(
     "_OptionalUpdateCrawlerScheduleRequestRequestTypeDef",
     {
         "Schedule": str,
     },
     total=False,
 )
 
+
 class UpdateCrawlerScheduleRequestRequestTypeDef(
     _RequiredUpdateCrawlerScheduleRequestRequestTypeDef,
     _OptionalUpdateCrawlerScheduleRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredUpdateDataQualityRulesetRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateDataQualityRulesetRequestRequestTypeDef",
     {
         "Name": str,
     },
 )
 _OptionalUpdateDataQualityRulesetRequestRequestTypeDef = TypedDict(
@@ -4439,20 +4666,22 @@
     {
         "Description": str,
         "Ruleset": str,
     },
     total=False,
 )
 
+
 class UpdateDataQualityRulesetRequestRequestTypeDef(
     _RequiredUpdateDataQualityRulesetRequestRequestTypeDef,
     _OptionalUpdateDataQualityRulesetRequestRequestTypeDef,
 ):
     pass
 
+
 UpdateJobFromSourceControlRequestRequestTypeDef = TypedDict(
     "UpdateJobFromSourceControlRequestRequestTypeDef",
     {
         "JobName": str,
         "Provider": SourceControlProviderType,
         "RepositoryName": str,
         "RepositoryOwner": str,
@@ -4493,19 +4722,21 @@
         "Description": str,
         "DefaultRunProperties": Mapping[str, str],
         "MaxConcurrentRuns": int,
     },
     total=False,
 )
 
+
 class UpdateWorkflowRequestRequestTypeDef(
     _RequiredUpdateWorkflowRequestRequestTypeDef, _OptionalUpdateWorkflowRequestRequestTypeDef
 ):
     pass
 
+
 WorkflowRunStatisticsTypeDef = TypedDict(
     "WorkflowRunStatisticsTypeDef",
     {
         "TotalActions": int,
         "TimeoutActions": int,
         "FailedActions": int,
         "StoppedActions": int,
@@ -4549,19 +4780,21 @@
         "WorkerType": WorkerTypeType,
         "NumberOfWorkers": int,
         "ExecutionClass": ExecutionClassType,
     },
     total=False,
 )
 
+
 class StartJobRunRequestRequestTypeDef(
     _RequiredStartJobRunRequestRequestTypeDef, _OptionalStartJobRunRequestRequestTypeDef
 ):
     pass
 
+
 AggregateTypeDef = TypedDict(
     "AggregateTypeDef",
     {
         "Name": str,
         "Inputs": List[str],
         "Groups": List[List[str]],
         "Aggs": List[AggregateOperationTypeDef],
@@ -4597,14 +4830,42 @@
         "TableSchema": List[OptionTypeDef],
         "StagingTable": str,
         "SelectedColumns": List[OptionTypeDef],
     },
     total=False,
 )
 
+SnowflakeNodeDataTypeDef = TypedDict(
+    "SnowflakeNodeDataTypeDef",
+    {
+        "SourceType": str,
+        "Connection": OptionTypeDef,
+        "Schema": str,
+        "Table": str,
+        "Database": str,
+        "TempDir": str,
+        "IamRole": OptionTypeDef,
+        "AdditionalOptions": Dict[str, str],
+        "SampleQuery": str,
+        "PreAction": str,
+        "PostAction": str,
+        "Action": str,
+        "Upsert": bool,
+        "MergeAction": str,
+        "MergeWhenMatched": str,
+        "MergeWhenNotMatched": str,
+        "MergeClause": str,
+        "StagingTable": str,
+        "SelectedColumns": List[OptionTypeDef],
+        "AutoPushdown": bool,
+        "TableSchema": List[OptionTypeDef],
+    },
+    total=False,
+)
+
 _RequiredGetUnfilteredPartitionMetadataRequestRequestTypeDef = TypedDict(
     "_RequiredGetUnfilteredPartitionMetadataRequestRequestTypeDef",
     {
         "CatalogId": str,
         "DatabaseName": str,
         "TableName": str,
         "PartitionValues": Sequence[str],
@@ -4615,20 +4876,22 @@
     "_OptionalGetUnfilteredPartitionMetadataRequestRequestTypeDef",
     {
         "AuditContext": AuditContextTypeDef,
     },
     total=False,
 )
 
+
 class GetUnfilteredPartitionMetadataRequestRequestTypeDef(
     _RequiredGetUnfilteredPartitionMetadataRequestRequestTypeDef,
     _OptionalGetUnfilteredPartitionMetadataRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredGetUnfilteredTableMetadataRequestRequestTypeDef = TypedDict(
     "_RequiredGetUnfilteredTableMetadataRequestRequestTypeDef",
     {
         "CatalogId": str,
         "DatabaseName": str,
         "Name": str,
         "SupportedPermissionTypes": Sequence[PermissionTypeType],
@@ -4638,20 +4901,22 @@
     "_OptionalGetUnfilteredTableMetadataRequestRequestTypeDef",
     {
         "AuditContext": AuditContextTypeDef,
     },
     total=False,
 )
 
+
 class GetUnfilteredTableMetadataRequestRequestTypeDef(
     _RequiredGetUnfilteredTableMetadataRequestRequestTypeDef,
     _OptionalGetUnfilteredTableMetadataRequestRequestTypeDef,
 ):
     pass
 
+
 BackfillErrorTypeDef = TypedDict(
     "BackfillErrorTypeDef",
     {
         "Code": BackfillErrorCodeType,
         "Partitions": List[PartitionValueListTypeDef],
     },
     total=False,
@@ -4669,20 +4934,22 @@
     "_OptionalBatchDeletePartitionRequestRequestTypeDef",
     {
         "CatalogId": str,
     },
     total=False,
 )
 
+
 class BatchDeletePartitionRequestRequestTypeDef(
     _RequiredBatchDeletePartitionRequestRequestTypeDef,
     _OptionalBatchDeletePartitionRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredBatchGetPartitionRequestRequestTypeDef = TypedDict(
     "_RequiredBatchGetPartitionRequestRequestTypeDef",
     {
         "DatabaseName": str,
         "TableName": str,
         "PartitionsToGet": Sequence[PartitionValueListTypeDef],
     },
@@ -4691,19 +4958,21 @@
     "_OptionalBatchGetPartitionRequestRequestTypeDef",
     {
         "CatalogId": str,
     },
     total=False,
 )
 
+
 class BatchGetPartitionRequestRequestTypeDef(
     _RequiredBatchGetPartitionRequestRequestTypeDef, _OptionalBatchGetPartitionRequestRequestTypeDef
 ):
     pass
 
+
 CancelMLTaskRunResponseTypeDef = TypedDict(
     "CancelMLTaskRunResponseTypeDef",
     {
         "TransformId": str,
         "TaskRunId": str,
         "Status": TaskStatusTypeType,
         "ResponseMetadata": ResponseMetadataTypeDef,
@@ -5507,19 +5776,21 @@
         "DetectSchema": bool,
         "StreamingOptions": KafkaStreamingSourceOptionsTypeDef,
         "DataPreviewOptions": StreamingDataPreviewOptionsTypeDef,
     },
     total=False,
 )
 
+
 class CatalogKafkaSourceTypeDef(
     _RequiredCatalogKafkaSourceTypeDef, _OptionalCatalogKafkaSourceTypeDef
 ):
     pass
 
+
 _RequiredDirectKafkaSourceTypeDef = TypedDict(
     "_RequiredDirectKafkaSourceTypeDef",
     {
         "Name": str,
     },
 )
 _OptionalDirectKafkaSourceTypeDef = TypedDict(
@@ -5529,19 +5800,21 @@
         "WindowSize": int,
         "DetectSchema": bool,
         "DataPreviewOptions": StreamingDataPreviewOptionsTypeDef,
     },
     total=False,
 )
 
+
 class DirectKafkaSourceTypeDef(
     _RequiredDirectKafkaSourceTypeDef, _OptionalDirectKafkaSourceTypeDef
 ):
     pass
 
+
 _RequiredCatalogKinesisSourceTypeDef = TypedDict(
     "_RequiredCatalogKinesisSourceTypeDef",
     {
         "Name": str,
         "Table": str,
         "Database": str,
     },
@@ -5553,19 +5826,21 @@
         "DetectSchema": bool,
         "StreamingOptions": KinesisStreamingSourceOptionsTypeDef,
         "DataPreviewOptions": StreamingDataPreviewOptionsTypeDef,
     },
     total=False,
 )
 
+
 class CatalogKinesisSourceTypeDef(
     _RequiredCatalogKinesisSourceTypeDef, _OptionalCatalogKinesisSourceTypeDef
 ):
     pass
 
+
 _RequiredDirectKinesisSourceTypeDef = TypedDict(
     "_RequiredDirectKinesisSourceTypeDef",
     {
         "Name": str,
     },
 )
 _OptionalDirectKinesisSourceTypeDef = TypedDict(
@@ -5575,19 +5850,21 @@
         "DetectSchema": bool,
         "StreamingOptions": KinesisStreamingSourceOptionsTypeDef,
         "DataPreviewOptions": StreamingDataPreviewOptionsTypeDef,
     },
     total=False,
 )
 
+
 class DirectKinesisSourceTypeDef(
     _RequiredDirectKinesisSourceTypeDef, _OptionalDirectKinesisSourceTypeDef
 ):
     pass
 
+
 _RequiredGovernedCatalogTargetTypeDef = TypedDict(
     "_RequiredGovernedCatalogTargetTypeDef",
     {
         "Name": str,
         "Inputs": List[str],
         "Table": str,
         "Database": str,
@@ -5598,19 +5875,21 @@
     {
         "PartitionKeys": List[List[str]],
         "SchemaChangePolicy": CatalogSchemaChangePolicyTypeDef,
     },
     total=False,
 )
 
+
 class GovernedCatalogTargetTypeDef(
     _RequiredGovernedCatalogTargetTypeDef, _OptionalGovernedCatalogTargetTypeDef
 ):
     pass
 
+
 _RequiredS3CatalogTargetTypeDef = TypedDict(
     "_RequiredS3CatalogTargetTypeDef",
     {
         "Name": str,
         "Inputs": List[str],
         "Table": str,
         "Database": str,
@@ -5621,17 +5900,19 @@
     {
         "PartitionKeys": List[List[str]],
         "SchemaChangePolicy": CatalogSchemaChangePolicyTypeDef,
     },
     total=False,
 )
 
+
 class S3CatalogTargetTypeDef(_RequiredS3CatalogTargetTypeDef, _OptionalS3CatalogTargetTypeDef):
     pass
 
+
 _RequiredS3DeltaCatalogTargetTypeDef = TypedDict(
     "_RequiredS3DeltaCatalogTargetTypeDef",
     {
         "Name": str,
         "Inputs": List[str],
         "Table": str,
         "Database": str,
@@ -5643,19 +5924,21 @@
         "PartitionKeys": List[List[str]],
         "AdditionalOptions": Dict[str, str],
         "SchemaChangePolicy": CatalogSchemaChangePolicyTypeDef,
     },
     total=False,
 )
 
+
 class S3DeltaCatalogTargetTypeDef(
     _RequiredS3DeltaCatalogTargetTypeDef, _OptionalS3DeltaCatalogTargetTypeDef
 ):
     pass
 
+
 _RequiredS3HudiCatalogTargetTypeDef = TypedDict(
     "_RequiredS3HudiCatalogTargetTypeDef",
     {
         "Name": str,
         "Inputs": List[str],
         "Table": str,
         "Database": str,
@@ -5667,19 +5950,21 @@
     {
         "PartitionKeys": List[List[str]],
         "SchemaChangePolicy": CatalogSchemaChangePolicyTypeDef,
     },
     total=False,
 )
 
+
 class S3HudiCatalogTargetTypeDef(
     _RequiredS3HudiCatalogTargetTypeDef, _OptionalS3HudiCatalogTargetTypeDef
 ):
     pass
 
+
 ClassifierTypeDef = TypedDict(
     "ClassifierTypeDef",
     {
         "GrokClassifier": GrokClassifierTypeDef,
         "XMLClassifier": XMLClassifierTypeDef,
         "JsonClassifier": JsonClassifierTypeDef,
         "CsvClassifier": CsvClassifierTypeDef,
@@ -5699,17 +5984,19 @@
     "_OptionalCodeGenNodeTypeDef",
     {
         "LineNumber": int,
     },
     total=False,
 )
 
+
 class CodeGenNodeTypeDef(_RequiredCodeGenNodeTypeDef, _OptionalCodeGenNodeTypeDef):
     pass
 
+
 LocationTypeDef = TypedDict(
     "LocationTypeDef",
     {
         "Jdbc": Sequence[CodeGenNodeArgTypeDef],
         "S3": Sequence[CodeGenNodeArgTypeDef],
         "DynamoDB": Sequence[CodeGenNodeArgTypeDef],
     },
@@ -5752,17 +6039,19 @@
         "Description": str,
         "MatchCriteria": Sequence[str],
         "PhysicalConnectionRequirements": PhysicalConnectionRequirementsTypeDef,
     },
     total=False,
 )
 
+
 class ConnectionInputTypeDef(_RequiredConnectionInputTypeDef, _OptionalConnectionInputTypeDef):
     pass
 
+
 ConnectionTypeDef = TypedDict(
     "ConnectionTypeDef",
     {
         "Name": str,
         "Description": str,
         "ConnectionType": ConnectionTypeType,
         "MatchCriteria": List[str],
@@ -5806,14 +6095,16 @@
     {
         "S3Targets": List[S3TargetTypeDef],
         "JdbcTargets": List[JdbcTargetTypeDef],
         "MongoDBTargets": List[MongoDBTargetTypeDef],
         "DynamoDBTargets": List[DynamoDBTargetTypeDef],
         "CatalogTargets": List[CatalogTargetTypeDef],
         "DeltaTargets": List[DeltaTargetTypeDef],
+        "IcebergTargets": List[IcebergTargetTypeDef],
+        "HudiTargets": List[HudiTargetTypeDef],
     },
     total=False,
 )
 
 _RequiredListCrawlsRequestRequestTypeDef = TypedDict(
     "_RequiredListCrawlsRequestRequestTypeDef",
     {
@@ -5826,19 +6117,21 @@
         "MaxResults": int,
         "Filters": Sequence[CrawlsFilterTypeDef],
         "NextToken": str,
     },
     total=False,
 )
 
+
 class ListCrawlsRequestRequestTypeDef(
     _RequiredListCrawlsRequestRequestTypeDef, _OptionalListCrawlsRequestRequestTypeDef
 ):
     pass
 
+
 CreateClassifierRequestRequestTypeDef = TypedDict(
     "CreateClassifierRequestRequestTypeDef",
     {
         "GrokClassifier": CreateGrokClassifierRequestTypeDef,
         "XMLClassifier": CreateXMLClassifierRequestTypeDef,
         "JsonClassifier": CreateJsonClassifierRequestTypeDef,
         "CsvClassifier": CreateCsvClassifierRequestTypeDef,
@@ -5860,20 +6153,22 @@
         "Tags": Mapping[str, str],
         "TargetTable": DataQualityTargetTableTypeDef,
         "ClientToken": str,
     },
     total=False,
 )
 
+
 class CreateDataQualityRulesetRequestRequestTypeDef(
     _RequiredCreateDataQualityRulesetRequestRequestTypeDef,
     _OptionalCreateDataQualityRulesetRequestRequestTypeDef,
 ):
     pass
 
+
 DataQualityRulesetListDetailsTypeDef = TypedDict(
     "DataQualityRulesetListDetailsTypeDef",
     {
         "Name": str,
         "Description": str,
         "CreatedOn": datetime,
         "LastModifiedOn": datetime,
@@ -5917,20 +6212,22 @@
     "_OptionalCreatePartitionIndexRequestRequestTypeDef",
     {
         "CatalogId": str,
     },
     total=False,
 )
 
+
 class CreatePartitionIndexRequestRequestTypeDef(
     _RequiredCreatePartitionIndexRequestRequestTypeDef,
     _OptionalCreatePartitionIndexRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredCreateSchemaInputRequestTypeDef = TypedDict(
     "_RequiredCreateSchemaInputRequestTypeDef",
     {
         "SchemaName": str,
         "DataFormat": DataFormatType,
     },
 )
@@ -5942,19 +6239,21 @@
         "Description": str,
         "Tags": Mapping[str, str],
         "SchemaDefinition": str,
     },
     total=False,
 )
 
+
 class CreateSchemaInputRequestTypeDef(
     _RequiredCreateSchemaInputRequestTypeDef, _OptionalCreateSchemaInputRequestTypeDef
 ):
     pass
 
+
 DeleteRegistryInputRequestTypeDef = TypedDict(
     "DeleteRegistryInputRequestTypeDef",
     {
         "RegistryId": RegistryIdTypeDef,
     },
 )
 
@@ -6006,19 +6305,21 @@
         "GlueVersion": str,
         "Tags": Mapping[str, str],
         "RequestOrigin": str,
     },
     total=False,
 )
 
+
 class CreateSessionRequestRequestTypeDef(
     _RequiredCreateSessionRequestRequestTypeDef, _OptionalCreateSessionRequestRequestTypeDef
 ):
     pass
 
+
 SessionTypeDef = TypedDict(
     "SessionTypeDef",
     {
         "Id": str,
         "CreatedOn": datetime,
         "Status": SessionStatusType,
         "ErrorMessage": str,
@@ -6050,19 +6351,21 @@
         "PublishingOptions": DQResultsPublishingOptionsTypeDef,
         "AdditionalOptions": Dict[Literal["performanceTuning.caching"], str],
         "StopJobOnFailureOptions": DQStopJobOnFailureOptionsTypeDef,
     },
     total=False,
 )
 
+
 class EvaluateDataQualityMultiFrameTypeDef(
     _RequiredEvaluateDataQualityMultiFrameTypeDef, _OptionalEvaluateDataQualityMultiFrameTypeDef
 ):
     pass
 
+
 _RequiredEvaluateDataQualityTypeDef = TypedDict(
     "_RequiredEvaluateDataQualityTypeDef",
     {
         "Name": str,
         "Inputs": List[str],
         "Ruleset": str,
     },
@@ -6073,19 +6376,21 @@
         "Output": DQTransformOutputType,
         "PublishingOptions": DQResultsPublishingOptionsTypeDef,
         "StopJobOnFailureOptions": DQStopJobOnFailureOptionsTypeDef,
     },
     total=False,
 )
 
+
 class EvaluateDataQualityTypeDef(
     _RequiredEvaluateDataQualityTypeDef, _OptionalEvaluateDataQualityTypeDef
 ):
     pass
 
+
 DataCatalogEncryptionSettingsTypeDef = TypedDict(
     "DataCatalogEncryptionSettingsTypeDef",
     {
         "EncryptionAtRest": EncryptionAtRestTypeDef,
         "ConnectionPasswordEncryption": ConnectionPasswordEncryptionTypeDef,
     },
     total=False,
@@ -6127,19 +6432,21 @@
         "CatalogId": str,
         "TransactionId": str,
         "QueryAsOfTime": TimestampTypeDef,
     },
     total=False,
 )
 
+
 class GetTableRequestRequestTypeDef(
     _RequiredGetTableRequestRequestTypeDef, _OptionalGetTableRequestRequestTypeDef
 ):
     pass
 
+
 _RequiredGetTablesRequestRequestTypeDef = TypedDict(
     "_RequiredGetTablesRequestRequestTypeDef",
     {
         "DatabaseName": str,
     },
 )
 _OptionalGetTablesRequestRequestTypeDef = TypedDict(
@@ -6151,19 +6458,21 @@
         "MaxResults": int,
         "TransactionId": str,
         "QueryAsOfTime": TimestampTypeDef,
     },
     total=False,
 )
 
+
 class GetTablesRequestRequestTypeDef(
     _RequiredGetTablesRequestRequestTypeDef, _OptionalGetTablesRequestRequestTypeDef
 ):
     pass
 
+
 TaskRunFilterCriteriaTypeDef = TypedDict(
     "TaskRunFilterCriteriaTypeDef",
     {
         "TaskRunType": TaskTypeType,
         "Status": TaskStatusTypeType,
         "StartedBefore": TimestampTypeDef,
         "StartedAfter": TimestampTypeDef,
@@ -6191,19 +6500,21 @@
     {
         "MinimumValue": DecimalNumberTypeDef,
         "MaximumValue": DecimalNumberTypeDef,
     },
     total=False,
 )
 
+
 class DecimalColumnStatisticsDataTypeDef(
     _RequiredDecimalColumnStatisticsDataTypeDef, _OptionalDecimalColumnStatisticsDataTypeDef
 ):
     pass
 
+
 DeleteSchemaInputRequestTypeDef = TypedDict(
     "DeleteSchemaInputRequestTypeDef",
     {
         "SchemaId": SchemaIdTypeDef,
     },
 )
 
@@ -6241,19 +6552,21 @@
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
+
 class ListSchemaVersionsInputRequestTypeDef(
     _RequiredListSchemaVersionsInputRequestTypeDef, _OptionalListSchemaVersionsInputRequestTypeDef
 ):
     pass
 
+
 RegisterSchemaVersionInputRequestTypeDef = TypedDict(
     "RegisterSchemaVersionInputRequestTypeDef",
     {
         "SchemaId": SchemaIdTypeDef,
         "SchemaDefinition": str,
     },
 )
@@ -6284,19 +6597,21 @@
         "UpdateEtlLibraries": bool,
         "DeleteArguments": Sequence[str],
         "AddArguments": Mapping[str, str],
     },
     total=False,
 )
 
+
 class UpdateDevEndpointRequestRequestTypeDef(
     _RequiredUpdateDevEndpointRequestRequestTypeDef, _OptionalUpdateDevEndpointRequestRequestTypeDef
 ):
     pass
 
+
 _RequiredS3DeltaDirectTargetTypeDef = TypedDict(
     "_RequiredS3DeltaDirectTargetTypeDef",
     {
         "Name": str,
         "Inputs": List[str],
         "Path": str,
         "Compression": DeltaTargetCompressionTypeType,
@@ -6309,19 +6624,21 @@
         "PartitionKeys": List[List[str]],
         "AdditionalOptions": Dict[str, str],
         "SchemaChangePolicy": DirectSchemaChangePolicyTypeDef,
     },
     total=False,
 )
 
+
 class S3DeltaDirectTargetTypeDef(
     _RequiredS3DeltaDirectTargetTypeDef, _OptionalS3DeltaDirectTargetTypeDef
 ):
     pass
 
+
 _RequiredS3DirectTargetTypeDef = TypedDict(
     "_RequiredS3DirectTargetTypeDef",
     {
         "Name": str,
         "Inputs": List[str],
         "Path": str,
         "Format": TargetFormatType,
@@ -6333,17 +6650,19 @@
         "PartitionKeys": List[List[str]],
         "Compression": str,
         "SchemaChangePolicy": DirectSchemaChangePolicyTypeDef,
     },
     total=False,
 )
 
+
 class S3DirectTargetTypeDef(_RequiredS3DirectTargetTypeDef, _OptionalS3DirectTargetTypeDef):
     pass
 
+
 _RequiredS3GlueParquetTargetTypeDef = TypedDict(
     "_RequiredS3GlueParquetTargetTypeDef",
     {
         "Name": str,
         "Inputs": List[str],
         "Path": str,
     },
@@ -6354,19 +6673,21 @@
         "PartitionKeys": List[List[str]],
         "Compression": ParquetCompressionTypeType,
         "SchemaChangePolicy": DirectSchemaChangePolicyTypeDef,
     },
     total=False,
 )
 
+
 class S3GlueParquetTargetTypeDef(
     _RequiredS3GlueParquetTargetTypeDef, _OptionalS3GlueParquetTargetTypeDef
 ):
     pass
 
+
 _RequiredS3HudiDirectTargetTypeDef = TypedDict(
     "_RequiredS3HudiDirectTargetTypeDef",
     {
         "Name": str,
         "Inputs": List[str],
         "Path": str,
         "Compression": HudiTargetCompressionTypeType,
@@ -6379,19 +6700,21 @@
     {
         "PartitionKeys": List[List[str]],
         "SchemaChangePolicy": DirectSchemaChangePolicyTypeDef,
     },
     total=False,
 )
 
+
 class S3HudiDirectTargetTypeDef(
     _RequiredS3HudiDirectTargetTypeDef, _OptionalS3HudiDirectTargetTypeDef
 ):
     pass
 
+
 EncryptionConfigurationTypeDef = TypedDict(
     "EncryptionConfigurationTypeDef",
     {
         "S3Encryption": Sequence[S3EncryptionTypeDef],
         "CloudWatchEncryption": CloudWatchEncryptionTypeDef,
         "JobBookmarksEncryption": JobBookmarksEncryptionTypeDef,
     },
@@ -6418,36 +6741,40 @@
     "_OptionalFilterExpressionTypeDef",
     {
         "Negated": bool,
     },
     total=False,
 )
 
+
 class FilterExpressionTypeDef(_RequiredFilterExpressionTypeDef, _OptionalFilterExpressionTypeDef):
     pass
 
+
 _RequiredTransformParametersTypeDef = TypedDict(
     "_RequiredTransformParametersTypeDef",
     {
         "TransformType": Literal["FIND_MATCHES"],
     },
 )
 _OptionalTransformParametersTypeDef = TypedDict(
     "_OptionalTransformParametersTypeDef",
     {
         "FindMatchesParameters": FindMatchesParametersTypeDef,
     },
     total=False,
 )
 
+
 class TransformParametersTypeDef(
     _RequiredTransformParametersTypeDef, _OptionalTransformParametersTypeDef
 ):
     pass
 
+
 GetClassifiersRequestGetClassifiersPaginateTypeDef = TypedDict(
     "GetClassifiersRequestGetClassifiersPaginateTypeDef",
     {
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
@@ -6497,20 +6824,22 @@
     "_OptionalGetJobRunsRequestGetJobRunsPaginateTypeDef",
     {
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
+
 class GetJobRunsRequestGetJobRunsPaginateTypeDef(
     _RequiredGetJobRunsRequestGetJobRunsPaginateTypeDef,
     _OptionalGetJobRunsRequestGetJobRunsPaginateTypeDef,
 ):
     pass
 
+
 GetJobsRequestGetJobsPaginateTypeDef = TypedDict(
     "GetJobsRequestGetJobsPaginateTypeDef",
     {
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
@@ -6527,20 +6856,22 @@
     {
         "CatalogId": str,
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
+
 class GetPartitionIndexesRequestGetPartitionIndexesPaginateTypeDef(
     _RequiredGetPartitionIndexesRequestGetPartitionIndexesPaginateTypeDef,
     _OptionalGetPartitionIndexesRequestGetPartitionIndexesPaginateTypeDef,
 ):
     pass
 
+
 GetResourcePoliciesRequestGetResourcePoliciesPaginateTypeDef = TypedDict(
     "GetResourcePoliciesRequestGetResourcePoliciesPaginateTypeDef",
     {
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
@@ -6565,20 +6896,22 @@
     {
         "CatalogId": str,
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
+
 class GetTableVersionsRequestGetTableVersionsPaginateTypeDef(
     _RequiredGetTableVersionsRequestGetTableVersionsPaginateTypeDef,
     _OptionalGetTableVersionsRequestGetTableVersionsPaginateTypeDef,
 ):
     pass
 
+
 _RequiredGetTablesRequestGetTablesPaginateTypeDef = TypedDict(
     "_RequiredGetTablesRequestGetTablesPaginateTypeDef",
     {
         "DatabaseName": str,
     },
 )
 _OptionalGetTablesRequestGetTablesPaginateTypeDef = TypedDict(
@@ -6589,20 +6922,22 @@
         "TransactionId": str,
         "QueryAsOfTime": TimestampTypeDef,
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
+
 class GetTablesRequestGetTablesPaginateTypeDef(
     _RequiredGetTablesRequestGetTablesPaginateTypeDef,
     _OptionalGetTablesRequestGetTablesPaginateTypeDef,
 ):
     pass
 
+
 GetTriggersRequestGetTriggersPaginateTypeDef = TypedDict(
     "GetTriggersRequestGetTriggersPaginateTypeDef",
     {
         "DependentJobName": str,
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
@@ -6620,20 +6955,22 @@
         "CatalogId": str,
         "DatabaseName": str,
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
+
 class GetUserDefinedFunctionsRequestGetUserDefinedFunctionsPaginateTypeDef(
     _RequiredGetUserDefinedFunctionsRequestGetUserDefinedFunctionsPaginateTypeDef,
     _OptionalGetUserDefinedFunctionsRequestGetUserDefinedFunctionsPaginateTypeDef,
 ):
     pass
 
+
 ListRegistriesInputListRegistriesPaginateTypeDef = TypedDict(
     "ListRegistriesInputListRegistriesPaginateTypeDef",
     {
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
@@ -6648,20 +6985,22 @@
     "_OptionalListSchemaVersionsInputListSchemaVersionsPaginateTypeDef",
     {
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
+
 class ListSchemaVersionsInputListSchemaVersionsPaginateTypeDef(
     _RequiredListSchemaVersionsInputListSchemaVersionsPaginateTypeDef,
     _OptionalListSchemaVersionsInputListSchemaVersionsPaginateTypeDef,
 ):
     pass
 
+
 ListSchemasInputListSchemasPaginateTypeDef = TypedDict(
     "ListSchemasInputListSchemasPaginateTypeDef",
     {
         "RegistryId": RegistryIdTypeDef,
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
@@ -6747,20 +7086,22 @@
         "TransactionId": str,
         "QueryAsOfTime": TimestampTypeDef,
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
+
 class GetPartitionsRequestGetPartitionsPaginateTypeDef(
     _RequiredGetPartitionsRequestGetPartitionsPaginateTypeDef,
     _OptionalGetPartitionsRequestGetPartitionsPaginateTypeDef,
 ):
     pass
 
+
 _RequiredGetPartitionsRequestRequestTypeDef = TypedDict(
     "_RequiredGetPartitionsRequestRequestTypeDef",
     {
         "DatabaseName": str,
         "TableName": str,
     },
 )
@@ -6775,19 +7116,21 @@
         "ExcludeColumnSchema": bool,
         "TransactionId": str,
         "QueryAsOfTime": TimestampTypeDef,
     },
     total=False,
 )
 
+
 class GetPartitionsRequestRequestTypeDef(
     _RequiredGetPartitionsRequestRequestTypeDef, _OptionalGetPartitionsRequestRequestTypeDef
 ):
     pass
 
+
 _RequiredGetUnfilteredPartitionsMetadataRequestRequestTypeDef = TypedDict(
     "_RequiredGetUnfilteredPartitionsMetadataRequestRequestTypeDef",
     {
         "CatalogId": str,
         "DatabaseName": str,
         "TableName": str,
         "SupportedPermissionTypes": Sequence[PermissionTypeType],
@@ -6801,20 +7144,22 @@
         "NextToken": str,
         "Segment": SegmentTypeDef,
         "MaxResults": int,
     },
     total=False,
 )
 
+
 class GetUnfilteredPartitionsMetadataRequestRequestTypeDef(
     _RequiredGetUnfilteredPartitionsMetadataRequestRequestTypeDef,
     _OptionalGetUnfilteredPartitionsMetadataRequestRequestTypeDef,
 ):
     pass
 
+
 GetResourcePoliciesResponseTypeDef = TypedDict(
     "GetResourcePoliciesResponseTypeDef",
     {
         "GetResourcePoliciesResponseList": List[GluePolicyTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -6852,19 +7197,21 @@
         "SchemaVersionNumber": SchemaVersionNumberTypeDef,
         "Compatibility": CompatibilityType,
         "Description": str,
     },
     total=False,
 )
 
+
 class UpdateSchemaInputRequestTypeDef(
     _RequiredUpdateSchemaInputRequestTypeDef, _OptionalUpdateSchemaInputRequestTypeDef
 ):
     pass
 
+
 GlueSchemaTypeDef = TypedDict(
     "GlueSchemaTypeDef",
     {
         "Columns": List[GlueStudioSchemaColumnTypeDef],
     },
     total=False,
 )
@@ -6882,19 +7229,21 @@
     {
         "PartitionPredicate": str,
         "AdditionalOptions": S3SourceAdditionalOptionsTypeDef,
     },
     total=False,
 )
 
+
 class GovernedCatalogSourceTypeDef(
     _RequiredGovernedCatalogSourceTypeDef, _OptionalGovernedCatalogSourceTypeDef
 ):
     pass
 
+
 _RequiredS3CatalogSourceTypeDef = TypedDict(
     "_RequiredS3CatalogSourceTypeDef",
     {
         "Name": str,
         "Database": str,
         "Table": str,
     },
@@ -6904,17 +7253,27 @@
     {
         "PartitionPredicate": str,
         "AdditionalOptions": S3SourceAdditionalOptionsTypeDef,
     },
     total=False,
 )
 
+
 class S3CatalogSourceTypeDef(_RequiredS3CatalogSourceTypeDef, _OptionalS3CatalogSourceTypeDef):
     pass
 
+
+OpenTableFormatInputTypeDef = TypedDict(
+    "OpenTableFormatInputTypeDef",
+    {
+        "IcebergInput": IcebergInputTypeDef,
+    },
+    total=False,
+)
+
 JobRunTypeDef = TypedDict(
     "JobRunTypeDef",
     {
         "Id": str,
         "Attempt": int,
         "PreviousRunId": str,
         "TriggerName": str,
@@ -7022,20 +7381,22 @@
         "SchemaId": SchemaIdTypeDef,
         "SchemaVersionNumber": SchemaVersionNumberTypeDef,
         "SchemaVersionId": str,
     },
     total=False,
 )
 
+
 class PutSchemaVersionMetadataInputRequestTypeDef(
     _RequiredPutSchemaVersionMetadataInputRequestTypeDef,
     _OptionalPutSchemaVersionMetadataInputRequestTypeDef,
 ):
     pass
 
+
 QuerySchemaVersionMetadataInputRequestTypeDef = TypedDict(
     "QuerySchemaVersionMetadataInputRequestTypeDef",
     {
         "SchemaId": SchemaIdTypeDef,
         "SchemaVersionNumber": SchemaVersionNumberTypeDef,
         "SchemaVersionId": str,
         "MetadataList": Sequence[MetadataKeyValuePairTypeDef],
@@ -7057,20 +7418,31 @@
         "SchemaId": SchemaIdTypeDef,
         "SchemaVersionNumber": SchemaVersionNumberTypeDef,
         "SchemaVersionId": str,
     },
     total=False,
 )
 
+
 class RemoveSchemaVersionMetadataInputRequestTypeDef(
     _RequiredRemoveSchemaVersionMetadataInputRequestTypeDef,
     _OptionalRemoveSchemaVersionMetadataInputRequestTypeDef,
 ):
     pass
 
+
+RecipeTypeDef = TypedDict(
+    "RecipeTypeDef",
+    {
+        "Name": str,
+        "Inputs": List[str],
+        "RecipeReference": RecipeReferenceTypeDef,
+    },
+)
+
 _RequiredRedshiftTargetTypeDef = TypedDict(
     "_RequiredRedshiftTargetTypeDef",
     {
         "Name": str,
         "Inputs": List[str],
         "Database": str,
         "Table": str,
@@ -7082,17 +7454,19 @@
         "RedshiftTmpDir": str,
         "TmpDirIAMRole": str,
         "UpsertRedshiftOptions": UpsertRedshiftTargetOptionsTypeDef,
     },
     total=False,
 )
 
+
 class RedshiftTargetTypeDef(_RequiredRedshiftTargetTypeDef, _OptionalRedshiftTargetTypeDef):
     pass
 
+
 UserDefinedFunctionInputTypeDef = TypedDict(
     "UserDefinedFunctionInputTypeDef",
     {
         "FunctionName": str,
         "ClassName": str,
         "OwnerName": str,
         "OwnerType": PrincipalTypeType,
@@ -7169,14 +7543,34 @@
         "Name": str,
         "Data": AmazonRedshiftNodeDataTypeDef,
         "Inputs": List[str],
     },
     total=False,
 )
 
+_RequiredSnowflakeTargetTypeDef = TypedDict(
+    "_RequiredSnowflakeTargetTypeDef",
+    {
+        "Name": str,
+        "Data": SnowflakeNodeDataTypeDef,
+    },
+)
+_OptionalSnowflakeTargetTypeDef = TypedDict(
+    "_OptionalSnowflakeTargetTypeDef",
+    {
+        "Inputs": List[str],
+    },
+    total=False,
+)
+
+
+class SnowflakeTargetTypeDef(_RequiredSnowflakeTargetTypeDef, _OptionalSnowflakeTargetTypeDef):
+    pass
+
+
 _RequiredPartitionIndexDescriptorTypeDef = TypedDict(
     "_RequiredPartitionIndexDescriptorTypeDef",
     {
         "IndexName": str,
         "Keys": List[KeySchemaElementTypeDef],
         "IndexStatus": PartitionIndexStatusType,
     },
@@ -7185,19 +7579,21 @@
     "_OptionalPartitionIndexDescriptorTypeDef",
     {
         "BackfillErrors": List[BackfillErrorTypeDef],
     },
     total=False,
 )
 
+
 class PartitionIndexDescriptorTypeDef(
     _RequiredPartitionIndexDescriptorTypeDef, _OptionalPartitionIndexDescriptorTypeDef
 ):
     pass
 
+
 BatchStopJobRunResponseTypeDef = TypedDict(
     "BatchStopJobRunResponseTypeDef",
     {
         "SuccessfulSubmissions": List[BatchStopJobRunSuccessfulSubmissionTypeDef],
         "Errors": List[BatchStopJobRunErrorTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -7307,19 +7703,21 @@
     {
         "Sinks": Sequence[CatalogEntryTypeDef],
         "Location": LocationTypeDef,
     },
     total=False,
 )
 
+
 class GetMappingRequestRequestTypeDef(
     _RequiredGetMappingRequestRequestTypeDef, _OptionalGetMappingRequestRequestTypeDef
 ):
     pass
 
+
 _RequiredGetPlanRequestRequestTypeDef = TypedDict(
     "_RequiredGetPlanRequestRequestTypeDef",
     {
         "Mapping": Sequence[MappingEntryTypeDef],
         "Source": CatalogEntryTypeDef,
     },
 )
@@ -7330,19 +7728,21 @@
         "Location": LocationTypeDef,
         "Language": LanguageType,
         "AdditionalPlanOptionsMap": Mapping[str, str],
     },
     total=False,
 )
 
+
 class GetPlanRequestRequestTypeDef(
     _RequiredGetPlanRequestRequestTypeDef, _OptionalGetPlanRequestRequestTypeDef
 ):
     pass
 
+
 _RequiredCreateTriggerRequestRequestTypeDef = TypedDict(
     "_RequiredCreateTriggerRequestRequestTypeDef",
     {
         "Name": str,
         "Type": TriggerTypeType,
         "Actions": Sequence[ActionTypeDef],
     },
@@ -7357,19 +7757,21 @@
         "StartOnCreation": bool,
         "Tags": Mapping[str, str],
         "EventBatchingCondition": EventBatchingConditionTypeDef,
     },
     total=False,
 )
 
+
 class CreateTriggerRequestRequestTypeDef(
     _RequiredCreateTriggerRequestRequestTypeDef, _OptionalCreateTriggerRequestRequestTypeDef
 ):
     pass
 
+
 TriggerTypeDef = TypedDict(
     "TriggerTypeDef",
     {
         "Name": str,
         "WorkflowName": str,
         "Id": str,
         "Type": TriggerTypeType,
@@ -7406,19 +7808,21 @@
     "_OptionalEvaluationMetricsTypeDef",
     {
         "FindMatchesMetrics": FindMatchesMetricsTypeDef,
     },
     total=False,
 )
 
+
 class EvaluationMetricsTypeDef(
     _RequiredEvaluationMetricsTypeDef, _OptionalEvaluationMetricsTypeDef
 ):
     pass
 
+
 _RequiredCreateConnectionRequestRequestTypeDef = TypedDict(
     "_RequiredCreateConnectionRequestRequestTypeDef",
     {
         "ConnectionInput": ConnectionInputTypeDef,
     },
 )
 _OptionalCreateConnectionRequestRequestTypeDef = TypedDict(
@@ -7426,19 +7830,21 @@
     {
         "CatalogId": str,
         "Tags": Mapping[str, str],
     },
     total=False,
 )
 
+
 class CreateConnectionRequestRequestTypeDef(
     _RequiredCreateConnectionRequestRequestTypeDef, _OptionalCreateConnectionRequestRequestTypeDef
 ):
     pass
 
+
 _RequiredUpdateConnectionRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateConnectionRequestRequestTypeDef",
     {
         "Name": str,
         "ConnectionInput": ConnectionInputTypeDef,
     },
 )
@@ -7446,19 +7852,21 @@
     "_OptionalUpdateConnectionRequestRequestTypeDef",
     {
         "CatalogId": str,
     },
     total=False,
 )
 
+
 class UpdateConnectionRequestRequestTypeDef(
     _RequiredUpdateConnectionRequestRequestTypeDef, _OptionalUpdateConnectionRequestRequestTypeDef
 ):
     pass
 
+
 GetConnectionResponseTypeDef = TypedDict(
     "GetConnectionResponseTypeDef",
     {
         "Connection": ConnectionTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -7522,19 +7930,21 @@
         "Configuration": str,
         "CrawlerSecurityConfiguration": str,
         "Tags": Mapping[str, str],
     },
     total=False,
 )
 
+
 class CreateCrawlerRequestRequestTypeDef(
     _RequiredCreateCrawlerRequestRequestTypeDef, _OptionalCreateCrawlerRequestRequestTypeDef
 ):
     pass
 
+
 _RequiredUpdateCrawlerRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateCrawlerRequestRequestTypeDef",
     {
         "Name": str,
     },
 )
 _OptionalUpdateCrawlerRequestRequestTypeDef = TypedDict(
@@ -7553,19 +7963,21 @@
         "LakeFormationConfiguration": LakeFormationConfigurationTypeDef,
         "Configuration": str,
         "CrawlerSecurityConfiguration": str,
     },
     total=False,
 )
 
+
 class UpdateCrawlerRequestRequestTypeDef(
     _RequiredUpdateCrawlerRequestRequestTypeDef, _OptionalUpdateCrawlerRequestRequestTypeDef
 ):
     pass
 
+
 ListDataQualityRulesetsResponseTypeDef = TypedDict(
     "ListDataQualityRulesetsResponseTypeDef",
     {
         "Rulesets": List[DataQualityRulesetListDetailsTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -7635,20 +8047,22 @@
     {
         "StartedBefore": TimestampTypeDef,
         "StartedAfter": TimestampTypeDef,
     },
     total=False,
 )
 
+
 class DataQualityRuleRecommendationRunFilterTypeDef(
     _RequiredDataQualityRuleRecommendationRunFilterTypeDef,
     _OptionalDataQualityRuleRecommendationRunFilterTypeDef,
 ):
     pass
 
+
 DataQualityRulesetEvaluationRunDescriptionTypeDef = TypedDict(
     "DataQualityRulesetEvaluationRunDescriptionTypeDef",
     {
         "RunId": str,
         "Status": TaskStatusTypeType,
         "StartedOn": datetime,
         "DataSource": DataSourceTypeDef,
@@ -7667,20 +8081,22 @@
     {
         "StartedBefore": TimestampTypeDef,
         "StartedAfter": TimestampTypeDef,
     },
     total=False,
 )
 
+
 class DataQualityRulesetEvaluationRunFilterTypeDef(
     _RequiredDataQualityRulesetEvaluationRunFilterTypeDef,
     _OptionalDataQualityRulesetEvaluationRunFilterTypeDef,
 ):
     pass
 
+
 GetDataQualityResultResponseTypeDef = TypedDict(
     "GetDataQualityResultResponseTypeDef",
     {
         "ResultId": str,
         "Score": float,
         "DataSource": DataSourceTypeDef,
         "RulesetName": str,
@@ -7751,20 +8167,22 @@
         "Timeout": int,
         "CreatedRulesetName": str,
         "ClientToken": str,
     },
     total=False,
 )
 
+
 class StartDataQualityRuleRecommendationRunRequestRequestTypeDef(
     _RequiredStartDataQualityRuleRecommendationRunRequestRequestTypeDef,
     _OptionalStartDataQualityRuleRecommendationRunRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredStartDataQualityRulesetEvaluationRunRequestRequestTypeDef = TypedDict(
     "_RequiredStartDataQualityRulesetEvaluationRunRequestRequestTypeDef",
     {
         "DataSource": DataSourceTypeDef,
         "Role": str,
         "RulesetNames": Sequence[str],
     },
@@ -7777,20 +8195,22 @@
         "ClientToken": str,
         "AdditionalRunOptions": DataQualityEvaluationRunAdditionalRunOptionsTypeDef,
         "AdditionalDataSources": Mapping[str, DataSourceTypeDef],
     },
     total=False,
 )
 
+
 class StartDataQualityRulesetEvaluationRunRequestRequestTypeDef(
     _RequiredStartDataQualityRulesetEvaluationRunRequestRequestTypeDef,
     _OptionalStartDataQualityRulesetEvaluationRunRequestRequestTypeDef,
 ):
     pass
 
+
 CreateSessionResponseTypeDef = TypedDict(
     "CreateSessionResponseTypeDef",
     {
         "Session": SessionTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -7831,20 +8251,22 @@
     "_OptionalPutDataCatalogEncryptionSettingsRequestRequestTypeDef",
     {
         "CatalogId": str,
     },
     total=False,
 )
 
+
 class PutDataCatalogEncryptionSettingsRequestRequestTypeDef(
     _RequiredPutDataCatalogEncryptionSettingsRequestRequestTypeDef,
     _OptionalPutDataCatalogEncryptionSettingsRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredDatabaseInputTypeDef = TypedDict(
     "_RequiredDatabaseInputTypeDef",
     {
         "Name": str,
     },
 )
 _OptionalDatabaseInputTypeDef = TypedDict(
@@ -7856,17 +8278,19 @@
         "CreateTableDefaultPermissions": Sequence[PrincipalPermissionsTypeDef],
         "TargetDatabase": DatabaseIdentifierTypeDef,
         "FederatedDatabase": FederatedDatabaseTypeDef,
     },
     total=False,
 )
 
+
 class DatabaseInputTypeDef(_RequiredDatabaseInputTypeDef, _OptionalDatabaseInputTypeDef):
     pass
 
+
 _RequiredDatabaseTypeDef = TypedDict(
     "_RequiredDatabaseTypeDef",
     {
         "Name": str,
     },
 )
 _OptionalDatabaseTypeDef = TypedDict(
@@ -7880,17 +8304,19 @@
         "TargetDatabase": DatabaseIdentifierTypeDef,
         "CatalogId": str,
         "FederatedDatabase": FederatedDatabaseTypeDef,
     },
     total=False,
 )
 
+
 class DatabaseTypeDef(_RequiredDatabaseTypeDef, _OptionalDatabaseTypeDef):
     pass
 
+
 ListDataQualityRulesetsRequestRequestTypeDef = TypedDict(
     "ListDataQualityRulesetsRequestRequestTypeDef",
     {
         "NextToken": str,
         "MaxResults": int,
         "Filter": DataQualityRulesetFilterCriteriaTypeDef,
         "Tags": Mapping[str, str],
@@ -7911,19 +8337,21 @@
         "MaxResults": int,
         "Filter": TaskRunFilterCriteriaTypeDef,
         "Sort": TaskRunSortCriteriaTypeDef,
     },
     total=False,
 )
 
+
 class GetMLTaskRunsRequestRequestTypeDef(
     _RequiredGetMLTaskRunsRequestRequestTypeDef, _OptionalGetMLTaskRunsRequestRequestTypeDef
 ):
     pass
 
+
 _RequiredDropNullFieldsTypeDef = TypedDict(
     "_RequiredDropNullFieldsTypeDef",
     {
         "Name": str,
         "Inputs": List[str],
     },
 )
@@ -7932,17 +8360,19 @@
     {
         "NullCheckBoxList": NullCheckBoxListTypeDef,
         "NullTextList": List[NullValueFieldTypeDef],
     },
     total=False,
 )
 
+
 class DropNullFieldsTypeDef(_RequiredDropNullFieldsTypeDef, _OptionalDropNullFieldsTypeDef):
     pass
 
+
 _RequiredColumnStatisticsDataTypeDef = TypedDict(
     "_RequiredColumnStatisticsDataTypeDef",
     {
         "Type": ColumnStatisticsTypeType,
     },
 )
 _OptionalColumnStatisticsDataTypeDef = TypedDict(
@@ -7955,19 +8385,21 @@
         "LongColumnStatisticsData": LongColumnStatisticsDataTypeDef,
         "StringColumnStatisticsData": StringColumnStatisticsDataTypeDef,
         "BinaryColumnStatisticsData": BinaryColumnStatisticsDataTypeDef,
     },
     total=False,
 )
 
+
 class ColumnStatisticsDataTypeDef(
     _RequiredColumnStatisticsDataTypeDef, _OptionalColumnStatisticsDataTypeDef
 ):
     pass
 
+
 StorageDescriptorTypeDef = TypedDict(
     "StorageDescriptorTypeDef",
     {
         "Columns": Sequence[ColumnTypeDef],
         "Location": str,
         "AdditionalLocations": Sequence[str],
         "InputFormat": str,
@@ -8040,19 +8472,21 @@
         "NumberOfWorkers": int,
         "Timeout": int,
         "MaxRetries": int,
     },
     total=False,
 )
 
+
 class UpdateMLTransformRequestRequestTypeDef(
     _RequiredUpdateMLTransformRequestRequestTypeDef, _OptionalUpdateMLTransformRequestRequestTypeDef
 ):
     pass
 
+
 GetMLTransformsRequestRequestTypeDef = TypedDict(
     "GetMLTransformsRequestRequestTypeDef",
     {
         "NextToken": str,
         "MaxResults": int,
         "Filter": TransformFilterCriteriaTypeDef,
         "Sort": TransformSortCriteriaTypeDef,
@@ -8087,19 +8521,21 @@
     {
         "ConnectionTable": str,
         "OutputSchemas": List[GlueSchemaTypeDef],
     },
     total=False,
 )
 
+
 class AthenaConnectorSourceTypeDef(
     _RequiredAthenaConnectorSourceTypeDef, _OptionalAthenaConnectorSourceTypeDef
 ):
     pass
 
+
 _RequiredCatalogDeltaSourceTypeDef = TypedDict(
     "_RequiredCatalogDeltaSourceTypeDef",
     {
         "Name": str,
         "Database": str,
         "Table": str,
     },
@@ -8109,19 +8545,21 @@
     {
         "AdditionalDeltaOptions": Dict[str, str],
         "OutputSchemas": List[GlueSchemaTypeDef],
     },
     total=False,
 )
 
+
 class CatalogDeltaSourceTypeDef(
     _RequiredCatalogDeltaSourceTypeDef, _OptionalCatalogDeltaSourceTypeDef
 ):
     pass
 
+
 _RequiredCatalogHudiSourceTypeDef = TypedDict(
     "_RequiredCatalogHudiSourceTypeDef",
     {
         "Name": str,
         "Database": str,
         "Table": str,
     },
@@ -8131,19 +8569,21 @@
     {
         "AdditionalHudiOptions": Dict[str, str],
         "OutputSchemas": List[GlueSchemaTypeDef],
     },
     total=False,
 )
 
+
 class CatalogHudiSourceTypeDef(
     _RequiredCatalogHudiSourceTypeDef, _OptionalCatalogHudiSourceTypeDef
 ):
     pass
 
+
 _RequiredCustomCodeTypeDef = TypedDict(
     "_RequiredCustomCodeTypeDef",
     {
         "Name": str,
         "Inputs": List[str],
         "Code": str,
         "ClassName": str,
@@ -8153,17 +8593,19 @@
     "_OptionalCustomCodeTypeDef",
     {
         "OutputSchemas": List[GlueSchemaTypeDef],
     },
     total=False,
 )
 
+
 class CustomCodeTypeDef(_RequiredCustomCodeTypeDef, _OptionalCustomCodeTypeDef):
     pass
 
+
 _RequiredDynamicTransformTypeDef = TypedDict(
     "_RequiredDynamicTransformTypeDef",
     {
         "Name": str,
         "TransformName": str,
         "Inputs": List[str],
         "FunctionName": str,
@@ -8176,17 +8618,19 @@
         "Parameters": List[TransformConfigParameterTypeDef],
         "Version": str,
         "OutputSchemas": List[GlueSchemaTypeDef],
     },
     total=False,
 )
 
+
 class DynamicTransformTypeDef(_RequiredDynamicTransformTypeDef, _OptionalDynamicTransformTypeDef):
     pass
 
+
 _RequiredJDBCConnectorSourceTypeDef = TypedDict(
     "_RequiredJDBCConnectorSourceTypeDef",
     {
         "Name": str,
         "ConnectionName": str,
         "ConnectorName": str,
         "ConnectionType": str,
@@ -8199,19 +8643,21 @@
         "ConnectionTable": str,
         "Query": str,
         "OutputSchemas": List[GlueSchemaTypeDef],
     },
     total=False,
 )
 
+
 class JDBCConnectorSourceTypeDef(
     _RequiredJDBCConnectorSourceTypeDef, _OptionalJDBCConnectorSourceTypeDef
 ):
     pass
 
+
 _RequiredJDBCConnectorTargetTypeDef = TypedDict(
     "_RequiredJDBCConnectorTargetTypeDef",
     {
         "Name": str,
         "Inputs": List[str],
         "ConnectionName": str,
         "ConnectionTable": str,
@@ -8224,19 +8670,21 @@
     {
         "AdditionalOptions": Dict[str, str],
         "OutputSchemas": List[GlueSchemaTypeDef],
     },
     total=False,
 )
 
+
 class JDBCConnectorTargetTypeDef(
     _RequiredJDBCConnectorTargetTypeDef, _OptionalJDBCConnectorTargetTypeDef
 ):
     pass
 
+
 _RequiredS3CatalogDeltaSourceTypeDef = TypedDict(
     "_RequiredS3CatalogDeltaSourceTypeDef",
     {
         "Name": str,
         "Database": str,
         "Table": str,
     },
@@ -8246,19 +8694,21 @@
     {
         "AdditionalDeltaOptions": Dict[str, str],
         "OutputSchemas": List[GlueSchemaTypeDef],
     },
     total=False,
 )
 
+
 class S3CatalogDeltaSourceTypeDef(
     _RequiredS3CatalogDeltaSourceTypeDef, _OptionalS3CatalogDeltaSourceTypeDef
 ):
     pass
 
+
 _RequiredS3CatalogHudiSourceTypeDef = TypedDict(
     "_RequiredS3CatalogHudiSourceTypeDef",
     {
         "Name": str,
         "Database": str,
         "Table": str,
     },
@@ -8268,19 +8718,21 @@
     {
         "AdditionalHudiOptions": Dict[str, str],
         "OutputSchemas": List[GlueSchemaTypeDef],
     },
     total=False,
 )
 
+
 class S3CatalogHudiSourceTypeDef(
     _RequiredS3CatalogHudiSourceTypeDef, _OptionalS3CatalogHudiSourceTypeDef
 ):
     pass
 
+
 _RequiredS3CsvSourceTypeDef = TypedDict(
     "_RequiredS3CsvSourceTypeDef",
     {
         "Name": str,
         "Paths": List[str],
         "Separator": SeparatorType,
         "QuoteChar": QuoteCharType,
@@ -8304,17 +8756,19 @@
         "SkipFirst": bool,
         "OptimizePerformance": bool,
         "OutputSchemas": List[GlueSchemaTypeDef],
     },
     total=False,
 )
 
+
 class S3CsvSourceTypeDef(_RequiredS3CsvSourceTypeDef, _OptionalS3CsvSourceTypeDef):
     pass
 
+
 _RequiredS3DeltaSourceTypeDef = TypedDict(
     "_RequiredS3DeltaSourceTypeDef",
     {
         "Name": str,
         "Paths": List[str],
     },
 )
@@ -8324,17 +8778,19 @@
         "AdditionalDeltaOptions": Dict[str, str],
         "AdditionalOptions": S3DirectSourceAdditionalOptionsTypeDef,
         "OutputSchemas": List[GlueSchemaTypeDef],
     },
     total=False,
 )
 
+
 class S3DeltaSourceTypeDef(_RequiredS3DeltaSourceTypeDef, _OptionalS3DeltaSourceTypeDef):
     pass
 
+
 _RequiredS3HudiSourceTypeDef = TypedDict(
     "_RequiredS3HudiSourceTypeDef",
     {
         "Name": str,
         "Paths": List[str],
     },
 )
@@ -8344,17 +8800,19 @@
         "AdditionalHudiOptions": Dict[str, str],
         "AdditionalOptions": S3DirectSourceAdditionalOptionsTypeDef,
         "OutputSchemas": List[GlueSchemaTypeDef],
     },
     total=False,
 )
 
+
 class S3HudiSourceTypeDef(_RequiredS3HudiSourceTypeDef, _OptionalS3HudiSourceTypeDef):
     pass
 
+
 _RequiredS3JsonSourceTypeDef = TypedDict(
     "_RequiredS3JsonSourceTypeDef",
     {
         "Name": str,
         "Paths": List[str],
     },
 )
@@ -8372,17 +8830,19 @@
         "JsonPath": str,
         "Multiline": bool,
         "OutputSchemas": List[GlueSchemaTypeDef],
     },
     total=False,
 )
 
+
 class S3JsonSourceTypeDef(_RequiredS3JsonSourceTypeDef, _OptionalS3JsonSourceTypeDef):
     pass
 
+
 _RequiredS3ParquetSourceTypeDef = TypedDict(
     "_RequiredS3ParquetSourceTypeDef",
     {
         "Name": str,
         "Paths": List[str],
     },
 )
@@ -8398,17 +8858,39 @@
         "MaxFilesInBand": int,
         "AdditionalOptions": S3DirectSourceAdditionalOptionsTypeDef,
         "OutputSchemas": List[GlueSchemaTypeDef],
     },
     total=False,
 )
 
+
 class S3ParquetSourceTypeDef(_RequiredS3ParquetSourceTypeDef, _OptionalS3ParquetSourceTypeDef):
     pass
 
+
+_RequiredSnowflakeSourceTypeDef = TypedDict(
+    "_RequiredSnowflakeSourceTypeDef",
+    {
+        "Name": str,
+        "Data": SnowflakeNodeDataTypeDef,
+    },
+)
+_OptionalSnowflakeSourceTypeDef = TypedDict(
+    "_OptionalSnowflakeSourceTypeDef",
+    {
+        "OutputSchemas": List[GlueSchemaTypeDef],
+    },
+    total=False,
+)
+
+
+class SnowflakeSourceTypeDef(_RequiredSnowflakeSourceTypeDef, _OptionalSnowflakeSourceTypeDef):
+    pass
+
+
 _RequiredSparkConnectorSourceTypeDef = TypedDict(
     "_RequiredSparkConnectorSourceTypeDef",
     {
         "Name": str,
         "ConnectionName": str,
         "ConnectorName": str,
         "ConnectionType": str,
@@ -8419,19 +8901,21 @@
     {
         "AdditionalOptions": Dict[str, str],
         "OutputSchemas": List[GlueSchemaTypeDef],
     },
     total=False,
 )
 
+
 class SparkConnectorSourceTypeDef(
     _RequiredSparkConnectorSourceTypeDef, _OptionalSparkConnectorSourceTypeDef
 ):
     pass
 
+
 _RequiredSparkConnectorTargetTypeDef = TypedDict(
     "_RequiredSparkConnectorTargetTypeDef",
     {
         "Name": str,
         "Inputs": List[str],
         "ConnectionName": str,
         "ConnectorName": str,
@@ -8443,19 +8927,21 @@
     {
         "AdditionalOptions": Dict[str, str],
         "OutputSchemas": List[GlueSchemaTypeDef],
     },
     total=False,
 )
 
+
 class SparkConnectorTargetTypeDef(
     _RequiredSparkConnectorTargetTypeDef, _OptionalSparkConnectorTargetTypeDef
 ):
     pass
 
+
 _RequiredSparkSQLTypeDef = TypedDict(
     "_RequiredSparkSQLTypeDef",
     {
         "Name": str,
         "Inputs": List[str],
         "SqlQuery": str,
         "SqlAliases": List[SqlAliasTypeDef],
@@ -8465,17 +8951,19 @@
     "_OptionalSparkSQLTypeDef",
     {
         "OutputSchemas": List[GlueSchemaTypeDef],
     },
     total=False,
 )
 
+
 class SparkSQLTypeDef(_RequiredSparkSQLTypeDef, _OptionalSparkSQLTypeDef):
     pass
 
+
 GetJobRunResponseTypeDef = TypedDict(
     "GetJobRunResponseTypeDef",
     {
         "JobRun": JobRunTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -8552,19 +9040,21 @@
         "MaxRetries": int,
         "Tags": Mapping[str, str],
         "TransformEncryption": TransformEncryptionTypeDef,
     },
     total=False,
 )
 
+
 class CreateMLTransformRequestRequestTypeDef(
     _RequiredCreateMLTransformRequestRequestTypeDef, _OptionalCreateMLTransformRequestRequestTypeDef
 ):
     pass
 
+
 QuerySchemaVersionMetadataResponseTypeDef = TypedDict(
     "QuerySchemaVersionMetadataResponseTypeDef",
     {
         "MetadataInfoMap": Dict[str, MetadataInfoTypeDef],
         "SchemaVersionId": str,
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
@@ -8582,20 +9072,22 @@
     "_OptionalCreateUserDefinedFunctionRequestRequestTypeDef",
     {
         "CatalogId": str,
     },
     total=False,
 )
 
+
 class CreateUserDefinedFunctionRequestRequestTypeDef(
     _RequiredCreateUserDefinedFunctionRequestRequestTypeDef,
     _OptionalCreateUserDefinedFunctionRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredUpdateUserDefinedFunctionRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateUserDefinedFunctionRequestRequestTypeDef",
     {
         "DatabaseName": str,
         "FunctionName": str,
         "FunctionInput": UserDefinedFunctionInputTypeDef,
     },
@@ -8604,20 +9096,22 @@
     "_OptionalUpdateUserDefinedFunctionRequestRequestTypeDef",
     {
         "CatalogId": str,
     },
     total=False,
 )
 
+
 class UpdateUserDefinedFunctionRequestRequestTypeDef(
     _RequiredUpdateUserDefinedFunctionRequestRequestTypeDef,
     _OptionalUpdateUserDefinedFunctionRequestRequestTypeDef,
 ):
     pass
 
+
 GetUserDefinedFunctionResponseTypeDef = TypedDict(
     "GetUserDefinedFunctionResponseTypeDef",
     {
         "UserDefinedFunction": UserDefinedFunctionTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -8859,19 +9353,21 @@
     {
         "CatalogId": str,
         "Tags": Mapping[str, str],
     },
     total=False,
 )
 
+
 class CreateDatabaseRequestRequestTypeDef(
     _RequiredCreateDatabaseRequestRequestTypeDef, _OptionalCreateDatabaseRequestRequestTypeDef
 ):
     pass
 
+
 _RequiredUpdateDatabaseRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateDatabaseRequestRequestTypeDef",
     {
         "Name": str,
         "DatabaseInput": DatabaseInputTypeDef,
     },
 )
@@ -8879,19 +9375,21 @@
     "_OptionalUpdateDatabaseRequestRequestTypeDef",
     {
         "CatalogId": str,
     },
     total=False,
 )
 
+
 class UpdateDatabaseRequestRequestTypeDef(
     _RequiredUpdateDatabaseRequestRequestTypeDef, _OptionalUpdateDatabaseRequestRequestTypeDef
 ):
     pass
 
+
 GetDatabaseResponseTypeDef = TypedDict(
     "GetDatabaseResponseTypeDef",
     {
         "Database": DatabaseTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -8964,17 +9462,19 @@
         "TableType": str,
         "Parameters": Mapping[str, str],
         "TargetTable": TableIdentifierTypeDef,
     },
     total=False,
 )
 
+
 class TableInputTypeDef(_RequiredTableInputTypeDef, _OptionalTableInputTypeDef):
     pass
 
+
 _RequiredTableTypeDef = TypedDict(
     "_RequiredTableTypeDef",
     {
         "Name": str,
     },
 )
 _OptionalTableTypeDef = TypedDict(
@@ -9000,17 +9500,19 @@
         "CatalogId": str,
         "VersionId": str,
         "FederatedTable": FederatedTableTypeDef,
     },
     total=False,
 )
 
+
 class TableTypeDef(_RequiredTableTypeDef, _OptionalTableTypeDef):
     pass
 
+
 GetSecurityConfigurationResponseTypeDef = TypedDict(
     "GetSecurityConfigurationResponseTypeDef",
     {
         "SecurityConfiguration": SecurityConfigurationTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -9089,14 +9591,17 @@
         "CatalogDeltaSource": CatalogDeltaSourceTypeDef,
         "S3DeltaSource": S3DeltaSourceTypeDef,
         "S3DeltaCatalogTarget": S3DeltaCatalogTargetTypeDef,
         "S3DeltaDirectTarget": S3DeltaDirectTargetTypeDef,
         "AmazonRedshiftSource": AmazonRedshiftSourceTypeDef,
         "AmazonRedshiftTarget": AmazonRedshiftTargetTypeDef,
         "EvaluateDataQualityMultiFrame": EvaluateDataQualityMultiFrameTypeDef,
+        "Recipe": RecipeTypeDef,
+        "SnowflakeSource": SnowflakeSourceTypeDef,
+        "SnowflakeTarget": SnowflakeTargetTypeDef,
     },
     total=False,
 )
 
 GetMLTaskRunsResponseTypeDef = TypedDict(
     "GetMLTaskRunsResponseTypeDef",
     {
@@ -9185,20 +9690,22 @@
     "_OptionalUpdateColumnStatisticsForPartitionRequestRequestTypeDef",
     {
         "CatalogId": str,
     },
     total=False,
 )
 
+
 class UpdateColumnStatisticsForPartitionRequestRequestTypeDef(
     _RequiredUpdateColumnStatisticsForPartitionRequestRequestTypeDef,
     _OptionalUpdateColumnStatisticsForPartitionRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredUpdateColumnStatisticsForTableRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateColumnStatisticsForTableRequestRequestTypeDef",
     {
         "DatabaseName": str,
         "TableName": str,
         "ColumnStatisticsList": Sequence[ColumnStatisticsTypeDef],
     },
@@ -9207,20 +9714,22 @@
     "_OptionalUpdateColumnStatisticsForTableRequestRequestTypeDef",
     {
         "CatalogId": str,
     },
     total=False,
 )
 
+
 class UpdateColumnStatisticsForTableRequestRequestTypeDef(
     _RequiredUpdateColumnStatisticsForTableRequestRequestTypeDef,
     _OptionalUpdateColumnStatisticsForTableRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredBatchCreatePartitionRequestRequestTypeDef = TypedDict(
     "_RequiredBatchCreatePartitionRequestRequestTypeDef",
     {
         "DatabaseName": str,
         "TableName": str,
         "PartitionInputList": Sequence[PartitionInputTypeDef],
     },
@@ -9229,20 +9738,22 @@
     "_OptionalBatchCreatePartitionRequestRequestTypeDef",
     {
         "CatalogId": str,
     },
     total=False,
 )
 
+
 class BatchCreatePartitionRequestRequestTypeDef(
     _RequiredBatchCreatePartitionRequestRequestTypeDef,
     _OptionalBatchCreatePartitionRequestRequestTypeDef,
 ):
     pass
 
+
 BatchUpdatePartitionRequestEntryTypeDef = TypedDict(
     "BatchUpdatePartitionRequestEntryTypeDef",
     {
         "PartitionValueList": Sequence[str],
         "PartitionInput": PartitionInputTypeDef,
     },
 )
@@ -9259,19 +9770,21 @@
     "_OptionalCreatePartitionRequestRequestTypeDef",
     {
         "CatalogId": str,
     },
     total=False,
 )
 
+
 class CreatePartitionRequestRequestTypeDef(
     _RequiredCreatePartitionRequestRequestTypeDef, _OptionalCreatePartitionRequestRequestTypeDef
 ):
     pass
 
+
 _RequiredUpdatePartitionRequestRequestTypeDef = TypedDict(
     "_RequiredUpdatePartitionRequestRequestTypeDef",
     {
         "DatabaseName": str,
         "TableName": str,
         "PartitionValueList": Sequence[str],
         "PartitionInput": PartitionInputTypeDef,
@@ -9281,19 +9794,21 @@
     "_OptionalUpdatePartitionRequestRequestTypeDef",
     {
         "CatalogId": str,
     },
     total=False,
 )
 
+
 class UpdatePartitionRequestRequestTypeDef(
     _RequiredUpdatePartitionRequestRequestTypeDef, _OptionalUpdatePartitionRequestRequestTypeDef
 ):
     pass
 
+
 BatchGetPartitionResponseTypeDef = TypedDict(
     "BatchGetPartitionResponseTypeDef",
     {
         "Partitions": List[PartitionTypeDef],
         "UnprocessedKeys": List[PartitionValueListTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -9345,23 +9860,26 @@
 )
 _OptionalCreateTableRequestRequestTypeDef = TypedDict(
     "_OptionalCreateTableRequestRequestTypeDef",
     {
         "CatalogId": str,
         "PartitionIndexes": Sequence[PartitionIndexTypeDef],
         "TransactionId": str,
+        "OpenTableFormatInput": OpenTableFormatInputTypeDef,
     },
     total=False,
 )
 
+
 class CreateTableRequestRequestTypeDef(
     _RequiredCreateTableRequestRequestTypeDef, _OptionalCreateTableRequestRequestTypeDef
 ):
     pass
 
+
 _RequiredUpdateTableRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateTableRequestRequestTypeDef",
     {
         "DatabaseName": str,
         "TableInput": TableInputTypeDef,
     },
 )
@@ -9372,19 +9890,21 @@
         "SkipArchive": bool,
         "TransactionId": str,
         "VersionId": str,
     },
     total=False,
 )
 
+
 class UpdateTableRequestRequestTypeDef(
     _RequiredUpdateTableRequestRequestTypeDef, _OptionalUpdateTableRequestRequestTypeDef
 ):
     pass
 
+
 GetTableResponseTypeDef = TypedDict(
     "GetTableResponseTypeDef",
     {
         "Table": TableTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -9457,19 +9977,21 @@
         "CodeGenConfigurationNodes": Mapping[str, CodeGenConfigurationNodeTypeDef],
         "ExecutionClass": ExecutionClassType,
         "SourceControlDetails": SourceControlDetailsTypeDef,
     },
     total=False,
 )
 
+
 class CreateJobRequestRequestTypeDef(
     _RequiredCreateJobRequestRequestTypeDef, _OptionalCreateJobRequestRequestTypeDef
 ):
     pass
 
+
 JobTypeDef = TypedDict(
     "JobTypeDef",
     {
         "Name": str,
         "Description": str,
         "LogUri": str,
         "Role": str,
@@ -9560,20 +10082,22 @@
     "_OptionalBatchUpdatePartitionRequestRequestTypeDef",
     {
         "CatalogId": str,
     },
     total=False,
 )
 
+
 class BatchUpdatePartitionRequestRequestTypeDef(
     _RequiredBatchUpdatePartitionRequestRequestTypeDef,
     _OptionalBatchUpdatePartitionRequestRequestTypeDef,
 ):
     pass
 
+
 GetUnfilteredPartitionsMetadataResponseTypeDef = TypedDict(
     "GetUnfilteredPartitionsMetadataResponseTypeDef",
     {
         "UnfilteredPartitions": List[UnfilteredPartitionTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
```

### Comparing `types-aiobotocore-glue-2.5.2.post3/types_aiobotocore_glue.egg-info/PKG-INFO` & `types-aiobotocore-glue-2.5.4/types_aiobotocore_glue.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-glue
-Version: 2.5.2.post3
-Summary: Type annotations for aiobotocore.Glue 2.5.2 service generated with mypy-boto3-builder 7.17.2
+Version: 2.5.4
+Summary: Type annotations for aiobotocore.Glue 2.5.4 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_glue/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-glue.svg?color=blue)](https://pypi.org/project/types-aiobotocore-glue)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_glue/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-glue)](https://pepy.tech/project/types-aiobotocore-glue)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.Glue 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue)
+[aiobotocore.Glue 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-glue-2.5.2.post3/types_aiobotocore_glue.egg-info/SOURCES.txt` & `types-aiobotocore-glue-2.5.4/types_aiobotocore_glue.egg-info/SOURCES.txt`

 * *Files identical despite different names*


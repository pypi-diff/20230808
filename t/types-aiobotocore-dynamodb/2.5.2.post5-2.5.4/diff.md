# Comparing `tmp/types-aiobotocore-dynamodb-2.5.2.post5.tar.gz` & `tmp/types-aiobotocore-dynamodb-2.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-dynamodb-2.5.2.post5.tar", last modified: Fri Aug  4 12:37:37 2023, max compression
+gzip compressed data, was "types-aiobotocore-dynamodb-2.5.4.tar", last modified: Tue Aug  8 01:23:38 2023, max compression
```

## Comparing `types-aiobotocore-dynamodb-2.5.2.post5.tar` & `types-aiobotocore-dynamodb-2.5.4.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:37:37.191658 types-aiobotocore-dynamodb-2.5.2.post5/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-04 12:21:53.000000 types-aiobotocore-dynamodb-2.5.2.post5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    16212 2023-08-04 12:37:37.187658 types-aiobotocore-dynamodb-2.5.2.post5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    14690 2023-08-04 12:21:53.000000 types-aiobotocore-dynamodb-2.5.2.post5/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-04 12:37:37.191658 types-aiobotocore-dynamodb-2.5.2.post5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2079 2023-08-04 12:21:53.000000 types-aiobotocore-dynamodb-2.5.2.post5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:37:37.179658 types-aiobotocore-dynamodb-2.5.2.post5/types_aiobotocore_dynamodb/
--rw-r--r--   0 runner    (1001) docker     (123)     1857 2023-08-04 12:21:53.000000 types-aiobotocore-dynamodb-2.5.2.post5/types_aiobotocore_dynamodb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1855 2023-08-04 12:21:53.000000 types-aiobotocore-dynamodb-2.5.2.post5/types_aiobotocore_dynamodb/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      947 2023-08-04 12:21:53.000000 types-aiobotocore-dynamodb-2.5.2.post5/types_aiobotocore_dynamodb/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    49966 2023-08-04 12:21:53.000000 types-aiobotocore-dynamodb-2.5.2.post5/types_aiobotocore_dynamodb/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    49897 2023-08-04 12:21:53.000000 types-aiobotocore-dynamodb-2.5.2.post5/types_aiobotocore_dynamodb/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    12866 2023-08-04 12:21:54.000000 types-aiobotocore-dynamodb-2.5.2.post5/types_aiobotocore_dynamodb/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    12864 2023-08-04 12:21:54.000000 types-aiobotocore-dynamodb-2.5.2.post5/types_aiobotocore_dynamodb/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     7850 2023-08-04 12:21:54.000000 types-aiobotocore-dynamodb-2.5.2.post5/types_aiobotocore_dynamodb/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     7843 2023-08-04 12:21:54.000000 types-aiobotocore-dynamodb-2.5.2.post5/types_aiobotocore_dynamodb/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 12:21:53.000000 types-aiobotocore-dynamodb-2.5.2.post5/types_aiobotocore_dynamodb/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    24190 2023-08-04 12:21:54.000000 types-aiobotocore-dynamodb-2.5.2.post5/types_aiobotocore_dynamodb/service_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)    24161 2023-08-04 12:21:53.000000 types-aiobotocore-dynamodb-2.5.2.post5/types_aiobotocore_dynamodb/service_resource.pyi
--rw-r--r--   0 runner    (1001) docker     (123)   110199 2023-08-04 12:21:57.000000 types-aiobotocore-dynamodb-2.5.2.post5/types_aiobotocore_dynamodb/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)   110060 2023-08-04 12:21:56.000000 types-aiobotocore-dynamodb-2.5.2.post5/types_aiobotocore_dynamodb/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-04 12:21:53.000000 types-aiobotocore-dynamodb-2.5.2.post5/types_aiobotocore_dynamodb/version.py
--rw-r--r--   0 runner    (1001) docker     (123)     2442 2023-08-04 12:21:54.000000 types-aiobotocore-dynamodb-2.5.2.post5/types_aiobotocore_dynamodb/waiter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2440 2023-08-04 12:21:54.000000 types-aiobotocore-dynamodb-2.5.2.post5/types_aiobotocore_dynamodb/waiter.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:37:37.187658 types-aiobotocore-dynamodb-2.5.2.post5/types_aiobotocore_dynamodb.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    16212 2023-08-04 12:37:36.000000 types-aiobotocore-dynamodb-2.5.2.post5/types_aiobotocore_dynamodb.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1002 2023-08-04 12:37:37.000000 types-aiobotocore-dynamodb-2.5.2.post5/types_aiobotocore_dynamodb.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 12:37:36.000000 types-aiobotocore-dynamodb-2.5.2.post5/types_aiobotocore_dynamodb.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 12:37:36.000000 types-aiobotocore-dynamodb-2.5.2.post5/types_aiobotocore_dynamodb.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-04 12:37:36.000000 types-aiobotocore-dynamodb-2.5.2.post5/types_aiobotocore_dynamodb.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-08-04 12:37:36.000000 types-aiobotocore-dynamodb-2.5.2.post5/types_aiobotocore_dynamodb.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:23:38.450694 types-aiobotocore-dynamodb-2.5.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-08 01:09:27.000000 types-aiobotocore-dynamodb-2.5.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    16206 2023-08-08 01:23:38.446694 types-aiobotocore-dynamodb-2.5.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    14690 2023-08-08 01:09:27.000000 types-aiobotocore-dynamodb-2.5.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-08 01:23:38.450694 types-aiobotocore-dynamodb-2.5.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2073 2023-08-08 01:09:27.000000 types-aiobotocore-dynamodb-2.5.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:23:38.434694 types-aiobotocore-dynamodb-2.5.4/types_aiobotocore_dynamodb/
+-rw-r--r--   0 runner    (1001) docker     (123)     1857 2023-08-08 01:09:27.000000 types-aiobotocore-dynamodb-2.5.4/types_aiobotocore_dynamodb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1855 2023-08-08 01:09:27.000000 types-aiobotocore-dynamodb-2.5.4/types_aiobotocore_dynamodb/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      935 2023-08-08 01:09:27.000000 types-aiobotocore-dynamodb-2.5.4/types_aiobotocore_dynamodb/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    50379 2023-08-08 01:09:27.000000 types-aiobotocore-dynamodb-2.5.4/types_aiobotocore_dynamodb/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    50310 2023-08-08 01:09:27.000000 types-aiobotocore-dynamodb-2.5.4/types_aiobotocore_dynamodb/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    12981 2023-08-08 01:09:28.000000 types-aiobotocore-dynamodb-2.5.4/types_aiobotocore_dynamodb/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12979 2023-08-08 01:09:28.000000 types-aiobotocore-dynamodb-2.5.4/types_aiobotocore_dynamodb/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     7850 2023-08-08 01:09:28.000000 types-aiobotocore-dynamodb-2.5.4/types_aiobotocore_dynamodb/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7843 2023-08-08 01:09:28.000000 types-aiobotocore-dynamodb-2.5.4/types_aiobotocore_dynamodb/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 01:09:27.000000 types-aiobotocore-dynamodb-2.5.4/types_aiobotocore_dynamodb/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    24511 2023-08-08 01:09:28.000000 types-aiobotocore-dynamodb-2.5.4/types_aiobotocore_dynamodb/service_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24482 2023-08-08 01:09:27.000000 types-aiobotocore-dynamodb-2.5.4/types_aiobotocore_dynamodb/service_resource.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)   111041 2023-08-08 01:09:31.000000 types-aiobotocore-dynamodb-2.5.4/types_aiobotocore_dynamodb/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)   110902 2023-08-08 01:09:30.000000 types-aiobotocore-dynamodb-2.5.4/types_aiobotocore_dynamodb/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-08-08 01:09:27.000000 types-aiobotocore-dynamodb-2.5.4/types_aiobotocore_dynamodb/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2442 2023-08-08 01:09:28.000000 types-aiobotocore-dynamodb-2.5.4/types_aiobotocore_dynamodb/waiter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2440 2023-08-08 01:09:28.000000 types-aiobotocore-dynamodb-2.5.4/types_aiobotocore_dynamodb/waiter.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:23:38.446694 types-aiobotocore-dynamodb-2.5.4/types_aiobotocore_dynamodb.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    16206 2023-08-08 01:23:38.000000 types-aiobotocore-dynamodb-2.5.4/types_aiobotocore_dynamodb.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1002 2023-08-08 01:23:38.000000 types-aiobotocore-dynamodb-2.5.4/types_aiobotocore_dynamodb.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 01:23:38.000000 types-aiobotocore-dynamodb-2.5.4/types_aiobotocore_dynamodb.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 01:23:38.000000 types-aiobotocore-dynamodb-2.5.4/types_aiobotocore_dynamodb.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-08 01:23:38.000000 types-aiobotocore-dynamodb-2.5.4/types_aiobotocore_dynamodb.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-08-08 01:23:38.000000 types-aiobotocore-dynamodb-2.5.4/types_aiobotocore_dynamodb.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-dynamodb-2.5.2.post5/LICENSE` & `types-aiobotocore-dynamodb-2.5.4/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-dynamodb-2.5.2.post5/PKG-INFO` & `types-aiobotocore-dynamodb-2.5.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-dynamodb
-Version: 2.5.2.post5
-Summary: Type annotations for aiobotocore.DynamoDB 2.5.2 service generated with mypy-boto3-builder 7.17.2
+Version: 2.5.4
+Summary: Type annotations for aiobotocore.DynamoDB 2.5.4 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dynamodb/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-dynamodb.svg?color=blue)](https://pypi.org/project/types-aiobotocore-dynamodb)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dynamodb/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-dynamodb)](https://pepy.tech/project/types-aiobotocore-dynamodb)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.DynamoDB 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB)
+[aiobotocore.DynamoDB 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-dynamodb-2.5.2.post5/README.md` & `types-aiobotocore-dynamodb-2.5.4/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-dynamodb.svg?color=blue)](https://pypi.org/project/types-aiobotocore-dynamodb)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dynamodb/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-dynamodb)](https://pepy.tech/project/types-aiobotocore-dynamodb)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.DynamoDB 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB)
+[aiobotocore.DynamoDB 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-dynamodb-2.5.2.post5/setup.py` & `types-aiobotocore-dynamodb-2.5.4/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-dynamodb",
-    version="2.5.2.post5",
+    version="2.5.4",
     packages=["types_aiobotocore_dynamodb"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.DynamoDB 2.5.2 service generated with mypy-boto3-builder"
+        "Type annotations for aiobotocore.DynamoDB 2.5.4 service generated with mypy-boto3-builder"
         " 7.17.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
```

### Comparing `types-aiobotocore-dynamodb-2.5.2.post5/types_aiobotocore_dynamodb/__init__.py` & `types-aiobotocore-dynamodb-2.5.4/types_aiobotocore_dynamodb/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-dynamodb-2.5.2.post5/types_aiobotocore_dynamodb/__init__.pyi` & `types-aiobotocore-dynamodb-2.5.4/types_aiobotocore_dynamodb/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-dynamodb-2.5.2.post5/types_aiobotocore_dynamodb/__main__.py` & `types-aiobotocore-dynamodb-2.5.4/types_aiobotocore_dynamodb/__main__.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.DynamoDB 2.5.2\nVersion:         2.5.2.post5\nBuilder"
-        " version: 7.17.2\nDocs:           "
+        "Type annotations for aiobotocore.DynamoDB 2.5.4\nVersion:         2.5.4\nBuilder version:"
+        " 7.17.2\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dynamodb//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB\nOther"
         " services:  https://pypi.org/project/boto3-stubs/\nChangelog:      "
         " https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("2.5.2.post5")
+    print("2.5.4")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `types-aiobotocore-dynamodb-2.5.2.post5/types_aiobotocore_dynamodb/client.py` & `types-aiobotocore-dynamodb-2.5.4/types_aiobotocore_dynamodb/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -26,14 +26,15 @@
     ConditionalOperatorType,
     ContributorInsightsActionType,
     ExportFormatType,
     InputCompressionTypeType,
     InputFormatType,
     ReturnConsumedCapacityType,
     ReturnItemCollectionMetricsType,
+    ReturnValuesOnConditionCheckFailureType,
     ReturnValueType,
     S3SseAlgorithmType,
     SelectType,
     TableClassType,
 )
 from .paginator import (
     ListBackupsPaginator,
@@ -315,15 +316,16 @@
         Expected: Mapping[str, ExpectedAttributeValueTypeDef] = ...,
         ConditionalOperator: ConditionalOperatorType = ...,
         ReturnValues: ReturnValueType = ...,
         ReturnConsumedCapacity: ReturnConsumedCapacityType = ...,
         ReturnItemCollectionMetrics: ReturnItemCollectionMetricsType = ...,
         ConditionExpression: str = ...,
         ExpressionAttributeNames: Mapping[str, str] = ...,
-        ExpressionAttributeValues: Mapping[str, UniversalAttributeValueTypeDef] = ...
+        ExpressionAttributeValues: Mapping[str, UniversalAttributeValueTypeDef] = ...,
+        ReturnValuesOnConditionCheckFailure: ReturnValuesOnConditionCheckFailureType = ...
     ) -> DeleteItemOutputTypeDef:
         """
         Deletes a single item in a table by primary key.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB.Client.delete_item)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dynamodb/client/#delete_item)
         """
@@ -482,15 +484,16 @@
         self,
         *,
         Statement: str,
         Parameters: Sequence[UniversalAttributeValueTypeDef] = ...,
         ConsistentRead: bool = ...,
         NextToken: str = ...,
         ReturnConsumedCapacity: ReturnConsumedCapacityType = ...,
-        Limit: int = ...
+        Limit: int = ...,
+        ReturnValuesOnConditionCheckFailure: ReturnValuesOnConditionCheckFailureType = ...
     ) -> ExecuteStatementOutputTypeDef:
         """
         This operation allows you to perform reads and singleton writes on data stored
         in DynamoDB, using PartiQL.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB.Client.execute_statement)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dynamodb/client/#execute_statement)
@@ -668,15 +671,16 @@
         Expected: Mapping[str, ExpectedAttributeValueTypeDef] = ...,
         ReturnValues: ReturnValueType = ...,
         ReturnConsumedCapacity: ReturnConsumedCapacityType = ...,
         ReturnItemCollectionMetrics: ReturnItemCollectionMetricsType = ...,
         ConditionalOperator: ConditionalOperatorType = ...,
         ConditionExpression: str = ...,
         ExpressionAttributeNames: Mapping[str, str] = ...,
-        ExpressionAttributeValues: Mapping[str, UniversalAttributeValueTypeDef] = ...
+        ExpressionAttributeValues: Mapping[str, UniversalAttributeValueTypeDef] = ...,
+        ReturnValuesOnConditionCheckFailure: ReturnValuesOnConditionCheckFailureType = ...
     ) -> PutItemOutputTypeDef:
         """
         Creates a new item, or replaces an old item with a new item.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB.Client.put_item)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dynamodb/client/#put_item)
         """
@@ -896,15 +900,16 @@
         ConditionalOperator: ConditionalOperatorType = ...,
         ReturnValues: ReturnValueType = ...,
         ReturnConsumedCapacity: ReturnConsumedCapacityType = ...,
         ReturnItemCollectionMetrics: ReturnItemCollectionMetricsType = ...,
         UpdateExpression: str = ...,
         ConditionExpression: str = ...,
         ExpressionAttributeNames: Mapping[str, str] = ...,
-        ExpressionAttributeValues: Mapping[str, UniversalAttributeValueTypeDef] = ...
+        ExpressionAttributeValues: Mapping[str, UniversalAttributeValueTypeDef] = ...,
+        ReturnValuesOnConditionCheckFailure: ReturnValuesOnConditionCheckFailureType = ...
     ) -> UpdateItemOutputTypeDef:
         """
         Edits an existing item's attributes, or adds a new item to the table if it does
         not already exist.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB.Client.update_item)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dynamodb/client/#update_item)
```

### Comparing `types-aiobotocore-dynamodb-2.5.2.post5/types_aiobotocore_dynamodb/client.pyi` & `types-aiobotocore-dynamodb-2.5.4/types_aiobotocore_dynamodb/client.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -26,14 +26,15 @@
     ConditionalOperatorType,
     ContributorInsightsActionType,
     ExportFormatType,
     InputCompressionTypeType,
     InputFormatType,
     ReturnConsumedCapacityType,
     ReturnItemCollectionMetricsType,
+    ReturnValuesOnConditionCheckFailureType,
     ReturnValueType,
     S3SseAlgorithmType,
     SelectType,
     TableClassType,
 )
 from .paginator import (
     ListBackupsPaginator,
@@ -301,15 +302,16 @@
         Expected: Mapping[str, ExpectedAttributeValueTypeDef] = ...,
         ConditionalOperator: ConditionalOperatorType = ...,
         ReturnValues: ReturnValueType = ...,
         ReturnConsumedCapacity: ReturnConsumedCapacityType = ...,
         ReturnItemCollectionMetrics: ReturnItemCollectionMetricsType = ...,
         ConditionExpression: str = ...,
         ExpressionAttributeNames: Mapping[str, str] = ...,
-        ExpressionAttributeValues: Mapping[str, UniversalAttributeValueTypeDef] = ...
+        ExpressionAttributeValues: Mapping[str, UniversalAttributeValueTypeDef] = ...,
+        ReturnValuesOnConditionCheckFailure: ReturnValuesOnConditionCheckFailureType = ...
     ) -> DeleteItemOutputTypeDef:
         """
         Deletes a single item in a table by primary key.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB.Client.delete_item)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dynamodb/client/#delete_item)
         """
@@ -451,15 +453,16 @@
         self,
         *,
         Statement: str,
         Parameters: Sequence[UniversalAttributeValueTypeDef] = ...,
         ConsistentRead: bool = ...,
         NextToken: str = ...,
         ReturnConsumedCapacity: ReturnConsumedCapacityType = ...,
-        Limit: int = ...
+        Limit: int = ...,
+        ReturnValuesOnConditionCheckFailure: ReturnValuesOnConditionCheckFailureType = ...
     ) -> ExecuteStatementOutputTypeDef:
         """
         This operation allows you to perform reads and singleton writes on data stored
         in DynamoDB, using PartiQL.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB.Client.execute_statement)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dynamodb/client/#execute_statement)
@@ -624,15 +627,16 @@
         Expected: Mapping[str, ExpectedAttributeValueTypeDef] = ...,
         ReturnValues: ReturnValueType = ...,
         ReturnConsumedCapacity: ReturnConsumedCapacityType = ...,
         ReturnItemCollectionMetrics: ReturnItemCollectionMetricsType = ...,
         ConditionalOperator: ConditionalOperatorType = ...,
         ConditionExpression: str = ...,
         ExpressionAttributeNames: Mapping[str, str] = ...,
-        ExpressionAttributeValues: Mapping[str, UniversalAttributeValueTypeDef] = ...
+        ExpressionAttributeValues: Mapping[str, UniversalAttributeValueTypeDef] = ...,
+        ReturnValuesOnConditionCheckFailure: ReturnValuesOnConditionCheckFailureType = ...
     ) -> PutItemOutputTypeDef:
         """
         Creates a new item, or replaces an old item with a new item.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB.Client.put_item)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dynamodb/client/#put_item)
         """
@@ -839,15 +843,16 @@
         ConditionalOperator: ConditionalOperatorType = ...,
         ReturnValues: ReturnValueType = ...,
         ReturnConsumedCapacity: ReturnConsumedCapacityType = ...,
         ReturnItemCollectionMetrics: ReturnItemCollectionMetricsType = ...,
         UpdateExpression: str = ...,
         ConditionExpression: str = ...,
         ExpressionAttributeNames: Mapping[str, str] = ...,
-        ExpressionAttributeValues: Mapping[str, UniversalAttributeValueTypeDef] = ...
+        ExpressionAttributeValues: Mapping[str, UniversalAttributeValueTypeDef] = ...,
+        ReturnValuesOnConditionCheckFailure: ReturnValuesOnConditionCheckFailureType = ...
     ) -> UpdateItemOutputTypeDef:
         """
         Edits an existing item's attributes, or adds a new item to the table if it does
         not already exist.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB.Client.update_item)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dynamodb/client/#update_item)
```

### Comparing `types-aiobotocore-dynamodb-2.5.2.post5/types_aiobotocore_dynamodb/literals.py` & `types-aiobotocore-dynamodb-2.5.4/types_aiobotocore_dynamodb/literals.py`

 * *Files 1% similar despite different names*

```diff
@@ -169,14 +169,15 @@
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
@@ -272,14 +273,15 @@
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
@@ -358,26 +360,28 @@
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
@@ -540,14 +544,15 @@
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

### Comparing `types-aiobotocore-dynamodb-2.5.2.post5/types_aiobotocore_dynamodb/literals.pyi` & `types-aiobotocore-dynamodb-2.5.4/types_aiobotocore_dynamodb/literals.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -167,14 +167,15 @@
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
@@ -270,14 +271,15 @@
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
@@ -356,26 +358,28 @@
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
@@ -538,14 +542,15 @@
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

### Comparing `types-aiobotocore-dynamodb-2.5.2.post5/types_aiobotocore_dynamodb/paginator.py` & `types-aiobotocore-dynamodb-2.5.4/types_aiobotocore_dynamodb/paginator.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-dynamodb-2.5.2.post5/types_aiobotocore_dynamodb/paginator.pyi` & `types-aiobotocore-dynamodb-2.5.4/types_aiobotocore_dynamodb/paginator.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-dynamodb-2.5.2.post5/types_aiobotocore_dynamodb/service_resource.py` & `types-aiobotocore-dynamodb-2.5.4/types_aiobotocore_dynamodb/service_resource.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,14 +23,15 @@
 
 from .client import DynamoDBClient
 from .literals import (
     BillingModeType,
     ConditionalOperatorType,
     ReturnConsumedCapacityType,
     ReturnItemCollectionMetricsType,
+    ReturnValuesOnConditionCheckFailureType,
     ReturnValueType,
     SelectType,
     TableClassType,
     TableStatusType,
 )
 from .type_defs import (
     ArchivalSummaryResponseTypeDef,
@@ -216,15 +217,16 @@
         Expected: Mapping[str, ExpectedAttributeValueTableTypeDef] = ...,
         ConditionalOperator: ConditionalOperatorType = ...,
         ReturnValues: ReturnValueType = ...,
         ReturnConsumedCapacity: ReturnConsumedCapacityType = ...,
         ReturnItemCollectionMetrics: ReturnItemCollectionMetricsType = ...,
         ConditionExpression: ConditionBaseImportTypeDef = ...,
         ExpressionAttributeNames: Mapping[str, str] = ...,
-        ExpressionAttributeValues: Mapping[str, TableAttributeValueTypeDef] = ...
+        ExpressionAttributeValues: Mapping[str, TableAttributeValueTypeDef] = ...,
+        ReturnValuesOnConditionCheckFailure: ReturnValuesOnConditionCheckFailureType = ...
     ) -> DeleteItemOutputTableTypeDef:
         """
         Deletes a single item in a table by primary key.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB.Table.delete_item)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dynamodb/service_resource/#tabledelete_item-method)
         """
@@ -271,15 +273,16 @@
         Expected: Mapping[str, ExpectedAttributeValueTableTypeDef] = ...,
         ReturnValues: ReturnValueType = ...,
         ReturnConsumedCapacity: ReturnConsumedCapacityType = ...,
         ReturnItemCollectionMetrics: ReturnItemCollectionMetricsType = ...,
         ConditionalOperator: ConditionalOperatorType = ...,
         ConditionExpression: ConditionBaseImportTypeDef = ...,
         ExpressionAttributeNames: Mapping[str, str] = ...,
-        ExpressionAttributeValues: Mapping[str, TableAttributeValueTypeDef] = ...
+        ExpressionAttributeValues: Mapping[str, TableAttributeValueTypeDef] = ...,
+        ReturnValuesOnConditionCheckFailure: ReturnValuesOnConditionCheckFailureType = ...
     ) -> PutItemOutputTableTypeDef:
         """
         Creates a new item, or replaces an old item with a new item.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB.Table.put_item)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dynamodb/service_resource/#tableput_item-method)
         """
@@ -378,15 +381,16 @@
         ConditionalOperator: ConditionalOperatorType = ...,
         ReturnValues: ReturnValueType = ...,
         ReturnConsumedCapacity: ReturnConsumedCapacityType = ...,
         ReturnItemCollectionMetrics: ReturnItemCollectionMetricsType = ...,
         UpdateExpression: str = ...,
         ConditionExpression: ConditionBaseImportTypeDef = ...,
         ExpressionAttributeNames: Mapping[str, str] = ...,
-        ExpressionAttributeValues: Mapping[str, TableAttributeValueTypeDef] = ...
+        ExpressionAttributeValues: Mapping[str, TableAttributeValueTypeDef] = ...,
+        ReturnValuesOnConditionCheckFailure: ReturnValuesOnConditionCheckFailureType = ...
     ) -> UpdateItemOutputTableTypeDef:
         """
         Edits an existing item's attributes, or adds a new item to the table if it does
         not already exist.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB.Table.update_item)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dynamodb/service_resource/#tableupdate_item-method)
```

### Comparing `types-aiobotocore-dynamodb-2.5.2.post5/types_aiobotocore_dynamodb/service_resource.pyi` & `types-aiobotocore-dynamodb-2.5.4/types_aiobotocore_dynamodb/service_resource.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -23,14 +23,15 @@
 
 from .client import DynamoDBClient
 from .literals import (
     BillingModeType,
     ConditionalOperatorType,
     ReturnConsumedCapacityType,
     ReturnItemCollectionMetricsType,
+    ReturnValuesOnConditionCheckFailureType,
     ReturnValueType,
     SelectType,
     TableClassType,
     TableStatusType,
 )
 from .type_defs import (
     ArchivalSummaryResponseTypeDef,
@@ -205,15 +206,16 @@
         Expected: Mapping[str, ExpectedAttributeValueTableTypeDef] = ...,
         ConditionalOperator: ConditionalOperatorType = ...,
         ReturnValues: ReturnValueType = ...,
         ReturnConsumedCapacity: ReturnConsumedCapacityType = ...,
         ReturnItemCollectionMetrics: ReturnItemCollectionMetricsType = ...,
         ConditionExpression: ConditionBaseImportTypeDef = ...,
         ExpressionAttributeNames: Mapping[str, str] = ...,
-        ExpressionAttributeValues: Mapping[str, TableAttributeValueTypeDef] = ...
+        ExpressionAttributeValues: Mapping[str, TableAttributeValueTypeDef] = ...,
+        ReturnValuesOnConditionCheckFailure: ReturnValuesOnConditionCheckFailureType = ...
     ) -> DeleteItemOutputTableTypeDef:
         """
         Deletes a single item in a table by primary key.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB.Table.delete_item)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dynamodb/service_resource/#tabledelete_item-method)
         """
@@ -256,15 +258,16 @@
         Expected: Mapping[str, ExpectedAttributeValueTableTypeDef] = ...,
         ReturnValues: ReturnValueType = ...,
         ReturnConsumedCapacity: ReturnConsumedCapacityType = ...,
         ReturnItemCollectionMetrics: ReturnItemCollectionMetricsType = ...,
         ConditionalOperator: ConditionalOperatorType = ...,
         ConditionExpression: ConditionBaseImportTypeDef = ...,
         ExpressionAttributeNames: Mapping[str, str] = ...,
-        ExpressionAttributeValues: Mapping[str, TableAttributeValueTypeDef] = ...
+        ExpressionAttributeValues: Mapping[str, TableAttributeValueTypeDef] = ...,
+        ReturnValuesOnConditionCheckFailure: ReturnValuesOnConditionCheckFailureType = ...
     ) -> PutItemOutputTableTypeDef:
         """
         Creates a new item, or replaces an old item with a new item.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB.Table.put_item)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dynamodb/service_resource/#tableput_item-method)
         """
@@ -358,15 +361,16 @@
         ConditionalOperator: ConditionalOperatorType = ...,
         ReturnValues: ReturnValueType = ...,
         ReturnConsumedCapacity: ReturnConsumedCapacityType = ...,
         ReturnItemCollectionMetrics: ReturnItemCollectionMetricsType = ...,
         UpdateExpression: str = ...,
         ConditionExpression: ConditionBaseImportTypeDef = ...,
         ExpressionAttributeNames: Mapping[str, str] = ...,
-        ExpressionAttributeValues: Mapping[str, TableAttributeValueTypeDef] = ...
+        ExpressionAttributeValues: Mapping[str, TableAttributeValueTypeDef] = ...,
+        ReturnValuesOnConditionCheckFailure: ReturnValuesOnConditionCheckFailureType = ...
     ) -> UpdateItemOutputTableTypeDef:
         """
         Edits an existing item's attributes, or adds a new item to the table if it does
         not already exist.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB.Table.update_item)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dynamodb/service_resource/#tableupdate_item-method)
```

### Comparing `types-aiobotocore-dynamodb-2.5.2.post5/types_aiobotocore_dynamodb/type_defs.py` & `types-aiobotocore-dynamodb-2.5.4/types_aiobotocore_dynamodb/type_defs.py`

 * *Files 1% similar despite different names*

```diff
@@ -71,15 +71,14 @@
     "AttributeDefinitionTypeDef",
     "AttributeValueTypeDef",
     "TableAttributeValueTypeDef",
     "AutoScalingTargetTrackingScalingPolicyConfigurationDescriptionTypeDef",
     "AutoScalingTargetTrackingScalingPolicyConfigurationUpdateTypeDef",
     "BackupDetailsTypeDef",
     "BackupSummaryTypeDef",
-    "BatchStatementErrorTypeDef",
     "BillingModeSummaryTypeDef",
     "CapacityTypeDef",
     "ConditionBaseImportTypeDef",
     "PointInTimeRecoveryDescriptionTypeDef",
     "ContributorInsightsSummaryTypeDef",
     "CreateBackupInputRequestTypeDef",
     "KeySchemaElementTypeDef",
@@ -143,14 +142,15 @@
     "ListTablesOutputTypeDef",
     "ProvisionedThroughputDescriptionResponseTypeDef",
     "RestoreSummaryResponseTypeDef",
     "SSEDescriptionResponseTypeDef",
     "StreamSpecificationResponseTypeDef",
     "TableClassSummaryResponseTypeDef",
     "UpdateContributorInsightsOutputTypeDef",
+    "BatchStatementErrorTypeDef",
     "ItemCollectionMetricsTypeDef",
     "ItemResponseTypeDef",
     "UniversalAttributeValueTypeDef",
     "AttributeValueUpdateTableTypeDef",
     "ConditionTableTypeDef",
     "DeleteRequestServiceResourceTypeDef",
     "ExpectedAttributeValueTableTypeDef",
@@ -159,15 +159,14 @@
     "ItemCollectionMetricsTableTypeDef",
     "KeysAndAttributesServiceResourceTypeDef",
     "PutRequestServiceResourceTypeDef",
     "AutoScalingPolicyDescriptionTypeDef",
     "AutoScalingPolicyUpdateTypeDef",
     "CreateBackupOutputTypeDef",
     "ListBackupsOutputTypeDef",
-    "BatchStatementResponseTypeDef",
     "ConsumedCapacityTypeDef",
     "ContinuousBackupsDescriptionTypeDef",
     "ListContributorInsightsOutputTypeDef",
     "LocalSecondaryIndexDescriptionTableTypeDef",
     "CreateGlobalSecondaryIndexActionTableTypeDef",
     "SourceTableDetailsTypeDef",
     "UpdateGlobalSecondaryIndexActionTypeDef",
@@ -201,14 +200,15 @@
     "ImportSummaryTypeDef",
     "ListBackupsInputListBackupsPaginateTypeDef",
     "ListTablesInputListTablesPaginateTypeDef",
     "ListTagsOfResourceInputListTagsOfResourcePaginateTypeDef",
     "UpdateContinuousBackupsInputRequestTypeDef",
     "UpdateTimeToLiveInputRequestTypeDef",
     "UpdateTimeToLiveOutputTypeDef",
+    "BatchStatementResponseTypeDef",
     "AttributeValueUpdateTypeDef",
     "BatchStatementRequestTypeDef",
     "ConditionCheckTypeDef",
     "ConditionTypeDef",
     "DeleteRequestTypeDef",
     "DeleteTypeDef",
     "ExecuteStatementInputRequestTypeDef",
@@ -227,15 +227,14 @@
     "DeleteItemInputTableDeleteItemTypeDef",
     "PutItemInputTablePutItemTypeDef",
     "UpdateItemInputTableUpdateItemTypeDef",
     "BatchGetItemInputServiceResourceBatchGetItemTypeDef",
     "WriteRequestServiceResourceTypeDef",
     "AutoScalingSettingsDescriptionTypeDef",
     "AutoScalingSettingsUpdateTypeDef",
-    "BatchExecuteStatementOutputTypeDef",
     "BatchGetItemOutputServiceResourceTypeDef",
     "DeleteItemOutputTableTypeDef",
     "DeleteItemOutputTypeDef",
     "ExecuteStatementOutputTypeDef",
     "ExecuteTransactionOutputTypeDef",
     "GetItemOutputTableTypeDef",
     "GetItemOutputTypeDef",
@@ -261,14 +260,15 @@
     "RestoreTableToPointInTimeInputRequestTypeDef",
     "ListGlobalTablesOutputTypeDef",
     "ReplicaDescriptionTypeDef",
     "CreateReplicationGroupMemberActionTypeDef",
     "UpdateReplicationGroupMemberActionTypeDef",
     "UpdateGlobalTableInputRequestTypeDef",
     "ListImportsOutputTypeDef",
+    "BatchExecuteStatementOutputTypeDef",
     "BatchExecuteStatementInputRequestTypeDef",
     "QueryInputRequestTypeDef",
     "ScanInputRequestTypeDef",
     "DeleteItemInputRequestTypeDef",
     "PutItemInputRequestTypeDef",
     "UpdateItemInputRequestTypeDef",
     "TransactGetItemTypeDef",
@@ -472,23 +472,14 @@
         "BackupStatus": BackupStatusType,
         "BackupType": BackupTypeType,
         "BackupSizeBytes": int,
     },
     total=False,
 )
 
-BatchStatementErrorTypeDef = TypedDict(
-    "BatchStatementErrorTypeDef",
-    {
-        "Code": BatchStatementErrorCodeEnumType,
-        "Message": str,
-    },
-    total=False,
-)
-
 BillingModeSummaryTypeDef = TypedDict(
     "BillingModeSummaryTypeDef",
     {
         "BillingMode": BillingModeType,
         "LastUpdateToPayPerRequestDateTime": datetime,
     },
     total=False,
@@ -1175,14 +1166,24 @@
         "TableName": str,
         "IndexName": str,
         "ContributorInsightsStatus": ContributorInsightsStatusType,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+BatchStatementErrorTypeDef = TypedDict(
+    "BatchStatementErrorTypeDef",
+    {
+        "Code": BatchStatementErrorCodeEnumType,
+        "Message": str,
+        "Item": Dict[str, AttributeValueTypeDef],
+    },
+    total=False,
+)
+
 ItemCollectionMetricsTypeDef = TypedDict(
     "ItemCollectionMetricsTypeDef",
     {
         "ItemCollectionKey": Dict[str, AttributeValueTypeDef],
         "SizeEstimateRangeGB": List[float],
     },
     total=False,
@@ -1381,24 +1382,14 @@
     {
         "BackupSummaries": List[BackupSummaryTypeDef],
         "LastEvaluatedBackupArn": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-BatchStatementResponseTypeDef = TypedDict(
-    "BatchStatementResponseTypeDef",
-    {
-        "Error": BatchStatementErrorTypeDef,
-        "TableName": str,
-        "Item": Dict[str, AttributeValueTypeDef],
-    },
-    total=False,
-)
-
 ConsumedCapacityTypeDef = TypedDict(
     "ConsumedCapacityTypeDef",
     {
         "TableName": str,
         "CapacityUnits": float,
         "ReadCapacityUnits": float,
         "WriteCapacityUnits": float,
@@ -1941,14 +1932,24 @@
     "UpdateTimeToLiveOutputTypeDef",
     {
         "TimeToLiveSpecification": TimeToLiveSpecificationTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+BatchStatementResponseTypeDef = TypedDict(
+    "BatchStatementResponseTypeDef",
+    {
+        "Error": BatchStatementErrorTypeDef,
+        "TableName": str,
+        "Item": Dict[str, AttributeValueTypeDef],
+    },
+    total=False,
+)
+
 AttributeValueUpdateTypeDef = TypedDict(
     "AttributeValueUpdateTypeDef",
     {
         "Value": UniversalAttributeValueTypeDef,
         "Action": AttributeActionType,
     },
     total=False,
@@ -1961,14 +1962,15 @@
     },
 )
 _OptionalBatchStatementRequestTypeDef = TypedDict(
     "_OptionalBatchStatementRequestTypeDef",
     {
         "Parameters": Sequence[UniversalAttributeValueTypeDef],
         "ConsistentRead": bool,
+        "ReturnValuesOnConditionCheckFailure": ReturnValuesOnConditionCheckFailureType,
     },
     total=False,
 )
 
 
 class BatchStatementRequestTypeDef(
     _RequiredBatchStatementRequestTypeDef, _OptionalBatchStatementRequestTypeDef
@@ -2058,14 +2060,15 @@
     "_OptionalExecuteStatementInputRequestTypeDef",
     {
         "Parameters": Sequence[UniversalAttributeValueTypeDef],
         "ConsistentRead": bool,
         "NextToken": str,
         "ReturnConsumedCapacity": ReturnConsumedCapacityType,
         "Limit": int,
+        "ReturnValuesOnConditionCheckFailure": ReturnValuesOnConditionCheckFailureType,
     },
     total=False,
 )
 
 
 class ExecuteStatementInputRequestTypeDef(
     _RequiredExecuteStatementInputRequestTypeDef, _OptionalExecuteStatementInputRequestTypeDef
@@ -2161,14 +2164,15 @@
         "Statement": str,
     },
 )
 _OptionalParameterizedStatementTypeDef = TypedDict(
     "_OptionalParameterizedStatementTypeDef",
     {
         "Parameters": Sequence[UniversalAttributeValueTypeDef],
+        "ReturnValuesOnConditionCheckFailure": ReturnValuesOnConditionCheckFailureType,
     },
     total=False,
 )
 
 
 class ParameterizedStatementTypeDef(
     _RequiredParameterizedStatementTypeDef, _OptionalParameterizedStatementTypeDef
@@ -2357,14 +2361,15 @@
         "ConditionalOperator": ConditionalOperatorType,
         "ReturnValues": ReturnValueType,
         "ReturnConsumedCapacity": ReturnConsumedCapacityType,
         "ReturnItemCollectionMetrics": ReturnItemCollectionMetricsType,
         "ConditionExpression": ConditionBaseImportTypeDef,
         "ExpressionAttributeNames": Mapping[str, str],
         "ExpressionAttributeValues": Mapping[str, TableAttributeValueTypeDef],
+        "ReturnValuesOnConditionCheckFailure": ReturnValuesOnConditionCheckFailureType,
     },
     total=False,
 )
 
 
 class DeleteItemInputTableDeleteItemTypeDef(
     _RequiredDeleteItemInputTableDeleteItemTypeDef, _OptionalDeleteItemInputTableDeleteItemTypeDef
@@ -2385,14 +2390,15 @@
         "ReturnValues": ReturnValueType,
         "ReturnConsumedCapacity": ReturnConsumedCapacityType,
         "ReturnItemCollectionMetrics": ReturnItemCollectionMetricsType,
         "ConditionalOperator": ConditionalOperatorType,
         "ConditionExpression": ConditionBaseImportTypeDef,
         "ExpressionAttributeNames": Mapping[str, str],
         "ExpressionAttributeValues": Mapping[str, TableAttributeValueTypeDef],
+        "ReturnValuesOnConditionCheckFailure": ReturnValuesOnConditionCheckFailureType,
     },
     total=False,
 )
 
 
 class PutItemInputTablePutItemTypeDef(
     _RequiredPutItemInputTablePutItemTypeDef, _OptionalPutItemInputTablePutItemTypeDef
@@ -2415,14 +2421,15 @@
         "ReturnValues": ReturnValueType,
         "ReturnConsumedCapacity": ReturnConsumedCapacityType,
         "ReturnItemCollectionMetrics": ReturnItemCollectionMetricsType,
         "UpdateExpression": str,
         "ConditionExpression": ConditionBaseImportTypeDef,
         "ExpressionAttributeNames": Mapping[str, str],
         "ExpressionAttributeValues": Mapping[str, TableAttributeValueTypeDef],
+        "ReturnValuesOnConditionCheckFailure": ReturnValuesOnConditionCheckFailureType,
     },
     total=False,
 )
 
 
 class UpdateItemInputTableUpdateItemTypeDef(
     _RequiredUpdateItemInputTableUpdateItemTypeDef, _OptionalUpdateItemInputTableUpdateItemTypeDef
@@ -2481,23 +2488,14 @@
         "AutoScalingDisabled": bool,
         "AutoScalingRoleArn": str,
         "ScalingPolicyUpdate": AutoScalingPolicyUpdateTypeDef,
     },
     total=False,
 )
 
-BatchExecuteStatementOutputTypeDef = TypedDict(
-    "BatchExecuteStatementOutputTypeDef",
-    {
-        "Responses": List[BatchStatementResponseTypeDef],
-        "ConsumedCapacity": List[ConsumedCapacityTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 BatchGetItemOutputServiceResourceTypeDef = TypedDict(
     "BatchGetItemOutputServiceResourceTypeDef",
     {
         "Responses": Dict[str, List[Dict[str, TableAttributeValueTypeDef]]],
         "UnprocessedKeys": Dict[str, KeysAndAttributesServiceResourceTypeDef],
         "ConsumedCapacity": List[ConsumedCapacityTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
@@ -2950,14 +2948,23 @@
     {
         "ImportSummaryList": List[ImportSummaryTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+BatchExecuteStatementOutputTypeDef = TypedDict(
+    "BatchExecuteStatementOutputTypeDef",
+    {
+        "Responses": List[BatchStatementResponseTypeDef],
+        "ConsumedCapacity": List[ConsumedCapacityTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 _RequiredBatchExecuteStatementInputRequestTypeDef = TypedDict(
     "_RequiredBatchExecuteStatementInputRequestTypeDef",
     {
         "Statements": Sequence[BatchStatementRequestTypeDef],
     },
 )
 _OptionalBatchExecuteStatementInputRequestTypeDef = TypedDict(
@@ -3059,14 +3066,15 @@
         "ConditionalOperator": ConditionalOperatorType,
         "ReturnValues": ReturnValueType,
         "ReturnConsumedCapacity": ReturnConsumedCapacityType,
         "ReturnItemCollectionMetrics": ReturnItemCollectionMetricsType,
         "ConditionExpression": str,
         "ExpressionAttributeNames": Mapping[str, str],
         "ExpressionAttributeValues": Mapping[str, UniversalAttributeValueTypeDef],
+        "ReturnValuesOnConditionCheckFailure": ReturnValuesOnConditionCheckFailureType,
     },
     total=False,
 )
 
 
 class DeleteItemInputRequestTypeDef(
     _RequiredDeleteItemInputRequestTypeDef, _OptionalDeleteItemInputRequestTypeDef
@@ -3088,14 +3096,15 @@
         "ReturnValues": ReturnValueType,
         "ReturnConsumedCapacity": ReturnConsumedCapacityType,
         "ReturnItemCollectionMetrics": ReturnItemCollectionMetricsType,
         "ConditionalOperator": ConditionalOperatorType,
         "ConditionExpression": str,
         "ExpressionAttributeNames": Mapping[str, str],
         "ExpressionAttributeValues": Mapping[str, UniversalAttributeValueTypeDef],
+        "ReturnValuesOnConditionCheckFailure": ReturnValuesOnConditionCheckFailureType,
     },
     total=False,
 )
 
 
 class PutItemInputRequestTypeDef(
     _RequiredPutItemInputRequestTypeDef, _OptionalPutItemInputRequestTypeDef
@@ -3119,14 +3128,15 @@
         "ReturnValues": ReturnValueType,
         "ReturnConsumedCapacity": ReturnConsumedCapacityType,
         "ReturnItemCollectionMetrics": ReturnItemCollectionMetricsType,
         "UpdateExpression": str,
         "ConditionExpression": str,
         "ExpressionAttributeNames": Mapping[str, str],
         "ExpressionAttributeValues": Mapping[str, UniversalAttributeValueTypeDef],
+        "ReturnValuesOnConditionCheckFailure": ReturnValuesOnConditionCheckFailureType,
     },
     total=False,
 )
 
 
 class UpdateItemInputRequestTypeDef(
     _RequiredUpdateItemInputRequestTypeDef, _OptionalUpdateItemInputRequestTypeDef
```

### Comparing `types-aiobotocore-dynamodb-2.5.2.post5/types_aiobotocore_dynamodb/type_defs.pyi` & `types-aiobotocore-dynamodb-2.5.4/types_aiobotocore_dynamodb/type_defs.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -70,15 +70,14 @@
     "AttributeDefinitionTypeDef",
     "AttributeValueTypeDef",
     "TableAttributeValueTypeDef",
     "AutoScalingTargetTrackingScalingPolicyConfigurationDescriptionTypeDef",
     "AutoScalingTargetTrackingScalingPolicyConfigurationUpdateTypeDef",
     "BackupDetailsTypeDef",
     "BackupSummaryTypeDef",
-    "BatchStatementErrorTypeDef",
     "BillingModeSummaryTypeDef",
     "CapacityTypeDef",
     "ConditionBaseImportTypeDef",
     "PointInTimeRecoveryDescriptionTypeDef",
     "ContributorInsightsSummaryTypeDef",
     "CreateBackupInputRequestTypeDef",
     "KeySchemaElementTypeDef",
@@ -142,14 +141,15 @@
     "ListTablesOutputTypeDef",
     "ProvisionedThroughputDescriptionResponseTypeDef",
     "RestoreSummaryResponseTypeDef",
     "SSEDescriptionResponseTypeDef",
     "StreamSpecificationResponseTypeDef",
     "TableClassSummaryResponseTypeDef",
     "UpdateContributorInsightsOutputTypeDef",
+    "BatchStatementErrorTypeDef",
     "ItemCollectionMetricsTypeDef",
     "ItemResponseTypeDef",
     "UniversalAttributeValueTypeDef",
     "AttributeValueUpdateTableTypeDef",
     "ConditionTableTypeDef",
     "DeleteRequestServiceResourceTypeDef",
     "ExpectedAttributeValueTableTypeDef",
@@ -158,15 +158,14 @@
     "ItemCollectionMetricsTableTypeDef",
     "KeysAndAttributesServiceResourceTypeDef",
     "PutRequestServiceResourceTypeDef",
     "AutoScalingPolicyDescriptionTypeDef",
     "AutoScalingPolicyUpdateTypeDef",
     "CreateBackupOutputTypeDef",
     "ListBackupsOutputTypeDef",
-    "BatchStatementResponseTypeDef",
     "ConsumedCapacityTypeDef",
     "ContinuousBackupsDescriptionTypeDef",
     "ListContributorInsightsOutputTypeDef",
     "LocalSecondaryIndexDescriptionTableTypeDef",
     "CreateGlobalSecondaryIndexActionTableTypeDef",
     "SourceTableDetailsTypeDef",
     "UpdateGlobalSecondaryIndexActionTypeDef",
@@ -200,14 +199,15 @@
     "ImportSummaryTypeDef",
     "ListBackupsInputListBackupsPaginateTypeDef",
     "ListTablesInputListTablesPaginateTypeDef",
     "ListTagsOfResourceInputListTagsOfResourcePaginateTypeDef",
     "UpdateContinuousBackupsInputRequestTypeDef",
     "UpdateTimeToLiveInputRequestTypeDef",
     "UpdateTimeToLiveOutputTypeDef",
+    "BatchStatementResponseTypeDef",
     "AttributeValueUpdateTypeDef",
     "BatchStatementRequestTypeDef",
     "ConditionCheckTypeDef",
     "ConditionTypeDef",
     "DeleteRequestTypeDef",
     "DeleteTypeDef",
     "ExecuteStatementInputRequestTypeDef",
@@ -226,15 +226,14 @@
     "DeleteItemInputTableDeleteItemTypeDef",
     "PutItemInputTablePutItemTypeDef",
     "UpdateItemInputTableUpdateItemTypeDef",
     "BatchGetItemInputServiceResourceBatchGetItemTypeDef",
     "WriteRequestServiceResourceTypeDef",
     "AutoScalingSettingsDescriptionTypeDef",
     "AutoScalingSettingsUpdateTypeDef",
-    "BatchExecuteStatementOutputTypeDef",
     "BatchGetItemOutputServiceResourceTypeDef",
     "DeleteItemOutputTableTypeDef",
     "DeleteItemOutputTypeDef",
     "ExecuteStatementOutputTypeDef",
     "ExecuteTransactionOutputTypeDef",
     "GetItemOutputTableTypeDef",
     "GetItemOutputTypeDef",
@@ -260,14 +259,15 @@
     "RestoreTableToPointInTimeInputRequestTypeDef",
     "ListGlobalTablesOutputTypeDef",
     "ReplicaDescriptionTypeDef",
     "CreateReplicationGroupMemberActionTypeDef",
     "UpdateReplicationGroupMemberActionTypeDef",
     "UpdateGlobalTableInputRequestTypeDef",
     "ListImportsOutputTypeDef",
+    "BatchExecuteStatementOutputTypeDef",
     "BatchExecuteStatementInputRequestTypeDef",
     "QueryInputRequestTypeDef",
     "ScanInputRequestTypeDef",
     "DeleteItemInputRequestTypeDef",
     "PutItemInputRequestTypeDef",
     "UpdateItemInputRequestTypeDef",
     "TransactGetItemTypeDef",
@@ -465,23 +465,14 @@
         "BackupStatus": BackupStatusType,
         "BackupType": BackupTypeType,
         "BackupSizeBytes": int,
     },
     total=False,
 )
 
-BatchStatementErrorTypeDef = TypedDict(
-    "BatchStatementErrorTypeDef",
-    {
-        "Code": BatchStatementErrorCodeEnumType,
-        "Message": str,
-    },
-    total=False,
-)
-
 BillingModeSummaryTypeDef = TypedDict(
     "BillingModeSummaryTypeDef",
     {
         "BillingMode": BillingModeType,
         "LastUpdateToPayPerRequestDateTime": datetime,
     },
     total=False,
@@ -1156,14 +1147,24 @@
         "TableName": str,
         "IndexName": str,
         "ContributorInsightsStatus": ContributorInsightsStatusType,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+BatchStatementErrorTypeDef = TypedDict(
+    "BatchStatementErrorTypeDef",
+    {
+        "Code": BatchStatementErrorCodeEnumType,
+        "Message": str,
+        "Item": Dict[str, AttributeValueTypeDef],
+    },
+    total=False,
+)
+
 ItemCollectionMetricsTypeDef = TypedDict(
     "ItemCollectionMetricsTypeDef",
     {
         "ItemCollectionKey": Dict[str, AttributeValueTypeDef],
         "SizeEstimateRangeGB": List[float],
     },
     total=False,
@@ -1354,24 +1355,14 @@
     {
         "BackupSummaries": List[BackupSummaryTypeDef],
         "LastEvaluatedBackupArn": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-BatchStatementResponseTypeDef = TypedDict(
-    "BatchStatementResponseTypeDef",
-    {
-        "Error": BatchStatementErrorTypeDef,
-        "TableName": str,
-        "Item": Dict[str, AttributeValueTypeDef],
-    },
-    total=False,
-)
-
 ConsumedCapacityTypeDef = TypedDict(
     "ConsumedCapacityTypeDef",
     {
         "TableName": str,
         "CapacityUnits": float,
         "ReadCapacityUnits": float,
         "WriteCapacityUnits": float,
@@ -1894,14 +1885,24 @@
     "UpdateTimeToLiveOutputTypeDef",
     {
         "TimeToLiveSpecification": TimeToLiveSpecificationTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+BatchStatementResponseTypeDef = TypedDict(
+    "BatchStatementResponseTypeDef",
+    {
+        "Error": BatchStatementErrorTypeDef,
+        "TableName": str,
+        "Item": Dict[str, AttributeValueTypeDef],
+    },
+    total=False,
+)
+
 AttributeValueUpdateTypeDef = TypedDict(
     "AttributeValueUpdateTypeDef",
     {
         "Value": UniversalAttributeValueTypeDef,
         "Action": AttributeActionType,
     },
     total=False,
@@ -1914,14 +1915,15 @@
     },
 )
 _OptionalBatchStatementRequestTypeDef = TypedDict(
     "_OptionalBatchStatementRequestTypeDef",
     {
         "Parameters": Sequence[UniversalAttributeValueTypeDef],
         "ConsistentRead": bool,
+        "ReturnValuesOnConditionCheckFailure": ReturnValuesOnConditionCheckFailureType,
     },
     total=False,
 )
 
 class BatchStatementRequestTypeDef(
     _RequiredBatchStatementRequestTypeDef, _OptionalBatchStatementRequestTypeDef
 ):
@@ -2003,14 +2005,15 @@
     "_OptionalExecuteStatementInputRequestTypeDef",
     {
         "Parameters": Sequence[UniversalAttributeValueTypeDef],
         "ConsistentRead": bool,
         "NextToken": str,
         "ReturnConsumedCapacity": ReturnConsumedCapacityType,
         "Limit": int,
+        "ReturnValuesOnConditionCheckFailure": ReturnValuesOnConditionCheckFailureType,
     },
     total=False,
 )
 
 class ExecuteStatementInputRequestTypeDef(
     _RequiredExecuteStatementInputRequestTypeDef, _OptionalExecuteStatementInputRequestTypeDef
 ):
@@ -2098,14 +2101,15 @@
         "Statement": str,
     },
 )
 _OptionalParameterizedStatementTypeDef = TypedDict(
     "_OptionalParameterizedStatementTypeDef",
     {
         "Parameters": Sequence[UniversalAttributeValueTypeDef],
+        "ReturnValuesOnConditionCheckFailure": ReturnValuesOnConditionCheckFailureType,
     },
     total=False,
 )
 
 class ParameterizedStatementTypeDef(
     _RequiredParameterizedStatementTypeDef, _OptionalParameterizedStatementTypeDef
 ):
@@ -2284,14 +2288,15 @@
         "ConditionalOperator": ConditionalOperatorType,
         "ReturnValues": ReturnValueType,
         "ReturnConsumedCapacity": ReturnConsumedCapacityType,
         "ReturnItemCollectionMetrics": ReturnItemCollectionMetricsType,
         "ConditionExpression": ConditionBaseImportTypeDef,
         "ExpressionAttributeNames": Mapping[str, str],
         "ExpressionAttributeValues": Mapping[str, TableAttributeValueTypeDef],
+        "ReturnValuesOnConditionCheckFailure": ReturnValuesOnConditionCheckFailureType,
     },
     total=False,
 )
 
 class DeleteItemInputTableDeleteItemTypeDef(
     _RequiredDeleteItemInputTableDeleteItemTypeDef, _OptionalDeleteItemInputTableDeleteItemTypeDef
 ):
@@ -2310,14 +2315,15 @@
         "ReturnValues": ReturnValueType,
         "ReturnConsumedCapacity": ReturnConsumedCapacityType,
         "ReturnItemCollectionMetrics": ReturnItemCollectionMetricsType,
         "ConditionalOperator": ConditionalOperatorType,
         "ConditionExpression": ConditionBaseImportTypeDef,
         "ExpressionAttributeNames": Mapping[str, str],
         "ExpressionAttributeValues": Mapping[str, TableAttributeValueTypeDef],
+        "ReturnValuesOnConditionCheckFailure": ReturnValuesOnConditionCheckFailureType,
     },
     total=False,
 )
 
 class PutItemInputTablePutItemTypeDef(
     _RequiredPutItemInputTablePutItemTypeDef, _OptionalPutItemInputTablePutItemTypeDef
 ):
@@ -2338,14 +2344,15 @@
         "ReturnValues": ReturnValueType,
         "ReturnConsumedCapacity": ReturnConsumedCapacityType,
         "ReturnItemCollectionMetrics": ReturnItemCollectionMetricsType,
         "UpdateExpression": str,
         "ConditionExpression": ConditionBaseImportTypeDef,
         "ExpressionAttributeNames": Mapping[str, str],
         "ExpressionAttributeValues": Mapping[str, TableAttributeValueTypeDef],
+        "ReturnValuesOnConditionCheckFailure": ReturnValuesOnConditionCheckFailureType,
     },
     total=False,
 )
 
 class UpdateItemInputTableUpdateItemTypeDef(
     _RequiredUpdateItemInputTableUpdateItemTypeDef, _OptionalUpdateItemInputTableUpdateItemTypeDef
 ):
@@ -2400,23 +2407,14 @@
         "AutoScalingDisabled": bool,
         "AutoScalingRoleArn": str,
         "ScalingPolicyUpdate": AutoScalingPolicyUpdateTypeDef,
     },
     total=False,
 )
 
-BatchExecuteStatementOutputTypeDef = TypedDict(
-    "BatchExecuteStatementOutputTypeDef",
-    {
-        "Responses": List[BatchStatementResponseTypeDef],
-        "ConsumedCapacity": List[ConsumedCapacityTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 BatchGetItemOutputServiceResourceTypeDef = TypedDict(
     "BatchGetItemOutputServiceResourceTypeDef",
     {
         "Responses": Dict[str, List[Dict[str, TableAttributeValueTypeDef]]],
         "UnprocessedKeys": Dict[str, KeysAndAttributesServiceResourceTypeDef],
         "ConsumedCapacity": List[ConsumedCapacityTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
@@ -2855,14 +2853,23 @@
     {
         "ImportSummaryList": List[ImportSummaryTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+BatchExecuteStatementOutputTypeDef = TypedDict(
+    "BatchExecuteStatementOutputTypeDef",
+    {
+        "Responses": List[BatchStatementResponseTypeDef],
+        "ConsumedCapacity": List[ConsumedCapacityTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 _RequiredBatchExecuteStatementInputRequestTypeDef = TypedDict(
     "_RequiredBatchExecuteStatementInputRequestTypeDef",
     {
         "Statements": Sequence[BatchStatementRequestTypeDef],
     },
 )
 _OptionalBatchExecuteStatementInputRequestTypeDef = TypedDict(
@@ -2958,14 +2965,15 @@
         "ConditionalOperator": ConditionalOperatorType,
         "ReturnValues": ReturnValueType,
         "ReturnConsumedCapacity": ReturnConsumedCapacityType,
         "ReturnItemCollectionMetrics": ReturnItemCollectionMetricsType,
         "ConditionExpression": str,
         "ExpressionAttributeNames": Mapping[str, str],
         "ExpressionAttributeValues": Mapping[str, UniversalAttributeValueTypeDef],
+        "ReturnValuesOnConditionCheckFailure": ReturnValuesOnConditionCheckFailureType,
     },
     total=False,
 )
 
 class DeleteItemInputRequestTypeDef(
     _RequiredDeleteItemInputRequestTypeDef, _OptionalDeleteItemInputRequestTypeDef
 ):
@@ -2985,14 +2993,15 @@
         "ReturnValues": ReturnValueType,
         "ReturnConsumedCapacity": ReturnConsumedCapacityType,
         "ReturnItemCollectionMetrics": ReturnItemCollectionMetricsType,
         "ConditionalOperator": ConditionalOperatorType,
         "ConditionExpression": str,
         "ExpressionAttributeNames": Mapping[str, str],
         "ExpressionAttributeValues": Mapping[str, UniversalAttributeValueTypeDef],
+        "ReturnValuesOnConditionCheckFailure": ReturnValuesOnConditionCheckFailureType,
     },
     total=False,
 )
 
 class PutItemInputRequestTypeDef(
     _RequiredPutItemInputRequestTypeDef, _OptionalPutItemInputRequestTypeDef
 ):
@@ -3014,14 +3023,15 @@
         "ReturnValues": ReturnValueType,
         "ReturnConsumedCapacity": ReturnConsumedCapacityType,
         "ReturnItemCollectionMetrics": ReturnItemCollectionMetricsType,
         "UpdateExpression": str,
         "ConditionExpression": str,
         "ExpressionAttributeNames": Mapping[str, str],
         "ExpressionAttributeValues": Mapping[str, UniversalAttributeValueTypeDef],
+        "ReturnValuesOnConditionCheckFailure": ReturnValuesOnConditionCheckFailureType,
     },
     total=False,
 )
 
 class UpdateItemInputRequestTypeDef(
     _RequiredUpdateItemInputRequestTypeDef, _OptionalUpdateItemInputRequestTypeDef
 ):
```

### Comparing `types-aiobotocore-dynamodb-2.5.2.post5/types_aiobotocore_dynamodb/waiter.py` & `types-aiobotocore-dynamodb-2.5.4/types_aiobotocore_dynamodb/waiter.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-dynamodb-2.5.2.post5/types_aiobotocore_dynamodb/waiter.pyi` & `types-aiobotocore-dynamodb-2.5.4/types_aiobotocore_dynamodb/waiter.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-dynamodb-2.5.2.post5/types_aiobotocore_dynamodb.egg-info/PKG-INFO` & `types-aiobotocore-dynamodb-2.5.4/types_aiobotocore_dynamodb.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-dynamodb
-Version: 2.5.2.post5
-Summary: Type annotations for aiobotocore.DynamoDB 2.5.2 service generated with mypy-boto3-builder 7.17.2
+Version: 2.5.4
+Summary: Type annotations for aiobotocore.DynamoDB 2.5.4 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dynamodb/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-dynamodb.svg?color=blue)](https://pypi.org/project/types-aiobotocore-dynamodb)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dynamodb/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-dynamodb)](https://pepy.tech/project/types-aiobotocore-dynamodb)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.DynamoDB 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB)
+[aiobotocore.DynamoDB 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-dynamodb-2.5.2.post5/types_aiobotocore_dynamodb.egg-info/SOURCES.txt` & `types-aiobotocore-dynamodb-2.5.4/types_aiobotocore_dynamodb.egg-info/SOURCES.txt`

 * *Files identical despite different names*


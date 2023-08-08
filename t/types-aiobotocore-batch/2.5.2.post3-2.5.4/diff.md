# Comparing `tmp/types-aiobotocore-batch-2.5.2.post3.tar.gz` & `tmp/types-aiobotocore-batch-2.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-batch-2.5.2.post3.tar", last modified: Fri Aug  4 12:37:21 2023, max compression
+gzip compressed data, was "types-aiobotocore-batch-2.5.4.tar", last modified: Tue Aug  8 01:23:21 2023, max compression
```

## Comparing `types-aiobotocore-batch-2.5.2.post3.tar` & `types-aiobotocore-batch-2.5.4.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:37:21.479279 types-aiobotocore-batch-2.5.2.post3/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-04 12:18:58.000000 types-aiobotocore-batch-2.5.2.post3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    13484 2023-08-04 12:37:21.479279 types-aiobotocore-batch-2.5.2.post3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    11974 2023-08-04 12:18:58.000000 types-aiobotocore-batch-2.5.2.post3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-04 12:37:21.479279 types-aiobotocore-batch-2.5.2.post3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2058 2023-08-04 12:18:57.000000 types-aiobotocore-batch-2.5.2.post3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:37:21.471279 types-aiobotocore-batch-2.5.2.post3/types_aiobotocore_batch/
--rw-r--r--   0 runner    (1001) docker     (123)     1579 2023-08-04 12:18:58.000000 types-aiobotocore-batch-2.5.2.post3/types_aiobotocore_batch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1578 2023-08-04 12:18:58.000000 types-aiobotocore-batch-2.5.2.post3/types_aiobotocore_batch/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      924 2023-08-04 12:18:58.000000 types-aiobotocore-batch-2.5.2.post3/types_aiobotocore_batch/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    22153 2023-08-04 12:18:58.000000 types-aiobotocore-batch-2.5.2.post3/types_aiobotocore_batch/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    22115 2023-08-04 12:18:58.000000 types-aiobotocore-batch-2.5.2.post3/types_aiobotocore_batch/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    10647 2023-08-04 12:18:58.000000 types-aiobotocore-batch-2.5.2.post3/types_aiobotocore_batch/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    10645 2023-08-04 12:18:58.000000 types-aiobotocore-batch-2.5.2.post3/types_aiobotocore_batch/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     6978 2023-08-04 12:18:58.000000 types-aiobotocore-batch-2.5.2.post3/types_aiobotocore_batch/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     6971 2023-08-04 12:18:58.000000 types-aiobotocore-batch-2.5.2.post3/types_aiobotocore_batch/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 12:18:58.000000 types-aiobotocore-batch-2.5.2.post3/types_aiobotocore_batch/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    44039 2023-08-04 12:19:00.000000 types-aiobotocore-batch-2.5.2.post3/types_aiobotocore_batch/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    43982 2023-08-04 12:18:58.000000 types-aiobotocore-batch-2.5.2.post3/types_aiobotocore_batch/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-04 12:18:58.000000 types-aiobotocore-batch-2.5.2.post3/types_aiobotocore_batch/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:37:21.475279 types-aiobotocore-batch-2.5.2.post3/types_aiobotocore_batch.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    13484 2023-08-04 12:37:21.000000 types-aiobotocore-batch-2.5.2.post3/types_aiobotocore_batch.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      775 2023-08-04 12:37:21.000000 types-aiobotocore-batch-2.5.2.post3/types_aiobotocore_batch.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 12:37:21.000000 types-aiobotocore-batch-2.5.2.post3/types_aiobotocore_batch.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 12:37:21.000000 types-aiobotocore-batch-2.5.2.post3/types_aiobotocore_batch.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-04 12:37:21.000000 types-aiobotocore-batch-2.5.2.post3/types_aiobotocore_batch.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-08-04 12:37:21.000000 types-aiobotocore-batch-2.5.2.post3/types_aiobotocore_batch.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:23:21.842620 types-aiobotocore-batch-2.5.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-08 01:06:43.000000 types-aiobotocore-batch-2.5.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    13478 2023-08-08 01:23:21.842620 types-aiobotocore-batch-2.5.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    11974 2023-08-08 01:06:43.000000 types-aiobotocore-batch-2.5.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-08 01:23:21.842620 types-aiobotocore-batch-2.5.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2052 2023-08-08 01:06:43.000000 types-aiobotocore-batch-2.5.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:23:21.842620 types-aiobotocore-batch-2.5.4/types_aiobotocore_batch/
+-rw-r--r--   0 runner    (1001) docker     (123)     1579 2023-08-08 01:06:43.000000 types-aiobotocore-batch-2.5.4/types_aiobotocore_batch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1578 2023-08-08 01:06:43.000000 types-aiobotocore-batch-2.5.4/types_aiobotocore_batch/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      912 2023-08-08 01:06:43.000000 types-aiobotocore-batch-2.5.4/types_aiobotocore_batch/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22153 2023-08-08 01:06:44.000000 types-aiobotocore-batch-2.5.4/types_aiobotocore_batch/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22115 2023-08-08 01:06:43.000000 types-aiobotocore-batch-2.5.4/types_aiobotocore_batch/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    10820 2023-08-08 01:06:44.000000 types-aiobotocore-batch-2.5.4/types_aiobotocore_batch/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10818 2023-08-08 01:06:44.000000 types-aiobotocore-batch-2.5.4/types_aiobotocore_batch/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     6978 2023-08-08 01:06:44.000000 types-aiobotocore-batch-2.5.4/types_aiobotocore_batch/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6971 2023-08-08 01:06:44.000000 types-aiobotocore-batch-2.5.4/types_aiobotocore_batch/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 01:06:43.000000 types-aiobotocore-batch-2.5.4/types_aiobotocore_batch/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    44340 2023-08-08 01:06:45.000000 types-aiobotocore-batch-2.5.4/types_aiobotocore_batch/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    44283 2023-08-08 01:06:44.000000 types-aiobotocore-batch-2.5.4/types_aiobotocore_batch/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-08-08 01:06:43.000000 types-aiobotocore-batch-2.5.4/types_aiobotocore_batch/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:23:21.842620 types-aiobotocore-batch-2.5.4/types_aiobotocore_batch.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    13478 2023-08-08 01:23:21.000000 types-aiobotocore-batch-2.5.4/types_aiobotocore_batch.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      775 2023-08-08 01:23:21.000000 types-aiobotocore-batch-2.5.4/types_aiobotocore_batch.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 01:23:21.000000 types-aiobotocore-batch-2.5.4/types_aiobotocore_batch.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 01:23:21.000000 types-aiobotocore-batch-2.5.4/types_aiobotocore_batch.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-08 01:23:21.000000 types-aiobotocore-batch-2.5.4/types_aiobotocore_batch.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-08-08 01:23:21.000000 types-aiobotocore-batch-2.5.4/types_aiobotocore_batch.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-batch-2.5.2.post3/LICENSE` & `types-aiobotocore-batch-2.5.4/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-batch-2.5.2.post3/PKG-INFO` & `types-aiobotocore-batch-2.5.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-batch
-Version: 2.5.2.post3
-Summary: Type annotations for aiobotocore.Batch 2.5.2 service generated with mypy-boto3-builder 7.17.2
+Version: 2.5.4
+Summary: Type annotations for aiobotocore.Batch 2.5.4 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_batch/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-batch.svg?color=blue)](https://pypi.org/project/types-aiobotocore-batch)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_batch/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-batch)](https://pepy.tech/project/types-aiobotocore-batch)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.Batch 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/batch.html#Batch)
+[aiobotocore.Batch 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/batch.html#Batch)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-batch-2.5.2.post3/README.md` & `types-aiobotocore-batch-2.5.4/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-batch.svg?color=blue)](https://pypi.org/project/types-aiobotocore-batch)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_batch/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-batch)](https://pepy.tech/project/types-aiobotocore-batch)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.Batch 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/batch.html#Batch)
+[aiobotocore.Batch 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/batch.html#Batch)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-batch-2.5.2.post3/setup.py` & `types-aiobotocore-batch-2.5.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-batch",
-    version="2.5.2.post3",
+    version="2.5.4",
     packages=["types_aiobotocore_batch"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.Batch 2.5.2 service generated with mypy-boto3-builder"
+        "Type annotations for aiobotocore.Batch 2.5.4 service generated with mypy-boto3-builder"
         " 7.17.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
```

### Comparing `types-aiobotocore-batch-2.5.2.post3/types_aiobotocore_batch/__init__.py` & `types-aiobotocore-batch-2.5.4/types_aiobotocore_batch/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-batch-2.5.2.post3/types_aiobotocore_batch/__init__.pyi` & `types-aiobotocore-batch-2.5.4/types_aiobotocore_batch/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-batch-2.5.2.post3/types_aiobotocore_batch/__main__.py` & `types-aiobotocore-batch-2.5.4/types_aiobotocore_batch/__main__.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.Batch 2.5.2\nVersion:         2.5.2.post3\nBuilder"
-        " version: 7.17.2\nDocs:           "
+        "Type annotations for aiobotocore.Batch 2.5.4\nVersion:         2.5.4\nBuilder version:"
+        " 7.17.2\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_batch//\nBoto3 docs:  "
         "    https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/batch.html#Batch\nOther"
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

### Comparing `types-aiobotocore-batch-2.5.2.post3/types_aiobotocore_batch/client.py` & `types-aiobotocore-batch-2.5.4/types_aiobotocore_batch/client.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-batch-2.5.2.post3/types_aiobotocore_batch/client.pyi` & `types-aiobotocore-batch-2.5.4/types_aiobotocore_batch/client.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-batch-2.5.2.post3/types_aiobotocore_batch/literals.py` & `types-aiobotocore-batch-2.5.4/types_aiobotocore_batch/literals.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -14,15 +14,14 @@
 import sys
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = (
     "ArrayJobDependencyType",
     "AssignPublicIpType",
     "CEStateType",
     "CEStatusType",
     "CETypeType",
     "CRAllocationStrategyType",
@@ -48,23 +47,26 @@
     "BatchServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "RegionName",
 )
 
-
 ArrayJobDependencyType = Literal["N_TO_N", "SEQUENTIAL"]
 AssignPublicIpType = Literal["DISABLED", "ENABLED"]
 CEStateType = Literal["DISABLED", "ENABLED"]
 CEStatusType = Literal["CREATING", "DELETED", "DELETING", "INVALID", "UPDATING", "VALID"]
 CETypeType = Literal["MANAGED", "UNMANAGED"]
-CRAllocationStrategyType = Literal["BEST_FIT", "BEST_FIT_PROGRESSIVE", "SPOT_CAPACITY_OPTIMIZED"]
+CRAllocationStrategyType = Literal[
+    "BEST_FIT", "BEST_FIT_PROGRESSIVE", "SPOT_CAPACITY_OPTIMIZED", "SPOT_PRICE_CAPACITY_OPTIMIZED"
+]
 CRTypeType = Literal["EC2", "FARGATE", "FARGATE_SPOT", "SPOT"]
-CRUpdateAllocationStrategyType = Literal["BEST_FIT_PROGRESSIVE", "SPOT_CAPACITY_OPTIMIZED"]
+CRUpdateAllocationStrategyType = Literal[
+    "BEST_FIT_PROGRESSIVE", "SPOT_CAPACITY_OPTIMIZED", "SPOT_PRICE_CAPACITY_OPTIMIZED"
+]
 DescribeComputeEnvironmentsPaginatorName = Literal["describe_compute_environments"]
 DescribeJobDefinitionsPaginatorName = Literal["describe_job_definitions"]
 DescribeJobQueuesPaginatorName = Literal["describe_job_queues"]
 DeviceCgroupPermissionType = Literal["MKNOD", "READ", "WRITE"]
 EFSAuthorizationConfigIAMType = Literal["DISABLED", "ENABLED"]
 EFSTransitEncryptionType = Literal["DISABLED", "ENABLED"]
 JQStateType = Literal["DISABLED", "ENABLED"]
@@ -92,14 +94,15 @@
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
@@ -195,14 +198,15 @@
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
@@ -281,26 +285,28 @@
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

### Comparing `types-aiobotocore-batch-2.5.2.post3/types_aiobotocore_batch/literals.pyi` & `types-aiobotocore-batch-2.5.4/types_aiobotocore_batch/literals.py`

 * *Files 5% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 import sys
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
+
 __all__ = (
     "ArrayJobDependencyType",
     "AssignPublicIpType",
     "CEStateType",
     "CEStatusType",
     "CETypeType",
     "CRAllocationStrategyType",
@@ -47,22 +48,27 @@
     "BatchServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "RegionName",
 )
 
+
 ArrayJobDependencyType = Literal["N_TO_N", "SEQUENTIAL"]
 AssignPublicIpType = Literal["DISABLED", "ENABLED"]
 CEStateType = Literal["DISABLED", "ENABLED"]
 CEStatusType = Literal["CREATING", "DELETED", "DELETING", "INVALID", "UPDATING", "VALID"]
 CETypeType = Literal["MANAGED", "UNMANAGED"]
-CRAllocationStrategyType = Literal["BEST_FIT", "BEST_FIT_PROGRESSIVE", "SPOT_CAPACITY_OPTIMIZED"]
+CRAllocationStrategyType = Literal[
+    "BEST_FIT", "BEST_FIT_PROGRESSIVE", "SPOT_CAPACITY_OPTIMIZED", "SPOT_PRICE_CAPACITY_OPTIMIZED"
+]
 CRTypeType = Literal["EC2", "FARGATE", "FARGATE_SPOT", "SPOT"]
-CRUpdateAllocationStrategyType = Literal["BEST_FIT_PROGRESSIVE", "SPOT_CAPACITY_OPTIMIZED"]
+CRUpdateAllocationStrategyType = Literal[
+    "BEST_FIT_PROGRESSIVE", "SPOT_CAPACITY_OPTIMIZED", "SPOT_PRICE_CAPACITY_OPTIMIZED"
+]
 DescribeComputeEnvironmentsPaginatorName = Literal["describe_compute_environments"]
 DescribeJobDefinitionsPaginatorName = Literal["describe_job_definitions"]
 DescribeJobQueuesPaginatorName = Literal["describe_job_queues"]
 DeviceCgroupPermissionType = Literal["MKNOD", "READ", "WRITE"]
 EFSAuthorizationConfigIAMType = Literal["DISABLED", "ENABLED"]
 EFSTransitEncryptionType = Literal["DISABLED", "ENABLED"]
 JQStateType = Literal["DISABLED", "ENABLED"]
@@ -90,14 +96,15 @@
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
@@ -193,14 +200,15 @@
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
@@ -279,26 +287,28 @@
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

### Comparing `types-aiobotocore-batch-2.5.2.post3/types_aiobotocore_batch/paginator.py` & `types-aiobotocore-batch-2.5.4/types_aiobotocore_batch/paginator.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-batch-2.5.2.post3/types_aiobotocore_batch/paginator.pyi` & `types-aiobotocore-batch-2.5.4/types_aiobotocore_batch/paginator.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-batch-2.5.2.post3/types_aiobotocore_batch/type_defs.py` & `types-aiobotocore-batch-2.5.4/types_aiobotocore_batch/type_defs.py`

 * *Files 1% similar despite different names*

```diff
@@ -56,14 +56,15 @@
     "LaunchTemplateSpecificationTypeDef",
     "EphemeralStorageTypeDef",
     "FargatePlatformConfigurationTypeDef",
     "KeyValuePairTypeDef",
     "MountPointTypeDef",
     "NetworkConfigurationTypeDef",
     "ResourceRequirementTypeDef",
+    "RuntimePlatformTypeDef",
     "SecretTypeDef",
     "UlimitTypeDef",
     "ContainerSummaryTypeDef",
     "ResponseMetadataTypeDef",
     "DeleteComputeEnvironmentRequestRequestTypeDef",
     "DeleteJobQueueRequestRequestTypeDef",
     "DeleteSchedulingPolicyRequestRequestTypeDef",
@@ -311,14 +312,23 @@
     "ResourceRequirementTypeDef",
     {
         "value": str,
         "type": ResourceTypeType,
     },
 )
 
+RuntimePlatformTypeDef = TypedDict(
+    "RuntimePlatformTypeDef",
+    {
+        "operatingSystemFamily": str,
+        "cpuArchitecture": str,
+    },
+    total=False,
+)
+
 SecretTypeDef = TypedDict(
     "SecretTypeDef",
     {
         "name": str,
         "valueFrom": str,
     },
 )
@@ -1527,14 +1537,15 @@
         "resourceRequirements": List[ResourceRequirementTypeDef],
         "linuxParameters": LinuxParametersTypeDef,
         "logConfiguration": LogConfigurationTypeDef,
         "secrets": List[SecretTypeDef],
         "networkConfiguration": NetworkConfigurationTypeDef,
         "fargatePlatformConfiguration": FargatePlatformConfigurationTypeDef,
         "ephemeralStorage": EphemeralStorageTypeDef,
+        "runtimePlatform": RuntimePlatformTypeDef,
     },
     total=False,
 )
 
 ContainerPropertiesTypeDef = TypedDict(
     "ContainerPropertiesTypeDef",
     {
@@ -1555,14 +1566,15 @@
         "resourceRequirements": List[ResourceRequirementTypeDef],
         "linuxParameters": LinuxParametersTypeDef,
         "logConfiguration": LogConfigurationTypeDef,
         "secrets": List[SecretTypeDef],
         "networkConfiguration": NetworkConfigurationTypeDef,
         "fargatePlatformConfiguration": FargatePlatformConfigurationTypeDef,
         "ephemeralStorage": EphemeralStorageTypeDef,
+        "runtimePlatform": RuntimePlatformTypeDef,
     },
     total=False,
 )
 
 EksPropertiesOverrideTypeDef = TypedDict(
     "EksPropertiesOverrideTypeDef",
     {
```

### Comparing `types-aiobotocore-batch-2.5.2.post3/types_aiobotocore_batch/type_defs.pyi` & `types-aiobotocore-batch-2.5.4/types_aiobotocore_batch/type_defs.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -55,14 +55,15 @@
     "LaunchTemplateSpecificationTypeDef",
     "EphemeralStorageTypeDef",
     "FargatePlatformConfigurationTypeDef",
     "KeyValuePairTypeDef",
     "MountPointTypeDef",
     "NetworkConfigurationTypeDef",
     "ResourceRequirementTypeDef",
+    "RuntimePlatformTypeDef",
     "SecretTypeDef",
     "UlimitTypeDef",
     "ContainerSummaryTypeDef",
     "ResponseMetadataTypeDef",
     "DeleteComputeEnvironmentRequestRequestTypeDef",
     "DeleteJobQueueRequestRequestTypeDef",
     "DeleteSchedulingPolicyRequestRequestTypeDef",
@@ -308,14 +309,23 @@
     "ResourceRequirementTypeDef",
     {
         "value": str,
         "type": ResourceTypeType,
     },
 )
 
+RuntimePlatformTypeDef = TypedDict(
+    "RuntimePlatformTypeDef",
+    {
+        "operatingSystemFamily": str,
+        "cpuArchitecture": str,
+    },
+    total=False,
+)
+
 SecretTypeDef = TypedDict(
     "SecretTypeDef",
     {
         "name": str,
         "valueFrom": str,
     },
 )
@@ -1480,14 +1490,15 @@
         "resourceRequirements": List[ResourceRequirementTypeDef],
         "linuxParameters": LinuxParametersTypeDef,
         "logConfiguration": LogConfigurationTypeDef,
         "secrets": List[SecretTypeDef],
         "networkConfiguration": NetworkConfigurationTypeDef,
         "fargatePlatformConfiguration": FargatePlatformConfigurationTypeDef,
         "ephemeralStorage": EphemeralStorageTypeDef,
+        "runtimePlatform": RuntimePlatformTypeDef,
     },
     total=False,
 )
 
 ContainerPropertiesTypeDef = TypedDict(
     "ContainerPropertiesTypeDef",
     {
@@ -1508,14 +1519,15 @@
         "resourceRequirements": List[ResourceRequirementTypeDef],
         "linuxParameters": LinuxParametersTypeDef,
         "logConfiguration": LogConfigurationTypeDef,
         "secrets": List[SecretTypeDef],
         "networkConfiguration": NetworkConfigurationTypeDef,
         "fargatePlatformConfiguration": FargatePlatformConfigurationTypeDef,
         "ephemeralStorage": EphemeralStorageTypeDef,
+        "runtimePlatform": RuntimePlatformTypeDef,
     },
     total=False,
 )
 
 EksPropertiesOverrideTypeDef = TypedDict(
     "EksPropertiesOverrideTypeDef",
     {
```

### Comparing `types-aiobotocore-batch-2.5.2.post3/types_aiobotocore_batch.egg-info/PKG-INFO` & `types-aiobotocore-batch-2.5.4/types_aiobotocore_batch.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-batch
-Version: 2.5.2.post3
-Summary: Type annotations for aiobotocore.Batch 2.5.2 service generated with mypy-boto3-builder 7.17.2
+Version: 2.5.4
+Summary: Type annotations for aiobotocore.Batch 2.5.4 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_batch/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-batch.svg?color=blue)](https://pypi.org/project/types-aiobotocore-batch)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_batch/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-batch)](https://pepy.tech/project/types-aiobotocore-batch)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.Batch 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/batch.html#Batch)
+[aiobotocore.Batch 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/batch.html#Batch)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-batch-2.5.2.post3/types_aiobotocore_batch.egg-info/SOURCES.txt` & `types-aiobotocore-batch-2.5.4/types_aiobotocore_batch.egg-info/SOURCES.txt`

 * *Files identical despite different names*


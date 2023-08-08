# Comparing `tmp/types-aiobotocore-emr-containers-2.5.2.post3.tar.gz` & `tmp/types-aiobotocore-emr-containers-2.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-emr-containers-2.5.2.post3.tar", last modified: Fri Aug  4 12:37:41 2023, max compression
+gzip compressed data, was "types-aiobotocore-emr-containers-2.5.4.tar", last modified: Tue Aug  8 01:23:42 2023, max compression
```

## Comparing `types-aiobotocore-emr-containers-2.5.2.post3.tar` & `types-aiobotocore-emr-containers-2.5.4.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:37:41.943770 types-aiobotocore-emr-containers-2.5.2.post3/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-04 12:23:29.000000 types-aiobotocore-emr-containers-2.5.2.post3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    13816 2023-08-04 12:37:41.943770 types-aiobotocore-emr-containers-2.5.2.post3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    12271 2023-08-04 12:23:29.000000 types-aiobotocore-emr-containers-2.5.2.post3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-04 12:37:41.943770 types-aiobotocore-emr-containers-2.5.2.post3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2120 2023-08-04 12:23:29.000000 types-aiobotocore-emr-containers-2.5.2.post3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:37:41.935770 types-aiobotocore-emr-containers-2.5.2.post3/types_aiobotocore_emr_containers/
--rw-r--r--   0 runner    (1001) docker     (123)     1360 2023-08-04 12:23:29.000000 types-aiobotocore-emr-containers-2.5.2.post3/types_aiobotocore_emr_containers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1359 2023-08-04 12:23:29.000000 types-aiobotocore-emr-containers-2.5.2.post3/types_aiobotocore_emr_containers/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      969 2023-08-04 12:23:29.000000 types-aiobotocore-emr-containers-2.5.2.post3/types_aiobotocore_emr_containers/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19929 2023-08-04 12:23:29.000000 types-aiobotocore-emr-containers-2.5.2.post3/types_aiobotocore_emr_containers/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    19896 2023-08-04 12:23:29.000000 types-aiobotocore-emr-containers-2.5.2.post3/types_aiobotocore_emr_containers/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9274 2023-08-04 12:23:30.000000 types-aiobotocore-emr-containers-2.5.2.post3/types_aiobotocore_emr_containers/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     9272 2023-08-04 12:23:30.000000 types-aiobotocore-emr-containers-2.5.2.post3/types_aiobotocore_emr_containers/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     6553 2023-08-04 12:23:29.000000 types-aiobotocore-emr-containers-2.5.2.post3/types_aiobotocore_emr_containers/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     6546 2023-08-04 12:23:29.000000 types-aiobotocore-emr-containers-2.5.2.post3/types_aiobotocore_emr_containers/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 12:23:29.000000 types-aiobotocore-emr-containers-2.5.2.post3/types_aiobotocore_emr_containers/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    25955 2023-08-04 12:23:31.000000 types-aiobotocore-emr-containers-2.5.2.post3/types_aiobotocore_emr_containers/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    25924 2023-08-04 12:23:30.000000 types-aiobotocore-emr-containers-2.5.2.post3/types_aiobotocore_emr_containers/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-04 12:23:29.000000 types-aiobotocore-emr-containers-2.5.2.post3/types_aiobotocore_emr_containers/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:37:41.943770 types-aiobotocore-emr-containers-2.5.2.post3/types_aiobotocore_emr_containers.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    13816 2023-08-04 12:37:41.000000 types-aiobotocore-emr-containers-2.5.2.post3/types_aiobotocore_emr_containers.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      946 2023-08-04 12:37:41.000000 types-aiobotocore-emr-containers-2.5.2.post3/types_aiobotocore_emr_containers.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 12:37:41.000000 types-aiobotocore-emr-containers-2.5.2.post3/types_aiobotocore_emr_containers.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 12:37:41.000000 types-aiobotocore-emr-containers-2.5.2.post3/types_aiobotocore_emr_containers.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-04 12:37:41.000000 types-aiobotocore-emr-containers-2.5.2.post3/types_aiobotocore_emr_containers.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-08-04 12:37:41.000000 types-aiobotocore-emr-containers-2.5.2.post3/types_aiobotocore_emr_containers.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:23:42.430711 types-aiobotocore-emr-containers-2.5.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-08 01:10:54.000000 types-aiobotocore-emr-containers-2.5.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    13810 2023-08-08 01:23:42.430711 types-aiobotocore-emr-containers-2.5.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    12271 2023-08-08 01:10:54.000000 types-aiobotocore-emr-containers-2.5.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-08 01:23:42.430711 types-aiobotocore-emr-containers-2.5.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2114 2023-08-08 01:10:54.000000 types-aiobotocore-emr-containers-2.5.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:23:42.414711 types-aiobotocore-emr-containers-2.5.4/types_aiobotocore_emr_containers/
+-rw-r--r--   0 runner    (1001) docker     (123)     1360 2023-08-08 01:10:54.000000 types-aiobotocore-emr-containers-2.5.4/types_aiobotocore_emr_containers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1359 2023-08-08 01:10:54.000000 types-aiobotocore-emr-containers-2.5.4/types_aiobotocore_emr_containers/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      957 2023-08-08 01:10:54.000000 types-aiobotocore-emr-containers-2.5.4/types_aiobotocore_emr_containers/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19929 2023-08-08 01:10:54.000000 types-aiobotocore-emr-containers-2.5.4/types_aiobotocore_emr_containers/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19896 2023-08-08 01:10:54.000000 types-aiobotocore-emr-containers-2.5.4/types_aiobotocore_emr_containers/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9405 2023-08-08 01:10:55.000000 types-aiobotocore-emr-containers-2.5.4/types_aiobotocore_emr_containers/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9403 2023-08-08 01:10:55.000000 types-aiobotocore-emr-containers-2.5.4/types_aiobotocore_emr_containers/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     6553 2023-08-08 01:10:54.000000 types-aiobotocore-emr-containers-2.5.4/types_aiobotocore_emr_containers/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6546 2023-08-08 01:10:54.000000 types-aiobotocore-emr-containers-2.5.4/types_aiobotocore_emr_containers/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 01:10:54.000000 types-aiobotocore-emr-containers-2.5.4/types_aiobotocore_emr_containers/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    25955 2023-08-08 01:10:55.000000 types-aiobotocore-emr-containers-2.5.4/types_aiobotocore_emr_containers/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25924 2023-08-08 01:10:55.000000 types-aiobotocore-emr-containers-2.5.4/types_aiobotocore_emr_containers/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-08-08 01:10:54.000000 types-aiobotocore-emr-containers-2.5.4/types_aiobotocore_emr_containers/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:23:42.430711 types-aiobotocore-emr-containers-2.5.4/types_aiobotocore_emr_containers.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    13810 2023-08-08 01:23:42.000000 types-aiobotocore-emr-containers-2.5.4/types_aiobotocore_emr_containers.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      946 2023-08-08 01:23:42.000000 types-aiobotocore-emr-containers-2.5.4/types_aiobotocore_emr_containers.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 01:23:42.000000 types-aiobotocore-emr-containers-2.5.4/types_aiobotocore_emr_containers.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 01:23:42.000000 types-aiobotocore-emr-containers-2.5.4/types_aiobotocore_emr_containers.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-08 01:23:42.000000 types-aiobotocore-emr-containers-2.5.4/types_aiobotocore_emr_containers.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-08-08 01:23:42.000000 types-aiobotocore-emr-containers-2.5.4/types_aiobotocore_emr_containers.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-emr-containers-2.5.2.post3/LICENSE` & `types-aiobotocore-emr-containers-2.5.4/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-emr-containers-2.5.2.post3/PKG-INFO` & `types-aiobotocore-emr-containers-2.5.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-emr-containers
-Version: 2.5.2.post3
-Summary: Type annotations for aiobotocore.EMRContainers 2.5.2 service generated with mypy-boto3-builder 7.17.2
+Version: 2.5.4
+Summary: Type annotations for aiobotocore.EMRContainers 2.5.4 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_emr_containers/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-emr-containers.svg?color=blue)](https://pypi.org/project/types-aiobotocore-emr-containers)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_emr_containers/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-emr-containers)](https://pepy.tech/project/types-aiobotocore-emr-containers)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.EMRContainers 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr-containers.html#EMRContainers)
+[aiobotocore.EMRContainers 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr-containers.html#EMRContainers)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-emr-containers-2.5.2.post3/README.md` & `types-aiobotocore-emr-containers-2.5.4/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-emr-containers.svg?color=blue)](https://pypi.org/project/types-aiobotocore-emr-containers)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_emr_containers/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-emr-containers)](https://pepy.tech/project/types-aiobotocore-emr-containers)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.EMRContainers 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr-containers.html#EMRContainers)
+[aiobotocore.EMRContainers 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr-containers.html#EMRContainers)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-emr-containers-2.5.2.post3/setup.py` & `types-aiobotocore-emr-containers-2.5.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-emr-containers",
-    version="2.5.2.post3",
+    version="2.5.4",
     packages=["types_aiobotocore_emr_containers"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.EMRContainers 2.5.2 service generated with"
+        "Type annotations for aiobotocore.EMRContainers 2.5.4 service generated with"
         " mypy-boto3-builder 7.17.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
```

### Comparing `types-aiobotocore-emr-containers-2.5.2.post3/types_aiobotocore_emr_containers/__init__.py` & `types-aiobotocore-emr-containers-2.5.4/types_aiobotocore_emr_containers/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-emr-containers-2.5.2.post3/types_aiobotocore_emr_containers/__init__.pyi` & `types-aiobotocore-emr-containers-2.5.4/types_aiobotocore_emr_containers/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-emr-containers-2.5.2.post3/types_aiobotocore_emr_containers/__main__.py` & `types-aiobotocore-emr-containers-2.5.4/types_aiobotocore_emr_containers/__main__.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.EMRContainers 2.5.2\nVersion:        "
-        " 2.5.2.post3\nBuilder version: 7.17.2\nDocs:           "
+        "Type annotations for aiobotocore.EMRContainers 2.5.4\nVersion:         2.5.4\nBuilder"
+        " version: 7.17.2\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_emr_containers//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr-containers.html#EMRContainers\nOther"
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

### Comparing `types-aiobotocore-emr-containers-2.5.2.post3/types_aiobotocore_emr_containers/client.py` & `types-aiobotocore-emr-containers-2.5.4/types_aiobotocore_emr_containers/client.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-emr-containers-2.5.2.post3/types_aiobotocore_emr_containers/client.pyi` & `types-aiobotocore-emr-containers-2.5.4/types_aiobotocore_emr_containers/client.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-emr-containers-2.5.2.post3/types_aiobotocore_emr_containers/literals.py` & `types-aiobotocore-emr-containers-2.5.4/types_aiobotocore_emr_containers/literals.pyi`

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
     "ContainerProviderTypeType",
     "EndpointStateType",
     "FailureReasonType",
     "JobRunStateType",
     "ListJobRunsPaginatorName",
     "ListJobTemplatesPaginatorName",
@@ -34,15 +33,14 @@
     "EMRContainersServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "RegionName",
 )
 
-
 ContainerProviderTypeType = Literal["EKS"]
 EndpointStateType = Literal[
     "ACTIVE", "CREATING", "TERMINATED", "TERMINATED_WITH_ERRORS", "TERMINATING"
 ]
 FailureReasonType = Literal[
     "CLUSTER_UNAVAILABLE", "INTERNAL_ERROR", "USER_ERROR", "VALIDATION_ERROR"
 ]
@@ -68,14 +66,15 @@
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
@@ -171,14 +170,15 @@
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
@@ -257,26 +257,28 @@
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
@@ -420,23 +422,25 @@
     "sns",
     "sqs",
 ]
 PaginatorName = Literal[
     "list_job_runs", "list_job_templates", "list_managed_endpoints", "list_virtual_clusters"
 ]
 RegionName = Literal[
+    "af-south-1",
     "ap-east-1",
     "ap-northeast-1",
     "ap-northeast-2",
     "ap-south-1",
     "ap-southeast-1",
     "ap-southeast-2",
     "ca-central-1",
     "eu-central-1",
     "eu-north-1",
+    "eu-south-1",
     "eu-west-1",
     "eu-west-2",
     "eu-west-3",
     "me-south-1",
     "sa-east-1",
     "us-east-1",
     "us-east-2",
```

### Comparing `types-aiobotocore-emr-containers-2.5.2.post3/types_aiobotocore_emr_containers/literals.pyi` & `types-aiobotocore-emr-containers-2.5.4/types_aiobotocore_emr_containers/literals.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 import sys
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
+
 __all__ = (
     "ContainerProviderTypeType",
     "EndpointStateType",
     "FailureReasonType",
     "JobRunStateType",
     "ListJobRunsPaginatorName",
     "ListJobTemplatesPaginatorName",
@@ -33,14 +34,15 @@
     "EMRContainersServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "RegionName",
 )
 
+
 ContainerProviderTypeType = Literal["EKS"]
 EndpointStateType = Literal[
     "ACTIVE", "CREATING", "TERMINATED", "TERMINATED_WITH_ERRORS", "TERMINATING"
 ]
 FailureReasonType = Literal[
     "CLUSTER_UNAVAILABLE", "INTERNAL_ERROR", "USER_ERROR", "VALIDATION_ERROR"
 ]
@@ -66,14 +68,15 @@
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
@@ -169,14 +172,15 @@
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
@@ -255,26 +259,28 @@
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
@@ -418,23 +424,25 @@
     "sns",
     "sqs",
 ]
 PaginatorName = Literal[
     "list_job_runs", "list_job_templates", "list_managed_endpoints", "list_virtual_clusters"
 ]
 RegionName = Literal[
+    "af-south-1",
     "ap-east-1",
     "ap-northeast-1",
     "ap-northeast-2",
     "ap-south-1",
     "ap-southeast-1",
     "ap-southeast-2",
     "ca-central-1",
     "eu-central-1",
     "eu-north-1",
+    "eu-south-1",
     "eu-west-1",
     "eu-west-2",
     "eu-west-3",
     "me-south-1",
     "sa-east-1",
     "us-east-1",
     "us-east-2",
```

### Comparing `types-aiobotocore-emr-containers-2.5.2.post3/types_aiobotocore_emr_containers/paginator.py` & `types-aiobotocore-emr-containers-2.5.4/types_aiobotocore_emr_containers/paginator.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-emr-containers-2.5.2.post3/types_aiobotocore_emr_containers/paginator.pyi` & `types-aiobotocore-emr-containers-2.5.4/types_aiobotocore_emr_containers/paginator.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-emr-containers-2.5.2.post3/types_aiobotocore_emr_containers/type_defs.py` & `types-aiobotocore-emr-containers-2.5.4/types_aiobotocore_emr_containers/type_defs.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-emr-containers-2.5.2.post3/types_aiobotocore_emr_containers/type_defs.pyi` & `types-aiobotocore-emr-containers-2.5.4/types_aiobotocore_emr_containers/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-emr-containers-2.5.2.post3/types_aiobotocore_emr_containers.egg-info/PKG-INFO` & `types-aiobotocore-emr-containers-2.5.4/types_aiobotocore_emr_containers.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-emr-containers
-Version: 2.5.2.post3
-Summary: Type annotations for aiobotocore.EMRContainers 2.5.2 service generated with mypy-boto3-builder 7.17.2
+Version: 2.5.4
+Summary: Type annotations for aiobotocore.EMRContainers 2.5.4 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_emr_containers/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-emr-containers.svg?color=blue)](https://pypi.org/project/types-aiobotocore-emr-containers)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_emr_containers/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-emr-containers)](https://pepy.tech/project/types-aiobotocore-emr-containers)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.EMRContainers 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr-containers.html#EMRContainers)
+[aiobotocore.EMRContainers 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr-containers.html#EMRContainers)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-emr-containers-2.5.2.post3/types_aiobotocore_emr_containers.egg-info/SOURCES.txt` & `types-aiobotocore-emr-containers-2.5.4/types_aiobotocore_emr_containers.egg-info/SOURCES.txt`

 * *Files identical despite different names*


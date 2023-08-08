# Comparing `tmp/types-aiobotocore-drs-2.5.2.post3.tar.gz` & `tmp/types-aiobotocore-drs-2.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-drs-2.5.2.post3.tar", last modified: Fri Aug  4 12:37:36 2023, max compression
+gzip compressed data, was "types-aiobotocore-drs-2.5.4.tar", last modified: Tue Aug  8 01:23:38 2023, max compression
```

## Comparing `types-aiobotocore-drs-2.5.2.post3.tar` & `types-aiobotocore-drs-2.5.4.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:37:36.791648 types-aiobotocore-drs-2.5.2.post3/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-04 12:21:45.000000 types-aiobotocore-drs-2.5.2.post3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    14400 2023-08-04 12:37:36.791648 types-aiobotocore-drs-2.5.2.post3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    12898 2023-08-04 12:21:45.000000 types-aiobotocore-drs-2.5.2.post3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-04 12:37:36.791648 types-aiobotocore-drs-2.5.2.post3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2020 2023-08-04 12:21:45.000000 types-aiobotocore-drs-2.5.2.post3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:37:36.787649 types-aiobotocore-drs-2.5.2.post3/types_aiobotocore_drs/
--rw-r--r--   0 runner    (1001) docker     (123)     3017 2023-08-04 12:21:45.000000 types-aiobotocore-drs-2.5.2.post3/types_aiobotocore_drs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3016 2023-08-04 12:21:45.000000 types-aiobotocore-drs-2.5.2.post3/types_aiobotocore_drs/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      916 2023-08-04 12:21:45.000000 types-aiobotocore-drs-2.5.2.post3/types_aiobotocore_drs/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    41944 2023-08-04 12:21:45.000000 types-aiobotocore-drs-2.5.2.post3/types_aiobotocore_drs/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    41878 2023-08-04 12:21:45.000000 types-aiobotocore-drs-2.5.2.post3/types_aiobotocore_drs/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    17043 2023-08-04 12:21:45.000000 types-aiobotocore-drs-2.5.2.post3/types_aiobotocore_drs/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    17041 2023-08-04 12:21:45.000000 types-aiobotocore-drs-2.5.2.post3/types_aiobotocore_drs/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    13548 2023-08-04 12:21:45.000000 types-aiobotocore-drs-2.5.2.post3/types_aiobotocore_drs/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)    13536 2023-08-04 12:21:45.000000 types-aiobotocore-drs-2.5.2.post3/types_aiobotocore_drs/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 12:21:45.000000 types-aiobotocore-drs-2.5.2.post3/types_aiobotocore_drs/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    56844 2023-08-04 12:21:46.000000 types-aiobotocore-drs-2.5.2.post3/types_aiobotocore_drs/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    56797 2023-08-04 12:21:46.000000 types-aiobotocore-drs-2.5.2.post3/types_aiobotocore_drs/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-04 12:21:45.000000 types-aiobotocore-drs-2.5.2.post3/types_aiobotocore_drs/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:37:36.791648 types-aiobotocore-drs-2.5.2.post3/types_aiobotocore_drs.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    14400 2023-08-04 12:37:36.000000 types-aiobotocore-drs-2.5.2.post3/types_aiobotocore_drs.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      737 2023-08-04 12:37:36.000000 types-aiobotocore-drs-2.5.2.post3/types_aiobotocore_drs.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 12:37:36.000000 types-aiobotocore-drs-2.5.2.post3/types_aiobotocore_drs.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 12:37:36.000000 types-aiobotocore-drs-2.5.2.post3/types_aiobotocore_drs.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-04 12:37:36.000000 types-aiobotocore-drs-2.5.2.post3/types_aiobotocore_drs.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-08-04 12:37:36.000000 types-aiobotocore-drs-2.5.2.post3/types_aiobotocore_drs.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:23:38.262693 types-aiobotocore-drs-2.5.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-08 01:09:19.000000 types-aiobotocore-drs-2.5.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    14394 2023-08-08 01:23:38.262693 types-aiobotocore-drs-2.5.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    12898 2023-08-08 01:09:19.000000 types-aiobotocore-drs-2.5.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-08 01:23:38.262693 types-aiobotocore-drs-2.5.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2014 2023-08-08 01:09:19.000000 types-aiobotocore-drs-2.5.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:23:38.262693 types-aiobotocore-drs-2.5.4/types_aiobotocore_drs/
+-rw-r--r--   0 runner    (1001) docker     (123)     3017 2023-08-08 01:09:19.000000 types-aiobotocore-drs-2.5.4/types_aiobotocore_drs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3016 2023-08-08 01:09:19.000000 types-aiobotocore-drs-2.5.4/types_aiobotocore_drs/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      904 2023-08-08 01:09:19.000000 types-aiobotocore-drs-2.5.4/types_aiobotocore_drs/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41944 2023-08-08 01:09:19.000000 types-aiobotocore-drs-2.5.4/types_aiobotocore_drs/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41878 2023-08-08 01:09:19.000000 types-aiobotocore-drs-2.5.4/types_aiobotocore_drs/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    17246 2023-08-08 01:09:20.000000 types-aiobotocore-drs-2.5.4/types_aiobotocore_drs/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17244 2023-08-08 01:09:20.000000 types-aiobotocore-drs-2.5.4/types_aiobotocore_drs/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    13548 2023-08-08 01:09:20.000000 types-aiobotocore-drs-2.5.4/types_aiobotocore_drs/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13536 2023-08-08 01:09:19.000000 types-aiobotocore-drs-2.5.4/types_aiobotocore_drs/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 01:09:19.000000 types-aiobotocore-drs-2.5.4/types_aiobotocore_drs/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    56844 2023-08-08 01:09:21.000000 types-aiobotocore-drs-2.5.4/types_aiobotocore_drs/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    56797 2023-08-08 01:09:20.000000 types-aiobotocore-drs-2.5.4/types_aiobotocore_drs/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-08-08 01:09:19.000000 types-aiobotocore-drs-2.5.4/types_aiobotocore_drs/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:23:38.262693 types-aiobotocore-drs-2.5.4/types_aiobotocore_drs.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    14394 2023-08-08 01:23:38.000000 types-aiobotocore-drs-2.5.4/types_aiobotocore_drs.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      737 2023-08-08 01:23:38.000000 types-aiobotocore-drs-2.5.4/types_aiobotocore_drs.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 01:23:38.000000 types-aiobotocore-drs-2.5.4/types_aiobotocore_drs.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 01:23:38.000000 types-aiobotocore-drs-2.5.4/types_aiobotocore_drs.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-08 01:23:38.000000 types-aiobotocore-drs-2.5.4/types_aiobotocore_drs.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-08-08 01:23:38.000000 types-aiobotocore-drs-2.5.4/types_aiobotocore_drs.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-drs-2.5.2.post3/LICENSE` & `types-aiobotocore-drs-2.5.4/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-drs-2.5.2.post3/PKG-INFO` & `types-aiobotocore-drs-2.5.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-drs
-Version: 2.5.2.post3
-Summary: Type annotations for aiobotocore.drs 2.5.2 service generated with mypy-boto3-builder 7.17.2
+Version: 2.5.4
+Summary: Type annotations for aiobotocore.drs 2.5.4 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_drs/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-drs.svg?color=blue)](https://pypi.org/project/types-aiobotocore-drs)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_drs/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-drs)](https://pepy.tech/project/types-aiobotocore-drs)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.drs 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/drs.html#drs)
+[aiobotocore.drs 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/drs.html#drs)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-drs-2.5.2.post3/README.md` & `types-aiobotocore-drs-2.5.4/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-drs.svg?color=blue)](https://pypi.org/project/types-aiobotocore-drs)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_drs/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-drs)](https://pepy.tech/project/types-aiobotocore-drs)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.drs 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/drs.html#drs)
+[aiobotocore.drs 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/drs.html#drs)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-drs-2.5.2.post3/setup.py` & `types-aiobotocore-drs-2.5.4/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-drs",
-    version="2.5.2.post3",
+    version="2.5.4",
     packages=["types_aiobotocore_drs"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.drs 2.5.2 service generated with mypy-boto3-builder"
+        "Type annotations for aiobotocore.drs 2.5.4 service generated with mypy-boto3-builder"
         " 7.17.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
```

### Comparing `types-aiobotocore-drs-2.5.2.post3/types_aiobotocore_drs/__init__.py` & `types-aiobotocore-drs-2.5.4/types_aiobotocore_drs/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-drs-2.5.2.post3/types_aiobotocore_drs/__init__.pyi` & `types-aiobotocore-drs-2.5.4/types_aiobotocore_drs/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-drs-2.5.2.post3/types_aiobotocore_drs/__main__.py` & `types-aiobotocore-drs-2.5.4/types_aiobotocore_drs/__main__.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.drs 2.5.2\nVersion:         2.5.2.post3\nBuilder version:"
+        "Type annotations for aiobotocore.drs 2.5.4\nVersion:         2.5.4\nBuilder version:"
         " 7.17.2\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_drs//\nBoto3 docs:    "
         "  https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/drs.html#drs\nOther"
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

### Comparing `types-aiobotocore-drs-2.5.2.post3/types_aiobotocore_drs/client.py` & `types-aiobotocore-drs-2.5.4/types_aiobotocore_drs/client.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-drs-2.5.2.post3/types_aiobotocore_drs/client.pyi` & `types-aiobotocore-drs-2.5.4/types_aiobotocore_drs/client.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-drs-2.5.2.post3/types_aiobotocore_drs/literals.py` & `types-aiobotocore-drs-2.5.4/types_aiobotocore_drs/literals.py`

 * *Files 0% similar despite different names*

```diff
@@ -263,15 +263,15 @@
 ReplicationConfigurationDefaultLargeStagingDiskTypeType = Literal["AUTO", "GP2", "GP3", "ST1"]
 ReplicationConfigurationEbsEncryptionType = Literal["CUSTOM", "DEFAULT", "NONE"]
 ReplicationConfigurationReplicatedDiskStagingDiskTypeType = Literal[
     "AUTO", "GP2", "GP3", "IO1", "SC1", "ST1", "STANDARD"
 ]
 ReplicationDirectionType = Literal["FAILBACK", "FAILOVER"]
 ReplicationStatusType = Literal["ERROR", "IN_PROGRESS", "PROTECTED", "STOPPED"]
-TargetInstanceTypeRightSizingMethodType = Literal["BASIC", "NONE"]
+TargetInstanceTypeRightSizingMethodType = Literal["BASIC", "IN_AWS", "NONE"]
 drsServiceName = Literal["drs"]
 ServiceName = Literal[
     "accessanalyzer",
     "account",
     "acm",
     "acm-pca",
     "alexaforbusiness",
@@ -280,14 +280,15 @@
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
@@ -383,14 +384,15 @@
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
@@ -469,26 +471,28 @@
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
@@ -647,24 +651,29 @@
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

### Comparing `types-aiobotocore-drs-2.5.2.post3/types_aiobotocore_drs/literals.pyi` & `types-aiobotocore-drs-2.5.4/types_aiobotocore_drs/literals.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -261,15 +261,15 @@
 ReplicationConfigurationDefaultLargeStagingDiskTypeType = Literal["AUTO", "GP2", "GP3", "ST1"]
 ReplicationConfigurationEbsEncryptionType = Literal["CUSTOM", "DEFAULT", "NONE"]
 ReplicationConfigurationReplicatedDiskStagingDiskTypeType = Literal[
     "AUTO", "GP2", "GP3", "IO1", "SC1", "ST1", "STANDARD"
 ]
 ReplicationDirectionType = Literal["FAILBACK", "FAILOVER"]
 ReplicationStatusType = Literal["ERROR", "IN_PROGRESS", "PROTECTED", "STOPPED"]
-TargetInstanceTypeRightSizingMethodType = Literal["BASIC", "NONE"]
+TargetInstanceTypeRightSizingMethodType = Literal["BASIC", "IN_AWS", "NONE"]
 drsServiceName = Literal["drs"]
 ServiceName = Literal[
     "accessanalyzer",
     "account",
     "acm",
     "acm-pca",
     "alexaforbusiness",
@@ -278,14 +278,15 @@
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
@@ -381,14 +382,15 @@
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
@@ -467,26 +469,28 @@
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
@@ -645,24 +649,29 @@
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

### Comparing `types-aiobotocore-drs-2.5.2.post3/types_aiobotocore_drs/paginator.py` & `types-aiobotocore-drs-2.5.4/types_aiobotocore_drs/paginator.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-drs-2.5.2.post3/types_aiobotocore_drs/paginator.pyi` & `types-aiobotocore-drs-2.5.4/types_aiobotocore_drs/paginator.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-drs-2.5.2.post3/types_aiobotocore_drs/type_defs.py` & `types-aiobotocore-drs-2.5.4/types_aiobotocore_drs/type_defs.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-drs-2.5.2.post3/types_aiobotocore_drs/type_defs.pyi` & `types-aiobotocore-drs-2.5.4/types_aiobotocore_drs/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-drs-2.5.2.post3/types_aiobotocore_drs.egg-info/PKG-INFO` & `types-aiobotocore-drs-2.5.4/types_aiobotocore_drs.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-drs
-Version: 2.5.2.post3
-Summary: Type annotations for aiobotocore.drs 2.5.2 service generated with mypy-boto3-builder 7.17.2
+Version: 2.5.4
+Summary: Type annotations for aiobotocore.drs 2.5.4 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_drs/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-drs.svg?color=blue)](https://pypi.org/project/types-aiobotocore-drs)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_drs/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-drs)](https://pepy.tech/project/types-aiobotocore-drs)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.drs 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/drs.html#drs)
+[aiobotocore.drs 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/drs.html#drs)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-drs-2.5.2.post3/types_aiobotocore_drs.egg-info/SOURCES.txt` & `types-aiobotocore-drs-2.5.4/types_aiobotocore_drs.egg-info/SOURCES.txt`

 * *Files identical despite different names*


# Comparing `tmp/types-aiobotocore-docdb-2.5.2.post3.tar.gz` & `tmp/types-aiobotocore-docdb-2.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-docdb-2.5.2.post3.tar", last modified: Fri Aug  4 12:37:36 2023, max compression
+gzip compressed data, was "types-aiobotocore-docdb-2.5.4.tar", last modified: Tue Aug  8 01:23:37 2023, max compression
```

## Comparing `types-aiobotocore-docdb-2.5.2.post3.tar` & `types-aiobotocore-docdb-2.5.4.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:37:36.823649 types-aiobotocore-docdb-2.5.2.post3/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-04 12:21:40.000000 types-aiobotocore-docdb-2.5.2.post3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    15951 2023-08-04 12:37:36.819649 types-aiobotocore-docdb-2.5.2.post3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    14441 2023-08-04 12:21:40.000000 types-aiobotocore-docdb-2.5.2.post3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-04 12:37:36.823649 types-aiobotocore-docdb-2.5.2.post3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2058 2023-08-04 12:21:40.000000 types-aiobotocore-docdb-2.5.2.post3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:37:36.819649 types-aiobotocore-docdb-2.5.2.post3/types_aiobotocore_docdb/
--rw-r--r--   0 runner    (1001) docker     (123)     4193 2023-08-04 12:21:40.000000 types-aiobotocore-docdb-2.5.2.post3/types_aiobotocore_docdb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4192 2023-08-04 12:21:40.000000 types-aiobotocore-docdb-2.5.2.post3/types_aiobotocore_docdb/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      924 2023-08-04 12:21:40.000000 types-aiobotocore-docdb-2.5.2.post3/types_aiobotocore_docdb/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    53689 2023-08-04 12:21:41.000000 types-aiobotocore-docdb-2.5.2.post3/types_aiobotocore_docdb/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    53612 2023-08-04 12:21:40.000000 types-aiobotocore-docdb-2.5.2.post3/types_aiobotocore_docdb/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    10731 2023-08-04 12:21:41.000000 types-aiobotocore-docdb-2.5.2.post3/types_aiobotocore_docdb/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    10729 2023-08-04 12:21:41.000000 types-aiobotocore-docdb-2.5.2.post3/types_aiobotocore_docdb/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    18071 2023-08-04 12:21:41.000000 types-aiobotocore-docdb-2.5.2.post3/types_aiobotocore_docdb/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)    18056 2023-08-04 12:21:41.000000 types-aiobotocore-docdb-2.5.2.post3/types_aiobotocore_docdb/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 12:21:40.000000 types-aiobotocore-docdb-2.5.2.post3/types_aiobotocore_docdb/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    60489 2023-08-04 12:21:42.000000 types-aiobotocore-docdb-2.5.2.post3/types_aiobotocore_docdb/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    60436 2023-08-04 12:21:42.000000 types-aiobotocore-docdb-2.5.2.post3/types_aiobotocore_docdb/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-04 12:21:40.000000 types-aiobotocore-docdb-2.5.2.post3/types_aiobotocore_docdb/version.py
--rw-r--r--   0 runner    (1001) docker     (123)     2863 2023-08-04 12:21:41.000000 types-aiobotocore-docdb-2.5.2.post3/types_aiobotocore_docdb/waiter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2861 2023-08-04 12:21:41.000000 types-aiobotocore-docdb-2.5.2.post3/types_aiobotocore_docdb/waiter.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:37:36.819649 types-aiobotocore-docdb-2.5.2.post3/types_aiobotocore_docdb.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    15951 2023-08-04 12:37:36.000000 types-aiobotocore-docdb-2.5.2.post3/types_aiobotocore_docdb.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      844 2023-08-04 12:37:36.000000 types-aiobotocore-docdb-2.5.2.post3/types_aiobotocore_docdb.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 12:37:36.000000 types-aiobotocore-docdb-2.5.2.post3/types_aiobotocore_docdb.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 12:37:36.000000 types-aiobotocore-docdb-2.5.2.post3/types_aiobotocore_docdb.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-04 12:37:36.000000 types-aiobotocore-docdb-2.5.2.post3/types_aiobotocore_docdb.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-08-04 12:37:36.000000 types-aiobotocore-docdb-2.5.2.post3/types_aiobotocore_docdb.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:23:37.686691 types-aiobotocore-docdb-2.5.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-08 01:09:15.000000 types-aiobotocore-docdb-2.5.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    15945 2023-08-08 01:23:37.686691 types-aiobotocore-docdb-2.5.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    14441 2023-08-08 01:09:15.000000 types-aiobotocore-docdb-2.5.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-08 01:23:37.686691 types-aiobotocore-docdb-2.5.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2052 2023-08-08 01:09:15.000000 types-aiobotocore-docdb-2.5.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:23:37.674691 types-aiobotocore-docdb-2.5.4/types_aiobotocore_docdb/
+-rw-r--r--   0 runner    (1001) docker     (123)     4193 2023-08-08 01:09:15.000000 types-aiobotocore-docdb-2.5.4/types_aiobotocore_docdb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4192 2023-08-08 01:09:15.000000 types-aiobotocore-docdb-2.5.4/types_aiobotocore_docdb/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      912 2023-08-08 01:09:15.000000 types-aiobotocore-docdb-2.5.4/types_aiobotocore_docdb/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    53735 2023-08-08 01:09:15.000000 types-aiobotocore-docdb-2.5.4/types_aiobotocore_docdb/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    53658 2023-08-08 01:09:15.000000 types-aiobotocore-docdb-2.5.4/types_aiobotocore_docdb/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    10846 2023-08-08 01:09:16.000000 types-aiobotocore-docdb-2.5.4/types_aiobotocore_docdb/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10844 2023-08-08 01:09:16.000000 types-aiobotocore-docdb-2.5.4/types_aiobotocore_docdb/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    18071 2023-08-08 01:09:16.000000 types-aiobotocore-docdb-2.5.4/types_aiobotocore_docdb/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18056 2023-08-08 01:09:16.000000 types-aiobotocore-docdb-2.5.4/types_aiobotocore_docdb/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 01:09:15.000000 types-aiobotocore-docdb-2.5.4/types_aiobotocore_docdb/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    60531 2023-08-08 01:09:17.000000 types-aiobotocore-docdb-2.5.4/types_aiobotocore_docdb/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    60478 2023-08-08 01:09:16.000000 types-aiobotocore-docdb-2.5.4/types_aiobotocore_docdb/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-08-08 01:09:15.000000 types-aiobotocore-docdb-2.5.4/types_aiobotocore_docdb/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2863 2023-08-08 01:09:16.000000 types-aiobotocore-docdb-2.5.4/types_aiobotocore_docdb/waiter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2861 2023-08-08 01:09:16.000000 types-aiobotocore-docdb-2.5.4/types_aiobotocore_docdb/waiter.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:23:37.686691 types-aiobotocore-docdb-2.5.4/types_aiobotocore_docdb.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    15945 2023-08-08 01:23:37.000000 types-aiobotocore-docdb-2.5.4/types_aiobotocore_docdb.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      844 2023-08-08 01:23:37.000000 types-aiobotocore-docdb-2.5.4/types_aiobotocore_docdb.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 01:23:37.000000 types-aiobotocore-docdb-2.5.4/types_aiobotocore_docdb.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 01:23:37.000000 types-aiobotocore-docdb-2.5.4/types_aiobotocore_docdb.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-08 01:23:37.000000 types-aiobotocore-docdb-2.5.4/types_aiobotocore_docdb.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-08-08 01:23:37.000000 types-aiobotocore-docdb-2.5.4/types_aiobotocore_docdb.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-docdb-2.5.2.post3/LICENSE` & `types-aiobotocore-docdb-2.5.4/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-docdb-2.5.2.post3/PKG-INFO` & `types-aiobotocore-docdb-2.5.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-docdb
-Version: 2.5.2.post3
-Summary: Type annotations for aiobotocore.DocDB 2.5.2 service generated with mypy-boto3-builder 7.17.2
+Version: 2.5.4
+Summary: Type annotations for aiobotocore.DocDB 2.5.4 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_docdb/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-docdb.svg?color=blue)](https://pypi.org/project/types-aiobotocore-docdb)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_docdb/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-docdb)](https://pepy.tech/project/types-aiobotocore-docdb)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.DocDB 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/docdb.html#DocDB)
+[aiobotocore.DocDB 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/docdb.html#DocDB)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-docdb-2.5.2.post3/README.md` & `types-aiobotocore-docdb-2.5.4/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-docdb.svg?color=blue)](https://pypi.org/project/types-aiobotocore-docdb)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_docdb/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-docdb)](https://pepy.tech/project/types-aiobotocore-docdb)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.DocDB 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/docdb.html#DocDB)
+[aiobotocore.DocDB 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/docdb.html#DocDB)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-docdb-2.5.2.post3/setup.py` & `types-aiobotocore-docdb-2.5.4/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-docdb",
-    version="2.5.2.post3",
+    version="2.5.4",
     packages=["types_aiobotocore_docdb"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.DocDB 2.5.2 service generated with mypy-boto3-builder"
+        "Type annotations for aiobotocore.DocDB 2.5.4 service generated with mypy-boto3-builder"
         " 7.17.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
```

### Comparing `types-aiobotocore-docdb-2.5.2.post3/types_aiobotocore_docdb/__init__.py` & `types-aiobotocore-docdb-2.5.4/types_aiobotocore_docdb/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-docdb-2.5.2.post3/types_aiobotocore_docdb/__init__.pyi` & `types-aiobotocore-docdb-2.5.4/types_aiobotocore_docdb/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-docdb-2.5.2.post3/types_aiobotocore_docdb/client.py` & `types-aiobotocore-docdb-2.5.4/types_aiobotocore_docdb/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -779,14 +779,15 @@
         VpcSecurityGroupIds: Sequence[str] = ...,
         Port: int = ...,
         MasterUserPassword: str = ...,
         PreferredBackupWindow: str = ...,
         PreferredMaintenanceWindow: str = ...,
         CloudwatchLogsExportConfiguration: CloudwatchLogsExportConfigurationTypeDef = ...,
         EngineVersion: str = ...,
+        AllowMajorVersionUpgrade: bool = ...,
         DeletionProtection: bool = ...
     ) -> ModifyDBClusterResultTypeDef:
         """
         Modifies a setting for an Amazon DocumentDB cluster.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/docdb.html#DocDB.Client.modify_db_cluster)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_docdb/client/#modify_db_cluster)
```

### Comparing `types-aiobotocore-docdb-2.5.2.post3/types_aiobotocore_docdb/client.pyi` & `types-aiobotocore-docdb-2.5.4/types_aiobotocore_docdb/client.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -734,14 +734,15 @@
         VpcSecurityGroupIds: Sequence[str] = ...,
         Port: int = ...,
         MasterUserPassword: str = ...,
         PreferredBackupWindow: str = ...,
         PreferredMaintenanceWindow: str = ...,
         CloudwatchLogsExportConfiguration: CloudwatchLogsExportConfigurationTypeDef = ...,
         EngineVersion: str = ...,
+        AllowMajorVersionUpgrade: bool = ...,
         DeletionProtection: bool = ...
     ) -> ModifyDBClusterResultTypeDef:
         """
         Modifies a setting for an Amazon DocumentDB cluster.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/docdb.html#DocDB.Client.modify_db_cluster)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_docdb/client/#modify_db_cluster)
```

### Comparing `types-aiobotocore-docdb-2.5.2.post3/types_aiobotocore_docdb/literals.py` & `types-aiobotocore-docdb-2.5.4/types_aiobotocore_docdb/literals.py`

 * *Files 1% similar despite different names*

```diff
@@ -82,14 +82,15 @@
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
@@ -185,14 +186,15 @@
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
@@ -271,26 +273,28 @@
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
@@ -467,14 +471,15 @@
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

### Comparing `types-aiobotocore-docdb-2.5.2.post3/types_aiobotocore_docdb/literals.pyi` & `types-aiobotocore-docdb-2.5.4/types_aiobotocore_docdb/literals.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -80,14 +80,15 @@
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
@@ -183,14 +184,15 @@
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
@@ -269,26 +271,28 @@
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
@@ -465,14 +469,15 @@
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

### Comparing `types-aiobotocore-docdb-2.5.2.post3/types_aiobotocore_docdb/paginator.py` & `types-aiobotocore-docdb-2.5.4/types_aiobotocore_docdb/paginator.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-docdb-2.5.2.post3/types_aiobotocore_docdb/paginator.pyi` & `types-aiobotocore-docdb-2.5.4/types_aiobotocore_docdb/paginator.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-docdb-2.5.2.post3/types_aiobotocore_docdb/type_defs.py` & `types-aiobotocore-docdb-2.5.4/types_aiobotocore_docdb/type_defs.py`

 * *Files 0% similar despite different names*

```diff
@@ -1140,14 +1140,15 @@
         "VpcSecurityGroupIds": Sequence[str],
         "Port": int,
         "MasterUserPassword": str,
         "PreferredBackupWindow": str,
         "PreferredMaintenanceWindow": str,
         "CloudwatchLogsExportConfiguration": CloudwatchLogsExportConfigurationTypeDef,
         "EngineVersion": str,
+        "AllowMajorVersionUpgrade": bool,
         "DeletionProtection": bool,
     },
     total=False,
 )
 
 
 class ModifyDBClusterMessageRequestTypeDef(
```

### Comparing `types-aiobotocore-docdb-2.5.2.post3/types_aiobotocore_docdb/type_defs.pyi` & `types-aiobotocore-docdb-2.5.4/types_aiobotocore_docdb/type_defs.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -1105,14 +1105,15 @@
         "VpcSecurityGroupIds": Sequence[str],
         "Port": int,
         "MasterUserPassword": str,
         "PreferredBackupWindow": str,
         "PreferredMaintenanceWindow": str,
         "CloudwatchLogsExportConfiguration": CloudwatchLogsExportConfigurationTypeDef,
         "EngineVersion": str,
+        "AllowMajorVersionUpgrade": bool,
         "DeletionProtection": bool,
     },
     total=False,
 )
 
 class ModifyDBClusterMessageRequestTypeDef(
     _RequiredModifyDBClusterMessageRequestTypeDef, _OptionalModifyDBClusterMessageRequestTypeDef
```

### Comparing `types-aiobotocore-docdb-2.5.2.post3/types_aiobotocore_docdb/waiter.py` & `types-aiobotocore-docdb-2.5.4/types_aiobotocore_docdb/waiter.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-docdb-2.5.2.post3/types_aiobotocore_docdb/waiter.pyi` & `types-aiobotocore-docdb-2.5.4/types_aiobotocore_docdb/waiter.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-docdb-2.5.2.post3/types_aiobotocore_docdb.egg-info/PKG-INFO` & `types-aiobotocore-docdb-2.5.4/types_aiobotocore_docdb.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-docdb
-Version: 2.5.2.post3
-Summary: Type annotations for aiobotocore.DocDB 2.5.2 service generated with mypy-boto3-builder 7.17.2
+Version: 2.5.4
+Summary: Type annotations for aiobotocore.DocDB 2.5.4 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_docdb/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-docdb.svg?color=blue)](https://pypi.org/project/types-aiobotocore-docdb)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_docdb/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-docdb)](https://pepy.tech/project/types-aiobotocore-docdb)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.DocDB 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/docdb.html#DocDB)
+[aiobotocore.DocDB 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/docdb.html#DocDB)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-docdb-2.5.2.post3/types_aiobotocore_docdb.egg-info/SOURCES.txt` & `types-aiobotocore-docdb-2.5.4/types_aiobotocore_docdb.egg-info/SOURCES.txt`

 * *Files identical despite different names*


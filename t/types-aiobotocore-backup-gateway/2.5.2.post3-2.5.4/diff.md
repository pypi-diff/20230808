# Comparing `tmp/types-aiobotocore-backup-gateway-2.5.2.post3.tar.gz` & `tmp/types-aiobotocore-backup-gateway-2.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-backup-gateway-2.5.2.post3.tar", last modified: Fri Aug  4 12:37:20 2023, max compression
+gzip compressed data, was "types-aiobotocore-backup-gateway-2.5.4.tar", last modified: Tue Aug  8 01:23:21 2023, max compression
```

## Comparing `types-aiobotocore-backup-gateway-2.5.2.post3.tar` & `types-aiobotocore-backup-gateway-2.5.4.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:37:20.079250 types-aiobotocore-backup-gateway-2.5.2.post3/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-04 12:18:55.000000 types-aiobotocore-backup-gateway-2.5.2.post3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    13632 2023-08-04 12:37:20.079250 types-aiobotocore-backup-gateway-2.5.2.post3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    12087 2023-08-04 12:18:55.000000 types-aiobotocore-backup-gateway-2.5.2.post3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-04 12:37:20.079250 types-aiobotocore-backup-gateway-2.5.2.post3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2120 2023-08-04 12:18:55.000000 types-aiobotocore-backup-gateway-2.5.2.post3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:37:20.079250 types-aiobotocore-backup-gateway-2.5.2.post3/types_aiobotocore_backup_gateway/
--rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-08-04 12:18:55.000000 types-aiobotocore-backup-gateway-2.5.2.post3/types_aiobotocore_backup_gateway/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1110 2023-08-04 12:18:55.000000 types-aiobotocore-backup-gateway-2.5.2.post3/types_aiobotocore_backup_gateway/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      969 2023-08-04 12:18:55.000000 types-aiobotocore-backup-gateway-2.5.2.post3/types_aiobotocore_backup_gateway/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    21669 2023-08-04 12:18:55.000000 types-aiobotocore-backup-gateway-2.5.2.post3/types_aiobotocore_backup_gateway/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    21632 2023-08-04 12:18:55.000000 types-aiobotocore-backup-gateway-2.5.2.post3/types_aiobotocore_backup_gateway/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8675 2023-08-04 12:18:55.000000 types-aiobotocore-backup-gateway-2.5.2.post3/types_aiobotocore_backup_gateway/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     8673 2023-08-04 12:18:55.000000 types-aiobotocore-backup-gateway-2.5.2.post3/types_aiobotocore_backup_gateway/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     4330 2023-08-04 12:18:55.000000 types-aiobotocore-backup-gateway-2.5.2.post3/types_aiobotocore_backup_gateway/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     4325 2023-08-04 12:18:55.000000 types-aiobotocore-backup-gateway-2.5.2.post3/types_aiobotocore_backup_gateway/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 12:18:55.000000 types-aiobotocore-backup-gateway-2.5.2.post3/types_aiobotocore_backup_gateway/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    19654 2023-08-04 12:18:56.000000 types-aiobotocore-backup-gateway-2.5.2.post3/types_aiobotocore_backup_gateway/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    19637 2023-08-04 12:18:55.000000 types-aiobotocore-backup-gateway-2.5.2.post3/types_aiobotocore_backup_gateway/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-04 12:18:55.000000 types-aiobotocore-backup-gateway-2.5.2.post3/types_aiobotocore_backup_gateway/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:37:20.079250 types-aiobotocore-backup-gateway-2.5.2.post3/types_aiobotocore_backup_gateway.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    13632 2023-08-04 12:37:19.000000 types-aiobotocore-backup-gateway-2.5.2.post3/types_aiobotocore_backup_gateway.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      946 2023-08-04 12:37:19.000000 types-aiobotocore-backup-gateway-2.5.2.post3/types_aiobotocore_backup_gateway.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 12:37:19.000000 types-aiobotocore-backup-gateway-2.5.2.post3/types_aiobotocore_backup_gateway.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 12:37:19.000000 types-aiobotocore-backup-gateway-2.5.2.post3/types_aiobotocore_backup_gateway.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-04 12:37:19.000000 types-aiobotocore-backup-gateway-2.5.2.post3/types_aiobotocore_backup_gateway.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-08-04 12:37:19.000000 types-aiobotocore-backup-gateway-2.5.2.post3/types_aiobotocore_backup_gateway.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:23:21.658620 types-aiobotocore-backup-gateway-2.5.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-08 01:06:41.000000 types-aiobotocore-backup-gateway-2.5.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    13626 2023-08-08 01:23:21.658620 types-aiobotocore-backup-gateway-2.5.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    12087 2023-08-08 01:06:41.000000 types-aiobotocore-backup-gateway-2.5.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-08 01:23:21.658620 types-aiobotocore-backup-gateway-2.5.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2114 2023-08-08 01:06:41.000000 types-aiobotocore-backup-gateway-2.5.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:23:21.658620 types-aiobotocore-backup-gateway-2.5.4/types_aiobotocore_backup_gateway/
+-rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-08-08 01:06:41.000000 types-aiobotocore-backup-gateway-2.5.4/types_aiobotocore_backup_gateway/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1110 2023-08-08 01:06:41.000000 types-aiobotocore-backup-gateway-2.5.4/types_aiobotocore_backup_gateway/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      957 2023-08-08 01:06:41.000000 types-aiobotocore-backup-gateway-2.5.4/types_aiobotocore_backup_gateway/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21669 2023-08-08 01:06:41.000000 types-aiobotocore-backup-gateway-2.5.4/types_aiobotocore_backup_gateway/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21632 2023-08-08 01:06:41.000000 types-aiobotocore-backup-gateway-2.5.4/types_aiobotocore_backup_gateway/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8770 2023-08-08 01:06:41.000000 types-aiobotocore-backup-gateway-2.5.4/types_aiobotocore_backup_gateway/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8768 2023-08-08 01:06:41.000000 types-aiobotocore-backup-gateway-2.5.4/types_aiobotocore_backup_gateway/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     4330 2023-08-08 01:06:41.000000 types-aiobotocore-backup-gateway-2.5.4/types_aiobotocore_backup_gateway/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4325 2023-08-08 01:06:41.000000 types-aiobotocore-backup-gateway-2.5.4/types_aiobotocore_backup_gateway/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 01:06:41.000000 types-aiobotocore-backup-gateway-2.5.4/types_aiobotocore_backup_gateway/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    19654 2023-08-08 01:06:41.000000 types-aiobotocore-backup-gateway-2.5.4/types_aiobotocore_backup_gateway/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19637 2023-08-08 01:06:41.000000 types-aiobotocore-backup-gateway-2.5.4/types_aiobotocore_backup_gateway/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-08-08 01:06:41.000000 types-aiobotocore-backup-gateway-2.5.4/types_aiobotocore_backup_gateway/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:23:21.658620 types-aiobotocore-backup-gateway-2.5.4/types_aiobotocore_backup_gateway.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    13626 2023-08-08 01:23:21.000000 types-aiobotocore-backup-gateway-2.5.4/types_aiobotocore_backup_gateway.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      946 2023-08-08 01:23:21.000000 types-aiobotocore-backup-gateway-2.5.4/types_aiobotocore_backup_gateway.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 01:23:21.000000 types-aiobotocore-backup-gateway-2.5.4/types_aiobotocore_backup_gateway.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 01:23:21.000000 types-aiobotocore-backup-gateway-2.5.4/types_aiobotocore_backup_gateway.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-08 01:23:21.000000 types-aiobotocore-backup-gateway-2.5.4/types_aiobotocore_backup_gateway.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-08-08 01:23:21.000000 types-aiobotocore-backup-gateway-2.5.4/types_aiobotocore_backup_gateway.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-backup-gateway-2.5.2.post3/LICENSE` & `types-aiobotocore-backup-gateway-2.5.4/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-backup-gateway-2.5.2.post3/PKG-INFO` & `types-aiobotocore-backup-gateway-2.5.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-backup-gateway
-Version: 2.5.2.post3
-Summary: Type annotations for aiobotocore.BackupGateway 2.5.2 service generated with mypy-boto3-builder 7.17.2
+Version: 2.5.4
+Summary: Type annotations for aiobotocore.BackupGateway 2.5.4 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_backup_gateway/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-backup-gateway.svg?color=blue)](https://pypi.org/project/types-aiobotocore-backup-gateway)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_backup_gateway/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-backup-gateway)](https://pepy.tech/project/types-aiobotocore-backup-gateway)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.BackupGateway 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup-gateway.html#BackupGateway)
+[aiobotocore.BackupGateway 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup-gateway.html#BackupGateway)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-backup-gateway-2.5.2.post3/README.md` & `types-aiobotocore-backup-gateway-2.5.4/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-backup-gateway.svg?color=blue)](https://pypi.org/project/types-aiobotocore-backup-gateway)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_backup_gateway/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-backup-gateway)](https://pepy.tech/project/types-aiobotocore-backup-gateway)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.BackupGateway 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup-gateway.html#BackupGateway)
+[aiobotocore.BackupGateway 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup-gateway.html#BackupGateway)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-backup-gateway-2.5.2.post3/setup.py` & `types-aiobotocore-backup-gateway-2.5.4/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-backup-gateway",
-    version="2.5.2.post3",
+    version="2.5.4",
     packages=["types_aiobotocore_backup_gateway"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.BackupGateway 2.5.2 service generated with"
+        "Type annotations for aiobotocore.BackupGateway 2.5.4 service generated with"
         " mypy-boto3-builder 7.17.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
```

### Comparing `types-aiobotocore-backup-gateway-2.5.2.post3/types_aiobotocore_backup_gateway/__init__.py` & `types-aiobotocore-backup-gateway-2.5.4/types_aiobotocore_backup_gateway/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-backup-gateway-2.5.2.post3/types_aiobotocore_backup_gateway/__init__.pyi` & `types-aiobotocore-backup-gateway-2.5.4/types_aiobotocore_backup_gateway/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-backup-gateway-2.5.2.post3/types_aiobotocore_backup_gateway/__main__.py` & `types-aiobotocore-backup-gateway-2.5.4/types_aiobotocore_backup_gateway/__main__.py`

 * *Files 15% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.BackupGateway 2.5.2\nVersion:        "
-        " 2.5.2.post3\nBuilder version: 7.17.2\nDocs:           "
+        "Type annotations for aiobotocore.BackupGateway 2.5.4\nVersion:         2.5.4\nBuilder"
+        " version: 7.17.2\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_backup_gateway//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup-gateway.html#BackupGateway\nOther"
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

### Comparing `types-aiobotocore-backup-gateway-2.5.2.post3/types_aiobotocore_backup_gateway/client.py` & `types-aiobotocore-backup-gateway-2.5.4/types_aiobotocore_backup_gateway/client.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-backup-gateway-2.5.2.post3/types_aiobotocore_backup_gateway/client.pyi` & `types-aiobotocore-backup-gateway-2.5.4/types_aiobotocore_backup_gateway/client.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-backup-gateway-2.5.2.post3/types_aiobotocore_backup_gateway/literals.py` & `types-aiobotocore-backup-gateway-2.5.4/types_aiobotocore_backup_gateway/literals.py`

 * *Files 1% similar despite different names*

```diff
@@ -52,14 +52,15 @@
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
@@ -155,14 +156,15 @@
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
@@ -241,26 +243,28 @@
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

### Comparing `types-aiobotocore-backup-gateway-2.5.2.post3/types_aiobotocore_backup_gateway/literals.pyi` & `types-aiobotocore-backup-gateway-2.5.4/types_aiobotocore_backup_gateway/literals.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -50,14 +50,15 @@
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
@@ -153,14 +154,15 @@
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
@@ -239,26 +241,28 @@
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

### Comparing `types-aiobotocore-backup-gateway-2.5.2.post3/types_aiobotocore_backup_gateway/paginator.py` & `types-aiobotocore-backup-gateway-2.5.4/types_aiobotocore_backup_gateway/paginator.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-backup-gateway-2.5.2.post3/types_aiobotocore_backup_gateway/paginator.pyi` & `types-aiobotocore-backup-gateway-2.5.4/types_aiobotocore_backup_gateway/paginator.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-backup-gateway-2.5.2.post3/types_aiobotocore_backup_gateway/type_defs.py` & `types-aiobotocore-backup-gateway-2.5.4/types_aiobotocore_backup_gateway/type_defs.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-backup-gateway-2.5.2.post3/types_aiobotocore_backup_gateway/type_defs.pyi` & `types-aiobotocore-backup-gateway-2.5.4/types_aiobotocore_backup_gateway/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-backup-gateway-2.5.2.post3/types_aiobotocore_backup_gateway.egg-info/PKG-INFO` & `types-aiobotocore-backup-gateway-2.5.4/types_aiobotocore_backup_gateway.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-backup-gateway
-Version: 2.5.2.post3
-Summary: Type annotations for aiobotocore.BackupGateway 2.5.2 service generated with mypy-boto3-builder 7.17.2
+Version: 2.5.4
+Summary: Type annotations for aiobotocore.BackupGateway 2.5.4 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_backup_gateway/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-backup-gateway.svg?color=blue)](https://pypi.org/project/types-aiobotocore-backup-gateway)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_backup_gateway/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-backup-gateway)](https://pepy.tech/project/types-aiobotocore-backup-gateway)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.BackupGateway 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup-gateway.html#BackupGateway)
+[aiobotocore.BackupGateway 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup-gateway.html#BackupGateway)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-backup-gateway-2.5.2.post3/types_aiobotocore_backup_gateway.egg-info/SOURCES.txt` & `types-aiobotocore-backup-gateway-2.5.4/types_aiobotocore_backup_gateway.egg-info/SOURCES.txt`

 * *Files identical despite different names*


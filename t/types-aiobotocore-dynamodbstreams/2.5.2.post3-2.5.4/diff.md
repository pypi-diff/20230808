# Comparing `tmp/types-aiobotocore-dynamodbstreams-2.5.2.post3.tar.gz` & `tmp/types-aiobotocore-dynamodbstreams-2.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-dynamodbstreams-2.5.2.post3.tar", last modified: Fri Aug  4 12:37:38 2023, max compression
+gzip compressed data, was "types-aiobotocore-dynamodbstreams-2.5.4.tar", last modified: Tue Aug  8 01:23:38 2023, max compression
```

## Comparing `types-aiobotocore-dynamodbstreams-2.5.2.post3.tar` & `types-aiobotocore-dynamodbstreams-2.5.4.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:37:38.751695 types-aiobotocore-dynamodbstreams-2.5.2.post3/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-04 12:21:57.000000 types-aiobotocore-dynamodbstreams-2.5.2.post3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    12598 2023-08-04 12:37:38.751695 types-aiobotocore-dynamodbstreams-2.5.2.post3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    11048 2023-08-04 12:21:57.000000 types-aiobotocore-dynamodbstreams-2.5.2.post3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-04 12:37:38.751695 types-aiobotocore-dynamodbstreams-2.5.2.post3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2128 2023-08-04 12:21:57.000000 types-aiobotocore-dynamodbstreams-2.5.2.post3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:37:38.747695 types-aiobotocore-dynamodbstreams-2.5.2.post3/types_aiobotocore_dynamodbstreams/
--rw-r--r--   0 runner    (1001) docker     (123)      506 2023-08-04 12:21:57.000000 types-aiobotocore-dynamodbstreams-2.5.2.post3/types_aiobotocore_dynamodbstreams/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      505 2023-08-04 12:21:57.000000 types-aiobotocore-dynamodbstreams-2.5.2.post3/types_aiobotocore_dynamodbstreams/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      975 2023-08-04 12:21:57.000000 types-aiobotocore-dynamodbstreams-2.5.2.post3/types_aiobotocore_dynamodbstreams/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6920 2023-08-04 12:21:57.000000 types-aiobotocore-dynamodbstreams-2.5.2.post3/types_aiobotocore_dynamodbstreams/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     6908 2023-08-04 12:21:57.000000 types-aiobotocore-dynamodbstreams-2.5.2.post3/types_aiobotocore_dynamodbstreams/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8602 2023-08-04 12:21:58.000000 types-aiobotocore-dynamodbstreams-2.5.2.post3/types_aiobotocore_dynamodbstreams/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     8600 2023-08-04 12:21:58.000000 types-aiobotocore-dynamodbstreams-2.5.2.post3/types_aiobotocore_dynamodbstreams/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 12:21:57.000000 types-aiobotocore-dynamodbstreams-2.5.2.post3/types_aiobotocore_dynamodbstreams/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     6300 2023-08-04 12:21:58.000000 types-aiobotocore-dynamodbstreams-2.5.2.post3/types_aiobotocore_dynamodbstreams/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)     6293 2023-08-04 12:21:58.000000 types-aiobotocore-dynamodbstreams-2.5.2.post3/types_aiobotocore_dynamodbstreams/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-04 12:21:57.000000 types-aiobotocore-dynamodbstreams-2.5.2.post3/types_aiobotocore_dynamodbstreams/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:37:38.751695 types-aiobotocore-dynamodbstreams-2.5.2.post3/types_aiobotocore_dynamodbstreams.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    12598 2023-08-04 12:37:38.000000 types-aiobotocore-dynamodbstreams-2.5.2.post3/types_aiobotocore_dynamodbstreams.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      870 2023-08-04 12:37:38.000000 types-aiobotocore-dynamodbstreams-2.5.2.post3/types_aiobotocore_dynamodbstreams.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 12:37:38.000000 types-aiobotocore-dynamodbstreams-2.5.2.post3/types_aiobotocore_dynamodbstreams.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 12:37:38.000000 types-aiobotocore-dynamodbstreams-2.5.2.post3/types_aiobotocore_dynamodbstreams.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-04 12:37:38.000000 types-aiobotocore-dynamodbstreams-2.5.2.post3/types_aiobotocore_dynamodbstreams.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-08-04 12:37:38.000000 types-aiobotocore-dynamodbstreams-2.5.2.post3/types_aiobotocore_dynamodbstreams.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:23:38.470694 types-aiobotocore-dynamodbstreams-2.5.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-08 01:09:31.000000 types-aiobotocore-dynamodbstreams-2.5.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    12592 2023-08-08 01:23:38.470694 types-aiobotocore-dynamodbstreams-2.5.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    11048 2023-08-08 01:09:31.000000 types-aiobotocore-dynamodbstreams-2.5.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-08 01:23:38.470694 types-aiobotocore-dynamodbstreams-2.5.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2122 2023-08-08 01:09:31.000000 types-aiobotocore-dynamodbstreams-2.5.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:23:38.466694 types-aiobotocore-dynamodbstreams-2.5.4/types_aiobotocore_dynamodbstreams/
+-rw-r--r--   0 runner    (1001) docker     (123)      506 2023-08-08 01:09:31.000000 types-aiobotocore-dynamodbstreams-2.5.4/types_aiobotocore_dynamodbstreams/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      505 2023-08-08 01:09:31.000000 types-aiobotocore-dynamodbstreams-2.5.4/types_aiobotocore_dynamodbstreams/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      963 2023-08-08 01:09:31.000000 types-aiobotocore-dynamodbstreams-2.5.4/types_aiobotocore_dynamodbstreams/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6920 2023-08-08 01:09:31.000000 types-aiobotocore-dynamodbstreams-2.5.4/types_aiobotocore_dynamodbstreams/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6908 2023-08-08 01:09:31.000000 types-aiobotocore-dynamodbstreams-2.5.4/types_aiobotocore_dynamodbstreams/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8717 2023-08-08 01:09:31.000000 types-aiobotocore-dynamodbstreams-2.5.4/types_aiobotocore_dynamodbstreams/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8715 2023-08-08 01:09:31.000000 types-aiobotocore-dynamodbstreams-2.5.4/types_aiobotocore_dynamodbstreams/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 01:09:31.000000 types-aiobotocore-dynamodbstreams-2.5.4/types_aiobotocore_dynamodbstreams/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     6300 2023-08-08 01:09:31.000000 types-aiobotocore-dynamodbstreams-2.5.4/types_aiobotocore_dynamodbstreams/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6293 2023-08-08 01:09:31.000000 types-aiobotocore-dynamodbstreams-2.5.4/types_aiobotocore_dynamodbstreams/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-08-08 01:09:31.000000 types-aiobotocore-dynamodbstreams-2.5.4/types_aiobotocore_dynamodbstreams/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:23:38.470694 types-aiobotocore-dynamodbstreams-2.5.4/types_aiobotocore_dynamodbstreams.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    12592 2023-08-08 01:23:38.000000 types-aiobotocore-dynamodbstreams-2.5.4/types_aiobotocore_dynamodbstreams.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      870 2023-08-08 01:23:38.000000 types-aiobotocore-dynamodbstreams-2.5.4/types_aiobotocore_dynamodbstreams.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 01:23:38.000000 types-aiobotocore-dynamodbstreams-2.5.4/types_aiobotocore_dynamodbstreams.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 01:23:38.000000 types-aiobotocore-dynamodbstreams-2.5.4/types_aiobotocore_dynamodbstreams.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-08 01:23:38.000000 types-aiobotocore-dynamodbstreams-2.5.4/types_aiobotocore_dynamodbstreams.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-08-08 01:23:38.000000 types-aiobotocore-dynamodbstreams-2.5.4/types_aiobotocore_dynamodbstreams.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-dynamodbstreams-2.5.2.post3/LICENSE` & `types-aiobotocore-dynamodbstreams-2.5.4/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-dynamodbstreams-2.5.2.post3/PKG-INFO` & `types-aiobotocore-dynamodbstreams-2.5.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-dynamodbstreams
-Version: 2.5.2.post3
-Summary: Type annotations for aiobotocore.DynamoDBStreams 2.5.2 service generated with mypy-boto3-builder 7.17.2
+Version: 2.5.4
+Summary: Type annotations for aiobotocore.DynamoDBStreams 2.5.4 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dynamodbstreams/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-dynamodbstreams.svg?color=blue)](https://pypi.org/project/types-aiobotocore-dynamodbstreams)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dynamodbstreams/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-dynamodbstreams)](https://pepy.tech/project/types-aiobotocore-dynamodbstreams)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.DynamoDBStreams 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodbstreams.html#DynamoDBStreams)
+[aiobotocore.DynamoDBStreams 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodbstreams.html#DynamoDBStreams)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-dynamodbstreams-2.5.2.post3/README.md` & `types-aiobotocore-dynamodbstreams-2.5.4/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-dynamodbstreams.svg?color=blue)](https://pypi.org/project/types-aiobotocore-dynamodbstreams)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dynamodbstreams/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-dynamodbstreams)](https://pepy.tech/project/types-aiobotocore-dynamodbstreams)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.DynamoDBStreams 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodbstreams.html#DynamoDBStreams)
+[aiobotocore.DynamoDBStreams 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodbstreams.html#DynamoDBStreams)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-dynamodbstreams-2.5.2.post3/setup.py` & `types-aiobotocore-dynamodbstreams-2.5.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-dynamodbstreams",
-    version="2.5.2.post3",
+    version="2.5.4",
     packages=["types_aiobotocore_dynamodbstreams"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.DynamoDBStreams 2.5.2 service generated with"
+        "Type annotations for aiobotocore.DynamoDBStreams 2.5.4 service generated with"
         " mypy-boto3-builder 7.17.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
```

### Comparing `types-aiobotocore-dynamodbstreams-2.5.2.post3/types_aiobotocore_dynamodbstreams/__main__.py` & `types-aiobotocore-dynamodbstreams-2.5.4/types_aiobotocore_dynamodbstreams/__main__.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.DynamoDBStreams 2.5.2\nVersion:        "
-        " 2.5.2.post3\nBuilder version: 7.17.2\nDocs:           "
+        "Type annotations for aiobotocore.DynamoDBStreams 2.5.4\nVersion:         2.5.4\nBuilder"
+        " version: 7.17.2\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dynamodbstreams//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodbstreams.html#DynamoDBStreams\nOther"
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

### Comparing `types-aiobotocore-dynamodbstreams-2.5.2.post3/types_aiobotocore_dynamodbstreams/client.py` & `types-aiobotocore-dynamodbstreams-2.5.4/types_aiobotocore_dynamodbstreams/client.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-dynamodbstreams-2.5.2.post3/types_aiobotocore_dynamodbstreams/client.pyi` & `types-aiobotocore-dynamodbstreams-2.5.4/types_aiobotocore_dynamodbstreams/client.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-dynamodbstreams-2.5.2.post3/types_aiobotocore_dynamodbstreams/literals.py` & `types-aiobotocore-dynamodbstreams-2.5.4/types_aiobotocore_dynamodbstreams/literals.py`

 * *Files 1% similar despite different names*

```diff
@@ -51,14 +51,15 @@
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
@@ -154,14 +155,15 @@
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
@@ -240,26 +242,28 @@
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
@@ -420,14 +424,15 @@
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

### Comparing `types-aiobotocore-dynamodbstreams-2.5.2.post3/types_aiobotocore_dynamodbstreams/literals.pyi` & `types-aiobotocore-dynamodbstreams-2.5.4/types_aiobotocore_dynamodbstreams/literals.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -49,14 +49,15 @@
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
@@ -152,14 +153,15 @@
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
@@ -238,26 +240,28 @@
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
@@ -418,14 +422,15 @@
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

### Comparing `types-aiobotocore-dynamodbstreams-2.5.2.post3/types_aiobotocore_dynamodbstreams/type_defs.py` & `types-aiobotocore-dynamodbstreams-2.5.4/types_aiobotocore_dynamodbstreams/type_defs.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-dynamodbstreams-2.5.2.post3/types_aiobotocore_dynamodbstreams/type_defs.pyi` & `types-aiobotocore-dynamodbstreams-2.5.4/types_aiobotocore_dynamodbstreams/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-dynamodbstreams-2.5.2.post3/types_aiobotocore_dynamodbstreams.egg-info/PKG-INFO` & `types-aiobotocore-dynamodbstreams-2.5.4/types_aiobotocore_dynamodbstreams.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-dynamodbstreams
-Version: 2.5.2.post3
-Summary: Type annotations for aiobotocore.DynamoDBStreams 2.5.2 service generated with mypy-boto3-builder 7.17.2
+Version: 2.5.4
+Summary: Type annotations for aiobotocore.DynamoDBStreams 2.5.4 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dynamodbstreams/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-dynamodbstreams.svg?color=blue)](https://pypi.org/project/types-aiobotocore-dynamodbstreams)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dynamodbstreams/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-dynamodbstreams)](https://pepy.tech/project/types-aiobotocore-dynamodbstreams)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.DynamoDBStreams 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodbstreams.html#DynamoDBStreams)
+[aiobotocore.DynamoDBStreams 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodbstreams.html#DynamoDBStreams)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-dynamodbstreams-2.5.2.post3/types_aiobotocore_dynamodbstreams.egg-info/SOURCES.txt` & `types-aiobotocore-dynamodbstreams-2.5.4/types_aiobotocore_dynamodbstreams.egg-info/SOURCES.txt`

 * *Files identical despite different names*


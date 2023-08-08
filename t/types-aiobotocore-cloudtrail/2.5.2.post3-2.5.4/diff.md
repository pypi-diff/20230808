# Comparing `tmp/types-aiobotocore-cloudtrail-2.5.2.post3.tar.gz` & `tmp/types-aiobotocore-cloudtrail-2.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-cloudtrail-2.5.2.post3.tar", last modified: Fri Aug  4 12:37:26 2023, max compression
+gzip compressed data, was "types-aiobotocore-cloudtrail-2.5.4.tar", last modified: Tue Aug  8 01:23:27 2023, max compression
```

## Comparing `types-aiobotocore-cloudtrail-2.5.2.post3.tar` & `types-aiobotocore-cloudtrail-2.5.4.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:37:26.507396 types-aiobotocore-cloudtrail-2.5.2.post3/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-04 12:19:53.000000 types-aiobotocore-cloudtrail-2.5.2.post3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    13667 2023-08-04 12:37:26.503396 types-aiobotocore-cloudtrail-2.5.2.post3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    12137 2023-08-04 12:19:53.000000 types-aiobotocore-cloudtrail-2.5.2.post3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-04 12:37:26.507396 types-aiobotocore-cloudtrail-2.5.2.post3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2093 2023-08-04 12:19:52.000000 types-aiobotocore-cloudtrail-2.5.2.post3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:37:26.499396 types-aiobotocore-cloudtrail-2.5.2.post3/types_aiobotocore_cloudtrail/
--rw-r--r--   0 runner    (1001) docker     (123)     1583 2023-08-04 12:19:53.000000 types-aiobotocore-cloudtrail-2.5.2.post3/types_aiobotocore_cloudtrail/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1582 2023-08-04 12:19:53.000000 types-aiobotocore-cloudtrail-2.5.2.post3/types_aiobotocore_cloudtrail/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      955 2023-08-04 12:19:53.000000 types-aiobotocore-cloudtrail-2.5.2.post3/types_aiobotocore_cloudtrail/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    41289 2023-08-04 12:19:53.000000 types-aiobotocore-cloudtrail-2.5.2.post3/types_aiobotocore_cloudtrail/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    41228 2023-08-04 12:19:53.000000 types-aiobotocore-cloudtrail-2.5.2.post3/types_aiobotocore_cloudtrail/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    10114 2023-08-04 12:19:53.000000 types-aiobotocore-cloudtrail-2.5.2.post3/types_aiobotocore_cloudtrail/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    10112 2023-08-04 12:19:53.000000 types-aiobotocore-cloudtrail-2.5.2.post3/types_aiobotocore_cloudtrail/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     7966 2023-08-04 12:19:53.000000 types-aiobotocore-cloudtrail-2.5.2.post3/types_aiobotocore_cloudtrail/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     7957 2023-08-04 12:19:53.000000 types-aiobotocore-cloudtrail-2.5.2.post3/types_aiobotocore_cloudtrail/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 12:19:53.000000 types-aiobotocore-cloudtrail-2.5.2.post3/types_aiobotocore_cloudtrail/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    39768 2023-08-04 12:19:55.000000 types-aiobotocore-cloudtrail-2.5.2.post3/types_aiobotocore_cloudtrail/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    39733 2023-08-04 12:19:54.000000 types-aiobotocore-cloudtrail-2.5.2.post3/types_aiobotocore_cloudtrail/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-04 12:19:53.000000 types-aiobotocore-cloudtrail-2.5.2.post3/types_aiobotocore_cloudtrail/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:37:26.503396 types-aiobotocore-cloudtrail-2.5.2.post3/types_aiobotocore_cloudtrail.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    13667 2023-08-04 12:37:26.000000 types-aiobotocore-cloudtrail-2.5.2.post3/types_aiobotocore_cloudtrail.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      870 2023-08-04 12:37:26.000000 types-aiobotocore-cloudtrail-2.5.2.post3/types_aiobotocore_cloudtrail.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 12:37:26.000000 types-aiobotocore-cloudtrail-2.5.2.post3/types_aiobotocore_cloudtrail.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 12:37:26.000000 types-aiobotocore-cloudtrail-2.5.2.post3/types_aiobotocore_cloudtrail.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-04 12:37:26.000000 types-aiobotocore-cloudtrail-2.5.2.post3/types_aiobotocore_cloudtrail.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-08-04 12:37:26.000000 types-aiobotocore-cloudtrail-2.5.2.post3/types_aiobotocore_cloudtrail.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:23:27.046627 types-aiobotocore-cloudtrail-2.5.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-08 01:07:34.000000 types-aiobotocore-cloudtrail-2.5.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    13661 2023-08-08 01:23:27.046627 types-aiobotocore-cloudtrail-2.5.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    12137 2023-08-08 01:07:34.000000 types-aiobotocore-cloudtrail-2.5.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-08 01:23:27.046627 types-aiobotocore-cloudtrail-2.5.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2087 2023-08-08 01:07:34.000000 types-aiobotocore-cloudtrail-2.5.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:23:27.034627 types-aiobotocore-cloudtrail-2.5.4/types_aiobotocore_cloudtrail/
+-rw-r--r--   0 runner    (1001) docker     (123)     1583 2023-08-08 01:07:34.000000 types-aiobotocore-cloudtrail-2.5.4/types_aiobotocore_cloudtrail/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1582 2023-08-08 01:07:34.000000 types-aiobotocore-cloudtrail-2.5.4/types_aiobotocore_cloudtrail/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      943 2023-08-08 01:07:34.000000 types-aiobotocore-cloudtrail-2.5.4/types_aiobotocore_cloudtrail/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41289 2023-08-08 01:07:34.000000 types-aiobotocore-cloudtrail-2.5.4/types_aiobotocore_cloudtrail/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41228 2023-08-08 01:07:34.000000 types-aiobotocore-cloudtrail-2.5.4/types_aiobotocore_cloudtrail/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    10229 2023-08-08 01:07:35.000000 types-aiobotocore-cloudtrail-2.5.4/types_aiobotocore_cloudtrail/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10227 2023-08-08 01:07:34.000000 types-aiobotocore-cloudtrail-2.5.4/types_aiobotocore_cloudtrail/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     7966 2023-08-08 01:07:34.000000 types-aiobotocore-cloudtrail-2.5.4/types_aiobotocore_cloudtrail/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7957 2023-08-08 01:07:34.000000 types-aiobotocore-cloudtrail-2.5.4/types_aiobotocore_cloudtrail/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 01:07:34.000000 types-aiobotocore-cloudtrail-2.5.4/types_aiobotocore_cloudtrail/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    39768 2023-08-08 01:07:36.000000 types-aiobotocore-cloudtrail-2.5.4/types_aiobotocore_cloudtrail/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39733 2023-08-08 01:07:35.000000 types-aiobotocore-cloudtrail-2.5.4/types_aiobotocore_cloudtrail/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-08-08 01:07:34.000000 types-aiobotocore-cloudtrail-2.5.4/types_aiobotocore_cloudtrail/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:23:27.046627 types-aiobotocore-cloudtrail-2.5.4/types_aiobotocore_cloudtrail.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    13661 2023-08-08 01:23:26.000000 types-aiobotocore-cloudtrail-2.5.4/types_aiobotocore_cloudtrail.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      870 2023-08-08 01:23:26.000000 types-aiobotocore-cloudtrail-2.5.4/types_aiobotocore_cloudtrail.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 01:23:26.000000 types-aiobotocore-cloudtrail-2.5.4/types_aiobotocore_cloudtrail.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 01:23:26.000000 types-aiobotocore-cloudtrail-2.5.4/types_aiobotocore_cloudtrail.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-08 01:23:26.000000 types-aiobotocore-cloudtrail-2.5.4/types_aiobotocore_cloudtrail.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-08-08 01:23:26.000000 types-aiobotocore-cloudtrail-2.5.4/types_aiobotocore_cloudtrail.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-cloudtrail-2.5.2.post3/LICENSE` & `types-aiobotocore-cloudtrail-2.5.4/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-cloudtrail-2.5.2.post3/PKG-INFO` & `types-aiobotocore-cloudtrail-2.5.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-cloudtrail
-Version: 2.5.2.post3
-Summary: Type annotations for aiobotocore.CloudTrail 2.5.2 service generated with mypy-boto3-builder 7.17.2
+Version: 2.5.4
+Summary: Type annotations for aiobotocore.CloudTrail 2.5.4 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudtrail/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-cloudtrail.svg?color=blue)](https://pypi.org/project/types-aiobotocore-cloudtrail)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudtrail/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-cloudtrail)](https://pepy.tech/project/types-aiobotocore-cloudtrail)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.CloudTrail 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudtrail.html#CloudTrail)
+[aiobotocore.CloudTrail 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudtrail.html#CloudTrail)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-cloudtrail-2.5.2.post3/README.md` & `types-aiobotocore-cloudtrail-2.5.4/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-cloudtrail.svg?color=blue)](https://pypi.org/project/types-aiobotocore-cloudtrail)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudtrail/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-cloudtrail)](https://pepy.tech/project/types-aiobotocore-cloudtrail)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.CloudTrail 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudtrail.html#CloudTrail)
+[aiobotocore.CloudTrail 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudtrail.html#CloudTrail)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-cloudtrail-2.5.2.post3/setup.py` & `types-aiobotocore-cloudtrail-2.5.4/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-cloudtrail",
-    version="2.5.2.post3",
+    version="2.5.4",
     packages=["types_aiobotocore_cloudtrail"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.CloudTrail 2.5.2 service generated with"
+        "Type annotations for aiobotocore.CloudTrail 2.5.4 service generated with"
         " mypy-boto3-builder 7.17.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
```

### Comparing `types-aiobotocore-cloudtrail-2.5.2.post3/types_aiobotocore_cloudtrail/__init__.py` & `types-aiobotocore-cloudtrail-2.5.4/types_aiobotocore_cloudtrail/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-cloudtrail-2.5.2.post3/types_aiobotocore_cloudtrail/__init__.pyi` & `types-aiobotocore-cloudtrail-2.5.4/types_aiobotocore_cloudtrail/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-cloudtrail-2.5.2.post3/types_aiobotocore_cloudtrail/__main__.py` & `types-aiobotocore-cloudtrail-2.5.4/types_aiobotocore_cloudtrail/__main__.py`

 * *Files 10% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.CloudTrail 2.5.2\nVersion:         2.5.2.post3\nBuilder"
+        "Type annotations for aiobotocore.CloudTrail 2.5.4\nVersion:         2.5.4\nBuilder"
         " version: 7.17.2\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudtrail//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudtrail.html#CloudTrail\nOther"
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

### Comparing `types-aiobotocore-cloudtrail-2.5.2.post3/types_aiobotocore_cloudtrail/client.py` & `types-aiobotocore-cloudtrail-2.5.4/types_aiobotocore_cloudtrail/client.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-cloudtrail-2.5.2.post3/types_aiobotocore_cloudtrail/client.pyi` & `types-aiobotocore-cloudtrail-2.5.4/types_aiobotocore_cloudtrail/client.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-cloudtrail-2.5.2.post3/types_aiobotocore_cloudtrail/literals.py` & `types-aiobotocore-cloudtrail-2.5.4/types_aiobotocore_cloudtrail/literals.py`

 * *Files 0% similar despite different names*

```diff
@@ -98,14 +98,15 @@
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
@@ -201,14 +202,15 @@
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
@@ -287,26 +289,28 @@
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
@@ -475,14 +479,15 @@
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

### Comparing `types-aiobotocore-cloudtrail-2.5.2.post3/types_aiobotocore_cloudtrail/literals.pyi` & `types-aiobotocore-cloudtrail-2.5.4/types_aiobotocore_cloudtrail/literals.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -96,14 +96,15 @@
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
@@ -199,14 +200,15 @@
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
@@ -285,26 +287,28 @@
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
@@ -473,14 +477,15 @@
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

### Comparing `types-aiobotocore-cloudtrail-2.5.2.post3/types_aiobotocore_cloudtrail/paginator.py` & `types-aiobotocore-cloudtrail-2.5.4/types_aiobotocore_cloudtrail/paginator.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-cloudtrail-2.5.2.post3/types_aiobotocore_cloudtrail/paginator.pyi` & `types-aiobotocore-cloudtrail-2.5.4/types_aiobotocore_cloudtrail/paginator.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-cloudtrail-2.5.2.post3/types_aiobotocore_cloudtrail/type_defs.py` & `types-aiobotocore-cloudtrail-2.5.4/types_aiobotocore_cloudtrail/type_defs.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-cloudtrail-2.5.2.post3/types_aiobotocore_cloudtrail/type_defs.pyi` & `types-aiobotocore-cloudtrail-2.5.4/types_aiobotocore_cloudtrail/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-cloudtrail-2.5.2.post3/types_aiobotocore_cloudtrail.egg-info/PKG-INFO` & `types-aiobotocore-cloudtrail-2.5.4/types_aiobotocore_cloudtrail.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-cloudtrail
-Version: 2.5.2.post3
-Summary: Type annotations for aiobotocore.CloudTrail 2.5.2 service generated with mypy-boto3-builder 7.17.2
+Version: 2.5.4
+Summary: Type annotations for aiobotocore.CloudTrail 2.5.4 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudtrail/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-cloudtrail.svg?color=blue)](https://pypi.org/project/types-aiobotocore-cloudtrail)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudtrail/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-cloudtrail)](https://pepy.tech/project/types-aiobotocore-cloudtrail)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.CloudTrail 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudtrail.html#CloudTrail)
+[aiobotocore.CloudTrail 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudtrail.html#CloudTrail)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-cloudtrail-2.5.2.post3/types_aiobotocore_cloudtrail.egg-info/SOURCES.txt` & `types-aiobotocore-cloudtrail-2.5.4/types_aiobotocore_cloudtrail.egg-info/SOURCES.txt`

 * *Files identical despite different names*


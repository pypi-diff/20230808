# Comparing `tmp/types-aiobotocore-cloudcontrol-2.5.2.post3.tar.gz` & `tmp/types-aiobotocore-cloudcontrol-2.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-cloudcontrol-2.5.2.post3.tar", last modified: Fri Aug  4 12:37:24 2023, max compression
+gzip compressed data, was "types-aiobotocore-cloudcontrol-2.5.4.tar", last modified: Tue Aug  8 01:23:24 2023, max compression
```

## Comparing `types-aiobotocore-cloudcontrol-2.5.2.post3.tar` & `types-aiobotocore-cloudcontrol-2.5.4.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:37:24.039336 types-aiobotocore-cloudcontrol-2.5.2.post3/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-04 12:19:29.000000 types-aiobotocore-cloudcontrol-2.5.2.post3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    14209 2023-08-04 12:37:24.039336 types-aiobotocore-cloudcontrol-2.5.2.post3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    12668 2023-08-04 12:19:29.000000 types-aiobotocore-cloudcontrol-2.5.2.post3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-04 12:37:24.039336 types-aiobotocore-cloudcontrol-2.5.2.post3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2110 2023-08-04 12:19:29.000000 types-aiobotocore-cloudcontrol-2.5.2.post3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:37:24.039336 types-aiobotocore-cloudcontrol-2.5.2.post3/types_aiobotocore_cloudcontrol/
--rw-r--r--   0 runner    (1001) docker     (123)     1173 2023-08-04 12:19:29.000000 types-aiobotocore-cloudcontrol-2.5.2.post3/types_aiobotocore_cloudcontrol/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1172 2023-08-04 12:19:29.000000 types-aiobotocore-cloudcontrol-2.5.2.post3/types_aiobotocore_cloudcontrol/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      969 2023-08-04 12:19:29.000000 types-aiobotocore-cloudcontrol-2.5.2.post3/types_aiobotocore_cloudcontrol/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12087 2023-08-04 12:19:29.000000 types-aiobotocore-cloudcontrol-2.5.2.post3/types_aiobotocore_cloudcontrol/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    12067 2023-08-04 12:19:29.000000 types-aiobotocore-cloudcontrol-2.5.2.post3/types_aiobotocore_cloudcontrol/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9217 2023-08-04 12:19:29.000000 types-aiobotocore-cloudcontrol-2.5.2.post3/types_aiobotocore_cloudcontrol/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     9215 2023-08-04 12:19:29.000000 types-aiobotocore-cloudcontrol-2.5.2.post3/types_aiobotocore_cloudcontrol/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     3482 2023-08-04 12:19:29.000000 types-aiobotocore-cloudcontrol-2.5.2.post3/types_aiobotocore_cloudcontrol/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     3478 2023-08-04 12:19:29.000000 types-aiobotocore-cloudcontrol-2.5.2.post3/types_aiobotocore_cloudcontrol/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 12:19:29.000000 types-aiobotocore-cloudcontrol-2.5.2.post3/types_aiobotocore_cloudcontrol/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     9719 2023-08-04 12:19:29.000000 types-aiobotocore-cloudcontrol-2.5.2.post3/types_aiobotocore_cloudcontrol/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)     9704 2023-08-04 12:19:29.000000 types-aiobotocore-cloudcontrol-2.5.2.post3/types_aiobotocore_cloudcontrol/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-04 12:19:29.000000 types-aiobotocore-cloudcontrol-2.5.2.post3/types_aiobotocore_cloudcontrol/version.py
--rw-r--r--   0 runner    (1001) docker     (123)     1681 2023-08-04 12:19:29.000000 types-aiobotocore-cloudcontrol-2.5.2.post3/types_aiobotocore_cloudcontrol/waiter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1680 2023-08-04 12:19:29.000000 types-aiobotocore-cloudcontrol-2.5.2.post3/types_aiobotocore_cloudcontrol/waiter.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:37:24.039336 types-aiobotocore-cloudcontrol-2.5.2.post3/types_aiobotocore_cloudcontrol.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    14209 2023-08-04 12:37:23.000000 types-aiobotocore-cloudcontrol-2.5.2.post3/types_aiobotocore_cloudcontrol.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      991 2023-08-04 12:37:23.000000 types-aiobotocore-cloudcontrol-2.5.2.post3/types_aiobotocore_cloudcontrol.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 12:37:23.000000 types-aiobotocore-cloudcontrol-2.5.2.post3/types_aiobotocore_cloudcontrol.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 12:37:23.000000 types-aiobotocore-cloudcontrol-2.5.2.post3/types_aiobotocore_cloudcontrol.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-04 12:37:23.000000 types-aiobotocore-cloudcontrol-2.5.2.post3/types_aiobotocore_cloudcontrol.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-08-04 12:37:23.000000 types-aiobotocore-cloudcontrol-2.5.2.post3/types_aiobotocore_cloudcontrol.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:23:24.750624 types-aiobotocore-cloudcontrol-2.5.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-08 01:07:13.000000 types-aiobotocore-cloudcontrol-2.5.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    14203 2023-08-08 01:23:24.750624 types-aiobotocore-cloudcontrol-2.5.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    12668 2023-08-08 01:07:13.000000 types-aiobotocore-cloudcontrol-2.5.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-08 01:23:24.750624 types-aiobotocore-cloudcontrol-2.5.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2104 2023-08-08 01:07:13.000000 types-aiobotocore-cloudcontrol-2.5.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:23:24.750624 types-aiobotocore-cloudcontrol-2.5.4/types_aiobotocore_cloudcontrol/
+-rw-r--r--   0 runner    (1001) docker     (123)     1173 2023-08-08 01:07:13.000000 types-aiobotocore-cloudcontrol-2.5.4/types_aiobotocore_cloudcontrol/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1172 2023-08-08 01:07:13.000000 types-aiobotocore-cloudcontrol-2.5.4/types_aiobotocore_cloudcontrol/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      957 2023-08-08 01:07:13.000000 types-aiobotocore-cloudcontrol-2.5.4/types_aiobotocore_cloudcontrol/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12087 2023-08-08 01:07:13.000000 types-aiobotocore-cloudcontrol-2.5.4/types_aiobotocore_cloudcontrol/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12067 2023-08-08 01:07:13.000000 types-aiobotocore-cloudcontrol-2.5.4/types_aiobotocore_cloudcontrol/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9332 2023-08-08 01:07:13.000000 types-aiobotocore-cloudcontrol-2.5.4/types_aiobotocore_cloudcontrol/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9330 2023-08-08 01:07:13.000000 types-aiobotocore-cloudcontrol-2.5.4/types_aiobotocore_cloudcontrol/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     3482 2023-08-08 01:07:13.000000 types-aiobotocore-cloudcontrol-2.5.4/types_aiobotocore_cloudcontrol/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3478 2023-08-08 01:07:13.000000 types-aiobotocore-cloudcontrol-2.5.4/types_aiobotocore_cloudcontrol/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 01:07:13.000000 types-aiobotocore-cloudcontrol-2.5.4/types_aiobotocore_cloudcontrol/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     9719 2023-08-08 01:07:13.000000 types-aiobotocore-cloudcontrol-2.5.4/types_aiobotocore_cloudcontrol/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9704 2023-08-08 01:07:13.000000 types-aiobotocore-cloudcontrol-2.5.4/types_aiobotocore_cloudcontrol/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-08-08 01:07:13.000000 types-aiobotocore-cloudcontrol-2.5.4/types_aiobotocore_cloudcontrol/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1681 2023-08-08 01:07:13.000000 types-aiobotocore-cloudcontrol-2.5.4/types_aiobotocore_cloudcontrol/waiter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1680 2023-08-08 01:07:13.000000 types-aiobotocore-cloudcontrol-2.5.4/types_aiobotocore_cloudcontrol/waiter.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:23:24.750624 types-aiobotocore-cloudcontrol-2.5.4/types_aiobotocore_cloudcontrol.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    14203 2023-08-08 01:23:24.000000 types-aiobotocore-cloudcontrol-2.5.4/types_aiobotocore_cloudcontrol.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      991 2023-08-08 01:23:24.000000 types-aiobotocore-cloudcontrol-2.5.4/types_aiobotocore_cloudcontrol.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 01:23:24.000000 types-aiobotocore-cloudcontrol-2.5.4/types_aiobotocore_cloudcontrol.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 01:23:24.000000 types-aiobotocore-cloudcontrol-2.5.4/types_aiobotocore_cloudcontrol.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-08 01:23:24.000000 types-aiobotocore-cloudcontrol-2.5.4/types_aiobotocore_cloudcontrol.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-08-08 01:23:24.000000 types-aiobotocore-cloudcontrol-2.5.4/types_aiobotocore_cloudcontrol.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-cloudcontrol-2.5.2.post3/LICENSE` & `types-aiobotocore-cloudcontrol-2.5.4/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-cloudcontrol-2.5.2.post3/PKG-INFO` & `types-aiobotocore-cloudcontrol-2.5.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-cloudcontrol
-Version: 2.5.2.post3
-Summary: Type annotations for aiobotocore.CloudControlApi 2.5.2 service generated with mypy-boto3-builder 7.17.2
+Version: 2.5.4
+Summary: Type annotations for aiobotocore.CloudControlApi 2.5.4 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudcontrol/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-cloudcontrol.svg?color=blue)](https://pypi.org/project/types-aiobotocore-cloudcontrol)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudcontrol/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-cloudcontrol)](https://pepy.tech/project/types-aiobotocore-cloudcontrol)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.CloudControlApi 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudcontrol.html#CloudControlApi)
+[aiobotocore.CloudControlApi 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudcontrol.html#CloudControlApi)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-cloudcontrol-2.5.2.post3/README.md` & `types-aiobotocore-cloudcontrol-2.5.4/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-cloudcontrol.svg?color=blue)](https://pypi.org/project/types-aiobotocore-cloudcontrol)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudcontrol/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-cloudcontrol)](https://pepy.tech/project/types-aiobotocore-cloudcontrol)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.CloudControlApi 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudcontrol.html#CloudControlApi)
+[aiobotocore.CloudControlApi 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudcontrol.html#CloudControlApi)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-cloudcontrol-2.5.2.post3/setup.py` & `types-aiobotocore-cloudcontrol-2.5.4/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-cloudcontrol",
-    version="2.5.2.post3",
+    version="2.5.4",
     packages=["types_aiobotocore_cloudcontrol"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.CloudControlApi 2.5.2 service generated with"
+        "Type annotations for aiobotocore.CloudControlApi 2.5.4 service generated with"
         " mypy-boto3-builder 7.17.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
```

### Comparing `types-aiobotocore-cloudcontrol-2.5.2.post3/types_aiobotocore_cloudcontrol/__init__.py` & `types-aiobotocore-cloudcontrol-2.5.4/types_aiobotocore_cloudcontrol/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-cloudcontrol-2.5.2.post3/types_aiobotocore_cloudcontrol/__init__.pyi` & `types-aiobotocore-cloudcontrol-2.5.4/types_aiobotocore_cloudcontrol/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-cloudcontrol-2.5.2.post3/types_aiobotocore_cloudcontrol/__main__.py` & `types-aiobotocore-cloudcontrol-2.5.4/types_aiobotocore_cloudcontrol/__main__.py`

 * *Files 21% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.CloudControlApi 2.5.2\nVersion:        "
-        " 2.5.2.post3\nBuilder version: 7.17.2\nDocs:           "
+        "Type annotations for aiobotocore.CloudControlApi 2.5.4\nVersion:         2.5.4\nBuilder"
+        " version: 7.17.2\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudcontrol//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudcontrol.html#CloudControlApi\nOther"
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

### Comparing `types-aiobotocore-cloudcontrol-2.5.2.post3/types_aiobotocore_cloudcontrol/client.py` & `types-aiobotocore-cloudcontrol-2.5.4/types_aiobotocore_cloudcontrol/client.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-cloudcontrol-2.5.2.post3/types_aiobotocore_cloudcontrol/client.pyi` & `types-aiobotocore-cloudcontrol-2.5.4/types_aiobotocore_cloudcontrol/client.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-cloudcontrol-2.5.2.post3/types_aiobotocore_cloudcontrol/literals.py` & `types-aiobotocore-cloudcontrol-2.5.4/types_aiobotocore_cloudcontrol/literals.py`

 * *Files 1% similar despite different names*

```diff
@@ -71,14 +71,15 @@
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
@@ -174,14 +175,15 @@
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
@@ -260,26 +262,28 @@
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
@@ -442,14 +446,15 @@
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

### Comparing `types-aiobotocore-cloudcontrol-2.5.2.post3/types_aiobotocore_cloudcontrol/literals.pyi` & `types-aiobotocore-cloudcontrol-2.5.4/types_aiobotocore_cloudcontrol/literals.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -69,14 +69,15 @@
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
@@ -172,14 +173,15 @@
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
@@ -258,26 +260,28 @@
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
@@ -440,14 +444,15 @@
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

### Comparing `types-aiobotocore-cloudcontrol-2.5.2.post3/types_aiobotocore_cloudcontrol/paginator.py` & `types-aiobotocore-cloudcontrol-2.5.4/types_aiobotocore_cloudcontrol/paginator.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-cloudcontrol-2.5.2.post3/types_aiobotocore_cloudcontrol/paginator.pyi` & `types-aiobotocore-cloudcontrol-2.5.4/types_aiobotocore_cloudcontrol/paginator.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-cloudcontrol-2.5.2.post3/types_aiobotocore_cloudcontrol/type_defs.py` & `types-aiobotocore-cloudcontrol-2.5.4/types_aiobotocore_cloudcontrol/type_defs.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-cloudcontrol-2.5.2.post3/types_aiobotocore_cloudcontrol/type_defs.pyi` & `types-aiobotocore-cloudcontrol-2.5.4/types_aiobotocore_cloudcontrol/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-cloudcontrol-2.5.2.post3/types_aiobotocore_cloudcontrol/waiter.py` & `types-aiobotocore-cloudcontrol-2.5.4/types_aiobotocore_cloudcontrol/waiter.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-cloudcontrol-2.5.2.post3/types_aiobotocore_cloudcontrol/waiter.pyi` & `types-aiobotocore-cloudcontrol-2.5.4/types_aiobotocore_cloudcontrol/waiter.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-cloudcontrol-2.5.2.post3/types_aiobotocore_cloudcontrol.egg-info/PKG-INFO` & `types-aiobotocore-cloudcontrol-2.5.4/types_aiobotocore_cloudcontrol.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-cloudcontrol
-Version: 2.5.2.post3
-Summary: Type annotations for aiobotocore.CloudControlApi 2.5.2 service generated with mypy-boto3-builder 7.17.2
+Version: 2.5.4
+Summary: Type annotations for aiobotocore.CloudControlApi 2.5.4 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudcontrol/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-cloudcontrol.svg?color=blue)](https://pypi.org/project/types-aiobotocore-cloudcontrol)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudcontrol/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-cloudcontrol)](https://pepy.tech/project/types-aiobotocore-cloudcontrol)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.CloudControlApi 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudcontrol.html#CloudControlApi)
+[aiobotocore.CloudControlApi 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudcontrol.html#CloudControlApi)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-cloudcontrol-2.5.2.post3/types_aiobotocore_cloudcontrol.egg-info/SOURCES.txt` & `types-aiobotocore-cloudcontrol-2.5.4/types_aiobotocore_cloudcontrol.egg-info/SOURCES.txt`

 * *Files identical despite different names*


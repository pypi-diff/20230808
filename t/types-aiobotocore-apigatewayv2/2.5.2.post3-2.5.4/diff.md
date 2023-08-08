# Comparing `tmp/types-aiobotocore-apigatewayv2-2.5.2.post3.tar.gz` & `tmp/types-aiobotocore-apigatewayv2-2.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-apigatewayv2-2.5.2.post3.tar", last modified: Fri Aug  4 12:37:16 2023, max compression
+gzip compressed data, was "types-aiobotocore-apigatewayv2-2.5.4.tar", last modified: Tue Aug  8 01:23:14 2023, max compression
```

## Comparing `types-aiobotocore-apigatewayv2-2.5.2.post3.tar` & `types-aiobotocore-apigatewayv2-2.5.4.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:37:16.351167 types-aiobotocore-apigatewayv2-2.5.2.post3/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-04 12:18:13.000000 types-aiobotocore-apigatewayv2-2.5.2.post3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    14347 2023-08-04 12:37:16.351167 types-aiobotocore-apigatewayv2-2.5.2.post3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    12809 2023-08-04 12:18:13.000000 types-aiobotocore-apigatewayv2-2.5.2.post3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-04 12:37:16.351167 types-aiobotocore-apigatewayv2-2.5.2.post3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2107 2023-08-04 12:18:12.000000 types-aiobotocore-apigatewayv2-2.5.2.post3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:37:16.347167 types-aiobotocore-apigatewayv2-2.5.2.post3/types_aiobotocore_apigatewayv2/
--rw-r--r--   0 runner    (1001) docker     (123)     2373 2023-08-04 12:18:13.000000 types-aiobotocore-apigatewayv2-2.5.2.post3/types_aiobotocore_apigatewayv2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2372 2023-08-04 12:18:13.000000 types-aiobotocore-apigatewayv2-2.5.2.post3/types_aiobotocore_apigatewayv2/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      963 2023-08-04 12:18:13.000000 types-aiobotocore-apigatewayv2-2.5.2.post3/types_aiobotocore_apigatewayv2/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    54790 2023-08-04 12:18:13.000000 types-aiobotocore-apigatewayv2-2.5.2.post3/types_aiobotocore_apigatewayv2/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    54699 2023-08-04 12:18:13.000000 types-aiobotocore-apigatewayv2-2.5.2.post3/types_aiobotocore_apigatewayv2/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    10680 2023-08-04 12:18:13.000000 types-aiobotocore-apigatewayv2-2.5.2.post3/types_aiobotocore_apigatewayv2/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    10678 2023-08-04 12:18:13.000000 types-aiobotocore-apigatewayv2-2.5.2.post3/types_aiobotocore_apigatewayv2/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    11883 2023-08-04 12:18:13.000000 types-aiobotocore-apigatewayv2-2.5.2.post3/types_aiobotocore_apigatewayv2/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)    11871 2023-08-04 12:18:13.000000 types-aiobotocore-apigatewayv2-2.5.2.post3/types_aiobotocore_apigatewayv2/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 12:18:13.000000 types-aiobotocore-apigatewayv2-2.5.2.post3/types_aiobotocore_apigatewayv2/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    75222 2023-08-04 12:18:15.000000 types-aiobotocore-apigatewayv2-2.5.2.post3/types_aiobotocore_apigatewayv2/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    75111 2023-08-04 12:18:15.000000 types-aiobotocore-apigatewayv2-2.5.2.post3/types_aiobotocore_apigatewayv2/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-04 12:18:13.000000 types-aiobotocore-apigatewayv2-2.5.2.post3/types_aiobotocore_apigatewayv2/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:37:16.351167 types-aiobotocore-apigatewayv2-2.5.2.post3/types_aiobotocore_apigatewayv2.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    14347 2023-08-04 12:37:16.000000 types-aiobotocore-apigatewayv2-2.5.2.post3/types_aiobotocore_apigatewayv2.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      908 2023-08-04 12:37:16.000000 types-aiobotocore-apigatewayv2-2.5.2.post3/types_aiobotocore_apigatewayv2.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 12:37:16.000000 types-aiobotocore-apigatewayv2-2.5.2.post3/types_aiobotocore_apigatewayv2.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 12:37:16.000000 types-aiobotocore-apigatewayv2-2.5.2.post3/types_aiobotocore_apigatewayv2.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-04 12:37:16.000000 types-aiobotocore-apigatewayv2-2.5.2.post3/types_aiobotocore_apigatewayv2.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-08-04 12:37:16.000000 types-aiobotocore-apigatewayv2-2.5.2.post3/types_aiobotocore_apigatewayv2.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:23:14.570491 types-aiobotocore-apigatewayv2-2.5.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-08 01:05:59.000000 types-aiobotocore-apigatewayv2-2.5.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    14341 2023-08-08 01:23:14.562491 types-aiobotocore-apigatewayv2-2.5.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    12809 2023-08-08 01:05:59.000000 types-aiobotocore-apigatewayv2-2.5.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-08 01:23:14.570491 types-aiobotocore-apigatewayv2-2.5.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2101 2023-08-08 01:05:59.000000 types-aiobotocore-apigatewayv2-2.5.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:23:14.562491 types-aiobotocore-apigatewayv2-2.5.4/types_aiobotocore_apigatewayv2/
+-rw-r--r--   0 runner    (1001) docker     (123)     2373 2023-08-08 01:05:59.000000 types-aiobotocore-apigatewayv2-2.5.4/types_aiobotocore_apigatewayv2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2372 2023-08-08 01:05:59.000000 types-aiobotocore-apigatewayv2-2.5.4/types_aiobotocore_apigatewayv2/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      951 2023-08-08 01:05:59.000000 types-aiobotocore-apigatewayv2-2.5.4/types_aiobotocore_apigatewayv2/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    54790 2023-08-08 01:06:00.000000 types-aiobotocore-apigatewayv2-2.5.4/types_aiobotocore_apigatewayv2/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    54699 2023-08-08 01:05:59.000000 types-aiobotocore-apigatewayv2-2.5.4/types_aiobotocore_apigatewayv2/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    10795 2023-08-08 01:06:00.000000 types-aiobotocore-apigatewayv2-2.5.4/types_aiobotocore_apigatewayv2/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10793 2023-08-08 01:06:00.000000 types-aiobotocore-apigatewayv2-2.5.4/types_aiobotocore_apigatewayv2/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    11883 2023-08-08 01:06:00.000000 types-aiobotocore-apigatewayv2-2.5.4/types_aiobotocore_apigatewayv2/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11871 2023-08-08 01:06:00.000000 types-aiobotocore-apigatewayv2-2.5.4/types_aiobotocore_apigatewayv2/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 01:05:59.000000 types-aiobotocore-apigatewayv2-2.5.4/types_aiobotocore_apigatewayv2/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    75222 2023-08-08 01:06:02.000000 types-aiobotocore-apigatewayv2-2.5.4/types_aiobotocore_apigatewayv2/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    75111 2023-08-08 01:06:01.000000 types-aiobotocore-apigatewayv2-2.5.4/types_aiobotocore_apigatewayv2/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-08-08 01:05:59.000000 types-aiobotocore-apigatewayv2-2.5.4/types_aiobotocore_apigatewayv2/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:23:14.562491 types-aiobotocore-apigatewayv2-2.5.4/types_aiobotocore_apigatewayv2.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    14341 2023-08-08 01:23:14.000000 types-aiobotocore-apigatewayv2-2.5.4/types_aiobotocore_apigatewayv2.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      908 2023-08-08 01:23:14.000000 types-aiobotocore-apigatewayv2-2.5.4/types_aiobotocore_apigatewayv2.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 01:23:14.000000 types-aiobotocore-apigatewayv2-2.5.4/types_aiobotocore_apigatewayv2.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 01:23:14.000000 types-aiobotocore-apigatewayv2-2.5.4/types_aiobotocore_apigatewayv2.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-08 01:23:14.000000 types-aiobotocore-apigatewayv2-2.5.4/types_aiobotocore_apigatewayv2.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-08-08 01:23:14.000000 types-aiobotocore-apigatewayv2-2.5.4/types_aiobotocore_apigatewayv2.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-apigatewayv2-2.5.2.post3/LICENSE` & `types-aiobotocore-apigatewayv2-2.5.4/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-apigatewayv2-2.5.2.post3/PKG-INFO` & `types-aiobotocore-apigatewayv2-2.5.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-apigatewayv2
-Version: 2.5.2.post3
-Summary: Type annotations for aiobotocore.ApiGatewayV2 2.5.2 service generated with mypy-boto3-builder 7.17.2
+Version: 2.5.4
+Summary: Type annotations for aiobotocore.ApiGatewayV2 2.5.4 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_apigatewayv2/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-apigatewayv2.svg?color=blue)](https://pypi.org/project/types-aiobotocore-apigatewayv2)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_apigatewayv2/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-apigatewayv2)](https://pepy.tech/project/types-aiobotocore-apigatewayv2)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.ApiGatewayV2 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigatewayv2.html#ApiGatewayV2)
+[aiobotocore.ApiGatewayV2 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigatewayv2.html#ApiGatewayV2)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-apigatewayv2-2.5.2.post3/README.md` & `types-aiobotocore-apigatewayv2-2.5.4/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-apigatewayv2.svg?color=blue)](https://pypi.org/project/types-aiobotocore-apigatewayv2)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_apigatewayv2/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-apigatewayv2)](https://pepy.tech/project/types-aiobotocore-apigatewayv2)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.ApiGatewayV2 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigatewayv2.html#ApiGatewayV2)
+[aiobotocore.ApiGatewayV2 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigatewayv2.html#ApiGatewayV2)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-apigatewayv2-2.5.2.post3/setup.py` & `types-aiobotocore-apigatewayv2-2.5.4/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-apigatewayv2",
-    version="2.5.2.post3",
+    version="2.5.4",
     packages=["types_aiobotocore_apigatewayv2"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.ApiGatewayV2 2.5.2 service generated with"
+        "Type annotations for aiobotocore.ApiGatewayV2 2.5.4 service generated with"
         " mypy-boto3-builder 7.17.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
```

### Comparing `types-aiobotocore-apigatewayv2-2.5.2.post3/types_aiobotocore_apigatewayv2/__init__.py` & `types-aiobotocore-apigatewayv2-2.5.4/types_aiobotocore_apigatewayv2/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-apigatewayv2-2.5.2.post3/types_aiobotocore_apigatewayv2/__init__.pyi` & `types-aiobotocore-apigatewayv2-2.5.4/types_aiobotocore_apigatewayv2/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-apigatewayv2-2.5.2.post3/types_aiobotocore_apigatewayv2/__main__.py` & `types-aiobotocore-apigatewayv2-2.5.4/types_aiobotocore_apigatewayv2/__main__.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.ApiGatewayV2 2.5.2\nVersion:         2.5.2.post3\nBuilder"
+        "Type annotations for aiobotocore.ApiGatewayV2 2.5.4\nVersion:         2.5.4\nBuilder"
         " version: 7.17.2\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_apigatewayv2//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigatewayv2.html#ApiGatewayV2\nOther"
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

### Comparing `types-aiobotocore-apigatewayv2-2.5.2.post3/types_aiobotocore_apigatewayv2/client.py` & `types-aiobotocore-apigatewayv2-2.5.4/types_aiobotocore_apigatewayv2/client.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-apigatewayv2-2.5.2.post3/types_aiobotocore_apigatewayv2/client.pyi` & `types-aiobotocore-apigatewayv2-2.5.4/types_aiobotocore_apigatewayv2/client.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-apigatewayv2-2.5.2.post3/types_aiobotocore_apigatewayv2/literals.py` & `types-aiobotocore-apigatewayv2-2.5.4/types_aiobotocore_apigatewayv2/literals.py`

 * *Files 0% similar despite different names*

```diff
@@ -94,14 +94,15 @@
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
@@ -197,14 +198,15 @@
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
@@ -283,26 +285,28 @@
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

### Comparing `types-aiobotocore-apigatewayv2-2.5.2.post3/types_aiobotocore_apigatewayv2/literals.pyi` & `types-aiobotocore-apigatewayv2-2.5.4/types_aiobotocore_apigatewayv2/literals.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -92,14 +92,15 @@
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
@@ -195,14 +196,15 @@
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
@@ -281,26 +283,28 @@
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

### Comparing `types-aiobotocore-apigatewayv2-2.5.2.post3/types_aiobotocore_apigatewayv2/paginator.py` & `types-aiobotocore-apigatewayv2-2.5.4/types_aiobotocore_apigatewayv2/paginator.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-apigatewayv2-2.5.2.post3/types_aiobotocore_apigatewayv2/paginator.pyi` & `types-aiobotocore-apigatewayv2-2.5.4/types_aiobotocore_apigatewayv2/paginator.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-apigatewayv2-2.5.2.post3/types_aiobotocore_apigatewayv2/type_defs.py` & `types-aiobotocore-apigatewayv2-2.5.4/types_aiobotocore_apigatewayv2/type_defs.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-apigatewayv2-2.5.2.post3/types_aiobotocore_apigatewayv2/type_defs.pyi` & `types-aiobotocore-apigatewayv2-2.5.4/types_aiobotocore_apigatewayv2/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-apigatewayv2-2.5.2.post3/types_aiobotocore_apigatewayv2.egg-info/PKG-INFO` & `types-aiobotocore-apigatewayv2-2.5.4/types_aiobotocore_apigatewayv2.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-apigatewayv2
-Version: 2.5.2.post3
-Summary: Type annotations for aiobotocore.ApiGatewayV2 2.5.2 service generated with mypy-boto3-builder 7.17.2
+Version: 2.5.4
+Summary: Type annotations for aiobotocore.ApiGatewayV2 2.5.4 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_apigatewayv2/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-apigatewayv2.svg?color=blue)](https://pypi.org/project/types-aiobotocore-apigatewayv2)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_apigatewayv2/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-apigatewayv2)](https://pepy.tech/project/types-aiobotocore-apigatewayv2)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.ApiGatewayV2 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigatewayv2.html#ApiGatewayV2)
+[aiobotocore.ApiGatewayV2 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigatewayv2.html#ApiGatewayV2)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-apigatewayv2-2.5.2.post3/types_aiobotocore_apigatewayv2.egg-info/SOURCES.txt` & `types-aiobotocore-apigatewayv2-2.5.4/types_aiobotocore_apigatewayv2.egg-info/SOURCES.txt`

 * *Files identical despite different names*


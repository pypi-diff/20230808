# Comparing `tmp/types-aiobotocore-ecr-2.5.2.post3.tar.gz` & `tmp/types-aiobotocore-ecr-2.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-ecr-2.5.2.post3.tar", last modified: Fri Aug  4 12:37:39 2023, max compression
+gzip compressed data, was "types-aiobotocore-ecr-2.5.4.tar", last modified: Tue Aug  8 01:23:39 2023, max compression
```

## Comparing `types-aiobotocore-ecr-2.5.2.post3.tar` & `types-aiobotocore-ecr-2.5.4.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:37:39.167704 types-aiobotocore-ecr-2.5.2.post3/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-04 12:22:53.000000 types-aiobotocore-ecr-2.5.2.post3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    14444 2023-08-04 12:37:39.167704 types-aiobotocore-ecr-2.5.2.post3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    12942 2023-08-04 12:22:53.000000 types-aiobotocore-ecr-2.5.2.post3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-04 12:37:39.167704 types-aiobotocore-ecr-2.5.2.post3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2020 2023-08-04 12:22:53.000000 types-aiobotocore-ecr-2.5.2.post3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:37:39.167704 types-aiobotocore-ecr-2.5.2.post3/types_aiobotocore_ecr/
--rw-r--r--   0 runner    (1001) docker     (123)     2313 2023-08-04 12:22:53.000000 types-aiobotocore-ecr-2.5.2.post3/types_aiobotocore_ecr/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2312 2023-08-04 12:22:53.000000 types-aiobotocore-ecr-2.5.2.post3/types_aiobotocore_ecr/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      916 2023-08-04 12:22:53.000000 types-aiobotocore-ecr-2.5.2.post3/types_aiobotocore_ecr/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    35705 2023-08-04 12:22:53.000000 types-aiobotocore-ecr-2.5.2.post3/types_aiobotocore_ecr/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    35647 2023-08-04 12:22:53.000000 types-aiobotocore-ecr-2.5.2.post3/types_aiobotocore_ecr/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    11110 2023-08-04 12:22:54.000000 types-aiobotocore-ecr-2.5.2.post3/types_aiobotocore_ecr/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    11108 2023-08-04 12:22:54.000000 types-aiobotocore-ecr-2.5.2.post3/types_aiobotocore_ecr/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8549 2023-08-04 12:22:53.000000 types-aiobotocore-ecr-2.5.2.post3/types_aiobotocore_ecr/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     8541 2023-08-04 12:22:53.000000 types-aiobotocore-ecr-2.5.2.post3/types_aiobotocore_ecr/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 12:22:53.000000 types-aiobotocore-ecr-2.5.2.post3/types_aiobotocore_ecr/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    51943 2023-08-04 12:22:55.000000 types-aiobotocore-ecr-2.5.2.post3/types_aiobotocore_ecr/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    51870 2023-08-04 12:22:54.000000 types-aiobotocore-ecr-2.5.2.post3/types_aiobotocore_ecr/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-04 12:22:53.000000 types-aiobotocore-ecr-2.5.2.post3/types_aiobotocore_ecr/version.py
--rw-r--r--   0 runner    (1001) docker     (123)     3106 2023-08-04 12:22:53.000000 types-aiobotocore-ecr-2.5.2.post3/types_aiobotocore_ecr/waiter.py
--rw-r--r--   0 runner    (1001) docker     (123)     3104 2023-08-04 12:22:53.000000 types-aiobotocore-ecr-2.5.2.post3/types_aiobotocore_ecr/waiter.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:37:39.167704 types-aiobotocore-ecr-2.5.2.post3/types_aiobotocore_ecr.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    14444 2023-08-04 12:37:38.000000 types-aiobotocore-ecr-2.5.2.post3/types_aiobotocore_ecr.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      802 2023-08-04 12:37:39.000000 types-aiobotocore-ecr-2.5.2.post3/types_aiobotocore_ecr.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 12:37:38.000000 types-aiobotocore-ecr-2.5.2.post3/types_aiobotocore_ecr.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 12:37:38.000000 types-aiobotocore-ecr-2.5.2.post3/types_aiobotocore_ecr.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-04 12:37:38.000000 types-aiobotocore-ecr-2.5.2.post3/types_aiobotocore_ecr.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-08-04 12:37:38.000000 types-aiobotocore-ecr-2.5.2.post3/types_aiobotocore_ecr.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:23:39.066696 types-aiobotocore-ecr-2.5.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-08 01:10:21.000000 types-aiobotocore-ecr-2.5.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    14438 2023-08-08 01:23:39.066696 types-aiobotocore-ecr-2.5.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    12942 2023-08-08 01:10:21.000000 types-aiobotocore-ecr-2.5.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-08 01:23:39.066696 types-aiobotocore-ecr-2.5.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2014 2023-08-08 01:10:21.000000 types-aiobotocore-ecr-2.5.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:23:39.066696 types-aiobotocore-ecr-2.5.4/types_aiobotocore_ecr/
+-rw-r--r--   0 runner    (1001) docker     (123)     2313 2023-08-08 01:10:21.000000 types-aiobotocore-ecr-2.5.4/types_aiobotocore_ecr/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2312 2023-08-08 01:10:21.000000 types-aiobotocore-ecr-2.5.4/types_aiobotocore_ecr/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      904 2023-08-08 01:10:21.000000 types-aiobotocore-ecr-2.5.4/types_aiobotocore_ecr/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35705 2023-08-08 01:10:21.000000 types-aiobotocore-ecr-2.5.4/types_aiobotocore_ecr/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35647 2023-08-08 01:10:21.000000 types-aiobotocore-ecr-2.5.4/types_aiobotocore_ecr/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    11225 2023-08-08 01:10:21.000000 types-aiobotocore-ecr-2.5.4/types_aiobotocore_ecr/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11223 2023-08-08 01:10:21.000000 types-aiobotocore-ecr-2.5.4/types_aiobotocore_ecr/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8549 2023-08-08 01:10:21.000000 types-aiobotocore-ecr-2.5.4/types_aiobotocore_ecr/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8541 2023-08-08 01:10:21.000000 types-aiobotocore-ecr-2.5.4/types_aiobotocore_ecr/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 01:10:21.000000 types-aiobotocore-ecr-2.5.4/types_aiobotocore_ecr/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    51943 2023-08-08 01:10:22.000000 types-aiobotocore-ecr-2.5.4/types_aiobotocore_ecr/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    51870 2023-08-08 01:10:22.000000 types-aiobotocore-ecr-2.5.4/types_aiobotocore_ecr/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-08-08 01:10:21.000000 types-aiobotocore-ecr-2.5.4/types_aiobotocore_ecr/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3106 2023-08-08 01:10:21.000000 types-aiobotocore-ecr-2.5.4/types_aiobotocore_ecr/waiter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3104 2023-08-08 01:10:21.000000 types-aiobotocore-ecr-2.5.4/types_aiobotocore_ecr/waiter.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:23:39.066696 types-aiobotocore-ecr-2.5.4/types_aiobotocore_ecr.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    14438 2023-08-08 01:23:38.000000 types-aiobotocore-ecr-2.5.4/types_aiobotocore_ecr.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      802 2023-08-08 01:23:38.000000 types-aiobotocore-ecr-2.5.4/types_aiobotocore_ecr.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 01:23:38.000000 types-aiobotocore-ecr-2.5.4/types_aiobotocore_ecr.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 01:23:38.000000 types-aiobotocore-ecr-2.5.4/types_aiobotocore_ecr.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-08 01:23:38.000000 types-aiobotocore-ecr-2.5.4/types_aiobotocore_ecr.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-08-08 01:23:38.000000 types-aiobotocore-ecr-2.5.4/types_aiobotocore_ecr.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-ecr-2.5.2.post3/LICENSE` & `types-aiobotocore-ecr-2.5.4/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-ecr-2.5.2.post3/PKG-INFO` & `types-aiobotocore-ecr-2.5.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-ecr
-Version: 2.5.2.post3
-Summary: Type annotations for aiobotocore.ECR 2.5.2 service generated with mypy-boto3-builder 7.17.2
+Version: 2.5.4
+Summary: Type annotations for aiobotocore.ECR 2.5.4 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ecr/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-ecr.svg?color=blue)](https://pypi.org/project/types-aiobotocore-ecr)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ecr/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-ecr)](https://pepy.tech/project/types-aiobotocore-ecr)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.ECR 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecr.html#ECR)
+[aiobotocore.ECR 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecr.html#ECR)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-ecr-2.5.2.post3/README.md` & `types-aiobotocore-ecr-2.5.4/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-ecr.svg?color=blue)](https://pypi.org/project/types-aiobotocore-ecr)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ecr/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-ecr)](https://pepy.tech/project/types-aiobotocore-ecr)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.ECR 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecr.html#ECR)
+[aiobotocore.ECR 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecr.html#ECR)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-ecr-2.5.2.post3/setup.py` & `types-aiobotocore-ecr-2.5.4/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-ecr",
-    version="2.5.2.post3",
+    version="2.5.4",
     packages=["types_aiobotocore_ecr"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.ECR 2.5.2 service generated with mypy-boto3-builder"
+        "Type annotations for aiobotocore.ECR 2.5.4 service generated with mypy-boto3-builder"
         " 7.17.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
```

### Comparing `types-aiobotocore-ecr-2.5.2.post3/types_aiobotocore_ecr/__init__.py` & `types-aiobotocore-ecr-2.5.4/types_aiobotocore_ecr/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-ecr-2.5.2.post3/types_aiobotocore_ecr/__init__.pyi` & `types-aiobotocore-ecr-2.5.4/types_aiobotocore_ecr/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-ecr-2.5.2.post3/types_aiobotocore_ecr/__main__.py` & `types-aiobotocore-ecr-2.5.4/types_aiobotocore_ecr/__main__.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.ECR 2.5.2\nVersion:         2.5.2.post3\nBuilder version:"
+        "Type annotations for aiobotocore.ECR 2.5.4\nVersion:         2.5.4\nBuilder version:"
         " 7.17.2\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ecr//\nBoto3 docs:    "
         "  https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecr.html#ECR\nOther"
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

### Comparing `types-aiobotocore-ecr-2.5.2.post3/types_aiobotocore_ecr/client.py` & `types-aiobotocore-ecr-2.5.4/types_aiobotocore_ecr/client.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-ecr-2.5.2.post3/types_aiobotocore_ecr/client.pyi` & `types-aiobotocore-ecr-2.5.4/types_aiobotocore_ecr/client.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-ecr-2.5.2.post3/types_aiobotocore_ecr/literals.py` & `types-aiobotocore-ecr-2.5.4/types_aiobotocore_ecr/literals.py`

 * *Files 2% similar despite different names*

```diff
@@ -106,14 +106,15 @@
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
@@ -209,14 +210,15 @@
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
@@ -295,26 +297,28 @@
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
@@ -484,14 +488,15 @@
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

### Comparing `types-aiobotocore-ecr-2.5.2.post3/types_aiobotocore_ecr/literals.pyi` & `types-aiobotocore-ecr-2.5.4/types_aiobotocore_ecr/literals.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -104,14 +104,15 @@
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
@@ -207,14 +208,15 @@
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
@@ -293,26 +295,28 @@
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
@@ -482,14 +486,15 @@
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

### Comparing `types-aiobotocore-ecr-2.5.2.post3/types_aiobotocore_ecr/paginator.py` & `types-aiobotocore-ecr-2.5.4/types_aiobotocore_ecr/paginator.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-ecr-2.5.2.post3/types_aiobotocore_ecr/paginator.pyi` & `types-aiobotocore-ecr-2.5.4/types_aiobotocore_ecr/paginator.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-ecr-2.5.2.post3/types_aiobotocore_ecr/type_defs.py` & `types-aiobotocore-ecr-2.5.4/types_aiobotocore_ecr/type_defs.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-ecr-2.5.2.post3/types_aiobotocore_ecr/type_defs.pyi` & `types-aiobotocore-ecr-2.5.4/types_aiobotocore_ecr/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-ecr-2.5.2.post3/types_aiobotocore_ecr/waiter.py` & `types-aiobotocore-ecr-2.5.4/types_aiobotocore_ecr/waiter.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-ecr-2.5.2.post3/types_aiobotocore_ecr/waiter.pyi` & `types-aiobotocore-ecr-2.5.4/types_aiobotocore_ecr/waiter.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-ecr-2.5.2.post3/types_aiobotocore_ecr.egg-info/PKG-INFO` & `types-aiobotocore-ecr-2.5.4/types_aiobotocore_ecr.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-ecr
-Version: 2.5.2.post3
-Summary: Type annotations for aiobotocore.ECR 2.5.2 service generated with mypy-boto3-builder 7.17.2
+Version: 2.5.4
+Summary: Type annotations for aiobotocore.ECR 2.5.4 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ecr/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-ecr.svg?color=blue)](https://pypi.org/project/types-aiobotocore-ecr)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ecr/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-ecr)](https://pepy.tech/project/types-aiobotocore-ecr)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.ECR 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecr.html#ECR)
+[aiobotocore.ECR 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecr.html#ECR)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-ecr-2.5.2.post3/types_aiobotocore_ecr.egg-info/SOURCES.txt` & `types-aiobotocore-ecr-2.5.4/types_aiobotocore_ecr.egg-info/SOURCES.txt`

 * *Files identical despite different names*


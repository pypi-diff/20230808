# Comparing `tmp/types-aiobotocore-emr-2.5.2.post3.tar.gz` & `tmp/types-aiobotocore-emr-2.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-emr-2.5.2.post3.tar", last modified: Fri Aug  4 12:37:41 2023, max compression
+gzip compressed data, was "types-aiobotocore-emr-2.5.4.tar", last modified: Tue Aug  8 01:23:42 2023, max compression
```

## Comparing `types-aiobotocore-emr-2.5.2.post3.tar` & `types-aiobotocore-emr-2.5.4.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:37:41.959770 types-aiobotocore-emr-2.5.2.post3/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-04 12:23:25.000000 types-aiobotocore-emr-2.5.2.post3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    14950 2023-08-04 12:37:41.951770 types-aiobotocore-emr-2.5.2.post3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    13448 2023-08-04 12:23:25.000000 types-aiobotocore-emr-2.5.2.post3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-04 12:37:41.959770 types-aiobotocore-emr-2.5.2.post3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2020 2023-08-04 12:23:25.000000 types-aiobotocore-emr-2.5.2.post3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:37:41.947770 types-aiobotocore-emr-2.5.2.post3/types_aiobotocore_emr/
--rw-r--r--   0 runner    (1001) docker     (123)     3097 2023-08-04 12:23:25.000000 types-aiobotocore-emr-2.5.2.post3/types_aiobotocore_emr/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3096 2023-08-04 12:23:25.000000 types-aiobotocore-emr-2.5.2.post3/types_aiobotocore_emr/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      916 2023-08-04 12:23:25.000000 types-aiobotocore-emr-2.5.2.post3/types_aiobotocore_emr/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    46357 2023-08-04 12:23:27.000000 types-aiobotocore-emr-2.5.2.post3/types_aiobotocore_emr/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    46281 2023-08-04 12:23:27.000000 types-aiobotocore-emr-2.5.2.post3/types_aiobotocore_emr/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    15745 2023-08-04 12:23:27.000000 types-aiobotocore-emr-2.5.2.post3/types_aiobotocore_emr/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    15743 2023-08-04 12:23:27.000000 types-aiobotocore-emr-2.5.2.post3/types_aiobotocore_emr/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    12801 2023-08-04 12:23:27.000000 types-aiobotocore-emr-2.5.2.post3/types_aiobotocore_emr/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)    12789 2023-08-04 12:23:27.000000 types-aiobotocore-emr-2.5.2.post3/types_aiobotocore_emr/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 12:23:25.000000 types-aiobotocore-emr-2.5.2.post3/types_aiobotocore_emr/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    79599 2023-08-04 12:23:29.000000 types-aiobotocore-emr-2.5.2.post3/types_aiobotocore_emr/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    79493 2023-08-04 12:23:28.000000 types-aiobotocore-emr-2.5.2.post3/types_aiobotocore_emr/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-04 12:23:25.000000 types-aiobotocore-emr-2.5.2.post3/types_aiobotocore_emr/version.py
--rw-r--r--   0 runner    (1001) docker     (123)     3321 2023-08-04 12:23:27.000000 types-aiobotocore-emr-2.5.2.post3/types_aiobotocore_emr/waiter.py
--rw-r--r--   0 runner    (1001) docker     (123)     3318 2023-08-04 12:23:27.000000 types-aiobotocore-emr-2.5.2.post3/types_aiobotocore_emr/waiter.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:37:41.951770 types-aiobotocore-emr-2.5.2.post3/types_aiobotocore_emr.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    14950 2023-08-04 12:37:41.000000 types-aiobotocore-emr-2.5.2.post3/types_aiobotocore_emr.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      802 2023-08-04 12:37:41.000000 types-aiobotocore-emr-2.5.2.post3/types_aiobotocore_emr.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 12:37:41.000000 types-aiobotocore-emr-2.5.2.post3/types_aiobotocore_emr.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 12:37:41.000000 types-aiobotocore-emr-2.5.2.post3/types_aiobotocore_emr.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-04 12:37:41.000000 types-aiobotocore-emr-2.5.2.post3/types_aiobotocore_emr.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-08-04 12:37:41.000000 types-aiobotocore-emr-2.5.2.post3/types_aiobotocore_emr.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:23:42.806712 types-aiobotocore-emr-2.5.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-08 01:10:50.000000 types-aiobotocore-emr-2.5.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    14944 2023-08-08 01:23:42.806712 types-aiobotocore-emr-2.5.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    13448 2023-08-08 01:10:50.000000 types-aiobotocore-emr-2.5.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-08 01:23:42.806712 types-aiobotocore-emr-2.5.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2014 2023-08-08 01:10:50.000000 types-aiobotocore-emr-2.5.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:23:42.794712 types-aiobotocore-emr-2.5.4/types_aiobotocore_emr/
+-rw-r--r--   0 runner    (1001) docker     (123)     3097 2023-08-08 01:10:51.000000 types-aiobotocore-emr-2.5.4/types_aiobotocore_emr/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3096 2023-08-08 01:10:50.000000 types-aiobotocore-emr-2.5.4/types_aiobotocore_emr/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      904 2023-08-08 01:10:51.000000 types-aiobotocore-emr-2.5.4/types_aiobotocore_emr/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46357 2023-08-08 01:10:52.000000 types-aiobotocore-emr-2.5.4/types_aiobotocore_emr/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46281 2023-08-08 01:10:51.000000 types-aiobotocore-emr-2.5.4/types_aiobotocore_emr/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    15860 2023-08-08 01:10:52.000000 types-aiobotocore-emr-2.5.4/types_aiobotocore_emr/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15858 2023-08-08 01:10:52.000000 types-aiobotocore-emr-2.5.4/types_aiobotocore_emr/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    12801 2023-08-08 01:10:52.000000 types-aiobotocore-emr-2.5.4/types_aiobotocore_emr/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12789 2023-08-08 01:10:52.000000 types-aiobotocore-emr-2.5.4/types_aiobotocore_emr/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 01:10:51.000000 types-aiobotocore-emr-2.5.4/types_aiobotocore_emr/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    79599 2023-08-08 01:10:54.000000 types-aiobotocore-emr-2.5.4/types_aiobotocore_emr/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    79493 2023-08-08 01:10:53.000000 types-aiobotocore-emr-2.5.4/types_aiobotocore_emr/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-08-08 01:10:50.000000 types-aiobotocore-emr-2.5.4/types_aiobotocore_emr/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3321 2023-08-08 01:10:52.000000 types-aiobotocore-emr-2.5.4/types_aiobotocore_emr/waiter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3318 2023-08-08 01:10:52.000000 types-aiobotocore-emr-2.5.4/types_aiobotocore_emr/waiter.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:23:42.806712 types-aiobotocore-emr-2.5.4/types_aiobotocore_emr.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    14944 2023-08-08 01:23:42.000000 types-aiobotocore-emr-2.5.4/types_aiobotocore_emr.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      802 2023-08-08 01:23:42.000000 types-aiobotocore-emr-2.5.4/types_aiobotocore_emr.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 01:23:42.000000 types-aiobotocore-emr-2.5.4/types_aiobotocore_emr.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 01:23:42.000000 types-aiobotocore-emr-2.5.4/types_aiobotocore_emr.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-08 01:23:42.000000 types-aiobotocore-emr-2.5.4/types_aiobotocore_emr.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-08-08 01:23:42.000000 types-aiobotocore-emr-2.5.4/types_aiobotocore_emr.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-emr-2.5.2.post3/LICENSE` & `types-aiobotocore-emr-2.5.4/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-emr-2.5.2.post3/PKG-INFO` & `types-aiobotocore-emr-2.5.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-emr
-Version: 2.5.2.post3
-Summary: Type annotations for aiobotocore.EMR 2.5.2 service generated with mypy-boto3-builder 7.17.2
+Version: 2.5.4
+Summary: Type annotations for aiobotocore.EMR 2.5.4 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_emr/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-emr.svg?color=blue)](https://pypi.org/project/types-aiobotocore-emr)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_emr/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-emr)](https://pepy.tech/project/types-aiobotocore-emr)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.EMR 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr.html#EMR)
+[aiobotocore.EMR 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr.html#EMR)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-emr-2.5.2.post3/README.md` & `types-aiobotocore-emr-2.5.4/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-emr.svg?color=blue)](https://pypi.org/project/types-aiobotocore-emr)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_emr/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-emr)](https://pepy.tech/project/types-aiobotocore-emr)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.EMR 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr.html#EMR)
+[aiobotocore.EMR 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr.html#EMR)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-emr-2.5.2.post3/setup.py` & `types-aiobotocore-emr-2.5.4/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-emr",
-    version="2.5.2.post3",
+    version="2.5.4",
     packages=["types_aiobotocore_emr"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.EMR 2.5.2 service generated with mypy-boto3-builder"
+        "Type annotations for aiobotocore.EMR 2.5.4 service generated with mypy-boto3-builder"
         " 7.17.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
```

### Comparing `types-aiobotocore-emr-2.5.2.post3/types_aiobotocore_emr/__init__.py` & `types-aiobotocore-emr-2.5.4/types_aiobotocore_emr/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-emr-2.5.2.post3/types_aiobotocore_emr/__init__.pyi` & `types-aiobotocore-emr-2.5.4/types_aiobotocore_emr/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-emr-2.5.2.post3/types_aiobotocore_emr/client.py` & `types-aiobotocore-emr-2.5.4/types_aiobotocore_emr/client.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-emr-2.5.2.post3/types_aiobotocore_emr/client.pyi` & `types-aiobotocore-emr-2.5.4/types_aiobotocore_emr/client.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-emr-2.5.2.post3/types_aiobotocore_emr/literals.py` & `types-aiobotocore-emr-2.5.4/types_aiobotocore_emr/literals.py`

 * *Files 0% similar despite different names*

```diff
@@ -254,14 +254,15 @@
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
@@ -357,14 +358,15 @@
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
@@ -443,26 +445,28 @@
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
@@ -636,14 +640,15 @@
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

### Comparing `types-aiobotocore-emr-2.5.2.post3/types_aiobotocore_emr/literals.pyi` & `types-aiobotocore-emr-2.5.4/types_aiobotocore_emr/literals.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -252,14 +252,15 @@
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
@@ -355,14 +356,15 @@
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
@@ -441,26 +443,28 @@
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
@@ -634,14 +638,15 @@
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

### Comparing `types-aiobotocore-emr-2.5.2.post3/types_aiobotocore_emr/paginator.py` & `types-aiobotocore-emr-2.5.4/types_aiobotocore_emr/paginator.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-emr-2.5.2.post3/types_aiobotocore_emr/paginator.pyi` & `types-aiobotocore-emr-2.5.4/types_aiobotocore_emr/paginator.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-emr-2.5.2.post3/types_aiobotocore_emr/type_defs.py` & `types-aiobotocore-emr-2.5.4/types_aiobotocore_emr/type_defs.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-emr-2.5.2.post3/types_aiobotocore_emr/type_defs.pyi` & `types-aiobotocore-emr-2.5.4/types_aiobotocore_emr/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-emr-2.5.2.post3/types_aiobotocore_emr/waiter.py` & `types-aiobotocore-emr-2.5.4/types_aiobotocore_emr/waiter.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-emr-2.5.2.post3/types_aiobotocore_emr/waiter.pyi` & `types-aiobotocore-emr-2.5.4/types_aiobotocore_emr/waiter.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-emr-2.5.2.post3/types_aiobotocore_emr.egg-info/PKG-INFO` & `types-aiobotocore-emr-2.5.4/types_aiobotocore_emr.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-emr
-Version: 2.5.2.post3
-Summary: Type annotations for aiobotocore.EMR 2.5.2 service generated with mypy-boto3-builder 7.17.2
+Version: 2.5.4
+Summary: Type annotations for aiobotocore.EMR 2.5.4 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_emr/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-emr.svg?color=blue)](https://pypi.org/project/types-aiobotocore-emr)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_emr/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-emr)](https://pepy.tech/project/types-aiobotocore-emr)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.EMR 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr.html#EMR)
+[aiobotocore.EMR 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr.html#EMR)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-emr-2.5.2.post3/types_aiobotocore_emr.egg-info/SOURCES.txt` & `types-aiobotocore-emr-2.5.4/types_aiobotocore_emr.egg-info/SOURCES.txt`

 * *Files identical despite different names*


# Comparing `tmp/types-aiobotocore-appconfigdata-2.5.2.post3.tar.gz` & `tmp/types-aiobotocore-appconfigdata-2.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-appconfigdata-2.5.2.post3.tar", last modified: Fri Aug  4 12:37:16 2023, max compression
+gzip compressed data, was "types-aiobotocore-appconfigdata-2.5.4.tar", last modified: Tue Aug  8 01:23:16 2023, max compression
```

## Comparing `types-aiobotocore-appconfigdata-2.5.2.post3.tar` & `types-aiobotocore-appconfigdata-2.5.4.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:37:16.315167 types-aiobotocore-appconfigdata-2.5.2.post3/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-04 12:18:18.000000 types-aiobotocore-appconfigdata-2.5.2.post3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    12562 2023-08-04 12:37:16.315167 types-aiobotocore-appconfigdata-2.5.2.post3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    11020 2023-08-04 12:18:18.000000 types-aiobotocore-appconfigdata-2.5.2.post3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-04 12:37:16.315167 types-aiobotocore-appconfigdata-2.5.2.post3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2114 2023-08-04 12:18:18.000000 types-aiobotocore-appconfigdata-2.5.2.post3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:37:16.303166 types-aiobotocore-appconfigdata-2.5.2.post3/types_aiobotocore_appconfigdata/
--rw-r--r--   0 runner    (1001) docker     (123)      490 2023-08-04 12:18:18.000000 types-aiobotocore-appconfigdata-2.5.2.post3/types_aiobotocore_appconfigdata/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      489 2023-08-04 12:18:18.000000 types-aiobotocore-appconfigdata-2.5.2.post3/types_aiobotocore_appconfigdata/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      967 2023-08-04 12:18:18.000000 types-aiobotocore-appconfigdata-2.5.2.post3/types_aiobotocore_appconfigdata/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5572 2023-08-04 12:18:18.000000 types-aiobotocore-appconfigdata-2.5.2.post3/types_aiobotocore_appconfigdata/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     5562 2023-08-04 12:18:18.000000 types-aiobotocore-appconfigdata-2.5.2.post3/types_aiobotocore_appconfigdata/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8110 2023-08-04 12:18:18.000000 types-aiobotocore-appconfigdata-2.5.2.post3/types_aiobotocore_appconfigdata/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     8108 2023-08-04 12:18:18.000000 types-aiobotocore-appconfigdata-2.5.2.post3/types_aiobotocore_appconfigdata/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 12:18:18.000000 types-aiobotocore-appconfigdata-2.5.2.post3/types_aiobotocore_appconfigdata/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     2453 2023-08-04 12:18:18.000000 types-aiobotocore-appconfigdata-2.5.2.post3/types_aiobotocore_appconfigdata/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)     2450 2023-08-04 12:18:18.000000 types-aiobotocore-appconfigdata-2.5.2.post3/types_aiobotocore_appconfigdata/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-04 12:18:18.000000 types-aiobotocore-appconfigdata-2.5.2.post3/types_aiobotocore_appconfigdata/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:37:16.315167 types-aiobotocore-appconfigdata-2.5.2.post3/types_aiobotocore_appconfigdata.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    12562 2023-08-04 12:37:16.000000 types-aiobotocore-appconfigdata-2.5.2.post3/types_aiobotocore_appconfigdata.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      836 2023-08-04 12:37:16.000000 types-aiobotocore-appconfigdata-2.5.2.post3/types_aiobotocore_appconfigdata.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 12:37:16.000000 types-aiobotocore-appconfigdata-2.5.2.post3/types_aiobotocore_appconfigdata.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 12:37:16.000000 types-aiobotocore-appconfigdata-2.5.2.post3/types_aiobotocore_appconfigdata.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-04 12:37:16.000000 types-aiobotocore-appconfigdata-2.5.2.post3/types_aiobotocore_appconfigdata.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-08-04 12:37:16.000000 types-aiobotocore-appconfigdata-2.5.2.post3/types_aiobotocore_appconfigdata.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:23:16.042495 types-aiobotocore-appconfigdata-2.5.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-08 01:06:04.000000 types-aiobotocore-appconfigdata-2.5.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    12556 2023-08-08 01:23:16.034495 types-aiobotocore-appconfigdata-2.5.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    11020 2023-08-08 01:06:04.000000 types-aiobotocore-appconfigdata-2.5.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-08 01:23:16.042495 types-aiobotocore-appconfigdata-2.5.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2108 2023-08-08 01:06:04.000000 types-aiobotocore-appconfigdata-2.5.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:23:16.026495 types-aiobotocore-appconfigdata-2.5.4/types_aiobotocore_appconfigdata/
+-rw-r--r--   0 runner    (1001) docker     (123)      490 2023-08-08 01:06:04.000000 types-aiobotocore-appconfigdata-2.5.4/types_aiobotocore_appconfigdata/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      489 2023-08-08 01:06:04.000000 types-aiobotocore-appconfigdata-2.5.4/types_aiobotocore_appconfigdata/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      955 2023-08-08 01:06:04.000000 types-aiobotocore-appconfigdata-2.5.4/types_aiobotocore_appconfigdata/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5572 2023-08-08 01:06:04.000000 types-aiobotocore-appconfigdata-2.5.4/types_aiobotocore_appconfigdata/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5562 2023-08-08 01:06:04.000000 types-aiobotocore-appconfigdata-2.5.4/types_aiobotocore_appconfigdata/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8225 2023-08-08 01:06:04.000000 types-aiobotocore-appconfigdata-2.5.4/types_aiobotocore_appconfigdata/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8223 2023-08-08 01:06:04.000000 types-aiobotocore-appconfigdata-2.5.4/types_aiobotocore_appconfigdata/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 01:06:04.000000 types-aiobotocore-appconfigdata-2.5.4/types_aiobotocore_appconfigdata/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     2453 2023-08-08 01:06:04.000000 types-aiobotocore-appconfigdata-2.5.4/types_aiobotocore_appconfigdata/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2450 2023-08-08 01:06:04.000000 types-aiobotocore-appconfigdata-2.5.4/types_aiobotocore_appconfigdata/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-08-08 01:06:04.000000 types-aiobotocore-appconfigdata-2.5.4/types_aiobotocore_appconfigdata/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:23:16.034495 types-aiobotocore-appconfigdata-2.5.4/types_aiobotocore_appconfigdata.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    12556 2023-08-08 01:23:15.000000 types-aiobotocore-appconfigdata-2.5.4/types_aiobotocore_appconfigdata.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      836 2023-08-08 01:23:15.000000 types-aiobotocore-appconfigdata-2.5.4/types_aiobotocore_appconfigdata.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 01:23:15.000000 types-aiobotocore-appconfigdata-2.5.4/types_aiobotocore_appconfigdata.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 01:23:15.000000 types-aiobotocore-appconfigdata-2.5.4/types_aiobotocore_appconfigdata.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-08 01:23:15.000000 types-aiobotocore-appconfigdata-2.5.4/types_aiobotocore_appconfigdata.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-08-08 01:23:15.000000 types-aiobotocore-appconfigdata-2.5.4/types_aiobotocore_appconfigdata.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-appconfigdata-2.5.2.post3/LICENSE` & `types-aiobotocore-appconfigdata-2.5.4/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-appconfigdata-2.5.2.post3/PKG-INFO` & `types-aiobotocore-appconfigdata-2.5.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-appconfigdata
-Version: 2.5.2.post3
-Summary: Type annotations for aiobotocore.AppConfigData 2.5.2 service generated with mypy-boto3-builder 7.17.2
+Version: 2.5.4
+Summary: Type annotations for aiobotocore.AppConfigData 2.5.4 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appconfigdata/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-appconfigdata.svg?color=blue)](https://pypi.org/project/types-aiobotocore-appconfigdata)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appconfigdata/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-appconfigdata)](https://pepy.tech/project/types-aiobotocore-appconfigdata)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.AppConfigData 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appconfigdata.html#AppConfigData)
+[aiobotocore.AppConfigData 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appconfigdata.html#AppConfigData)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-appconfigdata-2.5.2.post3/README.md` & `types-aiobotocore-appconfigdata-2.5.4/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-appconfigdata.svg?color=blue)](https://pypi.org/project/types-aiobotocore-appconfigdata)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appconfigdata/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-appconfigdata)](https://pepy.tech/project/types-aiobotocore-appconfigdata)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.AppConfigData 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appconfigdata.html#AppConfigData)
+[aiobotocore.AppConfigData 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appconfigdata.html#AppConfigData)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-appconfigdata-2.5.2.post3/setup.py` & `types-aiobotocore-appconfigdata-2.5.4/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-appconfigdata",
-    version="2.5.2.post3",
+    version="2.5.4",
     packages=["types_aiobotocore_appconfigdata"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.AppConfigData 2.5.2 service generated with"
+        "Type annotations for aiobotocore.AppConfigData 2.5.4 service generated with"
         " mypy-boto3-builder 7.17.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
```

### Comparing `types-aiobotocore-appconfigdata-2.5.2.post3/types_aiobotocore_appconfigdata/client.py` & `types-aiobotocore-appconfigdata-2.5.4/types_aiobotocore_appconfigdata/client.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-appconfigdata-2.5.2.post3/types_aiobotocore_appconfigdata/client.pyi` & `types-aiobotocore-appconfigdata-2.5.4/types_aiobotocore_appconfigdata/client.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-appconfigdata-2.5.2.post3/types_aiobotocore_appconfigdata/literals.py` & `types-aiobotocore-appconfigdata-2.5.4/types_aiobotocore_appconfigdata/literals.py`

 * *Files 2% similar despite different names*

```diff
@@ -34,14 +34,15 @@
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
@@ -137,14 +138,15 @@
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
@@ -223,26 +225,28 @@
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
@@ -403,14 +407,15 @@
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

### Comparing `types-aiobotocore-appconfigdata-2.5.2.post3/types_aiobotocore_appconfigdata/literals.pyi` & `types-aiobotocore-appconfigdata-2.5.4/types_aiobotocore_appconfigdata/literals.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -32,14 +32,15 @@
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
@@ -135,14 +136,15 @@
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
@@ -221,26 +223,28 @@
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
@@ -401,14 +405,15 @@
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

### Comparing `types-aiobotocore-appconfigdata-2.5.2.post3/types_aiobotocore_appconfigdata/type_defs.py` & `types-aiobotocore-appconfigdata-2.5.4/types_aiobotocore_appconfigdata/type_defs.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-appconfigdata-2.5.2.post3/types_aiobotocore_appconfigdata/type_defs.pyi` & `types-aiobotocore-appconfigdata-2.5.4/types_aiobotocore_appconfigdata/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-appconfigdata-2.5.2.post3/types_aiobotocore_appconfigdata.egg-info/PKG-INFO` & `types-aiobotocore-appconfigdata-2.5.4/types_aiobotocore_appconfigdata.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-appconfigdata
-Version: 2.5.2.post3
-Summary: Type annotations for aiobotocore.AppConfigData 2.5.2 service generated with mypy-boto3-builder 7.17.2
+Version: 2.5.4
+Summary: Type annotations for aiobotocore.AppConfigData 2.5.4 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appconfigdata/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-appconfigdata.svg?color=blue)](https://pypi.org/project/types-aiobotocore-appconfigdata)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appconfigdata/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-appconfigdata)](https://pepy.tech/project/types-aiobotocore-appconfigdata)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.AppConfigData 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appconfigdata.html#AppConfigData)
+[aiobotocore.AppConfigData 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appconfigdata.html#AppConfigData)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-appconfigdata-2.5.2.post3/types_aiobotocore_appconfigdata.egg-info/SOURCES.txt` & `types-aiobotocore-appconfigdata-2.5.4/types_aiobotocore_appconfigdata.egg-info/SOURCES.txt`

 * *Files identical despite different names*


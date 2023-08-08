# Comparing `tmp/types-aiobotocore-firehose-2.5.2.post3.tar.gz` & `tmp/types-aiobotocore-firehose-2.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-firehose-2.5.2.post3.tar", last modified: Fri Aug  4 12:37:44 2023, max compression
+gzip compressed data, was "types-aiobotocore-firehose-2.5.4.tar", last modified: Tue Aug  8 01:23:44 2023, max compression
```

## Comparing `types-aiobotocore-firehose-2.5.2.post3.tar` & `types-aiobotocore-firehose-2.5.4.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:37:44.287824 types-aiobotocore-firehose-2.5.2.post3/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-04 12:23:47.000000 types-aiobotocore-firehose-2.5.2.post3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    12341 2023-08-04 12:37:44.287824 types-aiobotocore-firehose-2.5.2.post3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    10819 2023-08-04 12:23:47.000000 types-aiobotocore-firehose-2.5.2.post3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-04 12:37:44.287824 types-aiobotocore-firehose-2.5.2.post3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2079 2023-08-04 12:23:47.000000 types-aiobotocore-firehose-2.5.2.post3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:37:44.283825 types-aiobotocore-firehose-2.5.2.post3/types_aiobotocore_firehose/
--rw-r--r--   0 runner    (1001) docker     (123)      450 2023-08-04 12:23:47.000000 types-aiobotocore-firehose-2.5.2.post3/types_aiobotocore_firehose/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      449 2023-08-04 12:23:47.000000 types-aiobotocore-firehose-2.5.2.post3/types_aiobotocore_firehose/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      947 2023-08-04 12:23:47.000000 types-aiobotocore-firehose-2.5.2.post3/types_aiobotocore_firehose/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14113 2023-08-04 12:23:47.000000 types-aiobotocore-firehose-2.5.2.post3/types_aiobotocore_firehose/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    14093 2023-08-04 12:23:47.000000 types-aiobotocore-firehose-2.5.2.post3/types_aiobotocore_firehose/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    11308 2023-08-04 12:23:47.000000 types-aiobotocore-firehose-2.5.2.post3/types_aiobotocore_firehose/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    11306 2023-08-04 12:23:47.000000 types-aiobotocore-firehose-2.5.2.post3/types_aiobotocore_firehose/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 12:23:47.000000 types-aiobotocore-firehose-2.5.2.post3/types_aiobotocore_firehose/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    45062 2023-08-04 12:23:48.000000 types-aiobotocore-firehose-2.5.2.post3/types_aiobotocore_firehose/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    45013 2023-08-04 12:23:48.000000 types-aiobotocore-firehose-2.5.2.post3/types_aiobotocore_firehose/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-04 12:23:47.000000 types-aiobotocore-firehose-2.5.2.post3/types_aiobotocore_firehose/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:37:44.283825 types-aiobotocore-firehose-2.5.2.post3/types_aiobotocore_firehose.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    12341 2023-08-04 12:37:44.000000 types-aiobotocore-firehose-2.5.2.post3/types_aiobotocore_firehose.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      751 2023-08-04 12:37:44.000000 types-aiobotocore-firehose-2.5.2.post3/types_aiobotocore_firehose.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 12:37:44.000000 types-aiobotocore-firehose-2.5.2.post3/types_aiobotocore_firehose.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 12:37:44.000000 types-aiobotocore-firehose-2.5.2.post3/types_aiobotocore_firehose.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-04 12:37:44.000000 types-aiobotocore-firehose-2.5.2.post3/types_aiobotocore_firehose.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-08-04 12:37:44.000000 types-aiobotocore-firehose-2.5.2.post3/types_aiobotocore_firehose.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:23:44.014716 types-aiobotocore-firehose-2.5.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-08 01:11:12.000000 types-aiobotocore-firehose-2.5.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    12335 2023-08-08 01:23:44.014716 types-aiobotocore-firehose-2.5.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10819 2023-08-08 01:11:12.000000 types-aiobotocore-firehose-2.5.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-08 01:23:44.014716 types-aiobotocore-firehose-2.5.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2073 2023-08-08 01:11:12.000000 types-aiobotocore-firehose-2.5.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:23:44.006716 types-aiobotocore-firehose-2.5.4/types_aiobotocore_firehose/
+-rw-r--r--   0 runner    (1001) docker     (123)      450 2023-08-08 01:11:12.000000 types-aiobotocore-firehose-2.5.4/types_aiobotocore_firehose/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      449 2023-08-08 01:11:12.000000 types-aiobotocore-firehose-2.5.4/types_aiobotocore_firehose/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      935 2023-08-08 01:11:12.000000 types-aiobotocore-firehose-2.5.4/types_aiobotocore_firehose/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14113 2023-08-08 01:11:12.000000 types-aiobotocore-firehose-2.5.4/types_aiobotocore_firehose/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14093 2023-08-08 01:11:12.000000 types-aiobotocore-firehose-2.5.4/types_aiobotocore_firehose/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    11423 2023-08-08 01:11:12.000000 types-aiobotocore-firehose-2.5.4/types_aiobotocore_firehose/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11421 2023-08-08 01:11:12.000000 types-aiobotocore-firehose-2.5.4/types_aiobotocore_firehose/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 01:11:12.000000 types-aiobotocore-firehose-2.5.4/types_aiobotocore_firehose/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    45062 2023-08-08 01:11:13.000000 types-aiobotocore-firehose-2.5.4/types_aiobotocore_firehose/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    45013 2023-08-08 01:11:13.000000 types-aiobotocore-firehose-2.5.4/types_aiobotocore_firehose/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-08-08 01:11:12.000000 types-aiobotocore-firehose-2.5.4/types_aiobotocore_firehose/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:23:44.014716 types-aiobotocore-firehose-2.5.4/types_aiobotocore_firehose.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    12335 2023-08-08 01:23:43.000000 types-aiobotocore-firehose-2.5.4/types_aiobotocore_firehose.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      751 2023-08-08 01:23:43.000000 types-aiobotocore-firehose-2.5.4/types_aiobotocore_firehose.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 01:23:43.000000 types-aiobotocore-firehose-2.5.4/types_aiobotocore_firehose.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 01:23:43.000000 types-aiobotocore-firehose-2.5.4/types_aiobotocore_firehose.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-08 01:23:43.000000 types-aiobotocore-firehose-2.5.4/types_aiobotocore_firehose.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-08-08 01:23:43.000000 types-aiobotocore-firehose-2.5.4/types_aiobotocore_firehose.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-firehose-2.5.2.post3/LICENSE` & `types-aiobotocore-firehose-2.5.4/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-firehose-2.5.2.post3/PKG-INFO` & `types-aiobotocore-firehose-2.5.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-firehose
-Version: 2.5.2.post3
-Summary: Type annotations for aiobotocore.Firehose 2.5.2 service generated with mypy-boto3-builder 7.17.2
+Version: 2.5.4
+Summary: Type annotations for aiobotocore.Firehose 2.5.4 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_firehose/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-firehose.svg?color=blue)](https://pypi.org/project/types-aiobotocore-firehose)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_firehose/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-firehose)](https://pepy.tech/project/types-aiobotocore-firehose)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.Firehose 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/firehose.html#Firehose)
+[aiobotocore.Firehose 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/firehose.html#Firehose)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-firehose-2.5.2.post3/README.md` & `types-aiobotocore-firehose-2.5.4/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-firehose.svg?color=blue)](https://pypi.org/project/types-aiobotocore-firehose)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_firehose/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-firehose)](https://pepy.tech/project/types-aiobotocore-firehose)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.Firehose 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/firehose.html#Firehose)
+[aiobotocore.Firehose 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/firehose.html#Firehose)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-firehose-2.5.2.post3/setup.py` & `types-aiobotocore-firehose-2.5.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-firehose",
-    version="2.5.2.post3",
+    version="2.5.4",
     packages=["types_aiobotocore_firehose"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.Firehose 2.5.2 service generated with mypy-boto3-builder"
+        "Type annotations for aiobotocore.Firehose 2.5.4 service generated with mypy-boto3-builder"
         " 7.17.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
```

### Comparing `types-aiobotocore-firehose-2.5.2.post3/types_aiobotocore_firehose/__main__.py` & `types-aiobotocore-firehose-2.5.4/types_aiobotocore_firehose/__main__.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.Firehose 2.5.2\nVersion:         2.5.2.post3\nBuilder"
-        " version: 7.17.2\nDocs:           "
+        "Type annotations for aiobotocore.Firehose 2.5.4\nVersion:         2.5.4\nBuilder version:"
+        " 7.17.2\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_firehose//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/firehose.html#Firehose\nOther"
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

### Comparing `types-aiobotocore-firehose-2.5.2.post3/types_aiobotocore_firehose/client.py` & `types-aiobotocore-firehose-2.5.4/types_aiobotocore_firehose/client.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-firehose-2.5.2.post3/types_aiobotocore_firehose/client.pyi` & `types-aiobotocore-firehose-2.5.4/types_aiobotocore_firehose/client.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-firehose-2.5.2.post3/types_aiobotocore_firehose/literals.py` & `types-aiobotocore-firehose-2.5.4/types_aiobotocore_firehose/literals.py`

 * *Files 0% similar despite different names*

```diff
@@ -123,14 +123,15 @@
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
@@ -226,14 +227,15 @@
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
@@ -312,26 +314,28 @@
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
@@ -492,14 +496,15 @@
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

### Comparing `types-aiobotocore-firehose-2.5.2.post3/types_aiobotocore_firehose/literals.pyi` & `types-aiobotocore-firehose-2.5.4/types_aiobotocore_firehose/literals.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -121,14 +121,15 @@
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
@@ -224,14 +225,15 @@
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
@@ -310,26 +312,28 @@
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
@@ -490,14 +494,15 @@
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

### Comparing `types-aiobotocore-firehose-2.5.2.post3/types_aiobotocore_firehose/type_defs.py` & `types-aiobotocore-firehose-2.5.4/types_aiobotocore_firehose/type_defs.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-firehose-2.5.2.post3/types_aiobotocore_firehose/type_defs.pyi` & `types-aiobotocore-firehose-2.5.4/types_aiobotocore_firehose/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-firehose-2.5.2.post3/types_aiobotocore_firehose.egg-info/PKG-INFO` & `types-aiobotocore-firehose-2.5.4/types_aiobotocore_firehose.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-firehose
-Version: 2.5.2.post3
-Summary: Type annotations for aiobotocore.Firehose 2.5.2 service generated with mypy-boto3-builder 7.17.2
+Version: 2.5.4
+Summary: Type annotations for aiobotocore.Firehose 2.5.4 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_firehose/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-firehose.svg?color=blue)](https://pypi.org/project/types-aiobotocore-firehose)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_firehose/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-firehose)](https://pepy.tech/project/types-aiobotocore-firehose)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.Firehose 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/firehose.html#Firehose)
+[aiobotocore.Firehose 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/firehose.html#Firehose)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-firehose-2.5.2.post3/types_aiobotocore_firehose.egg-info/SOURCES.txt` & `types-aiobotocore-firehose-2.5.4/types_aiobotocore_firehose.egg-info/SOURCES.txt`

 * *Files identical despite different names*


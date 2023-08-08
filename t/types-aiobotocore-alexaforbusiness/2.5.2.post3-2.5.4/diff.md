# Comparing `tmp/types-aiobotocore-alexaforbusiness-2.5.2.post3.tar.gz` & `tmp/types-aiobotocore-alexaforbusiness-2.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-alexaforbusiness-2.5.2.post3.tar", last modified: Fri Aug  4 12:37:13 2023, max compression
+gzip compressed data, was "types-aiobotocore-alexaforbusiness-2.5.4.tar", last modified: Tue Aug  8 01:23:11 2023, max compression
```

## Comparing `types-aiobotocore-alexaforbusiness-2.5.2.post3.tar` & `types-aiobotocore-alexaforbusiness-2.5.4.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:37:13.491096 types-aiobotocore-alexaforbusiness-2.5.2.post3/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-04 12:17:54.000000 types-aiobotocore-alexaforbusiness-2.5.2.post3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    15293 2023-08-04 12:37:13.491096 types-aiobotocore-alexaforbusiness-2.5.2.post3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    13739 2023-08-04 12:17:54.000000 types-aiobotocore-alexaforbusiness-2.5.2.post3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-04 12:37:13.491096 types-aiobotocore-alexaforbusiness-2.5.2.post3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2135 2023-08-04 12:17:53.000000 types-aiobotocore-alexaforbusiness-2.5.2.post3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:37:13.479096 types-aiobotocore-alexaforbusiness-2.5.2.post3/types_aiobotocore_alexaforbusiness/
--rw-r--r--   0 runner    (1001) docker     (123)     3331 2023-08-04 12:17:54.000000 types-aiobotocore-alexaforbusiness-2.5.2.post3/types_aiobotocore_alexaforbusiness/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3330 2023-08-04 12:17:54.000000 types-aiobotocore-alexaforbusiness-2.5.2.post3/types_aiobotocore_alexaforbusiness/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      979 2023-08-04 12:17:54.000000 types-aiobotocore-alexaforbusiness-2.5.2.post3/types_aiobotocore_alexaforbusiness/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    71050 2023-08-04 12:17:54.000000 types-aiobotocore-alexaforbusiness-2.5.2.post3/types_aiobotocore_alexaforbusiness/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    70935 2023-08-04 12:17:54.000000 types-aiobotocore-alexaforbusiness-2.5.2.post3/types_aiobotocore_alexaforbusiness/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    12605 2023-08-04 12:17:54.000000 types-aiobotocore-alexaforbusiness-2.5.2.post3/types_aiobotocore_alexaforbusiness/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    12603 2023-08-04 12:17:54.000000 types-aiobotocore-alexaforbusiness-2.5.2.post3/types_aiobotocore_alexaforbusiness/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    17038 2023-08-04 12:17:54.000000 types-aiobotocore-alexaforbusiness-2.5.2.post3/types_aiobotocore_alexaforbusiness/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)    17023 2023-08-04 12:17:54.000000 types-aiobotocore-alexaforbusiness-2.5.2.post3/types_aiobotocore_alexaforbusiness/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 12:17:54.000000 types-aiobotocore-alexaforbusiness-2.5.2.post3/types_aiobotocore_alexaforbusiness/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    71421 2023-08-04 12:17:57.000000 types-aiobotocore-alexaforbusiness-2.5.2.post3/types_aiobotocore_alexaforbusiness/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    71346 2023-08-04 12:17:55.000000 types-aiobotocore-alexaforbusiness-2.5.2.post3/types_aiobotocore_alexaforbusiness/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-04 12:17:54.000000 types-aiobotocore-alexaforbusiness-2.5.2.post3/types_aiobotocore_alexaforbusiness/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:37:13.491096 types-aiobotocore-alexaforbusiness-2.5.2.post3/types_aiobotocore_alexaforbusiness.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    15293 2023-08-04 12:37:13.000000 types-aiobotocore-alexaforbusiness-2.5.2.post3/types_aiobotocore_alexaforbusiness.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      984 2023-08-04 12:37:13.000000 types-aiobotocore-alexaforbusiness-2.5.2.post3/types_aiobotocore_alexaforbusiness.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 12:37:13.000000 types-aiobotocore-alexaforbusiness-2.5.2.post3/types_aiobotocore_alexaforbusiness.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 12:37:13.000000 types-aiobotocore-alexaforbusiness-2.5.2.post3/types_aiobotocore_alexaforbusiness.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-04 12:37:13.000000 types-aiobotocore-alexaforbusiness-2.5.2.post3/types_aiobotocore_alexaforbusiness.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-08-04 12:37:13.000000 types-aiobotocore-alexaforbusiness-2.5.2.post3/types_aiobotocore_alexaforbusiness.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:23:11.870483 types-aiobotocore-alexaforbusiness-2.5.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-08 01:05:42.000000 types-aiobotocore-alexaforbusiness-2.5.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    15287 2023-08-08 01:23:11.866483 types-aiobotocore-alexaforbusiness-2.5.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    13739 2023-08-08 01:05:42.000000 types-aiobotocore-alexaforbusiness-2.5.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-08 01:23:11.870483 types-aiobotocore-alexaforbusiness-2.5.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2129 2023-08-08 01:05:42.000000 types-aiobotocore-alexaforbusiness-2.5.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:23:11.862483 types-aiobotocore-alexaforbusiness-2.5.4/types_aiobotocore_alexaforbusiness/
+-rw-r--r--   0 runner    (1001) docker     (123)     3331 2023-08-08 01:05:42.000000 types-aiobotocore-alexaforbusiness-2.5.4/types_aiobotocore_alexaforbusiness/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3330 2023-08-08 01:05:42.000000 types-aiobotocore-alexaforbusiness-2.5.4/types_aiobotocore_alexaforbusiness/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      967 2023-08-08 01:05:42.000000 types-aiobotocore-alexaforbusiness-2.5.4/types_aiobotocore_alexaforbusiness/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    71050 2023-08-08 01:05:42.000000 types-aiobotocore-alexaforbusiness-2.5.4/types_aiobotocore_alexaforbusiness/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    70935 2023-08-08 01:05:42.000000 types-aiobotocore-alexaforbusiness-2.5.4/types_aiobotocore_alexaforbusiness/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    12700 2023-08-08 01:05:43.000000 types-aiobotocore-alexaforbusiness-2.5.4/types_aiobotocore_alexaforbusiness/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12698 2023-08-08 01:05:42.000000 types-aiobotocore-alexaforbusiness-2.5.4/types_aiobotocore_alexaforbusiness/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    17038 2023-08-08 01:05:42.000000 types-aiobotocore-alexaforbusiness-2.5.4/types_aiobotocore_alexaforbusiness/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17023 2023-08-08 01:05:42.000000 types-aiobotocore-alexaforbusiness-2.5.4/types_aiobotocore_alexaforbusiness/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 01:05:42.000000 types-aiobotocore-alexaforbusiness-2.5.4/types_aiobotocore_alexaforbusiness/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    71421 2023-08-08 01:05:44.000000 types-aiobotocore-alexaforbusiness-2.5.4/types_aiobotocore_alexaforbusiness/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    71346 2023-08-08 01:05:43.000000 types-aiobotocore-alexaforbusiness-2.5.4/types_aiobotocore_alexaforbusiness/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-08-08 01:05:42.000000 types-aiobotocore-alexaforbusiness-2.5.4/types_aiobotocore_alexaforbusiness/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:23:11.866483 types-aiobotocore-alexaforbusiness-2.5.4/types_aiobotocore_alexaforbusiness.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    15287 2023-08-08 01:23:11.000000 types-aiobotocore-alexaforbusiness-2.5.4/types_aiobotocore_alexaforbusiness.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      984 2023-08-08 01:23:11.000000 types-aiobotocore-alexaforbusiness-2.5.4/types_aiobotocore_alexaforbusiness.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 01:23:11.000000 types-aiobotocore-alexaforbusiness-2.5.4/types_aiobotocore_alexaforbusiness.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 01:23:11.000000 types-aiobotocore-alexaforbusiness-2.5.4/types_aiobotocore_alexaforbusiness.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-08 01:23:11.000000 types-aiobotocore-alexaforbusiness-2.5.4/types_aiobotocore_alexaforbusiness.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-08-08 01:23:11.000000 types-aiobotocore-alexaforbusiness-2.5.4/types_aiobotocore_alexaforbusiness.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-alexaforbusiness-2.5.2.post3/LICENSE` & `types-aiobotocore-alexaforbusiness-2.5.4/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-alexaforbusiness-2.5.2.post3/PKG-INFO` & `types-aiobotocore-alexaforbusiness-2.5.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-alexaforbusiness
-Version: 2.5.2.post3
-Summary: Type annotations for aiobotocore.AlexaForBusiness 2.5.2 service generated with mypy-boto3-builder 7.17.2
+Version: 2.5.4
+Summary: Type annotations for aiobotocore.AlexaForBusiness 2.5.4 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_alexaforbusiness/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-alexaforbusiness.svg?color=blue)](https://pypi.org/project/types-aiobotocore-alexaforbusiness)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_alexaforbusiness/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-alexaforbusiness)](https://pepy.tech/project/types-aiobotocore-alexaforbusiness)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.AlexaForBusiness 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/alexaforbusiness.html#AlexaForBusiness)
+[aiobotocore.AlexaForBusiness 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/alexaforbusiness.html#AlexaForBusiness)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-alexaforbusiness-2.5.2.post3/README.md` & `types-aiobotocore-alexaforbusiness-2.5.4/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-alexaforbusiness.svg?color=blue)](https://pypi.org/project/types-aiobotocore-alexaforbusiness)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_alexaforbusiness/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-alexaforbusiness)](https://pepy.tech/project/types-aiobotocore-alexaforbusiness)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.AlexaForBusiness 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/alexaforbusiness.html#AlexaForBusiness)
+[aiobotocore.AlexaForBusiness 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/alexaforbusiness.html#AlexaForBusiness)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-alexaforbusiness-2.5.2.post3/setup.py` & `types-aiobotocore-alexaforbusiness-2.5.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-alexaforbusiness",
-    version="2.5.2.post3",
+    version="2.5.4",
     packages=["types_aiobotocore_alexaforbusiness"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.AlexaForBusiness 2.5.2 service generated with"
+        "Type annotations for aiobotocore.AlexaForBusiness 2.5.4 service generated with"
         " mypy-boto3-builder 7.17.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
```

### Comparing `types-aiobotocore-alexaforbusiness-2.5.2.post3/types_aiobotocore_alexaforbusiness/__init__.py` & `types-aiobotocore-alexaforbusiness-2.5.4/types_aiobotocore_alexaforbusiness/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-alexaforbusiness-2.5.2.post3/types_aiobotocore_alexaforbusiness/__init__.pyi` & `types-aiobotocore-alexaforbusiness-2.5.4/types_aiobotocore_alexaforbusiness/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-alexaforbusiness-2.5.2.post3/types_aiobotocore_alexaforbusiness/__main__.py` & `types-aiobotocore-alexaforbusiness-2.5.4/types_aiobotocore_alexaforbusiness/__main__.py`

 * *Files 23% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.AlexaForBusiness 2.5.2\nVersion:        "
-        " 2.5.2.post3\nBuilder version: 7.17.2\nDocs:           "
+        "Type annotations for aiobotocore.AlexaForBusiness 2.5.4\nVersion:         2.5.4\nBuilder"
+        " version: 7.17.2\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_alexaforbusiness//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/alexaforbusiness.html#AlexaForBusiness\nOther"
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

### Comparing `types-aiobotocore-alexaforbusiness-2.5.2.post3/types_aiobotocore_alexaforbusiness/client.py` & `types-aiobotocore-alexaforbusiness-2.5.4/types_aiobotocore_alexaforbusiness/client.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-alexaforbusiness-2.5.2.post3/types_aiobotocore_alexaforbusiness/client.pyi` & `types-aiobotocore-alexaforbusiness-2.5.4/types_aiobotocore_alexaforbusiness/client.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-alexaforbusiness-2.5.2.post3/types_aiobotocore_alexaforbusiness/literals.py` & `types-aiobotocore-alexaforbusiness-2.5.4/types_aiobotocore_alexaforbusiness/literals.py`

 * *Files 1% similar despite different names*

```diff
@@ -157,14 +157,15 @@
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
@@ -260,14 +261,15 @@
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
@@ -346,26 +348,28 @@
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

### Comparing `types-aiobotocore-alexaforbusiness-2.5.2.post3/types_aiobotocore_alexaforbusiness/literals.pyi` & `types-aiobotocore-alexaforbusiness-2.5.4/types_aiobotocore_alexaforbusiness/literals.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -155,14 +155,15 @@
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
@@ -258,14 +259,15 @@
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
@@ -344,26 +346,28 @@
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

### Comparing `types-aiobotocore-alexaforbusiness-2.5.2.post3/types_aiobotocore_alexaforbusiness/paginator.py` & `types-aiobotocore-alexaforbusiness-2.5.4/types_aiobotocore_alexaforbusiness/paginator.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-alexaforbusiness-2.5.2.post3/types_aiobotocore_alexaforbusiness/paginator.pyi` & `types-aiobotocore-alexaforbusiness-2.5.4/types_aiobotocore_alexaforbusiness/paginator.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-alexaforbusiness-2.5.2.post3/types_aiobotocore_alexaforbusiness/type_defs.py` & `types-aiobotocore-alexaforbusiness-2.5.4/types_aiobotocore_alexaforbusiness/type_defs.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-alexaforbusiness-2.5.2.post3/types_aiobotocore_alexaforbusiness/type_defs.pyi` & `types-aiobotocore-alexaforbusiness-2.5.4/types_aiobotocore_alexaforbusiness/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-alexaforbusiness-2.5.2.post3/types_aiobotocore_alexaforbusiness.egg-info/PKG-INFO` & `types-aiobotocore-alexaforbusiness-2.5.4/types_aiobotocore_alexaforbusiness.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-alexaforbusiness
-Version: 2.5.2.post3
-Summary: Type annotations for aiobotocore.AlexaForBusiness 2.5.2 service generated with mypy-boto3-builder 7.17.2
+Version: 2.5.4
+Summary: Type annotations for aiobotocore.AlexaForBusiness 2.5.4 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_alexaforbusiness/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-alexaforbusiness.svg?color=blue)](https://pypi.org/project/types-aiobotocore-alexaforbusiness)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_alexaforbusiness/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-alexaforbusiness)](https://pepy.tech/project/types-aiobotocore-alexaforbusiness)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.AlexaForBusiness 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/alexaforbusiness.html#AlexaForBusiness)
+[aiobotocore.AlexaForBusiness 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/alexaforbusiness.html#AlexaForBusiness)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-alexaforbusiness-2.5.2.post3/types_aiobotocore_alexaforbusiness.egg-info/SOURCES.txt` & `types-aiobotocore-alexaforbusiness-2.5.4/types_aiobotocore_alexaforbusiness.egg-info/SOURCES.txt`

 * *Files identical despite different names*


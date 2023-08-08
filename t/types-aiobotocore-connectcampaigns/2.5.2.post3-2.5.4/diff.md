# Comparing `tmp/types-aiobotocore-connectcampaigns-2.5.2.post3.tar.gz` & `tmp/types-aiobotocore-connectcampaigns-2.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-connectcampaigns-2.5.2.post3.tar", last modified: Fri Aug  4 12:37:31 2023, max compression
+gzip compressed data, was "types-aiobotocore-connectcampaigns-2.5.4.tar", last modified: Tue Aug  8 01:23:33 2023, max compression
```

## Comparing `types-aiobotocore-connectcampaigns-2.5.2.post3.tar` & `types-aiobotocore-connectcampaigns-2.5.4.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:37:31.699526 types-aiobotocore-connectcampaigns-2.5.2.post3/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-04 12:20:58.000000 types-aiobotocore-connectcampaigns-2.5.2.post3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    13518 2023-08-04 12:37:31.699526 types-aiobotocore-connectcampaigns-2.5.2.post3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    11958 2023-08-04 12:20:58.000000 types-aiobotocore-connectcampaigns-2.5.2.post3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-04 12:37:31.699526 types-aiobotocore-connectcampaigns-2.5.2.post3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2141 2023-08-04 12:20:58.000000 types-aiobotocore-connectcampaigns-2.5.2.post3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:37:31.699526 types-aiobotocore-connectcampaigns-2.5.2.post3/types_aiobotocore_connectcampaigns/
--rw-r--r--   0 runner    (1001) docker     (123)      743 2023-08-04 12:20:58.000000 types-aiobotocore-connectcampaigns-2.5.2.post3/types_aiobotocore_connectcampaigns/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      742 2023-08-04 12:20:58.000000 types-aiobotocore-connectcampaigns-2.5.2.post3/types_aiobotocore_connectcampaigns/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      991 2023-08-04 12:20:58.000000 types-aiobotocore-connectcampaigns-2.5.2.post3/types_aiobotocore_connectcampaigns/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18370 2023-08-04 12:20:58.000000 types-aiobotocore-connectcampaigns-2.5.2.post3/types_aiobotocore_connectcampaigns/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    18338 2023-08-04 12:20:58.000000 types-aiobotocore-connectcampaigns-2.5.2.post3/types_aiobotocore_connectcampaigns/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8730 2023-08-04 12:20:59.000000 types-aiobotocore-connectcampaigns-2.5.2.post3/types_aiobotocore_connectcampaigns/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     8728 2023-08-04 12:20:59.000000 types-aiobotocore-connectcampaigns-2.5.2.post3/types_aiobotocore_connectcampaigns/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2195 2023-08-04 12:20:58.000000 types-aiobotocore-connectcampaigns-2.5.2.post3/types_aiobotocore_connectcampaigns/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     2192 2023-08-04 12:20:58.000000 types-aiobotocore-connectcampaigns-2.5.2.post3/types_aiobotocore_connectcampaigns/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 12:20:58.000000 types-aiobotocore-connectcampaigns-2.5.2.post3/types_aiobotocore_connectcampaigns/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    15124 2023-08-04 12:20:59.000000 types-aiobotocore-connectcampaigns-2.5.2.post3/types_aiobotocore_connectcampaigns/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    15111 2023-08-04 12:20:59.000000 types-aiobotocore-connectcampaigns-2.5.2.post3/types_aiobotocore_connectcampaigns/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-04 12:20:58.000000 types-aiobotocore-connectcampaigns-2.5.2.post3/types_aiobotocore_connectcampaigns/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:37:31.699526 types-aiobotocore-connectcampaigns-2.5.2.post3/types_aiobotocore_connectcampaigns.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    13518 2023-08-04 12:37:31.000000 types-aiobotocore-connectcampaigns-2.5.2.post3/types_aiobotocore_connectcampaigns.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      984 2023-08-04 12:37:31.000000 types-aiobotocore-connectcampaigns-2.5.2.post3/types_aiobotocore_connectcampaigns.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 12:37:31.000000 types-aiobotocore-connectcampaigns-2.5.2.post3/types_aiobotocore_connectcampaigns.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 12:37:31.000000 types-aiobotocore-connectcampaigns-2.5.2.post3/types_aiobotocore_connectcampaigns.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-04 12:37:31.000000 types-aiobotocore-connectcampaigns-2.5.2.post3/types_aiobotocore_connectcampaigns.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-08-04 12:37:31.000000 types-aiobotocore-connectcampaigns-2.5.2.post3/types_aiobotocore_connectcampaigns.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:23:33.530676 types-aiobotocore-connectcampaigns-2.5.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-08 01:08:34.000000 types-aiobotocore-connectcampaigns-2.5.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    13512 2023-08-08 01:23:33.522676 types-aiobotocore-connectcampaigns-2.5.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    11958 2023-08-08 01:08:34.000000 types-aiobotocore-connectcampaigns-2.5.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-08 01:23:33.530676 types-aiobotocore-connectcampaigns-2.5.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2135 2023-08-08 01:08:34.000000 types-aiobotocore-connectcampaigns-2.5.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:23:33.522676 types-aiobotocore-connectcampaigns-2.5.4/types_aiobotocore_connectcampaigns/
+-rw-r--r--   0 runner    (1001) docker     (123)      743 2023-08-08 01:08:34.000000 types-aiobotocore-connectcampaigns-2.5.4/types_aiobotocore_connectcampaigns/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      742 2023-08-08 01:08:34.000000 types-aiobotocore-connectcampaigns-2.5.4/types_aiobotocore_connectcampaigns/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      979 2023-08-08 01:08:34.000000 types-aiobotocore-connectcampaigns-2.5.4/types_aiobotocore_connectcampaigns/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18370 2023-08-08 01:08:35.000000 types-aiobotocore-connectcampaigns-2.5.4/types_aiobotocore_connectcampaigns/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18338 2023-08-08 01:08:34.000000 types-aiobotocore-connectcampaigns-2.5.4/types_aiobotocore_connectcampaigns/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8825 2023-08-08 01:08:35.000000 types-aiobotocore-connectcampaigns-2.5.4/types_aiobotocore_connectcampaigns/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8823 2023-08-08 01:08:35.000000 types-aiobotocore-connectcampaigns-2.5.4/types_aiobotocore_connectcampaigns/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2195 2023-08-08 01:08:35.000000 types-aiobotocore-connectcampaigns-2.5.4/types_aiobotocore_connectcampaigns/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2192 2023-08-08 01:08:35.000000 types-aiobotocore-connectcampaigns-2.5.4/types_aiobotocore_connectcampaigns/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 01:08:34.000000 types-aiobotocore-connectcampaigns-2.5.4/types_aiobotocore_connectcampaigns/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    15124 2023-08-08 01:08:36.000000 types-aiobotocore-connectcampaigns-2.5.4/types_aiobotocore_connectcampaigns/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15111 2023-08-08 01:08:36.000000 types-aiobotocore-connectcampaigns-2.5.4/types_aiobotocore_connectcampaigns/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-08-08 01:08:34.000000 types-aiobotocore-connectcampaigns-2.5.4/types_aiobotocore_connectcampaigns/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:23:33.522676 types-aiobotocore-connectcampaigns-2.5.4/types_aiobotocore_connectcampaigns.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    13512 2023-08-08 01:23:33.000000 types-aiobotocore-connectcampaigns-2.5.4/types_aiobotocore_connectcampaigns.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      984 2023-08-08 01:23:33.000000 types-aiobotocore-connectcampaigns-2.5.4/types_aiobotocore_connectcampaigns.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 01:23:33.000000 types-aiobotocore-connectcampaigns-2.5.4/types_aiobotocore_connectcampaigns.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 01:23:33.000000 types-aiobotocore-connectcampaigns-2.5.4/types_aiobotocore_connectcampaigns.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-08 01:23:33.000000 types-aiobotocore-connectcampaigns-2.5.4/types_aiobotocore_connectcampaigns.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-08-08 01:23:33.000000 types-aiobotocore-connectcampaigns-2.5.4/types_aiobotocore_connectcampaigns.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-connectcampaigns-2.5.2.post3/LICENSE` & `types-aiobotocore-connectcampaigns-2.5.4/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-connectcampaigns-2.5.2.post3/PKG-INFO` & `types-aiobotocore-connectcampaigns-2.5.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-connectcampaigns
-Version: 2.5.2.post3
-Summary: Type annotations for aiobotocore.ConnectCampaignService 2.5.2 service generated with mypy-boto3-builder 7.17.2
+Version: 2.5.4
+Summary: Type annotations for aiobotocore.ConnectCampaignService 2.5.4 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_connectcampaigns/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-connectcampaigns.svg?color=blue)](https://pypi.org/project/types-aiobotocore-connectcampaigns)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_connectcampaigns/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-connectcampaigns)](https://pepy.tech/project/types-aiobotocore-connectcampaigns)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.ConnectCampaignService 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connectcampaigns.html#ConnectCampaignService)
+[aiobotocore.ConnectCampaignService 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connectcampaigns.html#ConnectCampaignService)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-connectcampaigns-2.5.2.post3/README.md` & `types-aiobotocore-connectcampaigns-2.5.4/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-connectcampaigns.svg?color=blue)](https://pypi.org/project/types-aiobotocore-connectcampaigns)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_connectcampaigns/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-connectcampaigns)](https://pepy.tech/project/types-aiobotocore-connectcampaigns)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.ConnectCampaignService 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connectcampaigns.html#ConnectCampaignService)
+[aiobotocore.ConnectCampaignService 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connectcampaigns.html#ConnectCampaignService)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-connectcampaigns-2.5.2.post3/setup.py` & `types-aiobotocore-connectcampaigns-2.5.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-connectcampaigns",
-    version="2.5.2.post3",
+    version="2.5.4",
     packages=["types_aiobotocore_connectcampaigns"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.ConnectCampaignService 2.5.2 service generated with"
+        "Type annotations for aiobotocore.ConnectCampaignService 2.5.4 service generated with"
         " mypy-boto3-builder 7.17.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
```

### Comparing `types-aiobotocore-connectcampaigns-2.5.2.post3/types_aiobotocore_connectcampaigns/__init__.py` & `types-aiobotocore-connectcampaigns-2.5.4/types_aiobotocore_connectcampaigns/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-connectcampaigns-2.5.2.post3/types_aiobotocore_connectcampaigns/__init__.pyi` & `types-aiobotocore-connectcampaigns-2.5.4/types_aiobotocore_connectcampaigns/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-connectcampaigns-2.5.2.post3/types_aiobotocore_connectcampaigns/__main__.py` & `types-aiobotocore-connectcampaigns-2.5.4/types_aiobotocore_connectcampaigns/__main__.py`

 * *Files 10% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.ConnectCampaignService 2.5.2\nVersion:        "
-        " 2.5.2.post3\nBuilder version: 7.17.2\nDocs:           "
+        "Type annotations for aiobotocore.ConnectCampaignService 2.5.4\nVersion:        "
+        " 2.5.4\nBuilder version: 7.17.2\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_connectcampaigns//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connectcampaigns.html#ConnectCampaignService\nOther"
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

### Comparing `types-aiobotocore-connectcampaigns-2.5.2.post3/types_aiobotocore_connectcampaigns/client.py` & `types-aiobotocore-connectcampaigns-2.5.4/types_aiobotocore_connectcampaigns/client.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-connectcampaigns-2.5.2.post3/types_aiobotocore_connectcampaigns/client.pyi` & `types-aiobotocore-connectcampaigns-2.5.4/types_aiobotocore_connectcampaigns/client.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-connectcampaigns-2.5.2.post3/types_aiobotocore_connectcampaigns/literals.py` & `types-aiobotocore-connectcampaigns-2.5.4/types_aiobotocore_connectcampaigns/literals.py`

 * *Files 0% similar despite different names*

```diff
@@ -63,14 +63,15 @@
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
@@ -166,14 +167,15 @@
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
@@ -252,26 +254,28 @@
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

### Comparing `types-aiobotocore-connectcampaigns-2.5.2.post3/types_aiobotocore_connectcampaigns/literals.pyi` & `types-aiobotocore-connectcampaigns-2.5.4/types_aiobotocore_connectcampaigns/literals.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -61,14 +61,15 @@
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
@@ -164,14 +165,15 @@
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
@@ -250,26 +252,28 @@
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

### Comparing `types-aiobotocore-connectcampaigns-2.5.2.post3/types_aiobotocore_connectcampaigns/paginator.py` & `types-aiobotocore-connectcampaigns-2.5.4/types_aiobotocore_connectcampaigns/paginator.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-connectcampaigns-2.5.2.post3/types_aiobotocore_connectcampaigns/paginator.pyi` & `types-aiobotocore-connectcampaigns-2.5.4/types_aiobotocore_connectcampaigns/paginator.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-connectcampaigns-2.5.2.post3/types_aiobotocore_connectcampaigns/type_defs.py` & `types-aiobotocore-connectcampaigns-2.5.4/types_aiobotocore_connectcampaigns/type_defs.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-connectcampaigns-2.5.2.post3/types_aiobotocore_connectcampaigns/type_defs.pyi` & `types-aiobotocore-connectcampaigns-2.5.4/types_aiobotocore_connectcampaigns/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-connectcampaigns-2.5.2.post3/types_aiobotocore_connectcampaigns.egg-info/PKG-INFO` & `types-aiobotocore-connectcampaigns-2.5.4/types_aiobotocore_connectcampaigns.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-connectcampaigns
-Version: 2.5.2.post3
-Summary: Type annotations for aiobotocore.ConnectCampaignService 2.5.2 service generated with mypy-boto3-builder 7.17.2
+Version: 2.5.4
+Summary: Type annotations for aiobotocore.ConnectCampaignService 2.5.4 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_connectcampaigns/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-connectcampaigns.svg?color=blue)](https://pypi.org/project/types-aiobotocore-connectcampaigns)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_connectcampaigns/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-connectcampaigns)](https://pepy.tech/project/types-aiobotocore-connectcampaigns)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.ConnectCampaignService 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connectcampaigns.html#ConnectCampaignService)
+[aiobotocore.ConnectCampaignService 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connectcampaigns.html#ConnectCampaignService)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-connectcampaigns-2.5.2.post3/types_aiobotocore_connectcampaigns.egg-info/SOURCES.txt` & `types-aiobotocore-connectcampaigns-2.5.4/types_aiobotocore_connectcampaigns.egg-info/SOURCES.txt`

 * *Files identical despite different names*


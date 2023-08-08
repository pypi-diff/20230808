# Comparing `tmp/types-aiobotocore-gamesparks-2.5.2.post3.tar.gz` & `tmp/types-aiobotocore-gamesparks-2.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-gamesparks-2.5.2.post3.tar", last modified: Fri Aug  4 12:37:46 2023, max compression
+gzip compressed data, was "types-aiobotocore-gamesparks-2.5.4.tar", last modified: Tue Aug  8 01:23:45 2023, max compression
```

## Comparing `types-aiobotocore-gamesparks-2.5.2.post3.tar` & `types-aiobotocore-gamesparks-2.5.4.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:37:46.215870 types-aiobotocore-gamesparks-2.5.2.post3/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-04 12:24:14.000000 types-aiobotocore-gamesparks-2.5.2.post3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    13915 2023-08-04 12:37:46.215870 types-aiobotocore-gamesparks-2.5.2.post3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    12385 2023-08-04 12:24:14.000000 types-aiobotocore-gamesparks-2.5.2.post3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-04 12:37:46.215870 types-aiobotocore-gamesparks-2.5.2.post3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2093 2023-08-04 12:24:14.000000 types-aiobotocore-gamesparks-2.5.2.post3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:37:46.207869 types-aiobotocore-gamesparks-2.5.2.post3/types_aiobotocore_gamesparks/
--rw-r--r--   0 runner    (1001) docker     (123)     1903 2023-08-04 12:24:14.000000 types-aiobotocore-gamesparks-2.5.2.post3/types_aiobotocore_gamesparks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1902 2023-08-04 12:24:14.000000 types-aiobotocore-gamesparks-2.5.2.post3/types_aiobotocore_gamesparks/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      955 2023-08-04 12:24:14.000000 types-aiobotocore-gamesparks-2.5.2.post3/types_aiobotocore_gamesparks/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    26620 2023-08-04 12:24:14.000000 types-aiobotocore-gamesparks-2.5.2.post3/types_aiobotocore_gamesparks/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    26571 2023-08-04 12:24:14.000000 types-aiobotocore-gamesparks-2.5.2.post3/types_aiobotocore_gamesparks/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9131 2023-08-04 12:24:15.000000 types-aiobotocore-gamesparks-2.5.2.post3/types_aiobotocore_gamesparks/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     9129 2023-08-04 12:24:14.000000 types-aiobotocore-gamesparks-2.5.2.post3/types_aiobotocore_gamesparks/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8713 2023-08-04 12:24:14.000000 types-aiobotocore-gamesparks-2.5.2.post3/types_aiobotocore_gamesparks/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     8704 2023-08-04 12:24:14.000000 types-aiobotocore-gamesparks-2.5.2.post3/types_aiobotocore_gamesparks/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 12:24:14.000000 types-aiobotocore-gamesparks-2.5.2.post3/types_aiobotocore_gamesparks/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    29844 2023-08-04 12:24:15.000000 types-aiobotocore-gamesparks-2.5.2.post3/types_aiobotocore_gamesparks/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    29801 2023-08-04 12:24:15.000000 types-aiobotocore-gamesparks-2.5.2.post3/types_aiobotocore_gamesparks/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-04 12:24:14.000000 types-aiobotocore-gamesparks-2.5.2.post3/types_aiobotocore_gamesparks/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:37:46.215870 types-aiobotocore-gamesparks-2.5.2.post3/types_aiobotocore_gamesparks.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    13915 2023-08-04 12:37:46.000000 types-aiobotocore-gamesparks-2.5.2.post3/types_aiobotocore_gamesparks.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      870 2023-08-04 12:37:46.000000 types-aiobotocore-gamesparks-2.5.2.post3/types_aiobotocore_gamesparks.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 12:37:46.000000 types-aiobotocore-gamesparks-2.5.2.post3/types_aiobotocore_gamesparks.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 12:37:46.000000 types-aiobotocore-gamesparks-2.5.2.post3/types_aiobotocore_gamesparks.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-04 12:37:46.000000 types-aiobotocore-gamesparks-2.5.2.post3/types_aiobotocore_gamesparks.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-08-04 12:37:46.000000 types-aiobotocore-gamesparks-2.5.2.post3/types_aiobotocore_gamesparks.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:23:45.830721 types-aiobotocore-gamesparks-2.5.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-08 01:11:36.000000 types-aiobotocore-gamesparks-2.5.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    13909 2023-08-08 01:23:45.830721 types-aiobotocore-gamesparks-2.5.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    12385 2023-08-08 01:11:36.000000 types-aiobotocore-gamesparks-2.5.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-08 01:23:45.830721 types-aiobotocore-gamesparks-2.5.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2087 2023-08-08 01:11:36.000000 types-aiobotocore-gamesparks-2.5.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:23:45.826721 types-aiobotocore-gamesparks-2.5.4/types_aiobotocore_gamesparks/
+-rw-r--r--   0 runner    (1001) docker     (123)     1903 2023-08-08 01:11:36.000000 types-aiobotocore-gamesparks-2.5.4/types_aiobotocore_gamesparks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1902 2023-08-08 01:11:36.000000 types-aiobotocore-gamesparks-2.5.4/types_aiobotocore_gamesparks/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      943 2023-08-08 01:11:36.000000 types-aiobotocore-gamesparks-2.5.4/types_aiobotocore_gamesparks/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26620 2023-08-08 01:11:36.000000 types-aiobotocore-gamesparks-2.5.4/types_aiobotocore_gamesparks/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26571 2023-08-08 01:11:36.000000 types-aiobotocore-gamesparks-2.5.4/types_aiobotocore_gamesparks/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9226 2023-08-08 01:11:37.000000 types-aiobotocore-gamesparks-2.5.4/types_aiobotocore_gamesparks/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9224 2023-08-08 01:11:37.000000 types-aiobotocore-gamesparks-2.5.4/types_aiobotocore_gamesparks/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8713 2023-08-08 01:11:37.000000 types-aiobotocore-gamesparks-2.5.4/types_aiobotocore_gamesparks/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8704 2023-08-08 01:11:37.000000 types-aiobotocore-gamesparks-2.5.4/types_aiobotocore_gamesparks/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 01:11:36.000000 types-aiobotocore-gamesparks-2.5.4/types_aiobotocore_gamesparks/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    29844 2023-08-08 01:11:37.000000 types-aiobotocore-gamesparks-2.5.4/types_aiobotocore_gamesparks/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29801 2023-08-08 01:11:37.000000 types-aiobotocore-gamesparks-2.5.4/types_aiobotocore_gamesparks/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-08-08 01:11:36.000000 types-aiobotocore-gamesparks-2.5.4/types_aiobotocore_gamesparks/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:23:45.830721 types-aiobotocore-gamesparks-2.5.4/types_aiobotocore_gamesparks.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    13909 2023-08-08 01:23:45.000000 types-aiobotocore-gamesparks-2.5.4/types_aiobotocore_gamesparks.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      870 2023-08-08 01:23:45.000000 types-aiobotocore-gamesparks-2.5.4/types_aiobotocore_gamesparks.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 01:23:45.000000 types-aiobotocore-gamesparks-2.5.4/types_aiobotocore_gamesparks.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 01:23:45.000000 types-aiobotocore-gamesparks-2.5.4/types_aiobotocore_gamesparks.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-08 01:23:45.000000 types-aiobotocore-gamesparks-2.5.4/types_aiobotocore_gamesparks.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-08-08 01:23:45.000000 types-aiobotocore-gamesparks-2.5.4/types_aiobotocore_gamesparks.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-gamesparks-2.5.2.post3/LICENSE` & `types-aiobotocore-gamesparks-2.5.4/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-gamesparks-2.5.2.post3/PKG-INFO` & `types-aiobotocore-gamesparks-2.5.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-gamesparks
-Version: 2.5.2.post3
-Summary: Type annotations for aiobotocore.GameSparks 2.5.2 service generated with mypy-boto3-builder 7.17.2
+Version: 2.5.4
+Summary: Type annotations for aiobotocore.GameSparks 2.5.4 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_gamesparks/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-gamesparks.svg?color=blue)](https://pypi.org/project/types-aiobotocore-gamesparks)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_gamesparks/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-gamesparks)](https://pepy.tech/project/types-aiobotocore-gamesparks)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.GameSparks 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamesparks.html#GameSparks)
+[aiobotocore.GameSparks 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamesparks.html#GameSparks)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-gamesparks-2.5.2.post3/README.md` & `types-aiobotocore-gamesparks-2.5.4/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-gamesparks.svg?color=blue)](https://pypi.org/project/types-aiobotocore-gamesparks)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_gamesparks/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-gamesparks)](https://pepy.tech/project/types-aiobotocore-gamesparks)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.GameSparks 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamesparks.html#GameSparks)
+[aiobotocore.GameSparks 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamesparks.html#GameSparks)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-gamesparks-2.5.2.post3/setup.py` & `types-aiobotocore-gamesparks-2.5.4/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-gamesparks",
-    version="2.5.2.post3",
+    version="2.5.4",
     packages=["types_aiobotocore_gamesparks"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.GameSparks 2.5.2 service generated with"
+        "Type annotations for aiobotocore.GameSparks 2.5.4 service generated with"
         " mypy-boto3-builder 7.17.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
```

### Comparing `types-aiobotocore-gamesparks-2.5.2.post3/types_aiobotocore_gamesparks/__init__.py` & `types-aiobotocore-gamesparks-2.5.4/types_aiobotocore_gamesparks/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-gamesparks-2.5.2.post3/types_aiobotocore_gamesparks/__init__.pyi` & `types-aiobotocore-gamesparks-2.5.4/types_aiobotocore_gamesparks/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-gamesparks-2.5.2.post3/types_aiobotocore_gamesparks/__main__.py` & `types-aiobotocore-gamesparks-2.5.4/types_aiobotocore_gamesparks/__main__.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.GameSparks 2.5.2\nVersion:         2.5.2.post3\nBuilder"
+        "Type annotations for aiobotocore.GameSparks 2.5.4\nVersion:         2.5.4\nBuilder"
         " version: 7.17.2\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_gamesparks//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamesparks.html#GameSparks\nOther"
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

### Comparing `types-aiobotocore-gamesparks-2.5.2.post3/types_aiobotocore_gamesparks/client.py` & `types-aiobotocore-gamesparks-2.5.4/types_aiobotocore_gamesparks/client.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-gamesparks-2.5.2.post3/types_aiobotocore_gamesparks/client.pyi` & `types-aiobotocore-gamesparks-2.5.4/types_aiobotocore_gamesparks/client.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-gamesparks-2.5.2.post3/types_aiobotocore_gamesparks/literals.py` & `types-aiobotocore-gamesparks-2.5.4/types_aiobotocore_gamesparks/literals.py`

 * *Files 1% similar despite different names*

```diff
@@ -68,14 +68,15 @@
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
@@ -171,14 +172,15 @@
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
@@ -257,26 +259,28 @@
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

### Comparing `types-aiobotocore-gamesparks-2.5.2.post3/types_aiobotocore_gamesparks/literals.pyi` & `types-aiobotocore-gamesparks-2.5.4/types_aiobotocore_gamesparks/literals.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -66,14 +66,15 @@
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
@@ -169,14 +170,15 @@
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
@@ -255,26 +257,28 @@
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

### Comparing `types-aiobotocore-gamesparks-2.5.2.post3/types_aiobotocore_gamesparks/paginator.py` & `types-aiobotocore-gamesparks-2.5.4/types_aiobotocore_gamesparks/paginator.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-gamesparks-2.5.2.post3/types_aiobotocore_gamesparks/paginator.pyi` & `types-aiobotocore-gamesparks-2.5.4/types_aiobotocore_gamesparks/paginator.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-gamesparks-2.5.2.post3/types_aiobotocore_gamesparks/type_defs.py` & `types-aiobotocore-gamesparks-2.5.4/types_aiobotocore_gamesparks/type_defs.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-gamesparks-2.5.2.post3/types_aiobotocore_gamesparks/type_defs.pyi` & `types-aiobotocore-gamesparks-2.5.4/types_aiobotocore_gamesparks/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-gamesparks-2.5.2.post3/types_aiobotocore_gamesparks.egg-info/PKG-INFO` & `types-aiobotocore-gamesparks-2.5.4/types_aiobotocore_gamesparks.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-gamesparks
-Version: 2.5.2.post3
-Summary: Type annotations for aiobotocore.GameSparks 2.5.2 service generated with mypy-boto3-builder 7.17.2
+Version: 2.5.4
+Summary: Type annotations for aiobotocore.GameSparks 2.5.4 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_gamesparks/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-gamesparks.svg?color=blue)](https://pypi.org/project/types-aiobotocore-gamesparks)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_gamesparks/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-gamesparks)](https://pepy.tech/project/types-aiobotocore-gamesparks)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.GameSparks 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamesparks.html#GameSparks)
+[aiobotocore.GameSparks 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamesparks.html#GameSparks)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-gamesparks-2.5.2.post3/types_aiobotocore_gamesparks.egg-info/SOURCES.txt` & `types-aiobotocore-gamesparks-2.5.4/types_aiobotocore_gamesparks.egg-info/SOURCES.txt`

 * *Files identical despite different names*


# Comparing `tmp/types-aiobotocore-applicationcostprofiler-2.5.2.post3.tar.gz` & `tmp/types-aiobotocore-applicationcostprofiler-2.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-applicationcostprofiler-2.5.2.post3.tar", last modified: Fri Aug  4 12:37:17 2023, max compression
+gzip compressed data, was "types-aiobotocore-applicationcostprofiler-2.5.4.tar", last modified: Tue Aug  8 01:23:19 2023, max compression
```

## Comparing `types-aiobotocore-applicationcostprofiler-2.5.2.post3.tar` & `types-aiobotocore-applicationcostprofiler-2.5.4.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:37:17.491196 types-aiobotocore-applicationcostprofiler-2.5.2.post3/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-04 12:18:25.000000 types-aiobotocore-applicationcostprofiler-2.5.2.post3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    13924 2023-08-04 12:37:17.491196 types-aiobotocore-applicationcostprofiler-2.5.2.post3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    12342 2023-08-04 12:18:25.000000 types-aiobotocore-applicationcostprofiler-2.5.2.post3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-04 12:37:17.491196 types-aiobotocore-applicationcostprofiler-2.5.2.post3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2176 2023-08-04 12:18:25.000000 types-aiobotocore-applicationcostprofiler-2.5.2.post3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:37:17.491196 types-aiobotocore-applicationcostprofiler-2.5.2.post3/types_aiobotocore_applicationcostprofiler/
--rw-r--r--   0 runner    (1001) docker     (123)      819 2023-08-04 12:18:25.000000 types-aiobotocore-applicationcostprofiler-2.5.2.post3/types_aiobotocore_applicationcostprofiler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      818 2023-08-04 12:18:25.000000 types-aiobotocore-applicationcostprofiler-2.5.2.post3/types_aiobotocore_applicationcostprofiler/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1007 2023-08-04 12:18:25.000000 types-aiobotocore-applicationcostprofiler-2.5.2.post3/types_aiobotocore_applicationcostprofiler/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9517 2023-08-04 12:18:25.000000 types-aiobotocore-applicationcostprofiler-2.5.2.post3/types_aiobotocore_applicationcostprofiler/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     9501 2023-08-04 12:18:25.000000 types-aiobotocore-applicationcostprofiler-2.5.2.post3/types_aiobotocore_applicationcostprofiler/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8033 2023-08-04 12:18:25.000000 types-aiobotocore-applicationcostprofiler-2.5.2.post3/types_aiobotocore_applicationcostprofiler/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     8031 2023-08-04 12:18:25.000000 types-aiobotocore-applicationcostprofiler-2.5.2.post3/types_aiobotocore_applicationcostprofiler/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2269 2023-08-04 12:18:25.000000 types-aiobotocore-applicationcostprofiler-2.5.2.post3/types_aiobotocore_applicationcostprofiler/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     2266 2023-08-04 12:18:25.000000 types-aiobotocore-applicationcostprofiler-2.5.2.post3/types_aiobotocore_applicationcostprofiler/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 12:18:25.000000 types-aiobotocore-applicationcostprofiler-2.5.2.post3/types_aiobotocore_applicationcostprofiler/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     5661 2023-08-04 12:18:25.000000 types-aiobotocore-applicationcostprofiler-2.5.2.post3/types_aiobotocore_applicationcostprofiler/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)     5658 2023-08-04 12:18:25.000000 types-aiobotocore-applicationcostprofiler-2.5.2.post3/types_aiobotocore_applicationcostprofiler/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-04 12:18:25.000000 types-aiobotocore-applicationcostprofiler-2.5.2.post3/types_aiobotocore_applicationcostprofiler/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:37:17.491196 types-aiobotocore-applicationcostprofiler-2.5.2.post3/types_aiobotocore_applicationcostprofiler.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    13924 2023-08-04 12:37:17.000000 types-aiobotocore-applicationcostprofiler-2.5.2.post3/types_aiobotocore_applicationcostprofiler.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1117 2023-08-04 12:37:17.000000 types-aiobotocore-applicationcostprofiler-2.5.2.post3/types_aiobotocore_applicationcostprofiler.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 12:37:17.000000 types-aiobotocore-applicationcostprofiler-2.5.2.post3/types_aiobotocore_applicationcostprofiler.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 12:37:17.000000 types-aiobotocore-applicationcostprofiler-2.5.2.post3/types_aiobotocore_applicationcostprofiler.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-04 12:37:17.000000 types-aiobotocore-applicationcostprofiler-2.5.2.post3/types_aiobotocore_applicationcostprofiler.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-08-04 12:37:17.000000 types-aiobotocore-applicationcostprofiler-2.5.2.post3/types_aiobotocore_applicationcostprofiler.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:23:19.210516 types-aiobotocore-applicationcostprofiler-2.5.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-08 01:06:13.000000 types-aiobotocore-applicationcostprofiler-2.5.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    13918 2023-08-08 01:23:19.202515 types-aiobotocore-applicationcostprofiler-2.5.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    12342 2023-08-08 01:06:13.000000 types-aiobotocore-applicationcostprofiler-2.5.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-08 01:23:19.210516 types-aiobotocore-applicationcostprofiler-2.5.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2170 2023-08-08 01:06:13.000000 types-aiobotocore-applicationcostprofiler-2.5.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:23:19.202515 types-aiobotocore-applicationcostprofiler-2.5.4/types_aiobotocore_applicationcostprofiler/
+-rw-r--r--   0 runner    (1001) docker     (123)      819 2023-08-08 01:06:13.000000 types-aiobotocore-applicationcostprofiler-2.5.4/types_aiobotocore_applicationcostprofiler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      818 2023-08-08 01:06:13.000000 types-aiobotocore-applicationcostprofiler-2.5.4/types_aiobotocore_applicationcostprofiler/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      995 2023-08-08 01:06:13.000000 types-aiobotocore-applicationcostprofiler-2.5.4/types_aiobotocore_applicationcostprofiler/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9517 2023-08-08 01:06:13.000000 types-aiobotocore-applicationcostprofiler-2.5.4/types_aiobotocore_applicationcostprofiler/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9501 2023-08-08 01:06:13.000000 types-aiobotocore-applicationcostprofiler-2.5.4/types_aiobotocore_applicationcostprofiler/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8128 2023-08-08 01:06:13.000000 types-aiobotocore-applicationcostprofiler-2.5.4/types_aiobotocore_applicationcostprofiler/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8126 2023-08-08 01:06:13.000000 types-aiobotocore-applicationcostprofiler-2.5.4/types_aiobotocore_applicationcostprofiler/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2269 2023-08-08 01:06:13.000000 types-aiobotocore-applicationcostprofiler-2.5.4/types_aiobotocore_applicationcostprofiler/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2266 2023-08-08 01:06:13.000000 types-aiobotocore-applicationcostprofiler-2.5.4/types_aiobotocore_applicationcostprofiler/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 01:06:13.000000 types-aiobotocore-applicationcostprofiler-2.5.4/types_aiobotocore_applicationcostprofiler/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     5661 2023-08-08 01:06:13.000000 types-aiobotocore-applicationcostprofiler-2.5.4/types_aiobotocore_applicationcostprofiler/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5658 2023-08-08 01:06:13.000000 types-aiobotocore-applicationcostprofiler-2.5.4/types_aiobotocore_applicationcostprofiler/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-08-08 01:06:13.000000 types-aiobotocore-applicationcostprofiler-2.5.4/types_aiobotocore_applicationcostprofiler/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:23:19.202515 types-aiobotocore-applicationcostprofiler-2.5.4/types_aiobotocore_applicationcostprofiler.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    13918 2023-08-08 01:23:19.000000 types-aiobotocore-applicationcostprofiler-2.5.4/types_aiobotocore_applicationcostprofiler.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1117 2023-08-08 01:23:19.000000 types-aiobotocore-applicationcostprofiler-2.5.4/types_aiobotocore_applicationcostprofiler.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 01:23:19.000000 types-aiobotocore-applicationcostprofiler-2.5.4/types_aiobotocore_applicationcostprofiler.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 01:23:19.000000 types-aiobotocore-applicationcostprofiler-2.5.4/types_aiobotocore_applicationcostprofiler.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-08 01:23:19.000000 types-aiobotocore-applicationcostprofiler-2.5.4/types_aiobotocore_applicationcostprofiler.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-08-08 01:23:19.000000 types-aiobotocore-applicationcostprofiler-2.5.4/types_aiobotocore_applicationcostprofiler.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-applicationcostprofiler-2.5.2.post3/LICENSE` & `types-aiobotocore-applicationcostprofiler-2.5.4/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-applicationcostprofiler-2.5.2.post3/PKG-INFO` & `types-aiobotocore-applicationcostprofiler-2.5.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-applicationcostprofiler
-Version: 2.5.2.post3
-Summary: Type annotations for aiobotocore.ApplicationCostProfiler 2.5.2 service generated with mypy-boto3-builder 7.17.2
+Version: 2.5.4
+Summary: Type annotations for aiobotocore.ApplicationCostProfiler 2.5.4 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_applicationcostprofiler/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-applicationcostprofiler.svg?color=blue)](https://pypi.org/project/types-aiobotocore-applicationcostprofiler)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_applicationcostprofiler/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-applicationcostprofiler)](https://pepy.tech/project/types-aiobotocore-applicationcostprofiler)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.ApplicationCostProfiler 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/applicationcostprofiler.html#ApplicationCostProfiler)
+[aiobotocore.ApplicationCostProfiler 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/applicationcostprofiler.html#ApplicationCostProfiler)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-applicationcostprofiler-2.5.2.post3/README.md` & `types-aiobotocore-applicationcostprofiler-2.5.4/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-applicationcostprofiler.svg?color=blue)](https://pypi.org/project/types-aiobotocore-applicationcostprofiler)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_applicationcostprofiler/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-applicationcostprofiler)](https://pepy.tech/project/types-aiobotocore-applicationcostprofiler)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.ApplicationCostProfiler 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/applicationcostprofiler.html#ApplicationCostProfiler)
+[aiobotocore.ApplicationCostProfiler 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/applicationcostprofiler.html#ApplicationCostProfiler)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-applicationcostprofiler-2.5.2.post3/setup.py` & `types-aiobotocore-applicationcostprofiler-2.5.4/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-applicationcostprofiler",
-    version="2.5.2.post3",
+    version="2.5.4",
     packages=["types_aiobotocore_applicationcostprofiler"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.ApplicationCostProfiler 2.5.2 service generated with"
+        "Type annotations for aiobotocore.ApplicationCostProfiler 2.5.4 service generated with"
         " mypy-boto3-builder 7.17.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
```

### Comparing `types-aiobotocore-applicationcostprofiler-2.5.2.post3/types_aiobotocore_applicationcostprofiler/__init__.py` & `types-aiobotocore-applicationcostprofiler-2.5.4/types_aiobotocore_applicationcostprofiler/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-applicationcostprofiler-2.5.2.post3/types_aiobotocore_applicationcostprofiler/__init__.pyi` & `types-aiobotocore-applicationcostprofiler-2.5.4/types_aiobotocore_applicationcostprofiler/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-applicationcostprofiler-2.5.2.post3/types_aiobotocore_applicationcostprofiler/__main__.py` & `types-aiobotocore-applicationcostprofiler-2.5.4/types_aiobotocore_applicationcostprofiler/__main__.py`

 * *Files 19% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.ApplicationCostProfiler 2.5.2\nVersion:        "
-        " 2.5.2.post3\nBuilder version: 7.17.2\nDocs:           "
+        "Type annotations for aiobotocore.ApplicationCostProfiler 2.5.4\nVersion:        "
+        " 2.5.4\nBuilder version: 7.17.2\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_applicationcostprofiler//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/applicationcostprofiler.html#ApplicationCostProfiler\nOther"
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

### Comparing `types-aiobotocore-applicationcostprofiler-2.5.2.post3/types_aiobotocore_applicationcostprofiler/client.py` & `types-aiobotocore-applicationcostprofiler-2.5.4/types_aiobotocore_applicationcostprofiler/client.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-applicationcostprofiler-2.5.2.post3/types_aiobotocore_applicationcostprofiler/client.pyi` & `types-aiobotocore-applicationcostprofiler-2.5.4/types_aiobotocore_applicationcostprofiler/client.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-applicationcostprofiler-2.5.2.post3/types_aiobotocore_applicationcostprofiler/literals.py` & `types-aiobotocore-applicationcostprofiler-2.5.4/types_aiobotocore_applicationcostprofiler/literals.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -14,27 +14,25 @@
 import sys
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = (
     "FormatType",
     "ListReportDefinitionsPaginatorName",
     "ReportFrequencyType",
     "S3BucketRegionType",
     "ApplicationCostProfilerServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
 )
 
-
 FormatType = Literal["CSV", "PARQUET"]
 ListReportDefinitionsPaginatorName = Literal["list_report_definitions"]
 ReportFrequencyType = Literal["ALL", "DAILY", "MONTHLY"]
 S3BucketRegionType = Literal["af-south-1", "ap-east-1", "eu-south-1", "me-south-1"]
 ApplicationCostProfilerServiceName = Literal["applicationcostprofiler"]
 ServiceName = Literal[
     "accessanalyzer",
@@ -47,14 +45,15 @@
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
@@ -150,14 +149,15 @@
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
@@ -236,26 +236,28 @@
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

### Comparing `types-aiobotocore-applicationcostprofiler-2.5.2.post3/types_aiobotocore_applicationcostprofiler/literals.pyi` & `types-aiobotocore-applicationcostprofiler-2.5.4/types_aiobotocore_applicationcostprofiler/literals.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,25 +14,27 @@
 import sys
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
+
 __all__ = (
     "FormatType",
     "ListReportDefinitionsPaginatorName",
     "ReportFrequencyType",
     "S3BucketRegionType",
     "ApplicationCostProfilerServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
 )
 
+
 FormatType = Literal["CSV", "PARQUET"]
 ListReportDefinitionsPaginatorName = Literal["list_report_definitions"]
 ReportFrequencyType = Literal["ALL", "DAILY", "MONTHLY"]
 S3BucketRegionType = Literal["af-south-1", "ap-east-1", "eu-south-1", "me-south-1"]
 ApplicationCostProfilerServiceName = Literal["applicationcostprofiler"]
 ServiceName = Literal[
     "accessanalyzer",
@@ -45,14 +47,15 @@
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
@@ -148,14 +151,15 @@
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
@@ -234,26 +238,28 @@
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

### Comparing `types-aiobotocore-applicationcostprofiler-2.5.2.post3/types_aiobotocore_applicationcostprofiler/paginator.py` & `types-aiobotocore-applicationcostprofiler-2.5.4/types_aiobotocore_applicationcostprofiler/paginator.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-applicationcostprofiler-2.5.2.post3/types_aiobotocore_applicationcostprofiler/paginator.pyi` & `types-aiobotocore-applicationcostprofiler-2.5.4/types_aiobotocore_applicationcostprofiler/paginator.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-applicationcostprofiler-2.5.2.post3/types_aiobotocore_applicationcostprofiler/type_defs.py` & `types-aiobotocore-applicationcostprofiler-2.5.4/types_aiobotocore_applicationcostprofiler/type_defs.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-applicationcostprofiler-2.5.2.post3/types_aiobotocore_applicationcostprofiler/type_defs.pyi` & `types-aiobotocore-applicationcostprofiler-2.5.4/types_aiobotocore_applicationcostprofiler/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-applicationcostprofiler-2.5.2.post3/types_aiobotocore_applicationcostprofiler.egg-info/PKG-INFO` & `types-aiobotocore-applicationcostprofiler-2.5.4/types_aiobotocore_applicationcostprofiler.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-applicationcostprofiler
-Version: 2.5.2.post3
-Summary: Type annotations for aiobotocore.ApplicationCostProfiler 2.5.2 service generated with mypy-boto3-builder 7.17.2
+Version: 2.5.4
+Summary: Type annotations for aiobotocore.ApplicationCostProfiler 2.5.4 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_applicationcostprofiler/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-applicationcostprofiler.svg?color=blue)](https://pypi.org/project/types-aiobotocore-applicationcostprofiler)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_applicationcostprofiler/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-applicationcostprofiler)](https://pepy.tech/project/types-aiobotocore-applicationcostprofiler)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.ApplicationCostProfiler 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/applicationcostprofiler.html#ApplicationCostProfiler)
+[aiobotocore.ApplicationCostProfiler 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/applicationcostprofiler.html#ApplicationCostProfiler)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-applicationcostprofiler-2.5.2.post3/types_aiobotocore_applicationcostprofiler.egg-info/SOURCES.txt` & `types-aiobotocore-applicationcostprofiler-2.5.4/types_aiobotocore_applicationcostprofiler.egg-info/SOURCES.txt`

 * *Files identical despite different names*


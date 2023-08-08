# Comparing `tmp/types-aiobotocore-cur-2.5.2.post3.tar.gz` & `tmp/types-aiobotocore-cur-2.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-cur-2.5.2.post3.tar", last modified: Fri Aug  4 12:37:33 2023, max compression
+gzip compressed data, was "types-aiobotocore-cur-2.5.4.tar", last modified: Tue Aug  8 01:23:33 2023, max compression
```

## Comparing `types-aiobotocore-cur-2.5.2.post3.tar` & `types-aiobotocore-cur-2.5.4.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:37:33.939581 types-aiobotocore-cur-2.5.2.post3/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-04 12:21:03.000000 types-aiobotocore-cur-2.5.2.post3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    12999 2023-08-04 12:37:33.931581 types-aiobotocore-cur-2.5.2.post3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    11475 2023-08-04 12:21:03.000000 types-aiobotocore-cur-2.5.2.post3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-04 12:37:33.939581 types-aiobotocore-cur-2.5.2.post3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2042 2023-08-04 12:21:03.000000 types-aiobotocore-cur-2.5.2.post3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:37:33.931581 types-aiobotocore-cur-2.5.2.post3/types_aiobotocore_cur/
--rw-r--r--   0 runner    (1001) docker     (123)      793 2023-08-04 12:21:03.000000 types-aiobotocore-cur-2.5.2.post3/types_aiobotocore_cur/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      792 2023-08-04 12:21:03.000000 types-aiobotocore-cur-2.5.2.post3/types_aiobotocore_cur/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      960 2023-08-04 12:21:03.000000 types-aiobotocore-cur-2.5.2.post3/types_aiobotocore_cur/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7165 2023-08-04 12:21:03.000000 types-aiobotocore-cur-2.5.2.post3/types_aiobotocore_cur/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     7151 2023-08-04 12:21:03.000000 types-aiobotocore-cur-2.5.2.post3/types_aiobotocore_cur/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8896 2023-08-04 12:21:03.000000 types-aiobotocore-cur-2.5.2.post3/types_aiobotocore_cur/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     8894 2023-08-04 12:21:03.000000 types-aiobotocore-cur-2.5.2.post3/types_aiobotocore_cur/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2149 2023-08-04 12:21:03.000000 types-aiobotocore-cur-2.5.2.post3/types_aiobotocore_cur/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     2146 2023-08-04 12:21:03.000000 types-aiobotocore-cur-2.5.2.post3/types_aiobotocore_cur/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 12:21:03.000000 types-aiobotocore-cur-2.5.2.post3/types_aiobotocore_cur/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     3840 2023-08-04 12:21:03.000000 types-aiobotocore-cur-2.5.2.post3/types_aiobotocore_cur/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)     3837 2023-08-04 12:21:03.000000 types-aiobotocore-cur-2.5.2.post3/types_aiobotocore_cur/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-04 12:21:03.000000 types-aiobotocore-cur-2.5.2.post3/types_aiobotocore_cur/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:37:33.931581 types-aiobotocore-cur-2.5.2.post3/types_aiobotocore_cur.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    12999 2023-08-04 12:37:33.000000 types-aiobotocore-cur-2.5.2.post3/types_aiobotocore_cur.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      737 2023-08-04 12:37:33.000000 types-aiobotocore-cur-2.5.2.post3/types_aiobotocore_cur.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 12:37:33.000000 types-aiobotocore-cur-2.5.2.post3/types_aiobotocore_cur.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 12:37:33.000000 types-aiobotocore-cur-2.5.2.post3/types_aiobotocore_cur.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-04 12:37:33.000000 types-aiobotocore-cur-2.5.2.post3/types_aiobotocore_cur.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-08-04 12:37:33.000000 types-aiobotocore-cur-2.5.2.post3/types_aiobotocore_cur.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:23:33.734676 types-aiobotocore-cur-2.5.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-08 01:08:39.000000 types-aiobotocore-cur-2.5.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    12993 2023-08-08 01:23:33.734676 types-aiobotocore-cur-2.5.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    11475 2023-08-08 01:08:39.000000 types-aiobotocore-cur-2.5.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-08 01:23:33.734676 types-aiobotocore-cur-2.5.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2036 2023-08-08 01:08:39.000000 types-aiobotocore-cur-2.5.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:23:33.734676 types-aiobotocore-cur-2.5.4/types_aiobotocore_cur/
+-rw-r--r--   0 runner    (1001) docker     (123)      793 2023-08-08 01:08:39.000000 types-aiobotocore-cur-2.5.4/types_aiobotocore_cur/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      792 2023-08-08 01:08:39.000000 types-aiobotocore-cur-2.5.4/types_aiobotocore_cur/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      948 2023-08-08 01:08:39.000000 types-aiobotocore-cur-2.5.4/types_aiobotocore_cur/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7165 2023-08-08 01:08:39.000000 types-aiobotocore-cur-2.5.4/types_aiobotocore_cur/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7151 2023-08-08 01:08:39.000000 types-aiobotocore-cur-2.5.4/types_aiobotocore_cur/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8991 2023-08-08 01:08:39.000000 types-aiobotocore-cur-2.5.4/types_aiobotocore_cur/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8989 2023-08-08 01:08:39.000000 types-aiobotocore-cur-2.5.4/types_aiobotocore_cur/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2149 2023-08-08 01:08:39.000000 types-aiobotocore-cur-2.5.4/types_aiobotocore_cur/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2146 2023-08-08 01:08:39.000000 types-aiobotocore-cur-2.5.4/types_aiobotocore_cur/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 01:08:39.000000 types-aiobotocore-cur-2.5.4/types_aiobotocore_cur/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     3840 2023-08-08 01:08:39.000000 types-aiobotocore-cur-2.5.4/types_aiobotocore_cur/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3837 2023-08-08 01:08:39.000000 types-aiobotocore-cur-2.5.4/types_aiobotocore_cur/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-08-08 01:08:39.000000 types-aiobotocore-cur-2.5.4/types_aiobotocore_cur/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:23:33.734676 types-aiobotocore-cur-2.5.4/types_aiobotocore_cur.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    12993 2023-08-08 01:23:33.000000 types-aiobotocore-cur-2.5.4/types_aiobotocore_cur.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      737 2023-08-08 01:23:33.000000 types-aiobotocore-cur-2.5.4/types_aiobotocore_cur.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 01:23:33.000000 types-aiobotocore-cur-2.5.4/types_aiobotocore_cur.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 01:23:33.000000 types-aiobotocore-cur-2.5.4/types_aiobotocore_cur.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-08 01:23:33.000000 types-aiobotocore-cur-2.5.4/types_aiobotocore_cur.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-08-08 01:23:33.000000 types-aiobotocore-cur-2.5.4/types_aiobotocore_cur.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-cur-2.5.2.post3/LICENSE` & `types-aiobotocore-cur-2.5.4/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-cur-2.5.2.post3/PKG-INFO` & `types-aiobotocore-cur-2.5.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-cur
-Version: 2.5.2.post3
-Summary: Type annotations for aiobotocore.CostandUsageReportService 2.5.2 service generated with mypy-boto3-builder 7.17.2
+Version: 2.5.4
+Summary: Type annotations for aiobotocore.CostandUsageReportService 2.5.4 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cur/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-cur.svg?color=blue)](https://pypi.org/project/types-aiobotocore-cur)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cur/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-cur)](https://pepy.tech/project/types-aiobotocore-cur)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.CostandUsageReportService 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cur.html#CostandUsageReportService)
+[aiobotocore.CostandUsageReportService 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cur.html#CostandUsageReportService)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-cur-2.5.2.post3/README.md` & `types-aiobotocore-cur-2.5.4/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-cur.svg?color=blue)](https://pypi.org/project/types-aiobotocore-cur)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cur/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-cur)](https://pepy.tech/project/types-aiobotocore-cur)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.CostandUsageReportService 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cur.html#CostandUsageReportService)
+[aiobotocore.CostandUsageReportService 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cur.html#CostandUsageReportService)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-cur-2.5.2.post3/setup.py` & `types-aiobotocore-cur-2.5.4/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-cur",
-    version="2.5.2.post3",
+    version="2.5.4",
     packages=["types_aiobotocore_cur"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.CostandUsageReportService 2.5.2 service generated with"
+        "Type annotations for aiobotocore.CostandUsageReportService 2.5.4 service generated with"
         " mypy-boto3-builder 7.17.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
```

### Comparing `types-aiobotocore-cur-2.5.2.post3/types_aiobotocore_cur/__init__.py` & `types-aiobotocore-cur-2.5.4/types_aiobotocore_cur/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-cur-2.5.2.post3/types_aiobotocore_cur/__init__.pyi` & `types-aiobotocore-cur-2.5.4/types_aiobotocore_cur/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-cur-2.5.2.post3/types_aiobotocore_cur/__main__.py` & `types-aiobotocore-cur-2.5.4/types_aiobotocore_cur/__main__.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.CostandUsageReportService 2.5.2\nVersion:        "
-        " 2.5.2.post3\nBuilder version: 7.17.2\nDocs:           "
+        "Type annotations for aiobotocore.CostandUsageReportService 2.5.4\nVersion:        "
+        " 2.5.4\nBuilder version: 7.17.2\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cur//\nBoto3 docs:    "
         "  https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cur.html#CostandUsageReportService\nOther"
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

### Comparing `types-aiobotocore-cur-2.5.2.post3/types_aiobotocore_cur/client.py` & `types-aiobotocore-cur-2.5.4/types_aiobotocore_cur/client.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-cur-2.5.2.post3/types_aiobotocore_cur/client.pyi` & `types-aiobotocore-cur-2.5.4/types_aiobotocore_cur/client.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-cur-2.5.2.post3/types_aiobotocore_cur/literals.py` & `types-aiobotocore-cur-2.5.4/types_aiobotocore_cur/literals.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,14 @@
 import sys
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = (
     "AWSRegionType",
     "AdditionalArtifactType",
     "CompressionFormatType",
     "DescribeReportDefinitionsPaginatorName",
     "ReportFormatType",
     "ReportVersioningType",
@@ -31,15 +30,14 @@
     "CostandUsageReportServiceServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "RegionName",
 )
 
-
 AWSRegionType = Literal[
     "af-south-1",
     "ap-east-1",
     "ap-northeast-1",
     "ap-northeast-2",
     "ap-northeast-3",
     "ap-south-1",
@@ -85,14 +83,15 @@
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
@@ -188,14 +187,15 @@
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
@@ -274,26 +274,28 @@
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

### Comparing `types-aiobotocore-cur-2.5.2.post3/types_aiobotocore_cur/literals.pyi` & `types-aiobotocore-cur-2.5.4/types_aiobotocore_cur/literals.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 import sys
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
+
 __all__ = (
     "AWSRegionType",
     "AdditionalArtifactType",
     "CompressionFormatType",
     "DescribeReportDefinitionsPaginatorName",
     "ReportFormatType",
     "ReportVersioningType",
@@ -30,14 +31,15 @@
     "CostandUsageReportServiceServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "RegionName",
 )
 
+
 AWSRegionType = Literal[
     "af-south-1",
     "ap-east-1",
     "ap-northeast-1",
     "ap-northeast-2",
     "ap-northeast-3",
     "ap-south-1",
@@ -83,14 +85,15 @@
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
@@ -186,14 +189,15 @@
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
@@ -272,26 +276,28 @@
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

### Comparing `types-aiobotocore-cur-2.5.2.post3/types_aiobotocore_cur/paginator.py` & `types-aiobotocore-cur-2.5.4/types_aiobotocore_cur/paginator.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-cur-2.5.2.post3/types_aiobotocore_cur/paginator.pyi` & `types-aiobotocore-cur-2.5.4/types_aiobotocore_cur/paginator.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-cur-2.5.2.post3/types_aiobotocore_cur/type_defs.py` & `types-aiobotocore-cur-2.5.4/types_aiobotocore_cur/type_defs.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-cur-2.5.2.post3/types_aiobotocore_cur/type_defs.pyi` & `types-aiobotocore-cur-2.5.4/types_aiobotocore_cur/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-cur-2.5.2.post3/types_aiobotocore_cur.egg-info/PKG-INFO` & `types-aiobotocore-cur-2.5.4/types_aiobotocore_cur.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-cur
-Version: 2.5.2.post3
-Summary: Type annotations for aiobotocore.CostandUsageReportService 2.5.2 service generated with mypy-boto3-builder 7.17.2
+Version: 2.5.4
+Summary: Type annotations for aiobotocore.CostandUsageReportService 2.5.4 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cur/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-cur.svg?color=blue)](https://pypi.org/project/types-aiobotocore-cur)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cur/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-cur)](https://pepy.tech/project/types-aiobotocore-cur)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.CostandUsageReportService 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cur.html#CostandUsageReportService)
+[aiobotocore.CostandUsageReportService 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cur.html#CostandUsageReportService)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-cur-2.5.2.post3/types_aiobotocore_cur.egg-info/SOURCES.txt` & `types-aiobotocore-cur-2.5.4/types_aiobotocore_cur.egg-info/SOURCES.txt`

 * *Files identical despite different names*


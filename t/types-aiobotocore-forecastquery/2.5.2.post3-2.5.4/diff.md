# Comparing `tmp/types-aiobotocore-forecastquery-2.5.2.post3.tar.gz` & `tmp/types-aiobotocore-forecastquery-2.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-forecastquery-2.5.2.post3.tar", last modified: Fri Aug  4 12:37:44 2023, max compression
+gzip compressed data, was "types-aiobotocore-forecastquery-2.5.4.tar", last modified: Tue Aug  8 01:23:45 2023, max compression
```

## Comparing `types-aiobotocore-forecastquery-2.5.2.post3.tar` & `types-aiobotocore-forecastquery-2.5.4.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:37:44.559831 types-aiobotocore-forecastquery-2.5.2.post3/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-04 12:23:58.000000 types-aiobotocore-forecastquery-2.5.2.post3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    12585 2023-08-04 12:37:44.559831 types-aiobotocore-forecastquery-2.5.2.post3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    11036 2023-08-04 12:23:58.000000 types-aiobotocore-forecastquery-2.5.2.post3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-04 12:37:44.559831 types-aiobotocore-forecastquery-2.5.2.post3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2121 2023-08-04 12:23:58.000000 types-aiobotocore-forecastquery-2.5.2.post3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:37:44.559831 types-aiobotocore-forecastquery-2.5.2.post3/types_aiobotocore_forecastquery/
--rw-r--r--   0 runner    (1001) docker     (123)      525 2023-08-04 12:23:58.000000 types-aiobotocore-forecastquery-2.5.2.post3/types_aiobotocore_forecastquery/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      524 2023-08-04 12:23:58.000000 types-aiobotocore-forecastquery-2.5.2.post3/types_aiobotocore_forecastquery/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      981 2023-08-04 12:23:58.000000 types-aiobotocore-forecastquery-2.5.2.post3/types_aiobotocore_forecastquery/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5751 2023-08-04 12:23:58.000000 types-aiobotocore-forecastquery-2.5.2.post3/types_aiobotocore_forecastquery/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     5741 2023-08-04 12:23:58.000000 types-aiobotocore-forecastquery-2.5.2.post3/types_aiobotocore_forecastquery/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     7819 2023-08-04 12:23:58.000000 types-aiobotocore-forecastquery-2.5.2.post3/types_aiobotocore_forecastquery/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     7817 2023-08-04 12:23:58.000000 types-aiobotocore-forecastquery-2.5.2.post3/types_aiobotocore_forecastquery/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 12:23:58.000000 types-aiobotocore-forecastquery-2.5.2.post3/types_aiobotocore_forecastquery/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     2810 2023-08-04 12:23:58.000000 types-aiobotocore-forecastquery-2.5.2.post3/types_aiobotocore_forecastquery/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)     2805 2023-08-04 12:23:58.000000 types-aiobotocore-forecastquery-2.5.2.post3/types_aiobotocore_forecastquery/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-04 12:23:58.000000 types-aiobotocore-forecastquery-2.5.2.post3/types_aiobotocore_forecastquery/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:37:44.559831 types-aiobotocore-forecastquery-2.5.2.post3/types_aiobotocore_forecastquery.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    12585 2023-08-04 12:37:44.000000 types-aiobotocore-forecastquery-2.5.2.post3/types_aiobotocore_forecastquery.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      836 2023-08-04 12:37:44.000000 types-aiobotocore-forecastquery-2.5.2.post3/types_aiobotocore_forecastquery.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 12:37:44.000000 types-aiobotocore-forecastquery-2.5.2.post3/types_aiobotocore_forecastquery.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 12:37:44.000000 types-aiobotocore-forecastquery-2.5.2.post3/types_aiobotocore_forecastquery.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-04 12:37:44.000000 types-aiobotocore-forecastquery-2.5.2.post3/types_aiobotocore_forecastquery.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-08-04 12:37:44.000000 types-aiobotocore-forecastquery-2.5.2.post3/types_aiobotocore_forecastquery.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:23:45.546720 types-aiobotocore-forecastquery-2.5.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-08 01:11:22.000000 types-aiobotocore-forecastquery-2.5.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    12579 2023-08-08 01:23:45.542720 types-aiobotocore-forecastquery-2.5.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    11036 2023-08-08 01:11:22.000000 types-aiobotocore-forecastquery-2.5.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-08 01:23:45.546720 types-aiobotocore-forecastquery-2.5.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2115 2023-08-08 01:11:22.000000 types-aiobotocore-forecastquery-2.5.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:23:45.542720 types-aiobotocore-forecastquery-2.5.4/types_aiobotocore_forecastquery/
+-rw-r--r--   0 runner    (1001) docker     (123)      525 2023-08-08 01:11:22.000000 types-aiobotocore-forecastquery-2.5.4/types_aiobotocore_forecastquery/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      524 2023-08-08 01:11:22.000000 types-aiobotocore-forecastquery-2.5.4/types_aiobotocore_forecastquery/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      969 2023-08-08 01:11:22.000000 types-aiobotocore-forecastquery-2.5.4/types_aiobotocore_forecastquery/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5751 2023-08-08 01:11:22.000000 types-aiobotocore-forecastquery-2.5.4/types_aiobotocore_forecastquery/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5741 2023-08-08 01:11:22.000000 types-aiobotocore-forecastquery-2.5.4/types_aiobotocore_forecastquery/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     7914 2023-08-08 01:11:22.000000 types-aiobotocore-forecastquery-2.5.4/types_aiobotocore_forecastquery/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7912 2023-08-08 01:11:22.000000 types-aiobotocore-forecastquery-2.5.4/types_aiobotocore_forecastquery/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 01:11:22.000000 types-aiobotocore-forecastquery-2.5.4/types_aiobotocore_forecastquery/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     2810 2023-08-08 01:11:22.000000 types-aiobotocore-forecastquery-2.5.4/types_aiobotocore_forecastquery/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2805 2023-08-08 01:11:22.000000 types-aiobotocore-forecastquery-2.5.4/types_aiobotocore_forecastquery/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-08-08 01:11:22.000000 types-aiobotocore-forecastquery-2.5.4/types_aiobotocore_forecastquery/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:23:45.542720 types-aiobotocore-forecastquery-2.5.4/types_aiobotocore_forecastquery.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    12579 2023-08-08 01:23:45.000000 types-aiobotocore-forecastquery-2.5.4/types_aiobotocore_forecastquery.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      836 2023-08-08 01:23:45.000000 types-aiobotocore-forecastquery-2.5.4/types_aiobotocore_forecastquery.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 01:23:45.000000 types-aiobotocore-forecastquery-2.5.4/types_aiobotocore_forecastquery.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 01:23:45.000000 types-aiobotocore-forecastquery-2.5.4/types_aiobotocore_forecastquery.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-08 01:23:45.000000 types-aiobotocore-forecastquery-2.5.4/types_aiobotocore_forecastquery.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-08-08 01:23:45.000000 types-aiobotocore-forecastquery-2.5.4/types_aiobotocore_forecastquery.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-forecastquery-2.5.2.post3/LICENSE` & `types-aiobotocore-forecastquery-2.5.4/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-forecastquery-2.5.2.post3/PKG-INFO` & `types-aiobotocore-forecastquery-2.5.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-forecastquery
-Version: 2.5.2.post3
-Summary: Type annotations for aiobotocore.ForecastQueryService 2.5.2 service generated with mypy-boto3-builder 7.17.2
+Version: 2.5.4
+Summary: Type annotations for aiobotocore.ForecastQueryService 2.5.4 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_forecastquery/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-forecastquery.svg?color=blue)](https://pypi.org/project/types-aiobotocore-forecastquery)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_forecastquery/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-forecastquery)](https://pepy.tech/project/types-aiobotocore-forecastquery)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.ForecastQueryService 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/forecastquery.html#ForecastQueryService)
+[aiobotocore.ForecastQueryService 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/forecastquery.html#ForecastQueryService)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-forecastquery-2.5.2.post3/README.md` & `types-aiobotocore-forecastquery-2.5.4/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-forecastquery.svg?color=blue)](https://pypi.org/project/types-aiobotocore-forecastquery)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_forecastquery/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-forecastquery)](https://pepy.tech/project/types-aiobotocore-forecastquery)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.ForecastQueryService 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/forecastquery.html#ForecastQueryService)
+[aiobotocore.ForecastQueryService 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/forecastquery.html#ForecastQueryService)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-forecastquery-2.5.2.post3/setup.py` & `types-aiobotocore-forecastquery-2.5.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-forecastquery",
-    version="2.5.2.post3",
+    version="2.5.4",
     packages=["types_aiobotocore_forecastquery"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.ForecastQueryService 2.5.2 service generated with"
+        "Type annotations for aiobotocore.ForecastQueryService 2.5.4 service generated with"
         " mypy-boto3-builder 7.17.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
```

### Comparing `types-aiobotocore-forecastquery-2.5.2.post3/types_aiobotocore_forecastquery/__init__.py` & `types-aiobotocore-forecastquery-2.5.4/types_aiobotocore_forecastquery/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-forecastquery-2.5.2.post3/types_aiobotocore_forecastquery/__init__.pyi` & `types-aiobotocore-forecastquery-2.5.4/types_aiobotocore_forecastquery/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-forecastquery-2.5.2.post3/types_aiobotocore_forecastquery/__main__.py` & `types-aiobotocore-forecastquery-2.5.4/types_aiobotocore_forecastquery/__main__.py`

 * *Files 20% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.ForecastQueryService 2.5.2\nVersion:        "
-        " 2.5.2.post3\nBuilder version: 7.17.2\nDocs:           "
+        "Type annotations for aiobotocore.ForecastQueryService 2.5.4\nVersion:        "
+        " 2.5.4\nBuilder version: 7.17.2\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_forecastquery//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/forecastquery.html#ForecastQueryService\nOther"
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

### Comparing `types-aiobotocore-forecastquery-2.5.2.post3/types_aiobotocore_forecastquery/client.py` & `types-aiobotocore-forecastquery-2.5.4/types_aiobotocore_forecastquery/client.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-forecastquery-2.5.2.post3/types_aiobotocore_forecastquery/client.pyi` & `types-aiobotocore-forecastquery-2.5.4/types_aiobotocore_forecastquery/client.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-forecastquery-2.5.2.post3/types_aiobotocore_forecastquery/literals.py` & `types-aiobotocore-forecastquery-2.5.4/types_aiobotocore_forecastquery/literals.py`

 * *Files 0% similar despite different names*

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
```

### Comparing `types-aiobotocore-forecastquery-2.5.2.post3/types_aiobotocore_forecastquery/literals.pyi` & `types-aiobotocore-forecastquery-2.5.4/types_aiobotocore_forecastquery/literals.pyi`

 * *Files 0% similar despite different names*

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
```

### Comparing `types-aiobotocore-forecastquery-2.5.2.post3/types_aiobotocore_forecastquery/type_defs.py` & `types-aiobotocore-forecastquery-2.5.4/types_aiobotocore_forecastquery/type_defs.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-forecastquery-2.5.2.post3/types_aiobotocore_forecastquery/type_defs.pyi` & `types-aiobotocore-forecastquery-2.5.4/types_aiobotocore_forecastquery/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-forecastquery-2.5.2.post3/types_aiobotocore_forecastquery.egg-info/PKG-INFO` & `types-aiobotocore-forecastquery-2.5.4/types_aiobotocore_forecastquery.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-forecastquery
-Version: 2.5.2.post3
-Summary: Type annotations for aiobotocore.ForecastQueryService 2.5.2 service generated with mypy-boto3-builder 7.17.2
+Version: 2.5.4
+Summary: Type annotations for aiobotocore.ForecastQueryService 2.5.4 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_forecastquery/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-forecastquery.svg?color=blue)](https://pypi.org/project/types-aiobotocore-forecastquery)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_forecastquery/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-forecastquery)](https://pepy.tech/project/types-aiobotocore-forecastquery)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.ForecastQueryService 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/forecastquery.html#ForecastQueryService)
+[aiobotocore.ForecastQueryService 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/forecastquery.html#ForecastQueryService)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-forecastquery-2.5.2.post3/types_aiobotocore_forecastquery.egg-info/SOURCES.txt` & `types-aiobotocore-forecastquery-2.5.4/types_aiobotocore_forecastquery.egg-info/SOURCES.txt`

 * *Files identical despite different names*


# Comparing `tmp/types-aiobotocore-es-2.5.2.post3.tar.gz` & `tmp/types-aiobotocore-es-2.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-es-2.5.2.post3.tar", last modified: Fri Aug  4 12:37:42 2023, max compression
+gzip compressed data, was "types-aiobotocore-es-2.5.4.tar", last modified: Tue Aug  8 01:23:43 2023, max compression
```

## Comparing `types-aiobotocore-es-2.5.2.post3.tar` & `types-aiobotocore-es-2.5.4.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:37:42.219776 types-aiobotocore-es-2.5.2.post3/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-04 12:23:33.000000 types-aiobotocore-es-2.5.2.post3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    13852 2023-08-04 12:37:42.219776 types-aiobotocore-es-2.5.2.post3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    12336 2023-08-04 12:23:33.000000 types-aiobotocore-es-2.5.2.post3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-04 12:37:42.219776 types-aiobotocore-es-2.5.2.post3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2031 2023-08-04 12:23:33.000000 types-aiobotocore-es-2.5.2.post3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:37:42.207776 types-aiobotocore-es-2.5.2.post3/types_aiobotocore_es/
--rw-r--r--   0 runner    (1001) docker     (123)     2015 2023-08-04 12:23:33.000000 types-aiobotocore-es-2.5.2.post3/types_aiobotocore_es/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2014 2023-08-04 12:23:33.000000 types-aiobotocore-es-2.5.2.post3/types_aiobotocore_es/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      948 2023-08-04 12:23:33.000000 types-aiobotocore-es-2.5.2.post3/types_aiobotocore_es/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    43173 2023-08-04 12:23:33.000000 types-aiobotocore-es-2.5.2.post3/types_aiobotocore_es/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    43109 2023-08-04 12:23:33.000000 types-aiobotocore-es-2.5.2.post3/types_aiobotocore_es/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    14517 2023-08-04 12:23:34.000000 types-aiobotocore-es-2.5.2.post3/types_aiobotocore_es/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    14515 2023-08-04 12:23:34.000000 types-aiobotocore-es-2.5.2.post3/types_aiobotocore_es/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     7554 2023-08-04 12:23:33.000000 types-aiobotocore-es-2.5.2.post3/types_aiobotocore_es/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     7547 2023-08-04 12:23:33.000000 types-aiobotocore-es-2.5.2.post3/types_aiobotocore_es/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 12:23:33.000000 types-aiobotocore-es-2.5.2.post3/types_aiobotocore_es/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    63653 2023-08-04 12:23:36.000000 types-aiobotocore-es-2.5.2.post3/types_aiobotocore_es/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    63606 2023-08-04 12:23:34.000000 types-aiobotocore-es-2.5.2.post3/types_aiobotocore_es/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-04 12:23:33.000000 types-aiobotocore-es-2.5.2.post3/types_aiobotocore_es/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:37:42.219776 types-aiobotocore-es-2.5.2.post3/types_aiobotocore_es.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    13852 2023-08-04 12:37:41.000000 types-aiobotocore-es-2.5.2.post3/types_aiobotocore_es.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      718 2023-08-04 12:37:42.000000 types-aiobotocore-es-2.5.2.post3/types_aiobotocore_es.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 12:37:41.000000 types-aiobotocore-es-2.5.2.post3/types_aiobotocore_es.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 12:37:41.000000 types-aiobotocore-es-2.5.2.post3/types_aiobotocore_es.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-04 12:37:41.000000 types-aiobotocore-es-2.5.2.post3/types_aiobotocore_es.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-08-04 12:37:41.000000 types-aiobotocore-es-2.5.2.post3/types_aiobotocore_es.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:23:43.222714 types-aiobotocore-es-2.5.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-08 01:10:59.000000 types-aiobotocore-es-2.5.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    13846 2023-08-08 01:23:43.218714 types-aiobotocore-es-2.5.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    12336 2023-08-08 01:10:59.000000 types-aiobotocore-es-2.5.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-08 01:23:43.222714 types-aiobotocore-es-2.5.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2025 2023-08-08 01:10:59.000000 types-aiobotocore-es-2.5.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:23:43.214714 types-aiobotocore-es-2.5.4/types_aiobotocore_es/
+-rw-r--r--   0 runner    (1001) docker     (123)     2015 2023-08-08 01:10:59.000000 types-aiobotocore-es-2.5.4/types_aiobotocore_es/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2014 2023-08-08 01:10:59.000000 types-aiobotocore-es-2.5.4/types_aiobotocore_es/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      936 2023-08-08 01:10:59.000000 types-aiobotocore-es-2.5.4/types_aiobotocore_es/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    43173 2023-08-08 01:10:59.000000 types-aiobotocore-es-2.5.4/types_aiobotocore_es/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    43109 2023-08-08 01:10:59.000000 types-aiobotocore-es-2.5.4/types_aiobotocore_es/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    14632 2023-08-08 01:11:00.000000 types-aiobotocore-es-2.5.4/types_aiobotocore_es/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14630 2023-08-08 01:10:59.000000 types-aiobotocore-es-2.5.4/types_aiobotocore_es/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     7554 2023-08-08 01:10:59.000000 types-aiobotocore-es-2.5.4/types_aiobotocore_es/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7547 2023-08-08 01:10:59.000000 types-aiobotocore-es-2.5.4/types_aiobotocore_es/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 01:10:59.000000 types-aiobotocore-es-2.5.4/types_aiobotocore_es/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    63653 2023-08-08 01:11:02.000000 types-aiobotocore-es-2.5.4/types_aiobotocore_es/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    63606 2023-08-08 01:11:00.000000 types-aiobotocore-es-2.5.4/types_aiobotocore_es/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-08-08 01:10:59.000000 types-aiobotocore-es-2.5.4/types_aiobotocore_es/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:23:43.218714 types-aiobotocore-es-2.5.4/types_aiobotocore_es.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    13846 2023-08-08 01:23:43.000000 types-aiobotocore-es-2.5.4/types_aiobotocore_es.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      718 2023-08-08 01:23:43.000000 types-aiobotocore-es-2.5.4/types_aiobotocore_es.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 01:23:43.000000 types-aiobotocore-es-2.5.4/types_aiobotocore_es.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 01:23:43.000000 types-aiobotocore-es-2.5.4/types_aiobotocore_es.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-08 01:23:43.000000 types-aiobotocore-es-2.5.4/types_aiobotocore_es.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-08-08 01:23:43.000000 types-aiobotocore-es-2.5.4/types_aiobotocore_es.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-es-2.5.2.post3/LICENSE` & `types-aiobotocore-es-2.5.4/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-es-2.5.2.post3/PKG-INFO` & `types-aiobotocore-es-2.5.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-es
-Version: 2.5.2.post3
-Summary: Type annotations for aiobotocore.ElasticsearchService 2.5.2 service generated with mypy-boto3-builder 7.17.2
+Version: 2.5.4
+Summary: Type annotations for aiobotocore.ElasticsearchService 2.5.4 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_es/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-es.svg?color=blue)](https://pypi.org/project/types-aiobotocore-es)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_es/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-es)](https://pepy.tech/project/types-aiobotocore-es)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.ElasticsearchService 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/es.html#ElasticsearchService)
+[aiobotocore.ElasticsearchService 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/es.html#ElasticsearchService)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-es-2.5.2.post3/README.md` & `types-aiobotocore-es-2.5.4/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-es.svg?color=blue)](https://pypi.org/project/types-aiobotocore-es)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_es/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-es)](https://pepy.tech/project/types-aiobotocore-es)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.ElasticsearchService 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/es.html#ElasticsearchService)
+[aiobotocore.ElasticsearchService 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/es.html#ElasticsearchService)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-es-2.5.2.post3/setup.py` & `types-aiobotocore-es-2.5.4/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-es",
-    version="2.5.2.post3",
+    version="2.5.4",
     packages=["types_aiobotocore_es"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.ElasticsearchService 2.5.2 service generated with"
+        "Type annotations for aiobotocore.ElasticsearchService 2.5.4 service generated with"
         " mypy-boto3-builder 7.17.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
```

### Comparing `types-aiobotocore-es-2.5.2.post3/types_aiobotocore_es/__init__.py` & `types-aiobotocore-es-2.5.4/types_aiobotocore_es/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-es-2.5.2.post3/types_aiobotocore_es/__init__.pyi` & `types-aiobotocore-es-2.5.4/types_aiobotocore_es/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-es-2.5.2.post3/types_aiobotocore_es/__main__.py` & `types-aiobotocore-es-2.5.4/types_aiobotocore_es/__main__.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.ElasticsearchService 2.5.2\nVersion:        "
-        " 2.5.2.post3\nBuilder version: 7.17.2\nDocs:           "
+        "Type annotations for aiobotocore.ElasticsearchService 2.5.4\nVersion:        "
+        " 2.5.4\nBuilder version: 7.17.2\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_es//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/es.html#ElasticsearchService\nOther"
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

### Comparing `types-aiobotocore-es-2.5.2.post3/types_aiobotocore_es/client.py` & `types-aiobotocore-es-2.5.4/types_aiobotocore_es/client.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-es-2.5.2.post3/types_aiobotocore_es/client.pyi` & `types-aiobotocore-es-2.5.4/types_aiobotocore_es/client.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-es-2.5.2.post3/types_aiobotocore_es/literals.py` & `types-aiobotocore-es-2.5.4/types_aiobotocore_es/literals.py`

 * *Files 1% similar despite different names*

```diff
@@ -209,14 +209,15 @@
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
@@ -312,14 +313,15 @@
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
@@ -398,26 +400,28 @@
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
@@ -585,14 +589,15 @@
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

### Comparing `types-aiobotocore-es-2.5.2.post3/types_aiobotocore_es/literals.pyi` & `types-aiobotocore-es-2.5.4/types_aiobotocore_es/literals.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -207,14 +207,15 @@
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
@@ -310,14 +311,15 @@
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
@@ -396,26 +398,28 @@
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
@@ -583,14 +587,15 @@
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

### Comparing `types-aiobotocore-es-2.5.2.post3/types_aiobotocore_es/paginator.py` & `types-aiobotocore-es-2.5.4/types_aiobotocore_es/paginator.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-es-2.5.2.post3/types_aiobotocore_es/paginator.pyi` & `types-aiobotocore-es-2.5.4/types_aiobotocore_es/paginator.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-es-2.5.2.post3/types_aiobotocore_es/type_defs.py` & `types-aiobotocore-es-2.5.4/types_aiobotocore_es/type_defs.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-es-2.5.2.post3/types_aiobotocore_es/type_defs.pyi` & `types-aiobotocore-es-2.5.4/types_aiobotocore_es/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-es-2.5.2.post3/types_aiobotocore_es.egg-info/PKG-INFO` & `types-aiobotocore-es-2.5.4/types_aiobotocore_es.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-es
-Version: 2.5.2.post3
-Summary: Type annotations for aiobotocore.ElasticsearchService 2.5.2 service generated with mypy-boto3-builder 7.17.2
+Version: 2.5.4
+Summary: Type annotations for aiobotocore.ElasticsearchService 2.5.4 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_es/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-es.svg?color=blue)](https://pypi.org/project/types-aiobotocore-es)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_es/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-es)](https://pepy.tech/project/types-aiobotocore-es)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.ElasticsearchService 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/es.html#ElasticsearchService)
+[aiobotocore.ElasticsearchService 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/es.html#ElasticsearchService)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-es-2.5.2.post3/types_aiobotocore_es.egg-info/SOURCES.txt` & `types-aiobotocore-es-2.5.4/types_aiobotocore_es.egg-info/SOURCES.txt`

 * *Files identical despite different names*


# Comparing `tmp/types-aiobotocore-elastic-inference-2.5.2.post3.tar.gz` & `tmp/types-aiobotocore-elastic-inference-2.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-elastic-inference-2.5.2.post3.tar", last modified: Fri Aug  4 12:37:39 2023, max compression
+gzip compressed data, was "types-aiobotocore-elastic-inference-2.5.4.tar", last modified: Tue Aug  8 01:23:40 2023, max compression
```

## Comparing `types-aiobotocore-elastic-inference-2.5.2.post3.tar` & `types-aiobotocore-elastic-inference-2.5.4.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:37:39.707717 types-aiobotocore-elastic-inference-2.5.2.post3/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-04 12:23:09.000000 types-aiobotocore-elastic-inference-2.5.2.post3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    13564 2023-08-04 12:37:39.707717 types-aiobotocore-elastic-inference-2.5.2.post3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    12007 2023-08-04 12:23:09.000000 types-aiobotocore-elastic-inference-2.5.2.post3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-04 12:37:39.707717 types-aiobotocore-elastic-inference-2.5.2.post3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2141 2023-08-04 12:23:09.000000 types-aiobotocore-elastic-inference-2.5.2.post3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:37:39.707717 types-aiobotocore-elastic-inference-2.5.2.post3/types_aiobotocore_elastic_inference/
--rw-r--r--   0 runner    (1001) docker     (123)      758 2023-08-04 12:23:09.000000 types-aiobotocore-elastic-inference-2.5.2.post3/types_aiobotocore_elastic_inference/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      757 2023-08-04 12:23:09.000000 types-aiobotocore-elastic-inference-2.5.2.post3/types_aiobotocore_elastic_inference/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      981 2023-08-04 12:23:09.000000 types-aiobotocore-elastic-inference-2.5.2.post3/types_aiobotocore_elastic_inference/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8763 2023-08-04 12:23:09.000000 types-aiobotocore-elastic-inference-2.5.2.post3/types_aiobotocore_elastic_inference/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     8747 2023-08-04 12:23:09.000000 types-aiobotocore-elastic-inference-2.5.2.post3/types_aiobotocore_elastic_inference/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8041 2023-08-04 12:23:09.000000 types-aiobotocore-elastic-inference-2.5.2.post3/types_aiobotocore_elastic_inference/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     8039 2023-08-04 12:23:09.000000 types-aiobotocore-elastic-inference-2.5.2.post3/types_aiobotocore_elastic_inference/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2311 2023-08-04 12:23:09.000000 types-aiobotocore-elastic-inference-2.5.2.post3/types_aiobotocore_elastic_inference/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     2308 2023-08-04 12:23:09.000000 types-aiobotocore-elastic-inference-2.5.2.post3/types_aiobotocore_elastic_inference/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 12:23:09.000000 types-aiobotocore-elastic-inference-2.5.2.post3/types_aiobotocore_elastic_inference/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     5694 2023-08-04 12:23:09.000000 types-aiobotocore-elastic-inference-2.5.2.post3/types_aiobotocore_elastic_inference/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)     5691 2023-08-04 12:23:09.000000 types-aiobotocore-elastic-inference-2.5.2.post3/types_aiobotocore_elastic_inference/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-04 12:23:09.000000 types-aiobotocore-elastic-inference-2.5.2.post3/types_aiobotocore_elastic_inference/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:37:39.707717 types-aiobotocore-elastic-inference-2.5.2.post3/types_aiobotocore_elastic_inference.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    13564 2023-08-04 12:37:39.000000 types-aiobotocore-elastic-inference-2.5.2.post3/types_aiobotocore_elastic_inference.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1003 2023-08-04 12:37:39.000000 types-aiobotocore-elastic-inference-2.5.2.post3/types_aiobotocore_elastic_inference.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 12:37:39.000000 types-aiobotocore-elastic-inference-2.5.2.post3/types_aiobotocore_elastic_inference.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 12:37:39.000000 types-aiobotocore-elastic-inference-2.5.2.post3/types_aiobotocore_elastic_inference.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-04 12:37:39.000000 types-aiobotocore-elastic-inference-2.5.2.post3/types_aiobotocore_elastic_inference.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-08-04 12:37:39.000000 types-aiobotocore-elastic-inference-2.5.2.post3/types_aiobotocore_elastic_inference.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:23:40.882704 types-aiobotocore-elastic-inference-2.5.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-08 01:10:35.000000 types-aiobotocore-elastic-inference-2.5.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    13558 2023-08-08 01:23:40.882704 types-aiobotocore-elastic-inference-2.5.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    12007 2023-08-08 01:10:35.000000 types-aiobotocore-elastic-inference-2.5.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-08 01:23:40.882704 types-aiobotocore-elastic-inference-2.5.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2135 2023-08-08 01:10:35.000000 types-aiobotocore-elastic-inference-2.5.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:23:40.878704 types-aiobotocore-elastic-inference-2.5.4/types_aiobotocore_elastic_inference/
+-rw-r--r--   0 runner    (1001) docker     (123)      758 2023-08-08 01:10:35.000000 types-aiobotocore-elastic-inference-2.5.4/types_aiobotocore_elastic_inference/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      757 2023-08-08 01:10:35.000000 types-aiobotocore-elastic-inference-2.5.4/types_aiobotocore_elastic_inference/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      969 2023-08-08 01:10:35.000000 types-aiobotocore-elastic-inference-2.5.4/types_aiobotocore_elastic_inference/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8763 2023-08-08 01:10:35.000000 types-aiobotocore-elastic-inference-2.5.4/types_aiobotocore_elastic_inference/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8747 2023-08-08 01:10:35.000000 types-aiobotocore-elastic-inference-2.5.4/types_aiobotocore_elastic_inference/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8136 2023-08-08 01:10:35.000000 types-aiobotocore-elastic-inference-2.5.4/types_aiobotocore_elastic_inference/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8134 2023-08-08 01:10:35.000000 types-aiobotocore-elastic-inference-2.5.4/types_aiobotocore_elastic_inference/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2311 2023-08-08 01:10:35.000000 types-aiobotocore-elastic-inference-2.5.4/types_aiobotocore_elastic_inference/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2308 2023-08-08 01:10:35.000000 types-aiobotocore-elastic-inference-2.5.4/types_aiobotocore_elastic_inference/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 01:10:35.000000 types-aiobotocore-elastic-inference-2.5.4/types_aiobotocore_elastic_inference/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     5694 2023-08-08 01:10:35.000000 types-aiobotocore-elastic-inference-2.5.4/types_aiobotocore_elastic_inference/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5691 2023-08-08 01:10:35.000000 types-aiobotocore-elastic-inference-2.5.4/types_aiobotocore_elastic_inference/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-08-08 01:10:35.000000 types-aiobotocore-elastic-inference-2.5.4/types_aiobotocore_elastic_inference/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:23:40.882704 types-aiobotocore-elastic-inference-2.5.4/types_aiobotocore_elastic_inference.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    13558 2023-08-08 01:23:40.000000 types-aiobotocore-elastic-inference-2.5.4/types_aiobotocore_elastic_inference.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1003 2023-08-08 01:23:40.000000 types-aiobotocore-elastic-inference-2.5.4/types_aiobotocore_elastic_inference.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 01:23:40.000000 types-aiobotocore-elastic-inference-2.5.4/types_aiobotocore_elastic_inference.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 01:23:40.000000 types-aiobotocore-elastic-inference-2.5.4/types_aiobotocore_elastic_inference.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-08 01:23:40.000000 types-aiobotocore-elastic-inference-2.5.4/types_aiobotocore_elastic_inference.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-08-08 01:23:40.000000 types-aiobotocore-elastic-inference-2.5.4/types_aiobotocore_elastic_inference.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-elastic-inference-2.5.2.post3/LICENSE` & `types-aiobotocore-elastic-inference-2.5.4/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-elastic-inference-2.5.2.post3/PKG-INFO` & `types-aiobotocore-elastic-inference-2.5.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-elastic-inference
-Version: 2.5.2.post3
-Summary: Type annotations for aiobotocore.ElasticInference 2.5.2 service generated with mypy-boto3-builder 7.17.2
+Version: 2.5.4
+Summary: Type annotations for aiobotocore.ElasticInference 2.5.4 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elastic_inference/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-elastic-inference.svg?color=blue)](https://pypi.org/project/types-aiobotocore-elastic-inference)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elastic_inference/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-elastic-inference)](https://pepy.tech/project/types-aiobotocore-elastic-inference)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.ElasticInference 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elastic-inference.html#ElasticInference)
+[aiobotocore.ElasticInference 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elastic-inference.html#ElasticInference)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-elastic-inference-2.5.2.post3/README.md` & `types-aiobotocore-elastic-inference-2.5.4/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-elastic-inference.svg?color=blue)](https://pypi.org/project/types-aiobotocore-elastic-inference)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elastic_inference/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-elastic-inference)](https://pepy.tech/project/types-aiobotocore-elastic-inference)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.ElasticInference 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elastic-inference.html#ElasticInference)
+[aiobotocore.ElasticInference 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elastic-inference.html#ElasticInference)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-elastic-inference-2.5.2.post3/setup.py` & `types-aiobotocore-elastic-inference-2.5.4/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-elastic-inference",
-    version="2.5.2.post3",
+    version="2.5.4",
     packages=["types_aiobotocore_elastic_inference"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.ElasticInference 2.5.2 service generated with"
+        "Type annotations for aiobotocore.ElasticInference 2.5.4 service generated with"
         " mypy-boto3-builder 7.17.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
```

### Comparing `types-aiobotocore-elastic-inference-2.5.2.post3/types_aiobotocore_elastic_inference/__init__.py` & `types-aiobotocore-elastic-inference-2.5.4/types_aiobotocore_elastic_inference/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-elastic-inference-2.5.2.post3/types_aiobotocore_elastic_inference/__init__.pyi` & `types-aiobotocore-elastic-inference-2.5.4/types_aiobotocore_elastic_inference/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-elastic-inference-2.5.2.post3/types_aiobotocore_elastic_inference/__main__.py` & `types-aiobotocore-elastic-inference-2.5.4/types_aiobotocore_elastic_inference/__main__.py`

 * *Files 20% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.ElasticInference 2.5.2\nVersion:        "
-        " 2.5.2.post3\nBuilder version: 7.17.2\nDocs:           "
+        "Type annotations for aiobotocore.ElasticInference 2.5.4\nVersion:         2.5.4\nBuilder"
+        " version: 7.17.2\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elastic_inference//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elastic-inference.html#ElasticInference\nOther"
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

### Comparing `types-aiobotocore-elastic-inference-2.5.2.post3/types_aiobotocore_elastic_inference/client.py` & `types-aiobotocore-elastic-inference-2.5.4/types_aiobotocore_elastic_inference/client.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-elastic-inference-2.5.2.post3/types_aiobotocore_elastic_inference/client.pyi` & `types-aiobotocore-elastic-inference-2.5.4/types_aiobotocore_elastic_inference/client.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-elastic-inference-2.5.2.post3/types_aiobotocore_elastic_inference/literals.py` & `types-aiobotocore-elastic-inference-2.5.4/types_aiobotocore_elastic_inference/literals.py`

 * *Files 1% similar despite different names*

```diff
@@ -44,14 +44,15 @@
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
@@ -147,14 +148,15 @@
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
@@ -233,26 +235,28 @@
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

### Comparing `types-aiobotocore-elastic-inference-2.5.2.post3/types_aiobotocore_elastic_inference/literals.pyi` & `types-aiobotocore-elastic-inference-2.5.4/types_aiobotocore_elastic_inference/literals.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -42,14 +42,15 @@
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
@@ -145,14 +146,15 @@
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
@@ -231,26 +233,28 @@
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

### Comparing `types-aiobotocore-elastic-inference-2.5.2.post3/types_aiobotocore_elastic_inference/paginator.py` & `types-aiobotocore-elastic-inference-2.5.4/types_aiobotocore_elastic_inference/paginator.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-elastic-inference-2.5.2.post3/types_aiobotocore_elastic_inference/paginator.pyi` & `types-aiobotocore-elastic-inference-2.5.4/types_aiobotocore_elastic_inference/paginator.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-elastic-inference-2.5.2.post3/types_aiobotocore_elastic_inference/type_defs.py` & `types-aiobotocore-elastic-inference-2.5.4/types_aiobotocore_elastic_inference/type_defs.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-elastic-inference-2.5.2.post3/types_aiobotocore_elastic_inference/type_defs.pyi` & `types-aiobotocore-elastic-inference-2.5.4/types_aiobotocore_elastic_inference/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-elastic-inference-2.5.2.post3/types_aiobotocore_elastic_inference.egg-info/PKG-INFO` & `types-aiobotocore-elastic-inference-2.5.4/types_aiobotocore_elastic_inference.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-elastic-inference
-Version: 2.5.2.post3
-Summary: Type annotations for aiobotocore.ElasticInference 2.5.2 service generated with mypy-boto3-builder 7.17.2
+Version: 2.5.4
+Summary: Type annotations for aiobotocore.ElasticInference 2.5.4 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elastic_inference/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-elastic-inference.svg?color=blue)](https://pypi.org/project/types-aiobotocore-elastic-inference)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elastic_inference/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-elastic-inference)](https://pepy.tech/project/types-aiobotocore-elastic-inference)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.ElasticInference 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elastic-inference.html#ElasticInference)
+[aiobotocore.ElasticInference 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elastic-inference.html#ElasticInference)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-elastic-inference-2.5.2.post3/types_aiobotocore_elastic_inference.egg-info/SOURCES.txt` & `types-aiobotocore-elastic-inference-2.5.4/types_aiobotocore_elastic_inference.egg-info/SOURCES.txt`

 * *Files identical despite different names*


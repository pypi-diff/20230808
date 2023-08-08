# Comparing `tmp/types-aiobotocore-cloudsearch-2.5.2.post3.tar.gz` & `tmp/types-aiobotocore-cloudsearch-2.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-cloudsearch-2.5.2.post3.tar", last modified: Fri Aug  4 12:37:26 2023, max compression
+gzip compressed data, was "types-aiobotocore-cloudsearch-2.5.4.tar", last modified: Tue Aug  8 01:23:26 2023, max compression
```

## Comparing `types-aiobotocore-cloudsearch-2.5.2.post3.tar` & `types-aiobotocore-cloudsearch-2.5.4.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:37:26.347392 types-aiobotocore-cloudsearch-2.5.2.post3/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-04 12:19:51.000000 types-aiobotocore-cloudsearch-2.5.2.post3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    12406 2023-08-04 12:37:26.343392 types-aiobotocore-cloudsearch-2.5.2.post3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    10872 2023-08-04 12:19:51.000000 types-aiobotocore-cloudsearch-2.5.2.post3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-04 12:37:26.347392 types-aiobotocore-cloudsearch-2.5.2.post3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2100 2023-08-04 12:19:50.000000 types-aiobotocore-cloudsearch-2.5.2.post3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:37:26.343392 types-aiobotocore-cloudsearch-2.5.2.post3/types_aiobotocore_cloudsearch/
--rw-r--r--   0 runner    (1001) docker     (123)      474 2023-08-04 12:19:51.000000 types-aiobotocore-cloudsearch-2.5.2.post3/types_aiobotocore_cloudsearch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      473 2023-08-04 12:19:51.000000 types-aiobotocore-cloudsearch-2.5.2.post3/types_aiobotocore_cloudsearch/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      959 2023-08-04 12:19:51.000000 types-aiobotocore-cloudsearch-2.5.2.post3/types_aiobotocore_cloudsearch/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20176 2023-08-04 12:19:51.000000 types-aiobotocore-cloudsearch-2.5.2.post3/types_aiobotocore_cloudsearch/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    20142 2023-08-04 12:19:51.000000 types-aiobotocore-cloudsearch-2.5.2.post3/types_aiobotocore_cloudsearch/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9412 2023-08-04 12:19:51.000000 types-aiobotocore-cloudsearch-2.5.2.post3/types_aiobotocore_cloudsearch/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     9410 2023-08-04 12:19:51.000000 types-aiobotocore-cloudsearch-2.5.2.post3/types_aiobotocore_cloudsearch/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 12:19:51.000000 types-aiobotocore-cloudsearch-2.5.2.post3/types_aiobotocore_cloudsearch/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    25497 2023-08-04 12:19:51.000000 types-aiobotocore-cloudsearch-2.5.2.post3/types_aiobotocore_cloudsearch/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    25472 2023-08-04 12:19:51.000000 types-aiobotocore-cloudsearch-2.5.2.post3/types_aiobotocore_cloudsearch/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-04 12:19:51.000000 types-aiobotocore-cloudsearch-2.5.2.post3/types_aiobotocore_cloudsearch/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:37:26.343392 types-aiobotocore-cloudsearch-2.5.2.post3/types_aiobotocore_cloudsearch.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    12406 2023-08-04 12:37:26.000000 types-aiobotocore-cloudsearch-2.5.2.post3/types_aiobotocore_cloudsearch.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      802 2023-08-04 12:37:26.000000 types-aiobotocore-cloudsearch-2.5.2.post3/types_aiobotocore_cloudsearch.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 12:37:26.000000 types-aiobotocore-cloudsearch-2.5.2.post3/types_aiobotocore_cloudsearch.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 12:37:26.000000 types-aiobotocore-cloudsearch-2.5.2.post3/types_aiobotocore_cloudsearch.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-04 12:37:26.000000 types-aiobotocore-cloudsearch-2.5.2.post3/types_aiobotocore_cloudsearch.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-08-04 12:37:26.000000 types-aiobotocore-cloudsearch-2.5.2.post3/types_aiobotocore_cloudsearch.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:23:26.526626 types-aiobotocore-cloudsearch-2.5.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-08 01:07:32.000000 types-aiobotocore-cloudsearch-2.5.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    12400 2023-08-08 01:23:26.526626 types-aiobotocore-cloudsearch-2.5.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10872 2023-08-08 01:07:32.000000 types-aiobotocore-cloudsearch-2.5.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-08 01:23:26.526626 types-aiobotocore-cloudsearch-2.5.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2094 2023-08-08 01:07:32.000000 types-aiobotocore-cloudsearch-2.5.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:23:26.518626 types-aiobotocore-cloudsearch-2.5.4/types_aiobotocore_cloudsearch/
+-rw-r--r--   0 runner    (1001) docker     (123)      474 2023-08-08 01:07:32.000000 types-aiobotocore-cloudsearch-2.5.4/types_aiobotocore_cloudsearch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      473 2023-08-08 01:07:32.000000 types-aiobotocore-cloudsearch-2.5.4/types_aiobotocore_cloudsearch/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      947 2023-08-08 01:07:32.000000 types-aiobotocore-cloudsearch-2.5.4/types_aiobotocore_cloudsearch/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20176 2023-08-08 01:07:32.000000 types-aiobotocore-cloudsearch-2.5.4/types_aiobotocore_cloudsearch/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20142 2023-08-08 01:07:32.000000 types-aiobotocore-cloudsearch-2.5.4/types_aiobotocore_cloudsearch/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9507 2023-08-08 01:07:32.000000 types-aiobotocore-cloudsearch-2.5.4/types_aiobotocore_cloudsearch/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9505 2023-08-08 01:07:32.000000 types-aiobotocore-cloudsearch-2.5.4/types_aiobotocore_cloudsearch/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 01:07:32.000000 types-aiobotocore-cloudsearch-2.5.4/types_aiobotocore_cloudsearch/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    25497 2023-08-08 01:07:33.000000 types-aiobotocore-cloudsearch-2.5.4/types_aiobotocore_cloudsearch/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25472 2023-08-08 01:07:32.000000 types-aiobotocore-cloudsearch-2.5.4/types_aiobotocore_cloudsearch/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-08-08 01:07:32.000000 types-aiobotocore-cloudsearch-2.5.4/types_aiobotocore_cloudsearch/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:23:26.526626 types-aiobotocore-cloudsearch-2.5.4/types_aiobotocore_cloudsearch.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    12400 2023-08-08 01:23:26.000000 types-aiobotocore-cloudsearch-2.5.4/types_aiobotocore_cloudsearch.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      802 2023-08-08 01:23:26.000000 types-aiobotocore-cloudsearch-2.5.4/types_aiobotocore_cloudsearch.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 01:23:26.000000 types-aiobotocore-cloudsearch-2.5.4/types_aiobotocore_cloudsearch.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 01:23:26.000000 types-aiobotocore-cloudsearch-2.5.4/types_aiobotocore_cloudsearch.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-08 01:23:26.000000 types-aiobotocore-cloudsearch-2.5.4/types_aiobotocore_cloudsearch.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-08-08 01:23:26.000000 types-aiobotocore-cloudsearch-2.5.4/types_aiobotocore_cloudsearch.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-cloudsearch-2.5.2.post3/LICENSE` & `types-aiobotocore-cloudsearch-2.5.4/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-cloudsearch-2.5.2.post3/PKG-INFO` & `types-aiobotocore-cloudsearch-2.5.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-cloudsearch
-Version: 2.5.2.post3
-Summary: Type annotations for aiobotocore.CloudSearch 2.5.2 service generated with mypy-boto3-builder 7.17.2
+Version: 2.5.4
+Summary: Type annotations for aiobotocore.CloudSearch 2.5.4 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudsearch/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-cloudsearch.svg?color=blue)](https://pypi.org/project/types-aiobotocore-cloudsearch)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudsearch/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-cloudsearch)](https://pepy.tech/project/types-aiobotocore-cloudsearch)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.CloudSearch 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudsearch.html#CloudSearch)
+[aiobotocore.CloudSearch 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudsearch.html#CloudSearch)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-cloudsearch-2.5.2.post3/README.md` & `types-aiobotocore-cloudsearch-2.5.4/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-cloudsearch.svg?color=blue)](https://pypi.org/project/types-aiobotocore-cloudsearch)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudsearch/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-cloudsearch)](https://pepy.tech/project/types-aiobotocore-cloudsearch)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.CloudSearch 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudsearch.html#CloudSearch)
+[aiobotocore.CloudSearch 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudsearch.html#CloudSearch)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-cloudsearch-2.5.2.post3/setup.py` & `types-aiobotocore-cloudsearch-2.5.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-cloudsearch",
-    version="2.5.2.post3",
+    version="2.5.4",
     packages=["types_aiobotocore_cloudsearch"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.CloudSearch 2.5.2 service generated with"
+        "Type annotations for aiobotocore.CloudSearch 2.5.4 service generated with"
         " mypy-boto3-builder 7.17.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
```

### Comparing `types-aiobotocore-cloudsearch-2.5.2.post3/types_aiobotocore_cloudsearch/__main__.py` & `types-aiobotocore-cloudsearch-2.5.4/types_aiobotocore_cloudsearch/__main__.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.CloudSearch 2.5.2\nVersion:         2.5.2.post3\nBuilder"
+        "Type annotations for aiobotocore.CloudSearch 2.5.4\nVersion:         2.5.4\nBuilder"
         " version: 7.17.2\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudsearch//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudsearch.html#CloudSearch\nOther"
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

### Comparing `types-aiobotocore-cloudsearch-2.5.2.post3/types_aiobotocore_cloudsearch/client.py` & `types-aiobotocore-cloudsearch-2.5.4/types_aiobotocore_cloudsearch/client.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-cloudsearch-2.5.2.post3/types_aiobotocore_cloudsearch/client.pyi` & `types-aiobotocore-cloudsearch-2.5.4/types_aiobotocore_cloudsearch/client.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-cloudsearch-2.5.2.post3/types_aiobotocore_cloudsearch/literals.py` & `types-aiobotocore-cloudsearch-2.5.4/types_aiobotocore_cloudsearch/literals.py`

 * *Files 1% similar despite different names*

```diff
@@ -119,14 +119,15 @@
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
@@ -222,14 +223,15 @@
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
@@ -308,26 +310,28 @@
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

### Comparing `types-aiobotocore-cloudsearch-2.5.2.post3/types_aiobotocore_cloudsearch/literals.pyi` & `types-aiobotocore-cloudsearch-2.5.4/types_aiobotocore_cloudsearch/literals.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -117,14 +117,15 @@
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
@@ -220,14 +221,15 @@
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
@@ -306,26 +308,28 @@
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

### Comparing `types-aiobotocore-cloudsearch-2.5.2.post3/types_aiobotocore_cloudsearch/type_defs.py` & `types-aiobotocore-cloudsearch-2.5.4/types_aiobotocore_cloudsearch/type_defs.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-cloudsearch-2.5.2.post3/types_aiobotocore_cloudsearch/type_defs.pyi` & `types-aiobotocore-cloudsearch-2.5.4/types_aiobotocore_cloudsearch/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-cloudsearch-2.5.2.post3/types_aiobotocore_cloudsearch.egg-info/PKG-INFO` & `types-aiobotocore-cloudsearch-2.5.4/types_aiobotocore_cloudsearch.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-cloudsearch
-Version: 2.5.2.post3
-Summary: Type annotations for aiobotocore.CloudSearch 2.5.2 service generated with mypy-boto3-builder 7.17.2
+Version: 2.5.4
+Summary: Type annotations for aiobotocore.CloudSearch 2.5.4 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudsearch/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-cloudsearch.svg?color=blue)](https://pypi.org/project/types-aiobotocore-cloudsearch)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudsearch/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-cloudsearch)](https://pepy.tech/project/types-aiobotocore-cloudsearch)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.CloudSearch 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudsearch.html#CloudSearch)
+[aiobotocore.CloudSearch 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudsearch.html#CloudSearch)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-cloudsearch-2.5.2.post3/types_aiobotocore_cloudsearch.egg-info/SOURCES.txt` & `types-aiobotocore-cloudsearch-2.5.4/types_aiobotocore_cloudsearch.egg-info/SOURCES.txt`

 * *Files identical despite different names*


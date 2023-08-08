# Comparing `tmp/types-aiobotocore-cloud9-2.5.2.post3.tar.gz` & `tmp/types-aiobotocore-cloud9-2.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-cloud9-2.5.2.post3.tar", last modified: Fri Aug  4 12:37:24 2023, max compression
+gzip compressed data, was "types-aiobotocore-cloud9-2.5.4.tar", last modified: Tue Aug  8 01:23:24 2023, max compression
```

## Comparing `types-aiobotocore-cloud9-2.5.2.post3.tar` & `types-aiobotocore-cloud9-2.5.4.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:37:24.075336 types-aiobotocore-cloud9-2.5.2.post3/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-04 12:19:27.000000 types-aiobotocore-cloud9-2.5.2.post3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    13057 2023-08-04 12:37:24.071336 types-aiobotocore-cloud9-2.5.2.post3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    11543 2023-08-04 12:19:27.000000 types-aiobotocore-cloud9-2.5.2.post3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-04 12:37:24.075336 types-aiobotocore-cloud9-2.5.2.post3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2065 2023-08-04 12:19:27.000000 types-aiobotocore-cloud9-2.5.2.post3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:37:24.067336 types-aiobotocore-cloud9-2.5.2.post3/types_aiobotocore_cloud9/
--rw-r--r--   0 runner    (1001) docker     (123)      950 2023-08-04 12:19:27.000000 types-aiobotocore-cloud9-2.5.2.post3/types_aiobotocore_cloud9/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      949 2023-08-04 12:19:27.000000 types-aiobotocore-cloud9-2.5.2.post3/types_aiobotocore_cloud9/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      928 2023-08-04 12:19:28.000000 types-aiobotocore-cloud9-2.5.2.post3/types_aiobotocore_cloud9/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13609 2023-08-04 12:19:28.000000 types-aiobotocore-cloud9-2.5.2.post3/types_aiobotocore_cloud9/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    13585 2023-08-04 12:19:28.000000 types-aiobotocore-cloud9-2.5.2.post3/types_aiobotocore_cloud9/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9453 2023-08-04 12:19:28.000000 types-aiobotocore-cloud9-2.5.2.post3/types_aiobotocore_cloud9/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     9451 2023-08-04 12:19:28.000000 types-aiobotocore-cloud9-2.5.2.post3/types_aiobotocore_cloud9/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     3416 2023-08-04 12:19:28.000000 types-aiobotocore-cloud9-2.5.2.post3/types_aiobotocore_cloud9/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     3412 2023-08-04 12:19:28.000000 types-aiobotocore-cloud9-2.5.2.post3/types_aiobotocore_cloud9/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 12:19:28.000000 types-aiobotocore-cloud9-2.5.2.post3/types_aiobotocore_cloud9/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     9717 2023-08-04 12:19:29.000000 types-aiobotocore-cloud9-2.5.2.post3/types_aiobotocore_cloud9/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)     9708 2023-08-04 12:19:29.000000 types-aiobotocore-cloud9-2.5.2.post3/types_aiobotocore_cloud9/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-04 12:19:27.000000 types-aiobotocore-cloud9-2.5.2.post3/types_aiobotocore_cloud9/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:37:24.071336 types-aiobotocore-cloud9-2.5.2.post3/types_aiobotocore_cloud9.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    13057 2023-08-04 12:37:23.000000 types-aiobotocore-cloud9-2.5.2.post3/types_aiobotocore_cloud9.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      794 2023-08-04 12:37:23.000000 types-aiobotocore-cloud9-2.5.2.post3/types_aiobotocore_cloud9.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 12:37:23.000000 types-aiobotocore-cloud9-2.5.2.post3/types_aiobotocore_cloud9.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 12:37:23.000000 types-aiobotocore-cloud9-2.5.2.post3/types_aiobotocore_cloud9.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-04 12:37:23.000000 types-aiobotocore-cloud9-2.5.2.post3/types_aiobotocore_cloud9.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-08-04 12:37:23.000000 types-aiobotocore-cloud9-2.5.2.post3/types_aiobotocore_cloud9.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:23:24.610624 types-aiobotocore-cloud9-2.5.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-08 01:07:11.000000 types-aiobotocore-cloud9-2.5.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    13051 2023-08-08 01:23:24.598624 types-aiobotocore-cloud9-2.5.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    11543 2023-08-08 01:07:11.000000 types-aiobotocore-cloud9-2.5.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-08 01:23:24.610624 types-aiobotocore-cloud9-2.5.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2059 2023-08-08 01:07:11.000000 types-aiobotocore-cloud9-2.5.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:23:24.598624 types-aiobotocore-cloud9-2.5.4/types_aiobotocore_cloud9/
+-rw-r--r--   0 runner    (1001) docker     (123)      950 2023-08-08 01:07:11.000000 types-aiobotocore-cloud9-2.5.4/types_aiobotocore_cloud9/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      949 2023-08-08 01:07:11.000000 types-aiobotocore-cloud9-2.5.4/types_aiobotocore_cloud9/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      916 2023-08-08 01:07:11.000000 types-aiobotocore-cloud9-2.5.4/types_aiobotocore_cloud9/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13609 2023-08-08 01:07:11.000000 types-aiobotocore-cloud9-2.5.4/types_aiobotocore_cloud9/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13585 2023-08-08 01:07:11.000000 types-aiobotocore-cloud9-2.5.4/types_aiobotocore_cloud9/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9548 2023-08-08 01:07:12.000000 types-aiobotocore-cloud9-2.5.4/types_aiobotocore_cloud9/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9546 2023-08-08 01:07:11.000000 types-aiobotocore-cloud9-2.5.4/types_aiobotocore_cloud9/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     3416 2023-08-08 01:07:11.000000 types-aiobotocore-cloud9-2.5.4/types_aiobotocore_cloud9/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3412 2023-08-08 01:07:11.000000 types-aiobotocore-cloud9-2.5.4/types_aiobotocore_cloud9/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 01:07:11.000000 types-aiobotocore-cloud9-2.5.4/types_aiobotocore_cloud9/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     9717 2023-08-08 01:07:12.000000 types-aiobotocore-cloud9-2.5.4/types_aiobotocore_cloud9/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9708 2023-08-08 01:07:12.000000 types-aiobotocore-cloud9-2.5.4/types_aiobotocore_cloud9/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-08-08 01:07:11.000000 types-aiobotocore-cloud9-2.5.4/types_aiobotocore_cloud9/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:23:24.598624 types-aiobotocore-cloud9-2.5.4/types_aiobotocore_cloud9.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    13051 2023-08-08 01:23:24.000000 types-aiobotocore-cloud9-2.5.4/types_aiobotocore_cloud9.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      794 2023-08-08 01:23:24.000000 types-aiobotocore-cloud9-2.5.4/types_aiobotocore_cloud9.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 01:23:24.000000 types-aiobotocore-cloud9-2.5.4/types_aiobotocore_cloud9.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 01:23:24.000000 types-aiobotocore-cloud9-2.5.4/types_aiobotocore_cloud9.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-08 01:23:24.000000 types-aiobotocore-cloud9-2.5.4/types_aiobotocore_cloud9.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-08-08 01:23:24.000000 types-aiobotocore-cloud9-2.5.4/types_aiobotocore_cloud9.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-cloud9-2.5.2.post3/LICENSE` & `types-aiobotocore-cloud9-2.5.4/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-cloud9-2.5.2.post3/PKG-INFO` & `types-aiobotocore-cloud9-2.5.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-cloud9
-Version: 2.5.2.post3
-Summary: Type annotations for aiobotocore.Cloud9 2.5.2 service generated with mypy-boto3-builder 7.17.2
+Version: 2.5.4
+Summary: Type annotations for aiobotocore.Cloud9 2.5.4 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloud9/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-cloud9.svg?color=blue)](https://pypi.org/project/types-aiobotocore-cloud9)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloud9/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-cloud9)](https://pepy.tech/project/types-aiobotocore-cloud9)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.Cloud9 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloud9.html#Cloud9)
+[aiobotocore.Cloud9 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloud9.html#Cloud9)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-cloud9-2.5.2.post3/README.md` & `types-aiobotocore-cloud9-2.5.4/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-cloud9.svg?color=blue)](https://pypi.org/project/types-aiobotocore-cloud9)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloud9/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-cloud9)](https://pepy.tech/project/types-aiobotocore-cloud9)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.Cloud9 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloud9.html#Cloud9)
+[aiobotocore.Cloud9 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloud9.html#Cloud9)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-cloud9-2.5.2.post3/setup.py` & `types-aiobotocore-cloud9-2.5.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-cloud9",
-    version="2.5.2.post3",
+    version="2.5.4",
     packages=["types_aiobotocore_cloud9"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.Cloud9 2.5.2 service generated with mypy-boto3-builder"
+        "Type annotations for aiobotocore.Cloud9 2.5.4 service generated with mypy-boto3-builder"
         " 7.17.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
```

### Comparing `types-aiobotocore-cloud9-2.5.2.post3/types_aiobotocore_cloud9/__init__.py` & `types-aiobotocore-cloud9-2.5.4/types_aiobotocore_cloud9/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-cloud9-2.5.2.post3/types_aiobotocore_cloud9/__init__.pyi` & `types-aiobotocore-cloud9-2.5.4/types_aiobotocore_cloud9/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-cloud9-2.5.2.post3/types_aiobotocore_cloud9/__main__.py` & `types-aiobotocore-cloud9-2.5.4/types_aiobotocore_cloud9/__main__.py`

 * *Files 13% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.Cloud9 2.5.2\nVersion:         2.5.2.post3\nBuilder"
-        " version: 7.17.2\nDocs:           "
+        "Type annotations for aiobotocore.Cloud9 2.5.4\nVersion:         2.5.4\nBuilder version:"
+        " 7.17.2\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloud9//\nBoto3 docs: "
         "     https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloud9.html#Cloud9\nOther"
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

### Comparing `types-aiobotocore-cloud9-2.5.2.post3/types_aiobotocore_cloud9/client.py` & `types-aiobotocore-cloud9-2.5.4/types_aiobotocore_cloud9/client.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-cloud9-2.5.2.post3/types_aiobotocore_cloud9/client.pyi` & `types-aiobotocore-cloud9-2.5.4/types_aiobotocore_cloud9/client.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-cloud9-2.5.2.post3/types_aiobotocore_cloud9/literals.py` & `types-aiobotocore-cloud9-2.5.4/types_aiobotocore_cloud9/literals.py`

 * *Files 2% similar despite different names*

```diff
@@ -76,14 +76,15 @@
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
@@ -179,14 +180,15 @@
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
@@ -265,26 +267,28 @@
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

### Comparing `types-aiobotocore-cloud9-2.5.2.post3/types_aiobotocore_cloud9/literals.pyi` & `types-aiobotocore-cloud9-2.5.4/types_aiobotocore_cloud9/literals.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -74,14 +74,15 @@
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
@@ -177,14 +178,15 @@
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
@@ -263,26 +265,28 @@
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

### Comparing `types-aiobotocore-cloud9-2.5.2.post3/types_aiobotocore_cloud9/paginator.py` & `types-aiobotocore-cloud9-2.5.4/types_aiobotocore_cloud9/paginator.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-cloud9-2.5.2.post3/types_aiobotocore_cloud9/paginator.pyi` & `types-aiobotocore-cloud9-2.5.4/types_aiobotocore_cloud9/paginator.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-cloud9-2.5.2.post3/types_aiobotocore_cloud9/type_defs.py` & `types-aiobotocore-cloud9-2.5.4/types_aiobotocore_cloud9/type_defs.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-cloud9-2.5.2.post3/types_aiobotocore_cloud9/type_defs.pyi` & `types-aiobotocore-cloud9-2.5.4/types_aiobotocore_cloud9/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-cloud9-2.5.2.post3/types_aiobotocore_cloud9.egg-info/PKG-INFO` & `types-aiobotocore-cloud9-2.5.4/types_aiobotocore_cloud9.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-cloud9
-Version: 2.5.2.post3
-Summary: Type annotations for aiobotocore.Cloud9 2.5.2 service generated with mypy-boto3-builder 7.17.2
+Version: 2.5.4
+Summary: Type annotations for aiobotocore.Cloud9 2.5.4 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloud9/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-cloud9.svg?color=blue)](https://pypi.org/project/types-aiobotocore-cloud9)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloud9/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-cloud9)](https://pepy.tech/project/types-aiobotocore-cloud9)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.Cloud9 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloud9.html#Cloud9)
+[aiobotocore.Cloud9 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloud9.html#Cloud9)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-cloud9-2.5.2.post3/types_aiobotocore_cloud9.egg-info/SOURCES.txt` & `types-aiobotocore-cloud9-2.5.4/types_aiobotocore_cloud9.egg-info/SOURCES.txt`

 * *Files identical despite different names*


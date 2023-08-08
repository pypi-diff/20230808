# Comparing `tmp/types-aiobotocore-ds-2.5.2.post3.tar.gz` & `tmp/types-aiobotocore-ds-2.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-ds-2.5.2.post3.tar", last modified: Fri Aug  4 12:37:37 2023, max compression
+gzip compressed data, was "types-aiobotocore-ds-2.5.4.tar", last modified: Tue Aug  8 01:23:38 2023, max compression
```

## Comparing `types-aiobotocore-ds-2.5.2.post3.tar` & `types-aiobotocore-ds-2.5.4.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:37:36.995653 types-aiobotocore-ds-2.5.2.post3/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-04 12:21:47.000000 types-aiobotocore-ds-2.5.2.post3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    14973 2023-08-04 12:37:36.995653 types-aiobotocore-ds-2.5.2.post3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    13461 2023-08-04 12:21:47.000000 types-aiobotocore-ds-2.5.2.post3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-04 12:37:36.995653 types-aiobotocore-ds-2.5.2.post3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2027 2023-08-04 12:21:47.000000 types-aiobotocore-ds-2.5.2.post3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:37:36.983653 types-aiobotocore-ds-2.5.2.post3/types_aiobotocore_ds/
--rw-r--r--   0 runner    (1001) docker     (123)     3709 2023-08-04 12:21:47.000000 types-aiobotocore-ds-2.5.2.post3/types_aiobotocore_ds/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3708 2023-08-04 12:21:47.000000 types-aiobotocore-ds-2.5.2.post3/types_aiobotocore_ds/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      940 2023-08-04 12:21:47.000000 types-aiobotocore-ds-2.5.2.post3/types_aiobotocore_ds/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    54551 2023-08-04 12:21:47.000000 types-aiobotocore-ds-2.5.2.post3/types_aiobotocore_ds/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    54461 2023-08-04 12:21:47.000000 types-aiobotocore-ds-2.5.2.post3/types_aiobotocore_ds/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    13611 2023-08-04 12:21:49.000000 types-aiobotocore-ds-2.5.2.post3/types_aiobotocore_ds/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    13609 2023-08-04 12:21:49.000000 types-aiobotocore-ds-2.5.2.post3/types_aiobotocore_ds/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    17748 2023-08-04 12:21:48.000000 types-aiobotocore-ds-2.5.2.post3/types_aiobotocore_ds/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)    17731 2023-08-04 12:21:48.000000 types-aiobotocore-ds-2.5.2.post3/types_aiobotocore_ds/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 12:21:47.000000 types-aiobotocore-ds-2.5.2.post3/types_aiobotocore_ds/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    57645 2023-08-04 12:21:50.000000 types-aiobotocore-ds-2.5.2.post3/types_aiobotocore_ds/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    57572 2023-08-04 12:21:49.000000 types-aiobotocore-ds-2.5.2.post3/types_aiobotocore_ds/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-04 12:21:47.000000 types-aiobotocore-ds-2.5.2.post3/types_aiobotocore_ds/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:37:36.995653 types-aiobotocore-ds-2.5.2.post3/types_aiobotocore_ds.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    14973 2023-08-04 12:37:36.000000 types-aiobotocore-ds-2.5.2.post3/types_aiobotocore_ds.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      718 2023-08-04 12:37:36.000000 types-aiobotocore-ds-2.5.2.post3/types_aiobotocore_ds.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 12:37:36.000000 types-aiobotocore-ds-2.5.2.post3/types_aiobotocore_ds.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 12:37:36.000000 types-aiobotocore-ds-2.5.2.post3/types_aiobotocore_ds.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-04 12:37:36.000000 types-aiobotocore-ds-2.5.2.post3/types_aiobotocore_ds.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-08-04 12:37:36.000000 types-aiobotocore-ds-2.5.2.post3/types_aiobotocore_ds.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:23:38.282693 types-aiobotocore-ds-2.5.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-08 01:09:21.000000 types-aiobotocore-ds-2.5.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    14967 2023-08-08 01:23:38.278693 types-aiobotocore-ds-2.5.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    13461 2023-08-08 01:09:21.000000 types-aiobotocore-ds-2.5.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-08 01:23:38.282693 types-aiobotocore-ds-2.5.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2021 2023-08-08 01:09:21.000000 types-aiobotocore-ds-2.5.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:23:38.278693 types-aiobotocore-ds-2.5.4/types_aiobotocore_ds/
+-rw-r--r--   0 runner    (1001) docker     (123)     3709 2023-08-08 01:09:21.000000 types-aiobotocore-ds-2.5.4/types_aiobotocore_ds/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3708 2023-08-08 01:09:21.000000 types-aiobotocore-ds-2.5.4/types_aiobotocore_ds/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      928 2023-08-08 01:09:21.000000 types-aiobotocore-ds-2.5.4/types_aiobotocore_ds/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    54551 2023-08-08 01:09:22.000000 types-aiobotocore-ds-2.5.4/types_aiobotocore_ds/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    54461 2023-08-08 01:09:22.000000 types-aiobotocore-ds-2.5.4/types_aiobotocore_ds/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    13726 2023-08-08 01:09:22.000000 types-aiobotocore-ds-2.5.4/types_aiobotocore_ds/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13724 2023-08-08 01:09:22.000000 types-aiobotocore-ds-2.5.4/types_aiobotocore_ds/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    17748 2023-08-08 01:09:22.000000 types-aiobotocore-ds-2.5.4/types_aiobotocore_ds/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17731 2023-08-08 01:09:22.000000 types-aiobotocore-ds-2.5.4/types_aiobotocore_ds/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 01:09:21.000000 types-aiobotocore-ds-2.5.4/types_aiobotocore_ds/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    57645 2023-08-08 01:09:24.000000 types-aiobotocore-ds-2.5.4/types_aiobotocore_ds/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    57572 2023-08-08 01:09:23.000000 types-aiobotocore-ds-2.5.4/types_aiobotocore_ds/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-08-08 01:09:21.000000 types-aiobotocore-ds-2.5.4/types_aiobotocore_ds/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:23:38.278693 types-aiobotocore-ds-2.5.4/types_aiobotocore_ds.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    14967 2023-08-08 01:23:38.000000 types-aiobotocore-ds-2.5.4/types_aiobotocore_ds.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      718 2023-08-08 01:23:38.000000 types-aiobotocore-ds-2.5.4/types_aiobotocore_ds.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 01:23:38.000000 types-aiobotocore-ds-2.5.4/types_aiobotocore_ds.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 01:23:38.000000 types-aiobotocore-ds-2.5.4/types_aiobotocore_ds.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-08 01:23:38.000000 types-aiobotocore-ds-2.5.4/types_aiobotocore_ds.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-08-08 01:23:38.000000 types-aiobotocore-ds-2.5.4/types_aiobotocore_ds.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-ds-2.5.2.post3/LICENSE` & `types-aiobotocore-ds-2.5.4/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-ds-2.5.2.post3/PKG-INFO` & `types-aiobotocore-ds-2.5.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-ds
-Version: 2.5.2.post3
-Summary: Type annotations for aiobotocore.DirectoryService 2.5.2 service generated with mypy-boto3-builder 7.17.2
+Version: 2.5.4
+Summary: Type annotations for aiobotocore.DirectoryService 2.5.4 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ds/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-ds.svg?color=blue)](https://pypi.org/project/types-aiobotocore-ds)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ds/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-ds)](https://pepy.tech/project/types-aiobotocore-ds)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.DirectoryService 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ds.html#DirectoryService)
+[aiobotocore.DirectoryService 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ds.html#DirectoryService)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-ds-2.5.2.post3/README.md` & `types-aiobotocore-ds-2.5.4/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-ds.svg?color=blue)](https://pypi.org/project/types-aiobotocore-ds)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ds/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-ds)](https://pepy.tech/project/types-aiobotocore-ds)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.DirectoryService 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ds.html#DirectoryService)
+[aiobotocore.DirectoryService 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ds.html#DirectoryService)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-ds-2.5.2.post3/setup.py` & `types-aiobotocore-ds-2.5.4/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-ds",
-    version="2.5.2.post3",
+    version="2.5.4",
     packages=["types_aiobotocore_ds"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.DirectoryService 2.5.2 service generated with"
+        "Type annotations for aiobotocore.DirectoryService 2.5.4 service generated with"
         " mypy-boto3-builder 7.17.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
```

### Comparing `types-aiobotocore-ds-2.5.2.post3/types_aiobotocore_ds/__init__.py` & `types-aiobotocore-ds-2.5.4/types_aiobotocore_ds/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-ds-2.5.2.post3/types_aiobotocore_ds/__init__.pyi` & `types-aiobotocore-ds-2.5.4/types_aiobotocore_ds/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-ds-2.5.2.post3/types_aiobotocore_ds/__main__.py` & `types-aiobotocore-ds-2.5.4/types_aiobotocore_ds/__main__.py`

 * *Files 27% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.DirectoryService 2.5.2\nVersion:        "
-        " 2.5.2.post3\nBuilder version: 7.17.2\nDocs:           "
+        "Type annotations for aiobotocore.DirectoryService 2.5.4\nVersion:         2.5.4\nBuilder"
+        " version: 7.17.2\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ds//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ds.html#DirectoryService\nOther"
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

### Comparing `types-aiobotocore-ds-2.5.2.post3/types_aiobotocore_ds/client.py` & `types-aiobotocore-ds-2.5.4/types_aiobotocore_ds/client.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-ds-2.5.2.post3/types_aiobotocore_ds/client.pyi` & `types-aiobotocore-ds-2.5.4/types_aiobotocore_ds/client.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-ds-2.5.2.post3/types_aiobotocore_ds/literals.py` & `types-aiobotocore-ds-2.5.4/types_aiobotocore_ds/literals.py`

 * *Files 1% similar despite different names*

```diff
@@ -187,14 +187,15 @@
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
@@ -290,14 +291,15 @@
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
@@ -376,26 +378,28 @@
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
@@ -572,14 +576,15 @@
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

### Comparing `types-aiobotocore-ds-2.5.2.post3/types_aiobotocore_ds/literals.pyi` & `types-aiobotocore-ds-2.5.4/types_aiobotocore_ds/literals.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -185,14 +185,15 @@
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
@@ -288,14 +289,15 @@
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
@@ -374,26 +376,28 @@
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
@@ -570,14 +574,15 @@
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

### Comparing `types-aiobotocore-ds-2.5.2.post3/types_aiobotocore_ds/paginator.py` & `types-aiobotocore-ds-2.5.4/types_aiobotocore_ds/paginator.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-ds-2.5.2.post3/types_aiobotocore_ds/paginator.pyi` & `types-aiobotocore-ds-2.5.4/types_aiobotocore_ds/paginator.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-ds-2.5.2.post3/types_aiobotocore_ds/type_defs.py` & `types-aiobotocore-ds-2.5.4/types_aiobotocore_ds/type_defs.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-ds-2.5.2.post3/types_aiobotocore_ds/type_defs.pyi` & `types-aiobotocore-ds-2.5.4/types_aiobotocore_ds/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-ds-2.5.2.post3/types_aiobotocore_ds.egg-info/PKG-INFO` & `types-aiobotocore-ds-2.5.4/types_aiobotocore_ds.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-ds
-Version: 2.5.2.post3
-Summary: Type annotations for aiobotocore.DirectoryService 2.5.2 service generated with mypy-boto3-builder 7.17.2
+Version: 2.5.4
+Summary: Type annotations for aiobotocore.DirectoryService 2.5.4 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ds/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-ds.svg?color=blue)](https://pypi.org/project/types-aiobotocore-ds)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ds/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-ds)](https://pepy.tech/project/types-aiobotocore-ds)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.DirectoryService 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ds.html#DirectoryService)
+[aiobotocore.DirectoryService 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ds.html#DirectoryService)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-ds-2.5.2.post3/types_aiobotocore_ds.egg-info/SOURCES.txt` & `types-aiobotocore-ds-2.5.4/types_aiobotocore_ds.egg-info/SOURCES.txt`

 * *Files identical despite different names*


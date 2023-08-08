# Comparing `tmp/types-aiobotocore-efs-2.5.2.post3.tar.gz` & `tmp/types-aiobotocore-efs-2.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-efs-2.5.2.post3.tar", last modified: Fri Aug  4 12:37:39 2023, max compression
+gzip compressed data, was "types-aiobotocore-efs-2.5.4.tar", last modified: Tue Aug  8 01:23:40 2023, max compression
```

## Comparing `types-aiobotocore-efs-2.5.2.post3.tar` & `types-aiobotocore-efs-2.5.4.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:37:39.447711 types-aiobotocore-efs-2.5.2.post3/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-04 12:23:04.000000 types-aiobotocore-efs-2.5.2.post3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    13008 2023-08-04 12:37:39.447711 types-aiobotocore-efs-2.5.2.post3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    11506 2023-08-04 12:23:04.000000 types-aiobotocore-efs-2.5.2.post3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-04 12:37:39.447711 types-aiobotocore-efs-2.5.2.post3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2020 2023-08-04 12:23:04.000000 types-aiobotocore-efs-2.5.2.post3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:37:39.435711 types-aiobotocore-efs-2.5.2.post3/types_aiobotocore_efs/
--rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-08-04 12:23:04.000000 types-aiobotocore-efs-2.5.2.post3/types_aiobotocore_efs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-08-04 12:23:04.000000 types-aiobotocore-efs-2.5.2.post3/types_aiobotocore_efs/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      916 2023-08-04 12:23:04.000000 types-aiobotocore-efs-2.5.2.post3/types_aiobotocore_efs/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    25215 2023-08-04 12:23:04.000000 types-aiobotocore-efs-2.5.2.post3/types_aiobotocore_efs/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    25173 2023-08-04 12:23:04.000000 types-aiobotocore-efs-2.5.2.post3/types_aiobotocore_efs/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9485 2023-08-04 12:23:04.000000 types-aiobotocore-efs-2.5.2.post3/types_aiobotocore_efs/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     9483 2023-08-04 12:23:04.000000 types-aiobotocore-efs-2.5.2.post3/types_aiobotocore_efs/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     4330 2023-08-04 12:23:04.000000 types-aiobotocore-efs-2.5.2.post3/types_aiobotocore_efs/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     4325 2023-08-04 12:23:04.000000 types-aiobotocore-efs-2.5.2.post3/types_aiobotocore_efs/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 12:23:04.000000 types-aiobotocore-efs-2.5.2.post3/types_aiobotocore_efs/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    24148 2023-08-04 12:23:05.000000 types-aiobotocore-efs-2.5.2.post3/types_aiobotocore_efs/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    24119 2023-08-04 12:23:05.000000 types-aiobotocore-efs-2.5.2.post3/types_aiobotocore_efs/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-04 12:23:04.000000 types-aiobotocore-efs-2.5.2.post3/types_aiobotocore_efs/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:37:39.447711 types-aiobotocore-efs-2.5.2.post3/types_aiobotocore_efs.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    13008 2023-08-04 12:37:39.000000 types-aiobotocore-efs-2.5.2.post3/types_aiobotocore_efs.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      737 2023-08-04 12:37:39.000000 types-aiobotocore-efs-2.5.2.post3/types_aiobotocore_efs.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 12:37:39.000000 types-aiobotocore-efs-2.5.2.post3/types_aiobotocore_efs.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 12:37:39.000000 types-aiobotocore-efs-2.5.2.post3/types_aiobotocore_efs.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-04 12:37:39.000000 types-aiobotocore-efs-2.5.2.post3/types_aiobotocore_efs.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-08-04 12:37:39.000000 types-aiobotocore-efs-2.5.2.post3/types_aiobotocore_efs.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:23:40.690703 types-aiobotocore-efs-2.5.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-08 01:10:31.000000 types-aiobotocore-efs-2.5.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    13002 2023-08-08 01:23:40.690703 types-aiobotocore-efs-2.5.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    11506 2023-08-08 01:10:31.000000 types-aiobotocore-efs-2.5.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-08 01:23:40.690703 types-aiobotocore-efs-2.5.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2014 2023-08-08 01:10:30.000000 types-aiobotocore-efs-2.5.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:23:40.690703 types-aiobotocore-efs-2.5.4/types_aiobotocore_efs/
+-rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-08-08 01:10:31.000000 types-aiobotocore-efs-2.5.4/types_aiobotocore_efs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-08-08 01:10:31.000000 types-aiobotocore-efs-2.5.4/types_aiobotocore_efs/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      904 2023-08-08 01:10:31.000000 types-aiobotocore-efs-2.5.4/types_aiobotocore_efs/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25215 2023-08-08 01:10:31.000000 types-aiobotocore-efs-2.5.4/types_aiobotocore_efs/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25173 2023-08-08 01:10:31.000000 types-aiobotocore-efs-2.5.4/types_aiobotocore_efs/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9580 2023-08-08 01:10:31.000000 types-aiobotocore-efs-2.5.4/types_aiobotocore_efs/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9578 2023-08-08 01:10:31.000000 types-aiobotocore-efs-2.5.4/types_aiobotocore_efs/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     4330 2023-08-08 01:10:31.000000 types-aiobotocore-efs-2.5.4/types_aiobotocore_efs/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4325 2023-08-08 01:10:31.000000 types-aiobotocore-efs-2.5.4/types_aiobotocore_efs/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 01:10:31.000000 types-aiobotocore-efs-2.5.4/types_aiobotocore_efs/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    24148 2023-08-08 01:10:31.000000 types-aiobotocore-efs-2.5.4/types_aiobotocore_efs/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24119 2023-08-08 01:10:31.000000 types-aiobotocore-efs-2.5.4/types_aiobotocore_efs/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-08-08 01:10:31.000000 types-aiobotocore-efs-2.5.4/types_aiobotocore_efs/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:23:40.690703 types-aiobotocore-efs-2.5.4/types_aiobotocore_efs.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    13002 2023-08-08 01:23:40.000000 types-aiobotocore-efs-2.5.4/types_aiobotocore_efs.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      737 2023-08-08 01:23:40.000000 types-aiobotocore-efs-2.5.4/types_aiobotocore_efs.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 01:23:40.000000 types-aiobotocore-efs-2.5.4/types_aiobotocore_efs.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 01:23:40.000000 types-aiobotocore-efs-2.5.4/types_aiobotocore_efs.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-08 01:23:40.000000 types-aiobotocore-efs-2.5.4/types_aiobotocore_efs.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-08-08 01:23:40.000000 types-aiobotocore-efs-2.5.4/types_aiobotocore_efs.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-efs-2.5.2.post3/LICENSE` & `types-aiobotocore-efs-2.5.4/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-efs-2.5.2.post3/PKG-INFO` & `types-aiobotocore-efs-2.5.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-efs
-Version: 2.5.2.post3
-Summary: Type annotations for aiobotocore.EFS 2.5.2 service generated with mypy-boto3-builder 7.17.2
+Version: 2.5.4
+Summary: Type annotations for aiobotocore.EFS 2.5.4 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_efs/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-efs.svg?color=blue)](https://pypi.org/project/types-aiobotocore-efs)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_efs/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-efs)](https://pepy.tech/project/types-aiobotocore-efs)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.EFS 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/efs.html#EFS)
+[aiobotocore.EFS 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/efs.html#EFS)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-efs-2.5.2.post3/README.md` & `types-aiobotocore-efs-2.5.4/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-efs.svg?color=blue)](https://pypi.org/project/types-aiobotocore-efs)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_efs/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-efs)](https://pepy.tech/project/types-aiobotocore-efs)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.EFS 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/efs.html#EFS)
+[aiobotocore.EFS 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/efs.html#EFS)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-efs-2.5.2.post3/setup.py` & `types-aiobotocore-efs-2.5.4/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-efs",
-    version="2.5.2.post3",
+    version="2.5.4",
     packages=["types_aiobotocore_efs"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.EFS 2.5.2 service generated with mypy-boto3-builder"
+        "Type annotations for aiobotocore.EFS 2.5.4 service generated with mypy-boto3-builder"
         " 7.17.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
```

### Comparing `types-aiobotocore-efs-2.5.2.post3/types_aiobotocore_efs/__init__.py` & `types-aiobotocore-efs-2.5.4/types_aiobotocore_efs/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-efs-2.5.2.post3/types_aiobotocore_efs/__init__.pyi` & `types-aiobotocore-efs-2.5.4/types_aiobotocore_efs/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-efs-2.5.2.post3/types_aiobotocore_efs/__main__.py` & `types-aiobotocore-efs-2.5.4/types_aiobotocore_efs/__main__.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.EFS 2.5.2\nVersion:         2.5.2.post3\nBuilder version:"
+        "Type annotations for aiobotocore.EFS 2.5.4\nVersion:         2.5.4\nBuilder version:"
         " 7.17.2\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_efs//\nBoto3 docs:    "
         "  https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/efs.html#EFS\nOther"
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

### Comparing `types-aiobotocore-efs-2.5.2.post3/types_aiobotocore_efs/client.py` & `types-aiobotocore-efs-2.5.4/types_aiobotocore_efs/client.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-efs-2.5.2.post3/types_aiobotocore_efs/client.pyi` & `types-aiobotocore-efs-2.5.4/types_aiobotocore_efs/client.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-efs-2.5.2.post3/types_aiobotocore_efs/literals.py` & `types-aiobotocore-efs-2.5.4/types_aiobotocore_efs/literals.py`

 * *Files 0% similar despite different names*

```diff
@@ -71,14 +71,15 @@
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
@@ -174,14 +175,15 @@
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
@@ -260,26 +262,28 @@
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

### Comparing `types-aiobotocore-efs-2.5.2.post3/types_aiobotocore_efs/literals.pyi` & `types-aiobotocore-efs-2.5.4/types_aiobotocore_efs/literals.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -69,14 +69,15 @@
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
@@ -172,14 +173,15 @@
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
@@ -258,26 +260,28 @@
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

### Comparing `types-aiobotocore-efs-2.5.2.post3/types_aiobotocore_efs/paginator.py` & `types-aiobotocore-efs-2.5.4/types_aiobotocore_efs/paginator.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-efs-2.5.2.post3/types_aiobotocore_efs/paginator.pyi` & `types-aiobotocore-efs-2.5.4/types_aiobotocore_efs/paginator.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-efs-2.5.2.post3/types_aiobotocore_efs/type_defs.py` & `types-aiobotocore-efs-2.5.4/types_aiobotocore_efs/type_defs.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-efs-2.5.2.post3/types_aiobotocore_efs/type_defs.pyi` & `types-aiobotocore-efs-2.5.4/types_aiobotocore_efs/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-efs-2.5.2.post3/types_aiobotocore_efs.egg-info/PKG-INFO` & `types-aiobotocore-efs-2.5.4/types_aiobotocore_efs.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-efs
-Version: 2.5.2.post3
-Summary: Type annotations for aiobotocore.EFS 2.5.2 service generated with mypy-boto3-builder 7.17.2
+Version: 2.5.4
+Summary: Type annotations for aiobotocore.EFS 2.5.4 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_efs/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-efs.svg?color=blue)](https://pypi.org/project/types-aiobotocore-efs)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_efs/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-efs)](https://pepy.tech/project/types-aiobotocore-efs)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.EFS 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/efs.html#EFS)
+[aiobotocore.EFS 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/efs.html#EFS)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-efs-2.5.2.post3/types_aiobotocore_efs.egg-info/SOURCES.txt` & `types-aiobotocore-efs-2.5.4/types_aiobotocore_efs.egg-info/SOURCES.txt`

 * *Files identical despite different names*


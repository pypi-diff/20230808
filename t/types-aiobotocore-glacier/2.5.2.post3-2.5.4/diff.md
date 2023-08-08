# Comparing `tmp/types-aiobotocore-glacier-2.5.2.post3.tar.gz` & `tmp/types-aiobotocore-glacier-2.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-glacier-2.5.2.post3.tar", last modified: Fri Aug  4 12:37:46 2023, max compression
+gzip compressed data, was "types-aiobotocore-glacier-2.5.4.tar", last modified: Tue Aug  8 01:23:46 2023, max compression
```

## Comparing `types-aiobotocore-glacier-2.5.2.post3.tar` & `types-aiobotocore-glacier-2.5.4.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:37:46.383874 types-aiobotocore-glacier-2.5.2.post3/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-04 12:24:16.000000 types-aiobotocore-glacier-2.5.2.post3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    16428 2023-08-04 12:37:46.363873 types-aiobotocore-glacier-2.5.2.post3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    14910 2023-08-04 12:24:16.000000 types-aiobotocore-glacier-2.5.2.post3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-04 12:37:46.383874 types-aiobotocore-glacier-2.5.2.post3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2072 2023-08-04 12:24:16.000000 types-aiobotocore-glacier-2.5.2.post3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:37:46.363873 types-aiobotocore-glacier-2.5.2.post3/types_aiobotocore_glacier/
--rw-r--r--   0 runner    (1001) docker     (123)     1735 2023-08-04 12:24:16.000000 types-aiobotocore-glacier-2.5.2.post3/types_aiobotocore_glacier/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1733 2023-08-04 12:24:16.000000 types-aiobotocore-glacier-2.5.2.post3/types_aiobotocore_glacier/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      943 2023-08-04 12:24:16.000000 types-aiobotocore-glacier-2.5.2.post3/types_aiobotocore_glacier/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    28395 2023-08-04 12:24:16.000000 types-aiobotocore-glacier-2.5.2.post3/types_aiobotocore_glacier/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    28347 2023-08-04 12:24:16.000000 types-aiobotocore-glacier-2.5.2.post3/types_aiobotocore_glacier/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9647 2023-08-04 12:24:17.000000 types-aiobotocore-glacier-2.5.2.post3/types_aiobotocore_glacier/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     9645 2023-08-04 12:24:16.000000 types-aiobotocore-glacier-2.5.2.post3/types_aiobotocore_glacier/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     5310 2023-08-04 12:24:16.000000 types-aiobotocore-glacier-2.5.2.post3/types_aiobotocore_glacier/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     5304 2023-08-04 12:24:16.000000 types-aiobotocore-glacier-2.5.2.post3/types_aiobotocore_glacier/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 12:24:16.000000 types-aiobotocore-glacier-2.5.2.post3/types_aiobotocore_glacier/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    42777 2023-08-04 12:24:16.000000 types-aiobotocore-glacier-2.5.2.post3/types_aiobotocore_glacier/service_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)    42659 2023-08-04 12:24:16.000000 types-aiobotocore-glacier-2.5.2.post3/types_aiobotocore_glacier/service_resource.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    38711 2023-08-04 12:24:19.000000 types-aiobotocore-glacier-2.5.2.post3/types_aiobotocore_glacier/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    38639 2023-08-04 12:24:19.000000 types-aiobotocore-glacier-2.5.2.post3/types_aiobotocore_glacier/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-04 12:24:16.000000 types-aiobotocore-glacier-2.5.2.post3/types_aiobotocore_glacier/version.py
--rw-r--r--   0 runner    (1001) docker     (123)     2483 2023-08-04 12:24:16.000000 types-aiobotocore-glacier-2.5.2.post3/types_aiobotocore_glacier/waiter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2481 2023-08-04 12:24:16.000000 types-aiobotocore-glacier-2.5.2.post3/types_aiobotocore_glacier/waiter.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:37:46.363873 types-aiobotocore-glacier-2.5.2.post3/types_aiobotocore_glacier.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    16428 2023-08-04 12:37:46.000000 types-aiobotocore-glacier-2.5.2.post3/types_aiobotocore_glacier.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      979 2023-08-04 12:37:46.000000 types-aiobotocore-glacier-2.5.2.post3/types_aiobotocore_glacier.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 12:37:46.000000 types-aiobotocore-glacier-2.5.2.post3/types_aiobotocore_glacier.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 12:37:46.000000 types-aiobotocore-glacier-2.5.2.post3/types_aiobotocore_glacier.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-04 12:37:46.000000 types-aiobotocore-glacier-2.5.2.post3/types_aiobotocore_glacier.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-08-04 12:37:46.000000 types-aiobotocore-glacier-2.5.2.post3/types_aiobotocore_glacier.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:23:46.214722 types-aiobotocore-glacier-2.5.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-08 01:11:38.000000 types-aiobotocore-glacier-2.5.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    16422 2023-08-08 01:23:46.210722 types-aiobotocore-glacier-2.5.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    14910 2023-08-08 01:11:38.000000 types-aiobotocore-glacier-2.5.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-08 01:23:46.214722 types-aiobotocore-glacier-2.5.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2066 2023-08-08 01:11:38.000000 types-aiobotocore-glacier-2.5.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:23:46.210722 types-aiobotocore-glacier-2.5.4/types_aiobotocore_glacier/
+-rw-r--r--   0 runner    (1001) docker     (123)     1735 2023-08-08 01:11:38.000000 types-aiobotocore-glacier-2.5.4/types_aiobotocore_glacier/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1733 2023-08-08 01:11:38.000000 types-aiobotocore-glacier-2.5.4/types_aiobotocore_glacier/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      931 2023-08-08 01:11:38.000000 types-aiobotocore-glacier-2.5.4/types_aiobotocore_glacier/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28395 2023-08-08 01:11:38.000000 types-aiobotocore-glacier-2.5.4/types_aiobotocore_glacier/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28347 2023-08-08 01:11:38.000000 types-aiobotocore-glacier-2.5.4/types_aiobotocore_glacier/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9742 2023-08-08 01:11:39.000000 types-aiobotocore-glacier-2.5.4/types_aiobotocore_glacier/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9740 2023-08-08 01:11:38.000000 types-aiobotocore-glacier-2.5.4/types_aiobotocore_glacier/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     5310 2023-08-08 01:11:38.000000 types-aiobotocore-glacier-2.5.4/types_aiobotocore_glacier/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5304 2023-08-08 01:11:38.000000 types-aiobotocore-glacier-2.5.4/types_aiobotocore_glacier/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 01:11:38.000000 types-aiobotocore-glacier-2.5.4/types_aiobotocore_glacier/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    42777 2023-08-08 01:11:38.000000 types-aiobotocore-glacier-2.5.4/types_aiobotocore_glacier/service_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42659 2023-08-08 01:11:38.000000 types-aiobotocore-glacier-2.5.4/types_aiobotocore_glacier/service_resource.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    38711 2023-08-08 01:11:40.000000 types-aiobotocore-glacier-2.5.4/types_aiobotocore_glacier/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38639 2023-08-08 01:11:40.000000 types-aiobotocore-glacier-2.5.4/types_aiobotocore_glacier/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-08-08 01:11:38.000000 types-aiobotocore-glacier-2.5.4/types_aiobotocore_glacier/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2483 2023-08-08 01:11:38.000000 types-aiobotocore-glacier-2.5.4/types_aiobotocore_glacier/waiter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2481 2023-08-08 01:11:38.000000 types-aiobotocore-glacier-2.5.4/types_aiobotocore_glacier/waiter.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:23:46.210722 types-aiobotocore-glacier-2.5.4/types_aiobotocore_glacier.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    16422 2023-08-08 01:23:46.000000 types-aiobotocore-glacier-2.5.4/types_aiobotocore_glacier.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      979 2023-08-08 01:23:46.000000 types-aiobotocore-glacier-2.5.4/types_aiobotocore_glacier.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 01:23:46.000000 types-aiobotocore-glacier-2.5.4/types_aiobotocore_glacier.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 01:23:46.000000 types-aiobotocore-glacier-2.5.4/types_aiobotocore_glacier.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-08 01:23:46.000000 types-aiobotocore-glacier-2.5.4/types_aiobotocore_glacier.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-08-08 01:23:46.000000 types-aiobotocore-glacier-2.5.4/types_aiobotocore_glacier.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-glacier-2.5.2.post3/LICENSE` & `types-aiobotocore-glacier-2.5.4/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-glacier-2.5.2.post3/PKG-INFO` & `types-aiobotocore-glacier-2.5.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-glacier
-Version: 2.5.2.post3
-Summary: Type annotations for aiobotocore.Glacier 2.5.2 service generated with mypy-boto3-builder 7.17.2
+Version: 2.5.4
+Summary: Type annotations for aiobotocore.Glacier 2.5.4 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_glacier/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-glacier.svg?color=blue)](https://pypi.org/project/types-aiobotocore-glacier)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_glacier/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-glacier)](https://pepy.tech/project/types-aiobotocore-glacier)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.Glacier 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glacier.html#Glacier)
+[aiobotocore.Glacier 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glacier.html#Glacier)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-glacier-2.5.2.post3/README.md` & `types-aiobotocore-glacier-2.5.4/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-glacier.svg?color=blue)](https://pypi.org/project/types-aiobotocore-glacier)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_glacier/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-glacier)](https://pepy.tech/project/types-aiobotocore-glacier)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.Glacier 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glacier.html#Glacier)
+[aiobotocore.Glacier 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glacier.html#Glacier)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-glacier-2.5.2.post3/setup.py` & `types-aiobotocore-glacier-2.5.4/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-glacier",
-    version="2.5.2.post3",
+    version="2.5.4",
     packages=["types_aiobotocore_glacier"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.Glacier 2.5.2 service generated with mypy-boto3-builder"
+        "Type annotations for aiobotocore.Glacier 2.5.4 service generated with mypy-boto3-builder"
         " 7.17.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
```

### Comparing `types-aiobotocore-glacier-2.5.2.post3/types_aiobotocore_glacier/__init__.py` & `types-aiobotocore-glacier-2.5.4/types_aiobotocore_glacier/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-glacier-2.5.2.post3/types_aiobotocore_glacier/__init__.pyi` & `types-aiobotocore-glacier-2.5.4/types_aiobotocore_glacier/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-glacier-2.5.2.post3/types_aiobotocore_glacier/__main__.py` & `types-aiobotocore-glacier-2.5.4/types_aiobotocore_glacier/__main__.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.Glacier 2.5.2\nVersion:         2.5.2.post3\nBuilder"
-        " version: 7.17.2\nDocs:           "
+        "Type annotations for aiobotocore.Glacier 2.5.4\nVersion:         2.5.4\nBuilder version:"
+        " 7.17.2\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_glacier//\nBoto3 docs:"
         "     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glacier.html#Glacier\nOther"
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

### Comparing `types-aiobotocore-glacier-2.5.2.post3/types_aiobotocore_glacier/client.py` & `types-aiobotocore-glacier-2.5.4/types_aiobotocore_glacier/client.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-glacier-2.5.2.post3/types_aiobotocore_glacier/client.pyi` & `types-aiobotocore-glacier-2.5.4/types_aiobotocore_glacier/client.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-glacier-2.5.2.post3/types_aiobotocore_glacier/literals.py` & `types-aiobotocore-glacier-2.5.4/types_aiobotocore_glacier/literals.py`

 * *Files 1% similar despite different names*

```diff
@@ -81,14 +81,15 @@
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
@@ -184,14 +185,15 @@
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
@@ -270,26 +272,28 @@
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

### Comparing `types-aiobotocore-glacier-2.5.2.post3/types_aiobotocore_glacier/literals.pyi` & `types-aiobotocore-glacier-2.5.4/types_aiobotocore_glacier/literals.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -79,14 +79,15 @@
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
@@ -182,14 +183,15 @@
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
@@ -268,26 +270,28 @@
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

### Comparing `types-aiobotocore-glacier-2.5.2.post3/types_aiobotocore_glacier/paginator.py` & `types-aiobotocore-glacier-2.5.4/types_aiobotocore_glacier/paginator.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-glacier-2.5.2.post3/types_aiobotocore_glacier/paginator.pyi` & `types-aiobotocore-glacier-2.5.4/types_aiobotocore_glacier/paginator.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-glacier-2.5.2.post3/types_aiobotocore_glacier/service_resource.py` & `types-aiobotocore-glacier-2.5.4/types_aiobotocore_glacier/service_resource.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-glacier-2.5.2.post3/types_aiobotocore_glacier/service_resource.pyi` & `types-aiobotocore-glacier-2.5.4/types_aiobotocore_glacier/service_resource.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-glacier-2.5.2.post3/types_aiobotocore_glacier/type_defs.py` & `types-aiobotocore-glacier-2.5.4/types_aiobotocore_glacier/type_defs.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-glacier-2.5.2.post3/types_aiobotocore_glacier/type_defs.pyi` & `types-aiobotocore-glacier-2.5.4/types_aiobotocore_glacier/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-glacier-2.5.2.post3/types_aiobotocore_glacier/waiter.py` & `types-aiobotocore-glacier-2.5.4/types_aiobotocore_glacier/waiter.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-glacier-2.5.2.post3/types_aiobotocore_glacier/waiter.pyi` & `types-aiobotocore-glacier-2.5.4/types_aiobotocore_glacier/waiter.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-glacier-2.5.2.post3/types_aiobotocore_glacier.egg-info/PKG-INFO` & `types-aiobotocore-glacier-2.5.4/types_aiobotocore_glacier.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-glacier
-Version: 2.5.2.post3
-Summary: Type annotations for aiobotocore.Glacier 2.5.2 service generated with mypy-boto3-builder 7.17.2
+Version: 2.5.4
+Summary: Type annotations for aiobotocore.Glacier 2.5.4 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_glacier/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-glacier.svg?color=blue)](https://pypi.org/project/types-aiobotocore-glacier)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_glacier/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-glacier)](https://pepy.tech/project/types-aiobotocore-glacier)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.Glacier 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glacier.html#Glacier)
+[aiobotocore.Glacier 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glacier.html#Glacier)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-glacier-2.5.2.post3/types_aiobotocore_glacier.egg-info/SOURCES.txt` & `types-aiobotocore-glacier-2.5.4/types_aiobotocore_glacier.egg-info/SOURCES.txt`

 * *Files identical despite different names*


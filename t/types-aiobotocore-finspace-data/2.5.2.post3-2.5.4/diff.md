# Comparing `tmp/types-aiobotocore-finspace-data-2.5.2.post3.tar.gz` & `tmp/types-aiobotocore-finspace-data-2.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-finspace-data-2.5.2.post3.tar", last modified: Fri Aug  4 12:37:43 2023, max compression
+gzip compressed data, was "types-aiobotocore-finspace-data-2.5.4.tar", last modified: Tue Aug  8 01:23:43 2023, max compression
```

## Comparing `types-aiobotocore-finspace-data-2.5.2.post3.tar` & `types-aiobotocore-finspace-data-2.5.4.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:37:43.779813 types-aiobotocore-finspace-data-2.5.2.post3/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-04 12:23:44.000000 types-aiobotocore-finspace-data-2.5.2.post3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    13824 2023-08-04 12:37:43.779813 types-aiobotocore-finspace-data-2.5.2.post3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    12283 2023-08-04 12:23:44.000000 types-aiobotocore-finspace-data-2.5.2.post3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-04 12:37:43.779813 types-aiobotocore-finspace-data-2.5.2.post3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2113 2023-08-04 12:23:44.000000 types-aiobotocore-finspace-data-2.5.2.post3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:37:43.767812 types-aiobotocore-finspace-data-2.5.2.post3/types_aiobotocore_finspace_data/
--rw-r--r--   0 runner    (1001) docker     (123)     1466 2023-08-04 12:23:44.000000 types-aiobotocore-finspace-data-2.5.2.post3/types_aiobotocore_finspace_data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1465 2023-08-04 12:23:44.000000 types-aiobotocore-finspace-data-2.5.2.post3/types_aiobotocore_finspace_data/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      965 2023-08-04 12:23:44.000000 types-aiobotocore-finspace-data-2.5.2.post3/types_aiobotocore_finspace_data/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    27152 2023-08-04 12:23:44.000000 types-aiobotocore-finspace-data-2.5.2.post3/types_aiobotocore_finspace_data/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    27107 2023-08-04 12:23:44.000000 types-aiobotocore-finspace-data-2.5.2.post3/types_aiobotocore_finspace_data/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    10078 2023-08-04 12:23:44.000000 types-aiobotocore-finspace-data-2.5.2.post3/types_aiobotocore_finspace_data/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    10076 2023-08-04 12:23:44.000000 types-aiobotocore-finspace-data-2.5.2.post3/types_aiobotocore_finspace_data/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     6452 2023-08-04 12:23:44.000000 types-aiobotocore-finspace-data-2.5.2.post3/types_aiobotocore_finspace_data/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     6445 2023-08-04 12:23:44.000000 types-aiobotocore-finspace-data-2.5.2.post3/types_aiobotocore_finspace_data/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 12:23:44.000000 types-aiobotocore-finspace-data-2.5.2.post3/types_aiobotocore_finspace_data/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    34473 2023-08-04 12:23:45.000000 types-aiobotocore-finspace-data-2.5.2.post3/types_aiobotocore_finspace_data/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    34420 2023-08-04 12:23:45.000000 types-aiobotocore-finspace-data-2.5.2.post3/types_aiobotocore_finspace_data/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-04 12:23:44.000000 types-aiobotocore-finspace-data-2.5.2.post3/types_aiobotocore_finspace_data/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:37:43.767812 types-aiobotocore-finspace-data-2.5.2.post3/types_aiobotocore_finspace_data.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    13824 2023-08-04 12:37:43.000000 types-aiobotocore-finspace-data-2.5.2.post3/types_aiobotocore_finspace_data.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      927 2023-08-04 12:37:43.000000 types-aiobotocore-finspace-data-2.5.2.post3/types_aiobotocore_finspace_data.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 12:37:43.000000 types-aiobotocore-finspace-data-2.5.2.post3/types_aiobotocore_finspace_data.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 12:37:43.000000 types-aiobotocore-finspace-data-2.5.2.post3/types_aiobotocore_finspace_data.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-04 12:37:43.000000 types-aiobotocore-finspace-data-2.5.2.post3/types_aiobotocore_finspace_data.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-08-04 12:37:43.000000 types-aiobotocore-finspace-data-2.5.2.post3/types_aiobotocore_finspace_data.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:23:43.454714 types-aiobotocore-finspace-data-2.5.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-08 01:11:09.000000 types-aiobotocore-finspace-data-2.5.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    13818 2023-08-08 01:23:43.446714 types-aiobotocore-finspace-data-2.5.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    12283 2023-08-08 01:11:09.000000 types-aiobotocore-finspace-data-2.5.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-08 01:23:43.454714 types-aiobotocore-finspace-data-2.5.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2107 2023-08-08 01:11:09.000000 types-aiobotocore-finspace-data-2.5.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:23:43.446714 types-aiobotocore-finspace-data-2.5.4/types_aiobotocore_finspace_data/
+-rw-r--r--   0 runner    (1001) docker     (123)     1466 2023-08-08 01:11:09.000000 types-aiobotocore-finspace-data-2.5.4/types_aiobotocore_finspace_data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1465 2023-08-08 01:11:09.000000 types-aiobotocore-finspace-data-2.5.4/types_aiobotocore_finspace_data/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      953 2023-08-08 01:11:09.000000 types-aiobotocore-finspace-data-2.5.4/types_aiobotocore_finspace_data/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27152 2023-08-08 01:11:09.000000 types-aiobotocore-finspace-data-2.5.4/types_aiobotocore_finspace_data/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27107 2023-08-08 01:11:09.000000 types-aiobotocore-finspace-data-2.5.4/types_aiobotocore_finspace_data/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    10173 2023-08-08 01:11:10.000000 types-aiobotocore-finspace-data-2.5.4/types_aiobotocore_finspace_data/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10171 2023-08-08 01:11:10.000000 types-aiobotocore-finspace-data-2.5.4/types_aiobotocore_finspace_data/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     6452 2023-08-08 01:11:09.000000 types-aiobotocore-finspace-data-2.5.4/types_aiobotocore_finspace_data/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6445 2023-08-08 01:11:09.000000 types-aiobotocore-finspace-data-2.5.4/types_aiobotocore_finspace_data/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 01:11:09.000000 types-aiobotocore-finspace-data-2.5.4/types_aiobotocore_finspace_data/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    34473 2023-08-08 01:11:10.000000 types-aiobotocore-finspace-data-2.5.4/types_aiobotocore_finspace_data/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34420 2023-08-08 01:11:10.000000 types-aiobotocore-finspace-data-2.5.4/types_aiobotocore_finspace_data/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-08-08 01:11:09.000000 types-aiobotocore-finspace-data-2.5.4/types_aiobotocore_finspace_data/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:23:43.446714 types-aiobotocore-finspace-data-2.5.4/types_aiobotocore_finspace_data.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    13818 2023-08-08 01:23:43.000000 types-aiobotocore-finspace-data-2.5.4/types_aiobotocore_finspace_data.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      927 2023-08-08 01:23:43.000000 types-aiobotocore-finspace-data-2.5.4/types_aiobotocore_finspace_data.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 01:23:43.000000 types-aiobotocore-finspace-data-2.5.4/types_aiobotocore_finspace_data.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 01:23:43.000000 types-aiobotocore-finspace-data-2.5.4/types_aiobotocore_finspace_data.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-08 01:23:43.000000 types-aiobotocore-finspace-data-2.5.4/types_aiobotocore_finspace_data.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-08-08 01:23:43.000000 types-aiobotocore-finspace-data-2.5.4/types_aiobotocore_finspace_data.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-finspace-data-2.5.2.post3/LICENSE` & `types-aiobotocore-finspace-data-2.5.4/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-finspace-data-2.5.2.post3/PKG-INFO` & `types-aiobotocore-finspace-data-2.5.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-finspace-data
-Version: 2.5.2.post3
-Summary: Type annotations for aiobotocore.FinSpaceData 2.5.2 service generated with mypy-boto3-builder 7.17.2
+Version: 2.5.4
+Summary: Type annotations for aiobotocore.FinSpaceData 2.5.4 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_finspace_data/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-finspace-data.svg?color=blue)](https://pypi.org/project/types-aiobotocore-finspace-data)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_finspace_data/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-finspace-data)](https://pepy.tech/project/types-aiobotocore-finspace-data)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.FinSpaceData 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/finspace-data.html#FinSpaceData)
+[aiobotocore.FinSpaceData 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/finspace-data.html#FinSpaceData)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-finspace-data-2.5.2.post3/README.md` & `types-aiobotocore-finspace-data-2.5.4/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-finspace-data.svg?color=blue)](https://pypi.org/project/types-aiobotocore-finspace-data)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_finspace_data/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-finspace-data)](https://pepy.tech/project/types-aiobotocore-finspace-data)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.FinSpaceData 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/finspace-data.html#FinSpaceData)
+[aiobotocore.FinSpaceData 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/finspace-data.html#FinSpaceData)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-finspace-data-2.5.2.post3/setup.py` & `types-aiobotocore-finspace-data-2.5.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-finspace-data",
-    version="2.5.2.post3",
+    version="2.5.4",
     packages=["types_aiobotocore_finspace_data"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.FinSpaceData 2.5.2 service generated with"
+        "Type annotations for aiobotocore.FinSpaceData 2.5.4 service generated with"
         " mypy-boto3-builder 7.17.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
```

### Comparing `types-aiobotocore-finspace-data-2.5.2.post3/types_aiobotocore_finspace_data/__init__.py` & `types-aiobotocore-finspace-data-2.5.4/types_aiobotocore_finspace_data/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-finspace-data-2.5.2.post3/types_aiobotocore_finspace_data/__init__.pyi` & `types-aiobotocore-finspace-data-2.5.4/types_aiobotocore_finspace_data/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-finspace-data-2.5.2.post3/types_aiobotocore_finspace_data/__main__.py` & `types-aiobotocore-finspace-data-2.5.4/types_aiobotocore_finspace_data/__main__.py`

 * *Files 13% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.FinSpaceData 2.5.2\nVersion:         2.5.2.post3\nBuilder"
+        "Type annotations for aiobotocore.FinSpaceData 2.5.4\nVersion:         2.5.4\nBuilder"
         " version: 7.17.2\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_finspace_data//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/finspace-data.html#FinSpaceData\nOther"
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

### Comparing `types-aiobotocore-finspace-data-2.5.2.post3/types_aiobotocore_finspace_data/client.py` & `types-aiobotocore-finspace-data-2.5.4/types_aiobotocore_finspace_data/client.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-finspace-data-2.5.2.post3/types_aiobotocore_finspace_data/client.pyi` & `types-aiobotocore-finspace-data-2.5.4/types_aiobotocore_finspace_data/client.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-finspace-data-2.5.2.post3/types_aiobotocore_finspace_data/literals.py` & `types-aiobotocore-finspace-data-2.5.4/types_aiobotocore_finspace_data/literals.py`

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

### Comparing `types-aiobotocore-finspace-data-2.5.2.post3/types_aiobotocore_finspace_data/literals.pyi` & `types-aiobotocore-finspace-data-2.5.4/types_aiobotocore_finspace_data/literals.pyi`

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

### Comparing `types-aiobotocore-finspace-data-2.5.2.post3/types_aiobotocore_finspace_data/paginator.py` & `types-aiobotocore-finspace-data-2.5.4/types_aiobotocore_finspace_data/paginator.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-finspace-data-2.5.2.post3/types_aiobotocore_finspace_data/paginator.pyi` & `types-aiobotocore-finspace-data-2.5.4/types_aiobotocore_finspace_data/paginator.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-finspace-data-2.5.2.post3/types_aiobotocore_finspace_data/type_defs.py` & `types-aiobotocore-finspace-data-2.5.4/types_aiobotocore_finspace_data/type_defs.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-finspace-data-2.5.2.post3/types_aiobotocore_finspace_data/type_defs.pyi` & `types-aiobotocore-finspace-data-2.5.4/types_aiobotocore_finspace_data/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-finspace-data-2.5.2.post3/types_aiobotocore_finspace_data.egg-info/PKG-INFO` & `types-aiobotocore-finspace-data-2.5.4/types_aiobotocore_finspace_data.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-finspace-data
-Version: 2.5.2.post3
-Summary: Type annotations for aiobotocore.FinSpaceData 2.5.2 service generated with mypy-boto3-builder 7.17.2
+Version: 2.5.4
+Summary: Type annotations for aiobotocore.FinSpaceData 2.5.4 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_finspace_data/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-finspace-data.svg?color=blue)](https://pypi.org/project/types-aiobotocore-finspace-data)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_finspace_data/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-finspace-data)](https://pepy.tech/project/types-aiobotocore-finspace-data)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.FinSpaceData 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/finspace-data.html#FinSpaceData)
+[aiobotocore.FinSpaceData 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/finspace-data.html#FinSpaceData)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-finspace-data-2.5.2.post3/types_aiobotocore_finspace_data.egg-info/SOURCES.txt` & `types-aiobotocore-finspace-data-2.5.4/types_aiobotocore_finspace_data.egg-info/SOURCES.txt`

 * *Files identical despite different names*


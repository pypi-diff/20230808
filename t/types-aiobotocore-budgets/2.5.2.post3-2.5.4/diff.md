# Comparing `tmp/types-aiobotocore-budgets-2.5.2.post3.tar.gz` & `tmp/types-aiobotocore-budgets-2.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-budgets-2.5.2.post3.tar", last modified: Fri Aug  4 12:37:21 2023, max compression
+gzip compressed data, was "types-aiobotocore-budgets-2.5.4.tar", last modified: Tue Aug  8 01:23:22 2023, max compression
```

## Comparing `types-aiobotocore-budgets-2.5.2.post3.tar` & `types-aiobotocore-budgets-2.5.4.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:37:21.591281 types-aiobotocore-budgets-2.5.2.post3/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-04 12:19:04.000000 types-aiobotocore-budgets-2.5.2.post3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    14436 2023-08-04 12:37:21.587281 types-aiobotocore-budgets-2.5.2.post3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    12918 2023-08-04 12:19:04.000000 types-aiobotocore-budgets-2.5.2.post3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-04 12:37:21.591281 types-aiobotocore-budgets-2.5.2.post3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2072 2023-08-04 12:19:04.000000 types-aiobotocore-budgets-2.5.2.post3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:37:21.583281 types-aiobotocore-budgets-2.5.2.post3/types_aiobotocore_budgets/
--rw-r--r--   0 runner    (1001) docker     (123)     2791 2023-08-04 12:19:04.000000 types-aiobotocore-budgets-2.5.2.post3/types_aiobotocore_budgets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2790 2023-08-04 12:19:04.000000 types-aiobotocore-budgets-2.5.2.post3/types_aiobotocore_budgets/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      943 2023-08-04 12:19:04.000000 types-aiobotocore-budgets-2.5.2.post3/types_aiobotocore_budgets/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    23639 2023-08-04 12:19:04.000000 types-aiobotocore-budgets-2.5.2.post3/types_aiobotocore_budgets/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    23599 2023-08-04 12:19:04.000000 types-aiobotocore-budgets-2.5.2.post3/types_aiobotocore_budgets/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    10657 2023-08-04 12:19:04.000000 types-aiobotocore-budgets-2.5.2.post3/types_aiobotocore_budgets/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    10655 2023-08-04 12:19:04.000000 types-aiobotocore-budgets-2.5.2.post3/types_aiobotocore_budgets/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    11463 2023-08-04 12:19:04.000000 types-aiobotocore-budgets-2.5.2.post3/types_aiobotocore_budgets/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)    11453 2023-08-04 12:19:04.000000 types-aiobotocore-budgets-2.5.2.post3/types_aiobotocore_budgets/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 12:19:04.000000 types-aiobotocore-budgets-2.5.2.post3/types_aiobotocore_budgets/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    31394 2023-08-04 12:19:05.000000 types-aiobotocore-budgets-2.5.2.post3/types_aiobotocore_budgets/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    31345 2023-08-04 12:19:04.000000 types-aiobotocore-budgets-2.5.2.post3/types_aiobotocore_budgets/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-04 12:19:04.000000 types-aiobotocore-budgets-2.5.2.post3/types_aiobotocore_budgets/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:37:21.587281 types-aiobotocore-budgets-2.5.2.post3/types_aiobotocore_budgets.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    14436 2023-08-04 12:37:21.000000 types-aiobotocore-budgets-2.5.2.post3/types_aiobotocore_budgets.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      813 2023-08-04 12:37:21.000000 types-aiobotocore-budgets-2.5.2.post3/types_aiobotocore_budgets.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 12:37:21.000000 types-aiobotocore-budgets-2.5.2.post3/types_aiobotocore_budgets.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 12:37:21.000000 types-aiobotocore-budgets-2.5.2.post3/types_aiobotocore_budgets.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-04 12:37:21.000000 types-aiobotocore-budgets-2.5.2.post3/types_aiobotocore_budgets.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-08-04 12:37:21.000000 types-aiobotocore-budgets-2.5.2.post3/types_aiobotocore_budgets.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:23:22.346621 types-aiobotocore-budgets-2.5.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-08 01:06:48.000000 types-aiobotocore-budgets-2.5.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    14430 2023-08-08 01:23:22.346621 types-aiobotocore-budgets-2.5.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    12918 2023-08-08 01:06:48.000000 types-aiobotocore-budgets-2.5.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-08 01:23:22.346621 types-aiobotocore-budgets-2.5.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2066 2023-08-08 01:06:48.000000 types-aiobotocore-budgets-2.5.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:23:22.346621 types-aiobotocore-budgets-2.5.4/types_aiobotocore_budgets/
+-rw-r--r--   0 runner    (1001) docker     (123)     2791 2023-08-08 01:06:48.000000 types-aiobotocore-budgets-2.5.4/types_aiobotocore_budgets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2790 2023-08-08 01:06:48.000000 types-aiobotocore-budgets-2.5.4/types_aiobotocore_budgets/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      931 2023-08-08 01:06:48.000000 types-aiobotocore-budgets-2.5.4/types_aiobotocore_budgets/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23639 2023-08-08 01:06:49.000000 types-aiobotocore-budgets-2.5.4/types_aiobotocore_budgets/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23599 2023-08-08 01:06:49.000000 types-aiobotocore-budgets-2.5.4/types_aiobotocore_budgets/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    10752 2023-08-08 01:06:50.000000 types-aiobotocore-budgets-2.5.4/types_aiobotocore_budgets/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10750 2023-08-08 01:06:49.000000 types-aiobotocore-budgets-2.5.4/types_aiobotocore_budgets/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    11463 2023-08-08 01:06:49.000000 types-aiobotocore-budgets-2.5.4/types_aiobotocore_budgets/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11453 2023-08-08 01:06:49.000000 types-aiobotocore-budgets-2.5.4/types_aiobotocore_budgets/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 01:06:48.000000 types-aiobotocore-budgets-2.5.4/types_aiobotocore_budgets/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    31394 2023-08-08 01:06:50.000000 types-aiobotocore-budgets-2.5.4/types_aiobotocore_budgets/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31345 2023-08-08 01:06:50.000000 types-aiobotocore-budgets-2.5.4/types_aiobotocore_budgets/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-08-08 01:06:48.000000 types-aiobotocore-budgets-2.5.4/types_aiobotocore_budgets/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:23:22.346621 types-aiobotocore-budgets-2.5.4/types_aiobotocore_budgets.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    14430 2023-08-08 01:23:22.000000 types-aiobotocore-budgets-2.5.4/types_aiobotocore_budgets.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      813 2023-08-08 01:23:22.000000 types-aiobotocore-budgets-2.5.4/types_aiobotocore_budgets.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 01:23:22.000000 types-aiobotocore-budgets-2.5.4/types_aiobotocore_budgets.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 01:23:22.000000 types-aiobotocore-budgets-2.5.4/types_aiobotocore_budgets.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-08 01:23:22.000000 types-aiobotocore-budgets-2.5.4/types_aiobotocore_budgets.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-08-08 01:23:22.000000 types-aiobotocore-budgets-2.5.4/types_aiobotocore_budgets.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-budgets-2.5.2.post3/LICENSE` & `types-aiobotocore-budgets-2.5.4/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-budgets-2.5.2.post3/PKG-INFO` & `types-aiobotocore-budgets-2.5.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-budgets
-Version: 2.5.2.post3
-Summary: Type annotations for aiobotocore.Budgets 2.5.2 service generated with mypy-boto3-builder 7.17.2
+Version: 2.5.4
+Summary: Type annotations for aiobotocore.Budgets 2.5.4 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_budgets/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-budgets.svg?color=blue)](https://pypi.org/project/types-aiobotocore-budgets)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_budgets/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-budgets)](https://pepy.tech/project/types-aiobotocore-budgets)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.Budgets 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/budgets.html#Budgets)
+[aiobotocore.Budgets 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/budgets.html#Budgets)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-budgets-2.5.2.post3/README.md` & `types-aiobotocore-budgets-2.5.4/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-budgets.svg?color=blue)](https://pypi.org/project/types-aiobotocore-budgets)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_budgets/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-budgets)](https://pepy.tech/project/types-aiobotocore-budgets)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.Budgets 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/budgets.html#Budgets)
+[aiobotocore.Budgets 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/budgets.html#Budgets)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-budgets-2.5.2.post3/setup.py` & `types-aiobotocore-budgets-2.5.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-budgets",
-    version="2.5.2.post3",
+    version="2.5.4",
     packages=["types_aiobotocore_budgets"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.Budgets 2.5.2 service generated with mypy-boto3-builder"
+        "Type annotations for aiobotocore.Budgets 2.5.4 service generated with mypy-boto3-builder"
         " 7.17.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
```

### Comparing `types-aiobotocore-budgets-2.5.2.post3/types_aiobotocore_budgets/__init__.py` & `types-aiobotocore-budgets-2.5.4/types_aiobotocore_budgets/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-budgets-2.5.2.post3/types_aiobotocore_budgets/__init__.pyi` & `types-aiobotocore-budgets-2.5.4/types_aiobotocore_budgets/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-budgets-2.5.2.post3/types_aiobotocore_budgets/__main__.py` & `types-aiobotocore-budgets-2.5.4/types_aiobotocore_budgets/__main__.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.Budgets 2.5.2\nVersion:         2.5.2.post3\nBuilder"
-        " version: 7.17.2\nDocs:           "
+        "Type annotations for aiobotocore.Budgets 2.5.4\nVersion:         2.5.4\nBuilder version:"
+        " 7.17.2\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_budgets//\nBoto3 docs:"
         "     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/budgets.html#Budgets\nOther"
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

### Comparing `types-aiobotocore-budgets-2.5.2.post3/types_aiobotocore_budgets/client.py` & `types-aiobotocore-budgets-2.5.4/types_aiobotocore_budgets/client.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-budgets-2.5.2.post3/types_aiobotocore_budgets/client.pyi` & `types-aiobotocore-budgets-2.5.4/types_aiobotocore_budgets/client.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-budgets-2.5.2.post3/types_aiobotocore_budgets/literals.py` & `types-aiobotocore-budgets-2.5.4/types_aiobotocore_budgets/literals.py`

 * *Files 1% similar despite different names*

```diff
@@ -107,14 +107,15 @@
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
@@ -210,14 +211,15 @@
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
@@ -296,26 +298,28 @@
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

### Comparing `types-aiobotocore-budgets-2.5.2.post3/types_aiobotocore_budgets/literals.pyi` & `types-aiobotocore-budgets-2.5.4/types_aiobotocore_budgets/literals.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -105,14 +105,15 @@
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
@@ -208,14 +209,15 @@
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
@@ -294,26 +296,28 @@
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

### Comparing `types-aiobotocore-budgets-2.5.2.post3/types_aiobotocore_budgets/paginator.py` & `types-aiobotocore-budgets-2.5.4/types_aiobotocore_budgets/paginator.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-budgets-2.5.2.post3/types_aiobotocore_budgets/paginator.pyi` & `types-aiobotocore-budgets-2.5.4/types_aiobotocore_budgets/paginator.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-budgets-2.5.2.post3/types_aiobotocore_budgets/type_defs.py` & `types-aiobotocore-budgets-2.5.4/types_aiobotocore_budgets/type_defs.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-budgets-2.5.2.post3/types_aiobotocore_budgets/type_defs.pyi` & `types-aiobotocore-budgets-2.5.4/types_aiobotocore_budgets/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-budgets-2.5.2.post3/types_aiobotocore_budgets.egg-info/PKG-INFO` & `types-aiobotocore-budgets-2.5.4/types_aiobotocore_budgets.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-budgets
-Version: 2.5.2.post3
-Summary: Type annotations for aiobotocore.Budgets 2.5.2 service generated with mypy-boto3-builder 7.17.2
+Version: 2.5.4
+Summary: Type annotations for aiobotocore.Budgets 2.5.4 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_budgets/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-budgets.svg?color=blue)](https://pypi.org/project/types-aiobotocore-budgets)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_budgets/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-budgets)](https://pepy.tech/project/types-aiobotocore-budgets)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.Budgets 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/budgets.html#Budgets)
+[aiobotocore.Budgets 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/budgets.html#Budgets)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-budgets-2.5.2.post3/types_aiobotocore_budgets.egg-info/SOURCES.txt` & `types-aiobotocore-budgets-2.5.4/types_aiobotocore_budgets.egg-info/SOURCES.txt`

 * *Files identical despite different names*


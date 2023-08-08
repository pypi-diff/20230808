# Comparing `tmp/types-aiobotocore-apprunner-2.5.2.post3.tar.gz` & `tmp/types-aiobotocore-apprunner-2.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-apprunner-2.5.2.post3.tar", last modified: Fri Aug  4 12:37:18 2023, max compression
+gzip compressed data, was "types-aiobotocore-apprunner-2.5.4.tar", last modified: Tue Aug  8 01:23:19 2023, max compression
```

## Comparing `types-aiobotocore-apprunner-2.5.2.post3.tar` & `types-aiobotocore-apprunner-2.5.4.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:37:18.835224 types-aiobotocore-apprunner-2.5.2.post3/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-04 12:18:31.000000 types-aiobotocore-apprunner-2.5.2.post3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    12368 2023-08-04 12:37:18.835224 types-aiobotocore-apprunner-2.5.2.post3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    10842 2023-08-04 12:18:31.000000 types-aiobotocore-apprunner-2.5.2.post3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-04 12:37:18.835224 types-aiobotocore-apprunner-2.5.2.post3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2086 2023-08-04 12:18:31.000000 types-aiobotocore-apprunner-2.5.2.post3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:37:18.831224 types-aiobotocore-apprunner-2.5.2.post3/types_aiobotocore_apprunner/
--rw-r--r--   0 runner    (1001) docker     (123)      458 2023-08-04 12:18:31.000000 types-aiobotocore-apprunner-2.5.2.post3/types_aiobotocore_apprunner/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      457 2023-08-04 12:18:31.000000 types-aiobotocore-apprunner-2.5.2.post3/types_aiobotocore_apprunner/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      951 2023-08-04 12:18:31.000000 types-aiobotocore-apprunner-2.5.2.post3/types_aiobotocore_apprunner/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    27528 2023-08-04 12:18:31.000000 types-aiobotocore-apprunner-2.5.2.post3/types_aiobotocore_apprunner/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    27484 2023-08-04 12:18:31.000000 types-aiobotocore-apprunner-2.5.2.post3/types_aiobotocore_apprunner/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    10078 2023-08-04 12:18:32.000000 types-aiobotocore-apprunner-2.5.2.post3/types_aiobotocore_apprunner/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    10076 2023-08-04 12:18:31.000000 types-aiobotocore-apprunner-2.5.2.post3/types_aiobotocore_apprunner/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 12:18:31.000000 types-aiobotocore-apprunner-2.5.2.post3/types_aiobotocore_apprunner/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    35599 2023-08-04 12:18:32.000000 types-aiobotocore-apprunner-2.5.2.post3/types_aiobotocore_apprunner/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    35564 2023-08-04 12:18:32.000000 types-aiobotocore-apprunner-2.5.2.post3/types_aiobotocore_apprunner/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-04 12:18:31.000000 types-aiobotocore-apprunner-2.5.2.post3/types_aiobotocore_apprunner/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:37:18.835224 types-aiobotocore-apprunner-2.5.2.post3/types_aiobotocore_apprunner.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    12368 2023-08-04 12:37:18.000000 types-aiobotocore-apprunner-2.5.2.post3/types_aiobotocore_apprunner.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      768 2023-08-04 12:37:18.000000 types-aiobotocore-apprunner-2.5.2.post3/types_aiobotocore_apprunner.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 12:37:18.000000 types-aiobotocore-apprunner-2.5.2.post3/types_aiobotocore_apprunner.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 12:37:18.000000 types-aiobotocore-apprunner-2.5.2.post3/types_aiobotocore_apprunner.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-04 12:37:18.000000 types-aiobotocore-apprunner-2.5.2.post3/types_aiobotocore_apprunner.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-08-04 12:37:18.000000 types-aiobotocore-apprunner-2.5.2.post3/types_aiobotocore_apprunner.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:23:19.346522 types-aiobotocore-apprunner-2.5.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-08 01:06:18.000000 types-aiobotocore-apprunner-2.5.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    12362 2023-08-08 01:23:19.346522 types-aiobotocore-apprunner-2.5.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10842 2023-08-08 01:06:18.000000 types-aiobotocore-apprunner-2.5.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-08 01:23:19.346522 types-aiobotocore-apprunner-2.5.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2080 2023-08-08 01:06:18.000000 types-aiobotocore-apprunner-2.5.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:23:19.346522 types-aiobotocore-apprunner-2.5.4/types_aiobotocore_apprunner/
+-rw-r--r--   0 runner    (1001) docker     (123)      458 2023-08-08 01:06:18.000000 types-aiobotocore-apprunner-2.5.4/types_aiobotocore_apprunner/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      457 2023-08-08 01:06:18.000000 types-aiobotocore-apprunner-2.5.4/types_aiobotocore_apprunner/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      939 2023-08-08 01:06:18.000000 types-aiobotocore-apprunner-2.5.4/types_aiobotocore_apprunner/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27528 2023-08-08 01:06:19.000000 types-aiobotocore-apprunner-2.5.4/types_aiobotocore_apprunner/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27484 2023-08-08 01:06:18.000000 types-aiobotocore-apprunner-2.5.4/types_aiobotocore_apprunner/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    10173 2023-08-08 01:06:19.000000 types-aiobotocore-apprunner-2.5.4/types_aiobotocore_apprunner/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10171 2023-08-08 01:06:19.000000 types-aiobotocore-apprunner-2.5.4/types_aiobotocore_apprunner/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 01:06:18.000000 types-aiobotocore-apprunner-2.5.4/types_aiobotocore_apprunner/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    35599 2023-08-08 01:06:19.000000 types-aiobotocore-apprunner-2.5.4/types_aiobotocore_apprunner/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35564 2023-08-08 01:06:19.000000 types-aiobotocore-apprunner-2.5.4/types_aiobotocore_apprunner/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-08-08 01:06:18.000000 types-aiobotocore-apprunner-2.5.4/types_aiobotocore_apprunner/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:23:19.346522 types-aiobotocore-apprunner-2.5.4/types_aiobotocore_apprunner.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    12362 2023-08-08 01:23:19.000000 types-aiobotocore-apprunner-2.5.4/types_aiobotocore_apprunner.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      768 2023-08-08 01:23:19.000000 types-aiobotocore-apprunner-2.5.4/types_aiobotocore_apprunner.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 01:23:19.000000 types-aiobotocore-apprunner-2.5.4/types_aiobotocore_apprunner.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 01:23:19.000000 types-aiobotocore-apprunner-2.5.4/types_aiobotocore_apprunner.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-08 01:23:19.000000 types-aiobotocore-apprunner-2.5.4/types_aiobotocore_apprunner.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-08-08 01:23:19.000000 types-aiobotocore-apprunner-2.5.4/types_aiobotocore_apprunner.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-apprunner-2.5.2.post3/LICENSE` & `types-aiobotocore-apprunner-2.5.4/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-apprunner-2.5.2.post3/PKG-INFO` & `types-aiobotocore-apprunner-2.5.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-apprunner
-Version: 2.5.2.post3
-Summary: Type annotations for aiobotocore.AppRunner 2.5.2 service generated with mypy-boto3-builder 7.17.2
+Version: 2.5.4
+Summary: Type annotations for aiobotocore.AppRunner 2.5.4 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_apprunner/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-apprunner.svg?color=blue)](https://pypi.org/project/types-aiobotocore-apprunner)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_apprunner/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-apprunner)](https://pepy.tech/project/types-aiobotocore-apprunner)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.AppRunner 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apprunner.html#AppRunner)
+[aiobotocore.AppRunner 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apprunner.html#AppRunner)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-apprunner-2.5.2.post3/README.md` & `types-aiobotocore-apprunner-2.5.4/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-apprunner.svg?color=blue)](https://pypi.org/project/types-aiobotocore-apprunner)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_apprunner/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-apprunner)](https://pepy.tech/project/types-aiobotocore-apprunner)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.AppRunner 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apprunner.html#AppRunner)
+[aiobotocore.AppRunner 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apprunner.html#AppRunner)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-apprunner-2.5.2.post3/setup.py` & `types-aiobotocore-apprunner-2.5.4/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-apprunner",
-    version="2.5.2.post3",
+    version="2.5.4",
     packages=["types_aiobotocore_apprunner"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.AppRunner 2.5.2 service generated with mypy-boto3-builder"
+        "Type annotations for aiobotocore.AppRunner 2.5.4 service generated with mypy-boto3-builder"
         " 7.17.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
```

### Comparing `types-aiobotocore-apprunner-2.5.2.post3/types_aiobotocore_apprunner/__main__.py` & `types-aiobotocore-apprunner-2.5.4/types_aiobotocore_apprunner/__main__.py`

 * *Files 15% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.AppRunner 2.5.2\nVersion:         2.5.2.post3\nBuilder"
-        " version: 7.17.2\nDocs:           "
+        "Type annotations for aiobotocore.AppRunner 2.5.4\nVersion:         2.5.4\nBuilder version:"
+        " 7.17.2\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_apprunner//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apprunner.html#AppRunner\nOther"
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

### Comparing `types-aiobotocore-apprunner-2.5.2.post3/types_aiobotocore_apprunner/client.py` & `types-aiobotocore-apprunner-2.5.4/types_aiobotocore_apprunner/client.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-apprunner-2.5.2.post3/types_aiobotocore_apprunner/client.pyi` & `types-aiobotocore-apprunner-2.5.4/types_aiobotocore_apprunner/client.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-apprunner-2.5.2.post3/types_aiobotocore_apprunner/literals.py` & `types-aiobotocore-apprunner-2.5.4/types_aiobotocore_apprunner/literals.py`

 * *Files 1% similar despite different names*

```diff
@@ -120,14 +120,15 @@
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
@@ -223,14 +224,15 @@
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
@@ -309,26 +311,28 @@
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

### Comparing `types-aiobotocore-apprunner-2.5.2.post3/types_aiobotocore_apprunner/literals.pyi` & `types-aiobotocore-apprunner-2.5.4/types_aiobotocore_apprunner/literals.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -118,14 +118,15 @@
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
@@ -221,14 +222,15 @@
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
@@ -307,26 +309,28 @@
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

### Comparing `types-aiobotocore-apprunner-2.5.2.post3/types_aiobotocore_apprunner/type_defs.py` & `types-aiobotocore-apprunner-2.5.4/types_aiobotocore_apprunner/type_defs.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-apprunner-2.5.2.post3/types_aiobotocore_apprunner/type_defs.pyi` & `types-aiobotocore-apprunner-2.5.4/types_aiobotocore_apprunner/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-apprunner-2.5.2.post3/types_aiobotocore_apprunner.egg-info/PKG-INFO` & `types-aiobotocore-apprunner-2.5.4/types_aiobotocore_apprunner.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-apprunner
-Version: 2.5.2.post3
-Summary: Type annotations for aiobotocore.AppRunner 2.5.2 service generated with mypy-boto3-builder 7.17.2
+Version: 2.5.4
+Summary: Type annotations for aiobotocore.AppRunner 2.5.4 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_apprunner/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-apprunner.svg?color=blue)](https://pypi.org/project/types-aiobotocore-apprunner)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_apprunner/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-apprunner)](https://pepy.tech/project/types-aiobotocore-apprunner)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.AppRunner 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apprunner.html#AppRunner)
+[aiobotocore.AppRunner 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apprunner.html#AppRunner)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-apprunner-2.5.2.post3/types_aiobotocore_apprunner.egg-info/SOURCES.txt` & `types-aiobotocore-apprunner-2.5.4/types_aiobotocore_apprunner.egg-info/SOURCES.txt`

 * *Files identical despite different names*


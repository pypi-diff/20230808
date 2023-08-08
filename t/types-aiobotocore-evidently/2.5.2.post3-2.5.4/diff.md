# Comparing `tmp/types-aiobotocore-evidently-2.5.2.post3.tar.gz` & `tmp/types-aiobotocore-evidently-2.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-evidently-2.5.2.post3.tar", last modified: Fri Aug  4 12:37:43 2023, max compression
+gzip compressed data, was "types-aiobotocore-evidently-2.5.4.tar", last modified: Tue Aug  8 01:23:43 2023, max compression
```

## Comparing `types-aiobotocore-evidently-2.5.2.post3.tar` & `types-aiobotocore-evidently-2.5.4.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:37:43.659810 types-aiobotocore-evidently-2.5.2.post3/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-04 12:23:39.000000 types-aiobotocore-evidently-2.5.2.post3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    13798 2023-08-04 12:37:43.659810 types-aiobotocore-evidently-2.5.2.post3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    12262 2023-08-04 12:23:39.000000 types-aiobotocore-evidently-2.5.2.post3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-04 12:37:43.659810 types-aiobotocore-evidently-2.5.2.post3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2096 2023-08-04 12:23:39.000000 types-aiobotocore-evidently-2.5.2.post3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:37:43.659810 types-aiobotocore-evidently-2.5.2.post3/types_aiobotocore_evidently/
--rw-r--r--   0 runner    (1001) docker     (123)     1689 2023-08-04 12:23:39.000000 types-aiobotocore-evidently-2.5.2.post3/types_aiobotocore_evidently/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1688 2023-08-04 12:23:39.000000 types-aiobotocore-evidently-2.5.2.post3/types_aiobotocore_evidently/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      971 2023-08-04 12:23:39.000000 types-aiobotocore-evidently-2.5.2.post3/types_aiobotocore_evidently/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    32446 2023-08-04 12:23:39.000000 types-aiobotocore-evidently-2.5.2.post3/types_aiobotocore_evidently/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    32393 2023-08-04 12:23:39.000000 types-aiobotocore-evidently-2.5.2.post3/types_aiobotocore_evidently/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    10279 2023-08-04 12:23:40.000000 types-aiobotocore-evidently-2.5.2.post3/types_aiobotocore_evidently/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    10277 2023-08-04 12:23:40.000000 types-aiobotocore-evidently-2.5.2.post3/types_aiobotocore_evidently/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     7871 2023-08-04 12:23:39.000000 types-aiobotocore-evidently-2.5.2.post3/types_aiobotocore_evidently/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     7863 2023-08-04 12:23:39.000000 types-aiobotocore-evidently-2.5.2.post3/types_aiobotocore_evidently/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 12:23:39.000000 types-aiobotocore-evidently-2.5.2.post3/types_aiobotocore_evidently/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    45515 2023-08-04 12:23:42.000000 types-aiobotocore-evidently-2.5.2.post3/types_aiobotocore_evidently/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    45430 2023-08-04 12:23:42.000000 types-aiobotocore-evidently-2.5.2.post3/types_aiobotocore_evidently/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-04 12:23:39.000000 types-aiobotocore-evidently-2.5.2.post3/types_aiobotocore_evidently/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:37:43.659810 types-aiobotocore-evidently-2.5.2.post3/types_aiobotocore_evidently.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    13798 2023-08-04 12:37:43.000000 types-aiobotocore-evidently-2.5.2.post3/types_aiobotocore_evidently.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      851 2023-08-04 12:37:43.000000 types-aiobotocore-evidently-2.5.2.post3/types_aiobotocore_evidently.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 12:37:43.000000 types-aiobotocore-evidently-2.5.2.post3/types_aiobotocore_evidently.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 12:37:43.000000 types-aiobotocore-evidently-2.5.2.post3/types_aiobotocore_evidently.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-04 12:37:43.000000 types-aiobotocore-evidently-2.5.2.post3/types_aiobotocore_evidently.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-08-04 12:37:43.000000 types-aiobotocore-evidently-2.5.2.post3/types_aiobotocore_evidently.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:23:43.370714 types-aiobotocore-evidently-2.5.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-08 01:11:05.000000 types-aiobotocore-evidently-2.5.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    13792 2023-08-08 01:23:43.370714 types-aiobotocore-evidently-2.5.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    12262 2023-08-08 01:11:05.000000 types-aiobotocore-evidently-2.5.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-08 01:23:43.370714 types-aiobotocore-evidently-2.5.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2090 2023-08-08 01:11:05.000000 types-aiobotocore-evidently-2.5.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:23:43.370714 types-aiobotocore-evidently-2.5.4/types_aiobotocore_evidently/
+-rw-r--r--   0 runner    (1001) docker     (123)     1689 2023-08-08 01:11:05.000000 types-aiobotocore-evidently-2.5.4/types_aiobotocore_evidently/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1688 2023-08-08 01:11:05.000000 types-aiobotocore-evidently-2.5.4/types_aiobotocore_evidently/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      959 2023-08-08 01:11:05.000000 types-aiobotocore-evidently-2.5.4/types_aiobotocore_evidently/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32446 2023-08-08 01:11:05.000000 types-aiobotocore-evidently-2.5.4/types_aiobotocore_evidently/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32393 2023-08-08 01:11:05.000000 types-aiobotocore-evidently-2.5.4/types_aiobotocore_evidently/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    10374 2023-08-08 01:11:05.000000 types-aiobotocore-evidently-2.5.4/types_aiobotocore_evidently/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10372 2023-08-08 01:11:05.000000 types-aiobotocore-evidently-2.5.4/types_aiobotocore_evidently/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     7871 2023-08-08 01:11:05.000000 types-aiobotocore-evidently-2.5.4/types_aiobotocore_evidently/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7863 2023-08-08 01:11:05.000000 types-aiobotocore-evidently-2.5.4/types_aiobotocore_evidently/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 01:11:05.000000 types-aiobotocore-evidently-2.5.4/types_aiobotocore_evidently/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    45515 2023-08-08 01:11:07.000000 types-aiobotocore-evidently-2.5.4/types_aiobotocore_evidently/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    45430 2023-08-08 01:11:07.000000 types-aiobotocore-evidently-2.5.4/types_aiobotocore_evidently/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-08-08 01:11:05.000000 types-aiobotocore-evidently-2.5.4/types_aiobotocore_evidently/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:23:43.370714 types-aiobotocore-evidently-2.5.4/types_aiobotocore_evidently.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    13792 2023-08-08 01:23:43.000000 types-aiobotocore-evidently-2.5.4/types_aiobotocore_evidently.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      851 2023-08-08 01:23:43.000000 types-aiobotocore-evidently-2.5.4/types_aiobotocore_evidently.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 01:23:43.000000 types-aiobotocore-evidently-2.5.4/types_aiobotocore_evidently.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 01:23:43.000000 types-aiobotocore-evidently-2.5.4/types_aiobotocore_evidently.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-08 01:23:43.000000 types-aiobotocore-evidently-2.5.4/types_aiobotocore_evidently.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-08-08 01:23:43.000000 types-aiobotocore-evidently-2.5.4/types_aiobotocore_evidently.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-evidently-2.5.2.post3/LICENSE` & `types-aiobotocore-evidently-2.5.4/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-evidently-2.5.2.post3/PKG-INFO` & `types-aiobotocore-evidently-2.5.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-evidently
-Version: 2.5.2.post3
-Summary: Type annotations for aiobotocore.CloudWatchEvidently 2.5.2 service generated with mypy-boto3-builder 7.17.2
+Version: 2.5.4
+Summary: Type annotations for aiobotocore.CloudWatchEvidently 2.5.4 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_evidently/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-evidently.svg?color=blue)](https://pypi.org/project/types-aiobotocore-evidently)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_evidently/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-evidently)](https://pepy.tech/project/types-aiobotocore-evidently)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.CloudWatchEvidently 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/evidently.html#CloudWatchEvidently)
+[aiobotocore.CloudWatchEvidently 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/evidently.html#CloudWatchEvidently)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-evidently-2.5.2.post3/README.md` & `types-aiobotocore-evidently-2.5.4/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-evidently.svg?color=blue)](https://pypi.org/project/types-aiobotocore-evidently)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_evidently/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-evidently)](https://pepy.tech/project/types-aiobotocore-evidently)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.CloudWatchEvidently 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/evidently.html#CloudWatchEvidently)
+[aiobotocore.CloudWatchEvidently 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/evidently.html#CloudWatchEvidently)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-evidently-2.5.2.post3/setup.py` & `types-aiobotocore-evidently-2.5.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-evidently",
-    version="2.5.2.post3",
+    version="2.5.4",
     packages=["types_aiobotocore_evidently"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.CloudWatchEvidently 2.5.2 service generated with"
+        "Type annotations for aiobotocore.CloudWatchEvidently 2.5.4 service generated with"
         " mypy-boto3-builder 7.17.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
```

### Comparing `types-aiobotocore-evidently-2.5.2.post3/types_aiobotocore_evidently/__init__.py` & `types-aiobotocore-evidently-2.5.4/types_aiobotocore_evidently/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-evidently-2.5.2.post3/types_aiobotocore_evidently/__init__.pyi` & `types-aiobotocore-evidently-2.5.4/types_aiobotocore_evidently/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-evidently-2.5.2.post3/types_aiobotocore_evidently/__main__.py` & `types-aiobotocore-evidently-2.5.4/types_aiobotocore_evidently/__main__.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.CloudWatchEvidently 2.5.2\nVersion:        "
-        " 2.5.2.post3\nBuilder version: 7.17.2\nDocs:           "
+        "Type annotations for aiobotocore.CloudWatchEvidently 2.5.4\nVersion:        "
+        " 2.5.4\nBuilder version: 7.17.2\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_evidently//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/evidently.html#CloudWatchEvidently\nOther"
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

### Comparing `types-aiobotocore-evidently-2.5.2.post3/types_aiobotocore_evidently/client.py` & `types-aiobotocore-evidently-2.5.4/types_aiobotocore_evidently/client.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-evidently-2.5.2.post3/types_aiobotocore_evidently/client.pyi` & `types-aiobotocore-evidently-2.5.4/types_aiobotocore_evidently/client.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-evidently-2.5.2.post3/types_aiobotocore_evidently/literals.py` & `types-aiobotocore-evidently-2.5.4/types_aiobotocore_evidently/literals.py`

 * *Files 2% similar despite different names*

```diff
@@ -94,14 +94,15 @@
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
@@ -197,14 +198,15 @@
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
@@ -283,26 +285,28 @@
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

### Comparing `types-aiobotocore-evidently-2.5.2.post3/types_aiobotocore_evidently/literals.pyi` & `types-aiobotocore-evidently-2.5.4/types_aiobotocore_evidently/literals.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -92,14 +92,15 @@
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
@@ -195,14 +196,15 @@
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
@@ -281,26 +283,28 @@
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

### Comparing `types-aiobotocore-evidently-2.5.2.post3/types_aiobotocore_evidently/paginator.py` & `types-aiobotocore-evidently-2.5.4/types_aiobotocore_evidently/paginator.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-evidently-2.5.2.post3/types_aiobotocore_evidently/paginator.pyi` & `types-aiobotocore-evidently-2.5.4/types_aiobotocore_evidently/paginator.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-evidently-2.5.2.post3/types_aiobotocore_evidently/type_defs.py` & `types-aiobotocore-evidently-2.5.4/types_aiobotocore_evidently/type_defs.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-evidently-2.5.2.post3/types_aiobotocore_evidently/type_defs.pyi` & `types-aiobotocore-evidently-2.5.4/types_aiobotocore_evidently/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-evidently-2.5.2.post3/types_aiobotocore_evidently.egg-info/PKG-INFO` & `types-aiobotocore-evidently-2.5.4/types_aiobotocore_evidently.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-evidently
-Version: 2.5.2.post3
-Summary: Type annotations for aiobotocore.CloudWatchEvidently 2.5.2 service generated with mypy-boto3-builder 7.17.2
+Version: 2.5.4
+Summary: Type annotations for aiobotocore.CloudWatchEvidently 2.5.4 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_evidently/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-evidently.svg?color=blue)](https://pypi.org/project/types-aiobotocore-evidently)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_evidently/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-evidently)](https://pepy.tech/project/types-aiobotocore-evidently)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.CloudWatchEvidently 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/evidently.html#CloudWatchEvidently)
+[aiobotocore.CloudWatchEvidently 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/evidently.html#CloudWatchEvidently)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-evidently-2.5.2.post3/types_aiobotocore_evidently.egg-info/SOURCES.txt` & `types-aiobotocore-evidently-2.5.4/types_aiobotocore_evidently.egg-info/SOURCES.txt`

 * *Files identical despite different names*


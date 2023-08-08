# Comparing `tmp/types-aiobotocore-frauddetector-2.5.2.post3.tar.gz` & `tmp/types-aiobotocore-frauddetector-2.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-frauddetector-2.5.2.post3.tar", last modified: Fri Aug  4 12:37:44 2023, max compression
+gzip compressed data, was "types-aiobotocore-frauddetector-2.5.4.tar", last modified: Tue Aug  8 01:23:45 2023, max compression
```

## Comparing `types-aiobotocore-frauddetector-2.5.2.post3.tar` & `types-aiobotocore-frauddetector-2.5.4.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:37:44.579831 types-aiobotocore-frauddetector-2.5.2.post3/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-04 12:23:59.000000 types-aiobotocore-frauddetector-2.5.2.post3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    12514 2023-08-04 12:37:44.579831 types-aiobotocore-frauddetector-2.5.2.post3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    10972 2023-08-04 12:23:59.000000 types-aiobotocore-frauddetector-2.5.2.post3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-04 12:37:44.579831 types-aiobotocore-frauddetector-2.5.2.post3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2114 2023-08-04 12:23:59.000000 types-aiobotocore-frauddetector-2.5.2.post3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:37:44.563831 types-aiobotocore-frauddetector-2.5.2.post3/types_aiobotocore_frauddetector/
--rw-r--r--   0 runner    (1001) docker     (123)      490 2023-08-04 12:23:59.000000 types-aiobotocore-frauddetector-2.5.2.post3/types_aiobotocore_frauddetector/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      489 2023-08-04 12:23:59.000000 types-aiobotocore-frauddetector-2.5.2.post3/types_aiobotocore_frauddetector/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      967 2023-08-04 12:23:59.000000 types-aiobotocore-frauddetector-2.5.2.post3/types_aiobotocore_frauddetector/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    49150 2023-08-04 12:23:59.000000 types-aiobotocore-frauddetector-2.5.2.post3/types_aiobotocore_frauddetector/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    49068 2023-08-04 12:23:59.000000 types-aiobotocore-frauddetector-2.5.2.post3/types_aiobotocore_frauddetector/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9317 2023-08-04 12:23:59.000000 types-aiobotocore-frauddetector-2.5.2.post3/types_aiobotocore_frauddetector/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     9315 2023-08-04 12:23:59.000000 types-aiobotocore-frauddetector-2.5.2.post3/types_aiobotocore_frauddetector/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 12:23:59.000000 types-aiobotocore-frauddetector-2.5.2.post3/types_aiobotocore_frauddetector/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    59400 2023-08-04 12:24:01.000000 types-aiobotocore-frauddetector-2.5.2.post3/types_aiobotocore_frauddetector/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    59333 2023-08-04 12:24:00.000000 types-aiobotocore-frauddetector-2.5.2.post3/types_aiobotocore_frauddetector/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-04 12:23:59.000000 types-aiobotocore-frauddetector-2.5.2.post3/types_aiobotocore_frauddetector/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:37:44.579831 types-aiobotocore-frauddetector-2.5.2.post3/types_aiobotocore_frauddetector.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    12514 2023-08-04 12:37:44.000000 types-aiobotocore-frauddetector-2.5.2.post3/types_aiobotocore_frauddetector.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      836 2023-08-04 12:37:44.000000 types-aiobotocore-frauddetector-2.5.2.post3/types_aiobotocore_frauddetector.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 12:37:44.000000 types-aiobotocore-frauddetector-2.5.2.post3/types_aiobotocore_frauddetector.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 12:37:44.000000 types-aiobotocore-frauddetector-2.5.2.post3/types_aiobotocore_frauddetector.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-04 12:37:44.000000 types-aiobotocore-frauddetector-2.5.2.post3/types_aiobotocore_frauddetector.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-08-04 12:37:44.000000 types-aiobotocore-frauddetector-2.5.2.post3/types_aiobotocore_frauddetector.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:23:45.634720 types-aiobotocore-frauddetector-2.5.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-08 01:11:23.000000 types-aiobotocore-frauddetector-2.5.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    12508 2023-08-08 01:23:45.634720 types-aiobotocore-frauddetector-2.5.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10972 2023-08-08 01:11:23.000000 types-aiobotocore-frauddetector-2.5.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-08 01:23:45.634720 types-aiobotocore-frauddetector-2.5.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2108 2023-08-08 01:11:22.000000 types-aiobotocore-frauddetector-2.5.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:23:45.634720 types-aiobotocore-frauddetector-2.5.4/types_aiobotocore_frauddetector/
+-rw-r--r--   0 runner    (1001) docker     (123)      490 2023-08-08 01:11:23.000000 types-aiobotocore-frauddetector-2.5.4/types_aiobotocore_frauddetector/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      489 2023-08-08 01:11:23.000000 types-aiobotocore-frauddetector-2.5.4/types_aiobotocore_frauddetector/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      955 2023-08-08 01:11:23.000000 types-aiobotocore-frauddetector-2.5.4/types_aiobotocore_frauddetector/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    49150 2023-08-08 01:11:23.000000 types-aiobotocore-frauddetector-2.5.4/types_aiobotocore_frauddetector/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    49068 2023-08-08 01:11:23.000000 types-aiobotocore-frauddetector-2.5.4/types_aiobotocore_frauddetector/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9412 2023-08-08 01:11:23.000000 types-aiobotocore-frauddetector-2.5.4/types_aiobotocore_frauddetector/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9410 2023-08-08 01:11:23.000000 types-aiobotocore-frauddetector-2.5.4/types_aiobotocore_frauddetector/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 01:11:23.000000 types-aiobotocore-frauddetector-2.5.4/types_aiobotocore_frauddetector/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    59400 2023-08-08 01:11:24.000000 types-aiobotocore-frauddetector-2.5.4/types_aiobotocore_frauddetector/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    59333 2023-08-08 01:11:24.000000 types-aiobotocore-frauddetector-2.5.4/types_aiobotocore_frauddetector/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-08-08 01:11:23.000000 types-aiobotocore-frauddetector-2.5.4/types_aiobotocore_frauddetector/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:23:45.634720 types-aiobotocore-frauddetector-2.5.4/types_aiobotocore_frauddetector.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    12508 2023-08-08 01:23:45.000000 types-aiobotocore-frauddetector-2.5.4/types_aiobotocore_frauddetector.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      836 2023-08-08 01:23:45.000000 types-aiobotocore-frauddetector-2.5.4/types_aiobotocore_frauddetector.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 01:23:45.000000 types-aiobotocore-frauddetector-2.5.4/types_aiobotocore_frauddetector.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 01:23:45.000000 types-aiobotocore-frauddetector-2.5.4/types_aiobotocore_frauddetector.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-08 01:23:45.000000 types-aiobotocore-frauddetector-2.5.4/types_aiobotocore_frauddetector.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-08-08 01:23:45.000000 types-aiobotocore-frauddetector-2.5.4/types_aiobotocore_frauddetector.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-frauddetector-2.5.2.post3/LICENSE` & `types-aiobotocore-frauddetector-2.5.4/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-frauddetector-2.5.2.post3/PKG-INFO` & `types-aiobotocore-frauddetector-2.5.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-frauddetector
-Version: 2.5.2.post3
-Summary: Type annotations for aiobotocore.FraudDetector 2.5.2 service generated with mypy-boto3-builder 7.17.2
+Version: 2.5.4
+Summary: Type annotations for aiobotocore.FraudDetector 2.5.4 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_frauddetector/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-frauddetector.svg?color=blue)](https://pypi.org/project/types-aiobotocore-frauddetector)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_frauddetector/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-frauddetector)](https://pepy.tech/project/types-aiobotocore-frauddetector)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.FraudDetector 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/frauddetector.html#FraudDetector)
+[aiobotocore.FraudDetector 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/frauddetector.html#FraudDetector)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-frauddetector-2.5.2.post3/README.md` & `types-aiobotocore-frauddetector-2.5.4/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-frauddetector.svg?color=blue)](https://pypi.org/project/types-aiobotocore-frauddetector)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_frauddetector/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-frauddetector)](https://pepy.tech/project/types-aiobotocore-frauddetector)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.FraudDetector 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/frauddetector.html#FraudDetector)
+[aiobotocore.FraudDetector 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/frauddetector.html#FraudDetector)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-frauddetector-2.5.2.post3/setup.py` & `types-aiobotocore-frauddetector-2.5.4/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-frauddetector",
-    version="2.5.2.post3",
+    version="2.5.4",
     packages=["types_aiobotocore_frauddetector"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.FraudDetector 2.5.2 service generated with"
+        "Type annotations for aiobotocore.FraudDetector 2.5.4 service generated with"
         " mypy-boto3-builder 7.17.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
```

### Comparing `types-aiobotocore-frauddetector-2.5.2.post3/types_aiobotocore_frauddetector/__main__.py` & `types-aiobotocore-frauddetector-2.5.4/types_aiobotocore_frauddetector/__main__.py`

 * *Files 15% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.FraudDetector 2.5.2\nVersion:        "
-        " 2.5.2.post3\nBuilder version: 7.17.2\nDocs:           "
+        "Type annotations for aiobotocore.FraudDetector 2.5.4\nVersion:         2.5.4\nBuilder"
+        " version: 7.17.2\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_frauddetector//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/frauddetector.html#FraudDetector\nOther"
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

### Comparing `types-aiobotocore-frauddetector-2.5.2.post3/types_aiobotocore_frauddetector/client.py` & `types-aiobotocore-frauddetector-2.5.4/types_aiobotocore_frauddetector/client.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-frauddetector-2.5.2.post3/types_aiobotocore_frauddetector/client.pyi` & `types-aiobotocore-frauddetector-2.5.4/types_aiobotocore_frauddetector/client.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-frauddetector-2.5.2.post3/types_aiobotocore_frauddetector/literals.py` & `types-aiobotocore-frauddetector-2.5.4/types_aiobotocore_frauddetector/literals.py`

 * *Files 0% similar despite different names*

```diff
@@ -80,14 +80,15 @@
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
@@ -183,14 +184,15 @@
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
@@ -269,26 +271,28 @@
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

### Comparing `types-aiobotocore-frauddetector-2.5.2.post3/types_aiobotocore_frauddetector/literals.pyi` & `types-aiobotocore-frauddetector-2.5.4/types_aiobotocore_frauddetector/literals.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -78,14 +78,15 @@
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
@@ -181,14 +182,15 @@
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
@@ -267,26 +269,28 @@
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

### Comparing `types-aiobotocore-frauddetector-2.5.2.post3/types_aiobotocore_frauddetector/type_defs.py` & `types-aiobotocore-frauddetector-2.5.4/types_aiobotocore_frauddetector/type_defs.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-frauddetector-2.5.2.post3/types_aiobotocore_frauddetector/type_defs.pyi` & `types-aiobotocore-frauddetector-2.5.4/types_aiobotocore_frauddetector/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-frauddetector-2.5.2.post3/types_aiobotocore_frauddetector.egg-info/PKG-INFO` & `types-aiobotocore-frauddetector-2.5.4/types_aiobotocore_frauddetector.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-frauddetector
-Version: 2.5.2.post3
-Summary: Type annotations for aiobotocore.FraudDetector 2.5.2 service generated with mypy-boto3-builder 7.17.2
+Version: 2.5.4
+Summary: Type annotations for aiobotocore.FraudDetector 2.5.4 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_frauddetector/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-frauddetector.svg?color=blue)](https://pypi.org/project/types-aiobotocore-frauddetector)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_frauddetector/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-frauddetector)](https://pepy.tech/project/types-aiobotocore-frauddetector)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.FraudDetector 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/frauddetector.html#FraudDetector)
+[aiobotocore.FraudDetector 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/frauddetector.html#FraudDetector)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-frauddetector-2.5.2.post3/types_aiobotocore_frauddetector.egg-info/SOURCES.txt` & `types-aiobotocore-frauddetector-2.5.4/types_aiobotocore_frauddetector.egg-info/SOURCES.txt`

 * *Files identical despite different names*


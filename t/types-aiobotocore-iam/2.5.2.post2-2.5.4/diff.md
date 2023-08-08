# Comparing `tmp/types-aiobotocore-iam-2.5.2.post2.tar.gz` & `tmp/types-aiobotocore-iam-2.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-iam-2.5.2.post2.tar", last modified: Fri Aug  4 12:37:49 2023, max compression
+gzip compressed data, was "types-aiobotocore-iam-2.5.4.tar", last modified: Tue Aug  8 01:23:48 2023, max compression
```

## Comparing `types-aiobotocore-iam-2.5.2.post2.tar` & `types-aiobotocore-iam-2.5.4.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:37:49.119938 types-aiobotocore-iam-2.5.2.post2/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-04 12:24:58.000000 types-aiobotocore-iam-2.5.2.post2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    23510 2023-08-04 12:37:49.119938 types-aiobotocore-iam-2.5.2.post2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    22008 2023-08-04 12:24:58.000000 types-aiobotocore-iam-2.5.2.post2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-04 12:37:49.119938 types-aiobotocore-iam-2.5.2.post2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2020 2023-08-04 12:24:58.000000 types-aiobotocore-iam-2.5.2.post2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:37:49.099937 types-aiobotocore-iam-2.5.2.post2/types_aiobotocore_iam/
--rw-r--r--   0 runner    (1001) docker     (123)     8794 2023-08-04 12:24:58.000000 types-aiobotocore-iam-2.5.2.post2/types_aiobotocore_iam/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8792 2023-08-04 12:24:58.000000 types-aiobotocore-iam-2.5.2.post2/types_aiobotocore_iam/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      916 2023-08-04 12:24:58.000000 types-aiobotocore-iam-2.5.2.post2/types_aiobotocore_iam/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)   119024 2023-08-04 12:24:59.000000 types-aiobotocore-iam-2.5.2.post2/types_aiobotocore_iam/client.py
--rw-r--r--   0 runner    (1001) docker     (123)   118818 2023-08-04 12:24:59.000000 types-aiobotocore-iam-2.5.2.post2/types_aiobotocore_iam/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    15545 2023-08-04 12:25:02.000000 types-aiobotocore-iam-2.5.2.post2/types_aiobotocore_iam/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    15543 2023-08-04 12:25:02.000000 types-aiobotocore-iam-2.5.2.post2/types_aiobotocore_iam/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    40084 2023-08-04 12:25:02.000000 types-aiobotocore-iam-2.5.2.post2/types_aiobotocore_iam/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)    40048 2023-08-04 12:25:02.000000 types-aiobotocore-iam-2.5.2.post2/types_aiobotocore_iam/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 12:24:58.000000 types-aiobotocore-iam-2.5.2.post2/types_aiobotocore_iam/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)   154916 2023-08-04 12:25:02.000000 types-aiobotocore-iam-2.5.2.post2/types_aiobotocore_iam/service_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)   154535 2023-08-04 12:25:00.000000 types-aiobotocore-iam-2.5.2.post2/types_aiobotocore_iam/service_resource.pyi
--rw-r--r--   0 runner    (1001) docker     (123)   146322 2023-08-04 12:25:05.000000 types-aiobotocore-iam-2.5.2.post2/types_aiobotocore_iam/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)   146107 2023-08-04 12:25:04.000000 types-aiobotocore-iam-2.5.2.post2/types_aiobotocore_iam/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-04 12:24:58.000000 types-aiobotocore-iam-2.5.2.post2/types_aiobotocore_iam/version.py
--rw-r--r--   0 runner    (1001) docker     (123)     4212 2023-08-04 12:25:02.000000 types-aiobotocore-iam-2.5.2.post2/types_aiobotocore_iam/waiter.py
--rw-r--r--   0 runner    (1001) docker     (123)     4208 2023-08-04 12:25:02.000000 types-aiobotocore-iam-2.5.2.post2/types_aiobotocore_iam/waiter.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:37:49.119938 types-aiobotocore-iam-2.5.2.post2/types_aiobotocore_iam.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    23510 2023-08-04 12:37:48.000000 types-aiobotocore-iam-2.5.2.post2/types_aiobotocore_iam.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      887 2023-08-04 12:37:48.000000 types-aiobotocore-iam-2.5.2.post2/types_aiobotocore_iam.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 12:37:48.000000 types-aiobotocore-iam-2.5.2.post2/types_aiobotocore_iam.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 12:37:48.000000 types-aiobotocore-iam-2.5.2.post2/types_aiobotocore_iam.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-04 12:37:48.000000 types-aiobotocore-iam-2.5.2.post2/types_aiobotocore_iam.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-08-04 12:37:48.000000 types-aiobotocore-iam-2.5.2.post2/types_aiobotocore_iam.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:23:48.794729 types-aiobotocore-iam-2.5.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-08 01:12:16.000000 types-aiobotocore-iam-2.5.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    23504 2023-08-08 01:23:48.786729 types-aiobotocore-iam-2.5.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    22008 2023-08-08 01:12:16.000000 types-aiobotocore-iam-2.5.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-08 01:23:48.794729 types-aiobotocore-iam-2.5.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2014 2023-08-08 01:12:16.000000 types-aiobotocore-iam-2.5.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:23:48.782729 types-aiobotocore-iam-2.5.4/types_aiobotocore_iam/
+-rw-r--r--   0 runner    (1001) docker     (123)     8794 2023-08-08 01:12:16.000000 types-aiobotocore-iam-2.5.4/types_aiobotocore_iam/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8792 2023-08-08 01:12:16.000000 types-aiobotocore-iam-2.5.4/types_aiobotocore_iam/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      904 2023-08-08 01:12:16.000000 types-aiobotocore-iam-2.5.4/types_aiobotocore_iam/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   119024 2023-08-08 01:12:17.000000 types-aiobotocore-iam-2.5.4/types_aiobotocore_iam/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)   118818 2023-08-08 01:12:17.000000 types-aiobotocore-iam-2.5.4/types_aiobotocore_iam/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    15640 2023-08-08 01:12:20.000000 types-aiobotocore-iam-2.5.4/types_aiobotocore_iam/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15638 2023-08-08 01:12:20.000000 types-aiobotocore-iam-2.5.4/types_aiobotocore_iam/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    40084 2023-08-08 01:12:19.000000 types-aiobotocore-iam-2.5.4/types_aiobotocore_iam/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40048 2023-08-08 01:12:19.000000 types-aiobotocore-iam-2.5.4/types_aiobotocore_iam/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 01:12:16.000000 types-aiobotocore-iam-2.5.4/types_aiobotocore_iam/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)   154916 2023-08-08 01:12:19.000000 types-aiobotocore-iam-2.5.4/types_aiobotocore_iam/service_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)   154535 2023-08-08 01:12:17.000000 types-aiobotocore-iam-2.5.4/types_aiobotocore_iam/service_resource.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)   146322 2023-08-08 01:12:22.000000 types-aiobotocore-iam-2.5.4/types_aiobotocore_iam/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)   146107 2023-08-08 01:12:21.000000 types-aiobotocore-iam-2.5.4/types_aiobotocore_iam/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-08-08 01:12:16.000000 types-aiobotocore-iam-2.5.4/types_aiobotocore_iam/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4212 2023-08-08 01:12:19.000000 types-aiobotocore-iam-2.5.4/types_aiobotocore_iam/waiter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4208 2023-08-08 01:12:19.000000 types-aiobotocore-iam-2.5.4/types_aiobotocore_iam/waiter.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:23:48.786729 types-aiobotocore-iam-2.5.4/types_aiobotocore_iam.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    23504 2023-08-08 01:23:48.000000 types-aiobotocore-iam-2.5.4/types_aiobotocore_iam.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      887 2023-08-08 01:23:48.000000 types-aiobotocore-iam-2.5.4/types_aiobotocore_iam.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 01:23:48.000000 types-aiobotocore-iam-2.5.4/types_aiobotocore_iam.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 01:23:48.000000 types-aiobotocore-iam-2.5.4/types_aiobotocore_iam.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-08 01:23:48.000000 types-aiobotocore-iam-2.5.4/types_aiobotocore_iam.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-08-08 01:23:48.000000 types-aiobotocore-iam-2.5.4/types_aiobotocore_iam.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-iam-2.5.2.post2/LICENSE` & `types-aiobotocore-iam-2.5.4/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-iam-2.5.2.post2/PKG-INFO` & `types-aiobotocore-iam-2.5.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-iam
-Version: 2.5.2.post2
-Summary: Type annotations for aiobotocore.IAM 2.5.2 service generated with mypy-boto3-builder 7.17.2
+Version: 2.5.4
+Summary: Type annotations for aiobotocore.IAM 2.5.4 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iam/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-iam.svg?color=blue)](https://pypi.org/project/types-aiobotocore-iam)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iam/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-iam)](https://pepy.tech/project/types-aiobotocore-iam)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.IAM 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM)
+[aiobotocore.IAM 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-iam-2.5.2.post2/README.md` & `types-aiobotocore-iam-2.5.4/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-iam.svg?color=blue)](https://pypi.org/project/types-aiobotocore-iam)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iam/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-iam)](https://pepy.tech/project/types-aiobotocore-iam)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.IAM 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM)
+[aiobotocore.IAM 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-iam-2.5.2.post2/setup.py` & `types-aiobotocore-iam-2.5.4/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-iam",
-    version="2.5.2.post2",
+    version="2.5.4",
     packages=["types_aiobotocore_iam"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.IAM 2.5.2 service generated with mypy-boto3-builder"
+        "Type annotations for aiobotocore.IAM 2.5.4 service generated with mypy-boto3-builder"
         " 7.17.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
```

### Comparing `types-aiobotocore-iam-2.5.2.post2/types_aiobotocore_iam/__init__.py` & `types-aiobotocore-iam-2.5.4/types_aiobotocore_iam/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-iam-2.5.2.post2/types_aiobotocore_iam/__init__.pyi` & `types-aiobotocore-iam-2.5.4/types_aiobotocore_iam/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-iam-2.5.2.post2/types_aiobotocore_iam/__main__.py` & `types-aiobotocore-iam-2.5.4/types_aiobotocore_iam/__main__.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.IAM 2.5.2\nVersion:         2.5.2.post2\nBuilder version:"
+        "Type annotations for aiobotocore.IAM 2.5.4\nVersion:         2.5.4\nBuilder version:"
         " 7.17.2\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iam//\nBoto3 docs:    "
         "  https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM\nOther"
         " services:  https://pypi.org/project/boto3-stubs/\nChangelog:      "
         " https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("2.5.2.post2")
+    print("2.5.4")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `types-aiobotocore-iam-2.5.2.post2/types_aiobotocore_iam/client.py` & `types-aiobotocore-iam-2.5.4/types_aiobotocore_iam/client.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-iam-2.5.2.post2/types_aiobotocore_iam/client.pyi` & `types-aiobotocore-iam-2.5.4/types_aiobotocore_iam/client.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-iam-2.5.2.post2/types_aiobotocore_iam/literals.py` & `types-aiobotocore-iam-2.5.4/types_aiobotocore_iam/literals.py`

 * *Files 1% similar despite different names*

```diff
@@ -203,14 +203,15 @@
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
@@ -306,14 +307,15 @@
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
@@ -392,26 +394,28 @@
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

### Comparing `types-aiobotocore-iam-2.5.2.post2/types_aiobotocore_iam/literals.pyi` & `types-aiobotocore-iam-2.5.4/types_aiobotocore_iam/literals.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -201,14 +201,15 @@
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
@@ -304,14 +305,15 @@
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
@@ -390,26 +392,28 @@
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

### Comparing `types-aiobotocore-iam-2.5.2.post2/types_aiobotocore_iam/paginator.py` & `types-aiobotocore-iam-2.5.4/types_aiobotocore_iam/paginator.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-iam-2.5.2.post2/types_aiobotocore_iam/paginator.pyi` & `types-aiobotocore-iam-2.5.4/types_aiobotocore_iam/paginator.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-iam-2.5.2.post2/types_aiobotocore_iam/service_resource.py` & `types-aiobotocore-iam-2.5.4/types_aiobotocore_iam/service_resource.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-iam-2.5.2.post2/types_aiobotocore_iam/service_resource.pyi` & `types-aiobotocore-iam-2.5.4/types_aiobotocore_iam/service_resource.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-iam-2.5.2.post2/types_aiobotocore_iam/type_defs.py` & `types-aiobotocore-iam-2.5.4/types_aiobotocore_iam/type_defs.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-iam-2.5.2.post2/types_aiobotocore_iam/type_defs.pyi` & `types-aiobotocore-iam-2.5.4/types_aiobotocore_iam/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-iam-2.5.2.post2/types_aiobotocore_iam/waiter.py` & `types-aiobotocore-iam-2.5.4/types_aiobotocore_iam/waiter.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-iam-2.5.2.post2/types_aiobotocore_iam/waiter.pyi` & `types-aiobotocore-iam-2.5.4/types_aiobotocore_iam/waiter.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-iam-2.5.2.post2/types_aiobotocore_iam.egg-info/PKG-INFO` & `types-aiobotocore-iam-2.5.4/types_aiobotocore_iam.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-iam
-Version: 2.5.2.post2
-Summary: Type annotations for aiobotocore.IAM 2.5.2 service generated with mypy-boto3-builder 7.17.2
+Version: 2.5.4
+Summary: Type annotations for aiobotocore.IAM 2.5.4 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iam/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-iam.svg?color=blue)](https://pypi.org/project/types-aiobotocore-iam)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iam/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-iam)](https://pepy.tech/project/types-aiobotocore-iam)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.IAM 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM)
+[aiobotocore.IAM 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-iam-2.5.2.post2/types_aiobotocore_iam.egg-info/SOURCES.txt` & `types-aiobotocore-iam-2.5.4/types_aiobotocore_iam.egg-info/SOURCES.txt`

 * *Files identical despite different names*


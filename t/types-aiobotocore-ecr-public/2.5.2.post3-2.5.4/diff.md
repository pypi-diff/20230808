# Comparing `tmp/types-aiobotocore-ecr-public-2.5.2.post3.tar.gz` & `tmp/types-aiobotocore-ecr-public-2.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-ecr-public-2.5.2.post3.tar", last modified: Fri Aug  4 12:37:39 2023, max compression
+gzip compressed data, was "types-aiobotocore-ecr-public-2.5.4.tar", last modified: Tue Aug  8 01:23:39 2023, max compression
```

## Comparing `types-aiobotocore-ecr-public-2.5.2.post3.tar` & `types-aiobotocore-ecr-public-2.5.4.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:37:39.315708 types-aiobotocore-ecr-public-2.5.2.post3/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-04 12:22:55.000000 types-aiobotocore-ecr-public-2.5.2.post3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    13578 2023-08-04 12:37:39.311708 types-aiobotocore-ecr-public-2.5.2.post3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    12049 2023-08-04 12:22:55.000000 types-aiobotocore-ecr-public-2.5.2.post3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-04 12:37:39.315708 types-aiobotocore-ecr-public-2.5.2.post3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2092 2023-08-04 12:22:55.000000 types-aiobotocore-ecr-public-2.5.2.post3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:37:39.307708 types-aiobotocore-ecr-public-2.5.2.post3/types_aiobotocore_ecr_public/
--rw-r--r--   0 runner    (1001) docker     (123)     1340 2023-08-04 12:22:55.000000 types-aiobotocore-ecr-public-2.5.2.post3/types_aiobotocore_ecr_public/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1339 2023-08-04 12:22:55.000000 types-aiobotocore-ecr-public-2.5.2.post3/types_aiobotocore_ecr_public/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      953 2023-08-04 12:22:55.000000 types-aiobotocore-ecr-public-2.5.2.post3/types_aiobotocore_ecr_public/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    22126 2023-08-04 12:22:55.000000 types-aiobotocore-ecr-public-2.5.2.post3/types_aiobotocore_ecr_public/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    22090 2023-08-04 12:22:55.000000 types-aiobotocore-ecr-public-2.5.2.post3/types_aiobotocore_ecr_public/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8722 2023-08-04 12:22:55.000000 types-aiobotocore-ecr-public-2.5.2.post3/types_aiobotocore_ecr_public/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     8720 2023-08-04 12:22:55.000000 types-aiobotocore-ecr-public-2.5.2.post3/types_aiobotocore_ecr_public/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     5754 2023-08-04 12:22:55.000000 types-aiobotocore-ecr-public-2.5.2.post3/types_aiobotocore_ecr_public/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     5748 2023-08-04 12:22:55.000000 types-aiobotocore-ecr-public-2.5.2.post3/types_aiobotocore_ecr_public/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 12:22:55.000000 types-aiobotocore-ecr-public-2.5.2.post3/types_aiobotocore_ecr_public/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    23744 2023-08-04 12:22:56.000000 types-aiobotocore-ecr-public-2.5.2.post3/types_aiobotocore_ecr_public/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    23709 2023-08-04 12:22:56.000000 types-aiobotocore-ecr-public-2.5.2.post3/types_aiobotocore_ecr_public/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-04 12:22:55.000000 types-aiobotocore-ecr-public-2.5.2.post3/types_aiobotocore_ecr_public/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:37:39.311708 types-aiobotocore-ecr-public-2.5.2.post3/types_aiobotocore_ecr_public.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    13578 2023-08-04 12:37:39.000000 types-aiobotocore-ecr-public-2.5.2.post3/types_aiobotocore_ecr_public.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      870 2023-08-04 12:37:39.000000 types-aiobotocore-ecr-public-2.5.2.post3/types_aiobotocore_ecr_public.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 12:37:39.000000 types-aiobotocore-ecr-public-2.5.2.post3/types_aiobotocore_ecr_public.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 12:37:39.000000 types-aiobotocore-ecr-public-2.5.2.post3/types_aiobotocore_ecr_public.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-04 12:37:39.000000 types-aiobotocore-ecr-public-2.5.2.post3/types_aiobotocore_ecr_public.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-08-04 12:37:39.000000 types-aiobotocore-ecr-public-2.5.2.post3/types_aiobotocore_ecr_public.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:23:39.094696 types-aiobotocore-ecr-public-2.5.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-08 01:10:23.000000 types-aiobotocore-ecr-public-2.5.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    13572 2023-08-08 01:23:39.094696 types-aiobotocore-ecr-public-2.5.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    12049 2023-08-08 01:10:23.000000 types-aiobotocore-ecr-public-2.5.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-08 01:23:39.094696 types-aiobotocore-ecr-public-2.5.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2086 2023-08-08 01:10:22.000000 types-aiobotocore-ecr-public-2.5.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:23:39.094696 types-aiobotocore-ecr-public-2.5.4/types_aiobotocore_ecr_public/
+-rw-r--r--   0 runner    (1001) docker     (123)     1340 2023-08-08 01:10:23.000000 types-aiobotocore-ecr-public-2.5.4/types_aiobotocore_ecr_public/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1339 2023-08-08 01:10:23.000000 types-aiobotocore-ecr-public-2.5.4/types_aiobotocore_ecr_public/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      941 2023-08-08 01:10:23.000000 types-aiobotocore-ecr-public-2.5.4/types_aiobotocore_ecr_public/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22126 2023-08-08 01:10:23.000000 types-aiobotocore-ecr-public-2.5.4/types_aiobotocore_ecr_public/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22090 2023-08-08 01:10:23.000000 types-aiobotocore-ecr-public-2.5.4/types_aiobotocore_ecr_public/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8817 2023-08-08 01:10:23.000000 types-aiobotocore-ecr-public-2.5.4/types_aiobotocore_ecr_public/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8815 2023-08-08 01:10:23.000000 types-aiobotocore-ecr-public-2.5.4/types_aiobotocore_ecr_public/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     5754 2023-08-08 01:10:23.000000 types-aiobotocore-ecr-public-2.5.4/types_aiobotocore_ecr_public/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5748 2023-08-08 01:10:23.000000 types-aiobotocore-ecr-public-2.5.4/types_aiobotocore_ecr_public/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 01:10:23.000000 types-aiobotocore-ecr-public-2.5.4/types_aiobotocore_ecr_public/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    23744 2023-08-08 01:10:23.000000 types-aiobotocore-ecr-public-2.5.4/types_aiobotocore_ecr_public/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23709 2023-08-08 01:10:23.000000 types-aiobotocore-ecr-public-2.5.4/types_aiobotocore_ecr_public/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-08-08 01:10:23.000000 types-aiobotocore-ecr-public-2.5.4/types_aiobotocore_ecr_public/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:23:39.094696 types-aiobotocore-ecr-public-2.5.4/types_aiobotocore_ecr_public.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    13572 2023-08-08 01:23:38.000000 types-aiobotocore-ecr-public-2.5.4/types_aiobotocore_ecr_public.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      870 2023-08-08 01:23:38.000000 types-aiobotocore-ecr-public-2.5.4/types_aiobotocore_ecr_public.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 01:23:38.000000 types-aiobotocore-ecr-public-2.5.4/types_aiobotocore_ecr_public.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 01:23:38.000000 types-aiobotocore-ecr-public-2.5.4/types_aiobotocore_ecr_public.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-08 01:23:38.000000 types-aiobotocore-ecr-public-2.5.4/types_aiobotocore_ecr_public.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-08-08 01:23:38.000000 types-aiobotocore-ecr-public-2.5.4/types_aiobotocore_ecr_public.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-ecr-public-2.5.2.post3/LICENSE` & `types-aiobotocore-ecr-public-2.5.4/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-ecr-public-2.5.2.post3/PKG-INFO` & `types-aiobotocore-ecr-public-2.5.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-ecr-public
-Version: 2.5.2.post3
-Summary: Type annotations for aiobotocore.ECRPublic 2.5.2 service generated with mypy-boto3-builder 7.17.2
+Version: 2.5.4
+Summary: Type annotations for aiobotocore.ECRPublic 2.5.4 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ecr_public/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-ecr-public.svg?color=blue)](https://pypi.org/project/types-aiobotocore-ecr-public)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ecr_public/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-ecr-public)](https://pepy.tech/project/types-aiobotocore-ecr-public)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.ECRPublic 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecr-public.html#ECRPublic)
+[aiobotocore.ECRPublic 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecr-public.html#ECRPublic)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-ecr-public-2.5.2.post3/README.md` & `types-aiobotocore-ecr-public-2.5.4/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-ecr-public.svg?color=blue)](https://pypi.org/project/types-aiobotocore-ecr-public)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ecr_public/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-ecr-public)](https://pepy.tech/project/types-aiobotocore-ecr-public)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.ECRPublic 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecr-public.html#ECRPublic)
+[aiobotocore.ECRPublic 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecr-public.html#ECRPublic)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-ecr-public-2.5.2.post3/setup.py` & `types-aiobotocore-ecr-public-2.5.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-ecr-public",
-    version="2.5.2.post3",
+    version="2.5.4",
     packages=["types_aiobotocore_ecr_public"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.ECRPublic 2.5.2 service generated with mypy-boto3-builder"
+        "Type annotations for aiobotocore.ECRPublic 2.5.4 service generated with mypy-boto3-builder"
         " 7.17.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
```

### Comparing `types-aiobotocore-ecr-public-2.5.2.post3/types_aiobotocore_ecr_public/__init__.py` & `types-aiobotocore-ecr-public-2.5.4/types_aiobotocore_ecr_public/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-ecr-public-2.5.2.post3/types_aiobotocore_ecr_public/__init__.pyi` & `types-aiobotocore-ecr-public-2.5.4/types_aiobotocore_ecr_public/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-ecr-public-2.5.2.post3/types_aiobotocore_ecr_public/__main__.py` & `types-aiobotocore-ecr-public-2.5.4/types_aiobotocore_ecr_public/__main__.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.ECRPublic 2.5.2\nVersion:         2.5.2.post3\nBuilder"
-        " version: 7.17.2\nDocs:           "
+        "Type annotations for aiobotocore.ECRPublic 2.5.4\nVersion:         2.5.4\nBuilder version:"
+        " 7.17.2\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ecr_public//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecr-public.html#ECRPublic\nOther"
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

### Comparing `types-aiobotocore-ecr-public-2.5.2.post3/types_aiobotocore_ecr_public/client.py` & `types-aiobotocore-ecr-public-2.5.4/types_aiobotocore_ecr_public/client.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-ecr-public-2.5.2.post3/types_aiobotocore_ecr_public/client.pyi` & `types-aiobotocore-ecr-public-2.5.4/types_aiobotocore_ecr_public/client.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-ecr-public-2.5.2.post3/types_aiobotocore_ecr_public/literals.py` & `types-aiobotocore-ecr-public-2.5.4/types_aiobotocore_ecr_public/literals.py`

 * *Files 1% similar despite different names*

```diff
@@ -64,14 +64,15 @@
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
@@ -167,14 +168,15 @@
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
@@ -253,26 +255,28 @@
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

### Comparing `types-aiobotocore-ecr-public-2.5.2.post3/types_aiobotocore_ecr_public/literals.pyi` & `types-aiobotocore-ecr-public-2.5.4/types_aiobotocore_ecr_public/literals.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -62,14 +62,15 @@
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
@@ -165,14 +166,15 @@
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
@@ -251,26 +253,28 @@
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

### Comparing `types-aiobotocore-ecr-public-2.5.2.post3/types_aiobotocore_ecr_public/paginator.py` & `types-aiobotocore-ecr-public-2.5.4/types_aiobotocore_ecr_public/paginator.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-ecr-public-2.5.2.post3/types_aiobotocore_ecr_public/paginator.pyi` & `types-aiobotocore-ecr-public-2.5.4/types_aiobotocore_ecr_public/paginator.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-ecr-public-2.5.2.post3/types_aiobotocore_ecr_public/type_defs.py` & `types-aiobotocore-ecr-public-2.5.4/types_aiobotocore_ecr_public/type_defs.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-ecr-public-2.5.2.post3/types_aiobotocore_ecr_public/type_defs.pyi` & `types-aiobotocore-ecr-public-2.5.4/types_aiobotocore_ecr_public/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-ecr-public-2.5.2.post3/types_aiobotocore_ecr_public.egg-info/PKG-INFO` & `types-aiobotocore-ecr-public-2.5.4/types_aiobotocore_ecr_public.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-ecr-public
-Version: 2.5.2.post3
-Summary: Type annotations for aiobotocore.ECRPublic 2.5.2 service generated with mypy-boto3-builder 7.17.2
+Version: 2.5.4
+Summary: Type annotations for aiobotocore.ECRPublic 2.5.4 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ecr_public/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-ecr-public.svg?color=blue)](https://pypi.org/project/types-aiobotocore-ecr-public)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ecr_public/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-ecr-public)](https://pepy.tech/project/types-aiobotocore-ecr-public)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.ECRPublic 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecr-public.html#ECRPublic)
+[aiobotocore.ECRPublic 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecr-public.html#ECRPublic)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-ecr-public-2.5.2.post3/types_aiobotocore_ecr_public.egg-info/SOURCES.txt` & `types-aiobotocore-ecr-public-2.5.4/types_aiobotocore_ecr_public.egg-info/SOURCES.txt`

 * *Files identical despite different names*


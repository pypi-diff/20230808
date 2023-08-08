# Comparing `tmp/types-aiobotocore-dlm-2.5.2.post3.tar.gz` & `tmp/types-aiobotocore-dlm-2.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-dlm-2.5.2.post3.tar", last modified: Fri Aug  4 12:37:36 2023, max compression
+gzip compressed data, was "types-aiobotocore-dlm-2.5.4.tar", last modified: Tue Aug  8 01:23:36 2023, max compression
```

## Comparing `types-aiobotocore-dlm-2.5.2.post3.tar` & `types-aiobotocore-dlm-2.5.4.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:37:36.711647 types-aiobotocore-dlm-2.5.2.post3/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-04 12:21:33.000000 types-aiobotocore-dlm-2.5.2.post3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    11992 2023-08-04 12:37:36.707647 types-aiobotocore-dlm-2.5.2.post3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    10490 2023-08-04 12:21:33.000000 types-aiobotocore-dlm-2.5.2.post3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-04 12:37:36.711647 types-aiobotocore-dlm-2.5.2.post3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2020 2023-08-04 12:21:33.000000 types-aiobotocore-dlm-2.5.2.post3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:37:36.707647 types-aiobotocore-dlm-2.5.2.post3/types_aiobotocore_dlm/
--rw-r--r--   0 runner    (1001) docker     (123)      410 2023-08-04 12:21:33.000000 types-aiobotocore-dlm-2.5.2.post3/types_aiobotocore_dlm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      409 2023-08-04 12:21:33.000000 types-aiobotocore-dlm-2.5.2.post3/types_aiobotocore_dlm/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      916 2023-08-04 12:21:33.000000 types-aiobotocore-dlm-2.5.2.post3/types_aiobotocore_dlm/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8835 2023-08-04 12:21:33.000000 types-aiobotocore-dlm-2.5.2.post3/types_aiobotocore_dlm/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     8819 2023-08-04 12:21:33.000000 types-aiobotocore-dlm-2.5.2.post3/types_aiobotocore_dlm/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8976 2023-08-04 12:21:33.000000 types-aiobotocore-dlm-2.5.2.post3/types_aiobotocore_dlm/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     8974 2023-08-04 12:21:33.000000 types-aiobotocore-dlm-2.5.2.post3/types_aiobotocore_dlm/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 12:21:33.000000 types-aiobotocore-dlm-2.5.2.post3/types_aiobotocore_dlm/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    12399 2023-08-04 12:21:33.000000 types-aiobotocore-dlm-2.5.2.post3/types_aiobotocore_dlm/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    12382 2023-08-04 12:21:33.000000 types-aiobotocore-dlm-2.5.2.post3/types_aiobotocore_dlm/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-04 12:21:33.000000 types-aiobotocore-dlm-2.5.2.post3/types_aiobotocore_dlm/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:37:36.707647 types-aiobotocore-dlm-2.5.2.post3/types_aiobotocore_dlm.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    11992 2023-08-04 12:37:36.000000 types-aiobotocore-dlm-2.5.2.post3/types_aiobotocore_dlm.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      666 2023-08-04 12:37:36.000000 types-aiobotocore-dlm-2.5.2.post3/types_aiobotocore_dlm.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 12:37:36.000000 types-aiobotocore-dlm-2.5.2.post3/types_aiobotocore_dlm.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 12:37:36.000000 types-aiobotocore-dlm-2.5.2.post3/types_aiobotocore_dlm.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-04 12:37:36.000000 types-aiobotocore-dlm-2.5.2.post3/types_aiobotocore_dlm.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-08-04 12:37:36.000000 types-aiobotocore-dlm-2.5.2.post3/types_aiobotocore_dlm.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:23:36.470685 types-aiobotocore-dlm-2.5.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-08 01:09:07.000000 types-aiobotocore-dlm-2.5.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    11986 2023-08-08 01:23:36.466685 types-aiobotocore-dlm-2.5.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10490 2023-08-08 01:09:07.000000 types-aiobotocore-dlm-2.5.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-08 01:23:36.470685 types-aiobotocore-dlm-2.5.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2014 2023-08-08 01:09:07.000000 types-aiobotocore-dlm-2.5.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:23:36.462685 types-aiobotocore-dlm-2.5.4/types_aiobotocore_dlm/
+-rw-r--r--   0 runner    (1001) docker     (123)      410 2023-08-08 01:09:07.000000 types-aiobotocore-dlm-2.5.4/types_aiobotocore_dlm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      409 2023-08-08 01:09:07.000000 types-aiobotocore-dlm-2.5.4/types_aiobotocore_dlm/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      904 2023-08-08 01:09:07.000000 types-aiobotocore-dlm-2.5.4/types_aiobotocore_dlm/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8835 2023-08-08 01:09:07.000000 types-aiobotocore-dlm-2.5.4/types_aiobotocore_dlm/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8819 2023-08-08 01:09:07.000000 types-aiobotocore-dlm-2.5.4/types_aiobotocore_dlm/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9089 2023-08-08 01:09:08.000000 types-aiobotocore-dlm-2.5.4/types_aiobotocore_dlm/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9087 2023-08-08 01:09:07.000000 types-aiobotocore-dlm-2.5.4/types_aiobotocore_dlm/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 01:09:07.000000 types-aiobotocore-dlm-2.5.4/types_aiobotocore_dlm/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    12399 2023-08-08 01:09:08.000000 types-aiobotocore-dlm-2.5.4/types_aiobotocore_dlm/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12382 2023-08-08 01:09:08.000000 types-aiobotocore-dlm-2.5.4/types_aiobotocore_dlm/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-08-08 01:09:07.000000 types-aiobotocore-dlm-2.5.4/types_aiobotocore_dlm/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:23:36.466685 types-aiobotocore-dlm-2.5.4/types_aiobotocore_dlm.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    11986 2023-08-08 01:23:36.000000 types-aiobotocore-dlm-2.5.4/types_aiobotocore_dlm.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      666 2023-08-08 01:23:36.000000 types-aiobotocore-dlm-2.5.4/types_aiobotocore_dlm.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 01:23:36.000000 types-aiobotocore-dlm-2.5.4/types_aiobotocore_dlm.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 01:23:36.000000 types-aiobotocore-dlm-2.5.4/types_aiobotocore_dlm.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-08 01:23:36.000000 types-aiobotocore-dlm-2.5.4/types_aiobotocore_dlm.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-08-08 01:23:36.000000 types-aiobotocore-dlm-2.5.4/types_aiobotocore_dlm.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-dlm-2.5.2.post3/LICENSE` & `types-aiobotocore-dlm-2.5.4/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-dlm-2.5.2.post3/PKG-INFO` & `types-aiobotocore-dlm-2.5.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-dlm
-Version: 2.5.2.post3
-Summary: Type annotations for aiobotocore.DLM 2.5.2 service generated with mypy-boto3-builder 7.17.2
+Version: 2.5.4
+Summary: Type annotations for aiobotocore.DLM 2.5.4 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dlm/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-dlm.svg?color=blue)](https://pypi.org/project/types-aiobotocore-dlm)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dlm/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-dlm)](https://pepy.tech/project/types-aiobotocore-dlm)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.DLM 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dlm.html#DLM)
+[aiobotocore.DLM 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dlm.html#DLM)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-dlm-2.5.2.post3/README.md` & `types-aiobotocore-dlm-2.5.4/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-dlm.svg?color=blue)](https://pypi.org/project/types-aiobotocore-dlm)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dlm/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-dlm)](https://pepy.tech/project/types-aiobotocore-dlm)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.DLM 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dlm.html#DLM)
+[aiobotocore.DLM 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dlm.html#DLM)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-dlm-2.5.2.post3/setup.py` & `types-aiobotocore-dlm-2.5.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-dlm",
-    version="2.5.2.post3",
+    version="2.5.4",
     packages=["types_aiobotocore_dlm"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.DLM 2.5.2 service generated with mypy-boto3-builder"
+        "Type annotations for aiobotocore.DLM 2.5.4 service generated with mypy-boto3-builder"
         " 7.17.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
```

### Comparing `types-aiobotocore-dlm-2.5.2.post3/types_aiobotocore_dlm/__main__.py` & `types-aiobotocore-dlm-2.5.4/types_aiobotocore_dlm/__main__.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.DLM 2.5.2\nVersion:         2.5.2.post3\nBuilder version:"
+        "Type annotations for aiobotocore.DLM 2.5.4\nVersion:         2.5.4\nBuilder version:"
         " 7.17.2\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dlm//\nBoto3 docs:    "
         "  https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dlm.html#DLM\nOther"
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

### Comparing `types-aiobotocore-dlm-2.5.2.post3/types_aiobotocore_dlm/client.py` & `types-aiobotocore-dlm-2.5.4/types_aiobotocore_dlm/client.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-dlm-2.5.2.post3/types_aiobotocore_dlm/client.pyi` & `types-aiobotocore-dlm-2.5.4/types_aiobotocore_dlm/client.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-dlm-2.5.2.post3/types_aiobotocore_dlm/literals.py` & `types-aiobotocore-dlm-2.5.4/types_aiobotocore_dlm/literals.py`

 * *Files 2% similar despite different names*

```diff
@@ -59,14 +59,15 @@
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
@@ -162,14 +163,15 @@
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
@@ -248,26 +250,28 @@
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
@@ -414,14 +418,15 @@
 RegionName = Literal[
     "af-south-1",
     "ap-east-1",
     "ap-northeast-1",
     "ap-northeast-2",
     "ap-northeast-3",
     "ap-south-1",
+    "ap-south-2",
     "ap-southeast-1",
     "ap-southeast-2",
     "ap-southeast-3",
     "ap-southeast-4",
     "ca-central-1",
     "eu-central-1",
     "eu-central-2",
```

### Comparing `types-aiobotocore-dlm-2.5.2.post3/types_aiobotocore_dlm/literals.pyi` & `types-aiobotocore-dlm-2.5.4/types_aiobotocore_dlm/literals.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -57,14 +57,15 @@
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
@@ -160,14 +161,15 @@
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
@@ -246,26 +248,28 @@
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
@@ -412,14 +416,15 @@
 RegionName = Literal[
     "af-south-1",
     "ap-east-1",
     "ap-northeast-1",
     "ap-northeast-2",
     "ap-northeast-3",
     "ap-south-1",
+    "ap-south-2",
     "ap-southeast-1",
     "ap-southeast-2",
     "ap-southeast-3",
     "ap-southeast-4",
     "ca-central-1",
     "eu-central-1",
     "eu-central-2",
```

### Comparing `types-aiobotocore-dlm-2.5.2.post3/types_aiobotocore_dlm/type_defs.py` & `types-aiobotocore-dlm-2.5.4/types_aiobotocore_dlm/type_defs.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-dlm-2.5.2.post3/types_aiobotocore_dlm/type_defs.pyi` & `types-aiobotocore-dlm-2.5.4/types_aiobotocore_dlm/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-dlm-2.5.2.post3/types_aiobotocore_dlm.egg-info/PKG-INFO` & `types-aiobotocore-dlm-2.5.4/types_aiobotocore_dlm.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-dlm
-Version: 2.5.2.post3
-Summary: Type annotations for aiobotocore.DLM 2.5.2 service generated with mypy-boto3-builder 7.17.2
+Version: 2.5.4
+Summary: Type annotations for aiobotocore.DLM 2.5.4 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dlm/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-dlm.svg?color=blue)](https://pypi.org/project/types-aiobotocore-dlm)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dlm/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-dlm)](https://pepy.tech/project/types-aiobotocore-dlm)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.DLM 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dlm.html#DLM)
+[aiobotocore.DLM 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dlm.html#DLM)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-dlm-2.5.2.post3/types_aiobotocore_dlm.egg-info/SOURCES.txt` & `types-aiobotocore-dlm-2.5.4/types_aiobotocore_dlm.egg-info/SOURCES.txt`

 * *Files identical despite different names*


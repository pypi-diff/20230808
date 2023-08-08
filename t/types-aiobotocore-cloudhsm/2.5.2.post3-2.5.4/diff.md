# Comparing `tmp/types-aiobotocore-cloudhsm-2.5.2.post3.tar.gz` & `tmp/types-aiobotocore-cloudhsm-2.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-cloudhsm-2.5.2.post3.tar", last modified: Fri Aug  4 12:37:24 2023, max compression
+gzip compressed data, was "types-aiobotocore-cloudhsm-2.5.4.tar", last modified: Tue Aug  8 01:23:26 2023, max compression
```

## Comparing `types-aiobotocore-cloudhsm-2.5.2.post3.tar` & `types-aiobotocore-cloudhsm-2.5.4.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:37:24.799354 types-aiobotocore-cloudhsm-2.5.2.post3/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-04 12:19:48.000000 types-aiobotocore-cloudhsm-2.5.2.post3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    13171 2023-08-04 12:37:24.799354 types-aiobotocore-cloudhsm-2.5.2.post3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    11649 2023-08-04 12:19:48.000000 types-aiobotocore-cloudhsm-2.5.2.post3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-04 12:37:24.799354 types-aiobotocore-cloudhsm-2.5.2.post3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2079 2023-08-04 12:19:48.000000 types-aiobotocore-cloudhsm-2.5.2.post3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:37:24.799354 types-aiobotocore-cloudhsm-2.5.2.post3/types_aiobotocore_cloudhsm/
--rw-r--r--   0 runner    (1001) docker     (123)      984 2023-08-04 12:19:48.000000 types-aiobotocore-cloudhsm-2.5.2.post3/types_aiobotocore_cloudhsm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      983 2023-08-04 12:19:48.000000 types-aiobotocore-cloudhsm-2.5.2.post3/types_aiobotocore_cloudhsm/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      947 2023-08-04 12:19:48.000000 types-aiobotocore-cloudhsm-2.5.2.post3/types_aiobotocore_cloudhsm/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16664 2023-08-04 12:19:48.000000 types-aiobotocore-cloudhsm-2.5.2.post3/types_aiobotocore_cloudhsm/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    16632 2023-08-04 12:19:48.000000 types-aiobotocore-cloudhsm-2.5.2.post3/types_aiobotocore_cloudhsm/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8289 2023-08-04 12:19:48.000000 types-aiobotocore-cloudhsm-2.5.2.post3/types_aiobotocore_cloudhsm/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     8287 2023-08-04 12:19:48.000000 types-aiobotocore-cloudhsm-2.5.2.post3/types_aiobotocore_cloudhsm/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     4006 2023-08-04 12:19:48.000000 types-aiobotocore-cloudhsm-2.5.2.post3/types_aiobotocore_cloudhsm/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     4001 2023-08-04 12:19:48.000000 types-aiobotocore-cloudhsm-2.5.2.post3/types_aiobotocore_cloudhsm/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 12:19:48.000000 types-aiobotocore-cloudhsm-2.5.2.post3/types_aiobotocore_cloudhsm/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    12603 2023-08-04 12:19:48.000000 types-aiobotocore-cloudhsm-2.5.2.post3/types_aiobotocore_cloudhsm/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    12594 2023-08-04 12:19:48.000000 types-aiobotocore-cloudhsm-2.5.2.post3/types_aiobotocore_cloudhsm/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-04 12:19:48.000000 types-aiobotocore-cloudhsm-2.5.2.post3/types_aiobotocore_cloudhsm/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:37:24.799354 types-aiobotocore-cloudhsm-2.5.2.post3/types_aiobotocore_cloudhsm.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    13171 2023-08-04 12:37:24.000000 types-aiobotocore-cloudhsm-2.5.2.post3/types_aiobotocore_cloudhsm.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      832 2023-08-04 12:37:24.000000 types-aiobotocore-cloudhsm-2.5.2.post3/types_aiobotocore_cloudhsm.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 12:37:24.000000 types-aiobotocore-cloudhsm-2.5.2.post3/types_aiobotocore_cloudhsm.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 12:37:24.000000 types-aiobotocore-cloudhsm-2.5.2.post3/types_aiobotocore_cloudhsm.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-04 12:37:24.000000 types-aiobotocore-cloudhsm-2.5.2.post3/types_aiobotocore_cloudhsm.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-08-04 12:37:24.000000 types-aiobotocore-cloudhsm-2.5.2.post3/types_aiobotocore_cloudhsm.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:23:26.418626 types-aiobotocore-cloudhsm-2.5.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-08 01:07:29.000000 types-aiobotocore-cloudhsm-2.5.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    13165 2023-08-08 01:23:26.418626 types-aiobotocore-cloudhsm-2.5.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    11649 2023-08-08 01:07:29.000000 types-aiobotocore-cloudhsm-2.5.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-08 01:23:26.418626 types-aiobotocore-cloudhsm-2.5.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2073 2023-08-08 01:07:29.000000 types-aiobotocore-cloudhsm-2.5.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:23:26.418626 types-aiobotocore-cloudhsm-2.5.4/types_aiobotocore_cloudhsm/
+-rw-r--r--   0 runner    (1001) docker     (123)      984 2023-08-08 01:07:29.000000 types-aiobotocore-cloudhsm-2.5.4/types_aiobotocore_cloudhsm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      983 2023-08-08 01:07:29.000000 types-aiobotocore-cloudhsm-2.5.4/types_aiobotocore_cloudhsm/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      935 2023-08-08 01:07:29.000000 types-aiobotocore-cloudhsm-2.5.4/types_aiobotocore_cloudhsm/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16664 2023-08-08 01:07:29.000000 types-aiobotocore-cloudhsm-2.5.4/types_aiobotocore_cloudhsm/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16632 2023-08-08 01:07:29.000000 types-aiobotocore-cloudhsm-2.5.4/types_aiobotocore_cloudhsm/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8384 2023-08-08 01:07:30.000000 types-aiobotocore-cloudhsm-2.5.4/types_aiobotocore_cloudhsm/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8382 2023-08-08 01:07:29.000000 types-aiobotocore-cloudhsm-2.5.4/types_aiobotocore_cloudhsm/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     4006 2023-08-08 01:07:29.000000 types-aiobotocore-cloudhsm-2.5.4/types_aiobotocore_cloudhsm/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4001 2023-08-08 01:07:29.000000 types-aiobotocore-cloudhsm-2.5.4/types_aiobotocore_cloudhsm/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 01:07:29.000000 types-aiobotocore-cloudhsm-2.5.4/types_aiobotocore_cloudhsm/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    12603 2023-08-08 01:07:30.000000 types-aiobotocore-cloudhsm-2.5.4/types_aiobotocore_cloudhsm/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12594 2023-08-08 01:07:30.000000 types-aiobotocore-cloudhsm-2.5.4/types_aiobotocore_cloudhsm/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-08-08 01:07:29.000000 types-aiobotocore-cloudhsm-2.5.4/types_aiobotocore_cloudhsm/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:23:26.418626 types-aiobotocore-cloudhsm-2.5.4/types_aiobotocore_cloudhsm.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    13165 2023-08-08 01:23:26.000000 types-aiobotocore-cloudhsm-2.5.4/types_aiobotocore_cloudhsm.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      832 2023-08-08 01:23:26.000000 types-aiobotocore-cloudhsm-2.5.4/types_aiobotocore_cloudhsm.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 01:23:26.000000 types-aiobotocore-cloudhsm-2.5.4/types_aiobotocore_cloudhsm.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 01:23:26.000000 types-aiobotocore-cloudhsm-2.5.4/types_aiobotocore_cloudhsm.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-08 01:23:26.000000 types-aiobotocore-cloudhsm-2.5.4/types_aiobotocore_cloudhsm.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-08-08 01:23:26.000000 types-aiobotocore-cloudhsm-2.5.4/types_aiobotocore_cloudhsm.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-cloudhsm-2.5.2.post3/LICENSE` & `types-aiobotocore-cloudhsm-2.5.4/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-cloudhsm-2.5.2.post3/PKG-INFO` & `types-aiobotocore-cloudhsm-2.5.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-cloudhsm
-Version: 2.5.2.post3
-Summary: Type annotations for aiobotocore.CloudHSM 2.5.2 service generated with mypy-boto3-builder 7.17.2
+Version: 2.5.4
+Summary: Type annotations for aiobotocore.CloudHSM 2.5.4 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudhsm/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-cloudhsm.svg?color=blue)](https://pypi.org/project/types-aiobotocore-cloudhsm)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudhsm/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-cloudhsm)](https://pepy.tech/project/types-aiobotocore-cloudhsm)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.CloudHSM 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudhsm.html#CloudHSM)
+[aiobotocore.CloudHSM 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudhsm.html#CloudHSM)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-cloudhsm-2.5.2.post3/README.md` & `types-aiobotocore-cloudhsm-2.5.4/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-cloudhsm.svg?color=blue)](https://pypi.org/project/types-aiobotocore-cloudhsm)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudhsm/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-cloudhsm)](https://pepy.tech/project/types-aiobotocore-cloudhsm)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.CloudHSM 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudhsm.html#CloudHSM)
+[aiobotocore.CloudHSM 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudhsm.html#CloudHSM)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-cloudhsm-2.5.2.post3/setup.py` & `types-aiobotocore-cloudhsm-2.5.4/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-cloudhsm",
-    version="2.5.2.post3",
+    version="2.5.4",
     packages=["types_aiobotocore_cloudhsm"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.CloudHSM 2.5.2 service generated with mypy-boto3-builder"
+        "Type annotations for aiobotocore.CloudHSM 2.5.4 service generated with mypy-boto3-builder"
         " 7.17.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
```

### Comparing `types-aiobotocore-cloudhsm-2.5.2.post3/types_aiobotocore_cloudhsm/__init__.py` & `types-aiobotocore-cloudhsm-2.5.4/types_aiobotocore_cloudhsm/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-cloudhsm-2.5.2.post3/types_aiobotocore_cloudhsm/__init__.pyi` & `types-aiobotocore-cloudhsm-2.5.4/types_aiobotocore_cloudhsm/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-cloudhsm-2.5.2.post3/types_aiobotocore_cloudhsm/__main__.py` & `types-aiobotocore-cloudhsm-2.5.4/types_aiobotocore_cloudhsm/__main__.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.CloudHSM 2.5.2\nVersion:         2.5.2.post3\nBuilder"
-        " version: 7.17.2\nDocs:           "
+        "Type annotations for aiobotocore.CloudHSM 2.5.4\nVersion:         2.5.4\nBuilder version:"
+        " 7.17.2\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudhsm//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudhsm.html#CloudHSM\nOther"
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

### Comparing `types-aiobotocore-cloudhsm-2.5.2.post3/types_aiobotocore_cloudhsm/client.py` & `types-aiobotocore-cloudhsm-2.5.4/types_aiobotocore_cloudhsm/client.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-cloudhsm-2.5.2.post3/types_aiobotocore_cloudhsm/client.pyi` & `types-aiobotocore-cloudhsm-2.5.4/types_aiobotocore_cloudhsm/client.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-cloudhsm-2.5.2.post3/types_aiobotocore_cloudhsm/literals.py` & `types-aiobotocore-cloudhsm-2.5.4/types_aiobotocore_cloudhsm/literals.py`

 * *Files 0% similar despite different names*

```diff
@@ -56,14 +56,15 @@
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
@@ -159,14 +160,15 @@
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
@@ -245,26 +247,28 @@
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

### Comparing `types-aiobotocore-cloudhsm-2.5.2.post3/types_aiobotocore_cloudhsm/literals.pyi` & `types-aiobotocore-cloudhsm-2.5.4/types_aiobotocore_cloudhsm/literals.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -54,14 +54,15 @@
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
@@ -157,14 +158,15 @@
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
@@ -243,26 +245,28 @@
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

### Comparing `types-aiobotocore-cloudhsm-2.5.2.post3/types_aiobotocore_cloudhsm/paginator.py` & `types-aiobotocore-cloudhsm-2.5.4/types_aiobotocore_cloudhsm/paginator.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-cloudhsm-2.5.2.post3/types_aiobotocore_cloudhsm/paginator.pyi` & `types-aiobotocore-cloudhsm-2.5.4/types_aiobotocore_cloudhsm/paginator.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-cloudhsm-2.5.2.post3/types_aiobotocore_cloudhsm/type_defs.py` & `types-aiobotocore-cloudhsm-2.5.4/types_aiobotocore_cloudhsm/type_defs.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-cloudhsm-2.5.2.post3/types_aiobotocore_cloudhsm/type_defs.pyi` & `types-aiobotocore-cloudhsm-2.5.4/types_aiobotocore_cloudhsm/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-cloudhsm-2.5.2.post3/types_aiobotocore_cloudhsm.egg-info/PKG-INFO` & `types-aiobotocore-cloudhsm-2.5.4/types_aiobotocore_cloudhsm.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-cloudhsm
-Version: 2.5.2.post3
-Summary: Type annotations for aiobotocore.CloudHSM 2.5.2 service generated with mypy-boto3-builder 7.17.2
+Version: 2.5.4
+Summary: Type annotations for aiobotocore.CloudHSM 2.5.4 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudhsm/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-cloudhsm.svg?color=blue)](https://pypi.org/project/types-aiobotocore-cloudhsm)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudhsm/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-cloudhsm)](https://pepy.tech/project/types-aiobotocore-cloudhsm)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.CloudHSM 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudhsm.html#CloudHSM)
+[aiobotocore.CloudHSM 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudhsm.html#CloudHSM)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-cloudhsm-2.5.2.post3/types_aiobotocore_cloudhsm.egg-info/SOURCES.txt` & `types-aiobotocore-cloudhsm-2.5.4/types_aiobotocore_cloudhsm.egg-info/SOURCES.txt`

 * *Files identical despite different names*


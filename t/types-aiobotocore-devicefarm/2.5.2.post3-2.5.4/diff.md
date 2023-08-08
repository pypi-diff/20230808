# Comparing `tmp/types-aiobotocore-devicefarm-2.5.2.post3.tar.gz` & `tmp/types-aiobotocore-devicefarm-2.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-devicefarm-2.5.2.post3.tar", last modified: Fri Aug  4 12:37:34 2023, max compression
+gzip compressed data, was "types-aiobotocore-devicefarm-2.5.4.tar", last modified: Tue Aug  8 01:23:35 2023, max compression
```

## Comparing `types-aiobotocore-devicefarm-2.5.2.post3.tar` & `types-aiobotocore-devicefarm-2.5.4.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:37:34.671599 types-aiobotocore-devicefarm-2.5.2.post3/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-04 12:21:21.000000 types-aiobotocore-devicefarm-2.5.2.post3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    15745 2023-08-04 12:37:34.671599 types-aiobotocore-devicefarm-2.5.2.post3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    14215 2023-08-04 12:21:21.000000 types-aiobotocore-devicefarm-2.5.2.post3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-04 12:37:34.671599 types-aiobotocore-devicefarm-2.5.2.post3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2093 2023-08-04 12:21:21.000000 types-aiobotocore-devicefarm-2.5.2.post3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:37:34.671599 types-aiobotocore-devicefarm-2.5.2.post3/types_aiobotocore_devicefarm/
--rw-r--r--   0 runner    (1001) docker     (123)     4483 2023-08-04 12:21:21.000000 types-aiobotocore-devicefarm-2.5.2.post3/types_aiobotocore_devicefarm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4482 2023-08-04 12:21:21.000000 types-aiobotocore-devicefarm-2.5.2.post3/types_aiobotocore_devicefarm/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      955 2023-08-04 12:21:21.000000 types-aiobotocore-devicefarm-2.5.2.post3/types_aiobotocore_devicefarm/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    60953 2023-08-04 12:21:21.000000 types-aiobotocore-devicefarm-2.5.2.post3/types_aiobotocore_devicefarm/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    60847 2023-08-04 12:21:21.000000 types-aiobotocore-devicefarm-2.5.2.post3/types_aiobotocore_devicefarm/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    15719 2023-08-04 12:21:22.000000 types-aiobotocore-devicefarm-2.5.2.post3/types_aiobotocore_devicefarm/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    15717 2023-08-04 12:21:21.000000 types-aiobotocore-devicefarm-2.5.2.post3/types_aiobotocore_devicefarm/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    23366 2023-08-04 12:21:21.000000 types-aiobotocore-devicefarm-2.5.2.post3/types_aiobotocore_devicefarm/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)    23344 2023-08-04 12:21:21.000000 types-aiobotocore-devicefarm-2.5.2.post3/types_aiobotocore_devicefarm/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 12:21:21.000000 types-aiobotocore-devicefarm-2.5.2.post3/types_aiobotocore_devicefarm/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    73144 2023-08-04 12:21:24.000000 types-aiobotocore-devicefarm-2.5.2.post3/types_aiobotocore_devicefarm/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    73053 2023-08-04 12:21:22.000000 types-aiobotocore-devicefarm-2.5.2.post3/types_aiobotocore_devicefarm/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-04 12:21:21.000000 types-aiobotocore-devicefarm-2.5.2.post3/types_aiobotocore_devicefarm/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:37:34.671599 types-aiobotocore-devicefarm-2.5.2.post3/types_aiobotocore_devicefarm.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    15745 2023-08-04 12:37:34.000000 types-aiobotocore-devicefarm-2.5.2.post3/types_aiobotocore_devicefarm.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      870 2023-08-04 12:37:34.000000 types-aiobotocore-devicefarm-2.5.2.post3/types_aiobotocore_devicefarm.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 12:37:34.000000 types-aiobotocore-devicefarm-2.5.2.post3/types_aiobotocore_devicefarm.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 12:37:34.000000 types-aiobotocore-devicefarm-2.5.2.post3/types_aiobotocore_devicefarm.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-04 12:37:34.000000 types-aiobotocore-devicefarm-2.5.2.post3/types_aiobotocore_devicefarm.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-08-04 12:37:34.000000 types-aiobotocore-devicefarm-2.5.2.post3/types_aiobotocore_devicefarm.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:23:35.942683 types-aiobotocore-devicefarm-2.5.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-08 01:08:57.000000 types-aiobotocore-devicefarm-2.5.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    15739 2023-08-08 01:23:35.942683 types-aiobotocore-devicefarm-2.5.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    14215 2023-08-08 01:08:57.000000 types-aiobotocore-devicefarm-2.5.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-08 01:23:35.942683 types-aiobotocore-devicefarm-2.5.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2087 2023-08-08 01:08:57.000000 types-aiobotocore-devicefarm-2.5.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:23:35.942683 types-aiobotocore-devicefarm-2.5.4/types_aiobotocore_devicefarm/
+-rw-r--r--   0 runner    (1001) docker     (123)     4483 2023-08-08 01:08:57.000000 types-aiobotocore-devicefarm-2.5.4/types_aiobotocore_devicefarm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4482 2023-08-08 01:08:57.000000 types-aiobotocore-devicefarm-2.5.4/types_aiobotocore_devicefarm/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      943 2023-08-08 01:08:57.000000 types-aiobotocore-devicefarm-2.5.4/types_aiobotocore_devicefarm/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    60953 2023-08-08 01:08:57.000000 types-aiobotocore-devicefarm-2.5.4/types_aiobotocore_devicefarm/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    60847 2023-08-08 01:08:57.000000 types-aiobotocore-devicefarm-2.5.4/types_aiobotocore_devicefarm/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    15814 2023-08-08 01:08:58.000000 types-aiobotocore-devicefarm-2.5.4/types_aiobotocore_devicefarm/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15812 2023-08-08 01:08:57.000000 types-aiobotocore-devicefarm-2.5.4/types_aiobotocore_devicefarm/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    23366 2023-08-08 01:08:57.000000 types-aiobotocore-devicefarm-2.5.4/types_aiobotocore_devicefarm/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23344 2023-08-08 01:08:57.000000 types-aiobotocore-devicefarm-2.5.4/types_aiobotocore_devicefarm/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 01:08:57.000000 types-aiobotocore-devicefarm-2.5.4/types_aiobotocore_devicefarm/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    73144 2023-08-08 01:08:59.000000 types-aiobotocore-devicefarm-2.5.4/types_aiobotocore_devicefarm/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    73053 2023-08-08 01:08:58.000000 types-aiobotocore-devicefarm-2.5.4/types_aiobotocore_devicefarm/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-08-08 01:08:57.000000 types-aiobotocore-devicefarm-2.5.4/types_aiobotocore_devicefarm/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:23:35.942683 types-aiobotocore-devicefarm-2.5.4/types_aiobotocore_devicefarm.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    15739 2023-08-08 01:23:35.000000 types-aiobotocore-devicefarm-2.5.4/types_aiobotocore_devicefarm.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      870 2023-08-08 01:23:35.000000 types-aiobotocore-devicefarm-2.5.4/types_aiobotocore_devicefarm.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 01:23:35.000000 types-aiobotocore-devicefarm-2.5.4/types_aiobotocore_devicefarm.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 01:23:35.000000 types-aiobotocore-devicefarm-2.5.4/types_aiobotocore_devicefarm.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-08 01:23:35.000000 types-aiobotocore-devicefarm-2.5.4/types_aiobotocore_devicefarm.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-08-08 01:23:35.000000 types-aiobotocore-devicefarm-2.5.4/types_aiobotocore_devicefarm.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-devicefarm-2.5.2.post3/LICENSE` & `types-aiobotocore-devicefarm-2.5.4/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-devicefarm-2.5.2.post3/PKG-INFO` & `types-aiobotocore-devicefarm-2.5.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-devicefarm
-Version: 2.5.2.post3
-Summary: Type annotations for aiobotocore.DeviceFarm 2.5.2 service generated with mypy-boto3-builder 7.17.2
+Version: 2.5.4
+Summary: Type annotations for aiobotocore.DeviceFarm 2.5.4 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_devicefarm/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-devicefarm.svg?color=blue)](https://pypi.org/project/types-aiobotocore-devicefarm)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_devicefarm/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-devicefarm)](https://pepy.tech/project/types-aiobotocore-devicefarm)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.DeviceFarm 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devicefarm.html#DeviceFarm)
+[aiobotocore.DeviceFarm 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devicefarm.html#DeviceFarm)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-devicefarm-2.5.2.post3/README.md` & `types-aiobotocore-devicefarm-2.5.4/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-devicefarm.svg?color=blue)](https://pypi.org/project/types-aiobotocore-devicefarm)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_devicefarm/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-devicefarm)](https://pepy.tech/project/types-aiobotocore-devicefarm)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.DeviceFarm 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devicefarm.html#DeviceFarm)
+[aiobotocore.DeviceFarm 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devicefarm.html#DeviceFarm)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-devicefarm-2.5.2.post3/setup.py` & `types-aiobotocore-devicefarm-2.5.4/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-devicefarm",
-    version="2.5.2.post3",
+    version="2.5.4",
     packages=["types_aiobotocore_devicefarm"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.DeviceFarm 2.5.2 service generated with"
+        "Type annotations for aiobotocore.DeviceFarm 2.5.4 service generated with"
         " mypy-boto3-builder 7.17.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
```

### Comparing `types-aiobotocore-devicefarm-2.5.2.post3/types_aiobotocore_devicefarm/__init__.py` & `types-aiobotocore-devicefarm-2.5.4/types_aiobotocore_devicefarm/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-devicefarm-2.5.2.post3/types_aiobotocore_devicefarm/__init__.pyi` & `types-aiobotocore-devicefarm-2.5.4/types_aiobotocore_devicefarm/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-devicefarm-2.5.2.post3/types_aiobotocore_devicefarm/__main__.py` & `types-aiobotocore-devicefarm-2.5.4/types_aiobotocore_devicefarm/__main__.py`

 * *Files 9% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.DeviceFarm 2.5.2\nVersion:         2.5.2.post3\nBuilder"
+        "Type annotations for aiobotocore.DeviceFarm 2.5.4\nVersion:         2.5.4\nBuilder"
         " version: 7.17.2\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_devicefarm//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devicefarm.html#DeviceFarm\nOther"
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

### Comparing `types-aiobotocore-devicefarm-2.5.2.post3/types_aiobotocore_devicefarm/client.py` & `types-aiobotocore-devicefarm-2.5.4/types_aiobotocore_devicefarm/client.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-devicefarm-2.5.2.post3/types_aiobotocore_devicefarm/client.pyi` & `types-aiobotocore-devicefarm-2.5.4/types_aiobotocore_devicefarm/client.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-devicefarm-2.5.2.post3/types_aiobotocore_devicefarm/literals.py` & `types-aiobotocore-devicefarm-2.5.4/types_aiobotocore_devicefarm/literals.py`

 * *Files 1% similar despite different names*

```diff
@@ -286,14 +286,15 @@
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
@@ -389,14 +390,15 @@
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
@@ -475,26 +477,28 @@
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

### Comparing `types-aiobotocore-devicefarm-2.5.2.post3/types_aiobotocore_devicefarm/literals.pyi` & `types-aiobotocore-devicefarm-2.5.4/types_aiobotocore_devicefarm/literals.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -284,14 +284,15 @@
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
@@ -387,14 +388,15 @@
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
@@ -473,26 +475,28 @@
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

### Comparing `types-aiobotocore-devicefarm-2.5.2.post3/types_aiobotocore_devicefarm/paginator.py` & `types-aiobotocore-devicefarm-2.5.4/types_aiobotocore_devicefarm/paginator.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-devicefarm-2.5.2.post3/types_aiobotocore_devicefarm/paginator.pyi` & `types-aiobotocore-devicefarm-2.5.4/types_aiobotocore_devicefarm/paginator.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-devicefarm-2.5.2.post3/types_aiobotocore_devicefarm/type_defs.py` & `types-aiobotocore-devicefarm-2.5.4/types_aiobotocore_devicefarm/type_defs.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-devicefarm-2.5.2.post3/types_aiobotocore_devicefarm/type_defs.pyi` & `types-aiobotocore-devicefarm-2.5.4/types_aiobotocore_devicefarm/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-devicefarm-2.5.2.post3/types_aiobotocore_devicefarm.egg-info/PKG-INFO` & `types-aiobotocore-devicefarm-2.5.4/types_aiobotocore_devicefarm.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-devicefarm
-Version: 2.5.2.post3
-Summary: Type annotations for aiobotocore.DeviceFarm 2.5.2 service generated with mypy-boto3-builder 7.17.2
+Version: 2.5.4
+Summary: Type annotations for aiobotocore.DeviceFarm 2.5.4 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_devicefarm/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-devicefarm.svg?color=blue)](https://pypi.org/project/types-aiobotocore-devicefarm)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_devicefarm/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-devicefarm)](https://pepy.tech/project/types-aiobotocore-devicefarm)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.DeviceFarm 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devicefarm.html#DeviceFarm)
+[aiobotocore.DeviceFarm 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devicefarm.html#DeviceFarm)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-devicefarm-2.5.2.post3/types_aiobotocore_devicefarm.egg-info/SOURCES.txt` & `types-aiobotocore-devicefarm-2.5.4/types_aiobotocore_devicefarm.egg-info/SOURCES.txt`

 * *Files identical despite different names*


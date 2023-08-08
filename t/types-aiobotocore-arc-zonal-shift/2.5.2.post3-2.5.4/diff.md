# Comparing `tmp/types-aiobotocore-arc-zonal-shift-2.5.2.post3.tar.gz` & `tmp/types-aiobotocore-arc-zonal-shift-2.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-arc-zonal-shift-2.5.2.post3.tar", last modified: Fri Aug  4 12:37:18 2023, max compression
+gzip compressed data, was "types-aiobotocore-arc-zonal-shift-2.5.4.tar", last modified: Tue Aug  8 01:23:19 2023, max compression
```

## Comparing `types-aiobotocore-arc-zonal-shift-2.5.2.post3.tar` & `types-aiobotocore-arc-zonal-shift-2.5.4.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:37:18.951226 types-aiobotocore-arc-zonal-shift-2.5.2.post3/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-04 12:18:39.000000 types-aiobotocore-arc-zonal-shift-2.5.2.post3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    13574 2023-08-04 12:37:18.951226 types-aiobotocore-arc-zonal-shift-2.5.2.post3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    12026 2023-08-04 12:18:39.000000 types-aiobotocore-arc-zonal-shift-2.5.2.post3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-04 12:37:18.951226 types-aiobotocore-arc-zonal-shift-2.5.2.post3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2126 2023-08-04 12:18:39.000000 types-aiobotocore-arc-zonal-shift-2.5.2.post3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:37:18.939226 types-aiobotocore-arc-zonal-shift-2.5.2.post3/types_aiobotocore_arc_zonal_shift/
--rw-r--r--   0 runner    (1001) docker     (123)      948 2023-08-04 12:18:39.000000 types-aiobotocore-arc-zonal-shift-2.5.2.post3/types_aiobotocore_arc_zonal_shift/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      947 2023-08-04 12:18:39.000000 types-aiobotocore-arc-zonal-shift-2.5.2.post3/types_aiobotocore_arc_zonal_shift/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      971 2023-08-04 12:18:39.000000 types-aiobotocore-arc-zonal-shift-2.5.2.post3/types_aiobotocore_arc_zonal_shift/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9732 2023-08-04 12:18:39.000000 types-aiobotocore-arc-zonal-shift-2.5.2.post3/types_aiobotocore_arc_zonal_shift/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     9715 2023-08-04 12:18:39.000000 types-aiobotocore-arc-zonal-shift-2.5.2.post3/types_aiobotocore_arc_zonal_shift/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8587 2023-08-04 12:18:40.000000 types-aiobotocore-arc-zonal-shift-2.5.2.post3/types_aiobotocore_arc_zonal_shift/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     8585 2023-08-04 12:18:39.000000 types-aiobotocore-arc-zonal-shift-2.5.2.post3/types_aiobotocore_arc_zonal_shift/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     3352 2023-08-04 12:18:39.000000 types-aiobotocore-arc-zonal-shift-2.5.2.post3/types_aiobotocore_arc_zonal_shift/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     3348 2023-08-04 12:18:39.000000 types-aiobotocore-arc-zonal-shift-2.5.2.post3/types_aiobotocore_arc_zonal_shift/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 12:18:39.000000 types-aiobotocore-arc-zonal-shift-2.5.2.post3/types_aiobotocore_arc_zonal_shift/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     5866 2023-08-04 12:18:40.000000 types-aiobotocore-arc-zonal-shift-2.5.2.post3/types_aiobotocore_arc_zonal_shift/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)     5861 2023-08-04 12:18:40.000000 types-aiobotocore-arc-zonal-shift-2.5.2.post3/types_aiobotocore_arc_zonal_shift/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-04 12:18:39.000000 types-aiobotocore-arc-zonal-shift-2.5.2.post3/types_aiobotocore_arc_zonal_shift/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:37:18.951226 types-aiobotocore-arc-zonal-shift-2.5.2.post3/types_aiobotocore_arc_zonal_shift.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    13574 2023-08-04 12:37:18.000000 types-aiobotocore-arc-zonal-shift-2.5.2.post3/types_aiobotocore_arc_zonal_shift.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      965 2023-08-04 12:37:18.000000 types-aiobotocore-arc-zonal-shift-2.5.2.post3/types_aiobotocore_arc_zonal_shift.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 12:37:18.000000 types-aiobotocore-arc-zonal-shift-2.5.2.post3/types_aiobotocore_arc_zonal_shift.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 12:37:18.000000 types-aiobotocore-arc-zonal-shift-2.5.2.post3/types_aiobotocore_arc_zonal_shift.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-04 12:37:18.000000 types-aiobotocore-arc-zonal-shift-2.5.2.post3/types_aiobotocore_arc_zonal_shift.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-08-04 12:37:18.000000 types-aiobotocore-arc-zonal-shift-2.5.2.post3/types_aiobotocore_arc_zonal_shift.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:23:19.898551 types-aiobotocore-arc-zonal-shift-2.5.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-08 01:06:26.000000 types-aiobotocore-arc-zonal-shift-2.5.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    13568 2023-08-08 01:23:19.898551 types-aiobotocore-arc-zonal-shift-2.5.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    12026 2023-08-08 01:06:26.000000 types-aiobotocore-arc-zonal-shift-2.5.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-08 01:23:19.898551 types-aiobotocore-arc-zonal-shift-2.5.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2120 2023-08-08 01:06:26.000000 types-aiobotocore-arc-zonal-shift-2.5.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:23:19.898551 types-aiobotocore-arc-zonal-shift-2.5.4/types_aiobotocore_arc_zonal_shift/
+-rw-r--r--   0 runner    (1001) docker     (123)      948 2023-08-08 01:06:26.000000 types-aiobotocore-arc-zonal-shift-2.5.4/types_aiobotocore_arc_zonal_shift/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      947 2023-08-08 01:06:26.000000 types-aiobotocore-arc-zonal-shift-2.5.4/types_aiobotocore_arc_zonal_shift/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      959 2023-08-08 01:06:26.000000 types-aiobotocore-arc-zonal-shift-2.5.4/types_aiobotocore_arc_zonal_shift/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9732 2023-08-08 01:06:26.000000 types-aiobotocore-arc-zonal-shift-2.5.4/types_aiobotocore_arc_zonal_shift/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9715 2023-08-08 01:06:26.000000 types-aiobotocore-arc-zonal-shift-2.5.4/types_aiobotocore_arc_zonal_shift/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8702 2023-08-08 01:06:26.000000 types-aiobotocore-arc-zonal-shift-2.5.4/types_aiobotocore_arc_zonal_shift/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8700 2023-08-08 01:06:26.000000 types-aiobotocore-arc-zonal-shift-2.5.4/types_aiobotocore_arc_zonal_shift/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     3352 2023-08-08 01:06:26.000000 types-aiobotocore-arc-zonal-shift-2.5.4/types_aiobotocore_arc_zonal_shift/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3348 2023-08-08 01:06:26.000000 types-aiobotocore-arc-zonal-shift-2.5.4/types_aiobotocore_arc_zonal_shift/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 01:06:26.000000 types-aiobotocore-arc-zonal-shift-2.5.4/types_aiobotocore_arc_zonal_shift/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     5866 2023-08-08 01:06:26.000000 types-aiobotocore-arc-zonal-shift-2.5.4/types_aiobotocore_arc_zonal_shift/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5861 2023-08-08 01:06:26.000000 types-aiobotocore-arc-zonal-shift-2.5.4/types_aiobotocore_arc_zonal_shift/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-08-08 01:06:26.000000 types-aiobotocore-arc-zonal-shift-2.5.4/types_aiobotocore_arc_zonal_shift/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:23:19.898551 types-aiobotocore-arc-zonal-shift-2.5.4/types_aiobotocore_arc_zonal_shift.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    13568 2023-08-08 01:23:19.000000 types-aiobotocore-arc-zonal-shift-2.5.4/types_aiobotocore_arc_zonal_shift.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      965 2023-08-08 01:23:19.000000 types-aiobotocore-arc-zonal-shift-2.5.4/types_aiobotocore_arc_zonal_shift.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 01:23:19.000000 types-aiobotocore-arc-zonal-shift-2.5.4/types_aiobotocore_arc_zonal_shift.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 01:23:19.000000 types-aiobotocore-arc-zonal-shift-2.5.4/types_aiobotocore_arc_zonal_shift.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-08 01:23:19.000000 types-aiobotocore-arc-zonal-shift-2.5.4/types_aiobotocore_arc_zonal_shift.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-08-08 01:23:19.000000 types-aiobotocore-arc-zonal-shift-2.5.4/types_aiobotocore_arc_zonal_shift.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-arc-zonal-shift-2.5.2.post3/LICENSE` & `types-aiobotocore-arc-zonal-shift-2.5.4/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-arc-zonal-shift-2.5.2.post3/PKG-INFO` & `types-aiobotocore-arc-zonal-shift-2.5.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-arc-zonal-shift
-Version: 2.5.2.post3
-Summary: Type annotations for aiobotocore.ARCZonalShift 2.5.2 service generated with mypy-boto3-builder 7.17.2
+Version: 2.5.4
+Summary: Type annotations for aiobotocore.ARCZonalShift 2.5.4 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_arc_zonal_shift/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-arc-zonal-shift.svg?color=blue)](https://pypi.org/project/types-aiobotocore-arc-zonal-shift)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_arc_zonal_shift/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-arc-zonal-shift)](https://pepy.tech/project/types-aiobotocore-arc-zonal-shift)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.ARCZonalShift 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/arc-zonal-shift.html#ARCZonalShift)
+[aiobotocore.ARCZonalShift 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/arc-zonal-shift.html#ARCZonalShift)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-arc-zonal-shift-2.5.2.post3/README.md` & `types-aiobotocore-arc-zonal-shift-2.5.4/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-arc-zonal-shift.svg?color=blue)](https://pypi.org/project/types-aiobotocore-arc-zonal-shift)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_arc_zonal_shift/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-arc-zonal-shift)](https://pepy.tech/project/types-aiobotocore-arc-zonal-shift)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.ARCZonalShift 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/arc-zonal-shift.html#ARCZonalShift)
+[aiobotocore.ARCZonalShift 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/arc-zonal-shift.html#ARCZonalShift)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-arc-zonal-shift-2.5.2.post3/setup.py` & `types-aiobotocore-arc-zonal-shift-2.5.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-arc-zonal-shift",
-    version="2.5.2.post3",
+    version="2.5.4",
     packages=["types_aiobotocore_arc_zonal_shift"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.ARCZonalShift 2.5.2 service generated with"
+        "Type annotations for aiobotocore.ARCZonalShift 2.5.4 service generated with"
         " mypy-boto3-builder 7.17.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
```

### Comparing `types-aiobotocore-arc-zonal-shift-2.5.2.post3/types_aiobotocore_arc_zonal_shift/__init__.py` & `types-aiobotocore-arc-zonal-shift-2.5.4/types_aiobotocore_arc_zonal_shift/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-arc-zonal-shift-2.5.2.post3/types_aiobotocore_arc_zonal_shift/__init__.pyi` & `types-aiobotocore-arc-zonal-shift-2.5.4/types_aiobotocore_arc_zonal_shift/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-arc-zonal-shift-2.5.2.post3/types_aiobotocore_arc_zonal_shift/__main__.py` & `types-aiobotocore-arc-zonal-shift-2.5.4/types_aiobotocore_arc_zonal_shift/__main__.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.ARCZonalShift 2.5.2\nVersion:        "
-        " 2.5.2.post3\nBuilder version: 7.17.2\nDocs:           "
+        "Type annotations for aiobotocore.ARCZonalShift 2.5.4\nVersion:         2.5.4\nBuilder"
+        " version: 7.17.2\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_arc_zonal_shift//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/arc-zonal-shift.html#ARCZonalShift\nOther"
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

### Comparing `types-aiobotocore-arc-zonal-shift-2.5.2.post3/types_aiobotocore_arc_zonal_shift/client.py` & `types-aiobotocore-arc-zonal-shift-2.5.4/types_aiobotocore_arc_zonal_shift/client.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-arc-zonal-shift-2.5.2.post3/types_aiobotocore_arc_zonal_shift/client.pyi` & `types-aiobotocore-arc-zonal-shift-2.5.4/types_aiobotocore_arc_zonal_shift/client.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-arc-zonal-shift-2.5.2.post3/types_aiobotocore_arc_zonal_shift/literals.py` & `types-aiobotocore-arc-zonal-shift-2.5.4/types_aiobotocore_arc_zonal_shift/literals.py`

 * *Files 1% similar despite different names*

```diff
@@ -48,14 +48,15 @@
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
@@ -151,14 +152,15 @@
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
@@ -237,26 +239,28 @@
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
@@ -418,14 +422,15 @@
     "eu-central-2",
     "eu-north-1",
     "eu-south-1",
     "eu-south-2",
     "eu-west-1",
     "eu-west-2",
     "eu-west-3",
+    "il-central-1",
     "me-central-1",
     "me-south-1",
     "sa-east-1",
     "us-east-1",
     "us-east-2",
     "us-west-1",
     "us-west-2",
```

### Comparing `types-aiobotocore-arc-zonal-shift-2.5.2.post3/types_aiobotocore_arc_zonal_shift/literals.pyi` & `types-aiobotocore-arc-zonal-shift-2.5.4/types_aiobotocore_arc_zonal_shift/literals.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -46,14 +46,15 @@
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
@@ -149,14 +150,15 @@
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
@@ -235,26 +237,28 @@
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
@@ -416,14 +420,15 @@
     "eu-central-2",
     "eu-north-1",
     "eu-south-1",
     "eu-south-2",
     "eu-west-1",
     "eu-west-2",
     "eu-west-3",
+    "il-central-1",
     "me-central-1",
     "me-south-1",
     "sa-east-1",
     "us-east-1",
     "us-east-2",
     "us-west-1",
     "us-west-2",
```

### Comparing `types-aiobotocore-arc-zonal-shift-2.5.2.post3/types_aiobotocore_arc_zonal_shift/paginator.py` & `types-aiobotocore-arc-zonal-shift-2.5.4/types_aiobotocore_arc_zonal_shift/paginator.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-arc-zonal-shift-2.5.2.post3/types_aiobotocore_arc_zonal_shift/paginator.pyi` & `types-aiobotocore-arc-zonal-shift-2.5.4/types_aiobotocore_arc_zonal_shift/paginator.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-arc-zonal-shift-2.5.2.post3/types_aiobotocore_arc_zonal_shift/type_defs.py` & `types-aiobotocore-arc-zonal-shift-2.5.4/types_aiobotocore_arc_zonal_shift/type_defs.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-arc-zonal-shift-2.5.2.post3/types_aiobotocore_arc_zonal_shift/type_defs.pyi` & `types-aiobotocore-arc-zonal-shift-2.5.4/types_aiobotocore_arc_zonal_shift/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-arc-zonal-shift-2.5.2.post3/types_aiobotocore_arc_zonal_shift.egg-info/PKG-INFO` & `types-aiobotocore-arc-zonal-shift-2.5.4/types_aiobotocore_arc_zonal_shift.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-arc-zonal-shift
-Version: 2.5.2.post3
-Summary: Type annotations for aiobotocore.ARCZonalShift 2.5.2 service generated with mypy-boto3-builder 7.17.2
+Version: 2.5.4
+Summary: Type annotations for aiobotocore.ARCZonalShift 2.5.4 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_arc_zonal_shift/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-arc-zonal-shift.svg?color=blue)](https://pypi.org/project/types-aiobotocore-arc-zonal-shift)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_arc_zonal_shift/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-arc-zonal-shift)](https://pepy.tech/project/types-aiobotocore-arc-zonal-shift)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.ARCZonalShift 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/arc-zonal-shift.html#ARCZonalShift)
+[aiobotocore.ARCZonalShift 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/arc-zonal-shift.html#ARCZonalShift)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-arc-zonal-shift-2.5.2.post3/types_aiobotocore_arc_zonal_shift.egg-info/SOURCES.txt` & `types-aiobotocore-arc-zonal-shift-2.5.4/types_aiobotocore_arc_zonal_shift.egg-info/SOURCES.txt`

 * *Files identical despite different names*


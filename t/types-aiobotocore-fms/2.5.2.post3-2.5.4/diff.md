# Comparing `tmp/types-aiobotocore-fms-2.5.2.post3.tar.gz` & `tmp/types-aiobotocore-fms-2.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-fms-2.5.2.post3.tar", last modified: Fri Aug  4 12:37:44 2023, max compression
+gzip compressed data, was "types-aiobotocore-fms-2.5.4.tar", last modified: Tue Aug  8 01:23:45 2023, max compression
```

## Comparing `types-aiobotocore-fms-2.5.2.post3.tar` & `types-aiobotocore-fms-2.5.4.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:37:44.523830 types-aiobotocore-fms-2.5.2.post3/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-04 12:23:50.000000 types-aiobotocore-fms-2.5.2.post3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    13924 2023-08-04 12:37:44.507830 types-aiobotocore-fms-2.5.2.post3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    12422 2023-08-04 12:23:50.000000 types-aiobotocore-fms-2.5.2.post3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-04 12:37:44.523830 types-aiobotocore-fms-2.5.2.post3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2020 2023-08-04 12:23:50.000000 types-aiobotocore-fms-2.5.2.post3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:37:44.507830 types-aiobotocore-fms-2.5.2.post3/types_aiobotocore_fms/
--rw-r--r--   0 runner    (1001) docker     (123)     2379 2023-08-04 12:23:50.000000 types-aiobotocore-fms-2.5.2.post3/types_aiobotocore_fms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2378 2023-08-04 12:23:50.000000 types-aiobotocore-fms-2.5.2.post3/types_aiobotocore_fms/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      916 2023-08-04 12:23:50.000000 types-aiobotocore-fms-2.5.2.post3/types_aiobotocore_fms/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    32946 2023-08-04 12:23:50.000000 types-aiobotocore-fms-2.5.2.post3/types_aiobotocore_fms/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    32887 2023-08-04 12:23:50.000000 types-aiobotocore-fms-2.5.2.post3/types_aiobotocore_fms/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    12999 2023-08-04 12:23:52.000000 types-aiobotocore-fms-2.5.2.post3/types_aiobotocore_fms/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    12997 2023-08-04 12:23:52.000000 types-aiobotocore-fms-2.5.2.post3/types_aiobotocore_fms/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    10158 2023-08-04 12:23:50.000000 types-aiobotocore-fms-2.5.2.post3/types_aiobotocore_fms/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)    10148 2023-08-04 12:23:50.000000 types-aiobotocore-fms-2.5.2.post3/types_aiobotocore_fms/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 12:23:50.000000 types-aiobotocore-fms-2.5.2.post3/types_aiobotocore_fms/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    59427 2023-08-04 12:23:53.000000 types-aiobotocore-fms-2.5.2.post3/types_aiobotocore_fms/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    59360 2023-08-04 12:23:53.000000 types-aiobotocore-fms-2.5.2.post3/types_aiobotocore_fms/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-04 12:23:50.000000 types-aiobotocore-fms-2.5.2.post3/types_aiobotocore_fms/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:37:44.507830 types-aiobotocore-fms-2.5.2.post3/types_aiobotocore_fms.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    13924 2023-08-04 12:37:44.000000 types-aiobotocore-fms-2.5.2.post3/types_aiobotocore_fms.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      737 2023-08-04 12:37:44.000000 types-aiobotocore-fms-2.5.2.post3/types_aiobotocore_fms.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 12:37:44.000000 types-aiobotocore-fms-2.5.2.post3/types_aiobotocore_fms.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 12:37:44.000000 types-aiobotocore-fms-2.5.2.post3/types_aiobotocore_fms.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-04 12:37:44.000000 types-aiobotocore-fms-2.5.2.post3/types_aiobotocore_fms.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-08-04 12:37:44.000000 types-aiobotocore-fms-2.5.2.post3/types_aiobotocore_fms.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:23:45.218719 types-aiobotocore-fms-2.5.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-08 01:11:15.000000 types-aiobotocore-fms-2.5.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    13918 2023-08-08 01:23:45.218719 types-aiobotocore-fms-2.5.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    12422 2023-08-08 01:11:15.000000 types-aiobotocore-fms-2.5.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-08 01:23:45.218719 types-aiobotocore-fms-2.5.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2014 2023-08-08 01:11:15.000000 types-aiobotocore-fms-2.5.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:23:45.214719 types-aiobotocore-fms-2.5.4/types_aiobotocore_fms/
+-rw-r--r--   0 runner    (1001) docker     (123)     2379 2023-08-08 01:11:15.000000 types-aiobotocore-fms-2.5.4/types_aiobotocore_fms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2378 2023-08-08 01:11:15.000000 types-aiobotocore-fms-2.5.4/types_aiobotocore_fms/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      904 2023-08-08 01:11:15.000000 types-aiobotocore-fms-2.5.4/types_aiobotocore_fms/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32946 2023-08-08 01:11:16.000000 types-aiobotocore-fms-2.5.4/types_aiobotocore_fms/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32887 2023-08-08 01:11:15.000000 types-aiobotocore-fms-2.5.4/types_aiobotocore_fms/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    13094 2023-08-08 01:11:17.000000 types-aiobotocore-fms-2.5.4/types_aiobotocore_fms/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13092 2023-08-08 01:11:16.000000 types-aiobotocore-fms-2.5.4/types_aiobotocore_fms/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    10158 2023-08-08 01:11:16.000000 types-aiobotocore-fms-2.5.4/types_aiobotocore_fms/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10148 2023-08-08 01:11:16.000000 types-aiobotocore-fms-2.5.4/types_aiobotocore_fms/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 01:11:15.000000 types-aiobotocore-fms-2.5.4/types_aiobotocore_fms/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    59427 2023-08-08 01:11:18.000000 types-aiobotocore-fms-2.5.4/types_aiobotocore_fms/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    59360 2023-08-08 01:11:17.000000 types-aiobotocore-fms-2.5.4/types_aiobotocore_fms/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-08-08 01:11:15.000000 types-aiobotocore-fms-2.5.4/types_aiobotocore_fms/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:23:45.218719 types-aiobotocore-fms-2.5.4/types_aiobotocore_fms.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    13918 2023-08-08 01:23:45.000000 types-aiobotocore-fms-2.5.4/types_aiobotocore_fms.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      737 2023-08-08 01:23:45.000000 types-aiobotocore-fms-2.5.4/types_aiobotocore_fms.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 01:23:45.000000 types-aiobotocore-fms-2.5.4/types_aiobotocore_fms.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 01:23:45.000000 types-aiobotocore-fms-2.5.4/types_aiobotocore_fms.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-08 01:23:45.000000 types-aiobotocore-fms-2.5.4/types_aiobotocore_fms.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-08-08 01:23:45.000000 types-aiobotocore-fms-2.5.4/types_aiobotocore_fms.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-fms-2.5.2.post3/LICENSE` & `types-aiobotocore-fms-2.5.4/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-fms-2.5.2.post3/PKG-INFO` & `types-aiobotocore-fms-2.5.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-fms
-Version: 2.5.2.post3
-Summary: Type annotations for aiobotocore.FMS 2.5.2 service generated with mypy-boto3-builder 7.17.2
+Version: 2.5.4
+Summary: Type annotations for aiobotocore.FMS 2.5.4 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_fms/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-fms.svg?color=blue)](https://pypi.org/project/types-aiobotocore-fms)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_fms/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-fms)](https://pepy.tech/project/types-aiobotocore-fms)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.FMS 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fms.html#FMS)
+[aiobotocore.FMS 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fms.html#FMS)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-fms-2.5.2.post3/README.md` & `types-aiobotocore-fms-2.5.4/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-fms.svg?color=blue)](https://pypi.org/project/types-aiobotocore-fms)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_fms/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-fms)](https://pepy.tech/project/types-aiobotocore-fms)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.FMS 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fms.html#FMS)
+[aiobotocore.FMS 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fms.html#FMS)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-fms-2.5.2.post3/setup.py` & `types-aiobotocore-fms-2.5.4/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-fms",
-    version="2.5.2.post3",
+    version="2.5.4",
     packages=["types_aiobotocore_fms"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.FMS 2.5.2 service generated with mypy-boto3-builder"
+        "Type annotations for aiobotocore.FMS 2.5.4 service generated with mypy-boto3-builder"
         " 7.17.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
```

### Comparing `types-aiobotocore-fms-2.5.2.post3/types_aiobotocore_fms/__init__.py` & `types-aiobotocore-fms-2.5.4/types_aiobotocore_fms/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-fms-2.5.2.post3/types_aiobotocore_fms/__init__.pyi` & `types-aiobotocore-fms-2.5.4/types_aiobotocore_fms/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-fms-2.5.2.post3/types_aiobotocore_fms/__main__.py` & `types-aiobotocore-fms-2.5.4/types_aiobotocore_fms/__main__.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.FMS 2.5.2\nVersion:         2.5.2.post3\nBuilder version:"
+        "Type annotations for aiobotocore.FMS 2.5.4\nVersion:         2.5.4\nBuilder version:"
         " 7.17.2\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_fms//\nBoto3 docs:    "
         "  https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fms.html#FMS\nOther"
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

### Comparing `types-aiobotocore-fms-2.5.2.post3/types_aiobotocore_fms/client.py` & `types-aiobotocore-fms-2.5.4/types_aiobotocore_fms/client.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-fms-2.5.2.post3/types_aiobotocore_fms/client.pyi` & `types-aiobotocore-fms-2.5.4/types_aiobotocore_fms/client.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-fms-2.5.2.post3/types_aiobotocore_fms/literals.py` & `types-aiobotocore-fms-2.5.4/types_aiobotocore_fms/literals.py`

 * *Files 1% similar despite different names*

```diff
@@ -158,14 +158,15 @@
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
@@ -261,14 +262,15 @@
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
@@ -347,26 +349,28 @@
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

### Comparing `types-aiobotocore-fms-2.5.2.post3/types_aiobotocore_fms/literals.pyi` & `types-aiobotocore-fms-2.5.4/types_aiobotocore_fms/literals.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -156,14 +156,15 @@
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
@@ -259,14 +260,15 @@
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
@@ -345,26 +347,28 @@
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

### Comparing `types-aiobotocore-fms-2.5.2.post3/types_aiobotocore_fms/paginator.py` & `types-aiobotocore-fms-2.5.4/types_aiobotocore_fms/paginator.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-fms-2.5.2.post3/types_aiobotocore_fms/paginator.pyi` & `types-aiobotocore-fms-2.5.4/types_aiobotocore_fms/paginator.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-fms-2.5.2.post3/types_aiobotocore_fms/type_defs.py` & `types-aiobotocore-fms-2.5.4/types_aiobotocore_fms/type_defs.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-fms-2.5.2.post3/types_aiobotocore_fms/type_defs.pyi` & `types-aiobotocore-fms-2.5.4/types_aiobotocore_fms/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-fms-2.5.2.post3/types_aiobotocore_fms.egg-info/PKG-INFO` & `types-aiobotocore-fms-2.5.4/types_aiobotocore_fms.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-fms
-Version: 2.5.2.post3
-Summary: Type annotations for aiobotocore.FMS 2.5.2 service generated with mypy-boto3-builder 7.17.2
+Version: 2.5.4
+Summary: Type annotations for aiobotocore.FMS 2.5.4 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_fms/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-fms.svg?color=blue)](https://pypi.org/project/types-aiobotocore-fms)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_fms/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-fms)](https://pepy.tech/project/types-aiobotocore-fms)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.FMS 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fms.html#FMS)
+[aiobotocore.FMS 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fms.html#FMS)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-fms-2.5.2.post3/types_aiobotocore_fms.egg-info/SOURCES.txt` & `types-aiobotocore-fms-2.5.4/types_aiobotocore_fms.egg-info/SOURCES.txt`

 * *Files identical despite different names*


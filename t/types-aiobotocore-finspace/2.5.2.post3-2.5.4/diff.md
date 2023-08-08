# Comparing `tmp/types-aiobotocore-finspace-2.5.2.post3.tar.gz` & `tmp/types-aiobotocore-finspace-2.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-finspace-2.5.2.post3.tar", last modified: Fri Aug  4 12:37:43 2023, max compression
+gzip compressed data, was "types-aiobotocore-finspace-2.5.4.tar", last modified: Tue Aug  8 01:23:43 2023, max compression
```

## Comparing `types-aiobotocore-finspace-2.5.2.post3.tar` & `types-aiobotocore-finspace-2.5.4.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:37:43.967817 types-aiobotocore-finspace-2.5.2.post3/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-04 12:23:42.000000 types-aiobotocore-finspace-2.5.2.post3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    13016 2023-08-04 12:37:43.959817 types-aiobotocore-finspace-2.5.2.post3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    11494 2023-08-04 12:23:42.000000 types-aiobotocore-finspace-2.5.2.post3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-04 12:37:43.967817 types-aiobotocore-finspace-2.5.2.post3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2079 2023-08-04 12:23:42.000000 types-aiobotocore-finspace-2.5.2.post3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:37:43.955817 types-aiobotocore-finspace-2.5.2.post3/types_aiobotocore_finspace/
--rw-r--r--   0 runner    (1001) docker     (123)      681 2023-08-04 12:23:42.000000 types-aiobotocore-finspace-2.5.2.post3/types_aiobotocore_finspace/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      680 2023-08-04 12:23:42.000000 types-aiobotocore-finspace-2.5.2.post3/types_aiobotocore_finspace/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      947 2023-08-04 12:23:42.000000 types-aiobotocore-finspace-2.5.2.post3/types_aiobotocore_finspace/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    26541 2023-08-04 12:23:43.000000 types-aiobotocore-finspace-2.5.2.post3/types_aiobotocore_finspace/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    26497 2023-08-04 12:23:43.000000 types-aiobotocore-finspace-2.5.2.post3/types_aiobotocore_finspace/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9697 2023-08-04 12:23:43.000000 types-aiobotocore-finspace-2.5.2.post3/types_aiobotocore_finspace/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     9695 2023-08-04 12:23:43.000000 types-aiobotocore-finspace-2.5.2.post3/types_aiobotocore_finspace/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2042 2023-08-04 12:23:43.000000 types-aiobotocore-finspace-2.5.2.post3/types_aiobotocore_finspace/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     2039 2023-08-04 12:23:43.000000 types-aiobotocore-finspace-2.5.2.post3/types_aiobotocore_finspace/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 12:23:42.000000 types-aiobotocore-finspace-2.5.2.post3/types_aiobotocore_finspace/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    34891 2023-08-04 12:23:44.000000 types-aiobotocore-finspace-2.5.2.post3/types_aiobotocore_finspace/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    34853 2023-08-04 12:23:43.000000 types-aiobotocore-finspace-2.5.2.post3/types_aiobotocore_finspace/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-04 12:23:42.000000 types-aiobotocore-finspace-2.5.2.post3/types_aiobotocore_finspace/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:37:43.955817 types-aiobotocore-finspace-2.5.2.post3/types_aiobotocore_finspace.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    13016 2023-08-04 12:37:43.000000 types-aiobotocore-finspace-2.5.2.post3/types_aiobotocore_finspace.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      832 2023-08-04 12:37:43.000000 types-aiobotocore-finspace-2.5.2.post3/types_aiobotocore_finspace.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 12:37:43.000000 types-aiobotocore-finspace-2.5.2.post3/types_aiobotocore_finspace.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 12:37:43.000000 types-aiobotocore-finspace-2.5.2.post3/types_aiobotocore_finspace.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-04 12:37:43.000000 types-aiobotocore-finspace-2.5.2.post3/types_aiobotocore_finspace.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-08-04 12:37:43.000000 types-aiobotocore-finspace-2.5.2.post3/types_aiobotocore_finspace.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:23:43.886716 types-aiobotocore-finspace-2.5.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-08 01:11:08.000000 types-aiobotocore-finspace-2.5.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    13010 2023-08-08 01:23:43.886716 types-aiobotocore-finspace-2.5.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    11494 2023-08-08 01:11:08.000000 types-aiobotocore-finspace-2.5.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-08 01:23:43.886716 types-aiobotocore-finspace-2.5.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2073 2023-08-08 01:11:08.000000 types-aiobotocore-finspace-2.5.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:23:43.886716 types-aiobotocore-finspace-2.5.4/types_aiobotocore_finspace/
+-rw-r--r--   0 runner    (1001) docker     (123)      681 2023-08-08 01:11:08.000000 types-aiobotocore-finspace-2.5.4/types_aiobotocore_finspace/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      680 2023-08-08 01:11:08.000000 types-aiobotocore-finspace-2.5.4/types_aiobotocore_finspace/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      935 2023-08-08 01:11:08.000000 types-aiobotocore-finspace-2.5.4/types_aiobotocore_finspace/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26541 2023-08-08 01:11:08.000000 types-aiobotocore-finspace-2.5.4/types_aiobotocore_finspace/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26497 2023-08-08 01:11:08.000000 types-aiobotocore-finspace-2.5.4/types_aiobotocore_finspace/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9792 2023-08-08 01:11:08.000000 types-aiobotocore-finspace-2.5.4/types_aiobotocore_finspace/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9790 2023-08-08 01:11:08.000000 types-aiobotocore-finspace-2.5.4/types_aiobotocore_finspace/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2042 2023-08-08 01:11:08.000000 types-aiobotocore-finspace-2.5.4/types_aiobotocore_finspace/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2039 2023-08-08 01:11:08.000000 types-aiobotocore-finspace-2.5.4/types_aiobotocore_finspace/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 01:11:08.000000 types-aiobotocore-finspace-2.5.4/types_aiobotocore_finspace/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    34891 2023-08-08 01:11:09.000000 types-aiobotocore-finspace-2.5.4/types_aiobotocore_finspace/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34853 2023-08-08 01:11:08.000000 types-aiobotocore-finspace-2.5.4/types_aiobotocore_finspace/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-08-08 01:11:08.000000 types-aiobotocore-finspace-2.5.4/types_aiobotocore_finspace/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:23:43.886716 types-aiobotocore-finspace-2.5.4/types_aiobotocore_finspace.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    13010 2023-08-08 01:23:43.000000 types-aiobotocore-finspace-2.5.4/types_aiobotocore_finspace.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      832 2023-08-08 01:23:43.000000 types-aiobotocore-finspace-2.5.4/types_aiobotocore_finspace.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 01:23:43.000000 types-aiobotocore-finspace-2.5.4/types_aiobotocore_finspace.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 01:23:43.000000 types-aiobotocore-finspace-2.5.4/types_aiobotocore_finspace.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-08 01:23:43.000000 types-aiobotocore-finspace-2.5.4/types_aiobotocore_finspace.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-08-08 01:23:43.000000 types-aiobotocore-finspace-2.5.4/types_aiobotocore_finspace.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-finspace-2.5.2.post3/LICENSE` & `types-aiobotocore-finspace-2.5.4/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-finspace-2.5.2.post3/PKG-INFO` & `types-aiobotocore-finspace-2.5.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-finspace
-Version: 2.5.2.post3
-Summary: Type annotations for aiobotocore.finspace 2.5.2 service generated with mypy-boto3-builder 7.17.2
+Version: 2.5.4
+Summary: Type annotations for aiobotocore.finspace 2.5.4 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_finspace/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-finspace.svg?color=blue)](https://pypi.org/project/types-aiobotocore-finspace)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_finspace/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-finspace)](https://pepy.tech/project/types-aiobotocore-finspace)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.finspace 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/finspace.html#finspace)
+[aiobotocore.finspace 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/finspace.html#finspace)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-finspace-2.5.2.post3/README.md` & `types-aiobotocore-finspace-2.5.4/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-finspace.svg?color=blue)](https://pypi.org/project/types-aiobotocore-finspace)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_finspace/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-finspace)](https://pepy.tech/project/types-aiobotocore-finspace)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.finspace 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/finspace.html#finspace)
+[aiobotocore.finspace 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/finspace.html#finspace)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-finspace-2.5.2.post3/setup.py` & `types-aiobotocore-finspace-2.5.4/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-finspace",
-    version="2.5.2.post3",
+    version="2.5.4",
     packages=["types_aiobotocore_finspace"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.finspace 2.5.2 service generated with mypy-boto3-builder"
+        "Type annotations for aiobotocore.finspace 2.5.4 service generated with mypy-boto3-builder"
         " 7.17.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
```

### Comparing `types-aiobotocore-finspace-2.5.2.post3/types_aiobotocore_finspace/__init__.py` & `types-aiobotocore-finspace-2.5.4/types_aiobotocore_finspace/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-finspace-2.5.2.post3/types_aiobotocore_finspace/__init__.pyi` & `types-aiobotocore-finspace-2.5.4/types_aiobotocore_finspace/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-finspace-2.5.2.post3/types_aiobotocore_finspace/__main__.py` & `types-aiobotocore-finspace-2.5.4/types_aiobotocore_finspace/__main__.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.finspace 2.5.2\nVersion:         2.5.2.post3\nBuilder"
-        " version: 7.17.2\nDocs:           "
+        "Type annotations for aiobotocore.finspace 2.5.4\nVersion:         2.5.4\nBuilder version:"
+        " 7.17.2\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_finspace//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/finspace.html#finspace\nOther"
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

### Comparing `types-aiobotocore-finspace-2.5.2.post3/types_aiobotocore_finspace/client.py` & `types-aiobotocore-finspace-2.5.4/types_aiobotocore_finspace/client.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-finspace-2.5.2.post3/types_aiobotocore_finspace/client.pyi` & `types-aiobotocore-finspace-2.5.4/types_aiobotocore_finspace/client.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-finspace-2.5.2.post3/types_aiobotocore_finspace/literals.py` & `types-aiobotocore-finspace-2.5.4/types_aiobotocore_finspace/literals.py`

 * *Files 0% similar despite different names*

```diff
@@ -104,14 +104,15 @@
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
@@ -207,14 +208,15 @@
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
@@ -293,26 +295,28 @@
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

### Comparing `types-aiobotocore-finspace-2.5.2.post3/types_aiobotocore_finspace/literals.pyi` & `types-aiobotocore-finspace-2.5.4/types_aiobotocore_finspace/literals.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -102,14 +102,15 @@
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
@@ -205,14 +206,15 @@
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
@@ -291,26 +293,28 @@
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

### Comparing `types-aiobotocore-finspace-2.5.2.post3/types_aiobotocore_finspace/paginator.py` & `types-aiobotocore-finspace-2.5.4/types_aiobotocore_finspace/paginator.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-finspace-2.5.2.post3/types_aiobotocore_finspace/paginator.pyi` & `types-aiobotocore-finspace-2.5.4/types_aiobotocore_finspace/paginator.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-finspace-2.5.2.post3/types_aiobotocore_finspace/type_defs.py` & `types-aiobotocore-finspace-2.5.4/types_aiobotocore_finspace/type_defs.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-finspace-2.5.2.post3/types_aiobotocore_finspace/type_defs.pyi` & `types-aiobotocore-finspace-2.5.4/types_aiobotocore_finspace/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-finspace-2.5.2.post3/types_aiobotocore_finspace.egg-info/PKG-INFO` & `types-aiobotocore-finspace-2.5.4/types_aiobotocore_finspace.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-finspace
-Version: 2.5.2.post3
-Summary: Type annotations for aiobotocore.finspace 2.5.2 service generated with mypy-boto3-builder 7.17.2
+Version: 2.5.4
+Summary: Type annotations for aiobotocore.finspace 2.5.4 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_finspace/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-finspace.svg?color=blue)](https://pypi.org/project/types-aiobotocore-finspace)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_finspace/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-finspace)](https://pepy.tech/project/types-aiobotocore-finspace)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.finspace 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/finspace.html#finspace)
+[aiobotocore.finspace 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/finspace.html#finspace)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-finspace-2.5.2.post3/types_aiobotocore_finspace.egg-info/SOURCES.txt` & `types-aiobotocore-finspace-2.5.4/types_aiobotocore_finspace.egg-info/SOURCES.txt`

 * *Files identical despite different names*


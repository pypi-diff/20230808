# Comparing `tmp/types-aiobotocore-dataexchange-2.5.2.post3.tar.gz` & `tmp/types-aiobotocore-dataexchange-2.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-dataexchange-2.5.2.post3.tar", last modified: Fri Aug  4 12:37:34 2023, max compression
+gzip compressed data, was "types-aiobotocore-dataexchange-2.5.4.tar", last modified: Tue Aug  8 01:23:34 2023, max compression
```

## Comparing `types-aiobotocore-dataexchange-2.5.2.post3.tar` & `types-aiobotocore-dataexchange-2.5.4.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:37:34.227588 types-aiobotocore-dataexchange-2.5.2.post3/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-04 12:21:11.000000 types-aiobotocore-dataexchange-2.5.2.post3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    13773 2023-08-04 12:37:34.223588 types-aiobotocore-dataexchange-2.5.2.post3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    12235 2023-08-04 12:21:11.000000 types-aiobotocore-dataexchange-2.5.2.post3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-04 12:37:34.227588 types-aiobotocore-dataexchange-2.5.2.post3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2107 2023-08-04 12:21:11.000000 types-aiobotocore-dataexchange-2.5.2.post3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:37:34.223588 types-aiobotocore-dataexchange-2.5.2.post3/types_aiobotocore_dataexchange/
--rw-r--r--   0 runner    (1001) docker     (123)     1505 2023-08-04 12:21:11.000000 types-aiobotocore-dataexchange-2.5.2.post3/types_aiobotocore_dataexchange/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1504 2023-08-04 12:21:11.000000 types-aiobotocore-dataexchange-2.5.2.post3/types_aiobotocore_dataexchange/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      963 2023-08-04 12:21:11.000000 types-aiobotocore-dataexchange-2.5.2.post3/types_aiobotocore_dataexchange/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    23279 2023-08-04 12:21:11.000000 types-aiobotocore-dataexchange-2.5.2.post3/types_aiobotocore_dataexchange/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    23236 2023-08-04 12:21:11.000000 types-aiobotocore-dataexchange-2.5.2.post3/types_aiobotocore_dataexchange/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    10429 2023-08-04 12:21:11.000000 types-aiobotocore-dataexchange-2.5.2.post3/types_aiobotocore_dataexchange/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    10427 2023-08-04 12:21:11.000000 types-aiobotocore-dataexchange-2.5.2.post3/types_aiobotocore_dataexchange/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     6644 2023-08-04 12:21:11.000000 types-aiobotocore-dataexchange-2.5.2.post3/types_aiobotocore_dataexchange/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     6637 2023-08-04 12:21:11.000000 types-aiobotocore-dataexchange-2.5.2.post3/types_aiobotocore_dataexchange/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 12:21:11.000000 types-aiobotocore-dataexchange-2.5.2.post3/types_aiobotocore_dataexchange/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    45176 2023-08-04 12:21:12.000000 types-aiobotocore-dataexchange-2.5.2.post3/types_aiobotocore_dataexchange/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    45109 2023-08-04 12:21:12.000000 types-aiobotocore-dataexchange-2.5.2.post3/types_aiobotocore_dataexchange/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-04 12:21:11.000000 types-aiobotocore-dataexchange-2.5.2.post3/types_aiobotocore_dataexchange/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:37:34.223588 types-aiobotocore-dataexchange-2.5.2.post3/types_aiobotocore_dataexchange.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    13773 2023-08-04 12:37:34.000000 types-aiobotocore-dataexchange-2.5.2.post3/types_aiobotocore_dataexchange.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      908 2023-08-04 12:37:34.000000 types-aiobotocore-dataexchange-2.5.2.post3/types_aiobotocore_dataexchange.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 12:37:34.000000 types-aiobotocore-dataexchange-2.5.2.post3/types_aiobotocore_dataexchange.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 12:37:34.000000 types-aiobotocore-dataexchange-2.5.2.post3/types_aiobotocore_dataexchange.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-04 12:37:34.000000 types-aiobotocore-dataexchange-2.5.2.post3/types_aiobotocore_dataexchange.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-08-04 12:37:34.000000 types-aiobotocore-dataexchange-2.5.2.post3/types_aiobotocore_dataexchange.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:23:34.154677 types-aiobotocore-dataexchange-2.5.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-08 01:08:46.000000 types-aiobotocore-dataexchange-2.5.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    13767 2023-08-08 01:23:34.150677 types-aiobotocore-dataexchange-2.5.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    12235 2023-08-08 01:08:46.000000 types-aiobotocore-dataexchange-2.5.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-08 01:23:34.154677 types-aiobotocore-dataexchange-2.5.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2101 2023-08-08 01:08:46.000000 types-aiobotocore-dataexchange-2.5.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:23:34.146677 types-aiobotocore-dataexchange-2.5.4/types_aiobotocore_dataexchange/
+-rw-r--r--   0 runner    (1001) docker     (123)     1505 2023-08-08 01:08:46.000000 types-aiobotocore-dataexchange-2.5.4/types_aiobotocore_dataexchange/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1504 2023-08-08 01:08:46.000000 types-aiobotocore-dataexchange-2.5.4/types_aiobotocore_dataexchange/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      951 2023-08-08 01:08:46.000000 types-aiobotocore-dataexchange-2.5.4/types_aiobotocore_dataexchange/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23279 2023-08-08 01:08:46.000000 types-aiobotocore-dataexchange-2.5.4/types_aiobotocore_dataexchange/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23236 2023-08-08 01:08:46.000000 types-aiobotocore-dataexchange-2.5.4/types_aiobotocore_dataexchange/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    10524 2023-08-08 01:08:47.000000 types-aiobotocore-dataexchange-2.5.4/types_aiobotocore_dataexchange/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10522 2023-08-08 01:08:46.000000 types-aiobotocore-dataexchange-2.5.4/types_aiobotocore_dataexchange/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     6644 2023-08-08 01:08:46.000000 types-aiobotocore-dataexchange-2.5.4/types_aiobotocore_dataexchange/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6637 2023-08-08 01:08:46.000000 types-aiobotocore-dataexchange-2.5.4/types_aiobotocore_dataexchange/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 01:08:46.000000 types-aiobotocore-dataexchange-2.5.4/types_aiobotocore_dataexchange/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    45176 2023-08-08 01:08:48.000000 types-aiobotocore-dataexchange-2.5.4/types_aiobotocore_dataexchange/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    45109 2023-08-08 01:08:48.000000 types-aiobotocore-dataexchange-2.5.4/types_aiobotocore_dataexchange/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-08-08 01:08:46.000000 types-aiobotocore-dataexchange-2.5.4/types_aiobotocore_dataexchange/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:23:34.150677 types-aiobotocore-dataexchange-2.5.4/types_aiobotocore_dataexchange.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    13767 2023-08-08 01:23:33.000000 types-aiobotocore-dataexchange-2.5.4/types_aiobotocore_dataexchange.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      908 2023-08-08 01:23:34.000000 types-aiobotocore-dataexchange-2.5.4/types_aiobotocore_dataexchange.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 01:23:33.000000 types-aiobotocore-dataexchange-2.5.4/types_aiobotocore_dataexchange.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 01:23:33.000000 types-aiobotocore-dataexchange-2.5.4/types_aiobotocore_dataexchange.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-08 01:23:33.000000 types-aiobotocore-dataexchange-2.5.4/types_aiobotocore_dataexchange.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-08-08 01:23:33.000000 types-aiobotocore-dataexchange-2.5.4/types_aiobotocore_dataexchange.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-dataexchange-2.5.2.post3/LICENSE` & `types-aiobotocore-dataexchange-2.5.4/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-dataexchange-2.5.2.post3/PKG-INFO` & `types-aiobotocore-dataexchange-2.5.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-dataexchange
-Version: 2.5.2.post3
-Summary: Type annotations for aiobotocore.DataExchange 2.5.2 service generated with mypy-boto3-builder 7.17.2
+Version: 2.5.4
+Summary: Type annotations for aiobotocore.DataExchange 2.5.4 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dataexchange/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-dataexchange.svg?color=blue)](https://pypi.org/project/types-aiobotocore-dataexchange)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dataexchange/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-dataexchange)](https://pepy.tech/project/types-aiobotocore-dataexchange)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.DataExchange 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dataexchange.html#DataExchange)
+[aiobotocore.DataExchange 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dataexchange.html#DataExchange)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-dataexchange-2.5.2.post3/README.md` & `types-aiobotocore-dataexchange-2.5.4/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-dataexchange.svg?color=blue)](https://pypi.org/project/types-aiobotocore-dataexchange)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dataexchange/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-dataexchange)](https://pepy.tech/project/types-aiobotocore-dataexchange)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.DataExchange 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dataexchange.html#DataExchange)
+[aiobotocore.DataExchange 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dataexchange.html#DataExchange)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-dataexchange-2.5.2.post3/setup.py` & `types-aiobotocore-dataexchange-2.5.4/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-dataexchange",
-    version="2.5.2.post3",
+    version="2.5.4",
     packages=["types_aiobotocore_dataexchange"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.DataExchange 2.5.2 service generated with"
+        "Type annotations for aiobotocore.DataExchange 2.5.4 service generated with"
         " mypy-boto3-builder 7.17.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
```

### Comparing `types-aiobotocore-dataexchange-2.5.2.post3/types_aiobotocore_dataexchange/__init__.py` & `types-aiobotocore-dataexchange-2.5.4/types_aiobotocore_dataexchange/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-dataexchange-2.5.2.post3/types_aiobotocore_dataexchange/__init__.pyi` & `types-aiobotocore-dataexchange-2.5.4/types_aiobotocore_dataexchange/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-dataexchange-2.5.2.post3/types_aiobotocore_dataexchange/__main__.py` & `types-aiobotocore-dataexchange-2.5.4/types_aiobotocore_dataexchange/__main__.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.DataExchange 2.5.2\nVersion:         2.5.2.post3\nBuilder"
+        "Type annotations for aiobotocore.DataExchange 2.5.4\nVersion:         2.5.4\nBuilder"
         " version: 7.17.2\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dataexchange//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dataexchange.html#DataExchange\nOther"
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

### Comparing `types-aiobotocore-dataexchange-2.5.2.post3/types_aiobotocore_dataexchange/client.py` & `types-aiobotocore-dataexchange-2.5.4/types_aiobotocore_dataexchange/client.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-dataexchange-2.5.2.post3/types_aiobotocore_dataexchange/client.pyi` & `types-aiobotocore-dataexchange-2.5.4/types_aiobotocore_dataexchange/client.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-dataexchange-2.5.2.post3/types_aiobotocore_dataexchange/literals.py` & `types-aiobotocore-dataexchange-2.5.4/types_aiobotocore_dataexchange/literals.py`

 * *Files 1% similar despite different names*

```diff
@@ -108,14 +108,15 @@
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
@@ -211,14 +212,15 @@
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
@@ -297,26 +299,28 @@
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

### Comparing `types-aiobotocore-dataexchange-2.5.2.post3/types_aiobotocore_dataexchange/literals.pyi` & `types-aiobotocore-dataexchange-2.5.4/types_aiobotocore_dataexchange/literals.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -106,14 +106,15 @@
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
@@ -209,14 +210,15 @@
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
@@ -295,26 +297,28 @@
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

### Comparing `types-aiobotocore-dataexchange-2.5.2.post3/types_aiobotocore_dataexchange/paginator.py` & `types-aiobotocore-dataexchange-2.5.4/types_aiobotocore_dataexchange/paginator.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-dataexchange-2.5.2.post3/types_aiobotocore_dataexchange/paginator.pyi` & `types-aiobotocore-dataexchange-2.5.4/types_aiobotocore_dataexchange/paginator.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-dataexchange-2.5.2.post3/types_aiobotocore_dataexchange/type_defs.py` & `types-aiobotocore-dataexchange-2.5.4/types_aiobotocore_dataexchange/type_defs.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-dataexchange-2.5.2.post3/types_aiobotocore_dataexchange/type_defs.pyi` & `types-aiobotocore-dataexchange-2.5.4/types_aiobotocore_dataexchange/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-dataexchange-2.5.2.post3/types_aiobotocore_dataexchange.egg-info/PKG-INFO` & `types-aiobotocore-dataexchange-2.5.4/types_aiobotocore_dataexchange.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-dataexchange
-Version: 2.5.2.post3
-Summary: Type annotations for aiobotocore.DataExchange 2.5.2 service generated with mypy-boto3-builder 7.17.2
+Version: 2.5.4
+Summary: Type annotations for aiobotocore.DataExchange 2.5.4 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dataexchange/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-dataexchange.svg?color=blue)](https://pypi.org/project/types-aiobotocore-dataexchange)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dataexchange/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-dataexchange)](https://pepy.tech/project/types-aiobotocore-dataexchange)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.DataExchange 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dataexchange.html#DataExchange)
+[aiobotocore.DataExchange 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dataexchange.html#DataExchange)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-dataexchange-2.5.2.post3/types_aiobotocore_dataexchange.egg-info/SOURCES.txt` & `types-aiobotocore-dataexchange-2.5.4/types_aiobotocore_dataexchange.egg-info/SOURCES.txt`

 * *Files identical despite different names*


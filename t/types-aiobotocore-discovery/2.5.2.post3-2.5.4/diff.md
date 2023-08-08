# Comparing `tmp/types-aiobotocore-discovery-2.5.2.post3.tar.gz` & `tmp/types-aiobotocore-discovery-2.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-discovery-2.5.2.post3.tar", last modified: Fri Aug  4 12:37:36 2023, max compression
+gzip compressed data, was "types-aiobotocore-discovery-2.5.4.tar", last modified: Tue Aug  8 01:23:36 2023, max compression
```

## Comparing `types-aiobotocore-discovery-2.5.2.post3.tar` & `types-aiobotocore-discovery-2.5.4.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:37:36.635645 types-aiobotocore-discovery-2.5.2.post3/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-04 12:21:30.000000 types-aiobotocore-discovery-2.5.2.post3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    14062 2023-08-04 12:37:36.635645 types-aiobotocore-discovery-2.5.2.post3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    12518 2023-08-04 12:21:30.000000 types-aiobotocore-discovery-2.5.2.post3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-04 12:37:36.635645 types-aiobotocore-discovery-2.5.2.post3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2104 2023-08-04 12:21:30.000000 types-aiobotocore-discovery-2.5.2.post3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:37:36.627645 types-aiobotocore-discovery-2.5.2.post3/types_aiobotocore_discovery/
--rw-r--r--   0 runner    (1001) docker     (123)     1925 2023-08-04 12:21:30.000000 types-aiobotocore-discovery-2.5.2.post3/types_aiobotocore_discovery/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1924 2023-08-04 12:21:30.000000 types-aiobotocore-discovery-2.5.2.post3/types_aiobotocore_discovery/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      987 2023-08-04 12:21:30.000000 types-aiobotocore-discovery-2.5.2.post3/types_aiobotocore_discovery/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    24625 2023-08-04 12:21:31.000000 types-aiobotocore-discovery-2.5.2.post3/types_aiobotocore_discovery/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    24585 2023-08-04 12:21:31.000000 types-aiobotocore-discovery-2.5.2.post3/types_aiobotocore_discovery/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    10272 2023-08-04 12:21:31.000000 types-aiobotocore-discovery-2.5.2.post3/types_aiobotocore_discovery/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    10270 2023-08-04 12:21:31.000000 types-aiobotocore-discovery-2.5.2.post3/types_aiobotocore_discovery/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8685 2023-08-04 12:21:31.000000 types-aiobotocore-discovery-2.5.2.post3/types_aiobotocore_discovery/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     8677 2023-08-04 12:21:31.000000 types-aiobotocore-discovery-2.5.2.post3/types_aiobotocore_discovery/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 12:21:30.000000 types-aiobotocore-discovery-2.5.2.post3/types_aiobotocore_discovery/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    25203 2023-08-04 12:21:32.000000 types-aiobotocore-discovery-2.5.2.post3/types_aiobotocore_discovery/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    25182 2023-08-04 12:21:32.000000 types-aiobotocore-discovery-2.5.2.post3/types_aiobotocore_discovery/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-04 12:21:30.000000 types-aiobotocore-discovery-2.5.2.post3/types_aiobotocore_discovery/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:37:36.635645 types-aiobotocore-discovery-2.5.2.post3/types_aiobotocore_discovery.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    14062 2023-08-04 12:37:36.000000 types-aiobotocore-discovery-2.5.2.post3/types_aiobotocore_discovery.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      851 2023-08-04 12:37:36.000000 types-aiobotocore-discovery-2.5.2.post3/types_aiobotocore_discovery.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 12:37:36.000000 types-aiobotocore-discovery-2.5.2.post3/types_aiobotocore_discovery.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 12:37:36.000000 types-aiobotocore-discovery-2.5.2.post3/types_aiobotocore_discovery.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-04 12:37:36.000000 types-aiobotocore-discovery-2.5.2.post3/types_aiobotocore_discovery.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-08-04 12:37:36.000000 types-aiobotocore-discovery-2.5.2.post3/types_aiobotocore_discovery.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:23:36.278685 types-aiobotocore-discovery-2.5.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-08 01:09:06.000000 types-aiobotocore-discovery-2.5.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    14056 2023-08-08 01:23:36.274685 types-aiobotocore-discovery-2.5.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    12518 2023-08-08 01:09:06.000000 types-aiobotocore-discovery-2.5.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-08 01:23:36.278685 types-aiobotocore-discovery-2.5.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2098 2023-08-08 01:09:06.000000 types-aiobotocore-discovery-2.5.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:23:36.270685 types-aiobotocore-discovery-2.5.4/types_aiobotocore_discovery/
+-rw-r--r--   0 runner    (1001) docker     (123)     1925 2023-08-08 01:09:06.000000 types-aiobotocore-discovery-2.5.4/types_aiobotocore_discovery/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1924 2023-08-08 01:09:06.000000 types-aiobotocore-discovery-2.5.4/types_aiobotocore_discovery/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      975 2023-08-08 01:09:06.000000 types-aiobotocore-discovery-2.5.4/types_aiobotocore_discovery/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24625 2023-08-08 01:09:06.000000 types-aiobotocore-discovery-2.5.4/types_aiobotocore_discovery/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24585 2023-08-08 01:09:06.000000 types-aiobotocore-discovery-2.5.4/types_aiobotocore_discovery/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    10367 2023-08-08 01:09:06.000000 types-aiobotocore-discovery-2.5.4/types_aiobotocore_discovery/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10365 2023-08-08 01:09:06.000000 types-aiobotocore-discovery-2.5.4/types_aiobotocore_discovery/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8685 2023-08-08 01:09:06.000000 types-aiobotocore-discovery-2.5.4/types_aiobotocore_discovery/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8677 2023-08-08 01:09:06.000000 types-aiobotocore-discovery-2.5.4/types_aiobotocore_discovery/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 01:09:06.000000 types-aiobotocore-discovery-2.5.4/types_aiobotocore_discovery/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    25203 2023-08-08 01:09:07.000000 types-aiobotocore-discovery-2.5.4/types_aiobotocore_discovery/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25182 2023-08-08 01:09:06.000000 types-aiobotocore-discovery-2.5.4/types_aiobotocore_discovery/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-08-08 01:09:06.000000 types-aiobotocore-discovery-2.5.4/types_aiobotocore_discovery/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:23:36.274685 types-aiobotocore-discovery-2.5.4/types_aiobotocore_discovery.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    14056 2023-08-08 01:23:36.000000 types-aiobotocore-discovery-2.5.4/types_aiobotocore_discovery.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      851 2023-08-08 01:23:36.000000 types-aiobotocore-discovery-2.5.4/types_aiobotocore_discovery.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 01:23:36.000000 types-aiobotocore-discovery-2.5.4/types_aiobotocore_discovery.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 01:23:36.000000 types-aiobotocore-discovery-2.5.4/types_aiobotocore_discovery.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-08 01:23:36.000000 types-aiobotocore-discovery-2.5.4/types_aiobotocore_discovery.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-08-08 01:23:36.000000 types-aiobotocore-discovery-2.5.4/types_aiobotocore_discovery.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-discovery-2.5.2.post3/LICENSE` & `types-aiobotocore-discovery-2.5.4/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-discovery-2.5.2.post3/PKG-INFO` & `types-aiobotocore-discovery-2.5.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-discovery
-Version: 2.5.2.post3
-Summary: Type annotations for aiobotocore.ApplicationDiscoveryService 2.5.2 service generated with mypy-boto3-builder 7.17.2
+Version: 2.5.4
+Summary: Type annotations for aiobotocore.ApplicationDiscoveryService 2.5.4 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_discovery/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-discovery.svg?color=blue)](https://pypi.org/project/types-aiobotocore-discovery)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_discovery/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-discovery)](https://pepy.tech/project/types-aiobotocore-discovery)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.ApplicationDiscoveryService 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/discovery.html#ApplicationDiscoveryService)
+[aiobotocore.ApplicationDiscoveryService 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/discovery.html#ApplicationDiscoveryService)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-discovery-2.5.2.post3/README.md` & `types-aiobotocore-discovery-2.5.4/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-discovery.svg?color=blue)](https://pypi.org/project/types-aiobotocore-discovery)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_discovery/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-discovery)](https://pepy.tech/project/types-aiobotocore-discovery)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.ApplicationDiscoveryService 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/discovery.html#ApplicationDiscoveryService)
+[aiobotocore.ApplicationDiscoveryService 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/discovery.html#ApplicationDiscoveryService)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-discovery-2.5.2.post3/setup.py` & `types-aiobotocore-discovery-2.5.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-discovery",
-    version="2.5.2.post3",
+    version="2.5.4",
     packages=["types_aiobotocore_discovery"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.ApplicationDiscoveryService 2.5.2 service generated with"
+        "Type annotations for aiobotocore.ApplicationDiscoveryService 2.5.4 service generated with"
         " mypy-boto3-builder 7.17.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
```

### Comparing `types-aiobotocore-discovery-2.5.2.post3/types_aiobotocore_discovery/__init__.py` & `types-aiobotocore-discovery-2.5.4/types_aiobotocore_discovery/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-discovery-2.5.2.post3/types_aiobotocore_discovery/__init__.pyi` & `types-aiobotocore-discovery-2.5.4/types_aiobotocore_discovery/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-discovery-2.5.2.post3/types_aiobotocore_discovery/__main__.py` & `types-aiobotocore-discovery-2.5.4/types_aiobotocore_discovery/__main__.py`

 * *Files 10% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.ApplicationDiscoveryService 2.5.2\nVersion:        "
-        " 2.5.2.post3\nBuilder version: 7.17.2\nDocs:           "
+        "Type annotations for aiobotocore.ApplicationDiscoveryService 2.5.4\nVersion:        "
+        " 2.5.4\nBuilder version: 7.17.2\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_discovery//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/discovery.html#ApplicationDiscoveryService\nOther"
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

### Comparing `types-aiobotocore-discovery-2.5.2.post3/types_aiobotocore_discovery/client.py` & `types-aiobotocore-discovery-2.5.4/types_aiobotocore_discovery/client.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-discovery-2.5.2.post3/types_aiobotocore_discovery/client.pyi` & `types-aiobotocore-discovery-2.5.4/types_aiobotocore_discovery/client.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-discovery-2.5.2.post3/types_aiobotocore_discovery/literals.py` & `types-aiobotocore-discovery-2.5.4/types_aiobotocore_discovery/literals.py`

 * *Files 1% similar despite different names*

```diff
@@ -100,14 +100,15 @@
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
@@ -203,14 +204,15 @@
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
@@ -289,26 +291,28 @@
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

### Comparing `types-aiobotocore-discovery-2.5.2.post3/types_aiobotocore_discovery/literals.pyi` & `types-aiobotocore-discovery-2.5.4/types_aiobotocore_discovery/literals.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -98,14 +98,15 @@
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
@@ -201,14 +202,15 @@
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
@@ -287,26 +289,28 @@
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

### Comparing `types-aiobotocore-discovery-2.5.2.post3/types_aiobotocore_discovery/paginator.py` & `types-aiobotocore-discovery-2.5.4/types_aiobotocore_discovery/paginator.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-discovery-2.5.2.post3/types_aiobotocore_discovery/paginator.pyi` & `types-aiobotocore-discovery-2.5.4/types_aiobotocore_discovery/paginator.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-discovery-2.5.2.post3/types_aiobotocore_discovery/type_defs.py` & `types-aiobotocore-discovery-2.5.4/types_aiobotocore_discovery/type_defs.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-discovery-2.5.2.post3/types_aiobotocore_discovery/type_defs.pyi` & `types-aiobotocore-discovery-2.5.4/types_aiobotocore_discovery/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-discovery-2.5.2.post3/types_aiobotocore_discovery.egg-info/PKG-INFO` & `types-aiobotocore-discovery-2.5.4/types_aiobotocore_discovery.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-discovery
-Version: 2.5.2.post3
-Summary: Type annotations for aiobotocore.ApplicationDiscoveryService 2.5.2 service generated with mypy-boto3-builder 7.17.2
+Version: 2.5.4
+Summary: Type annotations for aiobotocore.ApplicationDiscoveryService 2.5.4 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_discovery/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-discovery.svg?color=blue)](https://pypi.org/project/types-aiobotocore-discovery)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_discovery/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-discovery)](https://pepy.tech/project/types-aiobotocore-discovery)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.ApplicationDiscoveryService 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/discovery.html#ApplicationDiscoveryService)
+[aiobotocore.ApplicationDiscoveryService 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/discovery.html#ApplicationDiscoveryService)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-discovery-2.5.2.post3/types_aiobotocore_discovery.egg-info/SOURCES.txt` & `types-aiobotocore-discovery-2.5.4/types_aiobotocore_discovery.egg-info/SOURCES.txt`

 * *Files identical despite different names*


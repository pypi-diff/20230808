# Comparing `tmp/types-aiobotocore-appmesh-2.5.2.post3.tar.gz` & `tmp/types-aiobotocore-appmesh-2.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-appmesh-2.5.2.post3.tar", last modified: Fri Aug  4 12:37:18 2023, max compression
+gzip compressed data, was "types-aiobotocore-appmesh-2.5.4.tar", last modified: Tue Aug  8 01:23:19 2023, max compression
```

## Comparing `types-aiobotocore-appmesh-2.5.2.post3.tar` & `types-aiobotocore-appmesh-2.5.4.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:37:18.859224 types-aiobotocore-appmesh-2.5.2.post3/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-04 12:18:28.000000 types-aiobotocore-appmesh-2.5.2.post3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    14004 2023-08-04 12:37:18.855224 types-aiobotocore-appmesh-2.5.2.post3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    12486 2023-08-04 12:18:28.000000 types-aiobotocore-appmesh-2.5.2.post3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-04 12:37:18.859224 types-aiobotocore-appmesh-2.5.2.post3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2072 2023-08-04 12:18:28.000000 types-aiobotocore-appmesh-2.5.2.post3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:37:18.855224 types-aiobotocore-appmesh-2.5.2.post3/types_aiobotocore_appmesh/
--rw-r--r--   0 runner    (1001) docker     (123)     2111 2023-08-04 12:18:28.000000 types-aiobotocore-appmesh-2.5.2.post3/types_aiobotocore_appmesh/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2110 2023-08-04 12:18:28.000000 types-aiobotocore-appmesh-2.5.2.post3/types_aiobotocore_appmesh/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      943 2023-08-04 12:18:28.000000 types-aiobotocore-appmesh-2.5.2.post3/types_aiobotocore_appmesh/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    32306 2023-08-04 12:18:28.000000 types-aiobotocore-appmesh-2.5.2.post3/types_aiobotocore_appmesh/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    32251 2023-08-04 12:18:28.000000 types-aiobotocore-appmesh-2.5.2.post3/types_aiobotocore_appmesh/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    11040 2023-08-04 12:18:28.000000 types-aiobotocore-appmesh-2.5.2.post3/types_aiobotocore_appmesh/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    11038 2023-08-04 12:18:28.000000 types-aiobotocore-appmesh-2.5.2.post3/types_aiobotocore_appmesh/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9947 2023-08-04 12:18:28.000000 types-aiobotocore-appmesh-2.5.2.post3/types_aiobotocore_appmesh/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     9937 2023-08-04 12:18:28.000000 types-aiobotocore-appmesh-2.5.2.post3/types_aiobotocore_appmesh/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 12:18:28.000000 types-aiobotocore-appmesh-2.5.2.post3/types_aiobotocore_appmesh/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    80416 2023-08-04 12:18:31.000000 types-aiobotocore-appmesh-2.5.2.post3/types_aiobotocore_appmesh/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    80265 2023-08-04 12:18:29.000000 types-aiobotocore-appmesh-2.5.2.post3/types_aiobotocore_appmesh/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-04 12:18:28.000000 types-aiobotocore-appmesh-2.5.2.post3/types_aiobotocore_appmesh/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:37:18.855224 types-aiobotocore-appmesh-2.5.2.post3/types_aiobotocore_appmesh.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    14004 2023-08-04 12:37:18.000000 types-aiobotocore-appmesh-2.5.2.post3/types_aiobotocore_appmesh.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      813 2023-08-04 12:37:18.000000 types-aiobotocore-appmesh-2.5.2.post3/types_aiobotocore_appmesh.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 12:37:18.000000 types-aiobotocore-appmesh-2.5.2.post3/types_aiobotocore_appmesh.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 12:37:18.000000 types-aiobotocore-appmesh-2.5.2.post3/types_aiobotocore_appmesh.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-04 12:37:18.000000 types-aiobotocore-appmesh-2.5.2.post3/types_aiobotocore_appmesh.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-08-04 12:37:18.000000 types-aiobotocore-appmesh-2.5.2.post3/types_aiobotocore_appmesh.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:23:19.302520 types-aiobotocore-appmesh-2.5.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-08 01:06:15.000000 types-aiobotocore-appmesh-2.5.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    13998 2023-08-08 01:23:19.294520 types-aiobotocore-appmesh-2.5.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    12486 2023-08-08 01:06:15.000000 types-aiobotocore-appmesh-2.5.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-08 01:23:19.302520 types-aiobotocore-appmesh-2.5.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2066 2023-08-08 01:06:15.000000 types-aiobotocore-appmesh-2.5.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:23:19.294520 types-aiobotocore-appmesh-2.5.4/types_aiobotocore_appmesh/
+-rw-r--r--   0 runner    (1001) docker     (123)     2111 2023-08-08 01:06:15.000000 types-aiobotocore-appmesh-2.5.4/types_aiobotocore_appmesh/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2110 2023-08-08 01:06:15.000000 types-aiobotocore-appmesh-2.5.4/types_aiobotocore_appmesh/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      931 2023-08-08 01:06:15.000000 types-aiobotocore-appmesh-2.5.4/types_aiobotocore_appmesh/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32306 2023-08-08 01:06:15.000000 types-aiobotocore-appmesh-2.5.4/types_aiobotocore_appmesh/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32251 2023-08-08 01:06:15.000000 types-aiobotocore-appmesh-2.5.4/types_aiobotocore_appmesh/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    11135 2023-08-08 01:06:16.000000 types-aiobotocore-appmesh-2.5.4/types_aiobotocore_appmesh/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11133 2023-08-08 01:06:15.000000 types-aiobotocore-appmesh-2.5.4/types_aiobotocore_appmesh/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9947 2023-08-08 01:06:15.000000 types-aiobotocore-appmesh-2.5.4/types_aiobotocore_appmesh/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9937 2023-08-08 01:06:15.000000 types-aiobotocore-appmesh-2.5.4/types_aiobotocore_appmesh/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 01:06:15.000000 types-aiobotocore-appmesh-2.5.4/types_aiobotocore_appmesh/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    80416 2023-08-08 01:06:17.000000 types-aiobotocore-appmesh-2.5.4/types_aiobotocore_appmesh/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    80265 2023-08-08 01:06:17.000000 types-aiobotocore-appmesh-2.5.4/types_aiobotocore_appmesh/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-08-08 01:06:15.000000 types-aiobotocore-appmesh-2.5.4/types_aiobotocore_appmesh/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:23:19.294520 types-aiobotocore-appmesh-2.5.4/types_aiobotocore_appmesh.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    13998 2023-08-08 01:23:19.000000 types-aiobotocore-appmesh-2.5.4/types_aiobotocore_appmesh.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      813 2023-08-08 01:23:19.000000 types-aiobotocore-appmesh-2.5.4/types_aiobotocore_appmesh.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 01:23:19.000000 types-aiobotocore-appmesh-2.5.4/types_aiobotocore_appmesh.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 01:23:19.000000 types-aiobotocore-appmesh-2.5.4/types_aiobotocore_appmesh.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-08 01:23:19.000000 types-aiobotocore-appmesh-2.5.4/types_aiobotocore_appmesh.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-08-08 01:23:19.000000 types-aiobotocore-appmesh-2.5.4/types_aiobotocore_appmesh.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-appmesh-2.5.2.post3/LICENSE` & `types-aiobotocore-appmesh-2.5.4/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-appmesh-2.5.2.post3/PKG-INFO` & `types-aiobotocore-appmesh-2.5.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-appmesh
-Version: 2.5.2.post3
-Summary: Type annotations for aiobotocore.AppMesh 2.5.2 service generated with mypy-boto3-builder 7.17.2
+Version: 2.5.4
+Summary: Type annotations for aiobotocore.AppMesh 2.5.4 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appmesh/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-appmesh.svg?color=blue)](https://pypi.org/project/types-aiobotocore-appmesh)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appmesh/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-appmesh)](https://pepy.tech/project/types-aiobotocore-appmesh)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.AppMesh 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appmesh.html#AppMesh)
+[aiobotocore.AppMesh 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appmesh.html#AppMesh)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-appmesh-2.5.2.post3/README.md` & `types-aiobotocore-appmesh-2.5.4/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-appmesh.svg?color=blue)](https://pypi.org/project/types-aiobotocore-appmesh)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appmesh/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-appmesh)](https://pepy.tech/project/types-aiobotocore-appmesh)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.AppMesh 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appmesh.html#AppMesh)
+[aiobotocore.AppMesh 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appmesh.html#AppMesh)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-appmesh-2.5.2.post3/setup.py` & `types-aiobotocore-appmesh-2.5.4/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-appmesh",
-    version="2.5.2.post3",
+    version="2.5.4",
     packages=["types_aiobotocore_appmesh"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.AppMesh 2.5.2 service generated with mypy-boto3-builder"
+        "Type annotations for aiobotocore.AppMesh 2.5.4 service generated with mypy-boto3-builder"
         " 7.17.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
```

### Comparing `types-aiobotocore-appmesh-2.5.2.post3/types_aiobotocore_appmesh/__init__.py` & `types-aiobotocore-appmesh-2.5.4/types_aiobotocore_appmesh/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-appmesh-2.5.2.post3/types_aiobotocore_appmesh/__init__.pyi` & `types-aiobotocore-appmesh-2.5.4/types_aiobotocore_appmesh/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-appmesh-2.5.2.post3/types_aiobotocore_appmesh/__main__.py` & `types-aiobotocore-appmesh-2.5.4/types_aiobotocore_appmesh/__main__.py`

 * *Files 15% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.AppMesh 2.5.2\nVersion:         2.5.2.post3\nBuilder"
-        " version: 7.17.2\nDocs:           "
+        "Type annotations for aiobotocore.AppMesh 2.5.4\nVersion:         2.5.4\nBuilder version:"
+        " 7.17.2\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appmesh//\nBoto3 docs:"
         "     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appmesh.html#AppMesh\nOther"
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

### Comparing `types-aiobotocore-appmesh-2.5.2.post3/types_aiobotocore_appmesh/client.py` & `types-aiobotocore-appmesh-2.5.4/types_aiobotocore_appmesh/client.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-appmesh-2.5.2.post3/types_aiobotocore_appmesh/client.pyi` & `types-aiobotocore-appmesh-2.5.4/types_aiobotocore_appmesh/client.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-appmesh-2.5.2.post3/types_aiobotocore_appmesh/literals.py` & `types-aiobotocore-appmesh-2.5.4/types_aiobotocore_appmesh/literals.py`

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

### Comparing `types-aiobotocore-appmesh-2.5.2.post3/types_aiobotocore_appmesh/literals.pyi` & `types-aiobotocore-appmesh-2.5.4/types_aiobotocore_appmesh/literals.pyi`

 * *Files 1% similar despite different names*

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

### Comparing `types-aiobotocore-appmesh-2.5.2.post3/types_aiobotocore_appmesh/paginator.py` & `types-aiobotocore-appmesh-2.5.4/types_aiobotocore_appmesh/paginator.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-appmesh-2.5.2.post3/types_aiobotocore_appmesh/paginator.pyi` & `types-aiobotocore-appmesh-2.5.4/types_aiobotocore_appmesh/paginator.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-appmesh-2.5.2.post3/types_aiobotocore_appmesh/type_defs.py` & `types-aiobotocore-appmesh-2.5.4/types_aiobotocore_appmesh/type_defs.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-appmesh-2.5.2.post3/types_aiobotocore_appmesh/type_defs.pyi` & `types-aiobotocore-appmesh-2.5.4/types_aiobotocore_appmesh/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-appmesh-2.5.2.post3/types_aiobotocore_appmesh.egg-info/PKG-INFO` & `types-aiobotocore-appmesh-2.5.4/types_aiobotocore_appmesh.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-appmesh
-Version: 2.5.2.post3
-Summary: Type annotations for aiobotocore.AppMesh 2.5.2 service generated with mypy-boto3-builder 7.17.2
+Version: 2.5.4
+Summary: Type annotations for aiobotocore.AppMesh 2.5.4 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appmesh/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-appmesh.svg?color=blue)](https://pypi.org/project/types-aiobotocore-appmesh)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appmesh/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-appmesh)](https://pepy.tech/project/types-aiobotocore-appmesh)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.AppMesh 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appmesh.html#AppMesh)
+[aiobotocore.AppMesh 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appmesh.html#AppMesh)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-appmesh-2.5.2.post3/types_aiobotocore_appmesh.egg-info/SOURCES.txt` & `types-aiobotocore-appmesh-2.5.4/types_aiobotocore_appmesh.egg-info/SOURCES.txt`

 * *Files identical despite different names*


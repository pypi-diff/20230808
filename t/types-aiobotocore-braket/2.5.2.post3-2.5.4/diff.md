# Comparing `tmp/types-aiobotocore-braket-2.5.2.post3.tar.gz` & `tmp/types-aiobotocore-braket-2.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-braket-2.5.2.post3.tar", last modified: Fri Aug  4 12:37:21 2023, max compression
+gzip compressed data, was "types-aiobotocore-braket-2.5.4.tar", last modified: Tue Aug  8 01:23:22 2023, max compression
```

## Comparing `types-aiobotocore-braket-2.5.2.post3.tar` & `types-aiobotocore-braket-2.5.4.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:37:21.623282 types-aiobotocore-braket-2.5.2.post3/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-04 12:19:02.000000 types-aiobotocore-braket-2.5.2.post3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    13121 2023-08-04 12:37:21.611281 types-aiobotocore-braket-2.5.2.post3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    11607 2023-08-04 12:19:02.000000 types-aiobotocore-braket-2.5.2.post3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-04 12:37:21.623282 types-aiobotocore-braket-2.5.2.post3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2065 2023-08-04 12:19:02.000000 types-aiobotocore-braket-2.5.2.post3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:37:21.611281 types-aiobotocore-braket-2.5.2.post3/types_aiobotocore_braket/
--rw-r--r--   0 runner    (1001) docker     (123)     1022 2023-08-04 12:19:02.000000 types-aiobotocore-braket-2.5.2.post3/types_aiobotocore_braket/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1021 2023-08-04 12:19:02.000000 types-aiobotocore-braket-2.5.2.post3/types_aiobotocore_braket/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      928 2023-08-04 12:19:02.000000 types-aiobotocore-braket-2.5.2.post3/types_aiobotocore_braket/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13725 2023-08-04 12:19:02.000000 types-aiobotocore-braket-2.5.2.post3/types_aiobotocore_braket/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    13700 2023-08-04 12:19:02.000000 types-aiobotocore-braket-2.5.2.post3/types_aiobotocore_braket/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    10069 2023-08-04 12:19:02.000000 types-aiobotocore-braket-2.5.2.post3/types_aiobotocore_braket/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    10067 2023-08-04 12:19:02.000000 types-aiobotocore-braket-2.5.2.post3/types_aiobotocore_braket/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     4387 2023-08-04 12:19:02.000000 types-aiobotocore-braket-2.5.2.post3/types_aiobotocore_braket/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     4382 2023-08-04 12:19:02.000000 types-aiobotocore-braket-2.5.2.post3/types_aiobotocore_braket/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 12:19:02.000000 types-aiobotocore-braket-2.5.2.post3/types_aiobotocore_braket/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    17655 2023-08-04 12:19:03.000000 types-aiobotocore-braket-2.5.2.post3/types_aiobotocore_braket/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    17624 2023-08-04 12:19:02.000000 types-aiobotocore-braket-2.5.2.post3/types_aiobotocore_braket/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-04 12:19:02.000000 types-aiobotocore-braket-2.5.2.post3/types_aiobotocore_braket/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:37:21.611281 types-aiobotocore-braket-2.5.2.post3/types_aiobotocore_braket.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    13121 2023-08-04 12:37:21.000000 types-aiobotocore-braket-2.5.2.post3/types_aiobotocore_braket.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      794 2023-08-04 12:37:21.000000 types-aiobotocore-braket-2.5.2.post3/types_aiobotocore_braket.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 12:37:21.000000 types-aiobotocore-braket-2.5.2.post3/types_aiobotocore_braket.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 12:37:21.000000 types-aiobotocore-braket-2.5.2.post3/types_aiobotocore_braket.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-04 12:37:21.000000 types-aiobotocore-braket-2.5.2.post3/types_aiobotocore_braket.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-08-04 12:37:21.000000 types-aiobotocore-braket-2.5.2.post3/types_aiobotocore_braket.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:23:22.262621 types-aiobotocore-braket-2.5.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-08 01:06:47.000000 types-aiobotocore-braket-2.5.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    13115 2023-08-08 01:23:22.262621 types-aiobotocore-braket-2.5.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    11607 2023-08-08 01:06:47.000000 types-aiobotocore-braket-2.5.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-08 01:23:22.262621 types-aiobotocore-braket-2.5.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2059 2023-08-08 01:06:47.000000 types-aiobotocore-braket-2.5.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:23:22.250621 types-aiobotocore-braket-2.5.4/types_aiobotocore_braket/
+-rw-r--r--   0 runner    (1001) docker     (123)     1022 2023-08-08 01:06:47.000000 types-aiobotocore-braket-2.5.4/types_aiobotocore_braket/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1021 2023-08-08 01:06:47.000000 types-aiobotocore-braket-2.5.4/types_aiobotocore_braket/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      916 2023-08-08 01:06:47.000000 types-aiobotocore-braket-2.5.4/types_aiobotocore_braket/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13725 2023-08-08 01:06:47.000000 types-aiobotocore-braket-2.5.4/types_aiobotocore_braket/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13700 2023-08-08 01:06:47.000000 types-aiobotocore-braket-2.5.4/types_aiobotocore_braket/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    10164 2023-08-08 01:06:48.000000 types-aiobotocore-braket-2.5.4/types_aiobotocore_braket/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10162 2023-08-08 01:06:48.000000 types-aiobotocore-braket-2.5.4/types_aiobotocore_braket/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     4387 2023-08-08 01:06:48.000000 types-aiobotocore-braket-2.5.4/types_aiobotocore_braket/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4382 2023-08-08 01:06:47.000000 types-aiobotocore-braket-2.5.4/types_aiobotocore_braket/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 01:06:47.000000 types-aiobotocore-braket-2.5.4/types_aiobotocore_braket/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    17655 2023-08-08 01:06:48.000000 types-aiobotocore-braket-2.5.4/types_aiobotocore_braket/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17624 2023-08-08 01:06:48.000000 types-aiobotocore-braket-2.5.4/types_aiobotocore_braket/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-08-08 01:06:47.000000 types-aiobotocore-braket-2.5.4/types_aiobotocore_braket/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:23:22.262621 types-aiobotocore-braket-2.5.4/types_aiobotocore_braket.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    13115 2023-08-08 01:23:22.000000 types-aiobotocore-braket-2.5.4/types_aiobotocore_braket.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      794 2023-08-08 01:23:22.000000 types-aiobotocore-braket-2.5.4/types_aiobotocore_braket.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 01:23:22.000000 types-aiobotocore-braket-2.5.4/types_aiobotocore_braket.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 01:23:22.000000 types-aiobotocore-braket-2.5.4/types_aiobotocore_braket.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-08 01:23:22.000000 types-aiobotocore-braket-2.5.4/types_aiobotocore_braket.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-08-08 01:23:22.000000 types-aiobotocore-braket-2.5.4/types_aiobotocore_braket.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-braket-2.5.2.post3/LICENSE` & `types-aiobotocore-braket-2.5.4/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-braket-2.5.2.post3/PKG-INFO` & `types-aiobotocore-braket-2.5.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-braket
-Version: 2.5.2.post3
-Summary: Type annotations for aiobotocore.Braket 2.5.2 service generated with mypy-boto3-builder 7.17.2
+Version: 2.5.4
+Summary: Type annotations for aiobotocore.Braket 2.5.4 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_braket/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-braket.svg?color=blue)](https://pypi.org/project/types-aiobotocore-braket)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_braket/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-braket)](https://pepy.tech/project/types-aiobotocore-braket)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.Braket 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/braket.html#Braket)
+[aiobotocore.Braket 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/braket.html#Braket)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-braket-2.5.2.post3/README.md` & `types-aiobotocore-braket-2.5.4/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-braket.svg?color=blue)](https://pypi.org/project/types-aiobotocore-braket)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_braket/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-braket)](https://pepy.tech/project/types-aiobotocore-braket)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.Braket 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/braket.html#Braket)
+[aiobotocore.Braket 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/braket.html#Braket)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-braket-2.5.2.post3/setup.py` & `types-aiobotocore-braket-2.5.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-braket",
-    version="2.5.2.post3",
+    version="2.5.4",
     packages=["types_aiobotocore_braket"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.Braket 2.5.2 service generated with mypy-boto3-builder"
+        "Type annotations for aiobotocore.Braket 2.5.4 service generated with mypy-boto3-builder"
         " 7.17.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
```

### Comparing `types-aiobotocore-braket-2.5.2.post3/types_aiobotocore_braket/__init__.py` & `types-aiobotocore-braket-2.5.4/types_aiobotocore_braket/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-braket-2.5.2.post3/types_aiobotocore_braket/__init__.pyi` & `types-aiobotocore-braket-2.5.4/types_aiobotocore_braket/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-braket-2.5.2.post3/types_aiobotocore_braket/__main__.py` & `types-aiobotocore-braket-2.5.4/types_aiobotocore_braket/__main__.py`

 * *Files 9% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.Braket 2.5.2\nVersion:         2.5.2.post3\nBuilder"
-        " version: 7.17.2\nDocs:           "
+        "Type annotations for aiobotocore.Braket 2.5.4\nVersion:         2.5.4\nBuilder version:"
+        " 7.17.2\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_braket//\nBoto3 docs: "
         "     https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/braket.html#Braket\nOther"
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

### Comparing `types-aiobotocore-braket-2.5.2.post3/types_aiobotocore_braket/client.py` & `types-aiobotocore-braket-2.5.4/types_aiobotocore_braket/client.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-braket-2.5.2.post3/types_aiobotocore_braket/client.pyi` & `types-aiobotocore-braket-2.5.4/types_aiobotocore_braket/client.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-braket-2.5.2.post3/types_aiobotocore_braket/literals.py` & `types-aiobotocore-braket-2.5.4/types_aiobotocore_braket/literals.py`

 * *Files 0% similar despite different names*

```diff
@@ -122,14 +122,15 @@
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
@@ -225,14 +226,15 @@
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
@@ -311,26 +313,28 @@
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

### Comparing `types-aiobotocore-braket-2.5.2.post3/types_aiobotocore_braket/literals.pyi` & `types-aiobotocore-braket-2.5.4/types_aiobotocore_braket/literals.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -120,14 +120,15 @@
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
@@ -223,14 +224,15 @@
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
@@ -309,26 +311,28 @@
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

### Comparing `types-aiobotocore-braket-2.5.2.post3/types_aiobotocore_braket/paginator.py` & `types-aiobotocore-braket-2.5.4/types_aiobotocore_braket/paginator.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-braket-2.5.2.post3/types_aiobotocore_braket/paginator.pyi` & `types-aiobotocore-braket-2.5.4/types_aiobotocore_braket/paginator.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-braket-2.5.2.post3/types_aiobotocore_braket/type_defs.py` & `types-aiobotocore-braket-2.5.4/types_aiobotocore_braket/type_defs.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-braket-2.5.2.post3/types_aiobotocore_braket/type_defs.pyi` & `types-aiobotocore-braket-2.5.4/types_aiobotocore_braket/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-braket-2.5.2.post3/types_aiobotocore_braket.egg-info/PKG-INFO` & `types-aiobotocore-braket-2.5.4/types_aiobotocore_braket.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-braket
-Version: 2.5.2.post3
-Summary: Type annotations for aiobotocore.Braket 2.5.2 service generated with mypy-boto3-builder 7.17.2
+Version: 2.5.4
+Summary: Type annotations for aiobotocore.Braket 2.5.4 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_braket/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-braket.svg?color=blue)](https://pypi.org/project/types-aiobotocore-braket)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_braket/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-braket)](https://pepy.tech/project/types-aiobotocore-braket)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.Braket 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/braket.html#Braket)
+[aiobotocore.Braket 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/braket.html#Braket)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-braket-2.5.2.post3/types_aiobotocore_braket.egg-info/SOURCES.txt` & `types-aiobotocore-braket-2.5.4/types_aiobotocore_braket.egg-info/SOURCES.txt`

 * *Files identical despite different names*


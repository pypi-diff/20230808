# Comparing `tmp/types-aiobotocore-appintegrations-2.5.2.post3.tar.gz` & `tmp/types-aiobotocore-appintegrations-2.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-appintegrations-2.5.2.post3.tar", last modified: Fri Aug  4 12:37:16 2023, max compression
+gzip compressed data, was "types-aiobotocore-appintegrations-2.5.4.tar", last modified: Tue Aug  8 01:23:17 2023, max compression
```

## Comparing `types-aiobotocore-appintegrations-2.5.2.post3.tar` & `types-aiobotocore-appintegrations-2.5.4.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:37:16.391168 types-aiobotocore-appintegrations-2.5.2.post3/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-04 12:18:21.000000 types-aiobotocore-appintegrations-2.5.2.post3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    12711 2023-08-04 12:37:16.391168 types-aiobotocore-appintegrations-2.5.2.post3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    11154 2023-08-04 12:18:21.000000 types-aiobotocore-appintegrations-2.5.2.post3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-04 12:37:16.391168 types-aiobotocore-appintegrations-2.5.2.post3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2135 2023-08-04 12:18:21.000000 types-aiobotocore-appintegrations-2.5.2.post3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:37:16.383168 types-aiobotocore-appintegrations-2.5.2.post3/types_aiobotocore_appintegrations/
--rw-r--r--   0 runner    (1001) docker     (123)      541 2023-08-04 12:18:21.000000 types-aiobotocore-appintegrations-2.5.2.post3/types_aiobotocore_appintegrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      540 2023-08-04 12:18:21.000000 types-aiobotocore-appintegrations-2.5.2.post3/types_aiobotocore_appintegrations/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      989 2023-08-04 12:18:21.000000 types-aiobotocore-appintegrations-2.5.2.post3/types_aiobotocore_appintegrations/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14095 2023-08-04 12:18:22.000000 types-aiobotocore-appintegrations-2.5.2.post3/types_aiobotocore_appintegrations/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    14072 2023-08-04 12:18:22.000000 types-aiobotocore-appintegrations-2.5.2.post3/types_aiobotocore_appintegrations/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     7840 2023-08-04 12:18:22.000000 types-aiobotocore-appintegrations-2.5.2.post3/types_aiobotocore_appintegrations/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     7838 2023-08-04 12:18:22.000000 types-aiobotocore-appintegrations-2.5.2.post3/types_aiobotocore_appintegrations/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 12:18:21.000000 types-aiobotocore-appintegrations-2.5.2.post3/types_aiobotocore_appintegrations/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    12467 2023-08-04 12:18:22.000000 types-aiobotocore-appintegrations-2.5.2.post3/types_aiobotocore_appintegrations/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    12450 2023-08-04 12:18:22.000000 types-aiobotocore-appintegrations-2.5.2.post3/types_aiobotocore_appintegrations/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-04 12:18:21.000000 types-aiobotocore-appintegrations-2.5.2.post3/types_aiobotocore_appintegrations/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:37:16.391168 types-aiobotocore-appintegrations-2.5.2.post3/types_aiobotocore_appintegrations.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    12711 2023-08-04 12:37:16.000000 types-aiobotocore-appintegrations-2.5.2.post3/types_aiobotocore_appintegrations.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      870 2023-08-04 12:37:16.000000 types-aiobotocore-appintegrations-2.5.2.post3/types_aiobotocore_appintegrations.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 12:37:16.000000 types-aiobotocore-appintegrations-2.5.2.post3/types_aiobotocore_appintegrations.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 12:37:16.000000 types-aiobotocore-appintegrations-2.5.2.post3/types_aiobotocore_appintegrations.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-04 12:37:16.000000 types-aiobotocore-appintegrations-2.5.2.post3/types_aiobotocore_appintegrations.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-08-04 12:37:16.000000 types-aiobotocore-appintegrations-2.5.2.post3/types_aiobotocore_appintegrations.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:23:16.990498 types-aiobotocore-appintegrations-2.5.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-08 01:06:09.000000 types-aiobotocore-appintegrations-2.5.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    12705 2023-08-08 01:23:16.986498 types-aiobotocore-appintegrations-2.5.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    11154 2023-08-08 01:06:09.000000 types-aiobotocore-appintegrations-2.5.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-08 01:23:16.990498 types-aiobotocore-appintegrations-2.5.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2129 2023-08-08 01:06:09.000000 types-aiobotocore-appintegrations-2.5.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:23:16.978498 types-aiobotocore-appintegrations-2.5.4/types_aiobotocore_appintegrations/
+-rw-r--r--   0 runner    (1001) docker     (123)      541 2023-08-08 01:06:09.000000 types-aiobotocore-appintegrations-2.5.4/types_aiobotocore_appintegrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      540 2023-08-08 01:06:09.000000 types-aiobotocore-appintegrations-2.5.4/types_aiobotocore_appintegrations/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      977 2023-08-08 01:06:09.000000 types-aiobotocore-appintegrations-2.5.4/types_aiobotocore_appintegrations/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14095 2023-08-08 01:06:09.000000 types-aiobotocore-appintegrations-2.5.4/types_aiobotocore_appintegrations/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14072 2023-08-08 01:06:09.000000 types-aiobotocore-appintegrations-2.5.4/types_aiobotocore_appintegrations/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     7935 2023-08-08 01:06:10.000000 types-aiobotocore-appintegrations-2.5.4/types_aiobotocore_appintegrations/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7933 2023-08-08 01:06:09.000000 types-aiobotocore-appintegrations-2.5.4/types_aiobotocore_appintegrations/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 01:06:09.000000 types-aiobotocore-appintegrations-2.5.4/types_aiobotocore_appintegrations/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    12467 2023-08-08 01:06:10.000000 types-aiobotocore-appintegrations-2.5.4/types_aiobotocore_appintegrations/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12450 2023-08-08 01:06:10.000000 types-aiobotocore-appintegrations-2.5.4/types_aiobotocore_appintegrations/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-08-08 01:06:09.000000 types-aiobotocore-appintegrations-2.5.4/types_aiobotocore_appintegrations/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:23:16.986498 types-aiobotocore-appintegrations-2.5.4/types_aiobotocore_appintegrations.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    12705 2023-08-08 01:23:16.000000 types-aiobotocore-appintegrations-2.5.4/types_aiobotocore_appintegrations.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      870 2023-08-08 01:23:16.000000 types-aiobotocore-appintegrations-2.5.4/types_aiobotocore_appintegrations.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 01:23:16.000000 types-aiobotocore-appintegrations-2.5.4/types_aiobotocore_appintegrations.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 01:23:16.000000 types-aiobotocore-appintegrations-2.5.4/types_aiobotocore_appintegrations.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-08 01:23:16.000000 types-aiobotocore-appintegrations-2.5.4/types_aiobotocore_appintegrations.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-08-08 01:23:16.000000 types-aiobotocore-appintegrations-2.5.4/types_aiobotocore_appintegrations.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-appintegrations-2.5.2.post3/LICENSE` & `types-aiobotocore-appintegrations-2.5.4/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-appintegrations-2.5.2.post3/PKG-INFO` & `types-aiobotocore-appintegrations-2.5.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-appintegrations
-Version: 2.5.2.post3
-Summary: Type annotations for aiobotocore.AppIntegrationsService 2.5.2 service generated with mypy-boto3-builder 7.17.2
+Version: 2.5.4
+Summary: Type annotations for aiobotocore.AppIntegrationsService 2.5.4 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appintegrations/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-appintegrations.svg?color=blue)](https://pypi.org/project/types-aiobotocore-appintegrations)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appintegrations/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-appintegrations)](https://pepy.tech/project/types-aiobotocore-appintegrations)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.AppIntegrationsService 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appintegrations.html#AppIntegrationsService)
+[aiobotocore.AppIntegrationsService 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appintegrations.html#AppIntegrationsService)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-appintegrations-2.5.2.post3/README.md` & `types-aiobotocore-appintegrations-2.5.4/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-appintegrations.svg?color=blue)](https://pypi.org/project/types-aiobotocore-appintegrations)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appintegrations/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-appintegrations)](https://pepy.tech/project/types-aiobotocore-appintegrations)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.AppIntegrationsService 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appintegrations.html#AppIntegrationsService)
+[aiobotocore.AppIntegrationsService 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appintegrations.html#AppIntegrationsService)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-appintegrations-2.5.2.post3/setup.py` & `types-aiobotocore-appintegrations-2.5.4/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-appintegrations",
-    version="2.5.2.post3",
+    version="2.5.4",
     packages=["types_aiobotocore_appintegrations"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.AppIntegrationsService 2.5.2 service generated with"
+        "Type annotations for aiobotocore.AppIntegrationsService 2.5.4 service generated with"
         " mypy-boto3-builder 7.17.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
```

### Comparing `types-aiobotocore-appintegrations-2.5.2.post3/types_aiobotocore_appintegrations/__init__.py` & `types-aiobotocore-appintegrations-2.5.4/types_aiobotocore_appintegrations/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-appintegrations-2.5.2.post3/types_aiobotocore_appintegrations/__init__.pyi` & `types-aiobotocore-appintegrations-2.5.4/types_aiobotocore_appintegrations/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-appintegrations-2.5.2.post3/types_aiobotocore_appintegrations/__main__.py` & `types-aiobotocore-appintegrations-2.5.4/types_aiobotocore_appintegrations/__main__.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.AppIntegrationsService 2.5.2\nVersion:        "
-        " 2.5.2.post3\nBuilder version: 7.17.2\nDocs:           "
+        "Type annotations for aiobotocore.AppIntegrationsService 2.5.4\nVersion:        "
+        " 2.5.4\nBuilder version: 7.17.2\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appintegrations//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appintegrations.html#AppIntegrationsService\nOther"
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

### Comparing `types-aiobotocore-appintegrations-2.5.2.post3/types_aiobotocore_appintegrations/client.py` & `types-aiobotocore-appintegrations-2.5.4/types_aiobotocore_appintegrations/client.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-appintegrations-2.5.2.post3/types_aiobotocore_appintegrations/client.pyi` & `types-aiobotocore-appintegrations-2.5.4/types_aiobotocore_appintegrations/client.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-appintegrations-2.5.2.post3/types_aiobotocore_appintegrations/literals.py` & `types-aiobotocore-appintegrations-2.5.4/types_aiobotocore_appintegrations/literals.py`

 * *Files 1% similar despite different names*

```diff
@@ -34,14 +34,15 @@
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
@@ -137,14 +138,15 @@
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
@@ -223,26 +225,28 @@
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

### Comparing `types-aiobotocore-appintegrations-2.5.2.post3/types_aiobotocore_appintegrations/literals.pyi` & `types-aiobotocore-appintegrations-2.5.4/types_aiobotocore_appintegrations/literals.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -32,14 +32,15 @@
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
@@ -135,14 +136,15 @@
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
@@ -221,26 +223,28 @@
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

### Comparing `types-aiobotocore-appintegrations-2.5.2.post3/types_aiobotocore_appintegrations/type_defs.py` & `types-aiobotocore-appintegrations-2.5.4/types_aiobotocore_appintegrations/type_defs.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-appintegrations-2.5.2.post3/types_aiobotocore_appintegrations/type_defs.pyi` & `types-aiobotocore-appintegrations-2.5.4/types_aiobotocore_appintegrations/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-appintegrations-2.5.2.post3/types_aiobotocore_appintegrations.egg-info/PKG-INFO` & `types-aiobotocore-appintegrations-2.5.4/types_aiobotocore_appintegrations.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-appintegrations
-Version: 2.5.2.post3
-Summary: Type annotations for aiobotocore.AppIntegrationsService 2.5.2 service generated with mypy-boto3-builder 7.17.2
+Version: 2.5.4
+Summary: Type annotations for aiobotocore.AppIntegrationsService 2.5.4 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appintegrations/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-appintegrations.svg?color=blue)](https://pypi.org/project/types-aiobotocore-appintegrations)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appintegrations/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-appintegrations)](https://pepy.tech/project/types-aiobotocore-appintegrations)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.AppIntegrationsService 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appintegrations.html#AppIntegrationsService)
+[aiobotocore.AppIntegrationsService 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appintegrations.html#AppIntegrationsService)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-appintegrations-2.5.2.post3/types_aiobotocore_appintegrations.egg-info/SOURCES.txt` & `types-aiobotocore-appintegrations-2.5.4/types_aiobotocore_appintegrations.egg-info/SOURCES.txt`

 * *Files identical despite different names*


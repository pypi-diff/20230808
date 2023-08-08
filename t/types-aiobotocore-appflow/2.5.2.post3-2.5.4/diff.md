# Comparing `tmp/types-aiobotocore-appflow-2.5.2.post3.tar.gz` & `tmp/types-aiobotocore-appflow-2.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-appflow-2.5.2.post3.tar", last modified: Fri Aug  4 12:37:16 2023, max compression
+gzip compressed data, was "types-aiobotocore-appflow-2.5.4.tar", last modified: Tue Aug  8 01:23:16 2023, max compression
```

## Comparing `types-aiobotocore-appflow-2.5.2.post3.tar` & `types-aiobotocore-appflow-2.5.4.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:37:16.371168 types-aiobotocore-appflow-2.5.2.post3/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-04 12:18:19.000000 types-aiobotocore-appflow-2.5.2.post3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    12196 2023-08-04 12:37:16.371168 types-aiobotocore-appflow-2.5.2.post3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    10678 2023-08-04 12:18:19.000000 types-aiobotocore-appflow-2.5.2.post3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-04 12:37:16.371168 types-aiobotocore-appflow-2.5.2.post3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2072 2023-08-04 12:18:19.000000 types-aiobotocore-appflow-2.5.2.post3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:37:16.367168 types-aiobotocore-appflow-2.5.2.post3/types_aiobotocore_appflow/
--rw-r--r--   0 runner    (1001) docker     (123)      442 2023-08-04 12:18:19.000000 types-aiobotocore-appflow-2.5.2.post3/types_aiobotocore_appflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      441 2023-08-04 12:18:19.000000 types-aiobotocore-appflow-2.5.2.post3/types_aiobotocore_appflow/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      943 2023-08-04 12:18:19.000000 types-aiobotocore-appflow-2.5.2.post3/types_aiobotocore_appflow/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    21145 2023-08-04 12:18:19.000000 types-aiobotocore-appflow-2.5.2.post3/types_aiobotocore_appflow/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    21111 2023-08-04 12:18:19.000000 types-aiobotocore-appflow-2.5.2.post3/types_aiobotocore_appflow/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    18362 2023-08-04 12:18:20.000000 types-aiobotocore-appflow-2.5.2.post3/types_aiobotocore_appflow/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    18360 2023-08-04 12:18:19.000000 types-aiobotocore-appflow-2.5.2.post3/types_aiobotocore_appflow/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 12:18:19.000000 types-aiobotocore-appflow-2.5.2.post3/types_aiobotocore_appflow/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    71159 2023-08-04 12:18:21.000000 types-aiobotocore-appflow-2.5.2.post3/types_aiobotocore_appflow/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    71057 2023-08-04 12:18:21.000000 types-aiobotocore-appflow-2.5.2.post3/types_aiobotocore_appflow/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-04 12:18:19.000000 types-aiobotocore-appflow-2.5.2.post3/types_aiobotocore_appflow/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:37:16.371168 types-aiobotocore-appflow-2.5.2.post3/types_aiobotocore_appflow.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    12196 2023-08-04 12:37:16.000000 types-aiobotocore-appflow-2.5.2.post3/types_aiobotocore_appflow.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      734 2023-08-04 12:37:16.000000 types-aiobotocore-appflow-2.5.2.post3/types_aiobotocore_appflow.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 12:37:16.000000 types-aiobotocore-appflow-2.5.2.post3/types_aiobotocore_appflow.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 12:37:16.000000 types-aiobotocore-appflow-2.5.2.post3/types_aiobotocore_appflow.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-04 12:37:16.000000 types-aiobotocore-appflow-2.5.2.post3/types_aiobotocore_appflow.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-08-04 12:37:16.000000 types-aiobotocore-appflow-2.5.2.post3/types_aiobotocore_appflow.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:23:16.934497 types-aiobotocore-appflow-2.5.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-08 01:06:07.000000 types-aiobotocore-appflow-2.5.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    12190 2023-08-08 01:23:16.934497 types-aiobotocore-appflow-2.5.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10678 2023-08-08 01:06:07.000000 types-aiobotocore-appflow-2.5.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-08 01:23:16.934497 types-aiobotocore-appflow-2.5.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2066 2023-08-08 01:06:07.000000 types-aiobotocore-appflow-2.5.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:23:16.930498 types-aiobotocore-appflow-2.5.4/types_aiobotocore_appflow/
+-rw-r--r--   0 runner    (1001) docker     (123)      442 2023-08-08 01:06:07.000000 types-aiobotocore-appflow-2.5.4/types_aiobotocore_appflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      441 2023-08-08 01:06:07.000000 types-aiobotocore-appflow-2.5.4/types_aiobotocore_appflow/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      931 2023-08-08 01:06:07.000000 types-aiobotocore-appflow-2.5.4/types_aiobotocore_appflow/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21145 2023-08-08 01:06:07.000000 types-aiobotocore-appflow-2.5.4/types_aiobotocore_appflow/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21111 2023-08-08 01:06:07.000000 types-aiobotocore-appflow-2.5.4/types_aiobotocore_appflow/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    18457 2023-08-08 01:06:07.000000 types-aiobotocore-appflow-2.5.4/types_aiobotocore_appflow/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18455 2023-08-08 01:06:07.000000 types-aiobotocore-appflow-2.5.4/types_aiobotocore_appflow/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 01:06:07.000000 types-aiobotocore-appflow-2.5.4/types_aiobotocore_appflow/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    71187 2023-08-08 01:06:09.000000 types-aiobotocore-appflow-2.5.4/types_aiobotocore_appflow/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    71085 2023-08-08 01:06:08.000000 types-aiobotocore-appflow-2.5.4/types_aiobotocore_appflow/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-08-08 01:06:07.000000 types-aiobotocore-appflow-2.5.4/types_aiobotocore_appflow/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:23:16.934497 types-aiobotocore-appflow-2.5.4/types_aiobotocore_appflow.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    12190 2023-08-08 01:23:16.000000 types-aiobotocore-appflow-2.5.4/types_aiobotocore_appflow.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      734 2023-08-08 01:23:16.000000 types-aiobotocore-appflow-2.5.4/types_aiobotocore_appflow.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 01:23:16.000000 types-aiobotocore-appflow-2.5.4/types_aiobotocore_appflow.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 01:23:16.000000 types-aiobotocore-appflow-2.5.4/types_aiobotocore_appflow.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-08 01:23:16.000000 types-aiobotocore-appflow-2.5.4/types_aiobotocore_appflow.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-08-08 01:23:16.000000 types-aiobotocore-appflow-2.5.4/types_aiobotocore_appflow.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-appflow-2.5.2.post3/LICENSE` & `types-aiobotocore-appflow-2.5.4/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-appflow-2.5.2.post3/PKG-INFO` & `types-aiobotocore-appflow-2.5.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-appflow
-Version: 2.5.2.post3
-Summary: Type annotations for aiobotocore.Appflow 2.5.2 service generated with mypy-boto3-builder 7.17.2
+Version: 2.5.4
+Summary: Type annotations for aiobotocore.Appflow 2.5.4 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appflow/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-appflow.svg?color=blue)](https://pypi.org/project/types-aiobotocore-appflow)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appflow/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-appflow)](https://pepy.tech/project/types-aiobotocore-appflow)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.Appflow 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appflow.html#Appflow)
+[aiobotocore.Appflow 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appflow.html#Appflow)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-appflow-2.5.2.post3/README.md` & `types-aiobotocore-appflow-2.5.4/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-appflow.svg?color=blue)](https://pypi.org/project/types-aiobotocore-appflow)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appflow/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-appflow)](https://pepy.tech/project/types-aiobotocore-appflow)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.Appflow 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appflow.html#Appflow)
+[aiobotocore.Appflow 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appflow.html#Appflow)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-appflow-2.5.2.post3/setup.py` & `types-aiobotocore-appflow-2.5.4/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-appflow",
-    version="2.5.2.post3",
+    version="2.5.4",
     packages=["types_aiobotocore_appflow"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.Appflow 2.5.2 service generated with mypy-boto3-builder"
+        "Type annotations for aiobotocore.Appflow 2.5.4 service generated with mypy-boto3-builder"
         " 7.17.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
```

### Comparing `types-aiobotocore-appflow-2.5.2.post3/types_aiobotocore_appflow/__main__.py` & `types-aiobotocore-appflow-2.5.4/types_aiobotocore_appflow/__main__.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.Appflow 2.5.2\nVersion:         2.5.2.post3\nBuilder"
-        " version: 7.17.2\nDocs:           "
+        "Type annotations for aiobotocore.Appflow 2.5.4\nVersion:         2.5.4\nBuilder version:"
+        " 7.17.2\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appflow//\nBoto3 docs:"
         "     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appflow.html#Appflow\nOther"
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

### Comparing `types-aiobotocore-appflow-2.5.2.post3/types_aiobotocore_appflow/client.py` & `types-aiobotocore-appflow-2.5.4/types_aiobotocore_appflow/client.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-appflow-2.5.2.post3/types_aiobotocore_appflow/client.pyi` & `types-aiobotocore-appflow-2.5.4/types_aiobotocore_appflow/client.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-appflow-2.5.2.post3/types_aiobotocore_appflow/literals.py` & `types-aiobotocore-appflow-2.5.4/types_aiobotocore_appflow/literals.py`

 * *Files 0% similar despite different names*

```diff
@@ -481,14 +481,15 @@
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
@@ -584,14 +585,15 @@
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
@@ -670,26 +672,28 @@
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

### Comparing `types-aiobotocore-appflow-2.5.2.post3/types_aiobotocore_appflow/literals.pyi` & `types-aiobotocore-appflow-2.5.4/types_aiobotocore_appflow/literals.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -479,14 +479,15 @@
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
@@ -582,14 +583,15 @@
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
@@ -668,26 +670,28 @@
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

### Comparing `types-aiobotocore-appflow-2.5.2.post3/types_aiobotocore_appflow/type_defs.py` & `types-aiobotocore-appflow-2.5.4/types_aiobotocore_appflow/type_defs.py`

 * *Files 0% similar despite different names*

```diff
@@ -1946,14 +1946,15 @@
 )
 _OptionalSAPODataConnectorProfilePropertiesTypeDef = TypedDict(
     "_OptionalSAPODataConnectorProfilePropertiesTypeDef",
     {
         "logonLanguage": str,
         "privateLinkServiceName": str,
         "oAuthProperties": OAuthPropertiesTypeDef,
+        "disableSSO": bool,
     },
     total=False,
 )
 
 
 class SAPODataConnectorProfilePropertiesTypeDef(
     _RequiredSAPODataConnectorProfilePropertiesTypeDef,
```

### Comparing `types-aiobotocore-appflow-2.5.2.post3/types_aiobotocore_appflow/type_defs.pyi` & `types-aiobotocore-appflow-2.5.4/types_aiobotocore_appflow/type_defs.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -1879,14 +1879,15 @@
 )
 _OptionalSAPODataConnectorProfilePropertiesTypeDef = TypedDict(
     "_OptionalSAPODataConnectorProfilePropertiesTypeDef",
     {
         "logonLanguage": str,
         "privateLinkServiceName": str,
         "oAuthProperties": OAuthPropertiesTypeDef,
+        "disableSSO": bool,
     },
     total=False,
 )
 
 class SAPODataConnectorProfilePropertiesTypeDef(
     _RequiredSAPODataConnectorProfilePropertiesTypeDef,
     _OptionalSAPODataConnectorProfilePropertiesTypeDef,
```

### Comparing `types-aiobotocore-appflow-2.5.2.post3/types_aiobotocore_appflow.egg-info/PKG-INFO` & `types-aiobotocore-appflow-2.5.4/types_aiobotocore_appflow.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-appflow
-Version: 2.5.2.post3
-Summary: Type annotations for aiobotocore.Appflow 2.5.2 service generated with mypy-boto3-builder 7.17.2
+Version: 2.5.4
+Summary: Type annotations for aiobotocore.Appflow 2.5.4 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appflow/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-appflow.svg?color=blue)](https://pypi.org/project/types-aiobotocore-appflow)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appflow/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-appflow)](https://pepy.tech/project/types-aiobotocore-appflow)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.Appflow 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appflow.html#Appflow)
+[aiobotocore.Appflow 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appflow.html#Appflow)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-appflow-2.5.2.post3/types_aiobotocore_appflow.egg-info/SOURCES.txt` & `types-aiobotocore-appflow-2.5.4/types_aiobotocore_appflow.egg-info/SOURCES.txt`

 * *Files identical despite different names*


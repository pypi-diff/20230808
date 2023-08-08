# Comparing `tmp/types-aiobotocore-chime-sdk-messaging-2.5.2.post3.tar.gz` & `tmp/types-aiobotocore-chime-sdk-messaging-2.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-chime-sdk-messaging-2.5.2.post3.tar", last modified: Fri Aug  4 12:37:23 2023, max compression
+gzip compressed data, was "types-aiobotocore-chime-sdk-messaging-2.5.4.tar", last modified: Tue Aug  8 01:23:24 2023, max compression
```

## Comparing `types-aiobotocore-chime-sdk-messaging-2.5.2.post3.tar` & `types-aiobotocore-chime-sdk-messaging-2.5.4.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:37:23.935333 types-aiobotocore-chime-sdk-messaging-2.5.2.post3/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-04 12:19:20.000000 types-aiobotocore-chime-sdk-messaging-2.5.2.post3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    12850 2023-08-04 12:37:23.935333 types-aiobotocore-chime-sdk-messaging-2.5.2.post3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    11286 2023-08-04 12:19:20.000000 types-aiobotocore-chime-sdk-messaging-2.5.2.post3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-04 12:37:23.935333 types-aiobotocore-chime-sdk-messaging-2.5.2.post3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2130 2023-08-04 12:19:19.000000 types-aiobotocore-chime-sdk-messaging-2.5.2.post3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:37:23.935333 types-aiobotocore-chime-sdk-messaging-2.5.2.post3/types_aiobotocore_chime_sdk_messaging/
--rw-r--r--   0 runner    (1001) docker     (123)      528 2023-08-04 12:19:20.000000 types-aiobotocore-chime-sdk-messaging-2.5.2.post3/types_aiobotocore_chime_sdk_messaging/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      527 2023-08-04 12:19:20.000000 types-aiobotocore-chime-sdk-messaging-2.5.2.post3/types_aiobotocore_chime_sdk_messaging/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      987 2023-08-04 12:19:20.000000 types-aiobotocore-chime-sdk-messaging-2.5.2.post3/types_aiobotocore_chime_sdk_messaging/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    40488 2023-08-04 12:19:21.000000 types-aiobotocore-chime-sdk-messaging-2.5.2.post3/types_aiobotocore_chime_sdk_messaging/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    40429 2023-08-04 12:19:20.000000 types-aiobotocore-chime-sdk-messaging-2.5.2.post3/types_aiobotocore_chime_sdk_messaging/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9351 2023-08-04 12:19:21.000000 types-aiobotocore-chime-sdk-messaging-2.5.2.post3/types_aiobotocore_chime_sdk_messaging/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     9349 2023-08-04 12:19:21.000000 types-aiobotocore-chime-sdk-messaging-2.5.2.post3/types_aiobotocore_chime_sdk_messaging/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 12:19:20.000000 types-aiobotocore-chime-sdk-messaging-2.5.2.post3/types_aiobotocore_chime_sdk_messaging/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    47633 2023-08-04 12:19:22.000000 types-aiobotocore-chime-sdk-messaging-2.5.2.post3/types_aiobotocore_chime_sdk_messaging/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    47576 2023-08-04 12:19:21.000000 types-aiobotocore-chime-sdk-messaging-2.5.2.post3/types_aiobotocore_chime_sdk_messaging/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-04 12:19:20.000000 types-aiobotocore-chime-sdk-messaging-2.5.2.post3/types_aiobotocore_chime_sdk_messaging/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:37:23.935333 types-aiobotocore-chime-sdk-messaging-2.5.2.post3/types_aiobotocore_chime_sdk_messaging.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    12850 2023-08-04 12:37:23.000000 types-aiobotocore-chime-sdk-messaging-2.5.2.post3/types_aiobotocore_chime_sdk_messaging.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      938 2023-08-04 12:37:23.000000 types-aiobotocore-chime-sdk-messaging-2.5.2.post3/types_aiobotocore_chime_sdk_messaging.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 12:37:23.000000 types-aiobotocore-chime-sdk-messaging-2.5.2.post3/types_aiobotocore_chime_sdk_messaging.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 12:37:23.000000 types-aiobotocore-chime-sdk-messaging-2.5.2.post3/types_aiobotocore_chime_sdk_messaging.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-04 12:37:23.000000 types-aiobotocore-chime-sdk-messaging-2.5.2.post3/types_aiobotocore_chime_sdk_messaging.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-04 12:37:23.000000 types-aiobotocore-chime-sdk-messaging-2.5.2.post3/types_aiobotocore_chime_sdk_messaging.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:23:24.142623 types-aiobotocore-chime-sdk-messaging-2.5.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-08 01:07:04.000000 types-aiobotocore-chime-sdk-messaging-2.5.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    12844 2023-08-08 01:23:24.134623 types-aiobotocore-chime-sdk-messaging-2.5.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    11286 2023-08-08 01:07:04.000000 types-aiobotocore-chime-sdk-messaging-2.5.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-08 01:23:24.142623 types-aiobotocore-chime-sdk-messaging-2.5.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2124 2023-08-08 01:07:04.000000 types-aiobotocore-chime-sdk-messaging-2.5.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:23:24.134623 types-aiobotocore-chime-sdk-messaging-2.5.4/types_aiobotocore_chime_sdk_messaging/
+-rw-r--r--   0 runner    (1001) docker     (123)      528 2023-08-08 01:07:04.000000 types-aiobotocore-chime-sdk-messaging-2.5.4/types_aiobotocore_chime_sdk_messaging/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      527 2023-08-08 01:07:04.000000 types-aiobotocore-chime-sdk-messaging-2.5.4/types_aiobotocore_chime_sdk_messaging/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      975 2023-08-08 01:07:04.000000 types-aiobotocore-chime-sdk-messaging-2.5.4/types_aiobotocore_chime_sdk_messaging/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40488 2023-08-08 01:07:04.000000 types-aiobotocore-chime-sdk-messaging-2.5.4/types_aiobotocore_chime_sdk_messaging/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40429 2023-08-08 01:07:04.000000 types-aiobotocore-chime-sdk-messaging-2.5.4/types_aiobotocore_chime_sdk_messaging/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9446 2023-08-08 01:07:04.000000 types-aiobotocore-chime-sdk-messaging-2.5.4/types_aiobotocore_chime_sdk_messaging/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9444 2023-08-08 01:07:04.000000 types-aiobotocore-chime-sdk-messaging-2.5.4/types_aiobotocore_chime_sdk_messaging/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 01:07:04.000000 types-aiobotocore-chime-sdk-messaging-2.5.4/types_aiobotocore_chime_sdk_messaging/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    47633 2023-08-08 01:07:06.000000 types-aiobotocore-chime-sdk-messaging-2.5.4/types_aiobotocore_chime_sdk_messaging/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    47576 2023-08-08 01:07:05.000000 types-aiobotocore-chime-sdk-messaging-2.5.4/types_aiobotocore_chime_sdk_messaging/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-08-08 01:07:04.000000 types-aiobotocore-chime-sdk-messaging-2.5.4/types_aiobotocore_chime_sdk_messaging/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:23:24.134623 types-aiobotocore-chime-sdk-messaging-2.5.4/types_aiobotocore_chime_sdk_messaging.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    12844 2023-08-08 01:23:23.000000 types-aiobotocore-chime-sdk-messaging-2.5.4/types_aiobotocore_chime_sdk_messaging.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      938 2023-08-08 01:23:23.000000 types-aiobotocore-chime-sdk-messaging-2.5.4/types_aiobotocore_chime_sdk_messaging.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 01:23:23.000000 types-aiobotocore-chime-sdk-messaging-2.5.4/types_aiobotocore_chime_sdk_messaging.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 01:23:23.000000 types-aiobotocore-chime-sdk-messaging-2.5.4/types_aiobotocore_chime_sdk_messaging.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-08 01:23:23.000000 types-aiobotocore-chime-sdk-messaging-2.5.4/types_aiobotocore_chime_sdk_messaging.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-08 01:23:23.000000 types-aiobotocore-chime-sdk-messaging-2.5.4/types_aiobotocore_chime_sdk_messaging.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-chime-sdk-messaging-2.5.2.post3/LICENSE` & `types-aiobotocore-chime-sdk-messaging-2.5.4/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-chime-sdk-messaging-2.5.2.post3/PKG-INFO` & `types-aiobotocore-chime-sdk-messaging-2.5.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-chime-sdk-messaging
-Version: 2.5.2.post3
-Summary: Type annotations for aiobotocore.ChimeSDKMessaging 2.5.2 service generated with mypy-boto3-builder 7.17.2
+Version: 2.5.4
+Summary: Type annotations for aiobotocore.ChimeSDKMessaging 2.5.4 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_chime_sdk_messaging/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-chime-sdk-messaging.svg?color=blue)](https://pypi.org/project/types-aiobotocore-chime-sdk-messaging)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_chime_sdk_messaging/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-chime-sdk-messaging)](https://pepy.tech/project/types-aiobotocore-chime-sdk-messaging)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.ChimeSDKMessaging 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-messaging.html#ChimeSDKMessaging)
+[aiobotocore.ChimeSDKMessaging 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-messaging.html#ChimeSDKMessaging)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-chime-sdk-messaging-2.5.2.post3/README.md` & `types-aiobotocore-chime-sdk-messaging-2.5.4/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-chime-sdk-messaging.svg?color=blue)](https://pypi.org/project/types-aiobotocore-chime-sdk-messaging)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_chime_sdk_messaging/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-chime-sdk-messaging)](https://pepy.tech/project/types-aiobotocore-chime-sdk-messaging)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.ChimeSDKMessaging 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-messaging.html#ChimeSDKMessaging)
+[aiobotocore.ChimeSDKMessaging 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-messaging.html#ChimeSDKMessaging)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-chime-sdk-messaging-2.5.2.post3/setup.py` & `types-aiobotocore-chime-sdk-messaging-2.5.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-chime-sdk-messaging",
-    version="2.5.2.post3",
+    version="2.5.4",
     packages=["types_aiobotocore_chime_sdk_messaging"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.ChimeSDKMessaging 2.5.2 service generated with"
+        "Type annotations for aiobotocore.ChimeSDKMessaging 2.5.4 service generated with"
         " mypy-boto3-builder 7.17.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
```

### Comparing `types-aiobotocore-chime-sdk-messaging-2.5.2.post3/types_aiobotocore_chime_sdk_messaging/__init__.py` & `types-aiobotocore-chime-sdk-messaging-2.5.4/types_aiobotocore_chime_sdk_messaging/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-chime-sdk-messaging-2.5.2.post3/types_aiobotocore_chime_sdk_messaging/__init__.pyi` & `types-aiobotocore-chime-sdk-messaging-2.5.4/types_aiobotocore_chime_sdk_messaging/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-chime-sdk-messaging-2.5.2.post3/types_aiobotocore_chime_sdk_messaging/__main__.py` & `types-aiobotocore-chime-sdk-messaging-2.5.4/types_aiobotocore_chime_sdk_messaging/__main__.py`

 * *Files 13% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.ChimeSDKMessaging 2.5.2\nVersion:        "
-        " 2.5.2.post3\nBuilder version: 7.17.2\nDocs:           "
+        "Type annotations for aiobotocore.ChimeSDKMessaging 2.5.4\nVersion:         2.5.4\nBuilder"
+        " version: 7.17.2\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_chime_sdk_messaging//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-messaging.html#ChimeSDKMessaging\nOther"
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

### Comparing `types-aiobotocore-chime-sdk-messaging-2.5.2.post3/types_aiobotocore_chime_sdk_messaging/client.py` & `types-aiobotocore-chime-sdk-messaging-2.5.4/types_aiobotocore_chime_sdk_messaging/client.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-chime-sdk-messaging-2.5.2.post3/types_aiobotocore_chime_sdk_messaging/client.pyi` & `types-aiobotocore-chime-sdk-messaging-2.5.4/types_aiobotocore_chime_sdk_messaging/client.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-chime-sdk-messaging-2.5.2.post3/types_aiobotocore_chime_sdk_messaging/literals.py` & `types-aiobotocore-chime-sdk-messaging-2.5.4/types_aiobotocore_chime_sdk_messaging/literals.py`

 * *Files 1% similar despite different names*

```diff
@@ -87,14 +87,15 @@
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
@@ -190,14 +191,15 @@
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
@@ -276,26 +278,28 @@
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

### Comparing `types-aiobotocore-chime-sdk-messaging-2.5.2.post3/types_aiobotocore_chime_sdk_messaging/literals.pyi` & `types-aiobotocore-chime-sdk-messaging-2.5.4/types_aiobotocore_chime_sdk_messaging/literals.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -85,14 +85,15 @@
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
@@ -188,14 +189,15 @@
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
@@ -274,26 +276,28 @@
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

### Comparing `types-aiobotocore-chime-sdk-messaging-2.5.2.post3/types_aiobotocore_chime_sdk_messaging/type_defs.py` & `types-aiobotocore-chime-sdk-messaging-2.5.4/types_aiobotocore_chime_sdk_messaging/type_defs.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-chime-sdk-messaging-2.5.2.post3/types_aiobotocore_chime_sdk_messaging/type_defs.pyi` & `types-aiobotocore-chime-sdk-messaging-2.5.4/types_aiobotocore_chime_sdk_messaging/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-chime-sdk-messaging-2.5.2.post3/types_aiobotocore_chime_sdk_messaging.egg-info/PKG-INFO` & `types-aiobotocore-chime-sdk-messaging-2.5.4/types_aiobotocore_chime_sdk_messaging.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-chime-sdk-messaging
-Version: 2.5.2.post3
-Summary: Type annotations for aiobotocore.ChimeSDKMessaging 2.5.2 service generated with mypy-boto3-builder 7.17.2
+Version: 2.5.4
+Summary: Type annotations for aiobotocore.ChimeSDKMessaging 2.5.4 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_chime_sdk_messaging/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-chime-sdk-messaging.svg?color=blue)](https://pypi.org/project/types-aiobotocore-chime-sdk-messaging)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_chime_sdk_messaging/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-chime-sdk-messaging)](https://pepy.tech/project/types-aiobotocore-chime-sdk-messaging)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.ChimeSDKMessaging 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-messaging.html#ChimeSDKMessaging)
+[aiobotocore.ChimeSDKMessaging 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-messaging.html#ChimeSDKMessaging)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-chime-sdk-messaging-2.5.2.post3/types_aiobotocore_chime_sdk_messaging.egg-info/SOURCES.txt` & `types-aiobotocore-chime-sdk-messaging-2.5.4/types_aiobotocore_chime_sdk_messaging.egg-info/SOURCES.txt`

 * *Files identical despite different names*

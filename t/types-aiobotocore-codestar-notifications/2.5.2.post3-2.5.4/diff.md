# Comparing `tmp/types-aiobotocore-codestar-notifications-2.5.2.post3.tar.gz` & `tmp/types-aiobotocore-codestar-notifications-2.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-codestar-notifications-2.5.2.post3.tar", last modified: Fri Aug  4 12:37:29 2023, max compression
+gzip compressed data, was "types-aiobotocore-codestar-notifications-2.5.4.tar", last modified: Tue Aug  8 01:23:30 2023, max compression
```

## Comparing `types-aiobotocore-codestar-notifications-2.5.2.post3.tar` & `types-aiobotocore-codestar-notifications-2.5.4.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:37:29.127462 types-aiobotocore-codestar-notifications-2.5.2.post3/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-04 12:20:23.000000 types-aiobotocore-codestar-notifications-2.5.2.post3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    14044 2023-08-04 12:37:29.123461 types-aiobotocore-codestar-notifications-2.5.2.post3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    12467 2023-08-04 12:20:23.000000 types-aiobotocore-codestar-notifications-2.5.2.post3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-04 12:37:29.127462 types-aiobotocore-codestar-notifications-2.5.2.post3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2168 2023-08-04 12:20:23.000000 types-aiobotocore-codestar-notifications-2.5.2.post3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:37:29.123461 types-aiobotocore-codestar-notifications-2.5.2.post3/types_aiobotocore_codestar_notifications/
--rw-r--r--   0 runner    (1001) docker     (123)     1177 2023-08-04 12:20:23.000000 types-aiobotocore-codestar-notifications-2.5.2.post3/types_aiobotocore_codestar_notifications/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1176 2023-08-04 12:20:23.000000 types-aiobotocore-codestar-notifications-2.5.2.post3/types_aiobotocore_codestar_notifications/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1001 2023-08-04 12:20:23.000000 types-aiobotocore-codestar-notifications-2.5.2.post3/types_aiobotocore_codestar_notifications/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15312 2023-08-04 12:20:23.000000 types-aiobotocore-codestar-notifications-2.5.2.post3/types_aiobotocore_codestar_notifications/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    15287 2023-08-04 12:20:23.000000 types-aiobotocore-codestar-notifications-2.5.2.post3/types_aiobotocore_codestar_notifications/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9028 2023-08-04 12:20:24.000000 types-aiobotocore-codestar-notifications-2.5.2.post3/types_aiobotocore_codestar_notifications/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     9026 2023-08-04 12:20:23.000000 types-aiobotocore-codestar-notifications-2.5.2.post3/types_aiobotocore_codestar_notifications/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     4857 2023-08-04 12:20:23.000000 types-aiobotocore-codestar-notifications-2.5.2.post3/types_aiobotocore_codestar_notifications/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     4852 2023-08-04 12:20:23.000000 types-aiobotocore-codestar-notifications-2.5.2.post3/types_aiobotocore_codestar_notifications/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 12:20:23.000000 types-aiobotocore-codestar-notifications-2.5.2.post3/types_aiobotocore_codestar_notifications/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    10925 2023-08-04 12:20:25.000000 types-aiobotocore-codestar-notifications-2.5.2.post3/types_aiobotocore_codestar_notifications/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    10916 2023-08-04 12:20:24.000000 types-aiobotocore-codestar-notifications-2.5.2.post3/types_aiobotocore_codestar_notifications/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-04 12:20:23.000000 types-aiobotocore-codestar-notifications-2.5.2.post3/types_aiobotocore_codestar_notifications/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:37:29.123461 types-aiobotocore-codestar-notifications-2.5.2.post3/types_aiobotocore_codestar_notifications.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    14044 2023-08-04 12:37:28.000000 types-aiobotocore-codestar-notifications-2.5.2.post3/types_aiobotocore_codestar_notifications.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1098 2023-08-04 12:37:28.000000 types-aiobotocore-codestar-notifications-2.5.2.post3/types_aiobotocore_codestar_notifications.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 12:37:28.000000 types-aiobotocore-codestar-notifications-2.5.2.post3/types_aiobotocore_codestar_notifications.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 12:37:28.000000 types-aiobotocore-codestar-notifications-2.5.2.post3/types_aiobotocore_codestar_notifications.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-04 12:37:28.000000 types-aiobotocore-codestar-notifications-2.5.2.post3/types_aiobotocore_codestar_notifications.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-08-04 12:37:28.000000 types-aiobotocore-codestar-notifications-2.5.2.post3/types_aiobotocore_codestar_notifications.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:23:30.250658 types-aiobotocore-codestar-notifications-2.5.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-08 01:08:02.000000 types-aiobotocore-codestar-notifications-2.5.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    14038 2023-08-08 01:23:30.250658 types-aiobotocore-codestar-notifications-2.5.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    12467 2023-08-08 01:08:02.000000 types-aiobotocore-codestar-notifications-2.5.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-08 01:23:30.250658 types-aiobotocore-codestar-notifications-2.5.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2162 2023-08-08 01:08:02.000000 types-aiobotocore-codestar-notifications-2.5.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:23:30.242658 types-aiobotocore-codestar-notifications-2.5.4/types_aiobotocore_codestar_notifications/
+-rw-r--r--   0 runner    (1001) docker     (123)     1177 2023-08-08 01:08:02.000000 types-aiobotocore-codestar-notifications-2.5.4/types_aiobotocore_codestar_notifications/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1176 2023-08-08 01:08:02.000000 types-aiobotocore-codestar-notifications-2.5.4/types_aiobotocore_codestar_notifications/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      989 2023-08-08 01:08:02.000000 types-aiobotocore-codestar-notifications-2.5.4/types_aiobotocore_codestar_notifications/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15312 2023-08-08 01:08:02.000000 types-aiobotocore-codestar-notifications-2.5.4/types_aiobotocore_codestar_notifications/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15287 2023-08-08 01:08:02.000000 types-aiobotocore-codestar-notifications-2.5.4/types_aiobotocore_codestar_notifications/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9123 2023-08-08 01:08:03.000000 types-aiobotocore-codestar-notifications-2.5.4/types_aiobotocore_codestar_notifications/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9121 2023-08-08 01:08:02.000000 types-aiobotocore-codestar-notifications-2.5.4/types_aiobotocore_codestar_notifications/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     4857 2023-08-08 01:08:02.000000 types-aiobotocore-codestar-notifications-2.5.4/types_aiobotocore_codestar_notifications/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4852 2023-08-08 01:08:02.000000 types-aiobotocore-codestar-notifications-2.5.4/types_aiobotocore_codestar_notifications/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 01:08:02.000000 types-aiobotocore-codestar-notifications-2.5.4/types_aiobotocore_codestar_notifications/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    10925 2023-08-08 01:08:03.000000 types-aiobotocore-codestar-notifications-2.5.4/types_aiobotocore_codestar_notifications/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10916 2023-08-08 01:08:03.000000 types-aiobotocore-codestar-notifications-2.5.4/types_aiobotocore_codestar_notifications/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-08-08 01:08:02.000000 types-aiobotocore-codestar-notifications-2.5.4/types_aiobotocore_codestar_notifications/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:23:30.250658 types-aiobotocore-codestar-notifications-2.5.4/types_aiobotocore_codestar_notifications.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    14038 2023-08-08 01:23:30.000000 types-aiobotocore-codestar-notifications-2.5.4/types_aiobotocore_codestar_notifications.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1098 2023-08-08 01:23:30.000000 types-aiobotocore-codestar-notifications-2.5.4/types_aiobotocore_codestar_notifications.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 01:23:30.000000 types-aiobotocore-codestar-notifications-2.5.4/types_aiobotocore_codestar_notifications.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 01:23:30.000000 types-aiobotocore-codestar-notifications-2.5.4/types_aiobotocore_codestar_notifications.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-08 01:23:30.000000 types-aiobotocore-codestar-notifications-2.5.4/types_aiobotocore_codestar_notifications.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-08-08 01:23:30.000000 types-aiobotocore-codestar-notifications-2.5.4/types_aiobotocore_codestar_notifications.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-codestar-notifications-2.5.2.post3/LICENSE` & `types-aiobotocore-codestar-notifications-2.5.4/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-codestar-notifications-2.5.2.post3/PKG-INFO` & `types-aiobotocore-codestar-notifications-2.5.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-codestar-notifications
-Version: 2.5.2.post3
-Summary: Type annotations for aiobotocore.CodeStarNotifications 2.5.2 service generated with mypy-boto3-builder 7.17.2
+Version: 2.5.4
+Summary: Type annotations for aiobotocore.CodeStarNotifications 2.5.4 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codestar_notifications/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-codestar-notifications.svg?color=blue)](https://pypi.org/project/types-aiobotocore-codestar-notifications)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codestar_notifications/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-codestar-notifications)](https://pepy.tech/project/types-aiobotocore-codestar-notifications)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.CodeStarNotifications 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codestar-notifications.html#CodeStarNotifications)
+[aiobotocore.CodeStarNotifications 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codestar-notifications.html#CodeStarNotifications)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-codestar-notifications-2.5.2.post3/README.md` & `types-aiobotocore-codestar-notifications-2.5.4/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-codestar-notifications.svg?color=blue)](https://pypi.org/project/types-aiobotocore-codestar-notifications)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codestar_notifications/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-codestar-notifications)](https://pepy.tech/project/types-aiobotocore-codestar-notifications)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.CodeStarNotifications 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codestar-notifications.html#CodeStarNotifications)
+[aiobotocore.CodeStarNotifications 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codestar-notifications.html#CodeStarNotifications)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-codestar-notifications-2.5.2.post3/setup.py` & `types-aiobotocore-codestar-notifications-2.5.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-codestar-notifications",
-    version="2.5.2.post3",
+    version="2.5.4",
     packages=["types_aiobotocore_codestar_notifications"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.CodeStarNotifications 2.5.2 service generated with"
+        "Type annotations for aiobotocore.CodeStarNotifications 2.5.4 service generated with"
         " mypy-boto3-builder 7.17.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
```

### Comparing `types-aiobotocore-codestar-notifications-2.5.2.post3/types_aiobotocore_codestar_notifications/__init__.py` & `types-aiobotocore-codestar-notifications-2.5.4/types_aiobotocore_codestar_notifications/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-codestar-notifications-2.5.2.post3/types_aiobotocore_codestar_notifications/__init__.pyi` & `types-aiobotocore-codestar-notifications-2.5.4/types_aiobotocore_codestar_notifications/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-codestar-notifications-2.5.2.post3/types_aiobotocore_codestar_notifications/__main__.py` & `types-aiobotocore-codestar-notifications-2.5.4/types_aiobotocore_codestar_notifications/__main__.py`

 * *Files 22% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.CodeStarNotifications 2.5.2\nVersion:        "
-        " 2.5.2.post3\nBuilder version: 7.17.2\nDocs:           "
+        "Type annotations for aiobotocore.CodeStarNotifications 2.5.4\nVersion:        "
+        " 2.5.4\nBuilder version: 7.17.2\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codestar_notifications//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codestar-notifications.html#CodeStarNotifications\nOther"
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

### Comparing `types-aiobotocore-codestar-notifications-2.5.2.post3/types_aiobotocore_codestar_notifications/client.py` & `types-aiobotocore-codestar-notifications-2.5.4/types_aiobotocore_codestar_notifications/client.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-codestar-notifications-2.5.2.post3/types_aiobotocore_codestar_notifications/client.pyi` & `types-aiobotocore-codestar-notifications-2.5.4/types_aiobotocore_codestar_notifications/client.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-codestar-notifications-2.5.2.post3/types_aiobotocore_codestar_notifications/literals.py` & `types-aiobotocore-codestar-notifications-2.5.4/types_aiobotocore_codestar_notifications/literals.py`

 * *Files 0% similar despite different names*

```diff
@@ -60,14 +60,15 @@
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
@@ -163,14 +164,15 @@
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
@@ -249,26 +251,28 @@
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

### Comparing `types-aiobotocore-codestar-notifications-2.5.2.post3/types_aiobotocore_codestar_notifications/literals.pyi` & `types-aiobotocore-codestar-notifications-2.5.4/types_aiobotocore_codestar_notifications/literals.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -58,14 +58,15 @@
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
@@ -161,14 +162,15 @@
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
@@ -247,26 +249,28 @@
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

### Comparing `types-aiobotocore-codestar-notifications-2.5.2.post3/types_aiobotocore_codestar_notifications/paginator.py` & `types-aiobotocore-codestar-notifications-2.5.4/types_aiobotocore_codestar_notifications/paginator.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-codestar-notifications-2.5.2.post3/types_aiobotocore_codestar_notifications/paginator.pyi` & `types-aiobotocore-codestar-notifications-2.5.4/types_aiobotocore_codestar_notifications/paginator.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-codestar-notifications-2.5.2.post3/types_aiobotocore_codestar_notifications/type_defs.py` & `types-aiobotocore-codestar-notifications-2.5.4/types_aiobotocore_codestar_notifications/type_defs.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-codestar-notifications-2.5.2.post3/types_aiobotocore_codestar_notifications/type_defs.pyi` & `types-aiobotocore-codestar-notifications-2.5.4/types_aiobotocore_codestar_notifications/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-codestar-notifications-2.5.2.post3/types_aiobotocore_codestar_notifications.egg-info/PKG-INFO` & `types-aiobotocore-codestar-notifications-2.5.4/types_aiobotocore_codestar_notifications.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-codestar-notifications
-Version: 2.5.2.post3
-Summary: Type annotations for aiobotocore.CodeStarNotifications 2.5.2 service generated with mypy-boto3-builder 7.17.2
+Version: 2.5.4
+Summary: Type annotations for aiobotocore.CodeStarNotifications 2.5.4 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codestar_notifications/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-codestar-notifications.svg?color=blue)](https://pypi.org/project/types-aiobotocore-codestar-notifications)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codestar_notifications/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-codestar-notifications)](https://pepy.tech/project/types-aiobotocore-codestar-notifications)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.CodeStarNotifications 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codestar-notifications.html#CodeStarNotifications)
+[aiobotocore.CodeStarNotifications 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codestar-notifications.html#CodeStarNotifications)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-codestar-notifications-2.5.2.post3/types_aiobotocore_codestar_notifications.egg-info/SOURCES.txt` & `types-aiobotocore-codestar-notifications-2.5.4/types_aiobotocore_codestar_notifications.egg-info/SOURCES.txt`

 * *Files identical despite different names*


# Comparing `tmp/types-aiobotocore-gamelift-2.5.2.post3.tar.gz` & `tmp/types-aiobotocore-gamelift-2.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-gamelift-2.5.2.post3.tar", last modified: Fri Aug  4 12:37:46 2023, max compression
+gzip compressed data, was "types-aiobotocore-gamelift-2.5.4.tar", last modified: Tue Aug  8 01:23:45 2023, max compression
```

## Comparing `types-aiobotocore-gamelift-2.5.2.post3.tar` & `types-aiobotocore-gamelift-2.5.4.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:37:46.127868 types-aiobotocore-gamelift-2.5.2.post3/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-04 12:24:09.000000 types-aiobotocore-gamelift-2.5.2.post3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    16377 2023-08-04 12:37:46.127868 types-aiobotocore-gamelift-2.5.2.post3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    14855 2023-08-04 12:24:09.000000 types-aiobotocore-gamelift-2.5.2.post3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-04 12:37:46.127868 types-aiobotocore-gamelift-2.5.2.post3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2079 2023-08-04 12:24:09.000000 types-aiobotocore-gamelift-2.5.2.post3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:37:46.119867 types-aiobotocore-gamelift-2.5.2.post3/types_aiobotocore_gamelift/
--rw-r--r--   0 runner    (1001) docker     (123)     5417 2023-08-04 12:24:09.000000 types-aiobotocore-gamelift-2.5.2.post3/types_aiobotocore_gamelift/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5416 2023-08-04 12:24:09.000000 types-aiobotocore-gamelift-2.5.2.post3/types_aiobotocore_gamelift/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      947 2023-08-04 12:24:09.000000 types-aiobotocore-gamelift-2.5.2.post3/types_aiobotocore_gamelift/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    88653 2023-08-04 12:24:10.000000 types-aiobotocore-gamelift-2.5.2.post3/types_aiobotocore_gamelift/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    88518 2023-08-04 12:24:09.000000 types-aiobotocore-gamelift-2.5.2.post3/types_aiobotocore_gamelift/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    20628 2023-08-04 12:24:10.000000 types-aiobotocore-gamelift-2.5.2.post3/types_aiobotocore_gamelift/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    20626 2023-08-04 12:24:10.000000 types-aiobotocore-gamelift-2.5.2.post3/types_aiobotocore_gamelift/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    27633 2023-08-04 12:24:10.000000 types-aiobotocore-gamelift-2.5.2.post3/types_aiobotocore_gamelift/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)    27609 2023-08-04 12:24:10.000000 types-aiobotocore-gamelift-2.5.2.post3/types_aiobotocore_gamelift/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 12:24:09.000000 types-aiobotocore-gamelift-2.5.2.post3/types_aiobotocore_gamelift/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    98077 2023-08-04 12:24:14.000000 types-aiobotocore-gamelift-2.5.2.post3/types_aiobotocore_gamelift/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    97978 2023-08-04 12:24:13.000000 types-aiobotocore-gamelift-2.5.2.post3/types_aiobotocore_gamelift/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-04 12:24:09.000000 types-aiobotocore-gamelift-2.5.2.post3/types_aiobotocore_gamelift/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:37:46.127868 types-aiobotocore-gamelift-2.5.2.post3/types_aiobotocore_gamelift.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    16377 2023-08-04 12:37:45.000000 types-aiobotocore-gamelift-2.5.2.post3/types_aiobotocore_gamelift.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      832 2023-08-04 12:37:45.000000 types-aiobotocore-gamelift-2.5.2.post3/types_aiobotocore_gamelift.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 12:37:45.000000 types-aiobotocore-gamelift-2.5.2.post3/types_aiobotocore_gamelift.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 12:37:45.000000 types-aiobotocore-gamelift-2.5.2.post3/types_aiobotocore_gamelift.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-04 12:37:45.000000 types-aiobotocore-gamelift-2.5.2.post3/types_aiobotocore_gamelift.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-08-04 12:37:45.000000 types-aiobotocore-gamelift-2.5.2.post3/types_aiobotocore_gamelift.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:23:45.770721 types-aiobotocore-gamelift-2.5.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-08 01:11:32.000000 types-aiobotocore-gamelift-2.5.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    16371 2023-08-08 01:23:45.770721 types-aiobotocore-gamelift-2.5.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    14855 2023-08-08 01:11:32.000000 types-aiobotocore-gamelift-2.5.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-08 01:23:45.770721 types-aiobotocore-gamelift-2.5.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2073 2023-08-08 01:11:32.000000 types-aiobotocore-gamelift-2.5.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:23:45.758721 types-aiobotocore-gamelift-2.5.4/types_aiobotocore_gamelift/
+-rw-r--r--   0 runner    (1001) docker     (123)     5417 2023-08-08 01:11:32.000000 types-aiobotocore-gamelift-2.5.4/types_aiobotocore_gamelift/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5416 2023-08-08 01:11:32.000000 types-aiobotocore-gamelift-2.5.4/types_aiobotocore_gamelift/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      935 2023-08-08 01:11:32.000000 types-aiobotocore-gamelift-2.5.4/types_aiobotocore_gamelift/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    88653 2023-08-08 01:11:32.000000 types-aiobotocore-gamelift-2.5.4/types_aiobotocore_gamelift/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    88518 2023-08-08 01:11:32.000000 types-aiobotocore-gamelift-2.5.4/types_aiobotocore_gamelift/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    20750 2023-08-08 01:11:33.000000 types-aiobotocore-gamelift-2.5.4/types_aiobotocore_gamelift/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20748 2023-08-08 01:11:33.000000 types-aiobotocore-gamelift-2.5.4/types_aiobotocore_gamelift/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    27633 2023-08-08 01:11:33.000000 types-aiobotocore-gamelift-2.5.4/types_aiobotocore_gamelift/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27609 2023-08-08 01:11:32.000000 types-aiobotocore-gamelift-2.5.4/types_aiobotocore_gamelift/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 01:11:32.000000 types-aiobotocore-gamelift-2.5.4/types_aiobotocore_gamelift/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    98077 2023-08-08 01:11:36.000000 types-aiobotocore-gamelift-2.5.4/types_aiobotocore_gamelift/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    97978 2023-08-08 01:11:35.000000 types-aiobotocore-gamelift-2.5.4/types_aiobotocore_gamelift/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-08-08 01:11:32.000000 types-aiobotocore-gamelift-2.5.4/types_aiobotocore_gamelift/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:23:45.770721 types-aiobotocore-gamelift-2.5.4/types_aiobotocore_gamelift.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    16371 2023-08-08 01:23:45.000000 types-aiobotocore-gamelift-2.5.4/types_aiobotocore_gamelift.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      832 2023-08-08 01:23:45.000000 types-aiobotocore-gamelift-2.5.4/types_aiobotocore_gamelift.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 01:23:45.000000 types-aiobotocore-gamelift-2.5.4/types_aiobotocore_gamelift.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 01:23:45.000000 types-aiobotocore-gamelift-2.5.4/types_aiobotocore_gamelift.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-08 01:23:45.000000 types-aiobotocore-gamelift-2.5.4/types_aiobotocore_gamelift.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-08-08 01:23:45.000000 types-aiobotocore-gamelift-2.5.4/types_aiobotocore_gamelift.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-gamelift-2.5.2.post3/LICENSE` & `types-aiobotocore-gamelift-2.5.4/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-gamelift-2.5.2.post3/PKG-INFO` & `types-aiobotocore-gamelift-2.5.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-gamelift
-Version: 2.5.2.post3
-Summary: Type annotations for aiobotocore.GameLift 2.5.2 service generated with mypy-boto3-builder 7.17.2
+Version: 2.5.4
+Summary: Type annotations for aiobotocore.GameLift 2.5.4 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_gamelift/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-gamelift.svg?color=blue)](https://pypi.org/project/types-aiobotocore-gamelift)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_gamelift/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-gamelift)](https://pepy.tech/project/types-aiobotocore-gamelift)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.GameLift 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamelift.html#GameLift)
+[aiobotocore.GameLift 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamelift.html#GameLift)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-gamelift-2.5.2.post3/README.md` & `types-aiobotocore-gamelift-2.5.4/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-gamelift.svg?color=blue)](https://pypi.org/project/types-aiobotocore-gamelift)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_gamelift/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-gamelift)](https://pepy.tech/project/types-aiobotocore-gamelift)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.GameLift 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamelift.html#GameLift)
+[aiobotocore.GameLift 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamelift.html#GameLift)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-gamelift-2.5.2.post3/setup.py` & `types-aiobotocore-gamelift-2.5.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-gamelift",
-    version="2.5.2.post3",
+    version="2.5.4",
     packages=["types_aiobotocore_gamelift"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.GameLift 2.5.2 service generated with mypy-boto3-builder"
+        "Type annotations for aiobotocore.GameLift 2.5.4 service generated with mypy-boto3-builder"
         " 7.17.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
```

### Comparing `types-aiobotocore-gamelift-2.5.2.post3/types_aiobotocore_gamelift/__init__.py` & `types-aiobotocore-gamelift-2.5.4/types_aiobotocore_gamelift/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-gamelift-2.5.2.post3/types_aiobotocore_gamelift/__init__.pyi` & `types-aiobotocore-gamelift-2.5.4/types_aiobotocore_gamelift/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-gamelift-2.5.2.post3/types_aiobotocore_gamelift/__main__.py` & `types-aiobotocore-gamelift-2.5.4/types_aiobotocore_gamelift/__main__.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.GameLift 2.5.2\nVersion:         2.5.2.post3\nBuilder"
-        " version: 7.17.2\nDocs:           "
+        "Type annotations for aiobotocore.GameLift 2.5.4\nVersion:         2.5.4\nBuilder version:"
+        " 7.17.2\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_gamelift//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamelift.html#GameLift\nOther"
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

### Comparing `types-aiobotocore-gamelift-2.5.2.post3/types_aiobotocore_gamelift/client.py` & `types-aiobotocore-gamelift-2.5.4/types_aiobotocore_gamelift/client.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-gamelift-2.5.2.post3/types_aiobotocore_gamelift/client.pyi` & `types-aiobotocore-gamelift-2.5.4/types_aiobotocore_gamelift/client.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-gamelift-2.5.2.post3/types_aiobotocore_gamelift/literals.py` & `types-aiobotocore-gamelift-2.5.4/types_aiobotocore_gamelift/literals.py`

 * *Files 1% similar despite different names*

```diff
@@ -422,15 +422,17 @@
     "CurrentPlayerSessions",
     "IdleInstances",
     "PercentAvailableGameSessions",
     "PercentIdleInstances",
     "QueueDepth",
     "WaitTime",
 ]
-OperatingSystemType = Literal["AMAZON_LINUX", "AMAZON_LINUX_2", "WINDOWS_2012", "WINDOWS_2016"]
+OperatingSystemType = Literal[
+    "AMAZON_LINUX", "AMAZON_LINUX_2", "AMAZON_LINUX_2023", "WINDOWS_2012", "WINDOWS_2016"
+]
 PlayerSessionCreationPolicyType = Literal["ACCEPT_ALL", "DENY_ALL"]
 PlayerSessionStatusType = Literal["ACTIVE", "COMPLETED", "RESERVED", "TIMEDOUT"]
 PolicyTypeType = Literal["RuleBased", "TargetBased"]
 PriorityTypeType = Literal["COST", "DESTINATION", "LATENCY", "LOCATION"]
 ProtectionPolicyType = Literal["FullProtection", "NoProtection"]
 RoutingStrategyTypeType = Literal["SIMPLE", "TERMINAL"]
 ScalingAdjustmentTypeType = Literal["ChangeInCapacity", "ExactCapacity", "PercentChangeInCapacity"]
@@ -451,14 +453,15 @@
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
@@ -554,14 +557,15 @@
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
@@ -640,26 +644,28 @@
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

### Comparing `types-aiobotocore-gamelift-2.5.2.post3/types_aiobotocore_gamelift/literals.pyi` & `types-aiobotocore-gamelift-2.5.4/types_aiobotocore_gamelift/literals.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -420,15 +420,17 @@
     "CurrentPlayerSessions",
     "IdleInstances",
     "PercentAvailableGameSessions",
     "PercentIdleInstances",
     "QueueDepth",
     "WaitTime",
 ]
-OperatingSystemType = Literal["AMAZON_LINUX", "AMAZON_LINUX_2", "WINDOWS_2012", "WINDOWS_2016"]
+OperatingSystemType = Literal[
+    "AMAZON_LINUX", "AMAZON_LINUX_2", "AMAZON_LINUX_2023", "WINDOWS_2012", "WINDOWS_2016"
+]
 PlayerSessionCreationPolicyType = Literal["ACCEPT_ALL", "DENY_ALL"]
 PlayerSessionStatusType = Literal["ACTIVE", "COMPLETED", "RESERVED", "TIMEDOUT"]
 PolicyTypeType = Literal["RuleBased", "TargetBased"]
 PriorityTypeType = Literal["COST", "DESTINATION", "LATENCY", "LOCATION"]
 ProtectionPolicyType = Literal["FullProtection", "NoProtection"]
 RoutingStrategyTypeType = Literal["SIMPLE", "TERMINAL"]
 ScalingAdjustmentTypeType = Literal["ChangeInCapacity", "ExactCapacity", "PercentChangeInCapacity"]
@@ -449,14 +451,15 @@
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
@@ -552,14 +555,15 @@
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
@@ -638,26 +642,28 @@
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

### Comparing `types-aiobotocore-gamelift-2.5.2.post3/types_aiobotocore_gamelift/paginator.py` & `types-aiobotocore-gamelift-2.5.4/types_aiobotocore_gamelift/paginator.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-gamelift-2.5.2.post3/types_aiobotocore_gamelift/paginator.pyi` & `types-aiobotocore-gamelift-2.5.4/types_aiobotocore_gamelift/paginator.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-gamelift-2.5.2.post3/types_aiobotocore_gamelift/type_defs.py` & `types-aiobotocore-gamelift-2.5.4/types_aiobotocore_gamelift/type_defs.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-gamelift-2.5.2.post3/types_aiobotocore_gamelift/type_defs.pyi` & `types-aiobotocore-gamelift-2.5.4/types_aiobotocore_gamelift/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-gamelift-2.5.2.post3/types_aiobotocore_gamelift.egg-info/PKG-INFO` & `types-aiobotocore-gamelift-2.5.4/types_aiobotocore_gamelift.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-gamelift
-Version: 2.5.2.post3
-Summary: Type annotations for aiobotocore.GameLift 2.5.2 service generated with mypy-boto3-builder 7.17.2
+Version: 2.5.4
+Summary: Type annotations for aiobotocore.GameLift 2.5.4 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_gamelift/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-gamelift.svg?color=blue)](https://pypi.org/project/types-aiobotocore-gamelift)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_gamelift/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-gamelift)](https://pepy.tech/project/types-aiobotocore-gamelift)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.GameLift 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamelift.html#GameLift)
+[aiobotocore.GameLift 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamelift.html#GameLift)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-gamelift-2.5.2.post3/types_aiobotocore_gamelift.egg-info/SOURCES.txt` & `types-aiobotocore-gamelift-2.5.4/types_aiobotocore_gamelift.egg-info/SOURCES.txt`

 * *Files identical despite different names*


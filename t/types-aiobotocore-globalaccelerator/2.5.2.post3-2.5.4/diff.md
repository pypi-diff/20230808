# Comparing `tmp/types-aiobotocore-globalaccelerator-2.5.2.post3.tar.gz` & `tmp/types-aiobotocore-globalaccelerator-2.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-globalaccelerator-2.5.2.post3.tar", last modified: Fri Aug  4 12:37:46 2023, max compression
+gzip compressed data, was "types-aiobotocore-globalaccelerator-2.5.4.tar", last modified: Tue Aug  8 01:23:46 2023, max compression
```

## Comparing `types-aiobotocore-globalaccelerator-2.5.2.post3.tar` & `types-aiobotocore-globalaccelerator-2.5.4.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:37:46.703881 types-aiobotocore-globalaccelerator-2.5.2.post3/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-04 12:24:19.000000 types-aiobotocore-globalaccelerator-2.5.2.post3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    14818 2023-08-04 12:37:46.703881 types-aiobotocore-globalaccelerator-2.5.2.post3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    13260 2023-08-04 12:24:19.000000 types-aiobotocore-globalaccelerator-2.5.2.post3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-04 12:37:46.703881 types-aiobotocore-globalaccelerator-2.5.2.post3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2142 2023-08-04 12:24:19.000000 types-aiobotocore-globalaccelerator-2.5.2.post3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:37:46.703881 types-aiobotocore-globalaccelerator-2.5.2.post3/types_aiobotocore_globalaccelerator/
--rw-r--r--   0 runner    (1001) docker     (123)     2559 2023-08-04 12:24:19.000000 types-aiobotocore-globalaccelerator-2.5.2.post3/types_aiobotocore_globalaccelerator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2558 2023-08-04 12:24:19.000000 types-aiobotocore-globalaccelerator-2.5.2.post3/types_aiobotocore_globalaccelerator/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      983 2023-08-04 12:24:19.000000 types-aiobotocore-globalaccelerator-2.5.2.post3/types_aiobotocore_globalaccelerator/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    43795 2023-08-04 12:24:20.000000 types-aiobotocore-globalaccelerator-2.5.2.post3/types_aiobotocore_globalaccelerator/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    43729 2023-08-04 12:24:20.000000 types-aiobotocore-globalaccelerator-2.5.2.post3/types_aiobotocore_globalaccelerator/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    10066 2023-08-04 12:24:20.000000 types-aiobotocore-globalaccelerator-2.5.2.post3/types_aiobotocore_globalaccelerator/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    10064 2023-08-04 12:24:20.000000 types-aiobotocore-globalaccelerator-2.5.2.post3/types_aiobotocore_globalaccelerator/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    11098 2023-08-04 12:24:20.000000 types-aiobotocore-globalaccelerator-2.5.2.post3/types_aiobotocore_globalaccelerator/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)    11088 2023-08-04 12:24:20.000000 types-aiobotocore-globalaccelerator-2.5.2.post3/types_aiobotocore_globalaccelerator/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 12:24:19.000000 types-aiobotocore-globalaccelerator-2.5.2.post3/types_aiobotocore_globalaccelerator/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    44656 2023-08-04 12:24:21.000000 types-aiobotocore-globalaccelerator-2.5.2.post3/types_aiobotocore_globalaccelerator/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    44607 2023-08-04 12:24:20.000000 types-aiobotocore-globalaccelerator-2.5.2.post3/types_aiobotocore_globalaccelerator/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-04 12:24:19.000000 types-aiobotocore-globalaccelerator-2.5.2.post3/types_aiobotocore_globalaccelerator/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:37:46.703881 types-aiobotocore-globalaccelerator-2.5.2.post3/types_aiobotocore_globalaccelerator.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    14818 2023-08-04 12:37:46.000000 types-aiobotocore-globalaccelerator-2.5.2.post3/types_aiobotocore_globalaccelerator.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1003 2023-08-04 12:37:46.000000 types-aiobotocore-globalaccelerator-2.5.2.post3/types_aiobotocore_globalaccelerator.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 12:37:46.000000 types-aiobotocore-globalaccelerator-2.5.2.post3/types_aiobotocore_globalaccelerator.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 12:37:46.000000 types-aiobotocore-globalaccelerator-2.5.2.post3/types_aiobotocore_globalaccelerator.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-04 12:37:46.000000 types-aiobotocore-globalaccelerator-2.5.2.post3/types_aiobotocore_globalaccelerator.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-08-04 12:37:46.000000 types-aiobotocore-globalaccelerator-2.5.2.post3/types_aiobotocore_globalaccelerator.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:23:46.370722 types-aiobotocore-globalaccelerator-2.5.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-08 01:11:41.000000 types-aiobotocore-globalaccelerator-2.5.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    14812 2023-08-08 01:23:46.370722 types-aiobotocore-globalaccelerator-2.5.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    13260 2023-08-08 01:11:41.000000 types-aiobotocore-globalaccelerator-2.5.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-08 01:23:46.370722 types-aiobotocore-globalaccelerator-2.5.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2136 2023-08-08 01:11:41.000000 types-aiobotocore-globalaccelerator-2.5.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:23:46.370722 types-aiobotocore-globalaccelerator-2.5.4/types_aiobotocore_globalaccelerator/
+-rw-r--r--   0 runner    (1001) docker     (123)     2559 2023-08-08 01:11:41.000000 types-aiobotocore-globalaccelerator-2.5.4/types_aiobotocore_globalaccelerator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2558 2023-08-08 01:11:41.000000 types-aiobotocore-globalaccelerator-2.5.4/types_aiobotocore_globalaccelerator/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      971 2023-08-08 01:11:41.000000 types-aiobotocore-globalaccelerator-2.5.4/types_aiobotocore_globalaccelerator/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    43795 2023-08-08 01:11:41.000000 types-aiobotocore-globalaccelerator-2.5.4/types_aiobotocore_globalaccelerator/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    43729 2023-08-08 01:11:41.000000 types-aiobotocore-globalaccelerator-2.5.4/types_aiobotocore_globalaccelerator/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    10161 2023-08-08 01:11:42.000000 types-aiobotocore-globalaccelerator-2.5.4/types_aiobotocore_globalaccelerator/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10159 2023-08-08 01:11:41.000000 types-aiobotocore-globalaccelerator-2.5.4/types_aiobotocore_globalaccelerator/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    11098 2023-08-08 01:11:41.000000 types-aiobotocore-globalaccelerator-2.5.4/types_aiobotocore_globalaccelerator/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11088 2023-08-08 01:11:41.000000 types-aiobotocore-globalaccelerator-2.5.4/types_aiobotocore_globalaccelerator/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 01:11:41.000000 types-aiobotocore-globalaccelerator-2.5.4/types_aiobotocore_globalaccelerator/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    44656 2023-08-08 01:11:42.000000 types-aiobotocore-globalaccelerator-2.5.4/types_aiobotocore_globalaccelerator/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    44607 2023-08-08 01:11:42.000000 types-aiobotocore-globalaccelerator-2.5.4/types_aiobotocore_globalaccelerator/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-08-08 01:11:41.000000 types-aiobotocore-globalaccelerator-2.5.4/types_aiobotocore_globalaccelerator/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:23:46.370722 types-aiobotocore-globalaccelerator-2.5.4/types_aiobotocore_globalaccelerator.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    14812 2023-08-08 01:23:46.000000 types-aiobotocore-globalaccelerator-2.5.4/types_aiobotocore_globalaccelerator.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1003 2023-08-08 01:23:46.000000 types-aiobotocore-globalaccelerator-2.5.4/types_aiobotocore_globalaccelerator.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 01:23:46.000000 types-aiobotocore-globalaccelerator-2.5.4/types_aiobotocore_globalaccelerator.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 01:23:46.000000 types-aiobotocore-globalaccelerator-2.5.4/types_aiobotocore_globalaccelerator.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-08 01:23:46.000000 types-aiobotocore-globalaccelerator-2.5.4/types_aiobotocore_globalaccelerator.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-08-08 01:23:46.000000 types-aiobotocore-globalaccelerator-2.5.4/types_aiobotocore_globalaccelerator.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-globalaccelerator-2.5.2.post3/LICENSE` & `types-aiobotocore-globalaccelerator-2.5.4/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-globalaccelerator-2.5.2.post3/PKG-INFO` & `types-aiobotocore-globalaccelerator-2.5.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-globalaccelerator
-Version: 2.5.2.post3
-Summary: Type annotations for aiobotocore.GlobalAccelerator 2.5.2 service generated with mypy-boto3-builder 7.17.2
+Version: 2.5.4
+Summary: Type annotations for aiobotocore.GlobalAccelerator 2.5.4 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_globalaccelerator/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-globalaccelerator.svg?color=blue)](https://pypi.org/project/types-aiobotocore-globalaccelerator)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_globalaccelerator/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-globalaccelerator)](https://pepy.tech/project/types-aiobotocore-globalaccelerator)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.GlobalAccelerator 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/globalaccelerator.html#GlobalAccelerator)
+[aiobotocore.GlobalAccelerator 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/globalaccelerator.html#GlobalAccelerator)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-globalaccelerator-2.5.2.post3/README.md` & `types-aiobotocore-globalaccelerator-2.5.4/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-globalaccelerator.svg?color=blue)](https://pypi.org/project/types-aiobotocore-globalaccelerator)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_globalaccelerator/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-globalaccelerator)](https://pepy.tech/project/types-aiobotocore-globalaccelerator)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.GlobalAccelerator 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/globalaccelerator.html#GlobalAccelerator)
+[aiobotocore.GlobalAccelerator 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/globalaccelerator.html#GlobalAccelerator)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-globalaccelerator-2.5.2.post3/setup.py` & `types-aiobotocore-globalaccelerator-2.5.4/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-globalaccelerator",
-    version="2.5.2.post3",
+    version="2.5.4",
     packages=["types_aiobotocore_globalaccelerator"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.GlobalAccelerator 2.5.2 service generated with"
+        "Type annotations for aiobotocore.GlobalAccelerator 2.5.4 service generated with"
         " mypy-boto3-builder 7.17.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
```

### Comparing `types-aiobotocore-globalaccelerator-2.5.2.post3/types_aiobotocore_globalaccelerator/__init__.py` & `types-aiobotocore-globalaccelerator-2.5.4/types_aiobotocore_globalaccelerator/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-globalaccelerator-2.5.2.post3/types_aiobotocore_globalaccelerator/__init__.pyi` & `types-aiobotocore-globalaccelerator-2.5.4/types_aiobotocore_globalaccelerator/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-globalaccelerator-2.5.2.post3/types_aiobotocore_globalaccelerator/__main__.py` & `types-aiobotocore-globalaccelerator-2.5.4/types_aiobotocore_globalaccelerator/__main__.py`

 * *Files 19% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.GlobalAccelerator 2.5.2\nVersion:        "
-        " 2.5.2.post3\nBuilder version: 7.17.2\nDocs:           "
+        "Type annotations for aiobotocore.GlobalAccelerator 2.5.4\nVersion:         2.5.4\nBuilder"
+        " version: 7.17.2\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_globalaccelerator//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/globalaccelerator.html#GlobalAccelerator\nOther"
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

### Comparing `types-aiobotocore-globalaccelerator-2.5.2.post3/types_aiobotocore_globalaccelerator/client.py` & `types-aiobotocore-globalaccelerator-2.5.4/types_aiobotocore_globalaccelerator/client.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-globalaccelerator-2.5.2.post3/types_aiobotocore_globalaccelerator/client.pyi` & `types-aiobotocore-globalaccelerator-2.5.4/types_aiobotocore_globalaccelerator/client.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-globalaccelerator-2.5.2.post3/types_aiobotocore_globalaccelerator/literals.py` & `types-aiobotocore-globalaccelerator-2.5.4/types_aiobotocore_globalaccelerator/literals.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -14,15 +14,14 @@
 import sys
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = (
     "AcceleratorStatusType",
     "ByoipCidrStateType",
     "ClientAffinityType",
     "CustomRoutingAcceleratorStatusType",
     "CustomRoutingDestinationTrafficStateType",
     "CustomRoutingProtocolType",
@@ -41,15 +40,14 @@
     "ProtocolType",
     "GlobalAcceleratorServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
 )
 
-
 AcceleratorStatusType = Literal["DEPLOYED", "IN_PROGRESS"]
 ByoipCidrStateType = Literal[
     "ADVERTISING",
     "DEPROVISIONED",
     "FAILED_ADVERTISING",
     "FAILED_DEPROVISION",
     "FAILED_PROVISION",
@@ -91,14 +89,15 @@
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
@@ -194,14 +193,15 @@
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
@@ -280,26 +280,28 @@
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

### Comparing `types-aiobotocore-globalaccelerator-2.5.2.post3/types_aiobotocore_globalaccelerator/literals.pyi` & `types-aiobotocore-globalaccelerator-2.5.4/types_aiobotocore_globalaccelerator/literals.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 import sys
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
+
 __all__ = (
     "AcceleratorStatusType",
     "ByoipCidrStateType",
     "ClientAffinityType",
     "CustomRoutingAcceleratorStatusType",
     "CustomRoutingDestinationTrafficStateType",
     "CustomRoutingProtocolType",
@@ -40,14 +41,15 @@
     "ProtocolType",
     "GlobalAcceleratorServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
 )
 
+
 AcceleratorStatusType = Literal["DEPLOYED", "IN_PROGRESS"]
 ByoipCidrStateType = Literal[
     "ADVERTISING",
     "DEPROVISIONED",
     "FAILED_ADVERTISING",
     "FAILED_DEPROVISION",
     "FAILED_PROVISION",
@@ -89,14 +91,15 @@
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
@@ -192,14 +195,15 @@
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
@@ -278,26 +282,28 @@
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

### Comparing `types-aiobotocore-globalaccelerator-2.5.2.post3/types_aiobotocore_globalaccelerator/paginator.py` & `types-aiobotocore-globalaccelerator-2.5.4/types_aiobotocore_globalaccelerator/paginator.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-globalaccelerator-2.5.2.post3/types_aiobotocore_globalaccelerator/paginator.pyi` & `types-aiobotocore-globalaccelerator-2.5.4/types_aiobotocore_globalaccelerator/paginator.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-globalaccelerator-2.5.2.post3/types_aiobotocore_globalaccelerator/type_defs.py` & `types-aiobotocore-globalaccelerator-2.5.4/types_aiobotocore_globalaccelerator/type_defs.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-globalaccelerator-2.5.2.post3/types_aiobotocore_globalaccelerator/type_defs.pyi` & `types-aiobotocore-globalaccelerator-2.5.4/types_aiobotocore_globalaccelerator/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-globalaccelerator-2.5.2.post3/types_aiobotocore_globalaccelerator.egg-info/PKG-INFO` & `types-aiobotocore-globalaccelerator-2.5.4/types_aiobotocore_globalaccelerator.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-globalaccelerator
-Version: 2.5.2.post3
-Summary: Type annotations for aiobotocore.GlobalAccelerator 2.5.2 service generated with mypy-boto3-builder 7.17.2
+Version: 2.5.4
+Summary: Type annotations for aiobotocore.GlobalAccelerator 2.5.4 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_globalaccelerator/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-globalaccelerator.svg?color=blue)](https://pypi.org/project/types-aiobotocore-globalaccelerator)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_globalaccelerator/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-globalaccelerator)](https://pepy.tech/project/types-aiobotocore-globalaccelerator)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.GlobalAccelerator 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/globalaccelerator.html#GlobalAccelerator)
+[aiobotocore.GlobalAccelerator 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/globalaccelerator.html#GlobalAccelerator)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-globalaccelerator-2.5.2.post3/types_aiobotocore_globalaccelerator.egg-info/SOURCES.txt` & `types-aiobotocore-globalaccelerator-2.5.4/types_aiobotocore_globalaccelerator.egg-info/SOURCES.txt`

 * *Files identical despite different names*


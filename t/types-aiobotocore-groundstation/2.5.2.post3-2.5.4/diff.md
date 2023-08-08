# Comparing `tmp/types-aiobotocore-groundstation-2.5.2.post3.tar.gz` & `tmp/types-aiobotocore-groundstation-2.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-groundstation-2.5.2.post3.tar", last modified: Fri Aug  4 12:37:47 2023, max compression
+gzip compressed data, was "types-aiobotocore-groundstation-2.5.4.tar", last modified: Tue Aug  8 01:23:48 2023, max compression
```

## Comparing `types-aiobotocore-groundstation-2.5.2.post3.tar` & `types-aiobotocore-groundstation-2.5.4.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:37:47.075890 types-aiobotocore-groundstation-2.5.2.post3/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-04 12:24:45.000000 types-aiobotocore-groundstation-2.5.2.post3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    14865 2023-08-04 12:37:47.071890 types-aiobotocore-groundstation-2.5.2.post3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    13323 2023-08-04 12:24:45.000000 types-aiobotocore-groundstation-2.5.2.post3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-04 12:37:47.075890 types-aiobotocore-groundstation-2.5.2.post3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2114 2023-08-04 12:24:45.000000 types-aiobotocore-groundstation-2.5.2.post3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:37:47.071890 types-aiobotocore-groundstation-2.5.2.post3/types_aiobotocore_groundstation/
--rw-r--r--   0 runner    (1001) docker     (123)     2169 2023-08-04 12:24:45.000000 types-aiobotocore-groundstation-2.5.2.post3/types_aiobotocore_groundstation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2168 2023-08-04 12:24:45.000000 types-aiobotocore-groundstation-2.5.2.post3/types_aiobotocore_groundstation/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      967 2023-08-04 12:24:45.000000 types-aiobotocore-groundstation-2.5.2.post3/types_aiobotocore_groundstation/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    28813 2023-08-04 12:24:46.000000 types-aiobotocore-groundstation-2.5.2.post3/types_aiobotocore_groundstation/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    28763 2023-08-04 12:24:45.000000 types-aiobotocore-groundstation-2.5.2.post3/types_aiobotocore_groundstation/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    10902 2023-08-04 12:24:46.000000 types-aiobotocore-groundstation-2.5.2.post3/types_aiobotocore_groundstation/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    10900 2023-08-04 12:24:46.000000 types-aiobotocore-groundstation-2.5.2.post3/types_aiobotocore_groundstation/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9382 2023-08-04 12:24:46.000000 types-aiobotocore-groundstation-2.5.2.post3/types_aiobotocore_groundstation/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     9373 2023-08-04 12:24:46.000000 types-aiobotocore-groundstation-2.5.2.post3/types_aiobotocore_groundstation/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 12:24:45.000000 types-aiobotocore-groundstation-2.5.2.post3/types_aiobotocore_groundstation/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    40155 2023-08-04 12:24:47.000000 types-aiobotocore-groundstation-2.5.2.post3/types_aiobotocore_groundstation/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    40106 2023-08-04 12:24:46.000000 types-aiobotocore-groundstation-2.5.2.post3/types_aiobotocore_groundstation/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-04 12:24:45.000000 types-aiobotocore-groundstation-2.5.2.post3/types_aiobotocore_groundstation/version.py
--rw-r--r--   0 runner    (1001) docker     (123)     1617 2023-08-04 12:24:46.000000 types-aiobotocore-groundstation-2.5.2.post3/types_aiobotocore_groundstation/waiter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1616 2023-08-04 12:24:46.000000 types-aiobotocore-groundstation-2.5.2.post3/types_aiobotocore_groundstation/waiter.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:37:47.071890 types-aiobotocore-groundstation-2.5.2.post3/types_aiobotocore_groundstation.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    14865 2023-08-04 12:37:46.000000 types-aiobotocore-groundstation-2.5.2.post3/types_aiobotocore_groundstation.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1012 2023-08-04 12:37:46.000000 types-aiobotocore-groundstation-2.5.2.post3/types_aiobotocore_groundstation.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 12:37:46.000000 types-aiobotocore-groundstation-2.5.2.post3/types_aiobotocore_groundstation.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 12:37:46.000000 types-aiobotocore-groundstation-2.5.2.post3/types_aiobotocore_groundstation.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-04 12:37:46.000000 types-aiobotocore-groundstation-2.5.2.post3/types_aiobotocore_groundstation.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-08-04 12:37:46.000000 types-aiobotocore-groundstation-2.5.2.post3/types_aiobotocore_groundstation.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:23:48.038727 types-aiobotocore-groundstation-2.5.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-08 01:12:05.000000 types-aiobotocore-groundstation-2.5.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    14859 2023-08-08 01:23:48.038727 types-aiobotocore-groundstation-2.5.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    13323 2023-08-08 01:12:05.000000 types-aiobotocore-groundstation-2.5.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-08 01:23:48.038727 types-aiobotocore-groundstation-2.5.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2108 2023-08-08 01:12:04.000000 types-aiobotocore-groundstation-2.5.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:23:48.030727 types-aiobotocore-groundstation-2.5.4/types_aiobotocore_groundstation/
+-rw-r--r--   0 runner    (1001) docker     (123)     2169 2023-08-08 01:12:05.000000 types-aiobotocore-groundstation-2.5.4/types_aiobotocore_groundstation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2168 2023-08-08 01:12:05.000000 types-aiobotocore-groundstation-2.5.4/types_aiobotocore_groundstation/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      955 2023-08-08 01:12:05.000000 types-aiobotocore-groundstation-2.5.4/types_aiobotocore_groundstation/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28813 2023-08-08 01:12:05.000000 types-aiobotocore-groundstation-2.5.4/types_aiobotocore_groundstation/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28763 2023-08-08 01:12:05.000000 types-aiobotocore-groundstation-2.5.4/types_aiobotocore_groundstation/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    10997 2023-08-08 01:12:05.000000 types-aiobotocore-groundstation-2.5.4/types_aiobotocore_groundstation/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10995 2023-08-08 01:12:05.000000 types-aiobotocore-groundstation-2.5.4/types_aiobotocore_groundstation/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9382 2023-08-08 01:12:05.000000 types-aiobotocore-groundstation-2.5.4/types_aiobotocore_groundstation/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9373 2023-08-08 01:12:05.000000 types-aiobotocore-groundstation-2.5.4/types_aiobotocore_groundstation/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 01:12:05.000000 types-aiobotocore-groundstation-2.5.4/types_aiobotocore_groundstation/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    40155 2023-08-08 01:12:06.000000 types-aiobotocore-groundstation-2.5.4/types_aiobotocore_groundstation/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40106 2023-08-08 01:12:05.000000 types-aiobotocore-groundstation-2.5.4/types_aiobotocore_groundstation/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-08-08 01:12:05.000000 types-aiobotocore-groundstation-2.5.4/types_aiobotocore_groundstation/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1617 2023-08-08 01:12:05.000000 types-aiobotocore-groundstation-2.5.4/types_aiobotocore_groundstation/waiter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1616 2023-08-08 01:12:05.000000 types-aiobotocore-groundstation-2.5.4/types_aiobotocore_groundstation/waiter.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:23:48.038727 types-aiobotocore-groundstation-2.5.4/types_aiobotocore_groundstation.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    14859 2023-08-08 01:23:47.000000 types-aiobotocore-groundstation-2.5.4/types_aiobotocore_groundstation.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1012 2023-08-08 01:23:47.000000 types-aiobotocore-groundstation-2.5.4/types_aiobotocore_groundstation.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 01:23:47.000000 types-aiobotocore-groundstation-2.5.4/types_aiobotocore_groundstation.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 01:23:47.000000 types-aiobotocore-groundstation-2.5.4/types_aiobotocore_groundstation.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-08 01:23:47.000000 types-aiobotocore-groundstation-2.5.4/types_aiobotocore_groundstation.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-08-08 01:23:47.000000 types-aiobotocore-groundstation-2.5.4/types_aiobotocore_groundstation.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-groundstation-2.5.2.post3/LICENSE` & `types-aiobotocore-groundstation-2.5.4/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-groundstation-2.5.2.post3/PKG-INFO` & `types-aiobotocore-groundstation-2.5.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-groundstation
-Version: 2.5.2.post3
-Summary: Type annotations for aiobotocore.GroundStation 2.5.2 service generated with mypy-boto3-builder 7.17.2
+Version: 2.5.4
+Summary: Type annotations for aiobotocore.GroundStation 2.5.4 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_groundstation/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-groundstation.svg?color=blue)](https://pypi.org/project/types-aiobotocore-groundstation)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_groundstation/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-groundstation)](https://pepy.tech/project/types-aiobotocore-groundstation)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.GroundStation 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/groundstation.html#GroundStation)
+[aiobotocore.GroundStation 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/groundstation.html#GroundStation)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-groundstation-2.5.2.post3/README.md` & `types-aiobotocore-groundstation-2.5.4/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-groundstation.svg?color=blue)](https://pypi.org/project/types-aiobotocore-groundstation)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_groundstation/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-groundstation)](https://pepy.tech/project/types-aiobotocore-groundstation)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.GroundStation 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/groundstation.html#GroundStation)
+[aiobotocore.GroundStation 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/groundstation.html#GroundStation)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-groundstation-2.5.2.post3/setup.py` & `types-aiobotocore-groundstation-2.5.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-groundstation",
-    version="2.5.2.post3",
+    version="2.5.4",
     packages=["types_aiobotocore_groundstation"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.GroundStation 2.5.2 service generated with"
+        "Type annotations for aiobotocore.GroundStation 2.5.4 service generated with"
         " mypy-boto3-builder 7.17.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
```

### Comparing `types-aiobotocore-groundstation-2.5.2.post3/types_aiobotocore_groundstation/__init__.py` & `types-aiobotocore-groundstation-2.5.4/types_aiobotocore_groundstation/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-groundstation-2.5.2.post3/types_aiobotocore_groundstation/__init__.pyi` & `types-aiobotocore-groundstation-2.5.4/types_aiobotocore_groundstation/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-groundstation-2.5.2.post3/types_aiobotocore_groundstation/__main__.py` & `types-aiobotocore-groundstation-2.5.4/types_aiobotocore_groundstation/__main__.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.GroundStation 2.5.2\nVersion:        "
-        " 2.5.2.post3\nBuilder version: 7.17.2\nDocs:           "
+        "Type annotations for aiobotocore.GroundStation 2.5.4\nVersion:         2.5.4\nBuilder"
+        " version: 7.17.2\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_groundstation//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/groundstation.html#GroundStation\nOther"
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

### Comparing `types-aiobotocore-groundstation-2.5.2.post3/types_aiobotocore_groundstation/client.py` & `types-aiobotocore-groundstation-2.5.4/types_aiobotocore_groundstation/client.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-groundstation-2.5.2.post3/types_aiobotocore_groundstation/client.pyi` & `types-aiobotocore-groundstation-2.5.4/types_aiobotocore_groundstation/client.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-groundstation-2.5.2.post3/types_aiobotocore_groundstation/literals.py` & `types-aiobotocore-groundstation-2.5.4/types_aiobotocore_groundstation/literals.pyi`

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
     "AgentStatusType",
     "AngleUnitsType",
     "AuditResultsType",
     "BandwidthUnitsType",
     "CapabilityHealthReasonType",
     "CapabilityHealthType",
@@ -48,15 +47,14 @@
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "WaiterName",
     "RegionName",
 )
 
-
 AgentStatusType = Literal["ACTIVE", "FAILED", "INACTIVE", "SUCCESS"]
 AngleUnitsType = Literal["DEGREE_ANGLE", "RADIAN"]
 AuditResultsType = Literal["HEALTHY", "UNHEALTHY"]
 BandwidthUnitsType = Literal["GHz", "MHz", "kHz"]
 CapabilityHealthReasonType = Literal[
     "DATAPLANE_FAILURE",
     "HEALTHY",
@@ -125,14 +123,15 @@
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
@@ -228,14 +227,15 @@
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
@@ -314,26 +314,28 @@
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

### Comparing `types-aiobotocore-groundstation-2.5.2.post3/types_aiobotocore_groundstation/literals.pyi` & `types-aiobotocore-groundstation-2.5.4/types_aiobotocore_groundstation/literals.py`

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
     "AgentStatusType",
     "AngleUnitsType",
     "AuditResultsType",
     "BandwidthUnitsType",
     "CapabilityHealthReasonType",
     "CapabilityHealthType",
@@ -47,14 +48,15 @@
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "WaiterName",
     "RegionName",
 )
 
+
 AgentStatusType = Literal["ACTIVE", "FAILED", "INACTIVE", "SUCCESS"]
 AngleUnitsType = Literal["DEGREE_ANGLE", "RADIAN"]
 AuditResultsType = Literal["HEALTHY", "UNHEALTHY"]
 BandwidthUnitsType = Literal["GHz", "MHz", "kHz"]
 CapabilityHealthReasonType = Literal[
     "DATAPLANE_FAILURE",
     "HEALTHY",
@@ -123,14 +125,15 @@
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
@@ -226,14 +229,15 @@
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
@@ -312,26 +316,28 @@
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

### Comparing `types-aiobotocore-groundstation-2.5.2.post3/types_aiobotocore_groundstation/paginator.py` & `types-aiobotocore-groundstation-2.5.4/types_aiobotocore_groundstation/paginator.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-groundstation-2.5.2.post3/types_aiobotocore_groundstation/paginator.pyi` & `types-aiobotocore-groundstation-2.5.4/types_aiobotocore_groundstation/paginator.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-groundstation-2.5.2.post3/types_aiobotocore_groundstation/type_defs.py` & `types-aiobotocore-groundstation-2.5.4/types_aiobotocore_groundstation/type_defs.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-groundstation-2.5.2.post3/types_aiobotocore_groundstation/type_defs.pyi` & `types-aiobotocore-groundstation-2.5.4/types_aiobotocore_groundstation/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-groundstation-2.5.2.post3/types_aiobotocore_groundstation/waiter.py` & `types-aiobotocore-groundstation-2.5.4/types_aiobotocore_groundstation/waiter.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-groundstation-2.5.2.post3/types_aiobotocore_groundstation/waiter.pyi` & `types-aiobotocore-groundstation-2.5.4/types_aiobotocore_groundstation/waiter.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-groundstation-2.5.2.post3/types_aiobotocore_groundstation.egg-info/PKG-INFO` & `types-aiobotocore-groundstation-2.5.4/types_aiobotocore_groundstation.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-groundstation
-Version: 2.5.2.post3
-Summary: Type annotations for aiobotocore.GroundStation 2.5.2 service generated with mypy-boto3-builder 7.17.2
+Version: 2.5.4
+Summary: Type annotations for aiobotocore.GroundStation 2.5.4 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_groundstation/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-groundstation.svg?color=blue)](https://pypi.org/project/types-aiobotocore-groundstation)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_groundstation/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-groundstation)](https://pepy.tech/project/types-aiobotocore-groundstation)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.GroundStation 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/groundstation.html#GroundStation)
+[aiobotocore.GroundStation 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/groundstation.html#GroundStation)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-groundstation-2.5.2.post3/types_aiobotocore_groundstation.egg-info/SOURCES.txt` & `types-aiobotocore-groundstation-2.5.4/types_aiobotocore_groundstation.egg-info/SOURCES.txt`

 * *Files identical despite different names*


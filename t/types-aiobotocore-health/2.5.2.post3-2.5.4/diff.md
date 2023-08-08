# Comparing `tmp/types-aiobotocore-health-2.5.2.post3.tar.gz` & `tmp/types-aiobotocore-health-2.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-health-2.5.2.post3.tar", last modified: Fri Aug  4 12:37:48 2023, max compression
+gzip compressed data, was "types-aiobotocore-health-2.5.4.tar", last modified: Tue Aug  8 01:23:48 2023, max compression
```

## Comparing `types-aiobotocore-health-2.5.2.post3.tar` & `types-aiobotocore-health-2.5.4.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:37:48.587925 types-aiobotocore-health-2.5.2.post3/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-04 12:24:52.000000 types-aiobotocore-health-2.5.2.post3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    14133 2023-08-04 12:37:48.575925 types-aiobotocore-health-2.5.2.post3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    12619 2023-08-04 12:24:52.000000 types-aiobotocore-health-2.5.2.post3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-04 12:37:48.587925 types-aiobotocore-health-2.5.2.post3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2065 2023-08-04 12:24:52.000000 types-aiobotocore-health-2.5.2.post3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:37:48.567925 types-aiobotocore-health-2.5.2.post3/types_aiobotocore_health/
--rw-r--r--   0 runner    (1001) docker     (123)     2353 2023-08-04 12:24:52.000000 types-aiobotocore-health-2.5.2.post3/types_aiobotocore_health/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2352 2023-08-04 12:24:52.000000 types-aiobotocore-health-2.5.2.post3/types_aiobotocore_health/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      928 2023-08-04 12:24:52.000000 types-aiobotocore-health-2.5.2.post3/types_aiobotocore_health/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17083 2023-08-04 12:24:52.000000 types-aiobotocore-health-2.5.2.post3/types_aiobotocore_health/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    17054 2023-08-04 12:24:52.000000 types-aiobotocore-health-2.5.2.post3/types_aiobotocore_health/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9400 2023-08-04 12:24:53.000000 types-aiobotocore-health-2.5.2.post3/types_aiobotocore_health/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     9398 2023-08-04 12:24:53.000000 types-aiobotocore-health-2.5.2.post3/types_aiobotocore_health/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    10245 2023-08-04 12:24:53.000000 types-aiobotocore-health-2.5.2.post3/types_aiobotocore_health/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)    10235 2023-08-04 12:24:53.000000 types-aiobotocore-health-2.5.2.post3/types_aiobotocore_health/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 12:24:52.000000 types-aiobotocore-health-2.5.2.post3/types_aiobotocore_health/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    21689 2023-08-04 12:24:53.000000 types-aiobotocore-health-2.5.2.post3/types_aiobotocore_health/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    21664 2023-08-04 12:24:53.000000 types-aiobotocore-health-2.5.2.post3/types_aiobotocore_health/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-04 12:24:52.000000 types-aiobotocore-health-2.5.2.post3/types_aiobotocore_health/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:37:48.575925 types-aiobotocore-health-2.5.2.post3/types_aiobotocore_health.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    14133 2023-08-04 12:37:48.000000 types-aiobotocore-health-2.5.2.post3/types_aiobotocore_health.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      794 2023-08-04 12:37:48.000000 types-aiobotocore-health-2.5.2.post3/types_aiobotocore_health.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 12:37:48.000000 types-aiobotocore-health-2.5.2.post3/types_aiobotocore_health.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 12:37:48.000000 types-aiobotocore-health-2.5.2.post3/types_aiobotocore_health.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-04 12:37:48.000000 types-aiobotocore-health-2.5.2.post3/types_aiobotocore_health.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-08-04 12:37:48.000000 types-aiobotocore-health-2.5.2.post3/types_aiobotocore_health.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:23:48.186728 types-aiobotocore-health-2.5.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-08 01:12:11.000000 types-aiobotocore-health-2.5.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    14127 2023-08-08 01:23:48.186728 types-aiobotocore-health-2.5.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    12619 2023-08-08 01:12:11.000000 types-aiobotocore-health-2.5.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-08 01:23:48.186728 types-aiobotocore-health-2.5.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2059 2023-08-08 01:12:11.000000 types-aiobotocore-health-2.5.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:23:48.182728 types-aiobotocore-health-2.5.4/types_aiobotocore_health/
+-rw-r--r--   0 runner    (1001) docker     (123)     2353 2023-08-08 01:12:11.000000 types-aiobotocore-health-2.5.4/types_aiobotocore_health/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2352 2023-08-08 01:12:11.000000 types-aiobotocore-health-2.5.4/types_aiobotocore_health/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      916 2023-08-08 01:12:11.000000 types-aiobotocore-health-2.5.4/types_aiobotocore_health/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17083 2023-08-08 01:12:11.000000 types-aiobotocore-health-2.5.4/types_aiobotocore_health/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17054 2023-08-08 01:12:11.000000 types-aiobotocore-health-2.5.4/types_aiobotocore_health/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9495 2023-08-08 01:12:11.000000 types-aiobotocore-health-2.5.4/types_aiobotocore_health/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9493 2023-08-08 01:12:11.000000 types-aiobotocore-health-2.5.4/types_aiobotocore_health/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    10245 2023-08-08 01:12:11.000000 types-aiobotocore-health-2.5.4/types_aiobotocore_health/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10235 2023-08-08 01:12:11.000000 types-aiobotocore-health-2.5.4/types_aiobotocore_health/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 01:12:11.000000 types-aiobotocore-health-2.5.4/types_aiobotocore_health/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    21689 2023-08-08 01:12:12.000000 types-aiobotocore-health-2.5.4/types_aiobotocore_health/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21664 2023-08-08 01:12:11.000000 types-aiobotocore-health-2.5.4/types_aiobotocore_health/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-08-08 01:12:11.000000 types-aiobotocore-health-2.5.4/types_aiobotocore_health/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:23:48.182728 types-aiobotocore-health-2.5.4/types_aiobotocore_health.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    14127 2023-08-08 01:23:48.000000 types-aiobotocore-health-2.5.4/types_aiobotocore_health.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      794 2023-08-08 01:23:48.000000 types-aiobotocore-health-2.5.4/types_aiobotocore_health.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 01:23:48.000000 types-aiobotocore-health-2.5.4/types_aiobotocore_health.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 01:23:47.000000 types-aiobotocore-health-2.5.4/types_aiobotocore_health.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-08 01:23:48.000000 types-aiobotocore-health-2.5.4/types_aiobotocore_health.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-08-08 01:23:48.000000 types-aiobotocore-health-2.5.4/types_aiobotocore_health.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-health-2.5.2.post3/LICENSE` & `types-aiobotocore-health-2.5.4/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-health-2.5.2.post3/PKG-INFO` & `types-aiobotocore-health-2.5.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-health
-Version: 2.5.2.post3
-Summary: Type annotations for aiobotocore.Health 2.5.2 service generated with mypy-boto3-builder 7.17.2
+Version: 2.5.4
+Summary: Type annotations for aiobotocore.Health 2.5.4 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_health/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-health.svg?color=blue)](https://pypi.org/project/types-aiobotocore-health)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_health/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-health)](https://pepy.tech/project/types-aiobotocore-health)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.Health 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/health.html#Health)
+[aiobotocore.Health 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/health.html#Health)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-health-2.5.2.post3/README.md` & `types-aiobotocore-health-2.5.4/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-health.svg?color=blue)](https://pypi.org/project/types-aiobotocore-health)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_health/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-health)](https://pepy.tech/project/types-aiobotocore-health)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.Health 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/health.html#Health)
+[aiobotocore.Health 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/health.html#Health)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-health-2.5.2.post3/setup.py` & `types-aiobotocore-health-2.5.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-health",
-    version="2.5.2.post3",
+    version="2.5.4",
     packages=["types_aiobotocore_health"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.Health 2.5.2 service generated with mypy-boto3-builder"
+        "Type annotations for aiobotocore.Health 2.5.4 service generated with mypy-boto3-builder"
         " 7.17.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
```

### Comparing `types-aiobotocore-health-2.5.2.post3/types_aiobotocore_health/__init__.py` & `types-aiobotocore-health-2.5.4/types_aiobotocore_health/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-health-2.5.2.post3/types_aiobotocore_health/__init__.pyi` & `types-aiobotocore-health-2.5.4/types_aiobotocore_health/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-health-2.5.2.post3/types_aiobotocore_health/__main__.py` & `types-aiobotocore-health-2.5.4/types_aiobotocore_health/__main__.py`

 * *Files 17% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.Health 2.5.2\nVersion:         2.5.2.post3\nBuilder"
-        " version: 7.17.2\nDocs:           "
+        "Type annotations for aiobotocore.Health 2.5.4\nVersion:         2.5.4\nBuilder version:"
+        " 7.17.2\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_health//\nBoto3 docs: "
         "     https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/health.html#Health\nOther"
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

### Comparing `types-aiobotocore-health-2.5.2.post3/types_aiobotocore_health/client.py` & `types-aiobotocore-health-2.5.4/types_aiobotocore_health/client.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-health-2.5.2.post3/types_aiobotocore_health/client.pyi` & `types-aiobotocore-health-2.5.4/types_aiobotocore_health/client.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-health-2.5.2.post3/types_aiobotocore_health/literals.py` & `types-aiobotocore-health-2.5.4/types_aiobotocore_health/literals.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,14 @@
 import sys
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = (
     "DescribeAffectedAccountsForOrganizationPaginatorName",
     "DescribeAffectedEntitiesForOrganizationPaginatorName",
     "DescribeAffectedEntitiesPaginatorName",
     "DescribeEventAggregatesPaginatorName",
     "DescribeEventTypesPaginatorName",
     "DescribeEventsForOrganizationPaginatorName",
@@ -35,15 +34,14 @@
     "HealthServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "RegionName",
 )
 
-
 DescribeAffectedAccountsForOrganizationPaginatorName = Literal[
     "describe_affected_accounts_for_organization"
 ]
 DescribeAffectedEntitiesForOrganizationPaginatorName = Literal[
     "describe_affected_entities_for_organization"
 ]
 DescribeAffectedEntitiesPaginatorName = Literal["describe_affected_entities"]
@@ -68,14 +66,15 @@
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
@@ -171,14 +170,15 @@
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
@@ -257,26 +257,28 @@
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

### Comparing `types-aiobotocore-health-2.5.2.post3/types_aiobotocore_health/literals.pyi` & `types-aiobotocore-health-2.5.4/types_aiobotocore_health/literals.py`

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
     "DescribeAffectedAccountsForOrganizationPaginatorName",
     "DescribeAffectedEntitiesForOrganizationPaginatorName",
     "DescribeAffectedEntitiesPaginatorName",
     "DescribeEventAggregatesPaginatorName",
     "DescribeEventTypesPaginatorName",
     "DescribeEventsForOrganizationPaginatorName",
@@ -34,14 +35,15 @@
     "HealthServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "RegionName",
 )
 
+
 DescribeAffectedAccountsForOrganizationPaginatorName = Literal[
     "describe_affected_accounts_for_organization"
 ]
 DescribeAffectedEntitiesForOrganizationPaginatorName = Literal[
     "describe_affected_entities_for_organization"
 ]
 DescribeAffectedEntitiesPaginatorName = Literal["describe_affected_entities"]
@@ -66,14 +68,15 @@
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
@@ -169,14 +172,15 @@
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
@@ -255,26 +259,28 @@
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

### Comparing `types-aiobotocore-health-2.5.2.post3/types_aiobotocore_health/paginator.py` & `types-aiobotocore-health-2.5.4/types_aiobotocore_health/paginator.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-health-2.5.2.post3/types_aiobotocore_health/paginator.pyi` & `types-aiobotocore-health-2.5.4/types_aiobotocore_health/paginator.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-health-2.5.2.post3/types_aiobotocore_health/type_defs.py` & `types-aiobotocore-health-2.5.4/types_aiobotocore_health/type_defs.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-health-2.5.2.post3/types_aiobotocore_health/type_defs.pyi` & `types-aiobotocore-health-2.5.4/types_aiobotocore_health/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-health-2.5.2.post3/types_aiobotocore_health.egg-info/PKG-INFO` & `types-aiobotocore-health-2.5.4/types_aiobotocore_health.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-health
-Version: 2.5.2.post3
-Summary: Type annotations for aiobotocore.Health 2.5.2 service generated with mypy-boto3-builder 7.17.2
+Version: 2.5.4
+Summary: Type annotations for aiobotocore.Health 2.5.4 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_health/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-health.svg?color=blue)](https://pypi.org/project/types-aiobotocore-health)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_health/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-health)](https://pepy.tech/project/types-aiobotocore-health)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.Health 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/health.html#Health)
+[aiobotocore.Health 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/health.html#Health)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-health-2.5.2.post3/types_aiobotocore_health.egg-info/SOURCES.txt` & `types-aiobotocore-health-2.5.4/types_aiobotocore_health.egg-info/SOURCES.txt`

 * *Files identical despite different names*


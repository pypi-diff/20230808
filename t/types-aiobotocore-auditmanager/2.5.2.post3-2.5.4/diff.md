# Comparing `tmp/types-aiobotocore-auditmanager-2.5.2.post3.tar.gz` & `tmp/types-aiobotocore-auditmanager-2.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-auditmanager-2.5.2.post3.tar", last modified: Fri Aug  4 12:37:19 2023, max compression
+gzip compressed data, was "types-aiobotocore-auditmanager-2.5.4.tar", last modified: Tue Aug  8 01:23:20 2023, max compression
```

## Comparing `types-aiobotocore-auditmanager-2.5.2.post3.tar` & `types-aiobotocore-auditmanager-2.5.4.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:37:19.015228 types-aiobotocore-auditmanager-2.5.2.post3/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-04 12:18:44.000000 types-aiobotocore-auditmanager-2.5.2.post3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    12443 2023-08-04 12:37:19.015228 types-aiobotocore-auditmanager-2.5.2.post3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    10905 2023-08-04 12:18:44.000000 types-aiobotocore-auditmanager-2.5.2.post3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-04 12:37:19.015228 types-aiobotocore-auditmanager-2.5.2.post3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2107 2023-08-04 12:18:44.000000 types-aiobotocore-auditmanager-2.5.2.post3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:37:19.015228 types-aiobotocore-auditmanager-2.5.2.post3/types_aiobotocore_auditmanager/
--rw-r--r--   0 runner    (1001) docker     (123)      482 2023-08-04 12:18:44.000000 types-aiobotocore-auditmanager-2.5.2.post3/types_aiobotocore_auditmanager/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      481 2023-08-04 12:18:44.000000 types-aiobotocore-auditmanager-2.5.2.post3/types_aiobotocore_auditmanager/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      963 2023-08-04 12:18:44.000000 types-aiobotocore-auditmanager-2.5.2.post3/types_aiobotocore_auditmanager/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    45840 2023-08-04 12:18:44.000000 types-aiobotocore-auditmanager-2.5.2.post3/types_aiobotocore_auditmanager/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    45770 2023-08-04 12:18:44.000000 types-aiobotocore-auditmanager-2.5.2.post3/types_aiobotocore_auditmanager/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    10640 2023-08-04 12:18:44.000000 types-aiobotocore-auditmanager-2.5.2.post3/types_aiobotocore_auditmanager/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    10638 2023-08-04 12:18:44.000000 types-aiobotocore-auditmanager-2.5.2.post3/types_aiobotocore_auditmanager/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 12:18:44.000000 types-aiobotocore-auditmanager-2.5.2.post3/types_aiobotocore_auditmanager/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    57739 2023-08-04 12:18:46.000000 types-aiobotocore-auditmanager-2.5.2.post3/types_aiobotocore_auditmanager/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    57694 2023-08-04 12:18:45.000000 types-aiobotocore-auditmanager-2.5.2.post3/types_aiobotocore_auditmanager/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-04 12:18:44.000000 types-aiobotocore-auditmanager-2.5.2.post3/types_aiobotocore_auditmanager/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:37:19.015228 types-aiobotocore-auditmanager-2.5.2.post3/types_aiobotocore_auditmanager.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    12443 2023-08-04 12:37:18.000000 types-aiobotocore-auditmanager-2.5.2.post3/types_aiobotocore_auditmanager.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      819 2023-08-04 12:37:18.000000 types-aiobotocore-auditmanager-2.5.2.post3/types_aiobotocore_auditmanager.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 12:37:18.000000 types-aiobotocore-auditmanager-2.5.2.post3/types_aiobotocore_auditmanager.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 12:37:18.000000 types-aiobotocore-auditmanager-2.5.2.post3/types_aiobotocore_auditmanager.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-04 12:37:18.000000 types-aiobotocore-auditmanager-2.5.2.post3/types_aiobotocore_auditmanager.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-08-04 12:37:18.000000 types-aiobotocore-auditmanager-2.5.2.post3/types_aiobotocore_auditmanager.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:23:20.634588 types-aiobotocore-auditmanager-2.5.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-08 01:06:31.000000 types-aiobotocore-auditmanager-2.5.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    12437 2023-08-08 01:23:20.630588 types-aiobotocore-auditmanager-2.5.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10905 2023-08-08 01:06:31.000000 types-aiobotocore-auditmanager-2.5.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-08 01:23:20.634588 types-aiobotocore-auditmanager-2.5.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2101 2023-08-08 01:06:31.000000 types-aiobotocore-auditmanager-2.5.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:23:20.630588 types-aiobotocore-auditmanager-2.5.4/types_aiobotocore_auditmanager/
+-rw-r--r--   0 runner    (1001) docker     (123)      482 2023-08-08 01:06:31.000000 types-aiobotocore-auditmanager-2.5.4/types_aiobotocore_auditmanager/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      481 2023-08-08 01:06:31.000000 types-aiobotocore-auditmanager-2.5.4/types_aiobotocore_auditmanager/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      951 2023-08-08 01:06:31.000000 types-aiobotocore-auditmanager-2.5.4/types_aiobotocore_auditmanager/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    45840 2023-08-08 01:06:31.000000 types-aiobotocore-auditmanager-2.5.4/types_aiobotocore_auditmanager/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    45770 2023-08-08 01:06:31.000000 types-aiobotocore-auditmanager-2.5.4/types_aiobotocore_auditmanager/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    10735 2023-08-08 01:06:31.000000 types-aiobotocore-auditmanager-2.5.4/types_aiobotocore_auditmanager/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10733 2023-08-08 01:06:31.000000 types-aiobotocore-auditmanager-2.5.4/types_aiobotocore_auditmanager/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 01:06:31.000000 types-aiobotocore-auditmanager-2.5.4/types_aiobotocore_auditmanager/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    57739 2023-08-08 01:06:32.000000 types-aiobotocore-auditmanager-2.5.4/types_aiobotocore_auditmanager/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    57694 2023-08-08 01:06:32.000000 types-aiobotocore-auditmanager-2.5.4/types_aiobotocore_auditmanager/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-08-08 01:06:31.000000 types-aiobotocore-auditmanager-2.5.4/types_aiobotocore_auditmanager/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:23:20.630588 types-aiobotocore-auditmanager-2.5.4/types_aiobotocore_auditmanager.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    12437 2023-08-08 01:23:20.000000 types-aiobotocore-auditmanager-2.5.4/types_aiobotocore_auditmanager.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      819 2023-08-08 01:23:20.000000 types-aiobotocore-auditmanager-2.5.4/types_aiobotocore_auditmanager.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 01:23:20.000000 types-aiobotocore-auditmanager-2.5.4/types_aiobotocore_auditmanager.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 01:23:20.000000 types-aiobotocore-auditmanager-2.5.4/types_aiobotocore_auditmanager.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-08 01:23:20.000000 types-aiobotocore-auditmanager-2.5.4/types_aiobotocore_auditmanager.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-08-08 01:23:20.000000 types-aiobotocore-auditmanager-2.5.4/types_aiobotocore_auditmanager.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-auditmanager-2.5.2.post3/LICENSE` & `types-aiobotocore-auditmanager-2.5.4/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-auditmanager-2.5.2.post3/PKG-INFO` & `types-aiobotocore-auditmanager-2.5.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-auditmanager
-Version: 2.5.2.post3
-Summary: Type annotations for aiobotocore.AuditManager 2.5.2 service generated with mypy-boto3-builder 7.17.2
+Version: 2.5.4
+Summary: Type annotations for aiobotocore.AuditManager 2.5.4 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_auditmanager/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-auditmanager.svg?color=blue)](https://pypi.org/project/types-aiobotocore-auditmanager)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_auditmanager/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-auditmanager)](https://pepy.tech/project/types-aiobotocore-auditmanager)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.AuditManager 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/auditmanager.html#AuditManager)
+[aiobotocore.AuditManager 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/auditmanager.html#AuditManager)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-auditmanager-2.5.2.post3/README.md` & `types-aiobotocore-auditmanager-2.5.4/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-auditmanager.svg?color=blue)](https://pypi.org/project/types-aiobotocore-auditmanager)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_auditmanager/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-auditmanager)](https://pepy.tech/project/types-aiobotocore-auditmanager)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.AuditManager 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/auditmanager.html#AuditManager)
+[aiobotocore.AuditManager 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/auditmanager.html#AuditManager)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-auditmanager-2.5.2.post3/setup.py` & `types-aiobotocore-auditmanager-2.5.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-auditmanager",
-    version="2.5.2.post3",
+    version="2.5.4",
     packages=["types_aiobotocore_auditmanager"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.AuditManager 2.5.2 service generated with"
+        "Type annotations for aiobotocore.AuditManager 2.5.4 service generated with"
         " mypy-boto3-builder 7.17.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
```

### Comparing `types-aiobotocore-auditmanager-2.5.2.post3/types_aiobotocore_auditmanager/__main__.py` & `types-aiobotocore-auditmanager-2.5.4/types_aiobotocore_auditmanager/__main__.py`

 * *Files 20% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.AuditManager 2.5.2\nVersion:         2.5.2.post3\nBuilder"
+        "Type annotations for aiobotocore.AuditManager 2.5.4\nVersion:         2.5.4\nBuilder"
         " version: 7.17.2\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_auditmanager//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/auditmanager.html#AuditManager\nOther"
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

### Comparing `types-aiobotocore-auditmanager-2.5.2.post3/types_aiobotocore_auditmanager/client.py` & `types-aiobotocore-auditmanager-2.5.4/types_aiobotocore_auditmanager/client.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-auditmanager-2.5.2.post3/types_aiobotocore_auditmanager/client.pyi` & `types-aiobotocore-auditmanager-2.5.4/types_aiobotocore_auditmanager/client.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-auditmanager-2.5.2.post3/types_aiobotocore_auditmanager/literals.py` & `types-aiobotocore-auditmanager-2.5.4/types_aiobotocore_auditmanager/literals.py`

 * *Files 1% similar despite different names*

```diff
@@ -115,14 +115,15 @@
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
@@ -218,14 +219,15 @@
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
@@ -304,26 +306,28 @@
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

### Comparing `types-aiobotocore-auditmanager-2.5.2.post3/types_aiobotocore_auditmanager/literals.pyi` & `types-aiobotocore-auditmanager-2.5.4/types_aiobotocore_auditmanager/literals.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -113,14 +113,15 @@
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
@@ -216,14 +217,15 @@
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
@@ -302,26 +304,28 @@
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

### Comparing `types-aiobotocore-auditmanager-2.5.2.post3/types_aiobotocore_auditmanager/type_defs.py` & `types-aiobotocore-auditmanager-2.5.4/types_aiobotocore_auditmanager/type_defs.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-auditmanager-2.5.2.post3/types_aiobotocore_auditmanager/type_defs.pyi` & `types-aiobotocore-auditmanager-2.5.4/types_aiobotocore_auditmanager/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-auditmanager-2.5.2.post3/types_aiobotocore_auditmanager.egg-info/PKG-INFO` & `types-aiobotocore-auditmanager-2.5.4/types_aiobotocore_auditmanager.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-auditmanager
-Version: 2.5.2.post3
-Summary: Type annotations for aiobotocore.AuditManager 2.5.2 service generated with mypy-boto3-builder 7.17.2
+Version: 2.5.4
+Summary: Type annotations for aiobotocore.AuditManager 2.5.4 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_auditmanager/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-auditmanager.svg?color=blue)](https://pypi.org/project/types-aiobotocore-auditmanager)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_auditmanager/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-auditmanager)](https://pepy.tech/project/types-aiobotocore-auditmanager)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.AuditManager 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/auditmanager.html#AuditManager)
+[aiobotocore.AuditManager 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/auditmanager.html#AuditManager)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-auditmanager-2.5.2.post3/types_aiobotocore_auditmanager.egg-info/SOURCES.txt` & `types-aiobotocore-auditmanager-2.5.4/types_aiobotocore_auditmanager.egg-info/SOURCES.txt`

 * *Files identical despite different names*


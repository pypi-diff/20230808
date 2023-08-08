# Comparing `tmp/types-aiobotocore-backup-2.5.2.post3.tar.gz` & `tmp/types-aiobotocore-backup-2.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-backup-2.5.2.post3.tar", last modified: Fri Aug  4 12:37:21 2023, max compression
+gzip compressed data, was "types-aiobotocore-backup-2.5.4.tar", last modified: Tue Aug  8 01:23:21 2023, max compression
```

## Comparing `types-aiobotocore-backup-2.5.2.post3.tar` & `types-aiobotocore-backup-2.5.4.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:37:21.475279 types-aiobotocore-backup-2.5.2.post3/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-04 12:18:52.000000 types-aiobotocore-backup-2.5.2.post3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    14883 2023-08-04 12:37:21.475279 types-aiobotocore-backup-2.5.2.post3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    13369 2023-08-04 12:18:52.000000 types-aiobotocore-backup-2.5.2.post3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-04 12:37:21.475279 types-aiobotocore-backup-2.5.2.post3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2065 2023-08-04 12:18:51.000000 types-aiobotocore-backup-2.5.2.post3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:37:21.471279 types-aiobotocore-backup-2.5.2.post3/types_aiobotocore_backup/
--rw-r--r--   0 runner    (1001) docker     (123)     3463 2023-08-04 12:18:52.000000 types-aiobotocore-backup-2.5.2.post3/types_aiobotocore_backup/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3462 2023-08-04 12:18:52.000000 types-aiobotocore-backup-2.5.2.post3/types_aiobotocore_backup/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      928 2023-08-04 12:18:52.000000 types-aiobotocore-backup-2.5.2.post3/types_aiobotocore_backup/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    57816 2023-08-04 12:18:52.000000 types-aiobotocore-backup-2.5.2.post3/types_aiobotocore_backup/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    57722 2023-08-04 12:18:52.000000 types-aiobotocore-backup-2.5.2.post3/types_aiobotocore_backup/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    11285 2023-08-04 12:18:53.000000 types-aiobotocore-backup-2.5.2.post3/types_aiobotocore_backup/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    11283 2023-08-04 12:18:53.000000 types-aiobotocore-backup-2.5.2.post3/types_aiobotocore_backup/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    17196 2023-08-04 12:18:53.000000 types-aiobotocore-backup-2.5.2.post3/types_aiobotocore_backup/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)    17181 2023-08-04 12:18:52.000000 types-aiobotocore-backup-2.5.2.post3/types_aiobotocore_backup/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 12:18:52.000000 types-aiobotocore-backup-2.5.2.post3/types_aiobotocore_backup/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    67674 2023-08-04 12:18:54.000000 types-aiobotocore-backup-2.5.2.post3/types_aiobotocore_backup/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    67599 2023-08-04 12:18:54.000000 types-aiobotocore-backup-2.5.2.post3/types_aiobotocore_backup/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-04 12:18:52.000000 types-aiobotocore-backup-2.5.2.post3/types_aiobotocore_backup/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:37:21.471279 types-aiobotocore-backup-2.5.2.post3/types_aiobotocore_backup.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    14883 2023-08-04 12:37:21.000000 types-aiobotocore-backup-2.5.2.post3/types_aiobotocore_backup.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      794 2023-08-04 12:37:21.000000 types-aiobotocore-backup-2.5.2.post3/types_aiobotocore_backup.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 12:37:21.000000 types-aiobotocore-backup-2.5.2.post3/types_aiobotocore_backup.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 12:37:21.000000 types-aiobotocore-backup-2.5.2.post3/types_aiobotocore_backup.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-04 12:37:21.000000 types-aiobotocore-backup-2.5.2.post3/types_aiobotocore_backup.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-08-04 12:37:21.000000 types-aiobotocore-backup-2.5.2.post3/types_aiobotocore_backup.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:23:21.690620 types-aiobotocore-backup-2.5.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-08 01:06:38.000000 types-aiobotocore-backup-2.5.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    14877 2023-08-08 01:23:21.690620 types-aiobotocore-backup-2.5.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    13369 2023-08-08 01:06:38.000000 types-aiobotocore-backup-2.5.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-08 01:23:21.690620 types-aiobotocore-backup-2.5.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2059 2023-08-08 01:06:38.000000 types-aiobotocore-backup-2.5.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:23:21.690620 types-aiobotocore-backup-2.5.4/types_aiobotocore_backup/
+-rw-r--r--   0 runner    (1001) docker     (123)     3463 2023-08-08 01:06:38.000000 types-aiobotocore-backup-2.5.4/types_aiobotocore_backup/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3462 2023-08-08 01:06:38.000000 types-aiobotocore-backup-2.5.4/types_aiobotocore_backup/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      916 2023-08-08 01:06:38.000000 types-aiobotocore-backup-2.5.4/types_aiobotocore_backup/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    57816 2023-08-08 01:06:38.000000 types-aiobotocore-backup-2.5.4/types_aiobotocore_backup/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    57722 2023-08-08 01:06:38.000000 types-aiobotocore-backup-2.5.4/types_aiobotocore_backup/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    11380 2023-08-08 01:06:38.000000 types-aiobotocore-backup-2.5.4/types_aiobotocore_backup/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11378 2023-08-08 01:06:38.000000 types-aiobotocore-backup-2.5.4/types_aiobotocore_backup/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    17196 2023-08-08 01:06:38.000000 types-aiobotocore-backup-2.5.4/types_aiobotocore_backup/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17181 2023-08-08 01:06:38.000000 types-aiobotocore-backup-2.5.4/types_aiobotocore_backup/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 01:06:38.000000 types-aiobotocore-backup-2.5.4/types_aiobotocore_backup/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    67674 2023-08-08 01:06:40.000000 types-aiobotocore-backup-2.5.4/types_aiobotocore_backup/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    67599 2023-08-08 01:06:40.000000 types-aiobotocore-backup-2.5.4/types_aiobotocore_backup/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-08-08 01:06:38.000000 types-aiobotocore-backup-2.5.4/types_aiobotocore_backup/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:23:21.690620 types-aiobotocore-backup-2.5.4/types_aiobotocore_backup.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    14877 2023-08-08 01:23:21.000000 types-aiobotocore-backup-2.5.4/types_aiobotocore_backup.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      794 2023-08-08 01:23:21.000000 types-aiobotocore-backup-2.5.4/types_aiobotocore_backup.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 01:23:21.000000 types-aiobotocore-backup-2.5.4/types_aiobotocore_backup.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 01:23:21.000000 types-aiobotocore-backup-2.5.4/types_aiobotocore_backup.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-08 01:23:21.000000 types-aiobotocore-backup-2.5.4/types_aiobotocore_backup.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-08-08 01:23:21.000000 types-aiobotocore-backup-2.5.4/types_aiobotocore_backup.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-backup-2.5.2.post3/LICENSE` & `types-aiobotocore-backup-2.5.4/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-backup-2.5.2.post3/PKG-INFO` & `types-aiobotocore-backup-2.5.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-backup
-Version: 2.5.2.post3
-Summary: Type annotations for aiobotocore.Backup 2.5.2 service generated with mypy-boto3-builder 7.17.2
+Version: 2.5.4
+Summary: Type annotations for aiobotocore.Backup 2.5.4 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_backup/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-backup.svg?color=blue)](https://pypi.org/project/types-aiobotocore-backup)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_backup/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-backup)](https://pepy.tech/project/types-aiobotocore-backup)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.Backup 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup.html#Backup)
+[aiobotocore.Backup 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup.html#Backup)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-backup-2.5.2.post3/README.md` & `types-aiobotocore-backup-2.5.4/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-backup.svg?color=blue)](https://pypi.org/project/types-aiobotocore-backup)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_backup/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-backup)](https://pepy.tech/project/types-aiobotocore-backup)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.Backup 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup.html#Backup)
+[aiobotocore.Backup 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup.html#Backup)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-backup-2.5.2.post3/setup.py` & `types-aiobotocore-backup-2.5.4/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-backup",
-    version="2.5.2.post3",
+    version="2.5.4",
     packages=["types_aiobotocore_backup"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.Backup 2.5.2 service generated with mypy-boto3-builder"
+        "Type annotations for aiobotocore.Backup 2.5.4 service generated with mypy-boto3-builder"
         " 7.17.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
```

### Comparing `types-aiobotocore-backup-2.5.2.post3/types_aiobotocore_backup/__init__.py` & `types-aiobotocore-backup-2.5.4/types_aiobotocore_backup/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-backup-2.5.2.post3/types_aiobotocore_backup/__init__.pyi` & `types-aiobotocore-backup-2.5.4/types_aiobotocore_backup/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-backup-2.5.2.post3/types_aiobotocore_backup/__main__.py` & `types-aiobotocore-backup-2.5.4/types_aiobotocore_backup/__main__.py`

 * *Files 9% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.Backup 2.5.2\nVersion:         2.5.2.post3\nBuilder"
-        " version: 7.17.2\nDocs:           "
+        "Type annotations for aiobotocore.Backup 2.5.4\nVersion:         2.5.4\nBuilder version:"
+        " 7.17.2\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_backup//\nBoto3 docs: "
         "     https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup.html#Backup\nOther"
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

### Comparing `types-aiobotocore-backup-2.5.2.post3/types_aiobotocore_backup/client.py` & `types-aiobotocore-backup-2.5.4/types_aiobotocore_backup/client.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-backup-2.5.2.post3/types_aiobotocore_backup/client.pyi` & `types-aiobotocore-backup-2.5.4/types_aiobotocore_backup/client.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-backup-2.5.2.post3/types_aiobotocore_backup/literals.py` & `types-aiobotocore-backup-2.5.4/types_aiobotocore_backup/literals.py`

 * *Files 2% similar despite different names*

```diff
@@ -110,14 +110,15 @@
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
@@ -213,14 +214,15 @@
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
@@ -299,26 +301,28 @@
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

### Comparing `types-aiobotocore-backup-2.5.2.post3/types_aiobotocore_backup/literals.pyi` & `types-aiobotocore-backup-2.5.4/types_aiobotocore_backup/literals.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -108,14 +108,15 @@
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
@@ -211,14 +212,15 @@
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
@@ -297,26 +299,28 @@
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

### Comparing `types-aiobotocore-backup-2.5.2.post3/types_aiobotocore_backup/paginator.py` & `types-aiobotocore-backup-2.5.4/types_aiobotocore_backup/paginator.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-backup-2.5.2.post3/types_aiobotocore_backup/paginator.pyi` & `types-aiobotocore-backup-2.5.4/types_aiobotocore_backup/paginator.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-backup-2.5.2.post3/types_aiobotocore_backup/type_defs.py` & `types-aiobotocore-backup-2.5.4/types_aiobotocore_backup/type_defs.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-backup-2.5.2.post3/types_aiobotocore_backup/type_defs.pyi` & `types-aiobotocore-backup-2.5.4/types_aiobotocore_backup/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-backup-2.5.2.post3/types_aiobotocore_backup.egg-info/PKG-INFO` & `types-aiobotocore-backup-2.5.4/types_aiobotocore_backup.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-backup
-Version: 2.5.2.post3
-Summary: Type annotations for aiobotocore.Backup 2.5.2 service generated with mypy-boto3-builder 7.17.2
+Version: 2.5.4
+Summary: Type annotations for aiobotocore.Backup 2.5.4 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_backup/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-backup.svg?color=blue)](https://pypi.org/project/types-aiobotocore-backup)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_backup/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-backup)](https://pepy.tech/project/types-aiobotocore-backup)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.Backup 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup.html#Backup)
+[aiobotocore.Backup 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup.html#Backup)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-backup-2.5.2.post3/types_aiobotocore_backup.egg-info/SOURCES.txt` & `types-aiobotocore-backup-2.5.4/types_aiobotocore_backup.egg-info/SOURCES.txt`

 * *Files identical despite different names*


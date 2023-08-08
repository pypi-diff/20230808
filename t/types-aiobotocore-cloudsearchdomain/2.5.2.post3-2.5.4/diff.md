# Comparing `tmp/types-aiobotocore-cloudsearchdomain-2.5.2.post3.tar.gz` & `tmp/types-aiobotocore-cloudsearchdomain-2.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-cloudsearchdomain-2.5.2.post3.tar", last modified: Fri Aug  4 12:37:26 2023, max compression
+gzip compressed data, was "types-aiobotocore-cloudsearchdomain-2.5.4.tar", last modified: Tue Aug  8 01:23:26 2023, max compression
```

## Comparing `types-aiobotocore-cloudsearchdomain-2.5.2.post3.tar` & `types-aiobotocore-cloudsearchdomain-2.5.4.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:37:26.483395 types-aiobotocore-cloudsearchdomain-2.5.2.post3/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-04 12:19:52.000000 types-aiobotocore-cloudsearchdomain-2.5.2.post3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    12692 2023-08-04 12:37:26.483395 types-aiobotocore-cloudsearchdomain-2.5.2.post3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    11134 2023-08-04 12:19:52.000000 types-aiobotocore-cloudsearchdomain-2.5.2.post3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-04 12:37:26.483395 types-aiobotocore-cloudsearchdomain-2.5.2.post3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2142 2023-08-04 12:19:51.000000 types-aiobotocore-cloudsearchdomain-2.5.2.post3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:37:26.483395 types-aiobotocore-cloudsearchdomain-2.5.2.post3/types_aiobotocore_cloudsearchdomain/
--rw-r--r--   0 runner    (1001) docker     (123)      522 2023-08-04 12:19:52.000000 types-aiobotocore-cloudsearchdomain-2.5.2.post3/types_aiobotocore_cloudsearchdomain/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      521 2023-08-04 12:19:52.000000 types-aiobotocore-cloudsearchdomain-2.5.2.post3/types_aiobotocore_cloudsearchdomain/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      983 2023-08-04 12:19:52.000000 types-aiobotocore-cloudsearchdomain-2.5.2.post3/types_aiobotocore_cloudsearchdomain/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6369 2023-08-04 12:19:52.000000 types-aiobotocore-cloudsearchdomain-2.5.2.post3/types_aiobotocore_cloudsearchdomain/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     6358 2023-08-04 12:19:52.000000 types-aiobotocore-cloudsearchdomain-2.5.2.post3/types_aiobotocore_cloudsearchdomain/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     7764 2023-08-04 12:19:52.000000 types-aiobotocore-cloudsearchdomain-2.5.2.post3/types_aiobotocore_cloudsearchdomain/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     7762 2023-08-04 12:19:52.000000 types-aiobotocore-cloudsearchdomain-2.5.2.post3/types_aiobotocore_cloudsearchdomain/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 12:19:52.000000 types-aiobotocore-cloudsearchdomain-2.5.2.post3/types_aiobotocore_cloudsearchdomain/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     5233 2023-08-04 12:19:52.000000 types-aiobotocore-cloudsearchdomain-2.5.2.post3/types_aiobotocore_cloudsearchdomain/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)     5228 2023-08-04 12:19:52.000000 types-aiobotocore-cloudsearchdomain-2.5.2.post3/types_aiobotocore_cloudsearchdomain/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-04 12:19:52.000000 types-aiobotocore-cloudsearchdomain-2.5.2.post3/types_aiobotocore_cloudsearchdomain/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:37:26.483395 types-aiobotocore-cloudsearchdomain-2.5.2.post3/types_aiobotocore_cloudsearchdomain.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    12692 2023-08-04 12:37:26.000000 types-aiobotocore-cloudsearchdomain-2.5.2.post3/types_aiobotocore_cloudsearchdomain.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      904 2023-08-04 12:37:26.000000 types-aiobotocore-cloudsearchdomain-2.5.2.post3/types_aiobotocore_cloudsearchdomain.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 12:37:26.000000 types-aiobotocore-cloudsearchdomain-2.5.2.post3/types_aiobotocore_cloudsearchdomain.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 12:37:26.000000 types-aiobotocore-cloudsearchdomain-2.5.2.post3/types_aiobotocore_cloudsearchdomain.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-04 12:37:26.000000 types-aiobotocore-cloudsearchdomain-2.5.2.post3/types_aiobotocore_cloudsearchdomain.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-08-04 12:37:26.000000 types-aiobotocore-cloudsearchdomain-2.5.2.post3/types_aiobotocore_cloudsearchdomain.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:23:26.718626 types-aiobotocore-cloudsearchdomain-2.5.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-08 01:07:33.000000 types-aiobotocore-cloudsearchdomain-2.5.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    12686 2023-08-08 01:23:26.718626 types-aiobotocore-cloudsearchdomain-2.5.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    11134 2023-08-08 01:07:33.000000 types-aiobotocore-cloudsearchdomain-2.5.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-08 01:23:26.718626 types-aiobotocore-cloudsearchdomain-2.5.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2136 2023-08-08 01:07:33.000000 types-aiobotocore-cloudsearchdomain-2.5.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:23:26.718626 types-aiobotocore-cloudsearchdomain-2.5.4/types_aiobotocore_cloudsearchdomain/
+-rw-r--r--   0 runner    (1001) docker     (123)      522 2023-08-08 01:07:33.000000 types-aiobotocore-cloudsearchdomain-2.5.4/types_aiobotocore_cloudsearchdomain/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      521 2023-08-08 01:07:33.000000 types-aiobotocore-cloudsearchdomain-2.5.4/types_aiobotocore_cloudsearchdomain/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      971 2023-08-08 01:07:33.000000 types-aiobotocore-cloudsearchdomain-2.5.4/types_aiobotocore_cloudsearchdomain/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6369 2023-08-08 01:07:33.000000 types-aiobotocore-cloudsearchdomain-2.5.4/types_aiobotocore_cloudsearchdomain/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6358 2023-08-08 01:07:33.000000 types-aiobotocore-cloudsearchdomain-2.5.4/types_aiobotocore_cloudsearchdomain/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     7859 2023-08-08 01:07:33.000000 types-aiobotocore-cloudsearchdomain-2.5.4/types_aiobotocore_cloudsearchdomain/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7857 2023-08-08 01:07:33.000000 types-aiobotocore-cloudsearchdomain-2.5.4/types_aiobotocore_cloudsearchdomain/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 01:07:33.000000 types-aiobotocore-cloudsearchdomain-2.5.4/types_aiobotocore_cloudsearchdomain/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     5233 2023-08-08 01:07:33.000000 types-aiobotocore-cloudsearchdomain-2.5.4/types_aiobotocore_cloudsearchdomain/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5228 2023-08-08 01:07:33.000000 types-aiobotocore-cloudsearchdomain-2.5.4/types_aiobotocore_cloudsearchdomain/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-08-08 01:07:33.000000 types-aiobotocore-cloudsearchdomain-2.5.4/types_aiobotocore_cloudsearchdomain/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:23:26.718626 types-aiobotocore-cloudsearchdomain-2.5.4/types_aiobotocore_cloudsearchdomain.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    12686 2023-08-08 01:23:26.000000 types-aiobotocore-cloudsearchdomain-2.5.4/types_aiobotocore_cloudsearchdomain.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      904 2023-08-08 01:23:26.000000 types-aiobotocore-cloudsearchdomain-2.5.4/types_aiobotocore_cloudsearchdomain.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 01:23:26.000000 types-aiobotocore-cloudsearchdomain-2.5.4/types_aiobotocore_cloudsearchdomain.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 01:23:26.000000 types-aiobotocore-cloudsearchdomain-2.5.4/types_aiobotocore_cloudsearchdomain.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-08 01:23:26.000000 types-aiobotocore-cloudsearchdomain-2.5.4/types_aiobotocore_cloudsearchdomain.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-08-08 01:23:26.000000 types-aiobotocore-cloudsearchdomain-2.5.4/types_aiobotocore_cloudsearchdomain.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-cloudsearchdomain-2.5.2.post3/LICENSE` & `types-aiobotocore-cloudsearchdomain-2.5.4/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-cloudsearchdomain-2.5.2.post3/PKG-INFO` & `types-aiobotocore-cloudsearchdomain-2.5.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-cloudsearchdomain
-Version: 2.5.2.post3
-Summary: Type annotations for aiobotocore.CloudSearchDomain 2.5.2 service generated with mypy-boto3-builder 7.17.2
+Version: 2.5.4
+Summary: Type annotations for aiobotocore.CloudSearchDomain 2.5.4 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudsearchdomain/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-cloudsearchdomain.svg?color=blue)](https://pypi.org/project/types-aiobotocore-cloudsearchdomain)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudsearchdomain/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-cloudsearchdomain)](https://pepy.tech/project/types-aiobotocore-cloudsearchdomain)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.CloudSearchDomain 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudsearchdomain.html#CloudSearchDomain)
+[aiobotocore.CloudSearchDomain 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudsearchdomain.html#CloudSearchDomain)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-cloudsearchdomain-2.5.2.post3/README.md` & `types-aiobotocore-cloudsearchdomain-2.5.4/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-cloudsearchdomain.svg?color=blue)](https://pypi.org/project/types-aiobotocore-cloudsearchdomain)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudsearchdomain/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-cloudsearchdomain)](https://pepy.tech/project/types-aiobotocore-cloudsearchdomain)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.CloudSearchDomain 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudsearchdomain.html#CloudSearchDomain)
+[aiobotocore.CloudSearchDomain 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudsearchdomain.html#CloudSearchDomain)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-cloudsearchdomain-2.5.2.post3/setup.py` & `types-aiobotocore-cloudsearchdomain-2.5.4/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-cloudsearchdomain",
-    version="2.5.2.post3",
+    version="2.5.4",
     packages=["types_aiobotocore_cloudsearchdomain"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.CloudSearchDomain 2.5.2 service generated with"
+        "Type annotations for aiobotocore.CloudSearchDomain 2.5.4 service generated with"
         " mypy-boto3-builder 7.17.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
```

### Comparing `types-aiobotocore-cloudsearchdomain-2.5.2.post3/types_aiobotocore_cloudsearchdomain/__init__.py` & `types-aiobotocore-cloudsearchdomain-2.5.4/types_aiobotocore_cloudsearchdomain/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-cloudsearchdomain-2.5.2.post3/types_aiobotocore_cloudsearchdomain/__init__.pyi` & `types-aiobotocore-cloudsearchdomain-2.5.4/types_aiobotocore_cloudsearchdomain/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-cloudsearchdomain-2.5.2.post3/types_aiobotocore_cloudsearchdomain/__main__.py` & `types-aiobotocore-cloudsearchdomain-2.5.4/types_aiobotocore_cloudsearchdomain/__main__.py`

 * *Files 20% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.CloudSearchDomain 2.5.2\nVersion:        "
-        " 2.5.2.post3\nBuilder version: 7.17.2\nDocs:           "
+        "Type annotations for aiobotocore.CloudSearchDomain 2.5.4\nVersion:         2.5.4\nBuilder"
+        " version: 7.17.2\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudsearchdomain//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudsearchdomain.html#CloudSearchDomain\nOther"
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

### Comparing `types-aiobotocore-cloudsearchdomain-2.5.2.post3/types_aiobotocore_cloudsearchdomain/client.py` & `types-aiobotocore-cloudsearchdomain-2.5.4/types_aiobotocore_cloudsearchdomain/client.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-cloudsearchdomain-2.5.2.post3/types_aiobotocore_cloudsearchdomain/client.pyi` & `types-aiobotocore-cloudsearchdomain-2.5.4/types_aiobotocore_cloudsearchdomain/client.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-cloudsearchdomain-2.5.2.post3/types_aiobotocore_cloudsearchdomain/literals.py` & `types-aiobotocore-cloudsearchdomain-2.5.4/types_aiobotocore_cloudsearchdomain/literals.py`

 * *Files 2% similar despite different names*

```diff
@@ -42,14 +42,15 @@
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
@@ -145,14 +146,15 @@
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
@@ -231,26 +233,28 @@
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

### Comparing `types-aiobotocore-cloudsearchdomain-2.5.2.post3/types_aiobotocore_cloudsearchdomain/literals.pyi` & `types-aiobotocore-cloudsearchdomain-2.5.4/types_aiobotocore_cloudsearchdomain/literals.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -40,14 +40,15 @@
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
@@ -143,14 +144,15 @@
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
@@ -229,26 +231,28 @@
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

### Comparing `types-aiobotocore-cloudsearchdomain-2.5.2.post3/types_aiobotocore_cloudsearchdomain/type_defs.py` & `types-aiobotocore-cloudsearchdomain-2.5.4/types_aiobotocore_cloudsearchdomain/type_defs.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-cloudsearchdomain-2.5.2.post3/types_aiobotocore_cloudsearchdomain/type_defs.pyi` & `types-aiobotocore-cloudsearchdomain-2.5.4/types_aiobotocore_cloudsearchdomain/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-cloudsearchdomain-2.5.2.post3/types_aiobotocore_cloudsearchdomain.egg-info/PKG-INFO` & `types-aiobotocore-cloudsearchdomain-2.5.4/types_aiobotocore_cloudsearchdomain.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-cloudsearchdomain
-Version: 2.5.2.post3
-Summary: Type annotations for aiobotocore.CloudSearchDomain 2.5.2 service generated with mypy-boto3-builder 7.17.2
+Version: 2.5.4
+Summary: Type annotations for aiobotocore.CloudSearchDomain 2.5.4 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudsearchdomain/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-cloudsearchdomain.svg?color=blue)](https://pypi.org/project/types-aiobotocore-cloudsearchdomain)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudsearchdomain/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-cloudsearchdomain)](https://pepy.tech/project/types-aiobotocore-cloudsearchdomain)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.CloudSearchDomain 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudsearchdomain.html#CloudSearchDomain)
+[aiobotocore.CloudSearchDomain 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudsearchdomain.html#CloudSearchDomain)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-cloudsearchdomain-2.5.2.post3/types_aiobotocore_cloudsearchdomain.egg-info/SOURCES.txt` & `types-aiobotocore-cloudsearchdomain-2.5.4/types_aiobotocore_cloudsearchdomain.egg-info/SOURCES.txt`

 * *Files identical despite different names*


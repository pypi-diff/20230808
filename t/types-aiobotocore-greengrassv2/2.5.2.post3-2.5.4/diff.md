# Comparing `tmp/types-aiobotocore-greengrassv2-2.5.2.post3.tar.gz` & `tmp/types-aiobotocore-greengrassv2-2.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-greengrassv2-2.5.2.post3.tar", last modified: Fri Aug  4 12:37:47 2023, max compression
+gzip compressed data, was "types-aiobotocore-greengrassv2-2.5.4.tar", last modified: Tue Aug  8 01:23:47 2023, max compression
```

## Comparing `types-aiobotocore-greengrassv2-2.5.2.post3.tar` & `types-aiobotocore-greengrassv2-2.5.4.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:37:47.011888 types-aiobotocore-greengrassv2-2.5.2.post3/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-04 12:24:42.000000 types-aiobotocore-greengrassv2-2.5.2.post3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    14329 2023-08-04 12:37:47.003888 types-aiobotocore-greengrassv2-2.5.2.post3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    12791 2023-08-04 12:24:42.000000 types-aiobotocore-greengrassv2-2.5.2.post3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-04 12:37:47.011888 types-aiobotocore-greengrassv2-2.5.2.post3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2107 2023-08-04 12:24:42.000000 types-aiobotocore-greengrassv2-2.5.2.post3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:37:47.003888 types-aiobotocore-greengrassv2-2.5.2.post3/types_aiobotocore_greengrassv2/
--rw-r--r--   0 runner    (1001) docker     (123)     2199 2023-08-04 12:24:44.000000 types-aiobotocore-greengrassv2-2.5.2.post3/types_aiobotocore_greengrassv2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2198 2023-08-04 12:24:42.000000 types-aiobotocore-greengrassv2-2.5.2.post3/types_aiobotocore_greengrassv2/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      963 2023-08-04 12:24:44.000000 types-aiobotocore-greengrassv2-2.5.2.post3/types_aiobotocore_greengrassv2/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    27438 2023-08-04 12:24:44.000000 types-aiobotocore-greengrassv2-2.5.2.post3/types_aiobotocore_greengrassv2/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    27393 2023-08-04 12:24:44.000000 types-aiobotocore-greengrassv2-2.5.2.post3/types_aiobotocore_greengrassv2/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    11048 2023-08-04 12:24:44.000000 types-aiobotocore-greengrassv2-2.5.2.post3/types_aiobotocore_greengrassv2/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    11046 2023-08-04 12:24:44.000000 types-aiobotocore-greengrassv2-2.5.2.post3/types_aiobotocore_greengrassv2/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9911 2023-08-04 12:24:44.000000 types-aiobotocore-greengrassv2-2.5.2.post3/types_aiobotocore_greengrassv2/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     9902 2023-08-04 12:24:44.000000 types-aiobotocore-greengrassv2-2.5.2.post3/types_aiobotocore_greengrassv2/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 12:24:44.000000 types-aiobotocore-greengrassv2-2.5.2.post3/types_aiobotocore_greengrassv2/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    37212 2023-08-04 12:24:45.000000 types-aiobotocore-greengrassv2-2.5.2.post3/types_aiobotocore_greengrassv2/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    37179 2023-08-04 12:24:44.000000 types-aiobotocore-greengrassv2-2.5.2.post3/types_aiobotocore_greengrassv2/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-04 12:24:42.000000 types-aiobotocore-greengrassv2-2.5.2.post3/types_aiobotocore_greengrassv2/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:37:47.003888 types-aiobotocore-greengrassv2-2.5.2.post3/types_aiobotocore_greengrassv2.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    14329 2023-08-04 12:37:46.000000 types-aiobotocore-greengrassv2-2.5.2.post3/types_aiobotocore_greengrassv2.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      908 2023-08-04 12:37:46.000000 types-aiobotocore-greengrassv2-2.5.2.post3/types_aiobotocore_greengrassv2.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 12:37:46.000000 types-aiobotocore-greengrassv2-2.5.2.post3/types_aiobotocore_greengrassv2.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 12:37:46.000000 types-aiobotocore-greengrassv2-2.5.2.post3/types_aiobotocore_greengrassv2.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-04 12:37:46.000000 types-aiobotocore-greengrassv2-2.5.2.post3/types_aiobotocore_greengrassv2.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-08-04 12:37:46.000000 types-aiobotocore-greengrassv2-2.5.2.post3/types_aiobotocore_greengrassv2.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:23:47.850727 types-aiobotocore-greengrassv2-2.5.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-08 01:12:03.000000 types-aiobotocore-greengrassv2-2.5.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    14323 2023-08-08 01:23:47.850727 types-aiobotocore-greengrassv2-2.5.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    12791 2023-08-08 01:12:03.000000 types-aiobotocore-greengrassv2-2.5.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-08 01:23:47.850727 types-aiobotocore-greengrassv2-2.5.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2101 2023-08-08 01:12:03.000000 types-aiobotocore-greengrassv2-2.5.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:23:47.850727 types-aiobotocore-greengrassv2-2.5.4/types_aiobotocore_greengrassv2/
+-rw-r--r--   0 runner    (1001) docker     (123)     2199 2023-08-08 01:12:03.000000 types-aiobotocore-greengrassv2-2.5.4/types_aiobotocore_greengrassv2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2198 2023-08-08 01:12:03.000000 types-aiobotocore-greengrassv2-2.5.4/types_aiobotocore_greengrassv2/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      951 2023-08-08 01:12:03.000000 types-aiobotocore-greengrassv2-2.5.4/types_aiobotocore_greengrassv2/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27438 2023-08-08 01:12:03.000000 types-aiobotocore-greengrassv2-2.5.4/types_aiobotocore_greengrassv2/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27393 2023-08-08 01:12:03.000000 types-aiobotocore-greengrassv2-2.5.4/types_aiobotocore_greengrassv2/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    11143 2023-08-08 01:12:03.000000 types-aiobotocore-greengrassv2-2.5.4/types_aiobotocore_greengrassv2/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11141 2023-08-08 01:12:03.000000 types-aiobotocore-greengrassv2-2.5.4/types_aiobotocore_greengrassv2/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9911 2023-08-08 01:12:03.000000 types-aiobotocore-greengrassv2-2.5.4/types_aiobotocore_greengrassv2/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9902 2023-08-08 01:12:03.000000 types-aiobotocore-greengrassv2-2.5.4/types_aiobotocore_greengrassv2/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 01:12:03.000000 types-aiobotocore-greengrassv2-2.5.4/types_aiobotocore_greengrassv2/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    37212 2023-08-08 01:12:04.000000 types-aiobotocore-greengrassv2-2.5.4/types_aiobotocore_greengrassv2/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37179 2023-08-08 01:12:04.000000 types-aiobotocore-greengrassv2-2.5.4/types_aiobotocore_greengrassv2/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-08-08 01:12:03.000000 types-aiobotocore-greengrassv2-2.5.4/types_aiobotocore_greengrassv2/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:23:47.850727 types-aiobotocore-greengrassv2-2.5.4/types_aiobotocore_greengrassv2.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    14323 2023-08-08 01:23:47.000000 types-aiobotocore-greengrassv2-2.5.4/types_aiobotocore_greengrassv2.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      908 2023-08-08 01:23:47.000000 types-aiobotocore-greengrassv2-2.5.4/types_aiobotocore_greengrassv2.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 01:23:47.000000 types-aiobotocore-greengrassv2-2.5.4/types_aiobotocore_greengrassv2.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 01:23:47.000000 types-aiobotocore-greengrassv2-2.5.4/types_aiobotocore_greengrassv2.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-08 01:23:47.000000 types-aiobotocore-greengrassv2-2.5.4/types_aiobotocore_greengrassv2.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-08-08 01:23:47.000000 types-aiobotocore-greengrassv2-2.5.4/types_aiobotocore_greengrassv2.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-greengrassv2-2.5.2.post3/LICENSE` & `types-aiobotocore-greengrassv2-2.5.4/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-greengrassv2-2.5.2.post3/PKG-INFO` & `types-aiobotocore-greengrassv2-2.5.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-greengrassv2
-Version: 2.5.2.post3
-Summary: Type annotations for aiobotocore.GreengrassV2 2.5.2 service generated with mypy-boto3-builder 7.17.2
+Version: 2.5.4
+Summary: Type annotations for aiobotocore.GreengrassV2 2.5.4 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_greengrassv2/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-greengrassv2.svg?color=blue)](https://pypi.org/project/types-aiobotocore-greengrassv2)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_greengrassv2/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-greengrassv2)](https://pepy.tech/project/types-aiobotocore-greengrassv2)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.GreengrassV2 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/greengrassv2.html#GreengrassV2)
+[aiobotocore.GreengrassV2 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/greengrassv2.html#GreengrassV2)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-greengrassv2-2.5.2.post3/README.md` & `types-aiobotocore-greengrassv2-2.5.4/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-greengrassv2.svg?color=blue)](https://pypi.org/project/types-aiobotocore-greengrassv2)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_greengrassv2/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-greengrassv2)](https://pepy.tech/project/types-aiobotocore-greengrassv2)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.GreengrassV2 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/greengrassv2.html#GreengrassV2)
+[aiobotocore.GreengrassV2 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/greengrassv2.html#GreengrassV2)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-greengrassv2-2.5.2.post3/setup.py` & `types-aiobotocore-greengrassv2-2.5.4/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-greengrassv2",
-    version="2.5.2.post3",
+    version="2.5.4",
     packages=["types_aiobotocore_greengrassv2"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.GreengrassV2 2.5.2 service generated with"
+        "Type annotations for aiobotocore.GreengrassV2 2.5.4 service generated with"
         " mypy-boto3-builder 7.17.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
```

### Comparing `types-aiobotocore-greengrassv2-2.5.2.post3/types_aiobotocore_greengrassv2/__init__.py` & `types-aiobotocore-greengrassv2-2.5.4/types_aiobotocore_greengrassv2/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-greengrassv2-2.5.2.post3/types_aiobotocore_greengrassv2/__init__.pyi` & `types-aiobotocore-greengrassv2-2.5.4/types_aiobotocore_greengrassv2/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-greengrassv2-2.5.2.post3/types_aiobotocore_greengrassv2/client.py` & `types-aiobotocore-greengrassv2-2.5.4/types_aiobotocore_greengrassv2/client.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-greengrassv2-2.5.2.post3/types_aiobotocore_greengrassv2/client.pyi` & `types-aiobotocore-greengrassv2-2.5.4/types_aiobotocore_greengrassv2/client.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-greengrassv2-2.5.2.post3/types_aiobotocore_greengrassv2/literals.py` & `types-aiobotocore-greengrassv2-2.5.4/types_aiobotocore_greengrassv2/literals.py`

 * *Files 1% similar despite different names*

```diff
@@ -98,14 +98,15 @@
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
@@ -201,14 +202,15 @@
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
@@ -287,26 +289,28 @@
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

### Comparing `types-aiobotocore-greengrassv2-2.5.2.post3/types_aiobotocore_greengrassv2/literals.pyi` & `types-aiobotocore-greengrassv2-2.5.4/types_aiobotocore_greengrassv2/literals.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -96,14 +96,15 @@
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
@@ -199,14 +200,15 @@
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
@@ -285,26 +287,28 @@
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

### Comparing `types-aiobotocore-greengrassv2-2.5.2.post3/types_aiobotocore_greengrassv2/paginator.py` & `types-aiobotocore-greengrassv2-2.5.4/types_aiobotocore_greengrassv2/paginator.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-greengrassv2-2.5.2.post3/types_aiobotocore_greengrassv2/paginator.pyi` & `types-aiobotocore-greengrassv2-2.5.4/types_aiobotocore_greengrassv2/paginator.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-greengrassv2-2.5.2.post3/types_aiobotocore_greengrassv2/type_defs.py` & `types-aiobotocore-greengrassv2-2.5.4/types_aiobotocore_greengrassv2/type_defs.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-greengrassv2-2.5.2.post3/types_aiobotocore_greengrassv2/type_defs.pyi` & `types-aiobotocore-greengrassv2-2.5.4/types_aiobotocore_greengrassv2/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-greengrassv2-2.5.2.post3/types_aiobotocore_greengrassv2.egg-info/PKG-INFO` & `types-aiobotocore-greengrassv2-2.5.4/types_aiobotocore_greengrassv2.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-greengrassv2
-Version: 2.5.2.post3
-Summary: Type annotations for aiobotocore.GreengrassV2 2.5.2 service generated with mypy-boto3-builder 7.17.2
+Version: 2.5.4
+Summary: Type annotations for aiobotocore.GreengrassV2 2.5.4 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_greengrassv2/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-greengrassv2.svg?color=blue)](https://pypi.org/project/types-aiobotocore-greengrassv2)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_greengrassv2/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-greengrassv2)](https://pepy.tech/project/types-aiobotocore-greengrassv2)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.GreengrassV2 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/greengrassv2.html#GreengrassV2)
+[aiobotocore.GreengrassV2 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/greengrassv2.html#GreengrassV2)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-greengrassv2-2.5.2.post3/types_aiobotocore_greengrassv2.egg-info/SOURCES.txt` & `types-aiobotocore-greengrassv2-2.5.4/types_aiobotocore_greengrassv2.egg-info/SOURCES.txt`

 * *Files identical despite different names*


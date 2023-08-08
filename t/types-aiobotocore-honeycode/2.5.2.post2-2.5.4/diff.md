# Comparing `tmp/types-aiobotocore-honeycode-2.5.2.post2.tar.gz` & `tmp/types-aiobotocore-honeycode-2.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-honeycode-2.5.2.post2.tar", last modified: Fri Aug  4 12:37:48 2023, max compression
+gzip compressed data, was "types-aiobotocore-honeycode-2.5.4.tar", last modified: Tue Aug  8 01:23:48 2023, max compression
```

## Comparing `types-aiobotocore-honeycode-2.5.2.post2.tar` & `types-aiobotocore-honeycode-2.5.4.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:37:48.751929 types-aiobotocore-honeycode-2.5.2.post2/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-04 12:24:54.000000 types-aiobotocore-honeycode-2.5.2.post2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    13404 2023-08-04 12:37:48.743929 types-aiobotocore-honeycode-2.5.2.post2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    11878 2023-08-04 12:24:54.000000 types-aiobotocore-honeycode-2.5.2.post2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-04 12:37:48.751929 types-aiobotocore-honeycode-2.5.2.post2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2086 2023-08-04 12:24:54.000000 types-aiobotocore-honeycode-2.5.2.post2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:37:48.743929 types-aiobotocore-honeycode-2.5.2.post2/types_aiobotocore_honeycode/
--rw-r--r--   0 runner    (1001) docker     (123)     1245 2023-08-04 12:24:54.000000 types-aiobotocore-honeycode-2.5.2.post2/types_aiobotocore_honeycode/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1244 2023-08-04 12:24:54.000000 types-aiobotocore-honeycode-2.5.2.post2/types_aiobotocore_honeycode/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      951 2023-08-04 12:24:54.000000 types-aiobotocore-honeycode-2.5.2.post2/types_aiobotocore_honeycode/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16914 2023-08-04 12:24:56.000000 types-aiobotocore-honeycode-2.5.2.post2/types_aiobotocore_honeycode/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    16886 2023-08-04 12:24:56.000000 types-aiobotocore-honeycode-2.5.2.post2/types_aiobotocore_honeycode/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9168 2023-08-04 12:24:56.000000 types-aiobotocore-honeycode-2.5.2.post2/types_aiobotocore_honeycode/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     9166 2023-08-04 12:24:56.000000 types-aiobotocore-honeycode-2.5.2.post2/types_aiobotocore_honeycode/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     5466 2023-08-04 12:24:56.000000 types-aiobotocore-honeycode-2.5.2.post2/types_aiobotocore_honeycode/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     5460 2023-08-04 12:24:56.000000 types-aiobotocore-honeycode-2.5.2.post2/types_aiobotocore_honeycode/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 12:24:54.000000 types-aiobotocore-honeycode-2.5.2.post2/types_aiobotocore_honeycode/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    20818 2023-08-04 12:24:57.000000 types-aiobotocore-honeycode-2.5.2.post2/types_aiobotocore_honeycode/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    20783 2023-08-04 12:24:56.000000 types-aiobotocore-honeycode-2.5.2.post2/types_aiobotocore_honeycode/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-04 12:24:54.000000 types-aiobotocore-honeycode-2.5.2.post2/types_aiobotocore_honeycode/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:37:48.743929 types-aiobotocore-honeycode-2.5.2.post2/types_aiobotocore_honeycode.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    13404 2023-08-04 12:37:48.000000 types-aiobotocore-honeycode-2.5.2.post2/types_aiobotocore_honeycode.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      851 2023-08-04 12:37:48.000000 types-aiobotocore-honeycode-2.5.2.post2/types_aiobotocore_honeycode.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 12:37:48.000000 types-aiobotocore-honeycode-2.5.2.post2/types_aiobotocore_honeycode.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 12:37:48.000000 types-aiobotocore-honeycode-2.5.2.post2/types_aiobotocore_honeycode.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-04 12:37:48.000000 types-aiobotocore-honeycode-2.5.2.post2/types_aiobotocore_honeycode.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-08-04 12:37:48.000000 types-aiobotocore-honeycode-2.5.2.post2/types_aiobotocore_honeycode.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:23:48.626729 types-aiobotocore-honeycode-2.5.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-08 01:12:13.000000 types-aiobotocore-honeycode-2.5.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    13398 2023-08-08 01:23:48.626729 types-aiobotocore-honeycode-2.5.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    11878 2023-08-08 01:12:13.000000 types-aiobotocore-honeycode-2.5.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-08 01:23:48.626729 types-aiobotocore-honeycode-2.5.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2080 2023-08-08 01:12:13.000000 types-aiobotocore-honeycode-2.5.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:23:48.626729 types-aiobotocore-honeycode-2.5.4/types_aiobotocore_honeycode/
+-rw-r--r--   0 runner    (1001) docker     (123)     1245 2023-08-08 01:12:13.000000 types-aiobotocore-honeycode-2.5.4/types_aiobotocore_honeycode/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1244 2023-08-08 01:12:13.000000 types-aiobotocore-honeycode-2.5.4/types_aiobotocore_honeycode/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      939 2023-08-08 01:12:13.000000 types-aiobotocore-honeycode-2.5.4/types_aiobotocore_honeycode/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16914 2023-08-08 01:12:14.000000 types-aiobotocore-honeycode-2.5.4/types_aiobotocore_honeycode/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16886 2023-08-08 01:12:13.000000 types-aiobotocore-honeycode-2.5.4/types_aiobotocore_honeycode/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9263 2023-08-08 01:12:14.000000 types-aiobotocore-honeycode-2.5.4/types_aiobotocore_honeycode/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9261 2023-08-08 01:12:14.000000 types-aiobotocore-honeycode-2.5.4/types_aiobotocore_honeycode/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     5466 2023-08-08 01:12:14.000000 types-aiobotocore-honeycode-2.5.4/types_aiobotocore_honeycode/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5460 2023-08-08 01:12:14.000000 types-aiobotocore-honeycode-2.5.4/types_aiobotocore_honeycode/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 01:12:13.000000 types-aiobotocore-honeycode-2.5.4/types_aiobotocore_honeycode/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    20818 2023-08-08 01:12:15.000000 types-aiobotocore-honeycode-2.5.4/types_aiobotocore_honeycode/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20783 2023-08-08 01:12:15.000000 types-aiobotocore-honeycode-2.5.4/types_aiobotocore_honeycode/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-08-08 01:12:13.000000 types-aiobotocore-honeycode-2.5.4/types_aiobotocore_honeycode/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:23:48.626729 types-aiobotocore-honeycode-2.5.4/types_aiobotocore_honeycode.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    13398 2023-08-08 01:23:48.000000 types-aiobotocore-honeycode-2.5.4/types_aiobotocore_honeycode.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      851 2023-08-08 01:23:48.000000 types-aiobotocore-honeycode-2.5.4/types_aiobotocore_honeycode.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 01:23:48.000000 types-aiobotocore-honeycode-2.5.4/types_aiobotocore_honeycode.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 01:23:48.000000 types-aiobotocore-honeycode-2.5.4/types_aiobotocore_honeycode.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-08 01:23:48.000000 types-aiobotocore-honeycode-2.5.4/types_aiobotocore_honeycode.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-08-08 01:23:48.000000 types-aiobotocore-honeycode-2.5.4/types_aiobotocore_honeycode.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-honeycode-2.5.2.post2/LICENSE` & `types-aiobotocore-honeycode-2.5.4/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-honeycode-2.5.2.post2/PKG-INFO` & `types-aiobotocore-honeycode-2.5.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-honeycode
-Version: 2.5.2.post2
-Summary: Type annotations for aiobotocore.Honeycode 2.5.2 service generated with mypy-boto3-builder 7.17.2
+Version: 2.5.4
+Summary: Type annotations for aiobotocore.Honeycode 2.5.4 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_honeycode/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-honeycode.svg?color=blue)](https://pypi.org/project/types-aiobotocore-honeycode)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_honeycode/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-honeycode)](https://pepy.tech/project/types-aiobotocore-honeycode)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.Honeycode 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/honeycode.html#Honeycode)
+[aiobotocore.Honeycode 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/honeycode.html#Honeycode)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-honeycode-2.5.2.post2/README.md` & `types-aiobotocore-honeycode-2.5.4/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-honeycode.svg?color=blue)](https://pypi.org/project/types-aiobotocore-honeycode)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_honeycode/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-honeycode)](https://pepy.tech/project/types-aiobotocore-honeycode)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.Honeycode 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/honeycode.html#Honeycode)
+[aiobotocore.Honeycode 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/honeycode.html#Honeycode)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-honeycode-2.5.2.post2/setup.py` & `types-aiobotocore-honeycode-2.5.4/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-honeycode",
-    version="2.5.2.post2",
+    version="2.5.4",
     packages=["types_aiobotocore_honeycode"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.Honeycode 2.5.2 service generated with mypy-boto3-builder"
+        "Type annotations for aiobotocore.Honeycode 2.5.4 service generated with mypy-boto3-builder"
         " 7.17.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
```

### Comparing `types-aiobotocore-honeycode-2.5.2.post2/types_aiobotocore_honeycode/__init__.py` & `types-aiobotocore-honeycode-2.5.4/types_aiobotocore_honeycode/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-honeycode-2.5.2.post2/types_aiobotocore_honeycode/__init__.pyi` & `types-aiobotocore-honeycode-2.5.4/types_aiobotocore_honeycode/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-honeycode-2.5.2.post2/types_aiobotocore_honeycode/__main__.py` & `types-aiobotocore-honeycode-2.5.4/types_aiobotocore_honeycode/__main__.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.Honeycode 2.5.2\nVersion:         2.5.2.post2\nBuilder"
-        " version: 7.17.2\nDocs:           "
+        "Type annotations for aiobotocore.Honeycode 2.5.4\nVersion:         2.5.4\nBuilder version:"
+        " 7.17.2\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_honeycode//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/honeycode.html#Honeycode\nOther"
         " services:  https://pypi.org/project/boto3-stubs/\nChangelog:      "
         " https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("2.5.2.post2")
+    print("2.5.4")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `types-aiobotocore-honeycode-2.5.2.post2/types_aiobotocore_honeycode/client.py` & `types-aiobotocore-honeycode-2.5.4/types_aiobotocore_honeycode/client.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-honeycode-2.5.2.post2/types_aiobotocore_honeycode/client.pyi` & `types-aiobotocore-honeycode-2.5.4/types_aiobotocore_honeycode/client.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-honeycode-2.5.2.post2/types_aiobotocore_honeycode/literals.py` & `types-aiobotocore-honeycode-2.5.4/types_aiobotocore_honeycode/literals.py`

 * *Files 2% similar despite different names*

```diff
@@ -90,14 +90,15 @@
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
@@ -193,14 +194,15 @@
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
@@ -279,26 +281,28 @@
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

### Comparing `types-aiobotocore-honeycode-2.5.2.post2/types_aiobotocore_honeycode/literals.pyi` & `types-aiobotocore-honeycode-2.5.4/types_aiobotocore_honeycode/literals.pyi`

 * *Files 3% similar despite different names*

```diff
@@ -88,14 +88,15 @@
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
@@ -191,14 +192,15 @@
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
@@ -277,26 +279,28 @@
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

### Comparing `types-aiobotocore-honeycode-2.5.2.post2/types_aiobotocore_honeycode/paginator.py` & `types-aiobotocore-honeycode-2.5.4/types_aiobotocore_honeycode/paginator.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-honeycode-2.5.2.post2/types_aiobotocore_honeycode/paginator.pyi` & `types-aiobotocore-honeycode-2.5.4/types_aiobotocore_honeycode/paginator.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-honeycode-2.5.2.post2/types_aiobotocore_honeycode/type_defs.py` & `types-aiobotocore-honeycode-2.5.4/types_aiobotocore_honeycode/type_defs.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-honeycode-2.5.2.post2/types_aiobotocore_honeycode/type_defs.pyi` & `types-aiobotocore-honeycode-2.5.4/types_aiobotocore_honeycode/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-honeycode-2.5.2.post2/types_aiobotocore_honeycode.egg-info/PKG-INFO` & `types-aiobotocore-honeycode-2.5.4/types_aiobotocore_honeycode.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-honeycode
-Version: 2.5.2.post2
-Summary: Type annotations for aiobotocore.Honeycode 2.5.2 service generated with mypy-boto3-builder 7.17.2
+Version: 2.5.4
+Summary: Type annotations for aiobotocore.Honeycode 2.5.4 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_honeycode/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-honeycode.svg?color=blue)](https://pypi.org/project/types-aiobotocore-honeycode)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_honeycode/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-honeycode)](https://pepy.tech/project/types-aiobotocore-honeycode)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.Honeycode 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/honeycode.html#Honeycode)
+[aiobotocore.Honeycode 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/honeycode.html#Honeycode)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-honeycode-2.5.2.post2/types_aiobotocore_honeycode.egg-info/SOURCES.txt` & `types-aiobotocore-honeycode-2.5.4/types_aiobotocore_honeycode.egg-info/SOURCES.txt`

 * *Files identical despite different names*


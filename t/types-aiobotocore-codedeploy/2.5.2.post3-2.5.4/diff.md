# Comparing `tmp/types-aiobotocore-codedeploy-2.5.2.post3.tar.gz` & `tmp/types-aiobotocore-codedeploy-2.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-codedeploy-2.5.2.post3.tar", last modified: Fri Aug  4 12:37:28 2023, max compression
+gzip compressed data, was "types-aiobotocore-codedeploy-2.5.4.tar", last modified: Tue Aug  8 01:23:28 2023, max compression
```

## Comparing `types-aiobotocore-codedeploy-2.5.2.post3.tar` & `types-aiobotocore-codedeploy-2.5.4.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:37:28.843454 types-aiobotocore-codedeploy-2.5.2.post3/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-04 12:20:13.000000 types-aiobotocore-codedeploy-2.5.2.post3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    15226 2023-08-04 12:37:28.831454 types-aiobotocore-codedeploy-2.5.2.post3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    13696 2023-08-04 12:20:13.000000 types-aiobotocore-codedeploy-2.5.2.post3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-04 12:37:28.843454 types-aiobotocore-codedeploy-2.5.2.post3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2093 2023-08-04 12:20:12.000000 types-aiobotocore-codedeploy-2.5.2.post3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:37:28.831454 types-aiobotocore-codedeploy-2.5.2.post3/types_aiobotocore_codedeploy/
--rw-r--r--   0 runner    (1001) docker     (123)     2845 2023-08-04 12:20:13.000000 types-aiobotocore-codedeploy-2.5.2.post3/types_aiobotocore_codedeploy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2844 2023-08-04 12:20:13.000000 types-aiobotocore-codedeploy-2.5.2.post3/types_aiobotocore_codedeploy/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      955 2023-08-04 12:20:13.000000 types-aiobotocore-codedeploy-2.5.2.post3/types_aiobotocore_codedeploy/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    48531 2023-08-04 12:20:13.000000 types-aiobotocore-codedeploy-2.5.2.post3/types_aiobotocore_codedeploy/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    48465 2023-08-04 12:20:13.000000 types-aiobotocore-codedeploy-2.5.2.post3/types_aiobotocore_codedeploy/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    14449 2023-08-04 12:20:13.000000 types-aiobotocore-codedeploy-2.5.2.post3/types_aiobotocore_codedeploy/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    14447 2023-08-04 12:20:13.000000 types-aiobotocore-codedeploy-2.5.2.post3/types_aiobotocore_codedeploy/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    12634 2023-08-04 12:20:13.000000 types-aiobotocore-codedeploy-2.5.2.post3/types_aiobotocore_codedeploy/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)    12623 2023-08-04 12:20:13.000000 types-aiobotocore-codedeploy-2.5.2.post3/types_aiobotocore_codedeploy/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 12:20:13.000000 types-aiobotocore-codedeploy-2.5.2.post3/types_aiobotocore_codedeploy/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    50667 2023-08-04 12:20:14.000000 types-aiobotocore-codedeploy-2.5.2.post3/types_aiobotocore_codedeploy/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    50634 2023-08-04 12:20:14.000000 types-aiobotocore-codedeploy-2.5.2.post3/types_aiobotocore_codedeploy/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-04 12:20:13.000000 types-aiobotocore-codedeploy-2.5.2.post3/types_aiobotocore_codedeploy/version.py
--rw-r--r--   0 runner    (1001) docker     (123)     1621 2023-08-04 12:20:13.000000 types-aiobotocore-codedeploy-2.5.2.post3/types_aiobotocore_codedeploy/waiter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1620 2023-08-04 12:20:13.000000 types-aiobotocore-codedeploy-2.5.2.post3/types_aiobotocore_codedeploy/waiter.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:37:28.831454 types-aiobotocore-codedeploy-2.5.2.post3/types_aiobotocore_codedeploy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    15226 2023-08-04 12:37:28.000000 types-aiobotocore-codedeploy-2.5.2.post3/types_aiobotocore_codedeploy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      949 2023-08-04 12:37:28.000000 types-aiobotocore-codedeploy-2.5.2.post3/types_aiobotocore_codedeploy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 12:37:28.000000 types-aiobotocore-codedeploy-2.5.2.post3/types_aiobotocore_codedeploy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 12:37:28.000000 types-aiobotocore-codedeploy-2.5.2.post3/types_aiobotocore_codedeploy.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-04 12:37:28.000000 types-aiobotocore-codedeploy-2.5.2.post3/types_aiobotocore_codedeploy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-08-04 12:37:28.000000 types-aiobotocore-codedeploy-2.5.2.post3/types_aiobotocore_codedeploy.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:23:28.890645 types-aiobotocore-codedeploy-2.5.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-08 01:07:52.000000 types-aiobotocore-codedeploy-2.5.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    15220 2023-08-08 01:23:28.882645 types-aiobotocore-codedeploy-2.5.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    13696 2023-08-08 01:07:52.000000 types-aiobotocore-codedeploy-2.5.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-08 01:23:28.890645 types-aiobotocore-codedeploy-2.5.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2087 2023-08-08 01:07:51.000000 types-aiobotocore-codedeploy-2.5.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:23:28.874645 types-aiobotocore-codedeploy-2.5.4/types_aiobotocore_codedeploy/
+-rw-r--r--   0 runner    (1001) docker     (123)     2845 2023-08-08 01:07:52.000000 types-aiobotocore-codedeploy-2.5.4/types_aiobotocore_codedeploy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2844 2023-08-08 01:07:52.000000 types-aiobotocore-codedeploy-2.5.4/types_aiobotocore_codedeploy/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      943 2023-08-08 01:07:52.000000 types-aiobotocore-codedeploy-2.5.4/types_aiobotocore_codedeploy/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    48531 2023-08-08 01:07:53.000000 types-aiobotocore-codedeploy-2.5.4/types_aiobotocore_codedeploy/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    48465 2023-08-08 01:07:52.000000 types-aiobotocore-codedeploy-2.5.4/types_aiobotocore_codedeploy/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    14564 2023-08-08 01:07:53.000000 types-aiobotocore-codedeploy-2.5.4/types_aiobotocore_codedeploy/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14562 2023-08-08 01:07:53.000000 types-aiobotocore-codedeploy-2.5.4/types_aiobotocore_codedeploy/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    12634 2023-08-08 01:07:53.000000 types-aiobotocore-codedeploy-2.5.4/types_aiobotocore_codedeploy/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12623 2023-08-08 01:07:53.000000 types-aiobotocore-codedeploy-2.5.4/types_aiobotocore_codedeploy/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 01:07:52.000000 types-aiobotocore-codedeploy-2.5.4/types_aiobotocore_codedeploy/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    50667 2023-08-08 01:07:54.000000 types-aiobotocore-codedeploy-2.5.4/types_aiobotocore_codedeploy/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    50634 2023-08-08 01:07:54.000000 types-aiobotocore-codedeploy-2.5.4/types_aiobotocore_codedeploy/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-08-08 01:07:52.000000 types-aiobotocore-codedeploy-2.5.4/types_aiobotocore_codedeploy/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1621 2023-08-08 01:07:53.000000 types-aiobotocore-codedeploy-2.5.4/types_aiobotocore_codedeploy/waiter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1620 2023-08-08 01:07:53.000000 types-aiobotocore-codedeploy-2.5.4/types_aiobotocore_codedeploy/waiter.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:23:28.882645 types-aiobotocore-codedeploy-2.5.4/types_aiobotocore_codedeploy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    15220 2023-08-08 01:23:28.000000 types-aiobotocore-codedeploy-2.5.4/types_aiobotocore_codedeploy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      949 2023-08-08 01:23:28.000000 types-aiobotocore-codedeploy-2.5.4/types_aiobotocore_codedeploy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 01:23:28.000000 types-aiobotocore-codedeploy-2.5.4/types_aiobotocore_codedeploy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 01:23:28.000000 types-aiobotocore-codedeploy-2.5.4/types_aiobotocore_codedeploy.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-08 01:23:28.000000 types-aiobotocore-codedeploy-2.5.4/types_aiobotocore_codedeploy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-08-08 01:23:28.000000 types-aiobotocore-codedeploy-2.5.4/types_aiobotocore_codedeploy.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-codedeploy-2.5.2.post3/LICENSE` & `types-aiobotocore-codedeploy-2.5.4/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-codedeploy-2.5.2.post3/PKG-INFO` & `types-aiobotocore-codedeploy-2.5.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-codedeploy
-Version: 2.5.2.post3
-Summary: Type annotations for aiobotocore.CodeDeploy 2.5.2 service generated with mypy-boto3-builder 7.17.2
+Version: 2.5.4
+Summary: Type annotations for aiobotocore.CodeDeploy 2.5.4 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codedeploy/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-codedeploy.svg?color=blue)](https://pypi.org/project/types-aiobotocore-codedeploy)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codedeploy/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-codedeploy)](https://pepy.tech/project/types-aiobotocore-codedeploy)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.CodeDeploy 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codedeploy.html#CodeDeploy)
+[aiobotocore.CodeDeploy 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codedeploy.html#CodeDeploy)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-codedeploy-2.5.2.post3/README.md` & `types-aiobotocore-codedeploy-2.5.4/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-codedeploy.svg?color=blue)](https://pypi.org/project/types-aiobotocore-codedeploy)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codedeploy/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-codedeploy)](https://pepy.tech/project/types-aiobotocore-codedeploy)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.CodeDeploy 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codedeploy.html#CodeDeploy)
+[aiobotocore.CodeDeploy 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codedeploy.html#CodeDeploy)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-codedeploy-2.5.2.post3/setup.py` & `types-aiobotocore-codedeploy-2.5.4/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-codedeploy",
-    version="2.5.2.post3",
+    version="2.5.4",
     packages=["types_aiobotocore_codedeploy"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.CodeDeploy 2.5.2 service generated with"
+        "Type annotations for aiobotocore.CodeDeploy 2.5.4 service generated with"
         " mypy-boto3-builder 7.17.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
```

### Comparing `types-aiobotocore-codedeploy-2.5.2.post3/types_aiobotocore_codedeploy/__init__.py` & `types-aiobotocore-codedeploy-2.5.4/types_aiobotocore_codedeploy/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-codedeploy-2.5.2.post3/types_aiobotocore_codedeploy/__init__.pyi` & `types-aiobotocore-codedeploy-2.5.4/types_aiobotocore_codedeploy/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-codedeploy-2.5.2.post3/types_aiobotocore_codedeploy/__main__.py` & `types-aiobotocore-codedeploy-2.5.4/types_aiobotocore_codedeploy/__main__.py`

 * *Files 13% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.CodeDeploy 2.5.2\nVersion:         2.5.2.post3\nBuilder"
+        "Type annotations for aiobotocore.CodeDeploy 2.5.4\nVersion:         2.5.4\nBuilder"
         " version: 7.17.2\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codedeploy//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codedeploy.html#CodeDeploy\nOther"
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

### Comparing `types-aiobotocore-codedeploy-2.5.2.post3/types_aiobotocore_codedeploy/client.py` & `types-aiobotocore-codedeploy-2.5.4/types_aiobotocore_codedeploy/client.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-codedeploy-2.5.2.post3/types_aiobotocore_codedeploy/client.pyi` & `types-aiobotocore-codedeploy-2.5.4/types_aiobotocore_codedeploy/client.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-codedeploy-2.5.2.post3/types_aiobotocore_codedeploy/literals.py` & `types-aiobotocore-codedeploy-2.5.4/types_aiobotocore_codedeploy/literals.py`

 * *Files 0% similar despite different names*

```diff
@@ -200,14 +200,15 @@
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
@@ -303,14 +304,15 @@
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
@@ -389,26 +391,28 @@
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
@@ -581,14 +585,15 @@
     "eu-central-2",
     "eu-north-1",
     "eu-south-1",
     "eu-south-2",
     "eu-west-1",
     "eu-west-2",
     "eu-west-3",
+    "il-central-1",
     "me-central-1",
     "me-south-1",
     "sa-east-1",
     "us-east-1",
     "us-east-2",
     "us-west-1",
     "us-west-2",
```

### Comparing `types-aiobotocore-codedeploy-2.5.2.post3/types_aiobotocore_codedeploy/literals.pyi` & `types-aiobotocore-codedeploy-2.5.4/types_aiobotocore_codedeploy/literals.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -198,14 +198,15 @@
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
@@ -301,14 +302,15 @@
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
@@ -387,26 +389,28 @@
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
@@ -579,14 +583,15 @@
     "eu-central-2",
     "eu-north-1",
     "eu-south-1",
     "eu-south-2",
     "eu-west-1",
     "eu-west-2",
     "eu-west-3",
+    "il-central-1",
     "me-central-1",
     "me-south-1",
     "sa-east-1",
     "us-east-1",
     "us-east-2",
     "us-west-1",
     "us-west-2",
```

### Comparing `types-aiobotocore-codedeploy-2.5.2.post3/types_aiobotocore_codedeploy/paginator.py` & `types-aiobotocore-codedeploy-2.5.4/types_aiobotocore_codedeploy/paginator.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-codedeploy-2.5.2.post3/types_aiobotocore_codedeploy/paginator.pyi` & `types-aiobotocore-codedeploy-2.5.4/types_aiobotocore_codedeploy/paginator.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-codedeploy-2.5.2.post3/types_aiobotocore_codedeploy/type_defs.py` & `types-aiobotocore-codedeploy-2.5.4/types_aiobotocore_codedeploy/type_defs.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-codedeploy-2.5.2.post3/types_aiobotocore_codedeploy/type_defs.pyi` & `types-aiobotocore-codedeploy-2.5.4/types_aiobotocore_codedeploy/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-codedeploy-2.5.2.post3/types_aiobotocore_codedeploy/waiter.py` & `types-aiobotocore-codedeploy-2.5.4/types_aiobotocore_codedeploy/waiter.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-codedeploy-2.5.2.post3/types_aiobotocore_codedeploy/waiter.pyi` & `types-aiobotocore-codedeploy-2.5.4/types_aiobotocore_codedeploy/waiter.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-codedeploy-2.5.2.post3/types_aiobotocore_codedeploy.egg-info/PKG-INFO` & `types-aiobotocore-codedeploy-2.5.4/types_aiobotocore_codedeploy.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-codedeploy
-Version: 2.5.2.post3
-Summary: Type annotations for aiobotocore.CodeDeploy 2.5.2 service generated with mypy-boto3-builder 7.17.2
+Version: 2.5.4
+Summary: Type annotations for aiobotocore.CodeDeploy 2.5.4 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codedeploy/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-codedeploy.svg?color=blue)](https://pypi.org/project/types-aiobotocore-codedeploy)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codedeploy/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-codedeploy)](https://pepy.tech/project/types-aiobotocore-codedeploy)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.CodeDeploy 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codedeploy.html#CodeDeploy)
+[aiobotocore.CodeDeploy 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codedeploy.html#CodeDeploy)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-codedeploy-2.5.2.post3/types_aiobotocore_codedeploy.egg-info/SOURCES.txt` & `types-aiobotocore-codedeploy-2.5.4/types_aiobotocore_codedeploy.egg-info/SOURCES.txt`

 * *Files identical despite different names*


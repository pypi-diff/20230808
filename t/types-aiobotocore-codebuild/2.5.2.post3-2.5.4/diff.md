# Comparing `tmp/types-aiobotocore-codebuild-2.5.2.post3.tar.gz` & `tmp/types-aiobotocore-codebuild-2.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-codebuild-2.5.2.post3.tar", last modified: Fri Aug  4 12:37:26 2023, max compression
+gzip compressed data, was "types-aiobotocore-codebuild-2.5.4.tar", last modified: Tue Aug  8 01:23:28 2023, max compression
```

## Comparing `types-aiobotocore-codebuild-2.5.2.post3.tar` & `types-aiobotocore-codebuild-2.5.4.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:37:26.655400 types-aiobotocore-codebuild-2.5.2.post3/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-04 12:20:03.000000 types-aiobotocore-codebuild-2.5.2.post3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    14792 2023-08-04 12:37:26.655400 types-aiobotocore-codebuild-2.5.2.post3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    13266 2023-08-04 12:20:03.000000 types-aiobotocore-codebuild-2.5.2.post3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-04 12:37:26.655400 types-aiobotocore-codebuild-2.5.2.post3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2086 2023-08-04 12:20:03.000000 types-aiobotocore-codebuild-2.5.2.post3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:37:26.651399 types-aiobotocore-codebuild-2.5.2.post3/types_aiobotocore_codebuild/
--rw-r--r--   0 runner    (1001) docker     (123)     3083 2023-08-04 12:20:03.000000 types-aiobotocore-codebuild-2.5.2.post3/types_aiobotocore_codebuild/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3082 2023-08-04 12:20:03.000000 types-aiobotocore-codebuild-2.5.2.post3/types_aiobotocore_codebuild/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      951 2023-08-04 12:20:03.000000 types-aiobotocore-codebuild-2.5.2.post3/types_aiobotocore_codebuild/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    43759 2023-08-04 12:20:03.000000 types-aiobotocore-codebuild-2.5.2.post3/types_aiobotocore_codebuild/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    43693 2023-08-04 12:20:03.000000 types-aiobotocore-codebuild-2.5.2.post3/types_aiobotocore_codebuild/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    14108 2023-08-04 12:20:03.000000 types-aiobotocore-codebuild-2.5.2.post3/types_aiobotocore_codebuild/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    14106 2023-08-04 12:20:03.000000 types-aiobotocore-codebuild-2.5.2.post3/types_aiobotocore_codebuild/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    15950 2023-08-04 12:20:03.000000 types-aiobotocore-codebuild-2.5.2.post3/types_aiobotocore_codebuild/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)    15936 2023-08-04 12:20:03.000000 types-aiobotocore-codebuild-2.5.2.post3/types_aiobotocore_codebuild/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 12:20:03.000000 types-aiobotocore-codebuild-2.5.2.post3/types_aiobotocore_codebuild/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    57197 2023-08-04 12:20:05.000000 types-aiobotocore-codebuild-2.5.2.post3/types_aiobotocore_codebuild/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    57138 2023-08-04 12:20:04.000000 types-aiobotocore-codebuild-2.5.2.post3/types_aiobotocore_codebuild/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-04 12:20:03.000000 types-aiobotocore-codebuild-2.5.2.post3/types_aiobotocore_codebuild/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:37:26.655400 types-aiobotocore-codebuild-2.5.2.post3/types_aiobotocore_codebuild.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    14792 2023-08-04 12:37:26.000000 types-aiobotocore-codebuild-2.5.2.post3/types_aiobotocore_codebuild.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      851 2023-08-04 12:37:26.000000 types-aiobotocore-codebuild-2.5.2.post3/types_aiobotocore_codebuild.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 12:37:26.000000 types-aiobotocore-codebuild-2.5.2.post3/types_aiobotocore_codebuild.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 12:37:26.000000 types-aiobotocore-codebuild-2.5.2.post3/types_aiobotocore_codebuild.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-04 12:37:26.000000 types-aiobotocore-codebuild-2.5.2.post3/types_aiobotocore_codebuild.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-08-04 12:37:26.000000 types-aiobotocore-codebuild-2.5.2.post3/types_aiobotocore_codebuild.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:23:28.774644 types-aiobotocore-codebuild-2.5.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-08 01:07:43.000000 types-aiobotocore-codebuild-2.5.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    14786 2023-08-08 01:23:28.774644 types-aiobotocore-codebuild-2.5.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    13266 2023-08-08 01:07:43.000000 types-aiobotocore-codebuild-2.5.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-08 01:23:28.774644 types-aiobotocore-codebuild-2.5.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2080 2023-08-08 01:07:43.000000 types-aiobotocore-codebuild-2.5.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:23:28.774644 types-aiobotocore-codebuild-2.5.4/types_aiobotocore_codebuild/
+-rw-r--r--   0 runner    (1001) docker     (123)     3083 2023-08-08 01:07:43.000000 types-aiobotocore-codebuild-2.5.4/types_aiobotocore_codebuild/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3082 2023-08-08 01:07:43.000000 types-aiobotocore-codebuild-2.5.4/types_aiobotocore_codebuild/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      939 2023-08-08 01:07:43.000000 types-aiobotocore-codebuild-2.5.4/types_aiobotocore_codebuild/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    43759 2023-08-08 01:07:44.000000 types-aiobotocore-codebuild-2.5.4/types_aiobotocore_codebuild/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    43693 2023-08-08 01:07:43.000000 types-aiobotocore-codebuild-2.5.4/types_aiobotocore_codebuild/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    14223 2023-08-08 01:07:44.000000 types-aiobotocore-codebuild-2.5.4/types_aiobotocore_codebuild/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14221 2023-08-08 01:07:44.000000 types-aiobotocore-codebuild-2.5.4/types_aiobotocore_codebuild/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    15950 2023-08-08 01:07:44.000000 types-aiobotocore-codebuild-2.5.4/types_aiobotocore_codebuild/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15936 2023-08-08 01:07:44.000000 types-aiobotocore-codebuild-2.5.4/types_aiobotocore_codebuild/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 01:07:43.000000 types-aiobotocore-codebuild-2.5.4/types_aiobotocore_codebuild/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    57197 2023-08-08 01:07:45.000000 types-aiobotocore-codebuild-2.5.4/types_aiobotocore_codebuild/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    57138 2023-08-08 01:07:44.000000 types-aiobotocore-codebuild-2.5.4/types_aiobotocore_codebuild/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-08-08 01:07:43.000000 types-aiobotocore-codebuild-2.5.4/types_aiobotocore_codebuild/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:23:28.774644 types-aiobotocore-codebuild-2.5.4/types_aiobotocore_codebuild.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    14786 2023-08-08 01:23:28.000000 types-aiobotocore-codebuild-2.5.4/types_aiobotocore_codebuild.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      851 2023-08-08 01:23:28.000000 types-aiobotocore-codebuild-2.5.4/types_aiobotocore_codebuild.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 01:23:28.000000 types-aiobotocore-codebuild-2.5.4/types_aiobotocore_codebuild.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 01:23:28.000000 types-aiobotocore-codebuild-2.5.4/types_aiobotocore_codebuild.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-08 01:23:28.000000 types-aiobotocore-codebuild-2.5.4/types_aiobotocore_codebuild.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-08-08 01:23:28.000000 types-aiobotocore-codebuild-2.5.4/types_aiobotocore_codebuild.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-codebuild-2.5.2.post3/LICENSE` & `types-aiobotocore-codebuild-2.5.4/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-codebuild-2.5.2.post3/PKG-INFO` & `types-aiobotocore-codebuild-2.5.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-codebuild
-Version: 2.5.2.post3
-Summary: Type annotations for aiobotocore.CodeBuild 2.5.2 service generated with mypy-boto3-builder 7.17.2
+Version: 2.5.4
+Summary: Type annotations for aiobotocore.CodeBuild 2.5.4 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codebuild/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-codebuild.svg?color=blue)](https://pypi.org/project/types-aiobotocore-codebuild)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codebuild/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-codebuild)](https://pepy.tech/project/types-aiobotocore-codebuild)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.CodeBuild 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codebuild.html#CodeBuild)
+[aiobotocore.CodeBuild 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codebuild.html#CodeBuild)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-codebuild-2.5.2.post3/README.md` & `types-aiobotocore-codebuild-2.5.4/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-codebuild.svg?color=blue)](https://pypi.org/project/types-aiobotocore-codebuild)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codebuild/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-codebuild)](https://pepy.tech/project/types-aiobotocore-codebuild)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.CodeBuild 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codebuild.html#CodeBuild)
+[aiobotocore.CodeBuild 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codebuild.html#CodeBuild)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-codebuild-2.5.2.post3/setup.py` & `types-aiobotocore-codebuild-2.5.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-codebuild",
-    version="2.5.2.post3",
+    version="2.5.4",
     packages=["types_aiobotocore_codebuild"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.CodeBuild 2.5.2 service generated with mypy-boto3-builder"
+        "Type annotations for aiobotocore.CodeBuild 2.5.4 service generated with mypy-boto3-builder"
         " 7.17.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
```

### Comparing `types-aiobotocore-codebuild-2.5.2.post3/types_aiobotocore_codebuild/__init__.py` & `types-aiobotocore-codebuild-2.5.4/types_aiobotocore_codebuild/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-codebuild-2.5.2.post3/types_aiobotocore_codebuild/__init__.pyi` & `types-aiobotocore-codebuild-2.5.4/types_aiobotocore_codebuild/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-codebuild-2.5.2.post3/types_aiobotocore_codebuild/__main__.py` & `types-aiobotocore-codebuild-2.5.4/types_aiobotocore_codebuild/__main__.py`

 * *Files 27% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.CodeBuild 2.5.2\nVersion:         2.5.2.post3\nBuilder"
-        " version: 7.17.2\nDocs:           "
+        "Type annotations for aiobotocore.CodeBuild 2.5.4\nVersion:         2.5.4\nBuilder version:"
+        " 7.17.2\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codebuild//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codebuild.html#CodeBuild\nOther"
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

### Comparing `types-aiobotocore-codebuild-2.5.2.post3/types_aiobotocore_codebuild/client.py` & `types-aiobotocore-codebuild-2.5.4/types_aiobotocore_codebuild/client.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-codebuild-2.5.2.post3/types_aiobotocore_codebuild/client.pyi` & `types-aiobotocore-codebuild-2.5.4/types_aiobotocore_codebuild/client.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-codebuild-2.5.2.post3/types_aiobotocore_codebuild/literals.py` & `types-aiobotocore-codebuild-2.5.4/types_aiobotocore_codebuild/literals.py`

 * *Files 1% similar despite different names*

```diff
@@ -187,14 +187,15 @@
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
@@ -290,14 +291,15 @@
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
@@ -376,26 +378,28 @@
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
@@ -570,14 +574,15 @@
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

### Comparing `types-aiobotocore-codebuild-2.5.2.post3/types_aiobotocore_codebuild/literals.pyi` & `types-aiobotocore-codebuild-2.5.4/types_aiobotocore_codebuild/literals.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -185,14 +185,15 @@
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
@@ -288,14 +289,15 @@
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
@@ -374,26 +376,28 @@
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
@@ -568,14 +572,15 @@
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

### Comparing `types-aiobotocore-codebuild-2.5.2.post3/types_aiobotocore_codebuild/paginator.py` & `types-aiobotocore-codebuild-2.5.4/types_aiobotocore_codebuild/paginator.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-codebuild-2.5.2.post3/types_aiobotocore_codebuild/paginator.pyi` & `types-aiobotocore-codebuild-2.5.4/types_aiobotocore_codebuild/paginator.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-codebuild-2.5.2.post3/types_aiobotocore_codebuild/type_defs.py` & `types-aiobotocore-codebuild-2.5.4/types_aiobotocore_codebuild/type_defs.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-codebuild-2.5.2.post3/types_aiobotocore_codebuild/type_defs.pyi` & `types-aiobotocore-codebuild-2.5.4/types_aiobotocore_codebuild/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-codebuild-2.5.2.post3/types_aiobotocore_codebuild.egg-info/PKG-INFO` & `types-aiobotocore-codebuild-2.5.4/types_aiobotocore_codebuild.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-codebuild
-Version: 2.5.2.post3
-Summary: Type annotations for aiobotocore.CodeBuild 2.5.2 service generated with mypy-boto3-builder 7.17.2
+Version: 2.5.4
+Summary: Type annotations for aiobotocore.CodeBuild 2.5.4 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codebuild/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-codebuild.svg?color=blue)](https://pypi.org/project/types-aiobotocore-codebuild)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codebuild/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-codebuild)](https://pepy.tech/project/types-aiobotocore-codebuild)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.CodeBuild 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codebuild.html#CodeBuild)
+[aiobotocore.CodeBuild 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codebuild.html#CodeBuild)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-codebuild-2.5.2.post3/types_aiobotocore_codebuild.egg-info/SOURCES.txt` & `types-aiobotocore-codebuild-2.5.4/types_aiobotocore_codebuild.egg-info/SOURCES.txt`

 * *Files identical despite different names*


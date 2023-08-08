# Comparing `tmp/types-aiobotocore-connect-contact-lens-2.5.2.post3.tar.gz` & `tmp/types-aiobotocore-connect-contact-lens-2.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-connect-contact-lens-2.5.2.post3.tar", last modified: Fri Aug  4 12:37:31 2023, max compression
+gzip compressed data, was "types-aiobotocore-connect-contact-lens-2.5.4.tar", last modified: Tue Aug  8 01:23:31 2023, max compression
```

## Comparing `types-aiobotocore-connect-contact-lens-2.5.2.post3.tar` & `types-aiobotocore-connect-contact-lens-2.5.4.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:37:31.727527 types-aiobotocore-connect-contact-lens-2.5.2.post3/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-04 12:20:58.000000 types-aiobotocore-connect-contact-lens-2.5.2.post3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    12861 2023-08-04 12:37:31.727527 types-aiobotocore-connect-contact-lens-2.5.2.post3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    11293 2023-08-04 12:20:58.000000 types-aiobotocore-connect-contact-lens-2.5.2.post3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-04 12:37:31.727527 types-aiobotocore-connect-contact-lens-2.5.2.post3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2153 2023-08-04 12:20:58.000000 types-aiobotocore-connect-contact-lens-2.5.2.post3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:37:31.723527 types-aiobotocore-connect-contact-lens-2.5.2.post3/types_aiobotocore_connect_contact_lens/
--rw-r--r--   0 runner    (1001) docker     (123)      536 2023-08-04 12:20:58.000000 types-aiobotocore-connect-contact-lens-2.5.2.post3/types_aiobotocore_connect_contact_lens/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      535 2023-08-04 12:20:58.000000 types-aiobotocore-connect-contact-lens-2.5.2.post3/types_aiobotocore_connect_contact_lens/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      991 2023-08-04 12:20:58.000000 types-aiobotocore-connect-contact-lens-2.5.2.post3/types_aiobotocore_connect_contact_lens/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5191 2023-08-04 12:20:58.000000 types-aiobotocore-connect-contact-lens-2.5.2.post3/types_aiobotocore_connect_contact_lens/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     5182 2023-08-04 12:20:58.000000 types-aiobotocore-connect-contact-lens-2.5.2.post3/types_aiobotocore_connect_contact_lens/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     7884 2023-08-04 12:20:58.000000 types-aiobotocore-connect-contact-lens-2.5.2.post3/types_aiobotocore_connect_contact_lens/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     7882 2023-08-04 12:20:58.000000 types-aiobotocore-connect-contact-lens-2.5.2.post3/types_aiobotocore_connect_contact_lens/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 12:20:58.000000 types-aiobotocore-connect-contact-lens-2.5.2.post3/types_aiobotocore_connect_contact_lens/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     3637 2023-08-04 12:20:58.000000 types-aiobotocore-connect-contact-lens-2.5.2.post3/types_aiobotocore_connect_contact_lens/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)     3632 2023-08-04 12:20:58.000000 types-aiobotocore-connect-contact-lens-2.5.2.post3/types_aiobotocore_connect_contact_lens/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-04 12:20:58.000000 types-aiobotocore-connect-contact-lens-2.5.2.post3/types_aiobotocore_connect_contact_lens/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:37:31.727527 types-aiobotocore-connect-contact-lens-2.5.2.post3/types_aiobotocore_connect_contact_lens.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    12861 2023-08-04 12:37:31.000000 types-aiobotocore-connect-contact-lens-2.5.2.post3/types_aiobotocore_connect_contact_lens.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      955 2023-08-04 12:37:31.000000 types-aiobotocore-connect-contact-lens-2.5.2.post3/types_aiobotocore_connect_contact_lens.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 12:37:31.000000 types-aiobotocore-connect-contact-lens-2.5.2.post3/types_aiobotocore_connect_contact_lens.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 12:37:31.000000 types-aiobotocore-connect-contact-lens-2.5.2.post3/types_aiobotocore_connect_contact_lens.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-04 12:37:31.000000 types-aiobotocore-connect-contact-lens-2.5.2.post3/types_aiobotocore_connect_contact_lens.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-08-04 12:37:31.000000 types-aiobotocore-connect-contact-lens-2.5.2.post3/types_aiobotocore_connect_contact_lens.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:23:31.838672 types-aiobotocore-connect-contact-lens-2.5.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-08 01:08:34.000000 types-aiobotocore-connect-contact-lens-2.5.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    12855 2023-08-08 01:23:31.834672 types-aiobotocore-connect-contact-lens-2.5.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    11293 2023-08-08 01:08:34.000000 types-aiobotocore-connect-contact-lens-2.5.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-08 01:23:31.838672 types-aiobotocore-connect-contact-lens-2.5.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2147 2023-08-08 01:08:34.000000 types-aiobotocore-connect-contact-lens-2.5.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:23:31.830672 types-aiobotocore-connect-contact-lens-2.5.4/types_aiobotocore_connect_contact_lens/
+-rw-r--r--   0 runner    (1001) docker     (123)      536 2023-08-08 01:08:34.000000 types-aiobotocore-connect-contact-lens-2.5.4/types_aiobotocore_connect_contact_lens/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      535 2023-08-08 01:08:34.000000 types-aiobotocore-connect-contact-lens-2.5.4/types_aiobotocore_connect_contact_lens/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      979 2023-08-08 01:08:34.000000 types-aiobotocore-connect-contact-lens-2.5.4/types_aiobotocore_connect_contact_lens/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5191 2023-08-08 01:08:34.000000 types-aiobotocore-connect-contact-lens-2.5.4/types_aiobotocore_connect_contact_lens/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5182 2023-08-08 01:08:34.000000 types-aiobotocore-connect-contact-lens-2.5.4/types_aiobotocore_connect_contact_lens/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8019 2023-08-08 01:08:34.000000 types-aiobotocore-connect-contact-lens-2.5.4/types_aiobotocore_connect_contact_lens/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8017 2023-08-08 01:08:34.000000 types-aiobotocore-connect-contact-lens-2.5.4/types_aiobotocore_connect_contact_lens/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 01:08:34.000000 types-aiobotocore-connect-contact-lens-2.5.4/types_aiobotocore_connect_contact_lens/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     3637 2023-08-08 01:08:34.000000 types-aiobotocore-connect-contact-lens-2.5.4/types_aiobotocore_connect_contact_lens/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3632 2023-08-08 01:08:34.000000 types-aiobotocore-connect-contact-lens-2.5.4/types_aiobotocore_connect_contact_lens/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-08-08 01:08:34.000000 types-aiobotocore-connect-contact-lens-2.5.4/types_aiobotocore_connect_contact_lens/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:23:31.834672 types-aiobotocore-connect-contact-lens-2.5.4/types_aiobotocore_connect_contact_lens.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    12855 2023-08-08 01:23:31.000000 types-aiobotocore-connect-contact-lens-2.5.4/types_aiobotocore_connect_contact_lens.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      955 2023-08-08 01:23:31.000000 types-aiobotocore-connect-contact-lens-2.5.4/types_aiobotocore_connect_contact_lens.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 01:23:31.000000 types-aiobotocore-connect-contact-lens-2.5.4/types_aiobotocore_connect_contact_lens.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 01:23:31.000000 types-aiobotocore-connect-contact-lens-2.5.4/types_aiobotocore_connect_contact_lens.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-08 01:23:31.000000 types-aiobotocore-connect-contact-lens-2.5.4/types_aiobotocore_connect_contact_lens.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-08-08 01:23:31.000000 types-aiobotocore-connect-contact-lens-2.5.4/types_aiobotocore_connect_contact_lens.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-connect-contact-lens-2.5.2.post3/LICENSE` & `types-aiobotocore-connect-contact-lens-2.5.4/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-connect-contact-lens-2.5.2.post3/PKG-INFO` & `types-aiobotocore-connect-contact-lens-2.5.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-connect-contact-lens
-Version: 2.5.2.post3
-Summary: Type annotations for aiobotocore.ConnectContactLens 2.5.2 service generated with mypy-boto3-builder 7.17.2
+Version: 2.5.4
+Summary: Type annotations for aiobotocore.ConnectContactLens 2.5.4 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_connect_contact_lens/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-connect-contact-lens.svg?color=blue)](https://pypi.org/project/types-aiobotocore-connect-contact-lens)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_connect_contact_lens/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-connect-contact-lens)](https://pepy.tech/project/types-aiobotocore-connect-contact-lens)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.ConnectContactLens 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect-contact-lens.html#ConnectContactLens)
+[aiobotocore.ConnectContactLens 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect-contact-lens.html#ConnectContactLens)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-connect-contact-lens-2.5.2.post3/README.md` & `types-aiobotocore-connect-contact-lens-2.5.4/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-connect-contact-lens.svg?color=blue)](https://pypi.org/project/types-aiobotocore-connect-contact-lens)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_connect_contact_lens/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-connect-contact-lens)](https://pepy.tech/project/types-aiobotocore-connect-contact-lens)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.ConnectContactLens 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect-contact-lens.html#ConnectContactLens)
+[aiobotocore.ConnectContactLens 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect-contact-lens.html#ConnectContactLens)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-connect-contact-lens-2.5.2.post3/setup.py` & `types-aiobotocore-connect-contact-lens-2.5.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-connect-contact-lens",
-    version="2.5.2.post3",
+    version="2.5.4",
     packages=["types_aiobotocore_connect_contact_lens"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.ConnectContactLens 2.5.2 service generated with"
+        "Type annotations for aiobotocore.ConnectContactLens 2.5.4 service generated with"
         " mypy-boto3-builder 7.17.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
```

### Comparing `types-aiobotocore-connect-contact-lens-2.5.2.post3/types_aiobotocore_connect_contact_lens/__init__.py` & `types-aiobotocore-connect-contact-lens-2.5.4/types_aiobotocore_connect_contact_lens/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-connect-contact-lens-2.5.2.post3/types_aiobotocore_connect_contact_lens/__init__.pyi` & `types-aiobotocore-connect-contact-lens-2.5.4/types_aiobotocore_connect_contact_lens/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-connect-contact-lens-2.5.2.post3/types_aiobotocore_connect_contact_lens/__main__.py` & `types-aiobotocore-connect-contact-lens-2.5.4/types_aiobotocore_connect_contact_lens/__main__.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.ConnectContactLens 2.5.2\nVersion:        "
-        " 2.5.2.post3\nBuilder version: 7.17.2\nDocs:           "
+        "Type annotations for aiobotocore.ConnectContactLens 2.5.4\nVersion:         2.5.4\nBuilder"
+        " version: 7.17.2\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_connect_contact_lens//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect-contact-lens.html#ConnectContactLens\nOther"
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

### Comparing `types-aiobotocore-connect-contact-lens-2.5.2.post3/types_aiobotocore_connect_contact_lens/client.py` & `types-aiobotocore-connect-contact-lens-2.5.4/types_aiobotocore_connect_contact_lens/client.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-connect-contact-lens-2.5.2.post3/types_aiobotocore_connect_contact_lens/client.pyi` & `types-aiobotocore-connect-contact-lens-2.5.4/types_aiobotocore_connect_contact_lens/client.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-connect-contact-lens-2.5.2.post3/types_aiobotocore_connect_contact_lens/literals.py` & `types-aiobotocore-connect-contact-lens-2.5.4/types_aiobotocore_connect_contact_lens/literals.py`

 * *Files 2% similar despite different names*

```diff
@@ -41,14 +41,15 @@
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
@@ -144,14 +145,15 @@
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
@@ -230,26 +232,28 @@
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
@@ -392,14 +396,16 @@
     "s3",
     "sns",
     "sqs",
 ]
 RegionName = Literal[
     "ap-northeast-1",
     "ap-northeast-2",
+    "ap-south-1",
+    "ap-southeast-1",
     "ap-southeast-2",
     "ca-central-1",
     "eu-central-1",
     "eu-west-2",
     "us-east-1",
     "us-west-2",
 ]
```

### Comparing `types-aiobotocore-connect-contact-lens-2.5.2.post3/types_aiobotocore_connect_contact_lens/literals.pyi` & `types-aiobotocore-connect-contact-lens-2.5.4/types_aiobotocore_connect_contact_lens/literals.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -39,14 +39,15 @@
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
@@ -142,14 +143,15 @@
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
@@ -228,26 +230,28 @@
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
@@ -390,14 +394,16 @@
     "s3",
     "sns",
     "sqs",
 ]
 RegionName = Literal[
     "ap-northeast-1",
     "ap-northeast-2",
+    "ap-south-1",
+    "ap-southeast-1",
     "ap-southeast-2",
     "ca-central-1",
     "eu-central-1",
     "eu-west-2",
     "us-east-1",
     "us-west-2",
 ]
```

### Comparing `types-aiobotocore-connect-contact-lens-2.5.2.post3/types_aiobotocore_connect_contact_lens/type_defs.py` & `types-aiobotocore-connect-contact-lens-2.5.4/types_aiobotocore_connect_contact_lens/type_defs.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-connect-contact-lens-2.5.2.post3/types_aiobotocore_connect_contact_lens/type_defs.pyi` & `types-aiobotocore-connect-contact-lens-2.5.4/types_aiobotocore_connect_contact_lens/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-connect-contact-lens-2.5.2.post3/types_aiobotocore_connect_contact_lens.egg-info/PKG-INFO` & `types-aiobotocore-connect-contact-lens-2.5.4/types_aiobotocore_connect_contact_lens.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-connect-contact-lens
-Version: 2.5.2.post3
-Summary: Type annotations for aiobotocore.ConnectContactLens 2.5.2 service generated with mypy-boto3-builder 7.17.2
+Version: 2.5.4
+Summary: Type annotations for aiobotocore.ConnectContactLens 2.5.4 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_connect_contact_lens/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-connect-contact-lens.svg?color=blue)](https://pypi.org/project/types-aiobotocore-connect-contact-lens)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_connect_contact_lens/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-connect-contact-lens)](https://pepy.tech/project/types-aiobotocore-connect-contact-lens)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.ConnectContactLens 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect-contact-lens.html#ConnectContactLens)
+[aiobotocore.ConnectContactLens 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect-contact-lens.html#ConnectContactLens)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-connect-contact-lens-2.5.2.post3/types_aiobotocore_connect_contact_lens.egg-info/SOURCES.txt` & `types-aiobotocore-connect-contact-lens-2.5.4/types_aiobotocore_connect_contact_lens.egg-info/SOURCES.txt`

 * *Files identical despite different names*


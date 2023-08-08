# Comparing `tmp/types-aiobotocore-cognito-identity-2.5.2.post3.tar.gz` & `tmp/types-aiobotocore-cognito-identity-2.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-cognito-identity-2.5.2.post3.tar", last modified: Fri Aug  4 12:37:29 2023, max compression
+gzip compressed data, was "types-aiobotocore-cognito-identity-2.5.4.tar", last modified: Tue Aug  8 01:23:31 2023, max compression
```

## Comparing `types-aiobotocore-cognito-identity-2.5.2.post3.tar` & `types-aiobotocore-cognito-identity-2.5.4.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:37:29.183463 types-aiobotocore-cognito-identity-2.5.2.post3/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-04 12:20:25.000000 types-aiobotocore-cognito-identity-2.5.2.post3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    13491 2023-08-04 12:37:29.183463 types-aiobotocore-cognito-identity-2.5.2.post3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    11938 2023-08-04 12:20:25.000000 types-aiobotocore-cognito-identity-2.5.2.post3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-04 12:37:29.183463 types-aiobotocore-cognito-identity-2.5.2.post3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2134 2023-08-04 12:20:25.000000 types-aiobotocore-cognito-identity-2.5.2.post3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:37:29.183463 types-aiobotocore-cognito-identity-2.5.2.post3/types_aiobotocore_cognito_identity/
--rw-r--r--   0 runner    (1001) docker     (123)      734 2023-08-04 12:20:25.000000 types-aiobotocore-cognito-identity-2.5.2.post3/types_aiobotocore_cognito_identity/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      733 2023-08-04 12:20:25.000000 types-aiobotocore-cognito-identity-2.5.2.post3/types_aiobotocore_cognito_identity/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      977 2023-08-04 12:20:25.000000 types-aiobotocore-cognito-identity-2.5.2.post3/types_aiobotocore_cognito_identity/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    21106 2023-08-04 12:20:25.000000 types-aiobotocore-cognito-identity-2.5.2.post3/types_aiobotocore_cognito_identity/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    21073 2023-08-04 12:20:25.000000 types-aiobotocore-cognito-identity-2.5.2.post3/types_aiobotocore_cognito_identity/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8540 2023-08-04 12:20:25.000000 types-aiobotocore-cognito-identity-2.5.2.post3/types_aiobotocore_cognito_identity/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     8538 2023-08-04 12:20:25.000000 types-aiobotocore-cognito-identity-2.5.2.post3/types_aiobotocore_cognito_identity/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2130 2023-08-04 12:20:25.000000 types-aiobotocore-cognito-identity-2.5.2.post3/types_aiobotocore_cognito_identity/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     2127 2023-08-04 12:20:25.000000 types-aiobotocore-cognito-identity-2.5.2.post3/types_aiobotocore_cognito_identity/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 12:20:25.000000 types-aiobotocore-cognito-identity-2.5.2.post3/types_aiobotocore_cognito_identity/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    18259 2023-08-04 12:20:26.000000 types-aiobotocore-cognito-identity-2.5.2.post3/types_aiobotocore_cognito_identity/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    18235 2023-08-04 12:20:25.000000 types-aiobotocore-cognito-identity-2.5.2.post3/types_aiobotocore_cognito_identity/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-04 12:20:25.000000 types-aiobotocore-cognito-identity-2.5.2.post3/types_aiobotocore_cognito_identity/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:37:29.183463 types-aiobotocore-cognito-identity-2.5.2.post3/types_aiobotocore_cognito_identity.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    13491 2023-08-04 12:37:28.000000 types-aiobotocore-cognito-identity-2.5.2.post3/types_aiobotocore_cognito_identity.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      984 2023-08-04 12:37:29.000000 types-aiobotocore-cognito-identity-2.5.2.post3/types_aiobotocore_cognito_identity.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 12:37:29.000000 types-aiobotocore-cognito-identity-2.5.2.post3/types_aiobotocore_cognito_identity.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 12:37:28.000000 types-aiobotocore-cognito-identity-2.5.2.post3/types_aiobotocore_cognito_identity.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-04 12:37:29.000000 types-aiobotocore-cognito-identity-2.5.2.post3/types_aiobotocore_cognito_identity.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-08-04 12:37:29.000000 types-aiobotocore-cognito-identity-2.5.2.post3/types_aiobotocore_cognito_identity.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:23:31.194667 types-aiobotocore-cognito-identity-2.5.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-08 01:08:03.000000 types-aiobotocore-cognito-identity-2.5.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    13485 2023-08-08 01:23:31.190667 types-aiobotocore-cognito-identity-2.5.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    11938 2023-08-08 01:08:03.000000 types-aiobotocore-cognito-identity-2.5.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-08 01:23:31.194667 types-aiobotocore-cognito-identity-2.5.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2128 2023-08-08 01:08:03.000000 types-aiobotocore-cognito-identity-2.5.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:23:31.190667 types-aiobotocore-cognito-identity-2.5.4/types_aiobotocore_cognito_identity/
+-rw-r--r--   0 runner    (1001) docker     (123)      734 2023-08-08 01:08:03.000000 types-aiobotocore-cognito-identity-2.5.4/types_aiobotocore_cognito_identity/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      733 2023-08-08 01:08:03.000000 types-aiobotocore-cognito-identity-2.5.4/types_aiobotocore_cognito_identity/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      965 2023-08-08 01:08:03.000000 types-aiobotocore-cognito-identity-2.5.4/types_aiobotocore_cognito_identity/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21106 2023-08-08 01:08:03.000000 types-aiobotocore-cognito-identity-2.5.4/types_aiobotocore_cognito_identity/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21073 2023-08-08 01:08:03.000000 types-aiobotocore-cognito-identity-2.5.4/types_aiobotocore_cognito_identity/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8635 2023-08-08 01:08:03.000000 types-aiobotocore-cognito-identity-2.5.4/types_aiobotocore_cognito_identity/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8633 2023-08-08 01:08:03.000000 types-aiobotocore-cognito-identity-2.5.4/types_aiobotocore_cognito_identity/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2130 2023-08-08 01:08:03.000000 types-aiobotocore-cognito-identity-2.5.4/types_aiobotocore_cognito_identity/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2127 2023-08-08 01:08:03.000000 types-aiobotocore-cognito-identity-2.5.4/types_aiobotocore_cognito_identity/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 01:08:03.000000 types-aiobotocore-cognito-identity-2.5.4/types_aiobotocore_cognito_identity/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    18259 2023-08-08 01:08:05.000000 types-aiobotocore-cognito-identity-2.5.4/types_aiobotocore_cognito_identity/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18235 2023-08-08 01:08:04.000000 types-aiobotocore-cognito-identity-2.5.4/types_aiobotocore_cognito_identity/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-08-08 01:08:03.000000 types-aiobotocore-cognito-identity-2.5.4/types_aiobotocore_cognito_identity/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:23:31.190667 types-aiobotocore-cognito-identity-2.5.4/types_aiobotocore_cognito_identity.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    13485 2023-08-08 01:23:31.000000 types-aiobotocore-cognito-identity-2.5.4/types_aiobotocore_cognito_identity.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      984 2023-08-08 01:23:31.000000 types-aiobotocore-cognito-identity-2.5.4/types_aiobotocore_cognito_identity.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 01:23:31.000000 types-aiobotocore-cognito-identity-2.5.4/types_aiobotocore_cognito_identity.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 01:23:31.000000 types-aiobotocore-cognito-identity-2.5.4/types_aiobotocore_cognito_identity.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-08 01:23:31.000000 types-aiobotocore-cognito-identity-2.5.4/types_aiobotocore_cognito_identity.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-08-08 01:23:31.000000 types-aiobotocore-cognito-identity-2.5.4/types_aiobotocore_cognito_identity.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-cognito-identity-2.5.2.post3/LICENSE` & `types-aiobotocore-cognito-identity-2.5.4/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-cognito-identity-2.5.2.post3/PKG-INFO` & `types-aiobotocore-cognito-identity-2.5.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-cognito-identity
-Version: 2.5.2.post3
-Summary: Type annotations for aiobotocore.CognitoIdentity 2.5.2 service generated with mypy-boto3-builder 7.17.2
+Version: 2.5.4
+Summary: Type annotations for aiobotocore.CognitoIdentity 2.5.4 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cognito_identity/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-cognito-identity.svg?color=blue)](https://pypi.org/project/types-aiobotocore-cognito-identity)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cognito_identity/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-cognito-identity)](https://pepy.tech/project/types-aiobotocore-cognito-identity)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.CognitoIdentity 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-identity.html#CognitoIdentity)
+[aiobotocore.CognitoIdentity 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-identity.html#CognitoIdentity)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-cognito-identity-2.5.2.post3/README.md` & `types-aiobotocore-cognito-identity-2.5.4/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-cognito-identity.svg?color=blue)](https://pypi.org/project/types-aiobotocore-cognito-identity)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cognito_identity/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-cognito-identity)](https://pepy.tech/project/types-aiobotocore-cognito-identity)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.CognitoIdentity 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-identity.html#CognitoIdentity)
+[aiobotocore.CognitoIdentity 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-identity.html#CognitoIdentity)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-cognito-identity-2.5.2.post3/setup.py` & `types-aiobotocore-cognito-identity-2.5.4/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-cognito-identity",
-    version="2.5.2.post3",
+    version="2.5.4",
     packages=["types_aiobotocore_cognito_identity"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.CognitoIdentity 2.5.2 service generated with"
+        "Type annotations for aiobotocore.CognitoIdentity 2.5.4 service generated with"
         " mypy-boto3-builder 7.17.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
```

### Comparing `types-aiobotocore-cognito-identity-2.5.2.post3/types_aiobotocore_cognito_identity/__init__.py` & `types-aiobotocore-cognito-identity-2.5.4/types_aiobotocore_cognito_identity/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-cognito-identity-2.5.2.post3/types_aiobotocore_cognito_identity/__init__.pyi` & `types-aiobotocore-cognito-identity-2.5.4/types_aiobotocore_cognito_identity/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-cognito-identity-2.5.2.post3/types_aiobotocore_cognito_identity/__main__.py` & `types-aiobotocore-cognito-identity-2.5.4/types_aiobotocore_cognito_identity/__main__.py`

 * *Files 19% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.CognitoIdentity 2.5.2\nVersion:        "
-        " 2.5.2.post3\nBuilder version: 7.17.2\nDocs:           "
+        "Type annotations for aiobotocore.CognitoIdentity 2.5.4\nVersion:         2.5.4\nBuilder"
+        " version: 7.17.2\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cognito_identity//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-identity.html#CognitoIdentity\nOther"
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

### Comparing `types-aiobotocore-cognito-identity-2.5.2.post3/types_aiobotocore_cognito_identity/client.py` & `types-aiobotocore-cognito-identity-2.5.4/types_aiobotocore_cognito_identity/client.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-cognito-identity-2.5.2.post3/types_aiobotocore_cognito_identity/client.pyi` & `types-aiobotocore-cognito-identity-2.5.4/types_aiobotocore_cognito_identity/client.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-cognito-identity-2.5.2.post3/types_aiobotocore_cognito_identity/literals.py` & `types-aiobotocore-cognito-identity-2.5.4/types_aiobotocore_cognito_identity/literals.py`

 * *Files 2% similar despite different names*

```diff
@@ -50,14 +50,15 @@
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
@@ -153,14 +154,15 @@
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
@@ -239,26 +241,28 @@
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

### Comparing `types-aiobotocore-cognito-identity-2.5.2.post3/types_aiobotocore_cognito_identity/literals.pyi` & `types-aiobotocore-cognito-identity-2.5.4/types_aiobotocore_cognito_identity/literals.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -48,14 +48,15 @@
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
@@ -151,14 +152,15 @@
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
@@ -237,26 +239,28 @@
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

### Comparing `types-aiobotocore-cognito-identity-2.5.2.post3/types_aiobotocore_cognito_identity/paginator.py` & `types-aiobotocore-cognito-identity-2.5.4/types_aiobotocore_cognito_identity/paginator.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-cognito-identity-2.5.2.post3/types_aiobotocore_cognito_identity/paginator.pyi` & `types-aiobotocore-cognito-identity-2.5.4/types_aiobotocore_cognito_identity/paginator.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-cognito-identity-2.5.2.post3/types_aiobotocore_cognito_identity/type_defs.py` & `types-aiobotocore-cognito-identity-2.5.4/types_aiobotocore_cognito_identity/type_defs.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-cognito-identity-2.5.2.post3/types_aiobotocore_cognito_identity/type_defs.pyi` & `types-aiobotocore-cognito-identity-2.5.4/types_aiobotocore_cognito_identity/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-cognito-identity-2.5.2.post3/types_aiobotocore_cognito_identity.egg-info/PKG-INFO` & `types-aiobotocore-cognito-identity-2.5.4/types_aiobotocore_cognito_identity.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-cognito-identity
-Version: 2.5.2.post3
-Summary: Type annotations for aiobotocore.CognitoIdentity 2.5.2 service generated with mypy-boto3-builder 7.17.2
+Version: 2.5.4
+Summary: Type annotations for aiobotocore.CognitoIdentity 2.5.4 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cognito_identity/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-cognito-identity.svg?color=blue)](https://pypi.org/project/types-aiobotocore-cognito-identity)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cognito_identity/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-cognito-identity)](https://pepy.tech/project/types-aiobotocore-cognito-identity)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.CognitoIdentity 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-identity.html#CognitoIdentity)
+[aiobotocore.CognitoIdentity 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-identity.html#CognitoIdentity)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-cognito-identity-2.5.2.post3/types_aiobotocore_cognito_identity.egg-info/SOURCES.txt` & `types-aiobotocore-cognito-identity-2.5.4/types_aiobotocore_cognito_identity.egg-info/SOURCES.txt`

 * *Files identical despite different names*


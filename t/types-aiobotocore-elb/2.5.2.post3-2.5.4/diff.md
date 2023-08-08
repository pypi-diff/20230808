# Comparing `tmp/types-aiobotocore-elb-2.5.2.post3.tar.gz` & `tmp/types-aiobotocore-elb-2.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-elb-2.5.2.post3.tar", last modified: Fri Aug  4 12:37:41 2023, max compression
+gzip compressed data, was "types-aiobotocore-elb-2.5.4.tar", last modified: Tue Aug  8 01:23:41 2023, max compression
```

## Comparing `types-aiobotocore-elb-2.5.2.post3.tar` & `types-aiobotocore-elb-2.5.4.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:37:41.711764 types-aiobotocore-elb-2.5.2.post3/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-04 12:23:20.000000 types-aiobotocore-elb-2.5.2.post3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    14111 2023-08-04 12:37:41.703764 types-aiobotocore-elb-2.5.2.post3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    12592 2023-08-04 12:23:20.000000 types-aiobotocore-elb-2.5.2.post3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-04 12:37:41.711764 types-aiobotocore-elb-2.5.2.post3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2037 2023-08-04 12:23:20.000000 types-aiobotocore-elb-2.5.2.post3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:37:41.699764 types-aiobotocore-elb-2.5.2.post3/types_aiobotocore_elb/
--rw-r--r--   0 runner    (1001) docker     (123)     1609 2023-08-04 12:23:20.000000 types-aiobotocore-elb-2.5.2.post3/types_aiobotocore_elb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1608 2023-08-04 12:23:20.000000 types-aiobotocore-elb-2.5.2.post3/types_aiobotocore_elb/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      950 2023-08-04 12:23:20.000000 types-aiobotocore-elb-2.5.2.post3/types_aiobotocore_elb/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    26720 2023-08-04 12:23:20.000000 types-aiobotocore-elb-2.5.2.post3/types_aiobotocore_elb/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    26677 2023-08-04 12:23:20.000000 types-aiobotocore-elb-2.5.2.post3/types_aiobotocore_elb/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8872 2023-08-04 12:23:20.000000 types-aiobotocore-elb-2.5.2.post3/types_aiobotocore_elb/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     8870 2023-08-04 12:23:20.000000 types-aiobotocore-elb-2.5.2.post3/types_aiobotocore_elb/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     3307 2023-08-04 12:23:20.000000 types-aiobotocore-elb-2.5.2.post3/types_aiobotocore_elb/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     3303 2023-08-04 12:23:20.000000 types-aiobotocore-elb-2.5.2.post3/types_aiobotocore_elb/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 12:23:20.000000 types-aiobotocore-elb-2.5.2.post3/types_aiobotocore_elb/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    24573 2023-08-04 12:23:22.000000 types-aiobotocore-elb-2.5.2.post3/types_aiobotocore_elb/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    24550 2023-08-04 12:23:22.000000 types-aiobotocore-elb-2.5.2.post3/types_aiobotocore_elb/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-04 12:23:20.000000 types-aiobotocore-elb-2.5.2.post3/types_aiobotocore_elb/version.py
--rw-r--r--   0 runner    (1001) docker     (123)     3913 2023-08-04 12:23:20.000000 types-aiobotocore-elb-2.5.2.post3/types_aiobotocore_elb/waiter.py
--rw-r--r--   0 runner    (1001) docker     (123)     3910 2023-08-04 12:23:20.000000 types-aiobotocore-elb-2.5.2.post3/types_aiobotocore_elb/waiter.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:37:41.703764 types-aiobotocore-elb-2.5.2.post3/types_aiobotocore_elb.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    14111 2023-08-04 12:37:41.000000 types-aiobotocore-elb-2.5.2.post3/types_aiobotocore_elb.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      802 2023-08-04 12:37:41.000000 types-aiobotocore-elb-2.5.2.post3/types_aiobotocore_elb.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 12:37:41.000000 types-aiobotocore-elb-2.5.2.post3/types_aiobotocore_elb.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 12:37:41.000000 types-aiobotocore-elb-2.5.2.post3/types_aiobotocore_elb.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-04 12:37:41.000000 types-aiobotocore-elb-2.5.2.post3/types_aiobotocore_elb.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-08-04 12:37:41.000000 types-aiobotocore-elb-2.5.2.post3/types_aiobotocore_elb.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:23:41.530707 types-aiobotocore-elb-2.5.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-08 01:10:46.000000 types-aiobotocore-elb-2.5.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    14105 2023-08-08 01:23:41.526707 types-aiobotocore-elb-2.5.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    12592 2023-08-08 01:10:46.000000 types-aiobotocore-elb-2.5.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-08 01:23:41.530707 types-aiobotocore-elb-2.5.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2031 2023-08-08 01:10:45.000000 types-aiobotocore-elb-2.5.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:23:41.518707 types-aiobotocore-elb-2.5.4/types_aiobotocore_elb/
+-rw-r--r--   0 runner    (1001) docker     (123)     1609 2023-08-08 01:10:46.000000 types-aiobotocore-elb-2.5.4/types_aiobotocore_elb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1608 2023-08-08 01:10:46.000000 types-aiobotocore-elb-2.5.4/types_aiobotocore_elb/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      938 2023-08-08 01:10:46.000000 types-aiobotocore-elb-2.5.4/types_aiobotocore_elb/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26720 2023-08-08 01:10:46.000000 types-aiobotocore-elb-2.5.4/types_aiobotocore_elb/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26677 2023-08-08 01:10:46.000000 types-aiobotocore-elb-2.5.4/types_aiobotocore_elb/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8987 2023-08-08 01:10:46.000000 types-aiobotocore-elb-2.5.4/types_aiobotocore_elb/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8985 2023-08-08 01:10:46.000000 types-aiobotocore-elb-2.5.4/types_aiobotocore_elb/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     3307 2023-08-08 01:10:46.000000 types-aiobotocore-elb-2.5.4/types_aiobotocore_elb/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3303 2023-08-08 01:10:46.000000 types-aiobotocore-elb-2.5.4/types_aiobotocore_elb/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 01:10:46.000000 types-aiobotocore-elb-2.5.4/types_aiobotocore_elb/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    24573 2023-08-08 01:10:48.000000 types-aiobotocore-elb-2.5.4/types_aiobotocore_elb/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24550 2023-08-08 01:10:47.000000 types-aiobotocore-elb-2.5.4/types_aiobotocore_elb/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-08-08 01:10:46.000000 types-aiobotocore-elb-2.5.4/types_aiobotocore_elb/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3913 2023-08-08 01:10:46.000000 types-aiobotocore-elb-2.5.4/types_aiobotocore_elb/waiter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3910 2023-08-08 01:10:46.000000 types-aiobotocore-elb-2.5.4/types_aiobotocore_elb/waiter.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:23:41.526707 types-aiobotocore-elb-2.5.4/types_aiobotocore_elb.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    14105 2023-08-08 01:23:41.000000 types-aiobotocore-elb-2.5.4/types_aiobotocore_elb.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      802 2023-08-08 01:23:41.000000 types-aiobotocore-elb-2.5.4/types_aiobotocore_elb.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 01:23:41.000000 types-aiobotocore-elb-2.5.4/types_aiobotocore_elb.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 01:23:41.000000 types-aiobotocore-elb-2.5.4/types_aiobotocore_elb.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-08 01:23:41.000000 types-aiobotocore-elb-2.5.4/types_aiobotocore_elb.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-08-08 01:23:41.000000 types-aiobotocore-elb-2.5.4/types_aiobotocore_elb.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-elb-2.5.2.post3/LICENSE` & `types-aiobotocore-elb-2.5.4/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-elb-2.5.2.post3/PKG-INFO` & `types-aiobotocore-elb-2.5.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-elb
-Version: 2.5.2.post3
-Summary: Type annotations for aiobotocore.ElasticLoadBalancing 2.5.2 service generated with mypy-boto3-builder 7.17.2
+Version: 2.5.4
+Summary: Type annotations for aiobotocore.ElasticLoadBalancing 2.5.4 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elb/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-elb.svg?color=blue)](https://pypi.org/project/types-aiobotocore-elb)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elb/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-elb)](https://pepy.tech/project/types-aiobotocore-elb)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.ElasticLoadBalancing 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elb.html#ElasticLoadBalancing)
+[aiobotocore.ElasticLoadBalancing 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elb.html#ElasticLoadBalancing)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-elb-2.5.2.post3/README.md` & `types-aiobotocore-elb-2.5.4/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-elb.svg?color=blue)](https://pypi.org/project/types-aiobotocore-elb)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elb/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-elb)](https://pepy.tech/project/types-aiobotocore-elb)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.ElasticLoadBalancing 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elb.html#ElasticLoadBalancing)
+[aiobotocore.ElasticLoadBalancing 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elb.html#ElasticLoadBalancing)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-elb-2.5.2.post3/setup.py` & `types-aiobotocore-elb-2.5.4/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-elb",
-    version="2.5.2.post3",
+    version="2.5.4",
     packages=["types_aiobotocore_elb"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.ElasticLoadBalancing 2.5.2 service generated with"
+        "Type annotations for aiobotocore.ElasticLoadBalancing 2.5.4 service generated with"
         " mypy-boto3-builder 7.17.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
```

### Comparing `types-aiobotocore-elb-2.5.2.post3/types_aiobotocore_elb/__init__.py` & `types-aiobotocore-elb-2.5.4/types_aiobotocore_elb/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-elb-2.5.2.post3/types_aiobotocore_elb/__init__.pyi` & `types-aiobotocore-elb-2.5.4/types_aiobotocore_elb/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-elb-2.5.2.post3/types_aiobotocore_elb/__main__.py` & `types-aiobotocore-elb-2.5.4/types_aiobotocore_elb/__main__.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.ElasticLoadBalancing 2.5.2\nVersion:        "
-        " 2.5.2.post3\nBuilder version: 7.17.2\nDocs:           "
+        "Type annotations for aiobotocore.ElasticLoadBalancing 2.5.4\nVersion:        "
+        " 2.5.4\nBuilder version: 7.17.2\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elb//\nBoto3 docs:    "
         "  https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elb.html#ElasticLoadBalancing\nOther"
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

### Comparing `types-aiobotocore-elb-2.5.2.post3/types_aiobotocore_elb/client.py` & `types-aiobotocore-elb-2.5.4/types_aiobotocore_elb/client.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-elb-2.5.2.post3/types_aiobotocore_elb/client.pyi` & `types-aiobotocore-elb-2.5.4/types_aiobotocore_elb/client.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-elb-2.5.2.post3/types_aiobotocore_elb/literals.py` & `types-aiobotocore-elb-2.5.4/types_aiobotocore_elb/literals.py`

 * *Files 1% similar despite different names*

```diff
@@ -51,14 +51,15 @@
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
@@ -154,14 +155,15 @@
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
@@ -240,26 +242,28 @@
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
@@ -422,14 +426,15 @@
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

### Comparing `types-aiobotocore-elb-2.5.2.post3/types_aiobotocore_elb/literals.pyi` & `types-aiobotocore-elb-2.5.4/types_aiobotocore_elb/literals.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -49,14 +49,15 @@
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
@@ -152,14 +153,15 @@
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
@@ -238,26 +240,28 @@
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
@@ -420,14 +424,15 @@
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

### Comparing `types-aiobotocore-elb-2.5.2.post3/types_aiobotocore_elb/paginator.py` & `types-aiobotocore-elb-2.5.4/types_aiobotocore_elb/paginator.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-elb-2.5.2.post3/types_aiobotocore_elb/paginator.pyi` & `types-aiobotocore-elb-2.5.4/types_aiobotocore_elb/paginator.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-elb-2.5.2.post3/types_aiobotocore_elb/type_defs.py` & `types-aiobotocore-elb-2.5.4/types_aiobotocore_elb/type_defs.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-elb-2.5.2.post3/types_aiobotocore_elb/type_defs.pyi` & `types-aiobotocore-elb-2.5.4/types_aiobotocore_elb/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-elb-2.5.2.post3/types_aiobotocore_elb/waiter.py` & `types-aiobotocore-elb-2.5.4/types_aiobotocore_elb/waiter.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-elb-2.5.2.post3/types_aiobotocore_elb/waiter.pyi` & `types-aiobotocore-elb-2.5.4/types_aiobotocore_elb/waiter.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-elb-2.5.2.post3/types_aiobotocore_elb.egg-info/PKG-INFO` & `types-aiobotocore-elb-2.5.4/types_aiobotocore_elb.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-elb
-Version: 2.5.2.post3
-Summary: Type annotations for aiobotocore.ElasticLoadBalancing 2.5.2 service generated with mypy-boto3-builder 7.17.2
+Version: 2.5.4
+Summary: Type annotations for aiobotocore.ElasticLoadBalancing 2.5.4 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elb/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-elb.svg?color=blue)](https://pypi.org/project/types-aiobotocore-elb)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elb/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-elb)](https://pepy.tech/project/types-aiobotocore-elb)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.ElasticLoadBalancing 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elb.html#ElasticLoadBalancing)
+[aiobotocore.ElasticLoadBalancing 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elb.html#ElasticLoadBalancing)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-elb-2.5.2.post3/types_aiobotocore_elb.egg-info/SOURCES.txt` & `types-aiobotocore-elb-2.5.4/types_aiobotocore_elb.egg-info/SOURCES.txt`

 * *Files identical despite different names*


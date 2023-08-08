# Comparing `tmp/types-aiobotocore-elasticbeanstalk-2.5.2.post3.tar.gz` & `tmp/types-aiobotocore-elasticbeanstalk-2.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-elasticbeanstalk-2.5.2.post3.tar", last modified: Fri Aug  4 12:37:41 2023, max compression
+gzip compressed data, was "types-aiobotocore-elasticbeanstalk-2.5.4.tar", last modified: Tue Aug  8 01:23:41 2023, max compression
```

## Comparing `types-aiobotocore-elasticbeanstalk-2.5.2.post3.tar` & `types-aiobotocore-elasticbeanstalk-2.5.4.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:37:41.335755 types-aiobotocore-elasticbeanstalk-2.5.2.post3/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-04 12:23:15.000000 types-aiobotocore-elasticbeanstalk-2.5.2.post3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    15311 2023-08-04 12:37:41.331755 types-aiobotocore-elasticbeanstalk-2.5.2.post3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    13757 2023-08-04 12:23:15.000000 types-aiobotocore-elasticbeanstalk-2.5.2.post3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-04 12:37:41.335755 types-aiobotocore-elasticbeanstalk-2.5.2.post3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2135 2023-08-04 12:23:15.000000 types-aiobotocore-elasticbeanstalk-2.5.2.post3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:37:41.331755 types-aiobotocore-elasticbeanstalk-2.5.2.post3/types_aiobotocore_elasticbeanstalk/
--rw-r--r--   0 runner    (1001) docker     (123)     2421 2023-08-04 12:23:15.000000 types-aiobotocore-elasticbeanstalk-2.5.2.post3/types_aiobotocore_elasticbeanstalk/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2420 2023-08-04 12:23:15.000000 types-aiobotocore-elasticbeanstalk-2.5.2.post3/types_aiobotocore_elasticbeanstalk/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      979 2023-08-04 12:23:15.000000 types-aiobotocore-elasticbeanstalk-2.5.2.post3/types_aiobotocore_elasticbeanstalk/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    45011 2023-08-04 12:23:15.000000 types-aiobotocore-elasticbeanstalk-2.5.2.post3/types_aiobotocore_elasticbeanstalk/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    44947 2023-08-04 12:23:15.000000 types-aiobotocore-elasticbeanstalk-2.5.2.post3/types_aiobotocore_elasticbeanstalk/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    11778 2023-08-04 12:23:16.000000 types-aiobotocore-elasticbeanstalk-2.5.2.post3/types_aiobotocore_elasticbeanstalk/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    11776 2023-08-04 12:23:15.000000 types-aiobotocore-elasticbeanstalk-2.5.2.post3/types_aiobotocore_elasticbeanstalk/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8175 2023-08-04 12:23:15.000000 types-aiobotocore-elasticbeanstalk-2.5.2.post3/types_aiobotocore_elasticbeanstalk/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     8168 2023-08-04 12:23:15.000000 types-aiobotocore-elasticbeanstalk-2.5.2.post3/types_aiobotocore_elasticbeanstalk/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 12:23:15.000000 types-aiobotocore-elasticbeanstalk-2.5.2.post3/types_aiobotocore_elasticbeanstalk/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    52786 2023-08-04 12:23:18.000000 types-aiobotocore-elasticbeanstalk-2.5.2.post3/types_aiobotocore_elasticbeanstalk/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    52747 2023-08-04 12:23:17.000000 types-aiobotocore-elasticbeanstalk-2.5.2.post3/types_aiobotocore_elasticbeanstalk/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-04 12:23:15.000000 types-aiobotocore-elasticbeanstalk-2.5.2.post3/types_aiobotocore_elasticbeanstalk/version.py
--rw-r--r--   0 runner    (1001) docker     (123)     4777 2023-08-04 12:23:15.000000 types-aiobotocore-elasticbeanstalk-2.5.2.post3/types_aiobotocore_elasticbeanstalk/waiter.py
--rw-r--r--   0 runner    (1001) docker     (123)     4774 2023-08-04 12:23:15.000000 types-aiobotocore-elasticbeanstalk-2.5.2.post3/types_aiobotocore_elasticbeanstalk/waiter.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:37:41.331755 types-aiobotocore-elasticbeanstalk-2.5.2.post3/types_aiobotocore_elasticbeanstalk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    15311 2023-08-04 12:37:41.000000 types-aiobotocore-elasticbeanstalk-2.5.2.post3/types_aiobotocore_elasticbeanstalk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-08-04 12:37:41.000000 types-aiobotocore-elasticbeanstalk-2.5.2.post3/types_aiobotocore_elasticbeanstalk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 12:37:41.000000 types-aiobotocore-elasticbeanstalk-2.5.2.post3/types_aiobotocore_elasticbeanstalk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 12:37:41.000000 types-aiobotocore-elasticbeanstalk-2.5.2.post3/types_aiobotocore_elasticbeanstalk.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-04 12:37:41.000000 types-aiobotocore-elasticbeanstalk-2.5.2.post3/types_aiobotocore_elasticbeanstalk.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-08-04 12:37:41.000000 types-aiobotocore-elasticbeanstalk-2.5.2.post3/types_aiobotocore_elasticbeanstalk.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:23:40.998705 types-aiobotocore-elasticbeanstalk-2.5.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-08 01:10:41.000000 types-aiobotocore-elasticbeanstalk-2.5.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    15305 2023-08-08 01:23:40.998705 types-aiobotocore-elasticbeanstalk-2.5.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    13757 2023-08-08 01:10:41.000000 types-aiobotocore-elasticbeanstalk-2.5.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-08 01:23:40.998705 types-aiobotocore-elasticbeanstalk-2.5.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2129 2023-08-08 01:10:41.000000 types-aiobotocore-elasticbeanstalk-2.5.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:23:40.998705 types-aiobotocore-elasticbeanstalk-2.5.4/types_aiobotocore_elasticbeanstalk/
+-rw-r--r--   0 runner    (1001) docker     (123)     2421 2023-08-08 01:10:41.000000 types-aiobotocore-elasticbeanstalk-2.5.4/types_aiobotocore_elasticbeanstalk/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2420 2023-08-08 01:10:41.000000 types-aiobotocore-elasticbeanstalk-2.5.4/types_aiobotocore_elasticbeanstalk/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      967 2023-08-08 01:10:41.000000 types-aiobotocore-elasticbeanstalk-2.5.4/types_aiobotocore_elasticbeanstalk/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    45011 2023-08-08 01:10:41.000000 types-aiobotocore-elasticbeanstalk-2.5.4/types_aiobotocore_elasticbeanstalk/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    44947 2023-08-08 01:10:41.000000 types-aiobotocore-elasticbeanstalk-2.5.4/types_aiobotocore_elasticbeanstalk/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    11893 2023-08-08 01:10:41.000000 types-aiobotocore-elasticbeanstalk-2.5.4/types_aiobotocore_elasticbeanstalk/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11891 2023-08-08 01:10:41.000000 types-aiobotocore-elasticbeanstalk-2.5.4/types_aiobotocore_elasticbeanstalk/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8175 2023-08-08 01:10:41.000000 types-aiobotocore-elasticbeanstalk-2.5.4/types_aiobotocore_elasticbeanstalk/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8168 2023-08-08 01:10:41.000000 types-aiobotocore-elasticbeanstalk-2.5.4/types_aiobotocore_elasticbeanstalk/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 01:10:41.000000 types-aiobotocore-elasticbeanstalk-2.5.4/types_aiobotocore_elasticbeanstalk/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    52786 2023-08-08 01:10:43.000000 types-aiobotocore-elasticbeanstalk-2.5.4/types_aiobotocore_elasticbeanstalk/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    52747 2023-08-08 01:10:43.000000 types-aiobotocore-elasticbeanstalk-2.5.4/types_aiobotocore_elasticbeanstalk/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-08-08 01:10:41.000000 types-aiobotocore-elasticbeanstalk-2.5.4/types_aiobotocore_elasticbeanstalk/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4777 2023-08-08 01:10:41.000000 types-aiobotocore-elasticbeanstalk-2.5.4/types_aiobotocore_elasticbeanstalk/waiter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4774 2023-08-08 01:10:41.000000 types-aiobotocore-elasticbeanstalk-2.5.4/types_aiobotocore_elasticbeanstalk/waiter.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:23:40.998705 types-aiobotocore-elasticbeanstalk-2.5.4/types_aiobotocore_elasticbeanstalk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    15305 2023-08-08 01:23:40.000000 types-aiobotocore-elasticbeanstalk-2.5.4/types_aiobotocore_elasticbeanstalk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-08-08 01:23:40.000000 types-aiobotocore-elasticbeanstalk-2.5.4/types_aiobotocore_elasticbeanstalk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 01:23:40.000000 types-aiobotocore-elasticbeanstalk-2.5.4/types_aiobotocore_elasticbeanstalk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 01:23:40.000000 types-aiobotocore-elasticbeanstalk-2.5.4/types_aiobotocore_elasticbeanstalk.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-08 01:23:40.000000 types-aiobotocore-elasticbeanstalk-2.5.4/types_aiobotocore_elasticbeanstalk.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-08-08 01:23:40.000000 types-aiobotocore-elasticbeanstalk-2.5.4/types_aiobotocore_elasticbeanstalk.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-elasticbeanstalk-2.5.2.post3/LICENSE` & `types-aiobotocore-elasticbeanstalk-2.5.4/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-elasticbeanstalk-2.5.2.post3/PKG-INFO` & `types-aiobotocore-elasticbeanstalk-2.5.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-elasticbeanstalk
-Version: 2.5.2.post3
-Summary: Type annotations for aiobotocore.ElasticBeanstalk 2.5.2 service generated with mypy-boto3-builder 7.17.2
+Version: 2.5.4
+Summary: Type annotations for aiobotocore.ElasticBeanstalk 2.5.4 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elasticbeanstalk/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-elasticbeanstalk.svg?color=blue)](https://pypi.org/project/types-aiobotocore-elasticbeanstalk)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elasticbeanstalk/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-elasticbeanstalk)](https://pepy.tech/project/types-aiobotocore-elasticbeanstalk)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.ElasticBeanstalk 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticbeanstalk.html#ElasticBeanstalk)
+[aiobotocore.ElasticBeanstalk 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticbeanstalk.html#ElasticBeanstalk)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-elasticbeanstalk-2.5.2.post3/README.md` & `types-aiobotocore-elasticbeanstalk-2.5.4/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-elasticbeanstalk.svg?color=blue)](https://pypi.org/project/types-aiobotocore-elasticbeanstalk)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elasticbeanstalk/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-elasticbeanstalk)](https://pepy.tech/project/types-aiobotocore-elasticbeanstalk)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.ElasticBeanstalk 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticbeanstalk.html#ElasticBeanstalk)
+[aiobotocore.ElasticBeanstalk 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticbeanstalk.html#ElasticBeanstalk)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-elasticbeanstalk-2.5.2.post3/setup.py` & `types-aiobotocore-elasticbeanstalk-2.5.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-elasticbeanstalk",
-    version="2.5.2.post3",
+    version="2.5.4",
     packages=["types_aiobotocore_elasticbeanstalk"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.ElasticBeanstalk 2.5.2 service generated with"
+        "Type annotations for aiobotocore.ElasticBeanstalk 2.5.4 service generated with"
         " mypy-boto3-builder 7.17.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
```

### Comparing `types-aiobotocore-elasticbeanstalk-2.5.2.post3/types_aiobotocore_elasticbeanstalk/__init__.py` & `types-aiobotocore-elasticbeanstalk-2.5.4/types_aiobotocore_elasticbeanstalk/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-elasticbeanstalk-2.5.2.post3/types_aiobotocore_elasticbeanstalk/__init__.pyi` & `types-aiobotocore-elasticbeanstalk-2.5.4/types_aiobotocore_elasticbeanstalk/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-elasticbeanstalk-2.5.2.post3/types_aiobotocore_elasticbeanstalk/__main__.py` & `types-aiobotocore-elasticbeanstalk-2.5.4/types_aiobotocore_elasticbeanstalk/__main__.py`

 * *Files 18% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.ElasticBeanstalk 2.5.2\nVersion:        "
-        " 2.5.2.post3\nBuilder version: 7.17.2\nDocs:           "
+        "Type annotations for aiobotocore.ElasticBeanstalk 2.5.4\nVersion:         2.5.4\nBuilder"
+        " version: 7.17.2\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elasticbeanstalk//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticbeanstalk.html#ElasticBeanstalk\nOther"
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

### Comparing `types-aiobotocore-elasticbeanstalk-2.5.2.post3/types_aiobotocore_elasticbeanstalk/client.py` & `types-aiobotocore-elasticbeanstalk-2.5.4/types_aiobotocore_elasticbeanstalk/client.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-elasticbeanstalk-2.5.2.post3/types_aiobotocore_elasticbeanstalk/client.pyi` & `types-aiobotocore-elasticbeanstalk-2.5.4/types_aiobotocore_elasticbeanstalk/client.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-elasticbeanstalk-2.5.2.post3/types_aiobotocore_elasticbeanstalk/literals.py` & `types-aiobotocore-elasticbeanstalk-2.5.4/types_aiobotocore_elasticbeanstalk/literals.py`

 * *Files 0% similar despite different names*

```diff
@@ -139,14 +139,15 @@
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
@@ -242,14 +243,15 @@
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
@@ -328,26 +330,28 @@
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
@@ -512,14 +516,15 @@
     "ca-central-1",
     "eu-central-1",
     "eu-north-1",
     "eu-south-1",
     "eu-west-1",
     "eu-west-2",
     "eu-west-3",
+    "il-central-1",
     "me-south-1",
     "sa-east-1",
     "us-east-1",
     "us-east-2",
     "us-west-1",
     "us-west-2",
 ]
```

### Comparing `types-aiobotocore-elasticbeanstalk-2.5.2.post3/types_aiobotocore_elasticbeanstalk/literals.pyi` & `types-aiobotocore-elasticbeanstalk-2.5.4/types_aiobotocore_elasticbeanstalk/literals.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -137,14 +137,15 @@
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
@@ -240,14 +241,15 @@
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
@@ -326,26 +328,28 @@
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
@@ -510,14 +514,15 @@
     "ca-central-1",
     "eu-central-1",
     "eu-north-1",
     "eu-south-1",
     "eu-west-1",
     "eu-west-2",
     "eu-west-3",
+    "il-central-1",
     "me-south-1",
     "sa-east-1",
     "us-east-1",
     "us-east-2",
     "us-west-1",
     "us-west-2",
 ]
```

### Comparing `types-aiobotocore-elasticbeanstalk-2.5.2.post3/types_aiobotocore_elasticbeanstalk/paginator.py` & `types-aiobotocore-elasticbeanstalk-2.5.4/types_aiobotocore_elasticbeanstalk/paginator.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-elasticbeanstalk-2.5.2.post3/types_aiobotocore_elasticbeanstalk/paginator.pyi` & `types-aiobotocore-elasticbeanstalk-2.5.4/types_aiobotocore_elasticbeanstalk/paginator.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-elasticbeanstalk-2.5.2.post3/types_aiobotocore_elasticbeanstalk/type_defs.py` & `types-aiobotocore-elasticbeanstalk-2.5.4/types_aiobotocore_elasticbeanstalk/type_defs.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-elasticbeanstalk-2.5.2.post3/types_aiobotocore_elasticbeanstalk/type_defs.pyi` & `types-aiobotocore-elasticbeanstalk-2.5.4/types_aiobotocore_elasticbeanstalk/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-elasticbeanstalk-2.5.2.post3/types_aiobotocore_elasticbeanstalk/waiter.py` & `types-aiobotocore-elasticbeanstalk-2.5.4/types_aiobotocore_elasticbeanstalk/waiter.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-elasticbeanstalk-2.5.2.post3/types_aiobotocore_elasticbeanstalk/waiter.pyi` & `types-aiobotocore-elasticbeanstalk-2.5.4/types_aiobotocore_elasticbeanstalk/waiter.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-elasticbeanstalk-2.5.2.post3/types_aiobotocore_elasticbeanstalk.egg-info/PKG-INFO` & `types-aiobotocore-elasticbeanstalk-2.5.4/types_aiobotocore_elasticbeanstalk.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-elasticbeanstalk
-Version: 2.5.2.post3
-Summary: Type annotations for aiobotocore.ElasticBeanstalk 2.5.2 service generated with mypy-boto3-builder 7.17.2
+Version: 2.5.4
+Summary: Type annotations for aiobotocore.ElasticBeanstalk 2.5.4 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elasticbeanstalk/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-elasticbeanstalk.svg?color=blue)](https://pypi.org/project/types-aiobotocore-elasticbeanstalk)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elasticbeanstalk/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-elasticbeanstalk)](https://pepy.tech/project/types-aiobotocore-elasticbeanstalk)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.ElasticBeanstalk 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticbeanstalk.html#ElasticBeanstalk)
+[aiobotocore.ElasticBeanstalk 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticbeanstalk.html#ElasticBeanstalk)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-elasticbeanstalk-2.5.2.post3/types_aiobotocore_elasticbeanstalk.egg-info/SOURCES.txt` & `types-aiobotocore-elasticbeanstalk-2.5.4/types_aiobotocore_elasticbeanstalk.egg-info/SOURCES.txt`

 * *Files identical despite different names*


# Comparing `tmp/types-aiobotocore-ec2-instance-connect-2.5.2.post3.tar.gz` & `tmp/types-aiobotocore-ec2-instance-connect-2.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-ec2-instance-connect-2.5.2.post3.tar", last modified: Fri Aug  4 12:37:39 2023, max compression
+gzip compressed data, was "types-aiobotocore-ec2-instance-connect-2.5.4.tar", last modified: Tue Aug  8 01:23:38 2023, max compression
```

## Comparing `types-aiobotocore-ec2-instance-connect-2.5.2.post3.tar` & `types-aiobotocore-ec2-instance-connect-2.5.4.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:37:39.099703 types-aiobotocore-ec2-instance-connect-2.5.2.post3/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-04 12:22:52.000000 types-aiobotocore-ec2-instance-connect-2.5.2.post3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    12885 2023-08-04 12:37:39.099703 types-aiobotocore-ec2-instance-connect-2.5.2.post3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    11317 2023-08-04 12:22:52.000000 types-aiobotocore-ec2-instance-connect-2.5.2.post3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-04 12:37:39.099703 types-aiobotocore-ec2-instance-connect-2.5.2.post3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2153 2023-08-04 12:22:52.000000 types-aiobotocore-ec2-instance-connect-2.5.2.post3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:37:39.099703 types-aiobotocore-ec2-instance-connect-2.5.2.post3/types_aiobotocore_ec2_instance_connect/
--rw-r--r--   0 runner    (1001) docker     (123)      536 2023-08-04 12:22:52.000000 types-aiobotocore-ec2-instance-connect-2.5.2.post3/types_aiobotocore_ec2_instance_connect/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      535 2023-08-04 12:22:52.000000 types-aiobotocore-ec2-instance-connect-2.5.2.post3/types_aiobotocore_ec2_instance_connect/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      991 2023-08-04 12:22:52.000000 types-aiobotocore-ec2-instance-connect-2.5.2.post3/types_aiobotocore_ec2_instance_connect/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6245 2023-08-04 12:22:52.000000 types-aiobotocore-ec2-instance-connect-2.5.2.post3/types_aiobotocore_ec2_instance_connect/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     6235 2023-08-04 12:22:52.000000 types-aiobotocore-ec2-instance-connect-2.5.2.post3/types_aiobotocore_ec2_instance_connect/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     7614 2023-08-04 12:22:53.000000 types-aiobotocore-ec2-instance-connect-2.5.2.post3/types_aiobotocore_ec2_instance_connect/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     7612 2023-08-04 12:22:52.000000 types-aiobotocore-ec2-instance-connect-2.5.2.post3/types_aiobotocore_ec2_instance_connect/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 12:22:52.000000 types-aiobotocore-ec2-instance-connect-2.5.2.post3/types_aiobotocore_ec2_instance_connect/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     2587 2023-08-04 12:22:53.000000 types-aiobotocore-ec2-instance-connect-2.5.2.post3/types_aiobotocore_ec2_instance_connect/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)     2582 2023-08-04 12:22:53.000000 types-aiobotocore-ec2-instance-connect-2.5.2.post3/types_aiobotocore_ec2_instance_connect/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-04 12:22:52.000000 types-aiobotocore-ec2-instance-connect-2.5.2.post3/types_aiobotocore_ec2_instance_connect/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:37:39.099703 types-aiobotocore-ec2-instance-connect-2.5.2.post3/types_aiobotocore_ec2_instance_connect.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    12885 2023-08-04 12:37:38.000000 types-aiobotocore-ec2-instance-connect-2.5.2.post3/types_aiobotocore_ec2_instance_connect.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      955 2023-08-04 12:37:38.000000 types-aiobotocore-ec2-instance-connect-2.5.2.post3/types_aiobotocore_ec2_instance_connect.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 12:37:38.000000 types-aiobotocore-ec2-instance-connect-2.5.2.post3/types_aiobotocore_ec2_instance_connect.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 12:37:38.000000 types-aiobotocore-ec2-instance-connect-2.5.2.post3/types_aiobotocore_ec2_instance_connect.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-04 12:37:38.000000 types-aiobotocore-ec2-instance-connect-2.5.2.post3/types_aiobotocore_ec2_instance_connect.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-08-04 12:37:38.000000 types-aiobotocore-ec2-instance-connect-2.5.2.post3/types_aiobotocore_ec2_instance_connect.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:23:38.654695 types-aiobotocore-ec2-instance-connect-2.5.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-08 01:10:20.000000 types-aiobotocore-ec2-instance-connect-2.5.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    12879 2023-08-08 01:23:38.654695 types-aiobotocore-ec2-instance-connect-2.5.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    11317 2023-08-08 01:10:20.000000 types-aiobotocore-ec2-instance-connect-2.5.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-08 01:23:38.654695 types-aiobotocore-ec2-instance-connect-2.5.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2147 2023-08-08 01:10:20.000000 types-aiobotocore-ec2-instance-connect-2.5.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:23:38.646695 types-aiobotocore-ec2-instance-connect-2.5.4/types_aiobotocore_ec2_instance_connect/
+-rw-r--r--   0 runner    (1001) docker     (123)      536 2023-08-08 01:10:20.000000 types-aiobotocore-ec2-instance-connect-2.5.4/types_aiobotocore_ec2_instance_connect/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      535 2023-08-08 01:10:20.000000 types-aiobotocore-ec2-instance-connect-2.5.4/types_aiobotocore_ec2_instance_connect/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      979 2023-08-08 01:10:20.000000 types-aiobotocore-ec2-instance-connect-2.5.4/types_aiobotocore_ec2_instance_connect/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6245 2023-08-08 01:10:20.000000 types-aiobotocore-ec2-instance-connect-2.5.4/types_aiobotocore_ec2_instance_connect/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6235 2023-08-08 01:10:20.000000 types-aiobotocore-ec2-instance-connect-2.5.4/types_aiobotocore_ec2_instance_connect/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     7709 2023-08-08 01:10:20.000000 types-aiobotocore-ec2-instance-connect-2.5.4/types_aiobotocore_ec2_instance_connect/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7707 2023-08-08 01:10:20.000000 types-aiobotocore-ec2-instance-connect-2.5.4/types_aiobotocore_ec2_instance_connect/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 01:10:20.000000 types-aiobotocore-ec2-instance-connect-2.5.4/types_aiobotocore_ec2_instance_connect/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     2587 2023-08-08 01:10:20.000000 types-aiobotocore-ec2-instance-connect-2.5.4/types_aiobotocore_ec2_instance_connect/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2582 2023-08-08 01:10:20.000000 types-aiobotocore-ec2-instance-connect-2.5.4/types_aiobotocore_ec2_instance_connect/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-08-08 01:10:20.000000 types-aiobotocore-ec2-instance-connect-2.5.4/types_aiobotocore_ec2_instance_connect/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:23:38.654695 types-aiobotocore-ec2-instance-connect-2.5.4/types_aiobotocore_ec2_instance_connect.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    12879 2023-08-08 01:23:38.000000 types-aiobotocore-ec2-instance-connect-2.5.4/types_aiobotocore_ec2_instance_connect.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      955 2023-08-08 01:23:38.000000 types-aiobotocore-ec2-instance-connect-2.5.4/types_aiobotocore_ec2_instance_connect.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 01:23:38.000000 types-aiobotocore-ec2-instance-connect-2.5.4/types_aiobotocore_ec2_instance_connect.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 01:23:38.000000 types-aiobotocore-ec2-instance-connect-2.5.4/types_aiobotocore_ec2_instance_connect.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-08 01:23:38.000000 types-aiobotocore-ec2-instance-connect-2.5.4/types_aiobotocore_ec2_instance_connect.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-08-08 01:23:38.000000 types-aiobotocore-ec2-instance-connect-2.5.4/types_aiobotocore_ec2_instance_connect.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-ec2-instance-connect-2.5.2.post3/LICENSE` & `types-aiobotocore-ec2-instance-connect-2.5.4/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-ec2-instance-connect-2.5.2.post3/PKG-INFO` & `types-aiobotocore-ec2-instance-connect-2.5.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-ec2-instance-connect
-Version: 2.5.2.post3
-Summary: Type annotations for aiobotocore.EC2InstanceConnect 2.5.2 service generated with mypy-boto3-builder 7.17.2
+Version: 2.5.4
+Summary: Type annotations for aiobotocore.EC2InstanceConnect 2.5.4 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ec2_instance_connect/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-ec2-instance-connect.svg?color=blue)](https://pypi.org/project/types-aiobotocore-ec2-instance-connect)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ec2_instance_connect/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-ec2-instance-connect)](https://pepy.tech/project/types-aiobotocore-ec2-instance-connect)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.EC2InstanceConnect 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2-instance-connect.html#EC2InstanceConnect)
+[aiobotocore.EC2InstanceConnect 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2-instance-connect.html#EC2InstanceConnect)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-ec2-instance-connect-2.5.2.post3/README.md` & `types-aiobotocore-ec2-instance-connect-2.5.4/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-ec2-instance-connect.svg?color=blue)](https://pypi.org/project/types-aiobotocore-ec2-instance-connect)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ec2_instance_connect/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-ec2-instance-connect)](https://pepy.tech/project/types-aiobotocore-ec2-instance-connect)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.EC2InstanceConnect 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2-instance-connect.html#EC2InstanceConnect)
+[aiobotocore.EC2InstanceConnect 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2-instance-connect.html#EC2InstanceConnect)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-ec2-instance-connect-2.5.2.post3/setup.py` & `types-aiobotocore-ec2-instance-connect-2.5.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-ec2-instance-connect",
-    version="2.5.2.post3",
+    version="2.5.4",
     packages=["types_aiobotocore_ec2_instance_connect"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.EC2InstanceConnect 2.5.2 service generated with"
+        "Type annotations for aiobotocore.EC2InstanceConnect 2.5.4 service generated with"
         " mypy-boto3-builder 7.17.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
```

### Comparing `types-aiobotocore-ec2-instance-connect-2.5.2.post3/types_aiobotocore_ec2_instance_connect/__init__.py` & `types-aiobotocore-ec2-instance-connect-2.5.4/types_aiobotocore_ec2_instance_connect/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-ec2-instance-connect-2.5.2.post3/types_aiobotocore_ec2_instance_connect/__init__.pyi` & `types-aiobotocore-ec2-instance-connect-2.5.4/types_aiobotocore_ec2_instance_connect/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-ec2-instance-connect-2.5.2.post3/types_aiobotocore_ec2_instance_connect/client.py` & `types-aiobotocore-ec2-instance-connect-2.5.4/types_aiobotocore_ec2_instance_connect/client.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-ec2-instance-connect-2.5.2.post3/types_aiobotocore_ec2_instance_connect/client.pyi` & `types-aiobotocore-ec2-instance-connect-2.5.4/types_aiobotocore_ec2_instance_connect/client.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-ec2-instance-connect-2.5.2.post3/types_aiobotocore_ec2_instance_connect/literals.py` & `types-aiobotocore-ec2-instance-connect-2.5.4/types_aiobotocore_ec2_instance_connect/literals.py`

 * *Files 1% similar despite different names*

```diff
@@ -34,14 +34,15 @@
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
@@ -137,14 +138,15 @@
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
@@ -223,26 +225,28 @@
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

### Comparing `types-aiobotocore-ec2-instance-connect-2.5.2.post3/types_aiobotocore_ec2_instance_connect/literals.pyi` & `types-aiobotocore-ec2-instance-connect-2.5.4/types_aiobotocore_ec2_instance_connect/literals.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -32,14 +32,15 @@
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
@@ -135,14 +136,15 @@
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
@@ -221,26 +223,28 @@
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

### Comparing `types-aiobotocore-ec2-instance-connect-2.5.2.post3/types_aiobotocore_ec2_instance_connect/type_defs.py` & `types-aiobotocore-ec2-instance-connect-2.5.4/types_aiobotocore_ec2_instance_connect/type_defs.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-ec2-instance-connect-2.5.2.post3/types_aiobotocore_ec2_instance_connect/type_defs.pyi` & `types-aiobotocore-ec2-instance-connect-2.5.4/types_aiobotocore_ec2_instance_connect/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-ec2-instance-connect-2.5.2.post3/types_aiobotocore_ec2_instance_connect.egg-info/PKG-INFO` & `types-aiobotocore-ec2-instance-connect-2.5.4/types_aiobotocore_ec2_instance_connect.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-ec2-instance-connect
-Version: 2.5.2.post3
-Summary: Type annotations for aiobotocore.EC2InstanceConnect 2.5.2 service generated with mypy-boto3-builder 7.17.2
+Version: 2.5.4
+Summary: Type annotations for aiobotocore.EC2InstanceConnect 2.5.4 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ec2_instance_connect/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-ec2-instance-connect.svg?color=blue)](https://pypi.org/project/types-aiobotocore-ec2-instance-connect)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ec2_instance_connect/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-ec2-instance-connect)](https://pepy.tech/project/types-aiobotocore-ec2-instance-connect)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.EC2InstanceConnect 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2-instance-connect.html#EC2InstanceConnect)
+[aiobotocore.EC2InstanceConnect 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2-instance-connect.html#EC2InstanceConnect)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-ec2-instance-connect-2.5.2.post3/types_aiobotocore_ec2_instance_connect.egg-info/SOURCES.txt` & `types-aiobotocore-ec2-instance-connect-2.5.4/types_aiobotocore_ec2_instance_connect.egg-info/SOURCES.txt`

 * *Files identical despite different names*


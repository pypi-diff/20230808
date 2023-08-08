# Comparing `tmp/types-aiobotocore-fis-2.5.2.post3.tar.gz` & `tmp/types-aiobotocore-fis-2.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-fis-2.5.2.post3.tar", last modified: Fri Aug  4 12:37:44 2023, max compression
+gzip compressed data, was "types-aiobotocore-fis-2.5.4.tar", last modified: Tue Aug  8 01:23:44 2023, max compression
```

## Comparing `types-aiobotocore-fis-2.5.2.post3.tar` & `types-aiobotocore-fis-2.5.4.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:37:44.287824 types-aiobotocore-fis-2.5.2.post3/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-04 12:23:49.000000 types-aiobotocore-fis-2.5.2.post3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    11992 2023-08-04 12:37:44.283825 types-aiobotocore-fis-2.5.2.post3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    10490 2023-08-04 12:23:49.000000 types-aiobotocore-fis-2.5.2.post3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-04 12:37:44.287824 types-aiobotocore-fis-2.5.2.post3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2020 2023-08-04 12:23:48.000000 types-aiobotocore-fis-2.5.2.post3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:37:44.283825 types-aiobotocore-fis-2.5.2.post3/types_aiobotocore_fis/
--rw-r--r--   0 runner    (1001) docker     (123)      410 2023-08-04 12:23:49.000000 types-aiobotocore-fis-2.5.2.post3/types_aiobotocore_fis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      409 2023-08-04 12:23:49.000000 types-aiobotocore-fis-2.5.2.post3/types_aiobotocore_fis/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      916 2023-08-04 12:23:49.000000 types-aiobotocore-fis-2.5.2.post3/types_aiobotocore_fis/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13614 2023-08-04 12:23:49.000000 types-aiobotocore-fis-2.5.2.post3/types_aiobotocore_fis/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    13590 2023-08-04 12:23:49.000000 types-aiobotocore-fis-2.5.2.post3/types_aiobotocore_fis/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     7833 2023-08-04 12:23:49.000000 types-aiobotocore-fis-2.5.2.post3/types_aiobotocore_fis/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     7831 2023-08-04 12:23:49.000000 types-aiobotocore-fis-2.5.2.post3/types_aiobotocore_fis/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 12:23:49.000000 types-aiobotocore-fis-2.5.2.post3/types_aiobotocore_fis/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    23889 2023-08-04 12:23:49.000000 types-aiobotocore-fis-2.5.2.post3/types_aiobotocore_fis/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    23866 2023-08-04 12:23:49.000000 types-aiobotocore-fis-2.5.2.post3/types_aiobotocore_fis/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-04 12:23:49.000000 types-aiobotocore-fis-2.5.2.post3/types_aiobotocore_fis/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:37:44.283825 types-aiobotocore-fis-2.5.2.post3/types_aiobotocore_fis.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    11992 2023-08-04 12:37:44.000000 types-aiobotocore-fis-2.5.2.post3/types_aiobotocore_fis.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      666 2023-08-04 12:37:44.000000 types-aiobotocore-fis-2.5.2.post3/types_aiobotocore_fis.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 12:37:44.000000 types-aiobotocore-fis-2.5.2.post3/types_aiobotocore_fis.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 12:37:44.000000 types-aiobotocore-fis-2.5.2.post3/types_aiobotocore_fis.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-04 12:37:44.000000 types-aiobotocore-fis-2.5.2.post3/types_aiobotocore_fis.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-08-04 12:37:44.000000 types-aiobotocore-fis-2.5.2.post3/types_aiobotocore_fis.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:23:44.778718 types-aiobotocore-fis-2.5.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-08 01:11:14.000000 types-aiobotocore-fis-2.5.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    11986 2023-08-08 01:23:44.778718 types-aiobotocore-fis-2.5.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10490 2023-08-08 01:11:14.000000 types-aiobotocore-fis-2.5.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-08 01:23:44.778718 types-aiobotocore-fis-2.5.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2014 2023-08-08 01:11:14.000000 types-aiobotocore-fis-2.5.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:23:44.774718 types-aiobotocore-fis-2.5.4/types_aiobotocore_fis/
+-rw-r--r--   0 runner    (1001) docker     (123)      410 2023-08-08 01:11:14.000000 types-aiobotocore-fis-2.5.4/types_aiobotocore_fis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      409 2023-08-08 01:11:14.000000 types-aiobotocore-fis-2.5.4/types_aiobotocore_fis/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      904 2023-08-08 01:11:14.000000 types-aiobotocore-fis-2.5.4/types_aiobotocore_fis/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13614 2023-08-08 01:11:14.000000 types-aiobotocore-fis-2.5.4/types_aiobotocore_fis/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13590 2023-08-08 01:11:14.000000 types-aiobotocore-fis-2.5.4/types_aiobotocore_fis/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     7928 2023-08-08 01:11:14.000000 types-aiobotocore-fis-2.5.4/types_aiobotocore_fis/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7926 2023-08-08 01:11:14.000000 types-aiobotocore-fis-2.5.4/types_aiobotocore_fis/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 01:11:14.000000 types-aiobotocore-fis-2.5.4/types_aiobotocore_fis/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    23889 2023-08-08 01:11:14.000000 types-aiobotocore-fis-2.5.4/types_aiobotocore_fis/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23866 2023-08-08 01:11:14.000000 types-aiobotocore-fis-2.5.4/types_aiobotocore_fis/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-08-08 01:11:14.000000 types-aiobotocore-fis-2.5.4/types_aiobotocore_fis/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:23:44.778718 types-aiobotocore-fis-2.5.4/types_aiobotocore_fis.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    11986 2023-08-08 01:23:44.000000 types-aiobotocore-fis-2.5.4/types_aiobotocore_fis.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      666 2023-08-08 01:23:44.000000 types-aiobotocore-fis-2.5.4/types_aiobotocore_fis.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 01:23:44.000000 types-aiobotocore-fis-2.5.4/types_aiobotocore_fis.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 01:23:44.000000 types-aiobotocore-fis-2.5.4/types_aiobotocore_fis.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-08 01:23:44.000000 types-aiobotocore-fis-2.5.4/types_aiobotocore_fis.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-08-08 01:23:44.000000 types-aiobotocore-fis-2.5.4/types_aiobotocore_fis.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-fis-2.5.2.post3/LICENSE` & `types-aiobotocore-fis-2.5.4/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-fis-2.5.2.post3/PKG-INFO` & `types-aiobotocore-fis-2.5.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-fis
-Version: 2.5.2.post3
-Summary: Type annotations for aiobotocore.FIS 2.5.2 service generated with mypy-boto3-builder 7.17.2
+Version: 2.5.4
+Summary: Type annotations for aiobotocore.FIS 2.5.4 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_fis/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-fis.svg?color=blue)](https://pypi.org/project/types-aiobotocore-fis)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_fis/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-fis)](https://pepy.tech/project/types-aiobotocore-fis)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.FIS 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fis.html#FIS)
+[aiobotocore.FIS 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fis.html#FIS)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-fis-2.5.2.post3/README.md` & `types-aiobotocore-fis-2.5.4/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-fis.svg?color=blue)](https://pypi.org/project/types-aiobotocore-fis)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_fis/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-fis)](https://pepy.tech/project/types-aiobotocore-fis)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.FIS 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fis.html#FIS)
+[aiobotocore.FIS 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fis.html#FIS)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-fis-2.5.2.post3/setup.py` & `types-aiobotocore-fis-2.5.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-fis",
-    version="2.5.2.post3",
+    version="2.5.4",
     packages=["types_aiobotocore_fis"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.FIS 2.5.2 service generated with mypy-boto3-builder"
+        "Type annotations for aiobotocore.FIS 2.5.4 service generated with mypy-boto3-builder"
         " 7.17.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
```

### Comparing `types-aiobotocore-fis-2.5.2.post3/types_aiobotocore_fis/client.py` & `types-aiobotocore-fis-2.5.4/types_aiobotocore_fis/client.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-fis-2.5.2.post3/types_aiobotocore_fis/client.pyi` & `types-aiobotocore-fis-2.5.4/types_aiobotocore_fis/client.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-fis-2.5.2.post3/types_aiobotocore_fis/literals.py` & `types-aiobotocore-fis-2.5.4/types_aiobotocore_fis/literals.py`

 * *Files 2% similar despite different names*

```diff
@@ -46,14 +46,15 @@
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
@@ -149,14 +150,15 @@
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
@@ -235,26 +237,28 @@
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

### Comparing `types-aiobotocore-fis-2.5.2.post3/types_aiobotocore_fis/literals.pyi` & `types-aiobotocore-fis-2.5.4/types_aiobotocore_fis/literals.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -44,14 +44,15 @@
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
@@ -147,14 +148,15 @@
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
@@ -233,26 +235,28 @@
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

### Comparing `types-aiobotocore-fis-2.5.2.post3/types_aiobotocore_fis/type_defs.py` & `types-aiobotocore-fis-2.5.4/types_aiobotocore_fis/type_defs.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-fis-2.5.2.post3/types_aiobotocore_fis/type_defs.pyi` & `types-aiobotocore-fis-2.5.4/types_aiobotocore_fis/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-fis-2.5.2.post3/types_aiobotocore_fis.egg-info/PKG-INFO` & `types-aiobotocore-fis-2.5.4/types_aiobotocore_fis.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-fis
-Version: 2.5.2.post3
-Summary: Type annotations for aiobotocore.FIS 2.5.2 service generated with mypy-boto3-builder 7.17.2
+Version: 2.5.4
+Summary: Type annotations for aiobotocore.FIS 2.5.4 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_fis/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-fis.svg?color=blue)](https://pypi.org/project/types-aiobotocore-fis)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_fis/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-fis)](https://pepy.tech/project/types-aiobotocore-fis)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.FIS 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fis.html#FIS)
+[aiobotocore.FIS 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fis.html#FIS)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-fis-2.5.2.post3/types_aiobotocore_fis.egg-info/SOURCES.txt` & `types-aiobotocore-fis-2.5.4/types_aiobotocore_fis.egg-info/SOURCES.txt`

 * *Files identical despite different names*


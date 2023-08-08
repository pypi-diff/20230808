# Comparing `tmp/types-aiobotocore-comprehendmedical-2.5.2.post3.tar.gz` & `tmp/types-aiobotocore-comprehendmedical-2.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-comprehendmedical-2.5.2.post3.tar", last modified: Fri Aug  4 12:37:31 2023, max compression
+gzip compressed data, was "types-aiobotocore-comprehendmedical-2.5.4.tar", last modified: Tue Aug  8 01:23:31 2023, max compression
```

## Comparing `types-aiobotocore-comprehendmedical-2.5.2.post3.tar` & `types-aiobotocore-comprehendmedical-2.5.4.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:37:31.423519 types-aiobotocore-comprehendmedical-2.5.2.post3/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-04 12:20:37.000000 types-aiobotocore-comprehendmedical-2.5.2.post3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    12698 2023-08-04 12:37:31.419519 types-aiobotocore-comprehendmedical-2.5.2.post3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    11140 2023-08-04 12:20:37.000000 types-aiobotocore-comprehendmedical-2.5.2.post3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-04 12:37:31.423519 types-aiobotocore-comprehendmedical-2.5.2.post3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2142 2023-08-04 12:20:37.000000 types-aiobotocore-comprehendmedical-2.5.2.post3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:37:31.415519 types-aiobotocore-comprehendmedical-2.5.2.post3/types_aiobotocore_comprehendmedical/
--rw-r--r--   0 runner    (1001) docker     (123)      522 2023-08-04 12:20:37.000000 types-aiobotocore-comprehendmedical-2.5.2.post3/types_aiobotocore_comprehendmedical/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      521 2023-08-04 12:20:37.000000 types-aiobotocore-comprehendmedical-2.5.2.post3/types_aiobotocore_comprehendmedical/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      983 2023-08-04 12:20:37.000000 types-aiobotocore-comprehendmedical-2.5.2.post3/types_aiobotocore_comprehendmedical/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    23289 2023-08-04 12:20:37.000000 types-aiobotocore-comprehendmedical-2.5.2.post3/types_aiobotocore_comprehendmedical/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    23254 2023-08-04 12:20:37.000000 types-aiobotocore-comprehendmedical-2.5.2.post3/types_aiobotocore_comprehendmedical/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    11640 2023-08-04 12:20:38.000000 types-aiobotocore-comprehendmedical-2.5.2.post3/types_aiobotocore_comprehendmedical/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    11638 2023-08-04 12:20:37.000000 types-aiobotocore-comprehendmedical-2.5.2.post3/types_aiobotocore_comprehendmedical/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 12:20:37.000000 types-aiobotocore-comprehendmedical-2.5.2.post3/types_aiobotocore_comprehendmedical/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    24964 2023-08-04 12:20:38.000000 types-aiobotocore-comprehendmedical-2.5.2.post3/types_aiobotocore_comprehendmedical/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    24949 2023-08-04 12:20:38.000000 types-aiobotocore-comprehendmedical-2.5.2.post3/types_aiobotocore_comprehendmedical/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-04 12:20:37.000000 types-aiobotocore-comprehendmedical-2.5.2.post3/types_aiobotocore_comprehendmedical/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:37:31.419519 types-aiobotocore-comprehendmedical-2.5.2.post3/types_aiobotocore_comprehendmedical.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    12698 2023-08-04 12:37:31.000000 types-aiobotocore-comprehendmedical-2.5.2.post3/types_aiobotocore_comprehendmedical.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      904 2023-08-04 12:37:31.000000 types-aiobotocore-comprehendmedical-2.5.2.post3/types_aiobotocore_comprehendmedical.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 12:37:31.000000 types-aiobotocore-comprehendmedical-2.5.2.post3/types_aiobotocore_comprehendmedical.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 12:37:31.000000 types-aiobotocore-comprehendmedical-2.5.2.post3/types_aiobotocore_comprehendmedical.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-04 12:37:31.000000 types-aiobotocore-comprehendmedical-2.5.2.post3/types_aiobotocore_comprehendmedical.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-08-04 12:37:31.000000 types-aiobotocore-comprehendmedical-2.5.2.post3/types_aiobotocore_comprehendmedical.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:23:31.350669 types-aiobotocore-comprehendmedical-2.5.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-08 01:08:15.000000 types-aiobotocore-comprehendmedical-2.5.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    12692 2023-08-08 01:23:31.350669 types-aiobotocore-comprehendmedical-2.5.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    11140 2023-08-08 01:08:15.000000 types-aiobotocore-comprehendmedical-2.5.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-08 01:23:31.350669 types-aiobotocore-comprehendmedical-2.5.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2136 2023-08-08 01:08:15.000000 types-aiobotocore-comprehendmedical-2.5.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:23:31.346669 types-aiobotocore-comprehendmedical-2.5.4/types_aiobotocore_comprehendmedical/
+-rw-r--r--   0 runner    (1001) docker     (123)      522 2023-08-08 01:08:15.000000 types-aiobotocore-comprehendmedical-2.5.4/types_aiobotocore_comprehendmedical/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      521 2023-08-08 01:08:15.000000 types-aiobotocore-comprehendmedical-2.5.4/types_aiobotocore_comprehendmedical/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      971 2023-08-08 01:08:15.000000 types-aiobotocore-comprehendmedical-2.5.4/types_aiobotocore_comprehendmedical/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23284 2023-08-08 01:08:15.000000 types-aiobotocore-comprehendmedical-2.5.4/types_aiobotocore_comprehendmedical/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23249 2023-08-08 01:08:15.000000 types-aiobotocore-comprehendmedical-2.5.4/types_aiobotocore_comprehendmedical/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    11735 2023-08-08 01:08:16.000000 types-aiobotocore-comprehendmedical-2.5.4/types_aiobotocore_comprehendmedical/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11733 2023-08-08 01:08:16.000000 types-aiobotocore-comprehendmedical-2.5.4/types_aiobotocore_comprehendmedical/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 01:08:15.000000 types-aiobotocore-comprehendmedical-2.5.4/types_aiobotocore_comprehendmedical/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    24964 2023-08-08 01:08:17.000000 types-aiobotocore-comprehendmedical-2.5.4/types_aiobotocore_comprehendmedical/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24949 2023-08-08 01:08:16.000000 types-aiobotocore-comprehendmedical-2.5.4/types_aiobotocore_comprehendmedical/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-08-08 01:08:15.000000 types-aiobotocore-comprehendmedical-2.5.4/types_aiobotocore_comprehendmedical/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:23:31.350669 types-aiobotocore-comprehendmedical-2.5.4/types_aiobotocore_comprehendmedical.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    12692 2023-08-08 01:23:31.000000 types-aiobotocore-comprehendmedical-2.5.4/types_aiobotocore_comprehendmedical.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      904 2023-08-08 01:23:31.000000 types-aiobotocore-comprehendmedical-2.5.4/types_aiobotocore_comprehendmedical.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 01:23:31.000000 types-aiobotocore-comprehendmedical-2.5.4/types_aiobotocore_comprehendmedical.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 01:23:31.000000 types-aiobotocore-comprehendmedical-2.5.4/types_aiobotocore_comprehendmedical.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-08 01:23:31.000000 types-aiobotocore-comprehendmedical-2.5.4/types_aiobotocore_comprehendmedical.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-08-08 01:23:31.000000 types-aiobotocore-comprehendmedical-2.5.4/types_aiobotocore_comprehendmedical.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-comprehendmedical-2.5.2.post3/LICENSE` & `types-aiobotocore-comprehendmedical-2.5.4/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-comprehendmedical-2.5.2.post3/PKG-INFO` & `types-aiobotocore-comprehendmedical-2.5.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-comprehendmedical
-Version: 2.5.2.post3
-Summary: Type annotations for aiobotocore.ComprehendMedical 2.5.2 service generated with mypy-boto3-builder 7.17.2
+Version: 2.5.4
+Summary: Type annotations for aiobotocore.ComprehendMedical 2.5.4 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_comprehendmedical/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-comprehendmedical.svg?color=blue)](https://pypi.org/project/types-aiobotocore-comprehendmedical)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_comprehendmedical/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-comprehendmedical)](https://pepy.tech/project/types-aiobotocore-comprehendmedical)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.ComprehendMedical 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehendmedical.html#ComprehendMedical)
+[aiobotocore.ComprehendMedical 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehendmedical.html#ComprehendMedical)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-comprehendmedical-2.5.2.post3/README.md` & `types-aiobotocore-comprehendmedical-2.5.4/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-comprehendmedical.svg?color=blue)](https://pypi.org/project/types-aiobotocore-comprehendmedical)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_comprehendmedical/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-comprehendmedical)](https://pepy.tech/project/types-aiobotocore-comprehendmedical)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.ComprehendMedical 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehendmedical.html#ComprehendMedical)
+[aiobotocore.ComprehendMedical 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehendmedical.html#ComprehendMedical)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-comprehendmedical-2.5.2.post3/setup.py` & `types-aiobotocore-comprehendmedical-2.5.4/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-comprehendmedical",
-    version="2.5.2.post3",
+    version="2.5.4",
     packages=["types_aiobotocore_comprehendmedical"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.ComprehendMedical 2.5.2 service generated with"
+        "Type annotations for aiobotocore.ComprehendMedical 2.5.4 service generated with"
         " mypy-boto3-builder 7.17.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
```

### Comparing `types-aiobotocore-comprehendmedical-2.5.2.post3/types_aiobotocore_comprehendmedical/__init__.py` & `types-aiobotocore-comprehendmedical-2.5.4/types_aiobotocore_comprehendmedical/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-comprehendmedical-2.5.2.post3/types_aiobotocore_comprehendmedical/__init__.pyi` & `types-aiobotocore-comprehendmedical-2.5.4/types_aiobotocore_comprehendmedical/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-comprehendmedical-2.5.2.post3/types_aiobotocore_comprehendmedical/__main__.py` & `types-aiobotocore-comprehendmedical-2.5.4/types_aiobotocore_comprehendmedical/__main__.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.ComprehendMedical 2.5.2\nVersion:        "
-        " 2.5.2.post3\nBuilder version: 7.17.2\nDocs:           "
+        "Type annotations for aiobotocore.ComprehendMedical 2.5.4\nVersion:         2.5.4\nBuilder"
+        " version: 7.17.2\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_comprehendmedical//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehendmedical.html#ComprehendMedical\nOther"
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

### Comparing `types-aiobotocore-comprehendmedical-2.5.2.post3/types_aiobotocore_comprehendmedical/client.py` & `types-aiobotocore-comprehendmedical-2.5.4/types_aiobotocore_comprehendmedical/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -270,15 +270,15 @@
         self,
         *,
         Filter: ComprehendMedicalAsyncJobFilterTypeDef = ...,
         NextToken: str = ...,
         MaxResults: int = ...
     ) -> ListPHIDetectionJobsResponseTypeDef:
         """
-        Gets a list of protected health information (PHI) detection jobs that you have
+        Gets a list of protected health information (PHI) detection jobs you have
         submitted.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehendmedical.html#ComprehendMedical.Client.list_phi_detection_jobs)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_comprehendmedical/client/#list_phi_detection_jobs)
         """
 
     async def list_rx_norm_inference_jobs(
```

### Comparing `types-aiobotocore-comprehendmedical-2.5.2.post3/types_aiobotocore_comprehendmedical/client.pyi` & `types-aiobotocore-comprehendmedical-2.5.4/types_aiobotocore_comprehendmedical/client.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -249,15 +249,15 @@
         self,
         *,
         Filter: ComprehendMedicalAsyncJobFilterTypeDef = ...,
         NextToken: str = ...,
         MaxResults: int = ...
     ) -> ListPHIDetectionJobsResponseTypeDef:
         """
-        Gets a list of protected health information (PHI) detection jobs that you have
+        Gets a list of protected health information (PHI) detection jobs you have
         submitted.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehendmedical.html#ComprehendMedical.Client.list_phi_detection_jobs)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_comprehendmedical/client/#list_phi_detection_jobs)
         """
     async def list_rx_norm_inference_jobs(
         self,
```

### Comparing `types-aiobotocore-comprehendmedical-2.5.2.post3/types_aiobotocore_comprehendmedical/literals.py` & `types-aiobotocore-comprehendmedical-2.5.4/types_aiobotocore_comprehendmedical/literals.py`

 * *Files 2% similar despite different names*

```diff
@@ -206,14 +206,15 @@
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
@@ -309,14 +310,15 @@
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
@@ -395,26 +397,28 @@
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

### Comparing `types-aiobotocore-comprehendmedical-2.5.2.post3/types_aiobotocore_comprehendmedical/literals.pyi` & `types-aiobotocore-comprehendmedical-2.5.4/types_aiobotocore_comprehendmedical/literals.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -204,14 +204,15 @@
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
@@ -307,14 +308,15 @@
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
@@ -393,26 +395,28 @@
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

### Comparing `types-aiobotocore-comprehendmedical-2.5.2.post3/types_aiobotocore_comprehendmedical/type_defs.py` & `types-aiobotocore-comprehendmedical-2.5.4/types_aiobotocore_comprehendmedical/type_defs.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-comprehendmedical-2.5.2.post3/types_aiobotocore_comprehendmedical/type_defs.pyi` & `types-aiobotocore-comprehendmedical-2.5.4/types_aiobotocore_comprehendmedical/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-comprehendmedical-2.5.2.post3/types_aiobotocore_comprehendmedical.egg-info/PKG-INFO` & `types-aiobotocore-comprehendmedical-2.5.4/types_aiobotocore_comprehendmedical.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-comprehendmedical
-Version: 2.5.2.post3
-Summary: Type annotations for aiobotocore.ComprehendMedical 2.5.2 service generated with mypy-boto3-builder 7.17.2
+Version: 2.5.4
+Summary: Type annotations for aiobotocore.ComprehendMedical 2.5.4 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_comprehendmedical/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-comprehendmedical.svg?color=blue)](https://pypi.org/project/types-aiobotocore-comprehendmedical)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_comprehendmedical/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-comprehendmedical)](https://pepy.tech/project/types-aiobotocore-comprehendmedical)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.ComprehendMedical 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehendmedical.html#ComprehendMedical)
+[aiobotocore.ComprehendMedical 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehendmedical.html#ComprehendMedical)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-comprehendmedical-2.5.2.post3/types_aiobotocore_comprehendmedical.egg-info/SOURCES.txt` & `types-aiobotocore-comprehendmedical-2.5.4/types_aiobotocore_comprehendmedical.egg-info/SOURCES.txt`

 * *Files identical despite different names*


# Comparing `tmp/types-aiobotocore-cloudfront-2.5.2.post3.tar.gz` & `tmp/types-aiobotocore-cloudfront-2.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-cloudfront-2.5.2.post3.tar", last modified: Fri Aug  4 12:37:24 2023, max compression
+gzip compressed data, was "types-aiobotocore-cloudfront-2.5.4.tar", last modified: Tue Aug  8 01:23:26 2023, max compression
```

## Comparing `types-aiobotocore-cloudfront-2.5.2.post3.tar` & `types-aiobotocore-cloudfront-2.5.4.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:37:24.247341 types-aiobotocore-cloudfront-2.5.2.post3/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-04 12:19:43.000000 types-aiobotocore-cloudfront-2.5.2.post3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    14813 2023-08-04 12:37:24.247341 types-aiobotocore-cloudfront-2.5.2.post3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    13283 2023-08-04 12:19:43.000000 types-aiobotocore-cloudfront-2.5.2.post3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-04 12:37:24.247341 types-aiobotocore-cloudfront-2.5.2.post3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2093 2023-08-04 12:19:43.000000 types-aiobotocore-cloudfront-2.5.2.post3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:37:24.247341 types-aiobotocore-cloudfront-2.5.2.post3/types_aiobotocore_cloudfront/
--rw-r--r--   0 runner    (1001) docker     (123)     2226 2023-08-04 12:19:43.000000 types-aiobotocore-cloudfront-2.5.2.post3/types_aiobotocore_cloudfront/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2225 2023-08-04 12:19:43.000000 types-aiobotocore-cloudfront-2.5.2.post3/types_aiobotocore_cloudfront/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      955 2023-08-04 12:19:43.000000 types-aiobotocore-cloudfront-2.5.2.post3/types_aiobotocore_cloudfront/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    83071 2023-08-04 12:19:44.000000 types-aiobotocore-cloudfront-2.5.2.post3/types_aiobotocore_cloudfront/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    82949 2023-08-04 12:19:43.000000 types-aiobotocore-cloudfront-2.5.2.post3/types_aiobotocore_cloudfront/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    12472 2023-08-04 12:19:44.000000 types-aiobotocore-cloudfront-2.5.2.post3/types_aiobotocore_cloudfront/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    12470 2023-08-04 12:19:44.000000 types-aiobotocore-cloudfront-2.5.2.post3/types_aiobotocore_cloudfront/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     5760 2023-08-04 12:19:44.000000 types-aiobotocore-cloudfront-2.5.2.post3/types_aiobotocore_cloudfront/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     5754 2023-08-04 12:19:44.000000 types-aiobotocore-cloudfront-2.5.2.post3/types_aiobotocore_cloudfront/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 12:19:43.000000 types-aiobotocore-cloudfront-2.5.2.post3/types_aiobotocore_cloudfront/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)   138333 2023-08-04 12:19:48.000000 types-aiobotocore-cloudfront-2.5.2.post3/types_aiobotocore_cloudfront/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)   138070 2023-08-04 12:19:46.000000 types-aiobotocore-cloudfront-2.5.2.post3/types_aiobotocore_cloudfront/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-04 12:19:43.000000 types-aiobotocore-cloudfront-2.5.2.post3/types_aiobotocore_cloudfront/version.py
--rw-r--r--   0 runner    (1001) docker     (123)     3770 2023-08-04 12:19:44.000000 types-aiobotocore-cloudfront-2.5.2.post3/types_aiobotocore_cloudfront/waiter.py
--rw-r--r--   0 runner    (1001) docker     (123)     3767 2023-08-04 12:19:44.000000 types-aiobotocore-cloudfront-2.5.2.post3/types_aiobotocore_cloudfront/waiter.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:37:24.247341 types-aiobotocore-cloudfront-2.5.2.post3/types_aiobotocore_cloudfront.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    14813 2023-08-04 12:37:24.000000 types-aiobotocore-cloudfront-2.5.2.post3/types_aiobotocore_cloudfront.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      949 2023-08-04 12:37:24.000000 types-aiobotocore-cloudfront-2.5.2.post3/types_aiobotocore_cloudfront.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 12:37:24.000000 types-aiobotocore-cloudfront-2.5.2.post3/types_aiobotocore_cloudfront.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 12:37:24.000000 types-aiobotocore-cloudfront-2.5.2.post3/types_aiobotocore_cloudfront.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-04 12:37:24.000000 types-aiobotocore-cloudfront-2.5.2.post3/types_aiobotocore_cloudfront.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-08-04 12:37:24.000000 types-aiobotocore-cloudfront-2.5.2.post3/types_aiobotocore_cloudfront.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:23:26.346626 types-aiobotocore-cloudfront-2.5.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-08 01:07:25.000000 types-aiobotocore-cloudfront-2.5.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    14807 2023-08-08 01:23:26.346626 types-aiobotocore-cloudfront-2.5.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    13283 2023-08-08 01:07:25.000000 types-aiobotocore-cloudfront-2.5.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-08 01:23:26.346626 types-aiobotocore-cloudfront-2.5.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2087 2023-08-08 01:07:25.000000 types-aiobotocore-cloudfront-2.5.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:23:26.346626 types-aiobotocore-cloudfront-2.5.4/types_aiobotocore_cloudfront/
+-rw-r--r--   0 runner    (1001) docker     (123)     2226 2023-08-08 01:07:25.000000 types-aiobotocore-cloudfront-2.5.4/types_aiobotocore_cloudfront/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2225 2023-08-08 01:07:25.000000 types-aiobotocore-cloudfront-2.5.4/types_aiobotocore_cloudfront/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      943 2023-08-08 01:07:25.000000 types-aiobotocore-cloudfront-2.5.4/types_aiobotocore_cloudfront/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    83100 2023-08-08 01:07:26.000000 types-aiobotocore-cloudfront-2.5.4/types_aiobotocore_cloudfront/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    82978 2023-08-08 01:07:25.000000 types-aiobotocore-cloudfront-2.5.4/types_aiobotocore_cloudfront/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    12588 2023-08-08 01:07:26.000000 types-aiobotocore-cloudfront-2.5.4/types_aiobotocore_cloudfront/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12586 2023-08-08 01:07:26.000000 types-aiobotocore-cloudfront-2.5.4/types_aiobotocore_cloudfront/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     5760 2023-08-08 01:07:26.000000 types-aiobotocore-cloudfront-2.5.4/types_aiobotocore_cloudfront/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5754 2023-08-08 01:07:26.000000 types-aiobotocore-cloudfront-2.5.4/types_aiobotocore_cloudfront/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 01:07:25.000000 types-aiobotocore-cloudfront-2.5.4/types_aiobotocore_cloudfront/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)   138374 2023-08-08 01:07:29.000000 types-aiobotocore-cloudfront-2.5.4/types_aiobotocore_cloudfront/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)   138111 2023-08-08 01:07:27.000000 types-aiobotocore-cloudfront-2.5.4/types_aiobotocore_cloudfront/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-08-08 01:07:25.000000 types-aiobotocore-cloudfront-2.5.4/types_aiobotocore_cloudfront/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3770 2023-08-08 01:07:26.000000 types-aiobotocore-cloudfront-2.5.4/types_aiobotocore_cloudfront/waiter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3767 2023-08-08 01:07:26.000000 types-aiobotocore-cloudfront-2.5.4/types_aiobotocore_cloudfront/waiter.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:23:26.346626 types-aiobotocore-cloudfront-2.5.4/types_aiobotocore_cloudfront.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    14807 2023-08-08 01:23:26.000000 types-aiobotocore-cloudfront-2.5.4/types_aiobotocore_cloudfront.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      949 2023-08-08 01:23:26.000000 types-aiobotocore-cloudfront-2.5.4/types_aiobotocore_cloudfront.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 01:23:26.000000 types-aiobotocore-cloudfront-2.5.4/types_aiobotocore_cloudfront.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 01:23:26.000000 types-aiobotocore-cloudfront-2.5.4/types_aiobotocore_cloudfront.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-08 01:23:26.000000 types-aiobotocore-cloudfront-2.5.4/types_aiobotocore_cloudfront.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-08-08 01:23:26.000000 types-aiobotocore-cloudfront-2.5.4/types_aiobotocore_cloudfront.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-cloudfront-2.5.2.post3/LICENSE` & `types-aiobotocore-cloudfront-2.5.4/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-cloudfront-2.5.2.post3/PKG-INFO` & `types-aiobotocore-cloudfront-2.5.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-cloudfront
-Version: 2.5.2.post3
-Summary: Type annotations for aiobotocore.CloudFront 2.5.2 service generated with mypy-boto3-builder 7.17.2
+Version: 2.5.4
+Summary: Type annotations for aiobotocore.CloudFront 2.5.4 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudfront/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-cloudfront.svg?color=blue)](https://pypi.org/project/types-aiobotocore-cloudfront)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudfront/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-cloudfront)](https://pepy.tech/project/types-aiobotocore-cloudfront)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.CloudFront 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront)
+[aiobotocore.CloudFront 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-cloudfront-2.5.2.post3/README.md` & `types-aiobotocore-cloudfront-2.5.4/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-cloudfront.svg?color=blue)](https://pypi.org/project/types-aiobotocore-cloudfront)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudfront/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-cloudfront)](https://pepy.tech/project/types-aiobotocore-cloudfront)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.CloudFront 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront)
+[aiobotocore.CloudFront 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-cloudfront-2.5.2.post3/setup.py` & `types-aiobotocore-cloudfront-2.5.4/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-cloudfront",
-    version="2.5.2.post3",
+    version="2.5.4",
     packages=["types_aiobotocore_cloudfront"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.CloudFront 2.5.2 service generated with"
+        "Type annotations for aiobotocore.CloudFront 2.5.4 service generated with"
         " mypy-boto3-builder 7.17.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
```

### Comparing `types-aiobotocore-cloudfront-2.5.2.post3/types_aiobotocore_cloudfront/__init__.py` & `types-aiobotocore-cloudfront-2.5.4/types_aiobotocore_cloudfront/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-cloudfront-2.5.2.post3/types_aiobotocore_cloudfront/__init__.pyi` & `types-aiobotocore-cloudfront-2.5.4/types_aiobotocore_cloudfront/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-cloudfront-2.5.2.post3/types_aiobotocore_cloudfront/__main__.py` & `types-aiobotocore-cloudfront-2.5.4/types_aiobotocore_cloudfront/__main__.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.CloudFront 2.5.2\nVersion:         2.5.2.post3\nBuilder"
+        "Type annotations for aiobotocore.CloudFront 2.5.4\nVersion:         2.5.4\nBuilder"
         " version: 7.17.2\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudfront//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront\nOther"
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

### Comparing `types-aiobotocore-cloudfront-2.5.2.post3/types_aiobotocore_cloudfront/client.py` & `types-aiobotocore-cloudfront-2.5.4/types_aiobotocore_cloudfront/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -361,15 +361,16 @@
 
     async def copy_distribution(
         self,
         *,
         PrimaryDistributionId: str,
         CallerReference: str,
         Staging: bool = ...,
-        IfMatch: str = ...
+        IfMatch: str = ...,
+        Enabled: bool = ...
     ) -> CopyDistributionResultTypeDef:
         """
         Creates a staging distribution using the configuration of the provided primary
         distribution.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.copy_distribution)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudfront/client/#copy_distribution)
```

### Comparing `types-aiobotocore-cloudfront-2.5.2.post3/types_aiobotocore_cloudfront/client.pyi` & `types-aiobotocore-cloudfront-2.5.4/types_aiobotocore_cloudfront/client.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -353,15 +353,16 @@
         """
     async def copy_distribution(
         self,
         *,
         PrimaryDistributionId: str,
         CallerReference: str,
         Staging: bool = ...,
-        IfMatch: str = ...
+        IfMatch: str = ...,
+        Enabled: bool = ...
     ) -> CopyDistributionResultTypeDef:
         """
         Creates a staging distribution using the configuration of the provided primary
         distribution.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.copy_distribution)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudfront/client/#copy_distribution)
```

### Comparing `types-aiobotocore-cloudfront-2.5.2.post3/types_aiobotocore_cloudfront/literals.py` & `types-aiobotocore-cloudfront-2.5.4/types_aiobotocore_cloudfront/literals.py`

 * *Files 2% similar despite different names*

```diff
@@ -74,15 +74,15 @@
 CachePolicyTypeType = Literal["custom", "managed"]
 CertificateSourceType = Literal["acm", "cloudfront", "iam"]
 ContinuousDeploymentPolicyTypeType = Literal["SingleHeader", "SingleWeight"]
 DistributionDeployedWaiterName = Literal["distribution_deployed"]
 EventTypeType = Literal["origin-request", "origin-response", "viewer-request", "viewer-response"]
 FormatType = Literal["URLEncoded"]
 FrameOptionsListType = Literal["DENY", "SAMEORIGIN"]
-FunctionRuntimeType = Literal["cloudfront-js-1.0"]
+FunctionRuntimeType = Literal["cloudfront-js-1.0", "cloudfront-js-2.0"]
 FunctionStageType = Literal["DEVELOPMENT", "LIVE"]
 GeoRestrictionTypeType = Literal["blacklist", "none", "whitelist"]
 HttpVersionType = Literal["http1.1", "http2", "http2and3", "http3"]
 ICPRecordalStatusType = Literal["APPROVED", "PENDING", "SUSPENDED"]
 InvalidationCompletedWaiterName = Literal["invalidation_completed"]
 ItemSelectionType = Literal["all", "none", "whitelist"]
 ListCloudFrontOriginAccessIdentitiesPaginatorName = Literal[
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
```

### Comparing `types-aiobotocore-cloudfront-2.5.2.post3/types_aiobotocore_cloudfront/literals.pyi` & `types-aiobotocore-cloudfront-2.5.4/types_aiobotocore_cloudfront/literals.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -72,15 +72,15 @@
 CachePolicyTypeType = Literal["custom", "managed"]
 CertificateSourceType = Literal["acm", "cloudfront", "iam"]
 ContinuousDeploymentPolicyTypeType = Literal["SingleHeader", "SingleWeight"]
 DistributionDeployedWaiterName = Literal["distribution_deployed"]
 EventTypeType = Literal["origin-request", "origin-response", "viewer-request", "viewer-response"]
 FormatType = Literal["URLEncoded"]
 FrameOptionsListType = Literal["DENY", "SAMEORIGIN"]
-FunctionRuntimeType = Literal["cloudfront-js-1.0"]
+FunctionRuntimeType = Literal["cloudfront-js-1.0", "cloudfront-js-2.0"]
 FunctionStageType = Literal["DEVELOPMENT", "LIVE"]
 GeoRestrictionTypeType = Literal["blacklist", "none", "whitelist"]
 HttpVersionType = Literal["http1.1", "http2", "http2and3", "http3"]
 ICPRecordalStatusType = Literal["APPROVED", "PENDING", "SUSPENDED"]
 InvalidationCompletedWaiterName = Literal["invalidation_completed"]
 ItemSelectionType = Literal["all", "none", "whitelist"]
 ListCloudFrontOriginAccessIdentitiesPaginatorName = Literal[
@@ -135,14 +135,15 @@
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
@@ -238,14 +239,15 @@
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
@@ -324,26 +326,28 @@
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

### Comparing `types-aiobotocore-cloudfront-2.5.2.post3/types_aiobotocore_cloudfront/paginator.py` & `types-aiobotocore-cloudfront-2.5.4/types_aiobotocore_cloudfront/paginator.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-cloudfront-2.5.2.post3/types_aiobotocore_cloudfront/paginator.pyi` & `types-aiobotocore-cloudfront-2.5.4/types_aiobotocore_cloudfront/paginator.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-cloudfront-2.5.2.post3/types_aiobotocore_cloudfront/type_defs.py` & `types-aiobotocore-cloudfront-2.5.4/types_aiobotocore_cloudfront/type_defs.py`

 * *Files 0% similar despite different names*

```diff
@@ -22,14 +22,15 @@
     CachePolicyHeaderBehaviorType,
     CachePolicyQueryStringBehaviorType,
     CachePolicyTypeType,
     CertificateSourceType,
     ContinuousDeploymentPolicyTypeType,
     EventTypeType,
     FrameOptionsListType,
+    FunctionRuntimeType,
     FunctionStageType,
     GeoRestrictionTypeType,
     HttpVersionType,
     ICPRecordalStatusType,
     ItemSelectionType,
     MethodType,
     MinimumProtocolVersionType,
@@ -661,14 +662,15 @@
     },
 )
 _OptionalCopyDistributionRequestRequestTypeDef = TypedDict(
     "_OptionalCopyDistributionRequestRequestTypeDef",
     {
         "Staging": bool,
         "IfMatch": str,
+        "Enabled": bool,
     },
     total=False,
 )
 
 
 class CopyDistributionRequestRequestTypeDef(
     _RequiredCopyDistributionRequestRequestTypeDef, _OptionalCopyDistributionRequestRequestTypeDef
@@ -687,15 +689,15 @@
     },
 )
 
 FunctionConfigTypeDef = TypedDict(
     "FunctionConfigTypeDef",
     {
         "Comment": str,
-        "Runtime": Literal["cloudfront-js-1.0"],
+        "Runtime": FunctionRuntimeType,
     },
 )
 
 _RequiredKeyGroupConfigTypeDef = TypedDict(
     "_RequiredKeyGroupConfigTypeDef",
     {
         "Name": str,
```

### Comparing `types-aiobotocore-cloudfront-2.5.2.post3/types_aiobotocore_cloudfront/type_defs.pyi` & `types-aiobotocore-cloudfront-2.5.4/types_aiobotocore_cloudfront/type_defs.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -22,14 +22,15 @@
     CachePolicyHeaderBehaviorType,
     CachePolicyQueryStringBehaviorType,
     CachePolicyTypeType,
     CertificateSourceType,
     ContinuousDeploymentPolicyTypeType,
     EventTypeType,
     FrameOptionsListType,
+    FunctionRuntimeType,
     FunctionStageType,
     GeoRestrictionTypeType,
     HttpVersionType,
     ICPRecordalStatusType,
     ItemSelectionType,
     MethodType,
     MinimumProtocolVersionType,
@@ -644,14 +645,15 @@
     },
 )
 _OptionalCopyDistributionRequestRequestTypeDef = TypedDict(
     "_OptionalCopyDistributionRequestRequestTypeDef",
     {
         "Staging": bool,
         "IfMatch": str,
+        "Enabled": bool,
     },
     total=False,
 )
 
 class CopyDistributionRequestRequestTypeDef(
     _RequiredCopyDistributionRequestRequestTypeDef, _OptionalCopyDistributionRequestRequestTypeDef
 ):
@@ -668,15 +670,15 @@
     },
 )
 
 FunctionConfigTypeDef = TypedDict(
     "FunctionConfigTypeDef",
     {
         "Comment": str,
-        "Runtime": Literal["cloudfront-js-1.0"],
+        "Runtime": FunctionRuntimeType,
     },
 )
 
 _RequiredKeyGroupConfigTypeDef = TypedDict(
     "_RequiredKeyGroupConfigTypeDef",
     {
         "Name": str,
```

### Comparing `types-aiobotocore-cloudfront-2.5.2.post3/types_aiobotocore_cloudfront/waiter.py` & `types-aiobotocore-cloudfront-2.5.4/types_aiobotocore_cloudfront/waiter.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-cloudfront-2.5.2.post3/types_aiobotocore_cloudfront/waiter.pyi` & `types-aiobotocore-cloudfront-2.5.4/types_aiobotocore_cloudfront/waiter.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-cloudfront-2.5.2.post3/types_aiobotocore_cloudfront.egg-info/PKG-INFO` & `types-aiobotocore-cloudfront-2.5.4/types_aiobotocore_cloudfront.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-cloudfront
-Version: 2.5.2.post3
-Summary: Type annotations for aiobotocore.CloudFront 2.5.2 service generated with mypy-boto3-builder 7.17.2
+Version: 2.5.4
+Summary: Type annotations for aiobotocore.CloudFront 2.5.4 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudfront/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-cloudfront.svg?color=blue)](https://pypi.org/project/types-aiobotocore-cloudfront)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudfront/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-cloudfront)](https://pepy.tech/project/types-aiobotocore-cloudfront)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.CloudFront 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront)
+[aiobotocore.CloudFront 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-cloudfront-2.5.2.post3/types_aiobotocore_cloudfront.egg-info/SOURCES.txt` & `types-aiobotocore-cloudfront-2.5.4/types_aiobotocore_cloudfront.egg-info/SOURCES.txt`

 * *Files identical despite different names*


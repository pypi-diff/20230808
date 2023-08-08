# Comparing `tmp/types-aiobotocore-codeartifact-2.5.2.post3.tar.gz` & `tmp/types-aiobotocore-codeartifact-2.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-codeartifact-2.5.2.post3.tar", last modified: Fri Aug  4 12:37:26 2023, max compression
+gzip compressed data, was "types-aiobotocore-codeartifact-2.5.4.tar", last modified: Tue Aug  8 01:23:27 2023, max compression
```

## Comparing `types-aiobotocore-codeartifact-2.5.2.post3.tar` & `types-aiobotocore-codeartifact-2.5.4.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:37:26.663400 types-aiobotocore-codeartifact-2.5.2.post3/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-04 12:19:59.000000 types-aiobotocore-codeartifact-2.5.2.post3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    13979 2023-08-04 12:37:26.663400 types-aiobotocore-codeartifact-2.5.2.post3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    12441 2023-08-04 12:19:59.000000 types-aiobotocore-codeartifact-2.5.2.post3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-04 12:37:26.663400 types-aiobotocore-codeartifact-2.5.2.post3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2107 2023-08-04 12:19:59.000000 types-aiobotocore-codeartifact-2.5.2.post3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:37:26.655400 types-aiobotocore-codeartifact-2.5.2.post3/types_aiobotocore_codeartifact/
--rw-r--r--   0 runner    (1001) docker     (123)     1803 2023-08-04 12:19:59.000000 types-aiobotocore-codeartifact-2.5.2.post3/types_aiobotocore_codeartifact/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1802 2023-08-04 12:19:59.000000 types-aiobotocore-codeartifact-2.5.2.post3/types_aiobotocore_codeartifact/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      963 2023-08-04 12:19:59.000000 types-aiobotocore-codeartifact-2.5.2.post3/types_aiobotocore_codeartifact/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    36361 2023-08-04 12:19:59.000000 types-aiobotocore-codeartifact-2.5.2.post3/types_aiobotocore_codeartifact/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    36308 2023-08-04 12:19:59.000000 types-aiobotocore-codeartifact-2.5.2.post3/types_aiobotocore_codeartifact/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9699 2023-08-04 12:20:00.000000 types-aiobotocore-codeartifact-2.5.2.post3/types_aiobotocore_codeartifact/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     9697 2023-08-04 12:20:00.000000 types-aiobotocore-codeartifact-2.5.2.post3/types_aiobotocore_codeartifact/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9037 2023-08-04 12:19:59.000000 types-aiobotocore-codeartifact-2.5.2.post3/types_aiobotocore_codeartifact/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     9028 2023-08-04 12:19:59.000000 types-aiobotocore-codeartifact-2.5.2.post3/types_aiobotocore_codeartifact/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 12:19:59.000000 types-aiobotocore-codeartifact-2.5.2.post3/types_aiobotocore_codeartifact/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    46914 2023-08-04 12:20:01.000000 types-aiobotocore-codeartifact-2.5.2.post3/types_aiobotocore_codeartifact/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    46835 2023-08-04 12:20:00.000000 types-aiobotocore-codeartifact-2.5.2.post3/types_aiobotocore_codeartifact/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-04 12:19:59.000000 types-aiobotocore-codeartifact-2.5.2.post3/types_aiobotocore_codeartifact/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:37:26.663400 types-aiobotocore-codeartifact-2.5.2.post3/types_aiobotocore_codeartifact.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    13979 2023-08-04 12:37:26.000000 types-aiobotocore-codeartifact-2.5.2.post3/types_aiobotocore_codeartifact.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      908 2023-08-04 12:37:26.000000 types-aiobotocore-codeartifact-2.5.2.post3/types_aiobotocore_codeartifact.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 12:37:26.000000 types-aiobotocore-codeartifact-2.5.2.post3/types_aiobotocore_codeartifact.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 12:37:26.000000 types-aiobotocore-codeartifact-2.5.2.post3/types_aiobotocore_codeartifact.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-04 12:37:26.000000 types-aiobotocore-codeartifact-2.5.2.post3/types_aiobotocore_codeartifact.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-08-04 12:37:26.000000 types-aiobotocore-codeartifact-2.5.2.post3/types_aiobotocore_codeartifact.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:23:27.846635 types-aiobotocore-codeartifact-2.5.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-08 01:07:40.000000 types-aiobotocore-codeartifact-2.5.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    13973 2023-08-08 01:23:27.846635 types-aiobotocore-codeartifact-2.5.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    12441 2023-08-08 01:07:40.000000 types-aiobotocore-codeartifact-2.5.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-08 01:23:27.846635 types-aiobotocore-codeartifact-2.5.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2101 2023-08-08 01:07:40.000000 types-aiobotocore-codeartifact-2.5.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:23:27.846635 types-aiobotocore-codeartifact-2.5.4/types_aiobotocore_codeartifact/
+-rw-r--r--   0 runner    (1001) docker     (123)     1803 2023-08-08 01:07:40.000000 types-aiobotocore-codeartifact-2.5.4/types_aiobotocore_codeartifact/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1802 2023-08-08 01:07:40.000000 types-aiobotocore-codeartifact-2.5.4/types_aiobotocore_codeartifact/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      951 2023-08-08 01:07:40.000000 types-aiobotocore-codeartifact-2.5.4/types_aiobotocore_codeartifact/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36361 2023-08-08 01:07:40.000000 types-aiobotocore-codeartifact-2.5.4/types_aiobotocore_codeartifact/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36308 2023-08-08 01:07:40.000000 types-aiobotocore-codeartifact-2.5.4/types_aiobotocore_codeartifact/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9794 2023-08-08 01:07:40.000000 types-aiobotocore-codeartifact-2.5.4/types_aiobotocore_codeartifact/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9792 2023-08-08 01:07:40.000000 types-aiobotocore-codeartifact-2.5.4/types_aiobotocore_codeartifact/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9037 2023-08-08 01:07:40.000000 types-aiobotocore-codeartifact-2.5.4/types_aiobotocore_codeartifact/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9028 2023-08-08 01:07:40.000000 types-aiobotocore-codeartifact-2.5.4/types_aiobotocore_codeartifact/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 01:07:40.000000 types-aiobotocore-codeartifact-2.5.4/types_aiobotocore_codeartifact/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    46914 2023-08-08 01:07:41.000000 types-aiobotocore-codeartifact-2.5.4/types_aiobotocore_codeartifact/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46835 2023-08-08 01:07:41.000000 types-aiobotocore-codeartifact-2.5.4/types_aiobotocore_codeartifact/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-08-08 01:07:40.000000 types-aiobotocore-codeartifact-2.5.4/types_aiobotocore_codeartifact/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:23:27.846635 types-aiobotocore-codeartifact-2.5.4/types_aiobotocore_codeartifact.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    13973 2023-08-08 01:23:27.000000 types-aiobotocore-codeartifact-2.5.4/types_aiobotocore_codeartifact.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      908 2023-08-08 01:23:27.000000 types-aiobotocore-codeartifact-2.5.4/types_aiobotocore_codeartifact.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 01:23:27.000000 types-aiobotocore-codeartifact-2.5.4/types_aiobotocore_codeartifact.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 01:23:27.000000 types-aiobotocore-codeartifact-2.5.4/types_aiobotocore_codeartifact.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-08 01:23:27.000000 types-aiobotocore-codeartifact-2.5.4/types_aiobotocore_codeartifact.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-08-08 01:23:27.000000 types-aiobotocore-codeartifact-2.5.4/types_aiobotocore_codeartifact.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-codeartifact-2.5.2.post3/LICENSE` & `types-aiobotocore-codeartifact-2.5.4/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-codeartifact-2.5.2.post3/PKG-INFO` & `types-aiobotocore-codeartifact-2.5.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-codeartifact
-Version: 2.5.2.post3
-Summary: Type annotations for aiobotocore.CodeArtifact 2.5.2 service generated with mypy-boto3-builder 7.17.2
+Version: 2.5.4
+Summary: Type annotations for aiobotocore.CodeArtifact 2.5.4 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codeartifact/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-codeartifact.svg?color=blue)](https://pypi.org/project/types-aiobotocore-codeartifact)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codeartifact/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-codeartifact)](https://pepy.tech/project/types-aiobotocore-codeartifact)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.CodeArtifact 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeartifact.html#CodeArtifact)
+[aiobotocore.CodeArtifact 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeartifact.html#CodeArtifact)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-codeartifact-2.5.2.post3/README.md` & `types-aiobotocore-codeartifact-2.5.4/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-codeartifact.svg?color=blue)](https://pypi.org/project/types-aiobotocore-codeartifact)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codeartifact/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-codeartifact)](https://pepy.tech/project/types-aiobotocore-codeartifact)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.CodeArtifact 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeartifact.html#CodeArtifact)
+[aiobotocore.CodeArtifact 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeartifact.html#CodeArtifact)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-codeartifact-2.5.2.post3/setup.py` & `types-aiobotocore-codeartifact-2.5.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-codeartifact",
-    version="2.5.2.post3",
+    version="2.5.4",
     packages=["types_aiobotocore_codeartifact"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.CodeArtifact 2.5.2 service generated with"
+        "Type annotations for aiobotocore.CodeArtifact 2.5.4 service generated with"
         " mypy-boto3-builder 7.17.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
```

### Comparing `types-aiobotocore-codeartifact-2.5.2.post3/types_aiobotocore_codeartifact/__init__.py` & `types-aiobotocore-codeartifact-2.5.4/types_aiobotocore_codeartifact/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-codeartifact-2.5.2.post3/types_aiobotocore_codeartifact/__init__.pyi` & `types-aiobotocore-codeartifact-2.5.4/types_aiobotocore_codeartifact/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-codeartifact-2.5.2.post3/types_aiobotocore_codeartifact/__main__.py` & `types-aiobotocore-codeartifact-2.5.4/types_aiobotocore_codeartifact/__main__.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.CodeArtifact 2.5.2\nVersion:         2.5.2.post3\nBuilder"
+        "Type annotations for aiobotocore.CodeArtifact 2.5.4\nVersion:         2.5.4\nBuilder"
         " version: 7.17.2\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codeartifact//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeartifact.html#CodeArtifact\nOther"
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

### Comparing `types-aiobotocore-codeartifact-2.5.2.post3/types_aiobotocore_codeartifact/client.py` & `types-aiobotocore-codeartifact-2.5.4/types_aiobotocore_codeartifact/client.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-codeartifact-2.5.2.post3/types_aiobotocore_codeartifact/client.pyi` & `types-aiobotocore-codeartifact-2.5.4/types_aiobotocore_codeartifact/client.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-codeartifact-2.5.2.post3/types_aiobotocore_codeartifact/literals.py` & `types-aiobotocore-codeartifact-2.5.4/types_aiobotocore_codeartifact/literals.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,14 @@
 import sys
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = (
     "AllowPublishType",
     "AllowUpstreamType",
     "DomainStatusType",
     "ExternalConnectionStatusType",
     "HashAlgorithmType",
     "ListDomainsPaginatorName",
@@ -39,15 +38,14 @@
     "CodeArtifactServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "RegionName",
 )
 
-
 AllowPublishType = Literal["ALLOW", "BLOCK"]
 AllowUpstreamType = Literal["ALLOW", "BLOCK"]
 DomainStatusType = Literal["Active", "Deleted"]
 ExternalConnectionStatusType = Literal["Available"]
 HashAlgorithmType = Literal["MD5", "SHA-1", "SHA-256", "SHA-512"]
 ListDomainsPaginatorName = Literal["list_domains"]
 ListPackageVersionAssetsPaginatorName = Literal["list_package_version_assets"]
@@ -81,14 +79,15 @@
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
@@ -184,14 +183,15 @@
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
@@ -270,26 +270,28 @@
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

### Comparing `types-aiobotocore-codeartifact-2.5.2.post3/types_aiobotocore_codeartifact/literals.pyi` & `types-aiobotocore-codeartifact-2.5.4/types_aiobotocore_codeartifact/literals.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 import sys
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
+
 __all__ = (
     "AllowPublishType",
     "AllowUpstreamType",
     "DomainStatusType",
     "ExternalConnectionStatusType",
     "HashAlgorithmType",
     "ListDomainsPaginatorName",
@@ -38,14 +39,15 @@
     "CodeArtifactServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "RegionName",
 )
 
+
 AllowPublishType = Literal["ALLOW", "BLOCK"]
 AllowUpstreamType = Literal["ALLOW", "BLOCK"]
 DomainStatusType = Literal["Active", "Deleted"]
 ExternalConnectionStatusType = Literal["Available"]
 HashAlgorithmType = Literal["MD5", "SHA-1", "SHA-256", "SHA-512"]
 ListDomainsPaginatorName = Literal["list_domains"]
 ListPackageVersionAssetsPaginatorName = Literal["list_package_version_assets"]
@@ -79,14 +81,15 @@
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
@@ -182,14 +185,15 @@
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
@@ -268,26 +272,28 @@
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

### Comparing `types-aiobotocore-codeartifact-2.5.2.post3/types_aiobotocore_codeartifact/paginator.py` & `types-aiobotocore-codeartifact-2.5.4/types_aiobotocore_codeartifact/paginator.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-codeartifact-2.5.2.post3/types_aiobotocore_codeartifact/paginator.pyi` & `types-aiobotocore-codeartifact-2.5.4/types_aiobotocore_codeartifact/paginator.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-codeartifact-2.5.2.post3/types_aiobotocore_codeartifact/type_defs.py` & `types-aiobotocore-codeartifact-2.5.4/types_aiobotocore_codeartifact/type_defs.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-codeartifact-2.5.2.post3/types_aiobotocore_codeartifact/type_defs.pyi` & `types-aiobotocore-codeartifact-2.5.4/types_aiobotocore_codeartifact/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-codeartifact-2.5.2.post3/types_aiobotocore_codeartifact.egg-info/PKG-INFO` & `types-aiobotocore-codeartifact-2.5.4/types_aiobotocore_codeartifact.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-codeartifact
-Version: 2.5.2.post3
-Summary: Type annotations for aiobotocore.CodeArtifact 2.5.2 service generated with mypy-boto3-builder 7.17.2
+Version: 2.5.4
+Summary: Type annotations for aiobotocore.CodeArtifact 2.5.4 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codeartifact/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-codeartifact.svg?color=blue)](https://pypi.org/project/types-aiobotocore-codeartifact)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codeartifact/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-codeartifact)](https://pepy.tech/project/types-aiobotocore-codeartifact)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.CodeArtifact 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeartifact.html#CodeArtifact)
+[aiobotocore.CodeArtifact 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeartifact.html#CodeArtifact)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-codeartifact-2.5.2.post3/types_aiobotocore_codeartifact.egg-info/SOURCES.txt` & `types-aiobotocore-codeartifact-2.5.4/types_aiobotocore_codeartifact.egg-info/SOURCES.txt`

 * *Files identical despite different names*


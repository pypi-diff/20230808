# Comparing `tmp/types-aiobotocore-codeguru-reviewer-2.5.2.post3.tar.gz` & `tmp/types-aiobotocore-codeguru-reviewer-2.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-codeguru-reviewer-2.5.2.post3.tar", last modified: Fri Aug  4 12:37:28 2023, max compression
+gzip compressed data, was "types-aiobotocore-codeguru-reviewer-2.5.4.tar", last modified: Tue Aug  8 01:23:28 2023, max compression
```

## Comparing `types-aiobotocore-codeguru-reviewer-2.5.2.post3.tar` & `types-aiobotocore-codeguru-reviewer-2.5.4.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:37:28.815454 types-aiobotocore-codeguru-reviewer-2.5.2.post3/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-04 12:20:15.000000 types-aiobotocore-codeguru-reviewer-2.5.2.post3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    14522 2023-08-04 12:37:28.815454 types-aiobotocore-codeguru-reviewer-2.5.2.post3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    12965 2023-08-04 12:20:15.000000 types-aiobotocore-codeguru-reviewer-2.5.2.post3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-04 12:37:28.815454 types-aiobotocore-codeguru-reviewer-2.5.2.post3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2141 2023-08-04 12:20:15.000000 types-aiobotocore-codeguru-reviewer-2.5.2.post3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:37:28.815454 types-aiobotocore-codeguru-reviewer-2.5.2.post3/types_aiobotocore_codeguru_reviewer/
--rw-r--r--   0 runner    (1001) docker     (123)     1297 2023-08-04 12:20:15.000000 types-aiobotocore-codeguru-reviewer-2.5.2.post3/types_aiobotocore_codeguru_reviewer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1296 2023-08-04 12:20:15.000000 types-aiobotocore-codeguru-reviewer-2.5.2.post3/types_aiobotocore_codeguru_reviewer/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      981 2023-08-04 12:20:15.000000 types-aiobotocore-codeguru-reviewer-2.5.2.post3/types_aiobotocore_codeguru_reviewer/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16599 2023-08-04 12:20:15.000000 types-aiobotocore-codeguru-reviewer-2.5.2.post3/types_aiobotocore_codeguru_reviewer/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    16573 2023-08-04 12:20:15.000000 types-aiobotocore-codeguru-reviewer-2.5.2.post3/types_aiobotocore_codeguru_reviewer/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9667 2023-08-04 12:20:15.000000 types-aiobotocore-codeguru-reviewer-2.5.2.post3/types_aiobotocore_codeguru_reviewer/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     9665 2023-08-04 12:20:15.000000 types-aiobotocore-codeguru-reviewer-2.5.2.post3/types_aiobotocore_codeguru_reviewer/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2542 2023-08-04 12:20:15.000000 types-aiobotocore-codeguru-reviewer-2.5.2.post3/types_aiobotocore_codeguru_reviewer/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     2539 2023-08-04 12:20:15.000000 types-aiobotocore-codeguru-reviewer-2.5.2.post3/types_aiobotocore_codeguru_reviewer/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 12:20:15.000000 types-aiobotocore-codeguru-reviewer-2.5.2.post3/types_aiobotocore_codeguru_reviewer/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    20999 2023-08-04 12:20:16.000000 types-aiobotocore-codeguru-reviewer-2.5.2.post3/types_aiobotocore_codeguru_reviewer/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    20977 2023-08-04 12:20:16.000000 types-aiobotocore-codeguru-reviewer-2.5.2.post3/types_aiobotocore_codeguru_reviewer/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-04 12:20:15.000000 types-aiobotocore-codeguru-reviewer-2.5.2.post3/types_aiobotocore_codeguru_reviewer/version.py
--rw-r--r--   0 runner    (1001) docker     (123)     2858 2023-08-04 12:20:15.000000 types-aiobotocore-codeguru-reviewer-2.5.2.post3/types_aiobotocore_codeguru_reviewer/waiter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2856 2023-08-04 12:20:15.000000 types-aiobotocore-codeguru-reviewer-2.5.2.post3/types_aiobotocore_codeguru_reviewer/waiter.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:37:28.815454 types-aiobotocore-codeguru-reviewer-2.5.2.post3/types_aiobotocore_codeguru_reviewer.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    14522 2023-08-04 12:37:28.000000 types-aiobotocore-codeguru-reviewer-2.5.2.post3/types_aiobotocore_codeguru_reviewer.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1096 2023-08-04 12:37:28.000000 types-aiobotocore-codeguru-reviewer-2.5.2.post3/types_aiobotocore_codeguru_reviewer.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 12:37:28.000000 types-aiobotocore-codeguru-reviewer-2.5.2.post3/types_aiobotocore_codeguru_reviewer.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 12:37:28.000000 types-aiobotocore-codeguru-reviewer-2.5.2.post3/types_aiobotocore_codeguru_reviewer.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-04 12:37:28.000000 types-aiobotocore-codeguru-reviewer-2.5.2.post3/types_aiobotocore_codeguru_reviewer.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-08-04 12:37:28.000000 types-aiobotocore-codeguru-reviewer-2.5.2.post3/types_aiobotocore_codeguru_reviewer.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:23:28.918645 types-aiobotocore-codeguru-reviewer-2.5.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-08 01:07:54.000000 types-aiobotocore-codeguru-reviewer-2.5.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    14516 2023-08-08 01:23:28.918645 types-aiobotocore-codeguru-reviewer-2.5.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    12965 2023-08-08 01:07:54.000000 types-aiobotocore-codeguru-reviewer-2.5.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-08 01:23:28.918645 types-aiobotocore-codeguru-reviewer-2.5.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2135 2023-08-08 01:07:54.000000 types-aiobotocore-codeguru-reviewer-2.5.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:23:28.898645 types-aiobotocore-codeguru-reviewer-2.5.4/types_aiobotocore_codeguru_reviewer/
+-rw-r--r--   0 runner    (1001) docker     (123)     1297 2023-08-08 01:07:54.000000 types-aiobotocore-codeguru-reviewer-2.5.4/types_aiobotocore_codeguru_reviewer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1296 2023-08-08 01:07:54.000000 types-aiobotocore-codeguru-reviewer-2.5.4/types_aiobotocore_codeguru_reviewer/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      969 2023-08-08 01:07:54.000000 types-aiobotocore-codeguru-reviewer-2.5.4/types_aiobotocore_codeguru_reviewer/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16599 2023-08-08 01:07:54.000000 types-aiobotocore-codeguru-reviewer-2.5.4/types_aiobotocore_codeguru_reviewer/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16573 2023-08-08 01:07:54.000000 types-aiobotocore-codeguru-reviewer-2.5.4/types_aiobotocore_codeguru_reviewer/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9762 2023-08-08 01:07:55.000000 types-aiobotocore-codeguru-reviewer-2.5.4/types_aiobotocore_codeguru_reviewer/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9760 2023-08-08 01:07:55.000000 types-aiobotocore-codeguru-reviewer-2.5.4/types_aiobotocore_codeguru_reviewer/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2542 2023-08-08 01:07:54.000000 types-aiobotocore-codeguru-reviewer-2.5.4/types_aiobotocore_codeguru_reviewer/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2539 2023-08-08 01:07:54.000000 types-aiobotocore-codeguru-reviewer-2.5.4/types_aiobotocore_codeguru_reviewer/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 01:07:54.000000 types-aiobotocore-codeguru-reviewer-2.5.4/types_aiobotocore_codeguru_reviewer/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    20999 2023-08-08 01:07:55.000000 types-aiobotocore-codeguru-reviewer-2.5.4/types_aiobotocore_codeguru_reviewer/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20977 2023-08-08 01:07:55.000000 types-aiobotocore-codeguru-reviewer-2.5.4/types_aiobotocore_codeguru_reviewer/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-08-08 01:07:54.000000 types-aiobotocore-codeguru-reviewer-2.5.4/types_aiobotocore_codeguru_reviewer/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2858 2023-08-08 01:07:54.000000 types-aiobotocore-codeguru-reviewer-2.5.4/types_aiobotocore_codeguru_reviewer/waiter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2856 2023-08-08 01:07:54.000000 types-aiobotocore-codeguru-reviewer-2.5.4/types_aiobotocore_codeguru_reviewer/waiter.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:23:28.918645 types-aiobotocore-codeguru-reviewer-2.5.4/types_aiobotocore_codeguru_reviewer.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    14516 2023-08-08 01:23:28.000000 types-aiobotocore-codeguru-reviewer-2.5.4/types_aiobotocore_codeguru_reviewer.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1096 2023-08-08 01:23:28.000000 types-aiobotocore-codeguru-reviewer-2.5.4/types_aiobotocore_codeguru_reviewer.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 01:23:28.000000 types-aiobotocore-codeguru-reviewer-2.5.4/types_aiobotocore_codeguru_reviewer.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 01:23:28.000000 types-aiobotocore-codeguru-reviewer-2.5.4/types_aiobotocore_codeguru_reviewer.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-08 01:23:28.000000 types-aiobotocore-codeguru-reviewer-2.5.4/types_aiobotocore_codeguru_reviewer.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-08-08 01:23:28.000000 types-aiobotocore-codeguru-reviewer-2.5.4/types_aiobotocore_codeguru_reviewer.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-codeguru-reviewer-2.5.2.post3/LICENSE` & `types-aiobotocore-codeguru-reviewer-2.5.4/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-codeguru-reviewer-2.5.2.post3/PKG-INFO` & `types-aiobotocore-codeguru-reviewer-2.5.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-codeguru-reviewer
-Version: 2.5.2.post3
-Summary: Type annotations for aiobotocore.CodeGuruReviewer 2.5.2 service generated with mypy-boto3-builder 7.17.2
+Version: 2.5.4
+Summary: Type annotations for aiobotocore.CodeGuruReviewer 2.5.4 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codeguru_reviewer/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-codeguru-reviewer.svg?color=blue)](https://pypi.org/project/types-aiobotocore-codeguru-reviewer)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codeguru_reviewer/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-codeguru-reviewer)](https://pepy.tech/project/types-aiobotocore-codeguru-reviewer)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.CodeGuruReviewer 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeguru-reviewer.html#CodeGuruReviewer)
+[aiobotocore.CodeGuruReviewer 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeguru-reviewer.html#CodeGuruReviewer)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-codeguru-reviewer-2.5.2.post3/README.md` & `types-aiobotocore-codeguru-reviewer-2.5.4/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-codeguru-reviewer.svg?color=blue)](https://pypi.org/project/types-aiobotocore-codeguru-reviewer)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codeguru_reviewer/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-codeguru-reviewer)](https://pepy.tech/project/types-aiobotocore-codeguru-reviewer)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.CodeGuruReviewer 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeguru-reviewer.html#CodeGuruReviewer)
+[aiobotocore.CodeGuruReviewer 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeguru-reviewer.html#CodeGuruReviewer)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-codeguru-reviewer-2.5.2.post3/setup.py` & `types-aiobotocore-codeguru-reviewer-2.5.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-codeguru-reviewer",
-    version="2.5.2.post3",
+    version="2.5.4",
     packages=["types_aiobotocore_codeguru_reviewer"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.CodeGuruReviewer 2.5.2 service generated with"
+        "Type annotations for aiobotocore.CodeGuruReviewer 2.5.4 service generated with"
         " mypy-boto3-builder 7.17.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
```

### Comparing `types-aiobotocore-codeguru-reviewer-2.5.2.post3/types_aiobotocore_codeguru_reviewer/__init__.py` & `types-aiobotocore-codeguru-reviewer-2.5.4/types_aiobotocore_codeguru_reviewer/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-codeguru-reviewer-2.5.2.post3/types_aiobotocore_codeguru_reviewer/__init__.pyi` & `types-aiobotocore-codeguru-reviewer-2.5.4/types_aiobotocore_codeguru_reviewer/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-codeguru-reviewer-2.5.2.post3/types_aiobotocore_codeguru_reviewer/client.py` & `types-aiobotocore-codeguru-reviewer-2.5.4/types_aiobotocore_codeguru_reviewer/client.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-codeguru-reviewer-2.5.2.post3/types_aiobotocore_codeguru_reviewer/client.pyi` & `types-aiobotocore-codeguru-reviewer-2.5.4/types_aiobotocore_codeguru_reviewer/client.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-codeguru-reviewer-2.5.2.post3/types_aiobotocore_codeguru_reviewer/literals.py` & `types-aiobotocore-codeguru-reviewer-2.5.4/types_aiobotocore_codeguru_reviewer/literals.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -14,15 +14,14 @@
 import sys
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = (
     "AnalysisTypeType",
     "CodeReviewCompletedWaiterName",
     "ConfigFileStateType",
     "EncryptionOptionType",
     "JobStateType",
     "ListRepositoryAssociationsPaginatorName",
@@ -38,15 +37,14 @@
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "WaiterName",
     "RegionName",
 )
 
-
 AnalysisTypeType = Literal["CodeQuality", "Security"]
 CodeReviewCompletedWaiterName = Literal["code_review_completed"]
 ConfigFileStateType = Literal["Absent", "Present", "PresentWithErrors"]
 EncryptionOptionType = Literal["AWS_OWNED_CMK", "CUSTOMER_MANAGED_CMK"]
 JobStateType = Literal["Completed", "Deleting", "Failed", "Pending"]
 ListRepositoryAssociationsPaginatorName = Literal["list_repository_associations"]
 ProviderTypeType = Literal[
@@ -85,14 +83,15 @@
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
@@ -188,14 +187,15 @@
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
@@ -274,26 +274,28 @@
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

### Comparing `types-aiobotocore-codeguru-reviewer-2.5.2.post3/types_aiobotocore_codeguru_reviewer/literals.pyi` & `types-aiobotocore-codeguru-reviewer-2.5.4/types_aiobotocore_codeguru_reviewer/literals.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 import sys
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
+
 __all__ = (
     "AnalysisTypeType",
     "CodeReviewCompletedWaiterName",
     "ConfigFileStateType",
     "EncryptionOptionType",
     "JobStateType",
     "ListRepositoryAssociationsPaginatorName",
@@ -37,14 +38,15 @@
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "WaiterName",
     "RegionName",
 )
 
+
 AnalysisTypeType = Literal["CodeQuality", "Security"]
 CodeReviewCompletedWaiterName = Literal["code_review_completed"]
 ConfigFileStateType = Literal["Absent", "Present", "PresentWithErrors"]
 EncryptionOptionType = Literal["AWS_OWNED_CMK", "CUSTOMER_MANAGED_CMK"]
 JobStateType = Literal["Completed", "Deleting", "Failed", "Pending"]
 ListRepositoryAssociationsPaginatorName = Literal["list_repository_associations"]
 ProviderTypeType = Literal[
@@ -83,14 +85,15 @@
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
@@ -186,14 +189,15 @@
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
@@ -272,26 +276,28 @@
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

### Comparing `types-aiobotocore-codeguru-reviewer-2.5.2.post3/types_aiobotocore_codeguru_reviewer/paginator.py` & `types-aiobotocore-codeguru-reviewer-2.5.4/types_aiobotocore_codeguru_reviewer/paginator.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-codeguru-reviewer-2.5.2.post3/types_aiobotocore_codeguru_reviewer/paginator.pyi` & `types-aiobotocore-codeguru-reviewer-2.5.4/types_aiobotocore_codeguru_reviewer/paginator.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-codeguru-reviewer-2.5.2.post3/types_aiobotocore_codeguru_reviewer/type_defs.py` & `types-aiobotocore-codeguru-reviewer-2.5.4/types_aiobotocore_codeguru_reviewer/type_defs.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-codeguru-reviewer-2.5.2.post3/types_aiobotocore_codeguru_reviewer/type_defs.pyi` & `types-aiobotocore-codeguru-reviewer-2.5.4/types_aiobotocore_codeguru_reviewer/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-codeguru-reviewer-2.5.2.post3/types_aiobotocore_codeguru_reviewer/waiter.py` & `types-aiobotocore-codeguru-reviewer-2.5.4/types_aiobotocore_codeguru_reviewer/waiter.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-codeguru-reviewer-2.5.2.post3/types_aiobotocore_codeguru_reviewer/waiter.pyi` & `types-aiobotocore-codeguru-reviewer-2.5.4/types_aiobotocore_codeguru_reviewer/waiter.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-codeguru-reviewer-2.5.2.post3/types_aiobotocore_codeguru_reviewer.egg-info/PKG-INFO` & `types-aiobotocore-codeguru-reviewer-2.5.4/types_aiobotocore_codeguru_reviewer.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-codeguru-reviewer
-Version: 2.5.2.post3
-Summary: Type annotations for aiobotocore.CodeGuruReviewer 2.5.2 service generated with mypy-boto3-builder 7.17.2
+Version: 2.5.4
+Summary: Type annotations for aiobotocore.CodeGuruReviewer 2.5.4 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codeguru_reviewer/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-codeguru-reviewer.svg?color=blue)](https://pypi.org/project/types-aiobotocore-codeguru-reviewer)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codeguru_reviewer/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-codeguru-reviewer)](https://pepy.tech/project/types-aiobotocore-codeguru-reviewer)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.CodeGuruReviewer 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeguru-reviewer.html#CodeGuruReviewer)
+[aiobotocore.CodeGuruReviewer 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeguru-reviewer.html#CodeGuruReviewer)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-codeguru-reviewer-2.5.2.post3/types_aiobotocore_codeguru_reviewer.egg-info/SOURCES.txt` & `types-aiobotocore-codeguru-reviewer-2.5.4/types_aiobotocore_codeguru_reviewer.egg-info/SOURCES.txt`

 * *Files identical despite different names*


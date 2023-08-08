# Comparing `tmp/types-aiobotocore-connectcases-2.5.2.post3.tar.gz` & `tmp/types-aiobotocore-connectcases-2.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-connectcases-2.5.2.post3.tar", last modified: Fri Aug  4 12:37:31 2023, max compression
+gzip compressed data, was "types-aiobotocore-connectcases-2.5.4.tar", last modified: Tue Aug  8 01:23:33 2023, max compression
```

## Comparing `types-aiobotocore-connectcases-2.5.2.post3.tar` & `types-aiobotocore-connectcases-2.5.4.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:37:31.699526 types-aiobotocore-connectcases-2.5.2.post3/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-04 12:20:59.000000 types-aiobotocore-connectcases-2.5.2.post3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    13361 2023-08-04 12:37:31.695526 types-aiobotocore-connectcases-2.5.2.post3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    11823 2023-08-04 12:20:59.000000 types-aiobotocore-connectcases-2.5.2.post3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-04 12:37:31.699526 types-aiobotocore-connectcases-2.5.2.post3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2107 2023-08-04 12:20:59.000000 types-aiobotocore-connectcases-2.5.2.post3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:37:31.691526 types-aiobotocore-connectcases-2.5.2.post3/types_aiobotocore_connectcases/
--rw-r--r--   0 runner    (1001) docker     (123)      877 2023-08-04 12:20:59.000000 types-aiobotocore-connectcases-2.5.2.post3/types_aiobotocore_connectcases/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      876 2023-08-04 12:20:59.000000 types-aiobotocore-connectcases-2.5.2.post3/types_aiobotocore_connectcases/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      963 2023-08-04 12:20:59.000000 types-aiobotocore-connectcases-2.5.2.post3/types_aiobotocore_connectcases/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    23885 2023-08-04 12:20:59.000000 types-aiobotocore-connectcases-2.5.2.post3/types_aiobotocore_connectcases/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    23844 2023-08-04 12:20:59.000000 types-aiobotocore-connectcases-2.5.2.post3/types_aiobotocore_connectcases/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8585 2023-08-04 12:21:00.000000 types-aiobotocore-connectcases-2.5.2.post3/types_aiobotocore_connectcases/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     8583 2023-08-04 12:21:00.000000 types-aiobotocore-connectcases-2.5.2.post3/types_aiobotocore_connectcases/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     3602 2023-08-04 12:21:00.000000 types-aiobotocore-connectcases-2.5.2.post3/types_aiobotocore_connectcases/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     3598 2023-08-04 12:21:00.000000 types-aiobotocore-connectcases-2.5.2.post3/types_aiobotocore_connectcases/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 12:20:59.000000 types-aiobotocore-connectcases-2.5.2.post3/types_aiobotocore_connectcases/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    29470 2023-08-04 12:21:00.000000 types-aiobotocore-connectcases-2.5.2.post3/types_aiobotocore_connectcases/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    29426 2023-08-04 12:21:00.000000 types-aiobotocore-connectcases-2.5.2.post3/types_aiobotocore_connectcases/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-04 12:20:59.000000 types-aiobotocore-connectcases-2.5.2.post3/types_aiobotocore_connectcases/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:37:31.695526 types-aiobotocore-connectcases-2.5.2.post3/types_aiobotocore_connectcases.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    13361 2023-08-04 12:37:31.000000 types-aiobotocore-connectcases-2.5.2.post3/types_aiobotocore_connectcases.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      908 2023-08-04 12:37:31.000000 types-aiobotocore-connectcases-2.5.2.post3/types_aiobotocore_connectcases.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 12:37:31.000000 types-aiobotocore-connectcases-2.5.2.post3/types_aiobotocore_connectcases.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 12:37:31.000000 types-aiobotocore-connectcases-2.5.2.post3/types_aiobotocore_connectcases.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-04 12:37:31.000000 types-aiobotocore-connectcases-2.5.2.post3/types_aiobotocore_connectcases.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-08-04 12:37:31.000000 types-aiobotocore-connectcases-2.5.2.post3/types_aiobotocore_connectcases.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:23:33.558676 types-aiobotocore-connectcases-2.5.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-08 01:08:36.000000 types-aiobotocore-connectcases-2.5.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    13355 2023-08-08 01:23:33.554676 types-aiobotocore-connectcases-2.5.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    11823 2023-08-08 01:08:36.000000 types-aiobotocore-connectcases-2.5.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-08 01:23:33.558676 types-aiobotocore-connectcases-2.5.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2101 2023-08-08 01:08:36.000000 types-aiobotocore-connectcases-2.5.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:23:33.550676 types-aiobotocore-connectcases-2.5.4/types_aiobotocore_connectcases/
+-rw-r--r--   0 runner    (1001) docker     (123)      877 2023-08-08 01:08:36.000000 types-aiobotocore-connectcases-2.5.4/types_aiobotocore_connectcases/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      876 2023-08-08 01:08:36.000000 types-aiobotocore-connectcases-2.5.4/types_aiobotocore_connectcases/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      951 2023-08-08 01:08:36.000000 types-aiobotocore-connectcases-2.5.4/types_aiobotocore_connectcases/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23891 2023-08-08 01:08:36.000000 types-aiobotocore-connectcases-2.5.4/types_aiobotocore_connectcases/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23850 2023-08-08 01:08:36.000000 types-aiobotocore-connectcases-2.5.4/types_aiobotocore_connectcases/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8680 2023-08-08 01:08:37.000000 types-aiobotocore-connectcases-2.5.4/types_aiobotocore_connectcases/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8678 2023-08-08 01:08:37.000000 types-aiobotocore-connectcases-2.5.4/types_aiobotocore_connectcases/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     3602 2023-08-08 01:08:36.000000 types-aiobotocore-connectcases-2.5.4/types_aiobotocore_connectcases/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3598 2023-08-08 01:08:36.000000 types-aiobotocore-connectcases-2.5.4/types_aiobotocore_connectcases/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 01:08:36.000000 types-aiobotocore-connectcases-2.5.4/types_aiobotocore_connectcases/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    29554 2023-08-08 01:08:37.000000 types-aiobotocore-connectcases-2.5.4/types_aiobotocore_connectcases/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29510 2023-08-08 01:08:37.000000 types-aiobotocore-connectcases-2.5.4/types_aiobotocore_connectcases/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-08-08 01:08:36.000000 types-aiobotocore-connectcases-2.5.4/types_aiobotocore_connectcases/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:23:33.554676 types-aiobotocore-connectcases-2.5.4/types_aiobotocore_connectcases.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    13355 2023-08-08 01:23:33.000000 types-aiobotocore-connectcases-2.5.4/types_aiobotocore_connectcases.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      908 2023-08-08 01:23:33.000000 types-aiobotocore-connectcases-2.5.4/types_aiobotocore_connectcases.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 01:23:33.000000 types-aiobotocore-connectcases-2.5.4/types_aiobotocore_connectcases.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 01:23:33.000000 types-aiobotocore-connectcases-2.5.4/types_aiobotocore_connectcases.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-08 01:23:33.000000 types-aiobotocore-connectcases-2.5.4/types_aiobotocore_connectcases.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-08-08 01:23:33.000000 types-aiobotocore-connectcases-2.5.4/types_aiobotocore_connectcases.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-connectcases-2.5.2.post3/LICENSE` & `types-aiobotocore-connectcases-2.5.4/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-connectcases-2.5.2.post3/PKG-INFO` & `types-aiobotocore-connectcases-2.5.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-connectcases
-Version: 2.5.2.post3
-Summary: Type annotations for aiobotocore.ConnectCases 2.5.2 service generated with mypy-boto3-builder 7.17.2
+Version: 2.5.4
+Summary: Type annotations for aiobotocore.ConnectCases 2.5.4 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_connectcases/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-connectcases.svg?color=blue)](https://pypi.org/project/types-aiobotocore-connectcases)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_connectcases/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-connectcases)](https://pepy.tech/project/types-aiobotocore-connectcases)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.ConnectCases 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connectcases.html#ConnectCases)
+[aiobotocore.ConnectCases 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connectcases.html#ConnectCases)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-connectcases-2.5.2.post3/README.md` & `types-aiobotocore-connectcases-2.5.4/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-connectcases.svg?color=blue)](https://pypi.org/project/types-aiobotocore-connectcases)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_connectcases/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-connectcases)](https://pepy.tech/project/types-aiobotocore-connectcases)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.ConnectCases 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connectcases.html#ConnectCases)
+[aiobotocore.ConnectCases 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connectcases.html#ConnectCases)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-connectcases-2.5.2.post3/setup.py` & `types-aiobotocore-connectcases-2.5.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-connectcases",
-    version="2.5.2.post3",
+    version="2.5.4",
     packages=["types_aiobotocore_connectcases"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.ConnectCases 2.5.2 service generated with"
+        "Type annotations for aiobotocore.ConnectCases 2.5.4 service generated with"
         " mypy-boto3-builder 7.17.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
```

### Comparing `types-aiobotocore-connectcases-2.5.2.post3/types_aiobotocore_connectcases/__init__.py` & `types-aiobotocore-connectcases-2.5.4/types_aiobotocore_connectcases/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-connectcases-2.5.2.post3/types_aiobotocore_connectcases/__init__.pyi` & `types-aiobotocore-connectcases-2.5.4/types_aiobotocore_connectcases/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-connectcases-2.5.2.post3/types_aiobotocore_connectcases/__main__.py` & `types-aiobotocore-connectcases-2.5.4/types_aiobotocore_connectcases/__main__.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.ConnectCases 2.5.2\nVersion:         2.5.2.post3\nBuilder"
+        "Type annotations for aiobotocore.ConnectCases 2.5.4\nVersion:         2.5.4\nBuilder"
         " version: 7.17.2\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_connectcases//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connectcases.html#ConnectCases\nOther"
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

### Comparing `types-aiobotocore-connectcases-2.5.2.post3/types_aiobotocore_connectcases/client.py` & `types-aiobotocore-connectcases-2.5.4/types_aiobotocore_connectcases/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -216,15 +216,15 @@
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connectcases.html#ConnectCases.Client.create_template)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_connectcases/client/#create_template)
         """
 
     async def delete_domain(self, *, domainId: str) -> Dict[str, Any]:
         """
-        Deletes a domain.
+        Deletes a Cases domain.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connectcases.html#ConnectCases.Client.delete_domain)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_connectcases/client/#delete_domain)
         """
 
     async def generate_presigned_url(
         self,
```

### Comparing `types-aiobotocore-connectcases-2.5.2.post3/types_aiobotocore_connectcases/client.pyi` & `types-aiobotocore-connectcases-2.5.4/types_aiobotocore_connectcases/client.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -201,15 +201,15 @@
         Creates a template in the Cases domain.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connectcases.html#ConnectCases.Client.create_template)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_connectcases/client/#create_template)
         """
     async def delete_domain(self, *, domainId: str) -> Dict[str, Any]:
         """
-        Deletes a domain.
+        Deletes a Cases domain.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connectcases.html#ConnectCases.Client.delete_domain)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_connectcases/client/#delete_domain)
         """
     async def generate_presigned_url(
         self,
         ClientMethod: str,
```

### Comparing `types-aiobotocore-connectcases-2.5.2.post3/types_aiobotocore_connectcases/literals.py` & `types-aiobotocore-connectcases-2.5.4/types_aiobotocore_connectcases/literals.py`

 * *Files 1% similar despite different names*

```diff
@@ -58,14 +58,15 @@
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
@@ -161,14 +162,15 @@
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
@@ -247,26 +249,28 @@
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

### Comparing `types-aiobotocore-connectcases-2.5.2.post3/types_aiobotocore_connectcases/literals.pyi` & `types-aiobotocore-connectcases-2.5.4/types_aiobotocore_connectcases/literals.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -56,14 +56,15 @@
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
@@ -159,14 +160,15 @@
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
@@ -245,26 +247,28 @@
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

### Comparing `types-aiobotocore-connectcases-2.5.2.post3/types_aiobotocore_connectcases/paginator.py` & `types-aiobotocore-connectcases-2.5.4/types_aiobotocore_connectcases/paginator.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-connectcases-2.5.2.post3/types_aiobotocore_connectcases/paginator.pyi` & `types-aiobotocore-connectcases-2.5.4/types_aiobotocore_connectcases/paginator.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-connectcases-2.5.2.post3/types_aiobotocore_connectcases/type_defs.py` & `types-aiobotocore-connectcases-2.5.4/types_aiobotocore_connectcases/type_defs.py`

 * *Files 0% similar despite different names*

```diff
@@ -338,14 +338,15 @@
 )
 
 FieldValueUnionTypeDef = TypedDict(
     "FieldValueUnionTypeDef",
     {
         "booleanValue": bool,
         "doubleValue": float,
+        "emptyValue": Mapping[str, Any],
         "stringValue": str,
     },
     total=False,
 )
 
 GetCaseEventConfigurationRequestRequestTypeDef = TypedDict(
     "GetCaseEventConfigurationRequestRequestTypeDef",
@@ -1176,14 +1177,15 @@
 
 CaseFilterTypeDef = TypedDict(
     "CaseFilterTypeDef",
     {
         "andAll": Sequence[Dict[str, Any]],
         "field": FieldFilterTypeDef,
         "not": Dict[str, Any],
+        "orAll": Sequence[Dict[str, Any]],
     },
     total=False,
 )
 
 SearchCasesResponseTypeDef = TypedDict(
     "SearchCasesResponseTypeDef",
     {
```

### Comparing `types-aiobotocore-connectcases-2.5.2.post3/types_aiobotocore_connectcases/type_defs.pyi` & `types-aiobotocore-connectcases-2.5.4/types_aiobotocore_connectcases/type_defs.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -331,14 +331,15 @@
 )
 
 FieldValueUnionTypeDef = TypedDict(
     "FieldValueUnionTypeDef",
     {
         "booleanValue": bool,
         "doubleValue": float,
+        "emptyValue": Mapping[str, Any],
         "stringValue": str,
     },
     total=False,
 )
 
 GetCaseEventConfigurationRequestRequestTypeDef = TypedDict(
     "GetCaseEventConfigurationRequestRequestTypeDef",
@@ -1133,14 +1134,15 @@
 
 CaseFilterTypeDef = TypedDict(
     "CaseFilterTypeDef",
     {
         "andAll": Sequence[Dict[str, Any]],
         "field": FieldFilterTypeDef,
         "not": Dict[str, Any],
+        "orAll": Sequence[Dict[str, Any]],
     },
     total=False,
 )
 
 SearchCasesResponseTypeDef = TypedDict(
     "SearchCasesResponseTypeDef",
     {
```

### Comparing `types-aiobotocore-connectcases-2.5.2.post3/types_aiobotocore_connectcases.egg-info/PKG-INFO` & `types-aiobotocore-connectcases-2.5.4/types_aiobotocore_connectcases.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-connectcases
-Version: 2.5.2.post3
-Summary: Type annotations for aiobotocore.ConnectCases 2.5.2 service generated with mypy-boto3-builder 7.17.2
+Version: 2.5.4
+Summary: Type annotations for aiobotocore.ConnectCases 2.5.4 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_connectcases/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-connectcases.svg?color=blue)](https://pypi.org/project/types-aiobotocore-connectcases)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_connectcases/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-connectcases)](https://pepy.tech/project/types-aiobotocore-connectcases)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.ConnectCases 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connectcases.html#ConnectCases)
+[aiobotocore.ConnectCases 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connectcases.html#ConnectCases)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-connectcases-2.5.2.post3/types_aiobotocore_connectcases.egg-info/SOURCES.txt` & `types-aiobotocore-connectcases-2.5.4/types_aiobotocore_connectcases.egg-info/SOURCES.txt`

 * *Files identical despite different names*


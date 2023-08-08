# Comparing `tmp/types-aiobotocore-elbv2-2.5.2.post3.tar.gz` & `tmp/types-aiobotocore-elbv2-2.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-elbv2-2.5.2.post3.tar", last modified: Fri Aug  4 12:37:41 2023, max compression
+gzip compressed data, was "types-aiobotocore-elbv2-2.5.4.tar", last modified: Tue Aug  8 01:23:41 2023, max compression
```

## Comparing `types-aiobotocore-elbv2-2.5.2.post3.tar` & `types-aiobotocore-elbv2-2.5.4.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:37:41.695764 types-aiobotocore-elbv2-2.5.2.post3/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-04 12:23:23.000000 types-aiobotocore-elbv2-2.5.2.post3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    15335 2023-08-04 12:37:41.691764 types-aiobotocore-elbv2-2.5.2.post3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    13808 2023-08-04 12:23:23.000000 types-aiobotocore-elbv2-2.5.2.post3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-04 12:37:41.695764 types-aiobotocore-elbv2-2.5.2.post3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2075 2023-08-04 12:23:23.000000 types-aiobotocore-elbv2-2.5.2.post3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:37:41.687764 types-aiobotocore-elbv2-2.5.2.post3/types_aiobotocore_elbv2/
--rw-r--r--   0 runner    (1001) docker     (123)     3161 2023-08-04 12:23:23.000000 types-aiobotocore-elbv2-2.5.2.post3/types_aiobotocore_elbv2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3160 2023-08-04 12:23:23.000000 types-aiobotocore-elbv2-2.5.2.post3/types_aiobotocore_elbv2/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      958 2023-08-04 12:23:23.000000 types-aiobotocore-elbv2-2.5.2.post3/types_aiobotocore_elbv2/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    35950 2023-08-04 12:23:23.000000 types-aiobotocore-elbv2-2.5.2.post3/types_aiobotocore_elbv2/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    35895 2023-08-04 12:23:23.000000 types-aiobotocore-elbv2-2.5.2.post3/types_aiobotocore_elbv2/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    11662 2023-08-04 12:23:24.000000 types-aiobotocore-elbv2-2.5.2.post3/types_aiobotocore_elbv2/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    11660 2023-08-04 12:23:23.000000 types-aiobotocore-elbv2-2.5.2.post3/types_aiobotocore_elbv2/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9594 2023-08-04 12:23:23.000000 types-aiobotocore-elbv2-2.5.2.post3/types_aiobotocore_elbv2/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     9585 2023-08-04 12:23:23.000000 types-aiobotocore-elbv2-2.5.2.post3/types_aiobotocore_elbv2/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 12:23:23.000000 types-aiobotocore-elbv2-2.5.2.post3/types_aiobotocore_elbv2/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    38622 2023-08-04 12:23:24.000000 types-aiobotocore-elbv2-2.5.2.post3/types_aiobotocore_elbv2/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    38581 2023-08-04 12:23:24.000000 types-aiobotocore-elbv2-2.5.2.post3/types_aiobotocore_elbv2/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-04 12:23:23.000000 types-aiobotocore-elbv2-2.5.2.post3/types_aiobotocore_elbv2/version.py
--rw-r--r--   0 runner    (1001) docker     (123)     6349 2023-08-04 12:23:23.000000 types-aiobotocore-elbv2-2.5.2.post3/types_aiobotocore_elbv2/waiter.py
--rw-r--r--   0 runner    (1001) docker     (123)     6344 2023-08-04 12:23:23.000000 types-aiobotocore-elbv2-2.5.2.post3/types_aiobotocore_elbv2/waiter.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:37:41.691764 types-aiobotocore-elbv2-2.5.2.post3/types_aiobotocore_elbv2.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    15335 2023-08-04 12:37:41.000000 types-aiobotocore-elbv2-2.5.2.post3/types_aiobotocore_elbv2.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      844 2023-08-04 12:37:41.000000 types-aiobotocore-elbv2-2.5.2.post3/types_aiobotocore_elbv2.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 12:37:41.000000 types-aiobotocore-elbv2-2.5.2.post3/types_aiobotocore_elbv2.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 12:37:41.000000 types-aiobotocore-elbv2-2.5.2.post3/types_aiobotocore_elbv2.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-04 12:37:41.000000 types-aiobotocore-elbv2-2.5.2.post3/types_aiobotocore_elbv2.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-08-04 12:37:41.000000 types-aiobotocore-elbv2-2.5.2.post3/types_aiobotocore_elbv2.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:23:41.590707 types-aiobotocore-elbv2-2.5.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-08 01:10:48.000000 types-aiobotocore-elbv2-2.5.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    15329 2023-08-08 01:23:41.590707 types-aiobotocore-elbv2-2.5.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    13808 2023-08-08 01:10:48.000000 types-aiobotocore-elbv2-2.5.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-08 01:23:41.590707 types-aiobotocore-elbv2-2.5.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2069 2023-08-08 01:10:48.000000 types-aiobotocore-elbv2-2.5.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:23:41.586707 types-aiobotocore-elbv2-2.5.4/types_aiobotocore_elbv2/
+-rw-r--r--   0 runner    (1001) docker     (123)     3161 2023-08-08 01:10:48.000000 types-aiobotocore-elbv2-2.5.4/types_aiobotocore_elbv2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3160 2023-08-08 01:10:48.000000 types-aiobotocore-elbv2-2.5.4/types_aiobotocore_elbv2/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      946 2023-08-08 01:10:48.000000 types-aiobotocore-elbv2-2.5.4/types_aiobotocore_elbv2/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35950 2023-08-08 01:10:49.000000 types-aiobotocore-elbv2-2.5.4/types_aiobotocore_elbv2/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35895 2023-08-08 01:10:48.000000 types-aiobotocore-elbv2-2.5.4/types_aiobotocore_elbv2/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    11777 2023-08-08 01:10:49.000000 types-aiobotocore-elbv2-2.5.4/types_aiobotocore_elbv2/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11775 2023-08-08 01:10:49.000000 types-aiobotocore-elbv2-2.5.4/types_aiobotocore_elbv2/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9594 2023-08-08 01:10:49.000000 types-aiobotocore-elbv2-2.5.4/types_aiobotocore_elbv2/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9585 2023-08-08 01:10:49.000000 types-aiobotocore-elbv2-2.5.4/types_aiobotocore_elbv2/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 01:10:48.000000 types-aiobotocore-elbv2-2.5.4/types_aiobotocore_elbv2/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    38622 2023-08-08 01:10:50.000000 types-aiobotocore-elbv2-2.5.4/types_aiobotocore_elbv2/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38581 2023-08-08 01:10:49.000000 types-aiobotocore-elbv2-2.5.4/types_aiobotocore_elbv2/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-08-08 01:10:48.000000 types-aiobotocore-elbv2-2.5.4/types_aiobotocore_elbv2/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6349 2023-08-08 01:10:49.000000 types-aiobotocore-elbv2-2.5.4/types_aiobotocore_elbv2/waiter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6344 2023-08-08 01:10:49.000000 types-aiobotocore-elbv2-2.5.4/types_aiobotocore_elbv2/waiter.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:23:41.590707 types-aiobotocore-elbv2-2.5.4/types_aiobotocore_elbv2.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    15329 2023-08-08 01:23:41.000000 types-aiobotocore-elbv2-2.5.4/types_aiobotocore_elbv2.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      844 2023-08-08 01:23:41.000000 types-aiobotocore-elbv2-2.5.4/types_aiobotocore_elbv2.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 01:23:41.000000 types-aiobotocore-elbv2-2.5.4/types_aiobotocore_elbv2.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 01:23:41.000000 types-aiobotocore-elbv2-2.5.4/types_aiobotocore_elbv2.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-08 01:23:41.000000 types-aiobotocore-elbv2-2.5.4/types_aiobotocore_elbv2.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-08-08 01:23:41.000000 types-aiobotocore-elbv2-2.5.4/types_aiobotocore_elbv2.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-elbv2-2.5.2.post3/LICENSE` & `types-aiobotocore-elbv2-2.5.4/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-elbv2-2.5.2.post3/PKG-INFO` & `types-aiobotocore-elbv2-2.5.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-elbv2
-Version: 2.5.2.post3
-Summary: Type annotations for aiobotocore.ElasticLoadBalancingv2 2.5.2 service generated with mypy-boto3-builder 7.17.2
+Version: 2.5.4
+Summary: Type annotations for aiobotocore.ElasticLoadBalancingv2 2.5.4 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elbv2/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-elbv2.svg?color=blue)](https://pypi.org/project/types-aiobotocore-elbv2)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elbv2/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-elbv2)](https://pepy.tech/project/types-aiobotocore-elbv2)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.ElasticLoadBalancingv2 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elbv2.html#ElasticLoadBalancingv2)
+[aiobotocore.ElasticLoadBalancingv2 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elbv2.html#ElasticLoadBalancingv2)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-elbv2-2.5.2.post3/README.md` & `types-aiobotocore-elbv2-2.5.4/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-elbv2.svg?color=blue)](https://pypi.org/project/types-aiobotocore-elbv2)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elbv2/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-elbv2)](https://pepy.tech/project/types-aiobotocore-elbv2)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.ElasticLoadBalancingv2 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elbv2.html#ElasticLoadBalancingv2)
+[aiobotocore.ElasticLoadBalancingv2 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elbv2.html#ElasticLoadBalancingv2)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-elbv2-2.5.2.post3/setup.py` & `types-aiobotocore-elbv2-2.5.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-elbv2",
-    version="2.5.2.post3",
+    version="2.5.4",
     packages=["types_aiobotocore_elbv2"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.ElasticLoadBalancingv2 2.5.2 service generated with"
+        "Type annotations for aiobotocore.ElasticLoadBalancingv2 2.5.4 service generated with"
         " mypy-boto3-builder 7.17.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
```

### Comparing `types-aiobotocore-elbv2-2.5.2.post3/types_aiobotocore_elbv2/__init__.py` & `types-aiobotocore-elbv2-2.5.4/types_aiobotocore_elbv2/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-elbv2-2.5.2.post3/types_aiobotocore_elbv2/__init__.pyi` & `types-aiobotocore-elbv2-2.5.4/types_aiobotocore_elbv2/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-elbv2-2.5.2.post3/types_aiobotocore_elbv2/__main__.py` & `types-aiobotocore-elbv2-2.5.4/types_aiobotocore_elbv2/__main__.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.ElasticLoadBalancingv2 2.5.2\nVersion:        "
-        " 2.5.2.post3\nBuilder version: 7.17.2\nDocs:           "
+        "Type annotations for aiobotocore.ElasticLoadBalancingv2 2.5.4\nVersion:        "
+        " 2.5.4\nBuilder version: 7.17.2\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elbv2//\nBoto3 docs:  "
         "    https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elbv2.html#ElasticLoadBalancingv2\nOther"
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

### Comparing `types-aiobotocore-elbv2-2.5.2.post3/types_aiobotocore_elbv2/client.py` & `types-aiobotocore-elbv2-2.5.4/types_aiobotocore_elbv2/client.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-elbv2-2.5.2.post3/types_aiobotocore_elbv2/client.pyi` & `types-aiobotocore-elbv2-2.5.4/types_aiobotocore_elbv2/client.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-elbv2-2.5.2.post3/types_aiobotocore_elbv2/literals.py` & `types-aiobotocore-elbv2-2.5.4/types_aiobotocore_elbv2/literals.pyi`

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
     "ActionTypeEnumType",
     "AuthenticateCognitoActionConditionalBehaviorEnumType",
     "AuthenticateOidcActionConditionalBehaviorEnumType",
     "DescribeAccountLimitsPaginatorName",
     "DescribeListenerCertificatesPaginatorName",
     "DescribeListenersPaginatorName",
@@ -49,15 +48,14 @@
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "WaiterName",
     "RegionName",
 )
 
-
 ActionTypeEnumType = Literal[
     "authenticate-cognito", "authenticate-oidc", "fixed-response", "forward", "redirect"
 ]
 AuthenticateCognitoActionConditionalBehaviorEnumType = Literal["allow", "authenticate", "deny"]
 AuthenticateOidcActionConditionalBehaviorEnumType = Literal["allow", "authenticate", "deny"]
 DescribeAccountLimitsPaginatorName = Literal["describe_account_limits"]
 DescribeListenerCertificatesPaginatorName = Literal["describe_listener_certificates"]
@@ -108,14 +106,15 @@
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
@@ -211,14 +210,15 @@
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
@@ -297,26 +297,28 @@
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
@@ -493,14 +495,15 @@
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

### Comparing `types-aiobotocore-elbv2-2.5.2.post3/types_aiobotocore_elbv2/literals.pyi` & `types-aiobotocore-elbv2-2.5.4/types_aiobotocore_elbv2/literals.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 import sys
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
+
 __all__ = (
     "ActionTypeEnumType",
     "AuthenticateCognitoActionConditionalBehaviorEnumType",
     "AuthenticateOidcActionConditionalBehaviorEnumType",
     "DescribeAccountLimitsPaginatorName",
     "DescribeListenerCertificatesPaginatorName",
     "DescribeListenersPaginatorName",
@@ -48,14 +49,15 @@
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "WaiterName",
     "RegionName",
 )
 
+
 ActionTypeEnumType = Literal[
     "authenticate-cognito", "authenticate-oidc", "fixed-response", "forward", "redirect"
 ]
 AuthenticateCognitoActionConditionalBehaviorEnumType = Literal["allow", "authenticate", "deny"]
 AuthenticateOidcActionConditionalBehaviorEnumType = Literal["allow", "authenticate", "deny"]
 DescribeAccountLimitsPaginatorName = Literal["describe_account_limits"]
 DescribeListenerCertificatesPaginatorName = Literal["describe_listener_certificates"]
@@ -106,14 +108,15 @@
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
@@ -209,14 +212,15 @@
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
@@ -295,26 +299,28 @@
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
@@ -491,14 +497,15 @@
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

### Comparing `types-aiobotocore-elbv2-2.5.2.post3/types_aiobotocore_elbv2/paginator.py` & `types-aiobotocore-elbv2-2.5.4/types_aiobotocore_elbv2/paginator.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-elbv2-2.5.2.post3/types_aiobotocore_elbv2/paginator.pyi` & `types-aiobotocore-elbv2-2.5.4/types_aiobotocore_elbv2/paginator.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-elbv2-2.5.2.post3/types_aiobotocore_elbv2/type_defs.py` & `types-aiobotocore-elbv2-2.5.4/types_aiobotocore_elbv2/type_defs.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-elbv2-2.5.2.post3/types_aiobotocore_elbv2/type_defs.pyi` & `types-aiobotocore-elbv2-2.5.4/types_aiobotocore_elbv2/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-elbv2-2.5.2.post3/types_aiobotocore_elbv2/waiter.py` & `types-aiobotocore-elbv2-2.5.4/types_aiobotocore_elbv2/waiter.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-elbv2-2.5.2.post3/types_aiobotocore_elbv2/waiter.pyi` & `types-aiobotocore-elbv2-2.5.4/types_aiobotocore_elbv2/waiter.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-elbv2-2.5.2.post3/types_aiobotocore_elbv2.egg-info/PKG-INFO` & `types-aiobotocore-elbv2-2.5.4/types_aiobotocore_elbv2.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-elbv2
-Version: 2.5.2.post3
-Summary: Type annotations for aiobotocore.ElasticLoadBalancingv2 2.5.2 service generated with mypy-boto3-builder 7.17.2
+Version: 2.5.4
+Summary: Type annotations for aiobotocore.ElasticLoadBalancingv2 2.5.4 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elbv2/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-elbv2.svg?color=blue)](https://pypi.org/project/types-aiobotocore-elbv2)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elbv2/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-elbv2)](https://pepy.tech/project/types-aiobotocore-elbv2)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.ElasticLoadBalancingv2 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elbv2.html#ElasticLoadBalancingv2)
+[aiobotocore.ElasticLoadBalancingv2 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elbv2.html#ElasticLoadBalancingv2)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-elbv2-2.5.2.post3/types_aiobotocore_elbv2.egg-info/SOURCES.txt` & `types-aiobotocore-elbv2-2.5.4/types_aiobotocore_elbv2.egg-info/SOURCES.txt`

 * *Files identical despite different names*


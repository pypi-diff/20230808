# Comparing `tmp/types-aiobotocore-amp-2.5.2.post3.tar.gz` & `tmp/types-aiobotocore-amp-2.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-amp-2.5.2.post3.tar", last modified: Fri Aug  4 12:37:13 2023, max compression
+gzip compressed data, was "types-aiobotocore-amp-2.5.4.tar", last modified: Tue Aug  8 01:23:11 2023, max compression
```

## Comparing `types-aiobotocore-amp-2.5.2.post3.tar` & `types-aiobotocore-amp-2.5.4.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:37:13.475096 types-aiobotocore-amp-2.5.2.post3/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-04 12:17:57.000000 types-aiobotocore-amp-2.5.2.post3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    13883 2023-08-04 12:37:13.471096 types-aiobotocore-amp-2.5.2.post3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    12367 2023-08-04 12:17:57.000000 types-aiobotocore-amp-2.5.2.post3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-04 12:37:13.475096 types-aiobotocore-amp-2.5.2.post3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2034 2023-08-04 12:17:57.000000 types-aiobotocore-amp-2.5.2.post3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:37:13.459095 types-aiobotocore-amp-2.5.2.post3/types_aiobotocore_amp/
--rw-r--r--   0 runner    (1001) docker     (123)     1324 2023-08-04 12:17:57.000000 types-aiobotocore-amp-2.5.2.post3/types_aiobotocore_amp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1323 2023-08-04 12:17:57.000000 types-aiobotocore-amp-2.5.2.post3/types_aiobotocore_amp/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      944 2023-08-04 12:17:57.000000 types-aiobotocore-amp-2.5.2.post3/types_aiobotocore_amp/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18387 2023-08-04 12:17:57.000000 types-aiobotocore-amp-2.5.2.post3/types_aiobotocore_amp/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    18353 2023-08-04 12:17:57.000000 types-aiobotocore-amp-2.5.2.post3/types_aiobotocore_amp/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9093 2023-08-04 12:17:57.000000 types-aiobotocore-amp-2.5.2.post3/types_aiobotocore_amp/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     9091 2023-08-04 12:17:57.000000 types-aiobotocore-amp-2.5.2.post3/types_aiobotocore_amp/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     3230 2023-08-04 12:17:57.000000 types-aiobotocore-amp-2.5.2.post3/types_aiobotocore_amp/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     3226 2023-08-04 12:17:57.000000 types-aiobotocore-amp-2.5.2.post3/types_aiobotocore_amp/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 12:17:57.000000 types-aiobotocore-amp-2.5.2.post3/types_aiobotocore_amp/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    22689 2023-08-04 12:17:58.000000 types-aiobotocore-amp-2.5.2.post3/types_aiobotocore_amp/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    22644 2023-08-04 12:17:57.000000 types-aiobotocore-amp-2.5.2.post3/types_aiobotocore_amp/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-04 12:17:57.000000 types-aiobotocore-amp-2.5.2.post3/types_aiobotocore_amp/version.py
--rw-r--r--   0 runner    (1001) docker     (123)     2493 2023-08-04 12:17:57.000000 types-aiobotocore-amp-2.5.2.post3/types_aiobotocore_amp/waiter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2491 2023-08-04 12:17:57.000000 types-aiobotocore-amp-2.5.2.post3/types_aiobotocore_amp/waiter.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:37:13.471096 types-aiobotocore-amp-2.5.2.post3/types_aiobotocore_amp.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    13883 2023-08-04 12:37:13.000000 types-aiobotocore-amp-2.5.2.post3/types_aiobotocore_amp.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      802 2023-08-04 12:37:13.000000 types-aiobotocore-amp-2.5.2.post3/types_aiobotocore_amp.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 12:37:13.000000 types-aiobotocore-amp-2.5.2.post3/types_aiobotocore_amp.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 12:37:13.000000 types-aiobotocore-amp-2.5.2.post3/types_aiobotocore_amp.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-04 12:37:13.000000 types-aiobotocore-amp-2.5.2.post3/types_aiobotocore_amp.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-08-04 12:37:13.000000 types-aiobotocore-amp-2.5.2.post3/types_aiobotocore_amp.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:23:11.862483 types-aiobotocore-amp-2.5.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-08 01:05:45.000000 types-aiobotocore-amp-2.5.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    13877 2023-08-08 01:23:11.858482 types-aiobotocore-amp-2.5.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    12367 2023-08-08 01:05:45.000000 types-aiobotocore-amp-2.5.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-08 01:23:11.862483 types-aiobotocore-amp-2.5.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2028 2023-08-08 01:05:45.000000 types-aiobotocore-amp-2.5.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:23:11.858482 types-aiobotocore-amp-2.5.4/types_aiobotocore_amp/
+-rw-r--r--   0 runner    (1001) docker     (123)     1324 2023-08-08 01:05:45.000000 types-aiobotocore-amp-2.5.4/types_aiobotocore_amp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1323 2023-08-08 01:05:45.000000 types-aiobotocore-amp-2.5.4/types_aiobotocore_amp/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      932 2023-08-08 01:05:45.000000 types-aiobotocore-amp-2.5.4/types_aiobotocore_amp/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18387 2023-08-08 01:05:45.000000 types-aiobotocore-amp-2.5.4/types_aiobotocore_amp/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18353 2023-08-08 01:05:45.000000 types-aiobotocore-amp-2.5.4/types_aiobotocore_amp/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9188 2023-08-08 01:05:45.000000 types-aiobotocore-amp-2.5.4/types_aiobotocore_amp/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9186 2023-08-08 01:05:45.000000 types-aiobotocore-amp-2.5.4/types_aiobotocore_amp/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     3230 2023-08-08 01:05:45.000000 types-aiobotocore-amp-2.5.4/types_aiobotocore_amp/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3226 2023-08-08 01:05:45.000000 types-aiobotocore-amp-2.5.4/types_aiobotocore_amp/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 01:05:45.000000 types-aiobotocore-amp-2.5.4/types_aiobotocore_amp/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    22689 2023-08-08 01:05:45.000000 types-aiobotocore-amp-2.5.4/types_aiobotocore_amp/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22644 2023-08-08 01:05:45.000000 types-aiobotocore-amp-2.5.4/types_aiobotocore_amp/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-08-08 01:05:45.000000 types-aiobotocore-amp-2.5.4/types_aiobotocore_amp/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2493 2023-08-08 01:05:45.000000 types-aiobotocore-amp-2.5.4/types_aiobotocore_amp/waiter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2491 2023-08-08 01:05:45.000000 types-aiobotocore-amp-2.5.4/types_aiobotocore_amp/waiter.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:23:11.858482 types-aiobotocore-amp-2.5.4/types_aiobotocore_amp.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    13877 2023-08-08 01:23:11.000000 types-aiobotocore-amp-2.5.4/types_aiobotocore_amp.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      802 2023-08-08 01:23:11.000000 types-aiobotocore-amp-2.5.4/types_aiobotocore_amp.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 01:23:11.000000 types-aiobotocore-amp-2.5.4/types_aiobotocore_amp.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 01:23:11.000000 types-aiobotocore-amp-2.5.4/types_aiobotocore_amp.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-08 01:23:11.000000 types-aiobotocore-amp-2.5.4/types_aiobotocore_amp.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-08-08 01:23:11.000000 types-aiobotocore-amp-2.5.4/types_aiobotocore_amp.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-amp-2.5.2.post3/LICENSE` & `types-aiobotocore-amp-2.5.4/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-amp-2.5.2.post3/PKG-INFO` & `types-aiobotocore-amp-2.5.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-amp
-Version: 2.5.2.post3
-Summary: Type annotations for aiobotocore.PrometheusService 2.5.2 service generated with mypy-boto3-builder 7.17.2
+Version: 2.5.4
+Summary: Type annotations for aiobotocore.PrometheusService 2.5.4 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_amp/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-amp.svg?color=blue)](https://pypi.org/project/types-aiobotocore-amp)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_amp/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-amp)](https://pepy.tech/project/types-aiobotocore-amp)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.PrometheusService 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amp.html#PrometheusService)
+[aiobotocore.PrometheusService 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amp.html#PrometheusService)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-amp-2.5.2.post3/README.md` & `types-aiobotocore-amp-2.5.4/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-amp.svg?color=blue)](https://pypi.org/project/types-aiobotocore-amp)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_amp/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-amp)](https://pepy.tech/project/types-aiobotocore-amp)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.PrometheusService 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amp.html#PrometheusService)
+[aiobotocore.PrometheusService 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amp.html#PrometheusService)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-amp-2.5.2.post3/setup.py` & `types-aiobotocore-amp-2.5.4/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-amp",
-    version="2.5.2.post3",
+    version="2.5.4",
     packages=["types_aiobotocore_amp"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.PrometheusService 2.5.2 service generated with"
+        "Type annotations for aiobotocore.PrometheusService 2.5.4 service generated with"
         " mypy-boto3-builder 7.17.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
```

### Comparing `types-aiobotocore-amp-2.5.2.post3/types_aiobotocore_amp/__init__.py` & `types-aiobotocore-amp-2.5.4/types_aiobotocore_amp/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-amp-2.5.2.post3/types_aiobotocore_amp/__init__.pyi` & `types-aiobotocore-amp-2.5.4/types_aiobotocore_amp/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-amp-2.5.2.post3/types_aiobotocore_amp/__main__.py` & `types-aiobotocore-amp-2.5.4/types_aiobotocore_amp/__main__.py`

 * *Files 9% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.PrometheusService 2.5.2\nVersion:        "
-        " 2.5.2.post3\nBuilder version: 7.17.2\nDocs:           "
+        "Type annotations for aiobotocore.PrometheusService 2.5.4\nVersion:         2.5.4\nBuilder"
+        " version: 7.17.2\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_amp//\nBoto3 docs:    "
         "  https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amp.html#PrometheusService\nOther"
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

### Comparing `types-aiobotocore-amp-2.5.2.post3/types_aiobotocore_amp/client.py` & `types-aiobotocore-amp-2.5.4/types_aiobotocore_amp/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -99,39 +99,39 @@
         Closes underlying endpoint connections.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amp.html#PrometheusService.Client.close)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_amp/client/#close)
         """
 
     async def create_alert_manager_definition(
-        self, *, data: BlobTypeDef, workspaceId: str, clientToken: str = ...
+        self, *, workspaceId: str, data: BlobTypeDef, clientToken: str = ...
     ) -> CreateAlertManagerDefinitionResponseTypeDef:
         """
         Create an alert manager definition.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amp.html#PrometheusService.Client.create_alert_manager_definition)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_amp/client/#create_alert_manager_definition)
         """
 
     async def create_logging_configuration(
-        self, *, logGroupArn: str, workspaceId: str, clientToken: str = ...
+        self, *, workspaceId: str, logGroupArn: str, clientToken: str = ...
     ) -> CreateLoggingConfigurationResponseTypeDef:
         """
         Create logging configuration.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amp.html#PrometheusService.Client.create_logging_configuration)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_amp/client/#create_logging_configuration)
         """
 
     async def create_rule_groups_namespace(
         self,
         *,
-        data: BlobTypeDef,
-        name: str,
         workspaceId: str,
+        name: str,
+        data: BlobTypeDef,
         clientToken: str = ...,
         tags: Mapping[str, str] = ...
     ) -> CreateRuleGroupsNamespaceResponseTypeDef:
         """
         Create a rule group namespace.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amp.html#PrometheusService.Client.create_rule_groups_namespace)
@@ -165,15 +165,15 @@
         Delete logging configuration.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amp.html#PrometheusService.Client.delete_logging_configuration)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_amp/client/#delete_logging_configuration)
         """
 
     async def delete_rule_groups_namespace(
-        self, *, name: str, workspaceId: str, clientToken: str = ...
+        self, *, workspaceId: str, name: str, clientToken: str = ...
     ) -> EmptyResponseMetadataTypeDef:
         """
         Delete a rule groups namespace.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amp.html#PrometheusService.Client.delete_rule_groups_namespace)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_amp/client/#delete_rule_groups_namespace)
         """
@@ -205,15 +205,15 @@
         Describes logging configuration.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amp.html#PrometheusService.Client.describe_logging_configuration)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_amp/client/#describe_logging_configuration)
         """
 
     async def describe_rule_groups_namespace(
-        self, *, name: str, workspaceId: str
+        self, *, workspaceId: str, name: str
     ) -> DescribeRuleGroupsNamespaceResponseTypeDef:
         """
         Describe a rule groups namespace.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amp.html#PrometheusService.Client.describe_rule_groups_namespace)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_amp/client/#describe_rule_groups_namespace)
         """
@@ -237,15 +237,15 @@
         Generate a presigned url given a client, its method, and arguments.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amp.html#PrometheusService.Client.generate_presigned_url)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_amp/client/#generate_presigned_url)
         """
 
     async def list_rule_groups_namespaces(
-        self, *, workspaceId: str, maxResults: int = ..., name: str = ..., nextToken: str = ...
+        self, *, workspaceId: str, name: str = ..., nextToken: str = ..., maxResults: int = ...
     ) -> ListRuleGroupsNamespacesResponseTypeDef:
         """
         Lists rule groups namespaces.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amp.html#PrometheusService.Client.list_rule_groups_namespaces)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_amp/client/#list_rule_groups_namespaces)
         """
@@ -257,35 +257,35 @@
         Lists the tags you have assigned to the resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amp.html#PrometheusService.Client.list_tags_for_resource)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_amp/client/#list_tags_for_resource)
         """
 
     async def list_workspaces(
-        self, *, alias: str = ..., maxResults: int = ..., nextToken: str = ...
+        self, *, nextToken: str = ..., alias: str = ..., maxResults: int = ...
     ) -> ListWorkspacesResponseTypeDef:
         """
         Lists all AMP workspaces, including workspaces being created or deleted.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amp.html#PrometheusService.Client.list_workspaces)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_amp/client/#list_workspaces)
         """
 
     async def put_alert_manager_definition(
-        self, *, data: BlobTypeDef, workspaceId: str, clientToken: str = ...
+        self, *, workspaceId: str, data: BlobTypeDef, clientToken: str = ...
     ) -> PutAlertManagerDefinitionResponseTypeDef:
         """
         Update an alert manager definition.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amp.html#PrometheusService.Client.put_alert_manager_definition)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_amp/client/#put_alert_manager_definition)
         """
 
     async def put_rule_groups_namespace(
-        self, *, data: BlobTypeDef, name: str, workspaceId: str, clientToken: str = ...
+        self, *, workspaceId: str, name: str, data: BlobTypeDef, clientToken: str = ...
     ) -> PutRuleGroupsNamespaceResponseTypeDef:
         """
         Update a rule groups namespace.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amp.html#PrometheusService.Client.put_rule_groups_namespace)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_amp/client/#put_rule_groups_namespace)
         """
@@ -303,15 +303,15 @@
         Deletes tags from the specified resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amp.html#PrometheusService.Client.untag_resource)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_amp/client/#untag_resource)
         """
 
     async def update_logging_configuration(
-        self, *, logGroupArn: str, workspaceId: str, clientToken: str = ...
+        self, *, workspaceId: str, logGroupArn: str, clientToken: str = ...
     ) -> UpdateLoggingConfigurationResponseTypeDef:
         """
         Update logging configuration.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amp.html#PrometheusService.Client.update_logging_configuration)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_amp/client/#update_logging_configuration)
         """
```

### Comparing `types-aiobotocore-amp-2.5.2.post3/types_aiobotocore_amp/client.pyi` & `types-aiobotocore-amp-2.5.4/types_aiobotocore_amp/client.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -92,37 +92,37 @@
         """
         Closes underlying endpoint connections.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amp.html#PrometheusService.Client.close)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_amp/client/#close)
         """
     async def create_alert_manager_definition(
-        self, *, data: BlobTypeDef, workspaceId: str, clientToken: str = ...
+        self, *, workspaceId: str, data: BlobTypeDef, clientToken: str = ...
     ) -> CreateAlertManagerDefinitionResponseTypeDef:
         """
         Create an alert manager definition.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amp.html#PrometheusService.Client.create_alert_manager_definition)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_amp/client/#create_alert_manager_definition)
         """
     async def create_logging_configuration(
-        self, *, logGroupArn: str, workspaceId: str, clientToken: str = ...
+        self, *, workspaceId: str, logGroupArn: str, clientToken: str = ...
     ) -> CreateLoggingConfigurationResponseTypeDef:
         """
         Create logging configuration.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amp.html#PrometheusService.Client.create_logging_configuration)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_amp/client/#create_logging_configuration)
         """
     async def create_rule_groups_namespace(
         self,
         *,
-        data: BlobTypeDef,
-        name: str,
         workspaceId: str,
+        name: str,
+        data: BlobTypeDef,
         clientToken: str = ...,
         tags: Mapping[str, str] = ...
     ) -> CreateRuleGroupsNamespaceResponseTypeDef:
         """
         Create a rule group namespace.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amp.html#PrometheusService.Client.create_rule_groups_namespace)
@@ -152,15 +152,15 @@
         """
         Delete logging configuration.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amp.html#PrometheusService.Client.delete_logging_configuration)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_amp/client/#delete_logging_configuration)
         """
     async def delete_rule_groups_namespace(
-        self, *, name: str, workspaceId: str, clientToken: str = ...
+        self, *, workspaceId: str, name: str, clientToken: str = ...
     ) -> EmptyResponseMetadataTypeDef:
         """
         Delete a rule groups namespace.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amp.html#PrometheusService.Client.delete_rule_groups_namespace)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_amp/client/#delete_rule_groups_namespace)
         """
@@ -188,15 +188,15 @@
         """
         Describes logging configuration.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amp.html#PrometheusService.Client.describe_logging_configuration)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_amp/client/#describe_logging_configuration)
         """
     async def describe_rule_groups_namespace(
-        self, *, name: str, workspaceId: str
+        self, *, workspaceId: str, name: str
     ) -> DescribeRuleGroupsNamespaceResponseTypeDef:
         """
         Describe a rule groups namespace.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amp.html#PrometheusService.Client.describe_rule_groups_namespace)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_amp/client/#describe_rule_groups_namespace)
         """
@@ -217,15 +217,15 @@
         """
         Generate a presigned url given a client, its method, and arguments.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amp.html#PrometheusService.Client.generate_presigned_url)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_amp/client/#generate_presigned_url)
         """
     async def list_rule_groups_namespaces(
-        self, *, workspaceId: str, maxResults: int = ..., name: str = ..., nextToken: str = ...
+        self, *, workspaceId: str, name: str = ..., nextToken: str = ..., maxResults: int = ...
     ) -> ListRuleGroupsNamespacesResponseTypeDef:
         """
         Lists rule groups namespaces.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amp.html#PrometheusService.Client.list_rule_groups_namespaces)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_amp/client/#list_rule_groups_namespaces)
         """
@@ -235,33 +235,33 @@
         """
         Lists the tags you have assigned to the resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amp.html#PrometheusService.Client.list_tags_for_resource)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_amp/client/#list_tags_for_resource)
         """
     async def list_workspaces(
-        self, *, alias: str = ..., maxResults: int = ..., nextToken: str = ...
+        self, *, nextToken: str = ..., alias: str = ..., maxResults: int = ...
     ) -> ListWorkspacesResponseTypeDef:
         """
         Lists all AMP workspaces, including workspaces being created or deleted.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amp.html#PrometheusService.Client.list_workspaces)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_amp/client/#list_workspaces)
         """
     async def put_alert_manager_definition(
-        self, *, data: BlobTypeDef, workspaceId: str, clientToken: str = ...
+        self, *, workspaceId: str, data: BlobTypeDef, clientToken: str = ...
     ) -> PutAlertManagerDefinitionResponseTypeDef:
         """
         Update an alert manager definition.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amp.html#PrometheusService.Client.put_alert_manager_definition)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_amp/client/#put_alert_manager_definition)
         """
     async def put_rule_groups_namespace(
-        self, *, data: BlobTypeDef, name: str, workspaceId: str, clientToken: str = ...
+        self, *, workspaceId: str, name: str, data: BlobTypeDef, clientToken: str = ...
     ) -> PutRuleGroupsNamespaceResponseTypeDef:
         """
         Update a rule groups namespace.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amp.html#PrometheusService.Client.put_rule_groups_namespace)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_amp/client/#put_rule_groups_namespace)
         """
@@ -276,15 +276,15 @@
         """
         Deletes tags from the specified resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amp.html#PrometheusService.Client.untag_resource)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_amp/client/#untag_resource)
         """
     async def update_logging_configuration(
-        self, *, logGroupArn: str, workspaceId: str, clientToken: str = ...
+        self, *, workspaceId: str, logGroupArn: str, clientToken: str = ...
     ) -> UpdateLoggingConfigurationResponseTypeDef:
         """
         Update logging configuration.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amp.html#PrometheusService.Client.update_logging_configuration)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_amp/client/#update_logging_configuration)
         """
```

### Comparing `types-aiobotocore-amp-2.5.2.post3/types_aiobotocore_amp/literals.py` & `types-aiobotocore-amp-2.5.4/types_aiobotocore_amp/literals.py`

 * *Files 2% similar despite different names*

```diff
@@ -63,14 +63,15 @@
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
@@ -166,14 +167,15 @@
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
@@ -252,26 +254,28 @@
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

### Comparing `types-aiobotocore-amp-2.5.2.post3/types_aiobotocore_amp/literals.pyi` & `types-aiobotocore-amp-2.5.4/types_aiobotocore_amp/literals.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -61,14 +61,15 @@
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
@@ -164,14 +165,15 @@
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
@@ -250,26 +252,28 @@
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

### Comparing `types-aiobotocore-amp-2.5.2.post3/types_aiobotocore_amp/paginator.py` & `types-aiobotocore-amp-2.5.4/types_aiobotocore_amp/paginator.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-amp-2.5.2.post3/types_aiobotocore_amp/paginator.pyi` & `types-aiobotocore-amp-2.5.4/types_aiobotocore_amp/paginator.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-amp-2.5.2.post3/types_aiobotocore_amp/type_defs.py` & `types-aiobotocore-amp-2.5.4/types_aiobotocore_amp/type_defs.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -119,16 +119,16 @@
         "RetryAttempts": int,
     },
 )
 
 _RequiredCreateLoggingConfigurationRequestRequestTypeDef = TypedDict(
     "_RequiredCreateLoggingConfigurationRequestRequestTypeDef",
     {
-        "logGroupArn": str,
         "workspaceId": str,
+        "logGroupArn": str,
     },
 )
 _OptionalCreateLoggingConfigurationRequestRequestTypeDef = TypedDict(
     "_OptionalCreateLoggingConfigurationRequestRequestTypeDef",
     {
         "clientToken": str,
     },
@@ -245,16 +245,16 @@
 ):
     pass
 
 
 _RequiredDeleteRuleGroupsNamespaceRequestRequestTypeDef = TypedDict(
     "_RequiredDeleteRuleGroupsNamespaceRequestRequestTypeDef",
     {
-        "name": str,
         "workspaceId": str,
+        "name": str,
     },
 )
 _OptionalDeleteRuleGroupsNamespaceRequestRequestTypeDef = TypedDict(
     "_OptionalDeleteRuleGroupsNamespaceRequestRequestTypeDef",
     {
         "clientToken": str,
     },
@@ -303,16 +303,16 @@
         "workspaceId": str,
     },
 )
 
 DescribeRuleGroupsNamespaceRequestRequestTypeDef = TypedDict(
     "DescribeRuleGroupsNamespaceRequestRequestTypeDef",
     {
-        "name": str,
         "workspaceId": str,
+        "name": str,
     },
 )
 
 DescribeWorkspaceRequestRequestTypeDef = TypedDict(
     "DescribeWorkspaceRequestRequestTypeDef",
     {
         "workspaceId": str,
@@ -343,17 +343,17 @@
     {
         "workspaceId": str,
     },
 )
 _OptionalListRuleGroupsNamespacesRequestRequestTypeDef = TypedDict(
     "_OptionalListRuleGroupsNamespacesRequestRequestTypeDef",
     {
-        "maxResults": int,
         "name": str,
         "nextToken": str,
+        "maxResults": int,
     },
     total=False,
 )
 
 
 class ListRuleGroupsNamespacesRequestRequestTypeDef(
     _RequiredListRuleGroupsNamespacesRequestRequestTypeDef,
@@ -368,17 +368,17 @@
         "resourceArn": str,
     },
 )
 
 ListWorkspacesRequestRequestTypeDef = TypedDict(
     "ListWorkspacesRequestRequestTypeDef",
     {
+        "nextToken": str,
         "alias": str,
         "maxResults": int,
-        "nextToken": str,
     },
     total=False,
 )
 
 TagResourceRequestRequestTypeDef = TypedDict(
     "TagResourceRequestRequestTypeDef",
     {
@@ -394,16 +394,16 @@
         "tagKeys": Sequence[str],
     },
 )
 
 _RequiredUpdateLoggingConfigurationRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateLoggingConfigurationRequestRequestTypeDef",
     {
-        "logGroupArn": str,
         "workspaceId": str,
+        "logGroupArn": str,
     },
 )
 _OptionalUpdateLoggingConfigurationRequestRequestTypeDef = TypedDict(
     "_OptionalUpdateLoggingConfigurationRequestRequestTypeDef",
     {
         "clientToken": str,
     },
@@ -440,26 +440,26 @@
 ):
     pass
 
 
 AlertManagerDefinitionDescriptionTypeDef = TypedDict(
     "AlertManagerDefinitionDescriptionTypeDef",
     {
-        "createdAt": datetime,
+        "status": AlertManagerDefinitionStatusTypeDef,
         "data": bytes,
+        "createdAt": datetime,
         "modifiedAt": datetime,
-        "status": AlertManagerDefinitionStatusTypeDef,
     },
 )
 
 _RequiredCreateAlertManagerDefinitionRequestRequestTypeDef = TypedDict(
     "_RequiredCreateAlertManagerDefinitionRequestRequestTypeDef",
     {
-        "data": BlobTypeDef,
         "workspaceId": str,
+        "data": BlobTypeDef,
     },
 )
 _OptionalCreateAlertManagerDefinitionRequestRequestTypeDef = TypedDict(
     "_OptionalCreateAlertManagerDefinitionRequestRequestTypeDef",
     {
         "clientToken": str,
     },
@@ -473,17 +473,17 @@
 ):
     pass
 
 
 _RequiredCreateRuleGroupsNamespaceRequestRequestTypeDef = TypedDict(
     "_RequiredCreateRuleGroupsNamespaceRequestRequestTypeDef",
     {
-        "data": BlobTypeDef,
-        "name": str,
         "workspaceId": str,
+        "name": str,
+        "data": BlobTypeDef,
     },
 )
 _OptionalCreateRuleGroupsNamespaceRequestRequestTypeDef = TypedDict(
     "_OptionalCreateRuleGroupsNamespaceRequestRequestTypeDef",
     {
         "clientToken": str,
         "tags": Mapping[str, str],
@@ -498,16 +498,16 @@
 ):
     pass
 
 
 _RequiredPutAlertManagerDefinitionRequestRequestTypeDef = TypedDict(
     "_RequiredPutAlertManagerDefinitionRequestRequestTypeDef",
     {
-        "data": BlobTypeDef,
         "workspaceId": str,
+        "data": BlobTypeDef,
     },
 )
 _OptionalPutAlertManagerDefinitionRequestRequestTypeDef = TypedDict(
     "_OptionalPutAlertManagerDefinitionRequestRequestTypeDef",
     {
         "clientToken": str,
     },
@@ -521,17 +521,17 @@
 ):
     pass
 
 
 _RequiredPutRuleGroupsNamespaceRequestRequestTypeDef = TypedDict(
     "_RequiredPutRuleGroupsNamespaceRequestRequestTypeDef",
     {
-        "data": BlobTypeDef,
-        "name": str,
         "workspaceId": str,
+        "name": str,
+        "data": BlobTypeDef,
     },
 )
 _OptionalPutRuleGroupsNamespaceRequestRequestTypeDef = TypedDict(
     "_OptionalPutRuleGroupsNamespaceRequestRequestTypeDef",
     {
         "clientToken": str,
     },
@@ -584,61 +584,61 @@
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 LoggingConfigurationMetadataTypeDef = TypedDict(
     "LoggingConfigurationMetadataTypeDef",
     {
-        "createdAt": datetime,
-        "logGroupArn": str,
-        "modifiedAt": datetime,
         "status": LoggingConfigurationStatusTypeDef,
         "workspace": str,
+        "logGroupArn": str,
+        "createdAt": datetime,
+        "modifiedAt": datetime,
     },
 )
 
 UpdateLoggingConfigurationResponseTypeDef = TypedDict(
     "UpdateLoggingConfigurationResponseTypeDef",
     {
         "status": LoggingConfigurationStatusTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateRuleGroupsNamespaceResponseTypeDef = TypedDict(
     "CreateRuleGroupsNamespaceResponseTypeDef",
     {
-        "arn": str,
         "name": str,
+        "arn": str,
         "status": RuleGroupsNamespaceStatusTypeDef,
         "tags": Dict[str, str],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 PutRuleGroupsNamespaceResponseTypeDef = TypedDict(
     "PutRuleGroupsNamespaceResponseTypeDef",
     {
-        "arn": str,
         "name": str,
+        "arn": str,
         "status": RuleGroupsNamespaceStatusTypeDef,
         "tags": Dict[str, str],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredRuleGroupsNamespaceDescriptionTypeDef = TypedDict(
     "_RequiredRuleGroupsNamespaceDescriptionTypeDef",
     {
         "arn": str,
-        "createdAt": datetime,
-        "data": bytes,
-        "modifiedAt": datetime,
         "name": str,
         "status": RuleGroupsNamespaceStatusTypeDef,
+        "data": bytes,
+        "createdAt": datetime,
+        "modifiedAt": datetime,
     },
 )
 _OptionalRuleGroupsNamespaceDescriptionTypeDef = TypedDict(
     "_OptionalRuleGroupsNamespaceDescriptionTypeDef",
     {
         "tags": Dict[str, str],
     },
@@ -652,18 +652,18 @@
     pass
 
 
 _RequiredRuleGroupsNamespaceSummaryTypeDef = TypedDict(
     "_RequiredRuleGroupsNamespaceSummaryTypeDef",
     {
         "arn": str,
-        "createdAt": datetime,
-        "modifiedAt": datetime,
         "name": str,
         "status": RuleGroupsNamespaceStatusTypeDef,
+        "createdAt": datetime,
+        "modifiedAt": datetime,
     },
 )
 _OptionalRuleGroupsNamespaceSummaryTypeDef = TypedDict(
     "_OptionalRuleGroupsNamespaceSummaryTypeDef",
     {
         "tags": Dict[str, str],
     },
@@ -676,29 +676,29 @@
 ):
     pass
 
 
 CreateWorkspaceResponseTypeDef = TypedDict(
     "CreateWorkspaceResponseTypeDef",
     {
+        "workspaceId": str,
         "arn": str,
         "status": WorkspaceStatusTypeDef,
         "tags": Dict[str, str],
-        "workspaceId": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredWorkspaceDescriptionTypeDef = TypedDict(
     "_RequiredWorkspaceDescriptionTypeDef",
     {
+        "workspaceId": str,
         "arn": str,
-        "createdAt": datetime,
         "status": WorkspaceStatusTypeDef,
-        "workspaceId": str,
+        "createdAt": datetime,
     },
 )
 _OptionalWorkspaceDescriptionTypeDef = TypedDict(
     "_OptionalWorkspaceDescriptionTypeDef",
     {
         "alias": str,
         "prometheusEndpoint": str,
@@ -713,18 +713,18 @@
 ):
     pass
 
 
 _RequiredWorkspaceSummaryTypeDef = TypedDict(
     "_RequiredWorkspaceSummaryTypeDef",
     {
+        "workspaceId": str,
         "arn": str,
-        "createdAt": datetime,
         "status": WorkspaceStatusTypeDef,
-        "workspaceId": str,
+        "createdAt": datetime,
     },
 )
 _OptionalWorkspaceSummaryTypeDef = TypedDict(
     "_OptionalWorkspaceSummaryTypeDef",
     {
         "alias": str,
         "tags": Dict[str, str],
@@ -836,16 +836,16 @@
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListRuleGroupsNamespacesResponseTypeDef = TypedDict(
     "ListRuleGroupsNamespacesResponseTypeDef",
     {
-        "nextToken": str,
         "ruleGroupsNamespaces": List[RuleGroupsNamespaceSummaryTypeDef],
+        "nextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeWorkspaceResponseTypeDef = TypedDict(
     "DescribeWorkspaceResponseTypeDef",
     {
@@ -853,12 +853,12 @@
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListWorkspacesResponseTypeDef = TypedDict(
     "ListWorkspacesResponseTypeDef",
     {
-        "nextToken": str,
         "workspaces": List[WorkspaceSummaryTypeDef],
+        "nextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `types-aiobotocore-amp-2.5.2.post3/types_aiobotocore_amp/type_defs.pyi` & `types-aiobotocore-amp-2.5.4/types_aiobotocore_amp/type_defs.pyi`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -116,16 +116,16 @@
         "RetryAttempts": int,
     },
 )
 
 _RequiredCreateLoggingConfigurationRequestRequestTypeDef = TypedDict(
     "_RequiredCreateLoggingConfigurationRequestRequestTypeDef",
     {
-        "logGroupArn": str,
         "workspaceId": str,
+        "logGroupArn": str,
     },
 )
 _OptionalCreateLoggingConfigurationRequestRequestTypeDef = TypedDict(
     "_OptionalCreateLoggingConfigurationRequestRequestTypeDef",
     {
         "clientToken": str,
     },
@@ -232,16 +232,16 @@
     _OptionalDeleteLoggingConfigurationRequestRequestTypeDef,
 ):
     pass
 
 _RequiredDeleteRuleGroupsNamespaceRequestRequestTypeDef = TypedDict(
     "_RequiredDeleteRuleGroupsNamespaceRequestRequestTypeDef",
     {
-        "name": str,
         "workspaceId": str,
+        "name": str,
     },
 )
 _OptionalDeleteRuleGroupsNamespaceRequestRequestTypeDef = TypedDict(
     "_OptionalDeleteRuleGroupsNamespaceRequestRequestTypeDef",
     {
         "clientToken": str,
     },
@@ -286,16 +286,16 @@
         "workspaceId": str,
     },
 )
 
 DescribeRuleGroupsNamespaceRequestRequestTypeDef = TypedDict(
     "DescribeRuleGroupsNamespaceRequestRequestTypeDef",
     {
-        "name": str,
         "workspaceId": str,
+        "name": str,
     },
 )
 
 DescribeWorkspaceRequestRequestTypeDef = TypedDict(
     "DescribeWorkspaceRequestRequestTypeDef",
     {
         "workspaceId": str,
@@ -326,17 +326,17 @@
     {
         "workspaceId": str,
     },
 )
 _OptionalListRuleGroupsNamespacesRequestRequestTypeDef = TypedDict(
     "_OptionalListRuleGroupsNamespacesRequestRequestTypeDef",
     {
-        "maxResults": int,
         "name": str,
         "nextToken": str,
+        "maxResults": int,
     },
     total=False,
 )
 
 class ListRuleGroupsNamespacesRequestRequestTypeDef(
     _RequiredListRuleGroupsNamespacesRequestRequestTypeDef,
     _OptionalListRuleGroupsNamespacesRequestRequestTypeDef,
@@ -349,17 +349,17 @@
         "resourceArn": str,
     },
 )
 
 ListWorkspacesRequestRequestTypeDef = TypedDict(
     "ListWorkspacesRequestRequestTypeDef",
     {
+        "nextToken": str,
         "alias": str,
         "maxResults": int,
-        "nextToken": str,
     },
     total=False,
 )
 
 TagResourceRequestRequestTypeDef = TypedDict(
     "TagResourceRequestRequestTypeDef",
     {
@@ -375,16 +375,16 @@
         "tagKeys": Sequence[str],
     },
 )
 
 _RequiredUpdateLoggingConfigurationRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateLoggingConfigurationRequestRequestTypeDef",
     {
-        "logGroupArn": str,
         "workspaceId": str,
+        "logGroupArn": str,
     },
 )
 _OptionalUpdateLoggingConfigurationRequestRequestTypeDef = TypedDict(
     "_OptionalUpdateLoggingConfigurationRequestRequestTypeDef",
     {
         "clientToken": str,
     },
@@ -417,26 +417,26 @@
     _OptionalUpdateWorkspaceAliasRequestRequestTypeDef,
 ):
     pass
 
 AlertManagerDefinitionDescriptionTypeDef = TypedDict(
     "AlertManagerDefinitionDescriptionTypeDef",
     {
-        "createdAt": datetime,
+        "status": AlertManagerDefinitionStatusTypeDef,
         "data": bytes,
+        "createdAt": datetime,
         "modifiedAt": datetime,
-        "status": AlertManagerDefinitionStatusTypeDef,
     },
 )
 
 _RequiredCreateAlertManagerDefinitionRequestRequestTypeDef = TypedDict(
     "_RequiredCreateAlertManagerDefinitionRequestRequestTypeDef",
     {
-        "data": BlobTypeDef,
         "workspaceId": str,
+        "data": BlobTypeDef,
     },
 )
 _OptionalCreateAlertManagerDefinitionRequestRequestTypeDef = TypedDict(
     "_OptionalCreateAlertManagerDefinitionRequestRequestTypeDef",
     {
         "clientToken": str,
     },
@@ -448,17 +448,17 @@
     _OptionalCreateAlertManagerDefinitionRequestRequestTypeDef,
 ):
     pass
 
 _RequiredCreateRuleGroupsNamespaceRequestRequestTypeDef = TypedDict(
     "_RequiredCreateRuleGroupsNamespaceRequestRequestTypeDef",
     {
-        "data": BlobTypeDef,
-        "name": str,
         "workspaceId": str,
+        "name": str,
+        "data": BlobTypeDef,
     },
 )
 _OptionalCreateRuleGroupsNamespaceRequestRequestTypeDef = TypedDict(
     "_OptionalCreateRuleGroupsNamespaceRequestRequestTypeDef",
     {
         "clientToken": str,
         "tags": Mapping[str, str],
@@ -471,16 +471,16 @@
     _OptionalCreateRuleGroupsNamespaceRequestRequestTypeDef,
 ):
     pass
 
 _RequiredPutAlertManagerDefinitionRequestRequestTypeDef = TypedDict(
     "_RequiredPutAlertManagerDefinitionRequestRequestTypeDef",
     {
-        "data": BlobTypeDef,
         "workspaceId": str,
+        "data": BlobTypeDef,
     },
 )
 _OptionalPutAlertManagerDefinitionRequestRequestTypeDef = TypedDict(
     "_OptionalPutAlertManagerDefinitionRequestRequestTypeDef",
     {
         "clientToken": str,
     },
@@ -492,17 +492,17 @@
     _OptionalPutAlertManagerDefinitionRequestRequestTypeDef,
 ):
     pass
 
 _RequiredPutRuleGroupsNamespaceRequestRequestTypeDef = TypedDict(
     "_RequiredPutRuleGroupsNamespaceRequestRequestTypeDef",
     {
-        "data": BlobTypeDef,
-        "name": str,
         "workspaceId": str,
+        "name": str,
+        "data": BlobTypeDef,
     },
 )
 _OptionalPutRuleGroupsNamespaceRequestRequestTypeDef = TypedDict(
     "_OptionalPutRuleGroupsNamespaceRequestRequestTypeDef",
     {
         "clientToken": str,
     },
@@ -553,61 +553,61 @@
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 LoggingConfigurationMetadataTypeDef = TypedDict(
     "LoggingConfigurationMetadataTypeDef",
     {
-        "createdAt": datetime,
-        "logGroupArn": str,
-        "modifiedAt": datetime,
         "status": LoggingConfigurationStatusTypeDef,
         "workspace": str,
+        "logGroupArn": str,
+        "createdAt": datetime,
+        "modifiedAt": datetime,
     },
 )
 
 UpdateLoggingConfigurationResponseTypeDef = TypedDict(
     "UpdateLoggingConfigurationResponseTypeDef",
     {
         "status": LoggingConfigurationStatusTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateRuleGroupsNamespaceResponseTypeDef = TypedDict(
     "CreateRuleGroupsNamespaceResponseTypeDef",
     {
-        "arn": str,
         "name": str,
+        "arn": str,
         "status": RuleGroupsNamespaceStatusTypeDef,
         "tags": Dict[str, str],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 PutRuleGroupsNamespaceResponseTypeDef = TypedDict(
     "PutRuleGroupsNamespaceResponseTypeDef",
     {
-        "arn": str,
         "name": str,
+        "arn": str,
         "status": RuleGroupsNamespaceStatusTypeDef,
         "tags": Dict[str, str],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredRuleGroupsNamespaceDescriptionTypeDef = TypedDict(
     "_RequiredRuleGroupsNamespaceDescriptionTypeDef",
     {
         "arn": str,
-        "createdAt": datetime,
-        "data": bytes,
-        "modifiedAt": datetime,
         "name": str,
         "status": RuleGroupsNamespaceStatusTypeDef,
+        "data": bytes,
+        "createdAt": datetime,
+        "modifiedAt": datetime,
     },
 )
 _OptionalRuleGroupsNamespaceDescriptionTypeDef = TypedDict(
     "_OptionalRuleGroupsNamespaceDescriptionTypeDef",
     {
         "tags": Dict[str, str],
     },
@@ -619,18 +619,18 @@
 ):
     pass
 
 _RequiredRuleGroupsNamespaceSummaryTypeDef = TypedDict(
     "_RequiredRuleGroupsNamespaceSummaryTypeDef",
     {
         "arn": str,
-        "createdAt": datetime,
-        "modifiedAt": datetime,
         "name": str,
         "status": RuleGroupsNamespaceStatusTypeDef,
+        "createdAt": datetime,
+        "modifiedAt": datetime,
     },
 )
 _OptionalRuleGroupsNamespaceSummaryTypeDef = TypedDict(
     "_OptionalRuleGroupsNamespaceSummaryTypeDef",
     {
         "tags": Dict[str, str],
     },
@@ -641,29 +641,29 @@
     _RequiredRuleGroupsNamespaceSummaryTypeDef, _OptionalRuleGroupsNamespaceSummaryTypeDef
 ):
     pass
 
 CreateWorkspaceResponseTypeDef = TypedDict(
     "CreateWorkspaceResponseTypeDef",
     {
+        "workspaceId": str,
         "arn": str,
         "status": WorkspaceStatusTypeDef,
         "tags": Dict[str, str],
-        "workspaceId": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredWorkspaceDescriptionTypeDef = TypedDict(
     "_RequiredWorkspaceDescriptionTypeDef",
     {
+        "workspaceId": str,
         "arn": str,
-        "createdAt": datetime,
         "status": WorkspaceStatusTypeDef,
-        "workspaceId": str,
+        "createdAt": datetime,
     },
 )
 _OptionalWorkspaceDescriptionTypeDef = TypedDict(
     "_OptionalWorkspaceDescriptionTypeDef",
     {
         "alias": str,
         "prometheusEndpoint": str,
@@ -676,18 +676,18 @@
     _RequiredWorkspaceDescriptionTypeDef, _OptionalWorkspaceDescriptionTypeDef
 ):
     pass
 
 _RequiredWorkspaceSummaryTypeDef = TypedDict(
     "_RequiredWorkspaceSummaryTypeDef",
     {
+        "workspaceId": str,
         "arn": str,
-        "createdAt": datetime,
         "status": WorkspaceStatusTypeDef,
-        "workspaceId": str,
+        "createdAt": datetime,
     },
 )
 _OptionalWorkspaceSummaryTypeDef = TypedDict(
     "_OptionalWorkspaceSummaryTypeDef",
     {
         "alias": str,
         "tags": Dict[str, str],
@@ -791,16 +791,16 @@
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListRuleGroupsNamespacesResponseTypeDef = TypedDict(
     "ListRuleGroupsNamespacesResponseTypeDef",
     {
-        "nextToken": str,
         "ruleGroupsNamespaces": List[RuleGroupsNamespaceSummaryTypeDef],
+        "nextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeWorkspaceResponseTypeDef = TypedDict(
     "DescribeWorkspaceResponseTypeDef",
     {
@@ -808,12 +808,12 @@
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListWorkspacesResponseTypeDef = TypedDict(
     "ListWorkspacesResponseTypeDef",
     {
-        "nextToken": str,
         "workspaces": List[WorkspaceSummaryTypeDef],
+        "nextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `types-aiobotocore-amp-2.5.2.post3/types_aiobotocore_amp/waiter.py` & `types-aiobotocore-amp-2.5.4/types_aiobotocore_amp/waiter.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-amp-2.5.2.post3/types_aiobotocore_amp/waiter.pyi` & `types-aiobotocore-amp-2.5.4/types_aiobotocore_amp/waiter.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-amp-2.5.2.post3/types_aiobotocore_amp.egg-info/PKG-INFO` & `types-aiobotocore-amp-2.5.4/types_aiobotocore_amp.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-amp
-Version: 2.5.2.post3
-Summary: Type annotations for aiobotocore.PrometheusService 2.5.2 service generated with mypy-boto3-builder 7.17.2
+Version: 2.5.4
+Summary: Type annotations for aiobotocore.PrometheusService 2.5.4 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_amp/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-amp.svg?color=blue)](https://pypi.org/project/types-aiobotocore-amp)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_amp/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-amp)](https://pepy.tech/project/types-aiobotocore-amp)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.PrometheusService 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amp.html#PrometheusService)
+[aiobotocore.PrometheusService 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amp.html#PrometheusService)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-amp-2.5.2.post3/types_aiobotocore_amp.egg-info/SOURCES.txt` & `types-aiobotocore-amp-2.5.4/types_aiobotocore_amp.egg-info/SOURCES.txt`

 * *Files identical despite different names*


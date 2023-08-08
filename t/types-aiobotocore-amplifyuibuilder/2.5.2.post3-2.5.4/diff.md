# Comparing `tmp/types-aiobotocore-amplifyuibuilder-2.5.2.post3.tar.gz` & `tmp/types-aiobotocore-amplifyuibuilder-2.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-amplifyuibuilder-2.5.2.post3.tar", last modified: Fri Aug  4 12:37:15 2023, max compression
+gzip compressed data, was "types-aiobotocore-amplifyuibuilder-2.5.4.tar", last modified: Tue Aug  8 01:23:13 2023, max compression
```

## Comparing `types-aiobotocore-amplifyuibuilder-2.5.2.post3.tar` & `types-aiobotocore-amplifyuibuilder-2.5.4.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:37:15.159138 types-aiobotocore-amplifyuibuilder-2.5.2.post3/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-04 12:18:04.000000 types-aiobotocore-amplifyuibuilder-2.5.2.post3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    14249 2023-08-04 12:37:15.151137 types-aiobotocore-amplifyuibuilder-2.5.2.post3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    12695 2023-08-04 12:18:04.000000 types-aiobotocore-amplifyuibuilder-2.5.2.post3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-04 12:37:15.159138 types-aiobotocore-amplifyuibuilder-2.5.2.post3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2135 2023-08-04 12:18:04.000000 types-aiobotocore-amplifyuibuilder-2.5.2.post3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:37:15.143137 types-aiobotocore-amplifyuibuilder-2.5.2.post3/types_aiobotocore_amplifyuibuilder/
--rw-r--r--   0 runner    (1001) docker     (123)     1819 2023-08-04 12:18:04.000000 types-aiobotocore-amplifyuibuilder-2.5.2.post3/types_aiobotocore_amplifyuibuilder/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1818 2023-08-04 12:18:04.000000 types-aiobotocore-amplifyuibuilder-2.5.2.post3/types_aiobotocore_amplifyuibuilder/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      979 2023-08-04 12:18:04.000000 types-aiobotocore-amplifyuibuilder-2.5.2.post3/types_aiobotocore_amplifyuibuilder/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    23796 2023-08-04 12:18:04.000000 types-aiobotocore-amplifyuibuilder-2.5.2.post3/types_aiobotocore_amplifyuibuilder/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    23755 2023-08-04 12:18:04.000000 types-aiobotocore-amplifyuibuilder-2.5.2.post3/types_aiobotocore_amplifyuibuilder/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    10288 2023-08-04 12:18:04.000000 types-aiobotocore-amplifyuibuilder-2.5.2.post3/types_aiobotocore_amplifyuibuilder/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    10286 2023-08-04 12:18:04.000000 types-aiobotocore-amplifyuibuilder-2.5.2.post3/types_aiobotocore_amplifyuibuilder/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8895 2023-08-04 12:18:04.000000 types-aiobotocore-amplifyuibuilder-2.5.2.post3/types_aiobotocore_amplifyuibuilder/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     8886 2023-08-04 12:18:04.000000 types-aiobotocore-amplifyuibuilder-2.5.2.post3/types_aiobotocore_amplifyuibuilder/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 12:18:04.000000 types-aiobotocore-amplifyuibuilder-2.5.2.post3/types_aiobotocore_amplifyuibuilder/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    47839 2023-08-04 12:18:06.000000 types-aiobotocore-amplifyuibuilder-2.5.2.post3/types_aiobotocore_amplifyuibuilder/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    47747 2023-08-04 12:18:06.000000 types-aiobotocore-amplifyuibuilder-2.5.2.post3/types_aiobotocore_amplifyuibuilder/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-04 12:18:04.000000 types-aiobotocore-amplifyuibuilder-2.5.2.post3/types_aiobotocore_amplifyuibuilder/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:37:15.151137 types-aiobotocore-amplifyuibuilder-2.5.2.post3/types_aiobotocore_amplifyuibuilder.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    14249 2023-08-04 12:37:14.000000 types-aiobotocore-amplifyuibuilder-2.5.2.post3/types_aiobotocore_amplifyuibuilder.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      984 2023-08-04 12:37:15.000000 types-aiobotocore-amplifyuibuilder-2.5.2.post3/types_aiobotocore_amplifyuibuilder.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 12:37:14.000000 types-aiobotocore-amplifyuibuilder-2.5.2.post3/types_aiobotocore_amplifyuibuilder.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 12:37:14.000000 types-aiobotocore-amplifyuibuilder-2.5.2.post3/types_aiobotocore_amplifyuibuilder.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-04 12:37:14.000000 types-aiobotocore-amplifyuibuilder-2.5.2.post3/types_aiobotocore_amplifyuibuilder.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-08-04 12:37:14.000000 types-aiobotocore-amplifyuibuilder-2.5.2.post3/types_aiobotocore_amplifyuibuilder.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:23:13.682488 types-aiobotocore-amplifyuibuilder-2.5.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-08 01:05:51.000000 types-aiobotocore-amplifyuibuilder-2.5.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    14243 2023-08-08 01:23:13.682488 types-aiobotocore-amplifyuibuilder-2.5.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    12695 2023-08-08 01:05:51.000000 types-aiobotocore-amplifyuibuilder-2.5.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-08 01:23:13.682488 types-aiobotocore-amplifyuibuilder-2.5.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2129 2023-08-08 01:05:51.000000 types-aiobotocore-amplifyuibuilder-2.5.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:23:13.682488 types-aiobotocore-amplifyuibuilder-2.5.4/types_aiobotocore_amplifyuibuilder/
+-rw-r--r--   0 runner    (1001) docker     (123)     1819 2023-08-08 01:05:51.000000 types-aiobotocore-amplifyuibuilder-2.5.4/types_aiobotocore_amplifyuibuilder/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1818 2023-08-08 01:05:51.000000 types-aiobotocore-amplifyuibuilder-2.5.4/types_aiobotocore_amplifyuibuilder/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      967 2023-08-08 01:05:51.000000 types-aiobotocore-amplifyuibuilder-2.5.4/types_aiobotocore_amplifyuibuilder/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23796 2023-08-08 01:05:52.000000 types-aiobotocore-amplifyuibuilder-2.5.4/types_aiobotocore_amplifyuibuilder/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23755 2023-08-08 01:05:51.000000 types-aiobotocore-amplifyuibuilder-2.5.4/types_aiobotocore_amplifyuibuilder/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    10383 2023-08-08 01:05:52.000000 types-aiobotocore-amplifyuibuilder-2.5.4/types_aiobotocore_amplifyuibuilder/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10381 2023-08-08 01:05:52.000000 types-aiobotocore-amplifyuibuilder-2.5.4/types_aiobotocore_amplifyuibuilder/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8895 2023-08-08 01:05:52.000000 types-aiobotocore-amplifyuibuilder-2.5.4/types_aiobotocore_amplifyuibuilder/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8886 2023-08-08 01:05:52.000000 types-aiobotocore-amplifyuibuilder-2.5.4/types_aiobotocore_amplifyuibuilder/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 01:05:51.000000 types-aiobotocore-amplifyuibuilder-2.5.4/types_aiobotocore_amplifyuibuilder/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    48451 2023-08-08 01:05:53.000000 types-aiobotocore-amplifyuibuilder-2.5.4/types_aiobotocore_amplifyuibuilder/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    48359 2023-08-08 01:05:53.000000 types-aiobotocore-amplifyuibuilder-2.5.4/types_aiobotocore_amplifyuibuilder/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-08-08 01:05:51.000000 types-aiobotocore-amplifyuibuilder-2.5.4/types_aiobotocore_amplifyuibuilder/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:23:13.682488 types-aiobotocore-amplifyuibuilder-2.5.4/types_aiobotocore_amplifyuibuilder.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    14243 2023-08-08 01:23:13.000000 types-aiobotocore-amplifyuibuilder-2.5.4/types_aiobotocore_amplifyuibuilder.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      984 2023-08-08 01:23:13.000000 types-aiobotocore-amplifyuibuilder-2.5.4/types_aiobotocore_amplifyuibuilder.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 01:23:13.000000 types-aiobotocore-amplifyuibuilder-2.5.4/types_aiobotocore_amplifyuibuilder.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 01:23:13.000000 types-aiobotocore-amplifyuibuilder-2.5.4/types_aiobotocore_amplifyuibuilder.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-08 01:23:13.000000 types-aiobotocore-amplifyuibuilder-2.5.4/types_aiobotocore_amplifyuibuilder.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-08-08 01:23:13.000000 types-aiobotocore-amplifyuibuilder-2.5.4/types_aiobotocore_amplifyuibuilder.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-amplifyuibuilder-2.5.2.post3/LICENSE` & `types-aiobotocore-amplifyuibuilder-2.5.4/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-amplifyuibuilder-2.5.2.post3/PKG-INFO` & `types-aiobotocore-amplifyuibuilder-2.5.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-amplifyuibuilder
-Version: 2.5.2.post3
-Summary: Type annotations for aiobotocore.AmplifyUIBuilder 2.5.2 service generated with mypy-boto3-builder 7.17.2
+Version: 2.5.4
+Summary: Type annotations for aiobotocore.AmplifyUIBuilder 2.5.4 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_amplifyuibuilder/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-amplifyuibuilder.svg?color=blue)](https://pypi.org/project/types-aiobotocore-amplifyuibuilder)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_amplifyuibuilder/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-amplifyuibuilder)](https://pepy.tech/project/types-aiobotocore-amplifyuibuilder)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.AmplifyUIBuilder 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amplifyuibuilder.html#AmplifyUIBuilder)
+[aiobotocore.AmplifyUIBuilder 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amplifyuibuilder.html#AmplifyUIBuilder)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-amplifyuibuilder-2.5.2.post3/README.md` & `types-aiobotocore-amplifyuibuilder-2.5.4/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-amplifyuibuilder.svg?color=blue)](https://pypi.org/project/types-aiobotocore-amplifyuibuilder)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_amplifyuibuilder/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-amplifyuibuilder)](https://pepy.tech/project/types-aiobotocore-amplifyuibuilder)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.AmplifyUIBuilder 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amplifyuibuilder.html#AmplifyUIBuilder)
+[aiobotocore.AmplifyUIBuilder 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amplifyuibuilder.html#AmplifyUIBuilder)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-amplifyuibuilder-2.5.2.post3/setup.py` & `types-aiobotocore-amplifyuibuilder-2.5.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-amplifyuibuilder",
-    version="2.5.2.post3",
+    version="2.5.4",
     packages=["types_aiobotocore_amplifyuibuilder"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.AmplifyUIBuilder 2.5.2 service generated with"
+        "Type annotations for aiobotocore.AmplifyUIBuilder 2.5.4 service generated with"
         " mypy-boto3-builder 7.17.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
```

### Comparing `types-aiobotocore-amplifyuibuilder-2.5.2.post3/types_aiobotocore_amplifyuibuilder/__init__.py` & `types-aiobotocore-amplifyuibuilder-2.5.4/types_aiobotocore_amplifyuibuilder/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-amplifyuibuilder-2.5.2.post3/types_aiobotocore_amplifyuibuilder/__init__.pyi` & `types-aiobotocore-amplifyuibuilder-2.5.4/types_aiobotocore_amplifyuibuilder/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-amplifyuibuilder-2.5.2.post3/types_aiobotocore_amplifyuibuilder/client.py` & `types-aiobotocore-amplifyuibuilder-2.5.4/types_aiobotocore_amplifyuibuilder/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -145,15 +145,15 @@
         *,
         appId: str,
         environmentName: str,
         formToCreate: CreateFormDataTypeDef,
         clientToken: str = ...
     ) -> CreateFormResponseTypeDef:
         """
-        Creates a new form for an Amplify.
+        Creates a new form for an Amplify app.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amplifyuibuilder.html#AmplifyUIBuilder.Client.create_form)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_amplifyuibuilder/client/#create_form)
         """
 
     async def create_theme(
         self,
@@ -377,15 +377,15 @@
         *,
         appId: str,
         environmentName: str,
         codegenJobToCreate: StartCodegenJobDataTypeDef,
         clientToken: str = ...
     ) -> StartCodegenJobResponseTypeDef:
         """
-        Starts a code generation job for for a specified Amplify app and backend
+        Starts a code generation job for a specified Amplify app and backend
         environment.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amplifyuibuilder.html#AmplifyUIBuilder.Client.start_codegen_job)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_amplifyuibuilder/client/#start_codegen_job)
         """
 
     async def update_component(
```

### Comparing `types-aiobotocore-amplifyuibuilder-2.5.2.post3/types_aiobotocore_amplifyuibuilder/client.pyi` & `types-aiobotocore-amplifyuibuilder-2.5.4/types_aiobotocore_amplifyuibuilder/client.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -137,15 +137,15 @@
         *,
         appId: str,
         environmentName: str,
         formToCreate: CreateFormDataTypeDef,
         clientToken: str = ...
     ) -> CreateFormResponseTypeDef:
         """
-        Creates a new form for an Amplify.
+        Creates a new form for an Amplify app.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amplifyuibuilder.html#AmplifyUIBuilder.Client.create_form)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_amplifyuibuilder/client/#create_form)
         """
     async def create_theme(
         self,
         *,
@@ -348,15 +348,15 @@
         *,
         appId: str,
         environmentName: str,
         codegenJobToCreate: StartCodegenJobDataTypeDef,
         clientToken: str = ...
     ) -> StartCodegenJobResponseTypeDef:
         """
-        Starts a code generation job for for a specified Amplify app and backend
+        Starts a code generation job for a specified Amplify app and backend
         environment.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amplifyuibuilder.html#AmplifyUIBuilder.Client.start_codegen_job)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_amplifyuibuilder/client/#start_codegen_job)
         """
     async def update_component(
         self,
```

### Comparing `types-aiobotocore-amplifyuibuilder-2.5.2.post3/types_aiobotocore_amplifyuibuilder/literals.py` & `types-aiobotocore-amplifyuibuilder-2.5.4/types_aiobotocore_amplifyuibuilder/literals.pyi`

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
     "CodegenGenericDataFieldDataTypeType",
     "CodegenJobGenericDataSourceTypeType",
     "CodegenJobStatusType",
     "ExportComponentsPaginatorName",
     "ExportFormsPaginatorName",
     "ExportThemesPaginatorName",
@@ -45,15 +44,14 @@
     "AmplifyUIBuilderServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "RegionName",
 )
 
-
 CodegenGenericDataFieldDataTypeType = Literal[
     "AWSDate",
     "AWSDateTime",
     "AWSEmail",
     "AWSIPAddress",
     "AWSJSON",
     "AWSPhone",
@@ -102,14 +100,15 @@
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
@@ -205,14 +204,15 @@
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
@@ -291,26 +291,28 @@
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

### Comparing `types-aiobotocore-amplifyuibuilder-2.5.2.post3/types_aiobotocore_amplifyuibuilder/literals.pyi` & `types-aiobotocore-amplifyuibuilder-2.5.4/types_aiobotocore_amplifyuibuilder/literals.py`

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
     "CodegenGenericDataFieldDataTypeType",
     "CodegenJobGenericDataSourceTypeType",
     "CodegenJobStatusType",
     "ExportComponentsPaginatorName",
     "ExportFormsPaginatorName",
     "ExportThemesPaginatorName",
@@ -44,14 +45,15 @@
     "AmplifyUIBuilderServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "RegionName",
 )
 
+
 CodegenGenericDataFieldDataTypeType = Literal[
     "AWSDate",
     "AWSDateTime",
     "AWSEmail",
     "AWSIPAddress",
     "AWSJSON",
     "AWSPhone",
@@ -100,14 +102,15 @@
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
@@ -203,14 +206,15 @@
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
@@ -289,26 +293,28 @@
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

### Comparing `types-aiobotocore-amplifyuibuilder-2.5.2.post3/types_aiobotocore_amplifyuibuilder/paginator.py` & `types-aiobotocore-amplifyuibuilder-2.5.4/types_aiobotocore_amplifyuibuilder/paginator.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-amplifyuibuilder-2.5.2.post3/types_aiobotocore_amplifyuibuilder/paginator.pyi` & `types-aiobotocore-amplifyuibuilder-2.5.4/types_aiobotocore_amplifyuibuilder/paginator.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-amplifyuibuilder-2.5.2.post3/types_aiobotocore_amplifyuibuilder/type_defs.py` & `types-aiobotocore-amplifyuibuilder-2.5.4/types_aiobotocore_amplifyuibuilder/type_defs.py`

 * *Files 1% similar despite different names*

```diff
@@ -38,19 +38,19 @@
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 
 __all__ = (
     "MutationActionSetStateParameterTypeDef",
+    "GraphQLRenderConfigTypeDef",
     "CodegenFeatureFlagsTypeDef",
     "CodegenGenericDataEnumTypeDef",
     "CodegenGenericDataRelationshipTypeTypeDef",
     "CodegenJobAssetTypeDef",
-    "ReactStartCodegenJobDataTypeDef",
     "CodegenJobSummaryTypeDef",
     "ComponentBindingPropertiesValuePropertiesTypeDef",
     "ComponentConditionPropertyTypeDef",
     "SortPropertyTypeDef",
     "ComponentPropertyBindingPropertiesTypeDef",
     "FormBindingElementTypeDef",
     "ComponentSummaryTypeDef",
@@ -87,16 +87,16 @@
     "PutMetadataFlagBodyTypeDef",
     "RefreshTokenRequestBodyTypeDef",
     "ThemeValueTypeDef",
     "ThemeValuesTypeDef",
     "UpdateThemeDataTypeDef",
     "ValueMappingTypeDef",
     "ActionParametersTypeDef",
+    "ApiConfigurationTypeDef",
     "CodegenGenericDataFieldTypeDef",
-    "CodegenJobRenderConfigTypeDef",
     "ComponentBindingPropertiesValueTypeDef",
     "ComponentDataConfigurationTypeDef",
     "ComponentPropertyTypeDef",
     "EmptyResponseMetadataTypeDef",
     "ExchangeCodeForTokenResponseTypeDef",
     "GetMetadataResponseTypeDef",
     "ListCodegenJobsResponseTypeDef",
@@ -122,23 +122,25 @@
     "FormInputValuePropertyTypeDef",
     "FormStyleTypeDef",
     "ListThemesResponseTypeDef",
     "PutMetadataFlagRequestRequestTypeDef",
     "RefreshTokenRequestRequestTypeDef",
     "UpdateThemeRequestRequestTypeDef",
     "ComponentEventTypeDef",
+    "ReactStartCodegenJobDataTypeDef",
     "CodegenGenericDataModelTypeDef",
     "CodegenGenericDataNonModelTypeDef",
     "ListFormsResponseTypeDef",
     "FormCTATypeDef",
     "ValueMappingsTypeDef",
     "ComponentChildTypeDef",
     "ComponentTypeDef",
     "CreateComponentDataTypeDef",
     "UpdateComponentDataTypeDef",
+    "CodegenJobRenderConfigTypeDef",
     "CodegenJobGenericDataSchemaTypeDef",
     "FieldInputConfigTypeDef",
     "CreateComponentResponseTypeDef",
     "ExportComponentsResponseTypeDef",
     "GetComponentResponseTypeDef",
     "UpdateComponentResponseTypeDef",
     "CreateComponentRequestRequestTypeDef",
@@ -165,14 +167,25 @@
     {
         "componentName": str,
         "property": str,
         "set": "ComponentPropertyTypeDef",
     },
 )
 
+GraphQLRenderConfigTypeDef = TypedDict(
+    "GraphQLRenderConfigTypeDef",
+    {
+        "typesFilePath": str,
+        "queriesFilePath": str,
+        "mutationsFilePath": str,
+        "subscriptionsFilePath": str,
+        "fragmentsFilePath": str,
+    },
+)
+
 CodegenFeatureFlagsTypeDef = TypedDict(
     "CodegenFeatureFlagsTypeDef",
     {
         "isRelationshipSupported": bool,
         "isNonModelSupported": bool,
     },
     total=False,
@@ -218,26 +231,14 @@
     "CodegenJobAssetTypeDef",
     {
         "downloadUrl": str,
     },
     total=False,
 )
 
-ReactStartCodegenJobDataTypeDef = TypedDict(
-    "ReactStartCodegenJobDataTypeDef",
-    {
-        "module": JSModuleType,
-        "target": JSTargetType,
-        "script": JSScriptType,
-        "renderTypeDeclarations": bool,
-        "inlineSourceMap": bool,
-    },
-    total=False,
-)
-
 _RequiredCodegenJobSummaryTypeDef = TypedDict(
     "_RequiredCodegenJobSummaryTypeDef",
     {
         "appId": str,
         "environmentName": str,
         "id": str,
     },
@@ -890,14 +891,24 @@
         "id": "ComponentPropertyTypeDef",
         "fields": Mapping[str, "ComponentPropertyTypeDef"],
         "state": MutationActionSetStateParameterTypeDef,
     },
     total=False,
 )
 
+ApiConfigurationTypeDef = TypedDict(
+    "ApiConfigurationTypeDef",
+    {
+        "graphQLConfig": GraphQLRenderConfigTypeDef,
+        "dataStoreConfig": Dict[str, Any],
+        "noApiConfig": Dict[str, Any],
+    },
+    total=False,
+)
+
 _RequiredCodegenGenericDataFieldTypeDef = TypedDict(
     "_RequiredCodegenGenericDataFieldTypeDef",
     {
         "dataType": CodegenGenericDataFieldDataTypeType,
         "dataTypeValue": str,
         "required": bool,
         "readOnly": bool,
@@ -915,22 +926,14 @@
 
 class CodegenGenericDataFieldTypeDef(
     _RequiredCodegenGenericDataFieldTypeDef, _OptionalCodegenGenericDataFieldTypeDef
 ):
     pass
 
 
-CodegenJobRenderConfigTypeDef = TypedDict(
-    "CodegenJobRenderConfigTypeDef",
-    {
-        "react": ReactStartCodegenJobDataTypeDef,
-    },
-    total=False,
-)
-
 ComponentBindingPropertiesValueTypeDef = TypedDict(
     "ComponentBindingPropertiesValueTypeDef",
     {
         "type": str,
         "bindingProperties": ComponentBindingPropertiesValuePropertiesTypeDef,
         "defaultValue": str,
     },
@@ -1390,14 +1393,27 @@
         "action": str,
         "parameters": ActionParametersTypeDef,
         "bindingEvent": str,
     },
     total=False,
 )
 
+ReactStartCodegenJobDataTypeDef = TypedDict(
+    "ReactStartCodegenJobDataTypeDef",
+    {
+        "module": JSModuleType,
+        "target": JSTargetType,
+        "script": JSScriptType,
+        "renderTypeDeclarations": bool,
+        "inlineSourceMap": bool,
+        "apiConfiguration": ApiConfigurationTypeDef,
+    },
+    total=False,
+)
+
 _RequiredCodegenGenericDataModelTypeDef = TypedDict(
     "_RequiredCodegenGenericDataModelTypeDef",
     {
         "fields": Dict[str, CodegenGenericDataFieldTypeDef],
         "primaryKeys": List[str],
     },
 )
@@ -1565,14 +1581,22 @@
         "collectionProperties": Mapping[str, ComponentDataConfigurationTypeDef],
         "events": Mapping[str, ComponentEventTypeDef],
         "schemaVersion": str,
     },
     total=False,
 )
 
+CodegenJobRenderConfigTypeDef = TypedDict(
+    "CodegenJobRenderConfigTypeDef",
+    {
+        "react": ReactStartCodegenJobDataTypeDef,
+    },
+    total=False,
+)
+
 CodegenJobGenericDataSchemaTypeDef = TypedDict(
     "CodegenJobGenericDataSchemaTypeDef",
     {
         "dataSourceType": Literal["DataStore"],
         "models": Dict[str, CodegenGenericDataModelTypeDef],
         "enums": Dict[str, CodegenGenericDataEnumTypeDef],
         "nonModels": Dict[str, CodegenGenericDataNonModelTypeDef],
```

### Comparing `types-aiobotocore-amplifyuibuilder-2.5.2.post3/types_aiobotocore_amplifyuibuilder/type_defs.pyi` & `types-aiobotocore-amplifyuibuilder-2.5.4/types_aiobotocore_amplifyuibuilder/type_defs.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -37,19 +37,19 @@
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
     "MutationActionSetStateParameterTypeDef",
+    "GraphQLRenderConfigTypeDef",
     "CodegenFeatureFlagsTypeDef",
     "CodegenGenericDataEnumTypeDef",
     "CodegenGenericDataRelationshipTypeTypeDef",
     "CodegenJobAssetTypeDef",
-    "ReactStartCodegenJobDataTypeDef",
     "CodegenJobSummaryTypeDef",
     "ComponentBindingPropertiesValuePropertiesTypeDef",
     "ComponentConditionPropertyTypeDef",
     "SortPropertyTypeDef",
     "ComponentPropertyBindingPropertiesTypeDef",
     "FormBindingElementTypeDef",
     "ComponentSummaryTypeDef",
@@ -86,16 +86,16 @@
     "PutMetadataFlagBodyTypeDef",
     "RefreshTokenRequestBodyTypeDef",
     "ThemeValueTypeDef",
     "ThemeValuesTypeDef",
     "UpdateThemeDataTypeDef",
     "ValueMappingTypeDef",
     "ActionParametersTypeDef",
+    "ApiConfigurationTypeDef",
     "CodegenGenericDataFieldTypeDef",
-    "CodegenJobRenderConfigTypeDef",
     "ComponentBindingPropertiesValueTypeDef",
     "ComponentDataConfigurationTypeDef",
     "ComponentPropertyTypeDef",
     "EmptyResponseMetadataTypeDef",
     "ExchangeCodeForTokenResponseTypeDef",
     "GetMetadataResponseTypeDef",
     "ListCodegenJobsResponseTypeDef",
@@ -121,23 +121,25 @@
     "FormInputValuePropertyTypeDef",
     "FormStyleTypeDef",
     "ListThemesResponseTypeDef",
     "PutMetadataFlagRequestRequestTypeDef",
     "RefreshTokenRequestRequestTypeDef",
     "UpdateThemeRequestRequestTypeDef",
     "ComponentEventTypeDef",
+    "ReactStartCodegenJobDataTypeDef",
     "CodegenGenericDataModelTypeDef",
     "CodegenGenericDataNonModelTypeDef",
     "ListFormsResponseTypeDef",
     "FormCTATypeDef",
     "ValueMappingsTypeDef",
     "ComponentChildTypeDef",
     "ComponentTypeDef",
     "CreateComponentDataTypeDef",
     "UpdateComponentDataTypeDef",
+    "CodegenJobRenderConfigTypeDef",
     "CodegenJobGenericDataSchemaTypeDef",
     "FieldInputConfigTypeDef",
     "CreateComponentResponseTypeDef",
     "ExportComponentsResponseTypeDef",
     "GetComponentResponseTypeDef",
     "UpdateComponentResponseTypeDef",
     "CreateComponentRequestRequestTypeDef",
@@ -164,14 +166,25 @@
     {
         "componentName": str,
         "property": str,
         "set": "ComponentPropertyTypeDef",
     },
 )
 
+GraphQLRenderConfigTypeDef = TypedDict(
+    "GraphQLRenderConfigTypeDef",
+    {
+        "typesFilePath": str,
+        "queriesFilePath": str,
+        "mutationsFilePath": str,
+        "subscriptionsFilePath": str,
+        "fragmentsFilePath": str,
+    },
+)
+
 CodegenFeatureFlagsTypeDef = TypedDict(
     "CodegenFeatureFlagsTypeDef",
     {
         "isRelationshipSupported": bool,
         "isNonModelSupported": bool,
     },
     total=False,
@@ -215,26 +228,14 @@
     "CodegenJobAssetTypeDef",
     {
         "downloadUrl": str,
     },
     total=False,
 )
 
-ReactStartCodegenJobDataTypeDef = TypedDict(
-    "ReactStartCodegenJobDataTypeDef",
-    {
-        "module": JSModuleType,
-        "target": JSTargetType,
-        "script": JSScriptType,
-        "renderTypeDeclarations": bool,
-        "inlineSourceMap": bool,
-    },
-    total=False,
-)
-
 _RequiredCodegenJobSummaryTypeDef = TypedDict(
     "_RequiredCodegenJobSummaryTypeDef",
     {
         "appId": str,
         "environmentName": str,
         "id": str,
     },
@@ -851,14 +852,24 @@
         "id": "ComponentPropertyTypeDef",
         "fields": Mapping[str, "ComponentPropertyTypeDef"],
         "state": MutationActionSetStateParameterTypeDef,
     },
     total=False,
 )
 
+ApiConfigurationTypeDef = TypedDict(
+    "ApiConfigurationTypeDef",
+    {
+        "graphQLConfig": GraphQLRenderConfigTypeDef,
+        "dataStoreConfig": Dict[str, Any],
+        "noApiConfig": Dict[str, Any],
+    },
+    total=False,
+)
+
 _RequiredCodegenGenericDataFieldTypeDef = TypedDict(
     "_RequiredCodegenGenericDataFieldTypeDef",
     {
         "dataType": CodegenGenericDataFieldDataTypeType,
         "dataTypeValue": str,
         "required": bool,
         "readOnly": bool,
@@ -874,22 +885,14 @@
 )
 
 class CodegenGenericDataFieldTypeDef(
     _RequiredCodegenGenericDataFieldTypeDef, _OptionalCodegenGenericDataFieldTypeDef
 ):
     pass
 
-CodegenJobRenderConfigTypeDef = TypedDict(
-    "CodegenJobRenderConfigTypeDef",
-    {
-        "react": ReactStartCodegenJobDataTypeDef,
-    },
-    total=False,
-)
-
 ComponentBindingPropertiesValueTypeDef = TypedDict(
     "ComponentBindingPropertiesValueTypeDef",
     {
         "type": str,
         "bindingProperties": ComponentBindingPropertiesValuePropertiesTypeDef,
         "defaultValue": str,
     },
@@ -1327,14 +1330,27 @@
         "action": str,
         "parameters": ActionParametersTypeDef,
         "bindingEvent": str,
     },
     total=False,
 )
 
+ReactStartCodegenJobDataTypeDef = TypedDict(
+    "ReactStartCodegenJobDataTypeDef",
+    {
+        "module": JSModuleType,
+        "target": JSTargetType,
+        "script": JSScriptType,
+        "renderTypeDeclarations": bool,
+        "inlineSourceMap": bool,
+        "apiConfiguration": ApiConfigurationTypeDef,
+    },
+    total=False,
+)
+
 _RequiredCodegenGenericDataModelTypeDef = TypedDict(
     "_RequiredCodegenGenericDataModelTypeDef",
     {
         "fields": Dict[str, CodegenGenericDataFieldTypeDef],
         "primaryKeys": List[str],
     },
 )
@@ -1492,14 +1508,22 @@
         "collectionProperties": Mapping[str, ComponentDataConfigurationTypeDef],
         "events": Mapping[str, ComponentEventTypeDef],
         "schemaVersion": str,
     },
     total=False,
 )
 
+CodegenJobRenderConfigTypeDef = TypedDict(
+    "CodegenJobRenderConfigTypeDef",
+    {
+        "react": ReactStartCodegenJobDataTypeDef,
+    },
+    total=False,
+)
+
 CodegenJobGenericDataSchemaTypeDef = TypedDict(
     "CodegenJobGenericDataSchemaTypeDef",
     {
         "dataSourceType": Literal["DataStore"],
         "models": Dict[str, CodegenGenericDataModelTypeDef],
         "enums": Dict[str, CodegenGenericDataEnumTypeDef],
         "nonModels": Dict[str, CodegenGenericDataNonModelTypeDef],
```

### Comparing `types-aiobotocore-amplifyuibuilder-2.5.2.post3/types_aiobotocore_amplifyuibuilder.egg-info/PKG-INFO` & `types-aiobotocore-amplifyuibuilder-2.5.4/types_aiobotocore_amplifyuibuilder.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-amplifyuibuilder
-Version: 2.5.2.post3
-Summary: Type annotations for aiobotocore.AmplifyUIBuilder 2.5.2 service generated with mypy-boto3-builder 7.17.2
+Version: 2.5.4
+Summary: Type annotations for aiobotocore.AmplifyUIBuilder 2.5.4 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_amplifyuibuilder/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-amplifyuibuilder.svg?color=blue)](https://pypi.org/project/types-aiobotocore-amplifyuibuilder)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_amplifyuibuilder/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-amplifyuibuilder)](https://pepy.tech/project/types-aiobotocore-amplifyuibuilder)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.AmplifyUIBuilder 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amplifyuibuilder.html#AmplifyUIBuilder)
+[aiobotocore.AmplifyUIBuilder 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amplifyuibuilder.html#AmplifyUIBuilder)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-amplifyuibuilder-2.5.2.post3/types_aiobotocore_amplifyuibuilder.egg-info/SOURCES.txt` & `types-aiobotocore-amplifyuibuilder-2.5.4/types_aiobotocore_amplifyuibuilder.egg-info/SOURCES.txt`

 * *Files identical despite different names*


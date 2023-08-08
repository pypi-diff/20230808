# Comparing `tmp/types-aiobotocore-codecatalyst-2.5.2.post3.tar.gz` & `tmp/types-aiobotocore-codecatalyst-2.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-codecatalyst-2.5.2.post3.tar", last modified: Fri Aug  4 12:37:26 2023, max compression
+gzip compressed data, was "types-aiobotocore-codecatalyst-2.5.4.tar", last modified: Tue Aug  8 01:23:28 2023, max compression
```

## Comparing `types-aiobotocore-codecatalyst-2.5.2.post3.tar` & `types-aiobotocore-codecatalyst-2.5.4.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:37:26.771402 types-aiobotocore-codecatalyst-2.5.2.post3/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-04 12:20:06.000000 types-aiobotocore-codecatalyst-2.5.2.post3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    14327 2023-08-04 12:37:26.771402 types-aiobotocore-codecatalyst-2.5.2.post3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    12789 2023-08-04 12:20:06.000000 types-aiobotocore-codecatalyst-2.5.2.post3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-04 12:37:26.771402 types-aiobotocore-codecatalyst-2.5.2.post3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2107 2023-08-04 12:20:06.000000 types-aiobotocore-codecatalyst-2.5.2.post3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:37:26.771402 types-aiobotocore-codecatalyst-2.5.2.post3/types_aiobotocore_codecatalyst/
--rw-r--r--   0 runner    (1001) docker     (123)     2261 2023-08-04 12:20:06.000000 types-aiobotocore-codecatalyst-2.5.2.post3/types_aiobotocore_codecatalyst/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2260 2023-08-04 12:20:06.000000 types-aiobotocore-codecatalyst-2.5.2.post3/types_aiobotocore_codecatalyst/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      963 2023-08-04 12:20:06.000000 types-aiobotocore-codecatalyst-2.5.2.post3/types_aiobotocore_codecatalyst/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    25852 2023-08-04 12:20:06.000000 types-aiobotocore-codecatalyst-2.5.2.post3/types_aiobotocore_codecatalyst/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    25809 2023-08-04 12:20:06.000000 types-aiobotocore-codecatalyst-2.5.2.post3/types_aiobotocore_codecatalyst/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9385 2023-08-04 12:20:06.000000 types-aiobotocore-codecatalyst-2.5.2.post3/types_aiobotocore_codecatalyst/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     9383 2023-08-04 12:20:06.000000 types-aiobotocore-codecatalyst-2.5.2.post3/types_aiobotocore_codecatalyst/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    10771 2023-08-04 12:20:06.000000 types-aiobotocore-codecatalyst-2.5.2.post3/types_aiobotocore_codecatalyst/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)    10761 2023-08-04 12:20:06.000000 types-aiobotocore-codecatalyst-2.5.2.post3/types_aiobotocore_codecatalyst/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 12:20:06.000000 types-aiobotocore-codecatalyst-2.5.2.post3/types_aiobotocore_codecatalyst/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    34760 2023-08-04 12:20:07.000000 types-aiobotocore-codecatalyst-2.5.2.post3/types_aiobotocore_codecatalyst/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    34697 2023-08-04 12:20:07.000000 types-aiobotocore-codecatalyst-2.5.2.post3/types_aiobotocore_codecatalyst/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-04 12:20:06.000000 types-aiobotocore-codecatalyst-2.5.2.post3/types_aiobotocore_codecatalyst/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:37:26.771402 types-aiobotocore-codecatalyst-2.5.2.post3/types_aiobotocore_codecatalyst.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    14327 2023-08-04 12:37:26.000000 types-aiobotocore-codecatalyst-2.5.2.post3/types_aiobotocore_codecatalyst.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      908 2023-08-04 12:37:26.000000 types-aiobotocore-codecatalyst-2.5.2.post3/types_aiobotocore_codecatalyst.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 12:37:26.000000 types-aiobotocore-codecatalyst-2.5.2.post3/types_aiobotocore_codecatalyst.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 12:37:26.000000 types-aiobotocore-codecatalyst-2.5.2.post3/types_aiobotocore_codecatalyst.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-04 12:37:26.000000 types-aiobotocore-codecatalyst-2.5.2.post3/types_aiobotocore_codecatalyst.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-08-04 12:37:26.000000 types-aiobotocore-codecatalyst-2.5.2.post3/types_aiobotocore_codecatalyst.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:23:28.790644 types-aiobotocore-codecatalyst-2.5.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-08 01:07:46.000000 types-aiobotocore-codecatalyst-2.5.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    14321 2023-08-08 01:23:28.790644 types-aiobotocore-codecatalyst-2.5.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    12789 2023-08-08 01:07:46.000000 types-aiobotocore-codecatalyst-2.5.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-08 01:23:28.790644 types-aiobotocore-codecatalyst-2.5.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2101 2023-08-08 01:07:46.000000 types-aiobotocore-codecatalyst-2.5.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:23:28.786644 types-aiobotocore-codecatalyst-2.5.4/types_aiobotocore_codecatalyst/
+-rw-r--r--   0 runner    (1001) docker     (123)     2261 2023-08-08 01:07:46.000000 types-aiobotocore-codecatalyst-2.5.4/types_aiobotocore_codecatalyst/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2260 2023-08-08 01:07:46.000000 types-aiobotocore-codecatalyst-2.5.4/types_aiobotocore_codecatalyst/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      951 2023-08-08 01:07:46.000000 types-aiobotocore-codecatalyst-2.5.4/types_aiobotocore_codecatalyst/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29789 2023-08-08 01:07:46.000000 types-aiobotocore-codecatalyst-2.5.4/types_aiobotocore_codecatalyst/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29739 2023-08-08 01:07:46.000000 types-aiobotocore-codecatalyst-2.5.4/types_aiobotocore_codecatalyst/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9480 2023-08-08 01:07:47.000000 types-aiobotocore-codecatalyst-2.5.4/types_aiobotocore_codecatalyst/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9478 2023-08-08 01:07:46.000000 types-aiobotocore-codecatalyst-2.5.4/types_aiobotocore_codecatalyst/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    10771 2023-08-08 01:07:46.000000 types-aiobotocore-codecatalyst-2.5.4/types_aiobotocore_codecatalyst/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10761 2023-08-08 01:07:46.000000 types-aiobotocore-codecatalyst-2.5.4/types_aiobotocore_codecatalyst/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 01:07:46.000000 types-aiobotocore-codecatalyst-2.5.4/types_aiobotocore_codecatalyst/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    39261 2023-08-08 01:07:47.000000 types-aiobotocore-codecatalyst-2.5.4/types_aiobotocore_codecatalyst/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39192 2023-08-08 01:07:47.000000 types-aiobotocore-codecatalyst-2.5.4/types_aiobotocore_codecatalyst/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-08-08 01:07:46.000000 types-aiobotocore-codecatalyst-2.5.4/types_aiobotocore_codecatalyst/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:23:28.790644 types-aiobotocore-codecatalyst-2.5.4/types_aiobotocore_codecatalyst.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    14321 2023-08-08 01:23:28.000000 types-aiobotocore-codecatalyst-2.5.4/types_aiobotocore_codecatalyst.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      908 2023-08-08 01:23:28.000000 types-aiobotocore-codecatalyst-2.5.4/types_aiobotocore_codecatalyst.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 01:23:28.000000 types-aiobotocore-codecatalyst-2.5.4/types_aiobotocore_codecatalyst.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 01:23:28.000000 types-aiobotocore-codecatalyst-2.5.4/types_aiobotocore_codecatalyst.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-08 01:23:28.000000 types-aiobotocore-codecatalyst-2.5.4/types_aiobotocore_codecatalyst.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-08-08 01:23:28.000000 types-aiobotocore-codecatalyst-2.5.4/types_aiobotocore_codecatalyst.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-codecatalyst-2.5.2.post3/LICENSE` & `types-aiobotocore-codecatalyst-2.5.4/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-codecatalyst-2.5.2.post3/PKG-INFO` & `types-aiobotocore-codecatalyst-2.5.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-codecatalyst
-Version: 2.5.2.post3
-Summary: Type annotations for aiobotocore.CodeCatalyst 2.5.2 service generated with mypy-boto3-builder 7.17.2
+Version: 2.5.4
+Summary: Type annotations for aiobotocore.CodeCatalyst 2.5.4 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codecatalyst/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-codecatalyst.svg?color=blue)](https://pypi.org/project/types-aiobotocore-codecatalyst)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codecatalyst/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-codecatalyst)](https://pepy.tech/project/types-aiobotocore-codecatalyst)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.CodeCatalyst 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codecatalyst.html#CodeCatalyst)
+[aiobotocore.CodeCatalyst 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codecatalyst.html#CodeCatalyst)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-codecatalyst-2.5.2.post3/README.md` & `types-aiobotocore-codecatalyst-2.5.4/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-codecatalyst.svg?color=blue)](https://pypi.org/project/types-aiobotocore-codecatalyst)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codecatalyst/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-codecatalyst)](https://pepy.tech/project/types-aiobotocore-codecatalyst)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.CodeCatalyst 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codecatalyst.html#CodeCatalyst)
+[aiobotocore.CodeCatalyst 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codecatalyst.html#CodeCatalyst)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-codecatalyst-2.5.2.post3/setup.py` & `types-aiobotocore-codecatalyst-2.5.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-codecatalyst",
-    version="2.5.2.post3",
+    version="2.5.4",
     packages=["types_aiobotocore_codecatalyst"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.CodeCatalyst 2.5.2 service generated with"
+        "Type annotations for aiobotocore.CodeCatalyst 2.5.4 service generated with"
         " mypy-boto3-builder 7.17.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
```

### Comparing `types-aiobotocore-codecatalyst-2.5.2.post3/types_aiobotocore_codecatalyst/__init__.py` & `types-aiobotocore-codecatalyst-2.5.4/types_aiobotocore_codecatalyst/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-codecatalyst-2.5.2.post3/types_aiobotocore_codecatalyst/__init__.pyi` & `types-aiobotocore-codecatalyst-2.5.4/types_aiobotocore_codecatalyst/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-codecatalyst-2.5.2.post3/types_aiobotocore_codecatalyst/__main__.py` & `types-aiobotocore-codecatalyst-2.5.4/types_aiobotocore_codecatalyst/__main__.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.CodeCatalyst 2.5.2\nVersion:         2.5.2.post3\nBuilder"
+        "Type annotations for aiobotocore.CodeCatalyst 2.5.4\nVersion:         2.5.4\nBuilder"
         " version: 7.17.2\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codecatalyst//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codecatalyst.html#CodeCatalyst\nOther"
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

### Comparing `types-aiobotocore-codecatalyst-2.5.2.post3/types_aiobotocore_codecatalyst/client.py` & `types-aiobotocore-codecatalyst-2.5.4/types_aiobotocore_codecatalyst/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,20 +32,25 @@
     ListSpacesPaginator,
 )
 from .type_defs import (
     CreateAccessTokenResponseTypeDef,
     CreateDevEnvironmentResponseTypeDef,
     CreateProjectResponseTypeDef,
     CreateSourceRepositoryBranchResponseTypeDef,
+    CreateSourceRepositoryResponseTypeDef,
     DeleteDevEnvironmentResponseTypeDef,
+    DeleteProjectResponseTypeDef,
+    DeleteSourceRepositoryResponseTypeDef,
+    DeleteSpaceResponseTypeDef,
     DevEnvironmentSessionConfigurationTypeDef,
     FilterTypeDef,
     GetDevEnvironmentResponseTypeDef,
     GetProjectResponseTypeDef,
     GetSourceRepositoryCloneUrlsResponseTypeDef,
+    GetSourceRepositoryResponseTypeDef,
     GetSpaceResponseTypeDef,
     GetSubscriptionResponseTypeDef,
     GetUserDetailsResponseTypeDef,
     IdeConfigurationTypeDef,
     ListAccessTokensResponseTypeDef,
     ListDevEnvironmentSessionsResponseTypeDef,
     ListDevEnvironmentsResponseTypeDef,
@@ -59,14 +64,16 @@
     RepositoryInputTypeDef,
     StartDevEnvironmentResponseTypeDef,
     StartDevEnvironmentSessionResponseTypeDef,
     StopDevEnvironmentResponseTypeDef,
     StopDevEnvironmentSessionResponseTypeDef,
     TimestampTypeDef,
     UpdateDevEnvironmentResponseTypeDef,
+    UpdateProjectResponseTypeDef,
+    UpdateSpaceResponseTypeDef,
     VerifySessionResponseTypeDef,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
@@ -164,14 +171,24 @@
         """
         Creates a project in a specified space.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codecatalyst.html#CodeCatalyst.Client.create_project)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codecatalyst/client/#create_project)
         """
 
+    async def create_source_repository(
+        self, *, spaceName: str, projectName: str, name: str, description: str = ...
+    ) -> CreateSourceRepositoryResponseTypeDef:
+        """
+        Creates an empty Git-based source repository in a specified project.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codecatalyst.html#CodeCatalyst.Client.create_source_repository)
+        [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codecatalyst/client/#create_source_repository)
+        """
+
     async def create_source_repository_branch(
         self,
         *,
         spaceName: str,
         projectName: str,
         sourceRepositoryName: str,
         name: str,
@@ -198,14 +215,40 @@
         """
         Deletes a Dev Environment.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codecatalyst.html#CodeCatalyst.Client.delete_dev_environment)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codecatalyst/client/#delete_dev_environment)
         """
 
+    async def delete_project(self, *, spaceName: str, name: str) -> DeleteProjectResponseTypeDef:
+        """
+        Deletes a project in a space.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codecatalyst.html#CodeCatalyst.Client.delete_project)
+        [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codecatalyst/client/#delete_project)
+        """
+
+    async def delete_source_repository(
+        self, *, spaceName: str, projectName: str, name: str
+    ) -> DeleteSourceRepositoryResponseTypeDef:
+        """
+        Deletes a source repository in Amazon CodeCatalyst.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codecatalyst.html#CodeCatalyst.Client.delete_source_repository)
+        [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codecatalyst/client/#delete_source_repository)
+        """
+
+    async def delete_space(self, *, name: str) -> DeleteSpaceResponseTypeDef:
+        """
+        Deletes a space.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codecatalyst.html#CodeCatalyst.Client.delete_space)
+        [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codecatalyst/client/#delete_space)
+        """
+
     async def generate_presigned_url(
         self,
         ClientMethod: str,
         Params: Mapping[str, Any] = ...,
         ExpiresIn: int = 3600,
         HttpMethod: str = ...,
     ) -> str:
@@ -231,14 +274,24 @@
         """
         Returns information about a project.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codecatalyst.html#CodeCatalyst.Client.get_project)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codecatalyst/client/#get_project)
         """
 
+    async def get_source_repository(
+        self, *, spaceName: str, projectName: str, name: str
+    ) -> GetSourceRepositoryResponseTypeDef:
+        """
+        Returns information about a source repository.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codecatalyst.html#CodeCatalyst.Client.get_source_repository)
+        [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codecatalyst/client/#get_source_repository)
+        """
+
     async def get_source_repository_clone_urls(
         self, *, spaceName: str, projectName: str, sourceRepositoryName: str
     ) -> GetSourceRepositoryCloneUrlsResponseTypeDef:
         """
         Returns information about the URLs that can be used with a Git client to clone a
         source repository.
 
@@ -450,14 +503,34 @@
         """
         Changes one or more values for a Dev Environment.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codecatalyst.html#CodeCatalyst.Client.update_dev_environment)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codecatalyst/client/#update_dev_environment)
         """
 
+    async def update_project(
+        self, *, spaceName: str, name: str, description: str = ...
+    ) -> UpdateProjectResponseTypeDef:
+        """
+        Changes one or more values for a project.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codecatalyst.html#CodeCatalyst.Client.update_project)
+        [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codecatalyst/client/#update_project)
+        """
+
+    async def update_space(
+        self, *, name: str, description: str = ...
+    ) -> UpdateSpaceResponseTypeDef:
+        """
+        Changes one or more values for a space.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codecatalyst.html#CodeCatalyst.Client.update_space)
+        [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codecatalyst/client/#update_space)
+        """
+
     async def verify_session(self) -> VerifySessionResponseTypeDef:
         """
         Verifies whether the calling user has a valid Amazon CodeCatalyst login and
         session.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codecatalyst.html#CodeCatalyst.Client.verify_session)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codecatalyst/client/#verify_session)
```

### Comparing `types-aiobotocore-codecatalyst-2.5.2.post3/types_aiobotocore_codecatalyst/client.pyi` & `types-aiobotocore-codecatalyst-2.5.4/types_aiobotocore_codecatalyst/client.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -32,20 +32,25 @@
     ListSpacesPaginator,
 )
 from .type_defs import (
     CreateAccessTokenResponseTypeDef,
     CreateDevEnvironmentResponseTypeDef,
     CreateProjectResponseTypeDef,
     CreateSourceRepositoryBranchResponseTypeDef,
+    CreateSourceRepositoryResponseTypeDef,
     DeleteDevEnvironmentResponseTypeDef,
+    DeleteProjectResponseTypeDef,
+    DeleteSourceRepositoryResponseTypeDef,
+    DeleteSpaceResponseTypeDef,
     DevEnvironmentSessionConfigurationTypeDef,
     FilterTypeDef,
     GetDevEnvironmentResponseTypeDef,
     GetProjectResponseTypeDef,
     GetSourceRepositoryCloneUrlsResponseTypeDef,
+    GetSourceRepositoryResponseTypeDef,
     GetSpaceResponseTypeDef,
     GetSubscriptionResponseTypeDef,
     GetUserDetailsResponseTypeDef,
     IdeConfigurationTypeDef,
     ListAccessTokensResponseTypeDef,
     ListDevEnvironmentSessionsResponseTypeDef,
     ListDevEnvironmentsResponseTypeDef,
@@ -59,14 +64,16 @@
     RepositoryInputTypeDef,
     StartDevEnvironmentResponseTypeDef,
     StartDevEnvironmentSessionResponseTypeDef,
     StopDevEnvironmentResponseTypeDef,
     StopDevEnvironmentSessionResponseTypeDef,
     TimestampTypeDef,
     UpdateDevEnvironmentResponseTypeDef,
+    UpdateProjectResponseTypeDef,
+    UpdateSpaceResponseTypeDef,
     VerifySessionResponseTypeDef,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
@@ -154,14 +161,23 @@
     ) -> CreateProjectResponseTypeDef:
         """
         Creates a project in a specified space.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codecatalyst.html#CodeCatalyst.Client.create_project)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codecatalyst/client/#create_project)
         """
+    async def create_source_repository(
+        self, *, spaceName: str, projectName: str, name: str, description: str = ...
+    ) -> CreateSourceRepositoryResponseTypeDef:
+        """
+        Creates an empty Git-based source repository in a specified project.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codecatalyst.html#CodeCatalyst.Client.create_source_repository)
+        [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codecatalyst/client/#create_source_repository)
+        """
     async def create_source_repository_branch(
         self,
         *,
         spaceName: str,
         projectName: str,
         sourceRepositoryName: str,
         name: str,
@@ -185,14 +201,37 @@
     ) -> DeleteDevEnvironmentResponseTypeDef:
         """
         Deletes a Dev Environment.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codecatalyst.html#CodeCatalyst.Client.delete_dev_environment)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codecatalyst/client/#delete_dev_environment)
         """
+    async def delete_project(self, *, spaceName: str, name: str) -> DeleteProjectResponseTypeDef:
+        """
+        Deletes a project in a space.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codecatalyst.html#CodeCatalyst.Client.delete_project)
+        [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codecatalyst/client/#delete_project)
+        """
+    async def delete_source_repository(
+        self, *, spaceName: str, projectName: str, name: str
+    ) -> DeleteSourceRepositoryResponseTypeDef:
+        """
+        Deletes a source repository in Amazon CodeCatalyst.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codecatalyst.html#CodeCatalyst.Client.delete_source_repository)
+        [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codecatalyst/client/#delete_source_repository)
+        """
+    async def delete_space(self, *, name: str) -> DeleteSpaceResponseTypeDef:
+        """
+        Deletes a space.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codecatalyst.html#CodeCatalyst.Client.delete_space)
+        [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codecatalyst/client/#delete_space)
+        """
     async def generate_presigned_url(
         self,
         ClientMethod: str,
         Params: Mapping[str, Any] = ...,
         ExpiresIn: int = 3600,
         HttpMethod: str = ...,
     ) -> str:
@@ -215,14 +254,23 @@
     async def get_project(self, *, spaceName: str, name: str) -> GetProjectResponseTypeDef:
         """
         Returns information about a project.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codecatalyst.html#CodeCatalyst.Client.get_project)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codecatalyst/client/#get_project)
         """
+    async def get_source_repository(
+        self, *, spaceName: str, projectName: str, name: str
+    ) -> GetSourceRepositoryResponseTypeDef:
+        """
+        Returns information about a source repository.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codecatalyst.html#CodeCatalyst.Client.get_source_repository)
+        [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codecatalyst/client/#get_source_repository)
+        """
     async def get_source_repository_clone_urls(
         self, *, spaceName: str, projectName: str, sourceRepositoryName: str
     ) -> GetSourceRepositoryCloneUrlsResponseTypeDef:
         """
         Returns information about the URLs that can be used with a Git client to clone a
         source repository.
 
@@ -417,14 +465,32 @@
     ) -> UpdateDevEnvironmentResponseTypeDef:
         """
         Changes one or more values for a Dev Environment.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codecatalyst.html#CodeCatalyst.Client.update_dev_environment)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codecatalyst/client/#update_dev_environment)
         """
+    async def update_project(
+        self, *, spaceName: str, name: str, description: str = ...
+    ) -> UpdateProjectResponseTypeDef:
+        """
+        Changes one or more values for a project.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codecatalyst.html#CodeCatalyst.Client.update_project)
+        [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codecatalyst/client/#update_project)
+        """
+    async def update_space(
+        self, *, name: str, description: str = ...
+    ) -> UpdateSpaceResponseTypeDef:
+        """
+        Changes one or more values for a space.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codecatalyst.html#CodeCatalyst.Client.update_space)
+        [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codecatalyst/client/#update_space)
+        """
     async def verify_session(self) -> VerifySessionResponseTypeDef:
         """
         Verifies whether the calling user has a valid Amazon CodeCatalyst login and
         session.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codecatalyst.html#CodeCatalyst.Client.verify_session)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codecatalyst/client/#verify_session)
```

### Comparing `types-aiobotocore-codecatalyst-2.5.2.post3/types_aiobotocore_codecatalyst/literals.py` & `types-aiobotocore-codecatalyst-2.5.4/types_aiobotocore_codecatalyst/literals.pyi`

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
     "ComparisonOperatorType",
     "DevEnvironmentSessionTypeType",
     "DevEnvironmentStatusType",
     "FilterKeyType",
     "InstanceTypeType",
     "ListAccessTokensPaginatorName",
@@ -37,15 +36,14 @@
     "UserTypeType",
     "CodeCatalystServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
 )
 
-
 ComparisonOperatorType = Literal["EQ", "GE", "GT", "LE", "LT"]
 DevEnvironmentSessionTypeType = Literal["SSH", "SSM"]
 DevEnvironmentStatusType = Literal[
     "DELETED", "DELETING", "FAILED", "PENDING", "RUNNING", "STARTING", "STOPPED", "STOPPING"
 ]
 FilterKeyType = Literal["hasAccessTo"]
 InstanceTypeType = Literal[
@@ -73,14 +71,15 @@
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
@@ -176,14 +175,15 @@
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
@@ -262,26 +262,28 @@
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

### Comparing `types-aiobotocore-codecatalyst-2.5.2.post3/types_aiobotocore_codecatalyst/literals.pyi` & `types-aiobotocore-codecatalyst-2.5.4/types_aiobotocore_codecatalyst/literals.py`

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
     "ComparisonOperatorType",
     "DevEnvironmentSessionTypeType",
     "DevEnvironmentStatusType",
     "FilterKeyType",
     "InstanceTypeType",
     "ListAccessTokensPaginatorName",
@@ -36,14 +37,15 @@
     "UserTypeType",
     "CodeCatalystServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
 )
 
+
 ComparisonOperatorType = Literal["EQ", "GE", "GT", "LE", "LT"]
 DevEnvironmentSessionTypeType = Literal["SSH", "SSM"]
 DevEnvironmentStatusType = Literal[
     "DELETED", "DELETING", "FAILED", "PENDING", "RUNNING", "STARTING", "STOPPED", "STOPPING"
 ]
 FilterKeyType = Literal["hasAccessTo"]
 InstanceTypeType = Literal[
@@ -71,14 +73,15 @@
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
@@ -174,14 +177,15 @@
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
@@ -260,26 +264,28 @@
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

### Comparing `types-aiobotocore-codecatalyst-2.5.2.post3/types_aiobotocore_codecatalyst/paginator.py` & `types-aiobotocore-codecatalyst-2.5.4/types_aiobotocore_codecatalyst/paginator.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-codecatalyst-2.5.2.post3/types_aiobotocore_codecatalyst/paginator.pyi` & `types-aiobotocore-codecatalyst-2.5.4/types_aiobotocore_codecatalyst/paginator.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-codecatalyst-2.5.2.post3/types_aiobotocore_codecatalyst/type_defs.py` & `types-aiobotocore-codecatalyst-2.5.4/types_aiobotocore_codecatalyst/type_defs.py`

 * *Files 3% similar despite different names*

```diff
@@ -39,30 +39,35 @@
     "TimestampTypeDef",
     "ResponseMetadataTypeDef",
     "IdeConfigurationTypeDef",
     "PersistentStorageConfigurationTypeDef",
     "RepositoryInputTypeDef",
     "CreateProjectRequestRequestTypeDef",
     "CreateSourceRepositoryBranchRequestRequestTypeDef",
+    "CreateSourceRepositoryRequestRequestTypeDef",
     "DeleteAccessTokenRequestRequestTypeDef",
     "DeleteDevEnvironmentRequestRequestTypeDef",
+    "DeleteProjectRequestRequestTypeDef",
+    "DeleteSourceRepositoryRequestRequestTypeDef",
+    "DeleteSpaceRequestRequestTypeDef",
     "DevEnvironmentAccessDetailsTypeDef",
     "DevEnvironmentRepositorySummaryTypeDef",
     "ExecuteCommandSessionConfigurationTypeDef",
     "DevEnvironmentSessionSummaryTypeDef",
     "IdeTypeDef",
     "PersistentStorageTypeDef",
     "EmailAddressTypeDef",
     "EventPayloadTypeDef",
     "ProjectInformationTypeDef",
     "UserIdentityTypeDef",
     "FilterTypeDef",
     "GetDevEnvironmentRequestRequestTypeDef",
     "GetProjectRequestRequestTypeDef",
     "GetSourceRepositoryCloneUrlsRequestRequestTypeDef",
+    "GetSourceRepositoryRequestRequestTypeDef",
     "GetSpaceRequestRequestTypeDef",
     "GetSubscriptionRequestRequestTypeDef",
     "GetUserDetailsRequestRequestTypeDef",
     "PaginatorConfigTypeDef",
     "ListAccessTokensRequestRequestTypeDef",
     "ListDevEnvironmentSessionsRequestRequestTypeDef",
     "ProjectListFilterTypeDef",
@@ -71,29 +76,38 @@
     "ListSourceRepositoriesRequestRequestTypeDef",
     "ListSourceRepositoryBranchesItemTypeDef",
     "ListSourceRepositoryBranchesRequestRequestTypeDef",
     "ListSpacesRequestRequestTypeDef",
     "SpaceSummaryTypeDef",
     "StopDevEnvironmentRequestRequestTypeDef",
     "StopDevEnvironmentSessionRequestRequestTypeDef",
+    "UpdateProjectRequestRequestTypeDef",
+    "UpdateSpaceRequestRequestTypeDef",
     "CreateAccessTokenRequestRequestTypeDef",
     "ListEventLogsRequestRequestTypeDef",
     "CreateAccessTokenResponseTypeDef",
     "CreateDevEnvironmentResponseTypeDef",
     "CreateProjectResponseTypeDef",
     "CreateSourceRepositoryBranchResponseTypeDef",
+    "CreateSourceRepositoryResponseTypeDef",
     "DeleteDevEnvironmentResponseTypeDef",
+    "DeleteProjectResponseTypeDef",
+    "DeleteSourceRepositoryResponseTypeDef",
+    "DeleteSpaceResponseTypeDef",
     "GetProjectResponseTypeDef",
     "GetSourceRepositoryCloneUrlsResponseTypeDef",
+    "GetSourceRepositoryResponseTypeDef",
     "GetSpaceResponseTypeDef",
     "GetSubscriptionResponseTypeDef",
     "ListAccessTokensResponseTypeDef",
     "StartDevEnvironmentResponseTypeDef",
     "StopDevEnvironmentResponseTypeDef",
     "StopDevEnvironmentSessionResponseTypeDef",
+    "UpdateProjectResponseTypeDef",
+    "UpdateSpaceResponseTypeDef",
     "VerifySessionResponseTypeDef",
     "StartDevEnvironmentRequestRequestTypeDef",
     "UpdateDevEnvironmentRequestRequestTypeDef",
     "UpdateDevEnvironmentResponseTypeDef",
     "CreateDevEnvironmentRequestRequestTypeDef",
     "StartDevEnvironmentSessionResponseTypeDef",
     "DevEnvironmentSessionConfigurationTypeDef",
@@ -233,14 +247,38 @@
 class CreateSourceRepositoryBranchRequestRequestTypeDef(
     _RequiredCreateSourceRepositoryBranchRequestRequestTypeDef,
     _OptionalCreateSourceRepositoryBranchRequestRequestTypeDef,
 ):
     pass
 
 
+_RequiredCreateSourceRepositoryRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateSourceRepositoryRequestRequestTypeDef",
+    {
+        "spaceName": str,
+        "projectName": str,
+        "name": str,
+    },
+)
+_OptionalCreateSourceRepositoryRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateSourceRepositoryRequestRequestTypeDef",
+    {
+        "description": str,
+    },
+    total=False,
+)
+
+
+class CreateSourceRepositoryRequestRequestTypeDef(
+    _RequiredCreateSourceRepositoryRequestRequestTypeDef,
+    _OptionalCreateSourceRepositoryRequestRequestTypeDef,
+):
+    pass
+
+
 DeleteAccessTokenRequestRequestTypeDef = TypedDict(
     "DeleteAccessTokenRequestRequestTypeDef",
     {
         "id": str,
     },
 )
 
@@ -249,14 +287,38 @@
     {
         "spaceName": str,
         "projectName": str,
         "id": str,
     },
 )
 
+DeleteProjectRequestRequestTypeDef = TypedDict(
+    "DeleteProjectRequestRequestTypeDef",
+    {
+        "spaceName": str,
+        "name": str,
+    },
+)
+
+DeleteSourceRepositoryRequestRequestTypeDef = TypedDict(
+    "DeleteSourceRepositoryRequestRequestTypeDef",
+    {
+        "spaceName": str,
+        "projectName": str,
+        "name": str,
+    },
+)
+
+DeleteSpaceRequestRequestTypeDef = TypedDict(
+    "DeleteSpaceRequestRequestTypeDef",
+    {
+        "name": str,
+    },
+)
+
 DevEnvironmentAccessDetailsTypeDef = TypedDict(
     "DevEnvironmentAccessDetailsTypeDef",
     {
         "streamUrl": str,
         "tokenValue": str,
     },
 )
@@ -421,14 +483,23 @@
     {
         "spaceName": str,
         "projectName": str,
         "sourceRepositoryName": str,
     },
 )
 
+GetSourceRepositoryRequestRequestTypeDef = TypedDict(
+    "GetSourceRepositoryRequestRequestTypeDef",
+    {
+        "spaceName": str,
+        "projectName": str,
+        "name": str,
+    },
+)
+
 GetSpaceRequestRequestTypeDef = TypedDict(
     "GetSpaceRequestRequestTypeDef",
     {
         "name": str,
     },
 )
 
@@ -662,14 +733,57 @@
         "spaceName": str,
         "projectName": str,
         "id": str,
         "sessionId": str,
     },
 )
 
+_RequiredUpdateProjectRequestRequestTypeDef = TypedDict(
+    "_RequiredUpdateProjectRequestRequestTypeDef",
+    {
+        "spaceName": str,
+        "name": str,
+    },
+)
+_OptionalUpdateProjectRequestRequestTypeDef = TypedDict(
+    "_OptionalUpdateProjectRequestRequestTypeDef",
+    {
+        "description": str,
+    },
+    total=False,
+)
+
+
+class UpdateProjectRequestRequestTypeDef(
+    _RequiredUpdateProjectRequestRequestTypeDef, _OptionalUpdateProjectRequestRequestTypeDef
+):
+    pass
+
+
+_RequiredUpdateSpaceRequestRequestTypeDef = TypedDict(
+    "_RequiredUpdateSpaceRequestRequestTypeDef",
+    {
+        "name": str,
+    },
+)
+_OptionalUpdateSpaceRequestRequestTypeDef = TypedDict(
+    "_OptionalUpdateSpaceRequestRequestTypeDef",
+    {
+        "description": str,
+    },
+    total=False,
+)
+
+
+class UpdateSpaceRequestRequestTypeDef(
+    _RequiredUpdateSpaceRequestRequestTypeDef, _OptionalUpdateSpaceRequestRequestTypeDef
+):
+    pass
+
+
 _RequiredCreateAccessTokenRequestRequestTypeDef = TypedDict(
     "_RequiredCreateAccessTokenRequestRequestTypeDef",
     {
         "name": str,
     },
 )
 _OptionalCreateAccessTokenRequestRequestTypeDef = TypedDict(
@@ -751,24 +865,64 @@
         "name": str,
         "lastUpdatedTime": datetime,
         "headCommitId": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+CreateSourceRepositoryResponseTypeDef = TypedDict(
+    "CreateSourceRepositoryResponseTypeDef",
+    {
+        "spaceName": str,
+        "projectName": str,
+        "name": str,
+        "description": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 DeleteDevEnvironmentResponseTypeDef = TypedDict(
     "DeleteDevEnvironmentResponseTypeDef",
     {
         "spaceName": str,
         "projectName": str,
         "id": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+DeleteProjectResponseTypeDef = TypedDict(
+    "DeleteProjectResponseTypeDef",
+    {
+        "spaceName": str,
+        "name": str,
+        "displayName": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DeleteSourceRepositoryResponseTypeDef = TypedDict(
+    "DeleteSourceRepositoryResponseTypeDef",
+    {
+        "spaceName": str,
+        "projectName": str,
+        "name": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DeleteSpaceResponseTypeDef = TypedDict(
+    "DeleteSpaceResponseTypeDef",
+    {
+        "name": str,
+        "displayName": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 GetProjectResponseTypeDef = TypedDict(
     "GetProjectResponseTypeDef",
     {
         "spaceName": str,
         "name": str,
         "displayName": str,
         "description": str,
@@ -780,14 +934,27 @@
     "GetSourceRepositoryCloneUrlsResponseTypeDef",
     {
         "https": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+GetSourceRepositoryResponseTypeDef = TypedDict(
+    "GetSourceRepositoryResponseTypeDef",
+    {
+        "spaceName": str,
+        "projectName": str,
+        "name": str,
+        "description": str,
+        "lastUpdatedTime": datetime,
+        "createdTime": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 GetSpaceResponseTypeDef = TypedDict(
     "GetSpaceResponseTypeDef",
     {
         "name": str,
         "regionName": str,
         "displayName": str,
         "description": str,
@@ -842,14 +1009,35 @@
         "projectName": str,
         "id": str,
         "sessionId": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+UpdateProjectResponseTypeDef = TypedDict(
+    "UpdateProjectResponseTypeDef",
+    {
+        "spaceName": str,
+        "name": str,
+        "displayName": str,
+        "description": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateSpaceResponseTypeDef = TypedDict(
+    "UpdateSpaceResponseTypeDef",
+    {
+        "name": str,
+        "displayName": str,
+        "description": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 VerifySessionResponseTypeDef = TypedDict(
     "VerifySessionResponseTypeDef",
     {
         "identity": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `types-aiobotocore-codecatalyst-2.5.2.post3/types_aiobotocore_codecatalyst/type_defs.pyi` & `types-aiobotocore-codecatalyst-2.5.4/types_aiobotocore_codecatalyst/type_defs.pyi`

 * *Files 3% similar despite different names*

```diff
@@ -38,30 +38,35 @@
     "TimestampTypeDef",
     "ResponseMetadataTypeDef",
     "IdeConfigurationTypeDef",
     "PersistentStorageConfigurationTypeDef",
     "RepositoryInputTypeDef",
     "CreateProjectRequestRequestTypeDef",
     "CreateSourceRepositoryBranchRequestRequestTypeDef",
+    "CreateSourceRepositoryRequestRequestTypeDef",
     "DeleteAccessTokenRequestRequestTypeDef",
     "DeleteDevEnvironmentRequestRequestTypeDef",
+    "DeleteProjectRequestRequestTypeDef",
+    "DeleteSourceRepositoryRequestRequestTypeDef",
+    "DeleteSpaceRequestRequestTypeDef",
     "DevEnvironmentAccessDetailsTypeDef",
     "DevEnvironmentRepositorySummaryTypeDef",
     "ExecuteCommandSessionConfigurationTypeDef",
     "DevEnvironmentSessionSummaryTypeDef",
     "IdeTypeDef",
     "PersistentStorageTypeDef",
     "EmailAddressTypeDef",
     "EventPayloadTypeDef",
     "ProjectInformationTypeDef",
     "UserIdentityTypeDef",
     "FilterTypeDef",
     "GetDevEnvironmentRequestRequestTypeDef",
     "GetProjectRequestRequestTypeDef",
     "GetSourceRepositoryCloneUrlsRequestRequestTypeDef",
+    "GetSourceRepositoryRequestRequestTypeDef",
     "GetSpaceRequestRequestTypeDef",
     "GetSubscriptionRequestRequestTypeDef",
     "GetUserDetailsRequestRequestTypeDef",
     "PaginatorConfigTypeDef",
     "ListAccessTokensRequestRequestTypeDef",
     "ListDevEnvironmentSessionsRequestRequestTypeDef",
     "ProjectListFilterTypeDef",
@@ -70,29 +75,38 @@
     "ListSourceRepositoriesRequestRequestTypeDef",
     "ListSourceRepositoryBranchesItemTypeDef",
     "ListSourceRepositoryBranchesRequestRequestTypeDef",
     "ListSpacesRequestRequestTypeDef",
     "SpaceSummaryTypeDef",
     "StopDevEnvironmentRequestRequestTypeDef",
     "StopDevEnvironmentSessionRequestRequestTypeDef",
+    "UpdateProjectRequestRequestTypeDef",
+    "UpdateSpaceRequestRequestTypeDef",
     "CreateAccessTokenRequestRequestTypeDef",
     "ListEventLogsRequestRequestTypeDef",
     "CreateAccessTokenResponseTypeDef",
     "CreateDevEnvironmentResponseTypeDef",
     "CreateProjectResponseTypeDef",
     "CreateSourceRepositoryBranchResponseTypeDef",
+    "CreateSourceRepositoryResponseTypeDef",
     "DeleteDevEnvironmentResponseTypeDef",
+    "DeleteProjectResponseTypeDef",
+    "DeleteSourceRepositoryResponseTypeDef",
+    "DeleteSpaceResponseTypeDef",
     "GetProjectResponseTypeDef",
     "GetSourceRepositoryCloneUrlsResponseTypeDef",
+    "GetSourceRepositoryResponseTypeDef",
     "GetSpaceResponseTypeDef",
     "GetSubscriptionResponseTypeDef",
     "ListAccessTokensResponseTypeDef",
     "StartDevEnvironmentResponseTypeDef",
     "StopDevEnvironmentResponseTypeDef",
     "StopDevEnvironmentSessionResponseTypeDef",
+    "UpdateProjectResponseTypeDef",
+    "UpdateSpaceResponseTypeDef",
     "VerifySessionResponseTypeDef",
     "StartDevEnvironmentRequestRequestTypeDef",
     "UpdateDevEnvironmentRequestRequestTypeDef",
     "UpdateDevEnvironmentResponseTypeDef",
     "CreateDevEnvironmentRequestRequestTypeDef",
     "StartDevEnvironmentSessionResponseTypeDef",
     "DevEnvironmentSessionConfigurationTypeDef",
@@ -224,14 +238,36 @@
 
 class CreateSourceRepositoryBranchRequestRequestTypeDef(
     _RequiredCreateSourceRepositoryBranchRequestRequestTypeDef,
     _OptionalCreateSourceRepositoryBranchRequestRequestTypeDef,
 ):
     pass
 
+_RequiredCreateSourceRepositoryRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateSourceRepositoryRequestRequestTypeDef",
+    {
+        "spaceName": str,
+        "projectName": str,
+        "name": str,
+    },
+)
+_OptionalCreateSourceRepositoryRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateSourceRepositoryRequestRequestTypeDef",
+    {
+        "description": str,
+    },
+    total=False,
+)
+
+class CreateSourceRepositoryRequestRequestTypeDef(
+    _RequiredCreateSourceRepositoryRequestRequestTypeDef,
+    _OptionalCreateSourceRepositoryRequestRequestTypeDef,
+):
+    pass
+
 DeleteAccessTokenRequestRequestTypeDef = TypedDict(
     "DeleteAccessTokenRequestRequestTypeDef",
     {
         "id": str,
     },
 )
 
@@ -240,14 +276,38 @@
     {
         "spaceName": str,
         "projectName": str,
         "id": str,
     },
 )
 
+DeleteProjectRequestRequestTypeDef = TypedDict(
+    "DeleteProjectRequestRequestTypeDef",
+    {
+        "spaceName": str,
+        "name": str,
+    },
+)
+
+DeleteSourceRepositoryRequestRequestTypeDef = TypedDict(
+    "DeleteSourceRepositoryRequestRequestTypeDef",
+    {
+        "spaceName": str,
+        "projectName": str,
+        "name": str,
+    },
+)
+
+DeleteSpaceRequestRequestTypeDef = TypedDict(
+    "DeleteSpaceRequestRequestTypeDef",
+    {
+        "name": str,
+    },
+)
+
 DevEnvironmentAccessDetailsTypeDef = TypedDict(
     "DevEnvironmentAccessDetailsTypeDef",
     {
         "streamUrl": str,
         "tokenValue": str,
     },
 )
@@ -404,14 +464,23 @@
     {
         "spaceName": str,
         "projectName": str,
         "sourceRepositoryName": str,
     },
 )
 
+GetSourceRepositoryRequestRequestTypeDef = TypedDict(
+    "GetSourceRepositoryRequestRequestTypeDef",
+    {
+        "spaceName": str,
+        "projectName": str,
+        "name": str,
+    },
+)
+
 GetSpaceRequestRequestTypeDef = TypedDict(
     "GetSpaceRequestRequestTypeDef",
     {
         "name": str,
     },
 )
 
@@ -631,14 +700,53 @@
         "spaceName": str,
         "projectName": str,
         "id": str,
         "sessionId": str,
     },
 )
 
+_RequiredUpdateProjectRequestRequestTypeDef = TypedDict(
+    "_RequiredUpdateProjectRequestRequestTypeDef",
+    {
+        "spaceName": str,
+        "name": str,
+    },
+)
+_OptionalUpdateProjectRequestRequestTypeDef = TypedDict(
+    "_OptionalUpdateProjectRequestRequestTypeDef",
+    {
+        "description": str,
+    },
+    total=False,
+)
+
+class UpdateProjectRequestRequestTypeDef(
+    _RequiredUpdateProjectRequestRequestTypeDef, _OptionalUpdateProjectRequestRequestTypeDef
+):
+    pass
+
+_RequiredUpdateSpaceRequestRequestTypeDef = TypedDict(
+    "_RequiredUpdateSpaceRequestRequestTypeDef",
+    {
+        "name": str,
+    },
+)
+_OptionalUpdateSpaceRequestRequestTypeDef = TypedDict(
+    "_OptionalUpdateSpaceRequestRequestTypeDef",
+    {
+        "description": str,
+    },
+    total=False,
+)
+
+class UpdateSpaceRequestRequestTypeDef(
+    _RequiredUpdateSpaceRequestRequestTypeDef, _OptionalUpdateSpaceRequestRequestTypeDef
+):
+    pass
+
 _RequiredCreateAccessTokenRequestRequestTypeDef = TypedDict(
     "_RequiredCreateAccessTokenRequestRequestTypeDef",
     {
         "name": str,
     },
 )
 _OptionalCreateAccessTokenRequestRequestTypeDef = TypedDict(
@@ -716,24 +824,64 @@
         "name": str,
         "lastUpdatedTime": datetime,
         "headCommitId": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+CreateSourceRepositoryResponseTypeDef = TypedDict(
+    "CreateSourceRepositoryResponseTypeDef",
+    {
+        "spaceName": str,
+        "projectName": str,
+        "name": str,
+        "description": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 DeleteDevEnvironmentResponseTypeDef = TypedDict(
     "DeleteDevEnvironmentResponseTypeDef",
     {
         "spaceName": str,
         "projectName": str,
         "id": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+DeleteProjectResponseTypeDef = TypedDict(
+    "DeleteProjectResponseTypeDef",
+    {
+        "spaceName": str,
+        "name": str,
+        "displayName": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DeleteSourceRepositoryResponseTypeDef = TypedDict(
+    "DeleteSourceRepositoryResponseTypeDef",
+    {
+        "spaceName": str,
+        "projectName": str,
+        "name": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DeleteSpaceResponseTypeDef = TypedDict(
+    "DeleteSpaceResponseTypeDef",
+    {
+        "name": str,
+        "displayName": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 GetProjectResponseTypeDef = TypedDict(
     "GetProjectResponseTypeDef",
     {
         "spaceName": str,
         "name": str,
         "displayName": str,
         "description": str,
@@ -745,14 +893,27 @@
     "GetSourceRepositoryCloneUrlsResponseTypeDef",
     {
         "https": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+GetSourceRepositoryResponseTypeDef = TypedDict(
+    "GetSourceRepositoryResponseTypeDef",
+    {
+        "spaceName": str,
+        "projectName": str,
+        "name": str,
+        "description": str,
+        "lastUpdatedTime": datetime,
+        "createdTime": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 GetSpaceResponseTypeDef = TypedDict(
     "GetSpaceResponseTypeDef",
     {
         "name": str,
         "regionName": str,
         "displayName": str,
         "description": str,
@@ -807,14 +968,35 @@
         "projectName": str,
         "id": str,
         "sessionId": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+UpdateProjectResponseTypeDef = TypedDict(
+    "UpdateProjectResponseTypeDef",
+    {
+        "spaceName": str,
+        "name": str,
+        "displayName": str,
+        "description": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateSpaceResponseTypeDef = TypedDict(
+    "UpdateSpaceResponseTypeDef",
+    {
+        "name": str,
+        "displayName": str,
+        "description": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 VerifySessionResponseTypeDef = TypedDict(
     "VerifySessionResponseTypeDef",
     {
         "identity": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `types-aiobotocore-codecatalyst-2.5.2.post3/types_aiobotocore_codecatalyst.egg-info/PKG-INFO` & `types-aiobotocore-codecatalyst-2.5.4/types_aiobotocore_codecatalyst.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-codecatalyst
-Version: 2.5.2.post3
-Summary: Type annotations for aiobotocore.CodeCatalyst 2.5.2 service generated with mypy-boto3-builder 7.17.2
+Version: 2.5.4
+Summary: Type annotations for aiobotocore.CodeCatalyst 2.5.4 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codecatalyst/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-codecatalyst.svg?color=blue)](https://pypi.org/project/types-aiobotocore-codecatalyst)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codecatalyst/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-codecatalyst)](https://pepy.tech/project/types-aiobotocore-codecatalyst)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.CodeCatalyst 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codecatalyst.html#CodeCatalyst)
+[aiobotocore.CodeCatalyst 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codecatalyst.html#CodeCatalyst)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-codecatalyst-2.5.2.post3/types_aiobotocore_codecatalyst.egg-info/SOURCES.txt` & `types-aiobotocore-codecatalyst-2.5.4/types_aiobotocore_codecatalyst.egg-info/SOURCES.txt`

 * *Files identical despite different names*


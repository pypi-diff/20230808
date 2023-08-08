# Comparing `tmp/types-aiobotocore-codestar-connections-2.5.2.post3.tar.gz` & `tmp/types-aiobotocore-codestar-connections-2.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-codestar-connections-2.5.2.post3.tar", last modified: Fri Aug  4 12:37:29 2023, max compression
+gzip compressed data, was "types-aiobotocore-codestar-connections-2.5.4.tar", last modified: Tue Aug  8 01:23:29 2023, max compression
```

## Comparing `types-aiobotocore-codestar-connections-2.5.2.post3.tar` & `types-aiobotocore-codestar-connections-2.5.4.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:37:29.143462 types-aiobotocore-codestar-connections-2.5.2.post3/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-04 12:20:22.000000 types-aiobotocore-codestar-connections-2.5.2.post3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    12864 2023-08-04 12:37:29.143462 types-aiobotocore-codestar-connections-2.5.2.post3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    11295 2023-08-04 12:20:22.000000 types-aiobotocore-codestar-connections-2.5.2.post3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-04 12:37:29.143462 types-aiobotocore-codestar-connections-2.5.2.post3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2154 2023-08-04 12:20:22.000000 types-aiobotocore-codestar-connections-2.5.2.post3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:37:29.135462 types-aiobotocore-codestar-connections-2.5.2.post3/types_aiobotocore_codestar_connections/
--rw-r--r--   0 runner    (1001) docker     (123)      541 2023-08-04 12:20:22.000000 types-aiobotocore-codestar-connections-2.5.2.post3/types_aiobotocore_codestar_connections/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      540 2023-08-04 12:20:22.000000 types-aiobotocore-codestar-connections-2.5.2.post3/types_aiobotocore_codestar_connections/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      993 2023-08-04 12:20:22.000000 types-aiobotocore-codestar-connections-2.5.2.post3/types_aiobotocore_codestar_connections/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11748 2023-08-04 12:20:23.000000 types-aiobotocore-codestar-connections-2.5.2.post3/types_aiobotocore_codestar_connections/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    11728 2023-08-04 12:20:23.000000 types-aiobotocore-codestar-connections-2.5.2.post3/types_aiobotocore_codestar_connections/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8154 2023-08-04 12:20:23.000000 types-aiobotocore-codestar-connections-2.5.2.post3/types_aiobotocore_codestar_connections/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     8152 2023-08-04 12:20:23.000000 types-aiobotocore-codestar-connections-2.5.2.post3/types_aiobotocore_codestar_connections/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 12:20:22.000000 types-aiobotocore-codestar-connections-2.5.2.post3/types_aiobotocore_codestar_connections/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     7326 2023-08-04 12:20:23.000000 types-aiobotocore-codestar-connections-2.5.2.post3/types_aiobotocore_codestar_connections/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)     7317 2023-08-04 12:20:23.000000 types-aiobotocore-codestar-connections-2.5.2.post3/types_aiobotocore_codestar_connections/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-04 12:20:22.000000 types-aiobotocore-codestar-connections-2.5.2.post3/types_aiobotocore_codestar_connections/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:37:29.143462 types-aiobotocore-codestar-connections-2.5.2.post3/types_aiobotocore_codestar_connections.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    12864 2023-08-04 12:37:28.000000 types-aiobotocore-codestar-connections-2.5.2.post3/types_aiobotocore_codestar_connections.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      955 2023-08-04 12:37:28.000000 types-aiobotocore-codestar-connections-2.5.2.post3/types_aiobotocore_codestar_connections.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 12:37:28.000000 types-aiobotocore-codestar-connections-2.5.2.post3/types_aiobotocore_codestar_connections.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 12:37:28.000000 types-aiobotocore-codestar-connections-2.5.2.post3/types_aiobotocore_codestar_connections.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-04 12:37:28.000000 types-aiobotocore-codestar-connections-2.5.2.post3/types_aiobotocore_codestar_connections.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-08-04 12:37:28.000000 types-aiobotocore-codestar-connections-2.5.2.post3/types_aiobotocore_codestar_connections.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:23:29.510651 types-aiobotocore-codestar-connections-2.5.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-08 01:08:02.000000 types-aiobotocore-codestar-connections-2.5.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    12858 2023-08-08 01:23:29.510651 types-aiobotocore-codestar-connections-2.5.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    11295 2023-08-08 01:08:02.000000 types-aiobotocore-codestar-connections-2.5.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-08 01:23:29.510651 types-aiobotocore-codestar-connections-2.5.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2148 2023-08-08 01:08:01.000000 types-aiobotocore-codestar-connections-2.5.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:23:29.510651 types-aiobotocore-codestar-connections-2.5.4/types_aiobotocore_codestar_connections/
+-rw-r--r--   0 runner    (1001) docker     (123)      541 2023-08-08 01:08:02.000000 types-aiobotocore-codestar-connections-2.5.4/types_aiobotocore_codestar_connections/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      540 2023-08-08 01:08:02.000000 types-aiobotocore-codestar-connections-2.5.4/types_aiobotocore_codestar_connections/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      981 2023-08-08 01:08:02.000000 types-aiobotocore-codestar-connections-2.5.4/types_aiobotocore_codestar_connections/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11780 2023-08-08 01:08:02.000000 types-aiobotocore-codestar-connections-2.5.4/types_aiobotocore_codestar_connections/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11760 2023-08-08 01:08:02.000000 types-aiobotocore-codestar-connections-2.5.4/types_aiobotocore_codestar_connections/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8259 2023-08-08 01:08:02.000000 types-aiobotocore-codestar-connections-2.5.4/types_aiobotocore_codestar_connections/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8257 2023-08-08 01:08:02.000000 types-aiobotocore-codestar-connections-2.5.4/types_aiobotocore_codestar_connections/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 01:08:02.000000 types-aiobotocore-codestar-connections-2.5.4/types_aiobotocore_codestar_connections/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     7326 2023-08-08 01:08:02.000000 types-aiobotocore-codestar-connections-2.5.4/types_aiobotocore_codestar_connections/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7317 2023-08-08 01:08:02.000000 types-aiobotocore-codestar-connections-2.5.4/types_aiobotocore_codestar_connections/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-08-08 01:08:02.000000 types-aiobotocore-codestar-connections-2.5.4/types_aiobotocore_codestar_connections/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:23:29.510651 types-aiobotocore-codestar-connections-2.5.4/types_aiobotocore_codestar_connections.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    12858 2023-08-08 01:23:29.000000 types-aiobotocore-codestar-connections-2.5.4/types_aiobotocore_codestar_connections.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      955 2023-08-08 01:23:29.000000 types-aiobotocore-codestar-connections-2.5.4/types_aiobotocore_codestar_connections.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 01:23:29.000000 types-aiobotocore-codestar-connections-2.5.4/types_aiobotocore_codestar_connections.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 01:23:29.000000 types-aiobotocore-codestar-connections-2.5.4/types_aiobotocore_codestar_connections.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-08 01:23:29.000000 types-aiobotocore-codestar-connections-2.5.4/types_aiobotocore_codestar_connections.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-08-08 01:23:29.000000 types-aiobotocore-codestar-connections-2.5.4/types_aiobotocore_codestar_connections.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-codestar-connections-2.5.2.post3/LICENSE` & `types-aiobotocore-codestar-connections-2.5.4/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-codestar-connections-2.5.2.post3/PKG-INFO` & `types-aiobotocore-codestar-connections-2.5.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-codestar-connections
-Version: 2.5.2.post3
-Summary: Type annotations for aiobotocore.CodeStarconnections 2.5.2 service generated with mypy-boto3-builder 7.17.2
+Version: 2.5.4
+Summary: Type annotations for aiobotocore.CodeStarconnections 2.5.4 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codestar_connections/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-codestar-connections.svg?color=blue)](https://pypi.org/project/types-aiobotocore-codestar-connections)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codestar_connections/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-codestar-connections)](https://pepy.tech/project/types-aiobotocore-codestar-connections)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.CodeStarconnections 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codestar-connections.html#CodeStarconnections)
+[aiobotocore.CodeStarconnections 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codestar-connections.html#CodeStarconnections)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-codestar-connections-2.5.2.post3/README.md` & `types-aiobotocore-codestar-connections-2.5.4/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-codestar-connections.svg?color=blue)](https://pypi.org/project/types-aiobotocore-codestar-connections)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codestar_connections/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-codestar-connections)](https://pepy.tech/project/types-aiobotocore-codestar-connections)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.CodeStarconnections 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codestar-connections.html#CodeStarconnections)
+[aiobotocore.CodeStarconnections 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codestar-connections.html#CodeStarconnections)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-codestar-connections-2.5.2.post3/setup.py` & `types-aiobotocore-codestar-connections-2.5.4/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-codestar-connections",
-    version="2.5.2.post3",
+    version="2.5.4",
     packages=["types_aiobotocore_codestar_connections"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.CodeStarconnections 2.5.2 service generated with"
+        "Type annotations for aiobotocore.CodeStarconnections 2.5.4 service generated with"
         " mypy-boto3-builder 7.17.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
```

### Comparing `types-aiobotocore-codestar-connections-2.5.2.post3/types_aiobotocore_codestar_connections/__init__.py` & `types-aiobotocore-codestar-connections-2.5.4/types_aiobotocore_codestar_connections/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-codestar-connections-2.5.2.post3/types_aiobotocore_codestar_connections/__init__.pyi` & `types-aiobotocore-codestar-connections-2.5.4/types_aiobotocore_codestar_connections/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-codestar-connections-2.5.2.post3/types_aiobotocore_codestar_connections/__main__.py` & `types-aiobotocore-codestar-connections-2.5.4/types_aiobotocore_codestar_connections/__main__.py`

 * *Files 10% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.CodeStarconnections 2.5.2\nVersion:        "
-        " 2.5.2.post3\nBuilder version: 7.17.2\nDocs:           "
+        "Type annotations for aiobotocore.CodeStarconnections 2.5.4\nVersion:        "
+        " 2.5.4\nBuilder version: 7.17.2\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codestar_connections//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codestar-connections.html#CodeStarconnections\nOther"
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

### Comparing `types-aiobotocore-codestar-connections-2.5.2.post3/types_aiobotocore_codestar_connections/client.py` & `types-aiobotocore-codestar-connections-2.5.4/types_aiobotocore_codestar_connections/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -90,16 +90,16 @@
         *,
         ConnectionName: str,
         ProviderType: ProviderTypeType = ...,
         Tags: Sequence[TagTypeDef] = ...,
         HostArn: str = ...
     ) -> CreateConnectionOutputTypeDef:
         """
-        Creates a connection that can then be given to other AWS services like
-        CodePipeline so that it can access third-party code repositories.
+        Creates a connection that can then be given to other Amazon Web Services
+        services like CodePipeline so that it can access third-party code repositories.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codestar-connections.html#CodeStarconnections.Client.create_connection)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codestar_connections/client/#create_connection)
         """
 
     async def create_host(
         self,
@@ -204,15 +204,15 @@
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codestar-connections.html#CodeStarconnections.Client.tag_resource)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codestar_connections/client/#tag_resource)
         """
 
     async def untag_resource(self, *, ResourceArn: str, TagKeys: Sequence[str]) -> Dict[str, Any]:
         """
-        Removes tags from an AWS resource.
+        Removes tags from an Amazon Web Services resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codestar-connections.html#CodeStarconnections.Client.untag_resource)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codestar_connections/client/#untag_resource)
         """
 
     async def update_host(
         self,
```

### Comparing `types-aiobotocore-codestar-connections-2.5.2.post3/types_aiobotocore_codestar_connections/client.pyi` & `types-aiobotocore-codestar-connections-2.5.4/types_aiobotocore_codestar_connections/client.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -84,16 +84,16 @@
         *,
         ConnectionName: str,
         ProviderType: ProviderTypeType = ...,
         Tags: Sequence[TagTypeDef] = ...,
         HostArn: str = ...
     ) -> CreateConnectionOutputTypeDef:
         """
-        Creates a connection that can then be given to other AWS services like
-        CodePipeline so that it can access third-party code repositories.
+        Creates a connection that can then be given to other Amazon Web Services
+        services like CodePipeline so that it can access third-party code repositories.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codestar-connections.html#CodeStarconnections.Client.create_connection)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codestar_connections/client/#create_connection)
         """
     async def create_host(
         self,
         *,
@@ -187,15 +187,15 @@
         Adds to or modifies the tags of the given resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codestar-connections.html#CodeStarconnections.Client.tag_resource)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codestar_connections/client/#tag_resource)
         """
     async def untag_resource(self, *, ResourceArn: str, TagKeys: Sequence[str]) -> Dict[str, Any]:
         """
-        Removes tags from an AWS resource.
+        Removes tags from an Amazon Web Services resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codestar-connections.html#CodeStarconnections.Client.untag_resource)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codestar_connections/client/#untag_resource)
         """
     async def update_host(
         self,
         *,
```

### Comparing `types-aiobotocore-codestar-connections-2.5.2.post3/types_aiobotocore_codestar_connections/literals.py` & `types-aiobotocore-codestar-connections-2.5.4/types_aiobotocore_codestar_connections/literals.py`

 * *Files 1% similar despite different names*

```diff
@@ -26,15 +26,15 @@
     "ServiceName",
     "ResourceServiceName",
     "RegionName",
 )
 
 
 ConnectionStatusType = Literal["AVAILABLE", "ERROR", "PENDING"]
-ProviderTypeType = Literal["Bitbucket", "GitHub", "GitHubEnterpriseServer"]
+ProviderTypeType = Literal["Bitbucket", "GitHub", "GitHubEnterpriseServer", "GitLab"]
 CodeStarconnectionsServiceName = Literal["codestar-connections"]
 ServiceName = Literal[
     "accessanalyzer",
     "account",
     "acm",
     "acm-pca",
     "alexaforbusiness",
@@ -43,14 +43,15 @@
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
@@ -146,14 +147,15 @@
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
@@ -232,26 +234,28 @@
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

### Comparing `types-aiobotocore-codestar-connections-2.5.2.post3/types_aiobotocore_codestar_connections/literals.pyi` & `types-aiobotocore-codestar-connections-2.5.4/types_aiobotocore_codestar_connections/literals.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -24,15 +24,15 @@
     "CodeStarconnectionsServiceName",
     "ServiceName",
     "ResourceServiceName",
     "RegionName",
 )
 
 ConnectionStatusType = Literal["AVAILABLE", "ERROR", "PENDING"]
-ProviderTypeType = Literal["Bitbucket", "GitHub", "GitHubEnterpriseServer"]
+ProviderTypeType = Literal["Bitbucket", "GitHub", "GitHubEnterpriseServer", "GitLab"]
 CodeStarconnectionsServiceName = Literal["codestar-connections"]
 ServiceName = Literal[
     "accessanalyzer",
     "account",
     "acm",
     "acm-pca",
     "alexaforbusiness",
@@ -41,14 +41,15 @@
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
@@ -144,14 +145,15 @@
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
@@ -230,26 +232,28 @@
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

### Comparing `types-aiobotocore-codestar-connections-2.5.2.post3/types_aiobotocore_codestar_connections/type_defs.py` & `types-aiobotocore-codestar-connections-2.5.4/types_aiobotocore_codestar_connections/type_defs.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-codestar-connections-2.5.2.post3/types_aiobotocore_codestar_connections/type_defs.pyi` & `types-aiobotocore-codestar-connections-2.5.4/types_aiobotocore_codestar_connections/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-codestar-connections-2.5.2.post3/types_aiobotocore_codestar_connections.egg-info/PKG-INFO` & `types-aiobotocore-codestar-connections-2.5.4/types_aiobotocore_codestar_connections.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-codestar-connections
-Version: 2.5.2.post3
-Summary: Type annotations for aiobotocore.CodeStarconnections 2.5.2 service generated with mypy-boto3-builder 7.17.2
+Version: 2.5.4
+Summary: Type annotations for aiobotocore.CodeStarconnections 2.5.4 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codestar_connections/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-codestar-connections.svg?color=blue)](https://pypi.org/project/types-aiobotocore-codestar-connections)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codestar_connections/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-codestar-connections)](https://pepy.tech/project/types-aiobotocore-codestar-connections)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.CodeStarconnections 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codestar-connections.html#CodeStarconnections)
+[aiobotocore.CodeStarconnections 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codestar-connections.html#CodeStarconnections)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-codestar-connections-2.5.2.post3/types_aiobotocore_codestar_connections.egg-info/SOURCES.txt` & `types-aiobotocore-codestar-connections-2.5.4/types_aiobotocore_codestar_connections.egg-info/SOURCES.txt`

 * *Files identical despite different names*


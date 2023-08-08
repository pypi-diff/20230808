# Comparing `tmp/types-aiobotocore-connect-2.5.2.post3.tar.gz` & `tmp/types-aiobotocore-connect-2.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-connect-2.5.2.post3.tar", last modified: Fri Aug  4 12:37:31 2023, max compression
+gzip compressed data, was "types-aiobotocore-connect-2.5.4.tar", last modified: Tue Aug  8 01:23:32 2023, max compression
```

## Comparing `types-aiobotocore-connect-2.5.2.post3.tar` & `types-aiobotocore-connect-2.5.4.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:37:31.735527 types-aiobotocore-connect-2.5.2.post3/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-04 12:20:48.000000 types-aiobotocore-connect-2.5.2.post3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    19814 2023-08-04 12:37:31.731527 types-aiobotocore-connect-2.5.2.post3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    18296 2023-08-04 12:20:48.000000 types-aiobotocore-connect-2.5.2.post3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-04 12:37:31.735527 types-aiobotocore-connect-2.5.2.post3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2072 2023-08-04 12:20:48.000000 types-aiobotocore-connect-2.5.2.post3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:37:31.727527 types-aiobotocore-connect-2.5.2.post3/types_aiobotocore_connect/
--rw-r--r--   0 runner    (1001) docker     (123)    10331 2023-08-04 12:20:48.000000 types-aiobotocore-connect-2.5.2.post3/types_aiobotocore_connect/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10330 2023-08-04 12:20:48.000000 types-aiobotocore-connect-2.5.2.post3/types_aiobotocore_connect/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      943 2023-08-04 12:20:48.000000 types-aiobotocore-connect-2.5.2.post3/types_aiobotocore_connect/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)   156901 2023-08-04 12:20:50.000000 types-aiobotocore-connect-2.5.2.post3/types_aiobotocore_connect/client.py
--rw-r--r--   0 runner    (1001) docker     (123)   156653 2023-08-04 12:20:50.000000 types-aiobotocore-connect-2.5.2.post3/types_aiobotocore_connect/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    25347 2023-08-04 12:20:51.000000 types-aiobotocore-connect-2.5.2.post3/types_aiobotocore_connect/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    25345 2023-08-04 12:20:51.000000 types-aiobotocore-connect-2.5.2.post3/types_aiobotocore_connect/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    56326 2023-08-04 12:20:51.000000 types-aiobotocore-connect-2.5.2.post3/types_aiobotocore_connect/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)    56279 2023-08-04 12:20:51.000000 types-aiobotocore-connect-2.5.2.post3/types_aiobotocore_connect/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 12:20:48.000000 types-aiobotocore-connect-2.5.2.post3/types_aiobotocore_connect/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)   217314 2023-08-04 12:20:58.000000 types-aiobotocore-connect-2.5.2.post3/types_aiobotocore_connect/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)   216983 2023-08-04 12:20:54.000000 types-aiobotocore-connect-2.5.2.post3/types_aiobotocore_connect/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-04 12:20:48.000000 types-aiobotocore-connect-2.5.2.post3/types_aiobotocore_connect/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:37:31.731527 types-aiobotocore-connect-2.5.2.post3/types_aiobotocore_connect.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    19814 2023-08-04 12:37:31.000000 types-aiobotocore-connect-2.5.2.post3/types_aiobotocore_connect.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      813 2023-08-04 12:37:31.000000 types-aiobotocore-connect-2.5.2.post3/types_aiobotocore_connect.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 12:37:31.000000 types-aiobotocore-connect-2.5.2.post3/types_aiobotocore_connect.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 12:37:31.000000 types-aiobotocore-connect-2.5.2.post3/types_aiobotocore_connect.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-04 12:37:31.000000 types-aiobotocore-connect-2.5.2.post3/types_aiobotocore_connect.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-08-04 12:37:31.000000 types-aiobotocore-connect-2.5.2.post3/types_aiobotocore_connect.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:23:32.562674 types-aiobotocore-connect-2.5.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-08 01:08:26.000000 types-aiobotocore-connect-2.5.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    19808 2023-08-08 01:23:32.562674 types-aiobotocore-connect-2.5.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    18296 2023-08-08 01:08:26.000000 types-aiobotocore-connect-2.5.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-08 01:23:32.562674 types-aiobotocore-connect-2.5.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2066 2023-08-08 01:08:26.000000 types-aiobotocore-connect-2.5.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:23:32.562674 types-aiobotocore-connect-2.5.4/types_aiobotocore_connect/
+-rw-r--r--   0 runner    (1001) docker     (123)    10331 2023-08-08 01:08:26.000000 types-aiobotocore-connect-2.5.4/types_aiobotocore_connect/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10330 2023-08-08 01:08:26.000000 types-aiobotocore-connect-2.5.4/types_aiobotocore_connect/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      931 2023-08-08 01:08:26.000000 types-aiobotocore-connect-2.5.4/types_aiobotocore_connect/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   157883 2023-08-08 01:08:28.000000 types-aiobotocore-connect-2.5.4/types_aiobotocore_connect/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)   157633 2023-08-08 01:08:27.000000 types-aiobotocore-connect-2.5.4/types_aiobotocore_connect/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    25503 2023-08-08 01:08:29.000000 types-aiobotocore-connect-2.5.4/types_aiobotocore_connect/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25501 2023-08-08 01:08:29.000000 types-aiobotocore-connect-2.5.4/types_aiobotocore_connect/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    56326 2023-08-08 01:08:29.000000 types-aiobotocore-connect-2.5.4/types_aiobotocore_connect/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    56279 2023-08-08 01:08:28.000000 types-aiobotocore-connect-2.5.4/types_aiobotocore_connect/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 01:08:26.000000 types-aiobotocore-connect-2.5.4/types_aiobotocore_connect/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)   217736 2023-08-08 01:08:34.000000 types-aiobotocore-connect-2.5.4/types_aiobotocore_connect/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)   217405 2023-08-08 01:08:32.000000 types-aiobotocore-connect-2.5.4/types_aiobotocore_connect/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-08-08 01:08:26.000000 types-aiobotocore-connect-2.5.4/types_aiobotocore_connect/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:23:32.562674 types-aiobotocore-connect-2.5.4/types_aiobotocore_connect.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    19808 2023-08-08 01:23:32.000000 types-aiobotocore-connect-2.5.4/types_aiobotocore_connect.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      813 2023-08-08 01:23:32.000000 types-aiobotocore-connect-2.5.4/types_aiobotocore_connect.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 01:23:32.000000 types-aiobotocore-connect-2.5.4/types_aiobotocore_connect.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 01:23:32.000000 types-aiobotocore-connect-2.5.4/types_aiobotocore_connect.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-08 01:23:32.000000 types-aiobotocore-connect-2.5.4/types_aiobotocore_connect.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-08-08 01:23:32.000000 types-aiobotocore-connect-2.5.4/types_aiobotocore_connect.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-connect-2.5.2.post3/LICENSE` & `types-aiobotocore-connect-2.5.4/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-connect-2.5.2.post3/PKG-INFO` & `types-aiobotocore-connect-2.5.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-connect
-Version: 2.5.2.post3
-Summary: Type annotations for aiobotocore.Connect 2.5.2 service generated with mypy-boto3-builder 7.17.2
+Version: 2.5.4
+Summary: Type annotations for aiobotocore.Connect 2.5.4 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_connect/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-connect.svg?color=blue)](https://pypi.org/project/types-aiobotocore-connect)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_connect/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-connect)](https://pepy.tech/project/types-aiobotocore-connect)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.Connect 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect)
+[aiobotocore.Connect 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-connect-2.5.2.post3/README.md` & `types-aiobotocore-connect-2.5.4/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-connect.svg?color=blue)](https://pypi.org/project/types-aiobotocore-connect)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_connect/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-connect)](https://pepy.tech/project/types-aiobotocore-connect)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.Connect 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect)
+[aiobotocore.Connect 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-connect-2.5.2.post3/setup.py` & `types-aiobotocore-connect-2.5.4/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-connect",
-    version="2.5.2.post3",
+    version="2.5.4",
     packages=["types_aiobotocore_connect"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.Connect 2.5.2 service generated with mypy-boto3-builder"
+        "Type annotations for aiobotocore.Connect 2.5.4 service generated with mypy-boto3-builder"
         " 7.17.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
```

### Comparing `types-aiobotocore-connect-2.5.2.post3/types_aiobotocore_connect/__init__.py` & `types-aiobotocore-connect-2.5.4/types_aiobotocore_connect/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-connect-2.5.2.post3/types_aiobotocore_connect/__init__.pyi` & `types-aiobotocore-connect-2.5.4/types_aiobotocore_connect/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-connect-2.5.2.post3/types_aiobotocore_connect/__main__.py` & `types-aiobotocore-connect-2.5.4/types_aiobotocore_connect/__main__.py`

 * *Files 20% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.Connect 2.5.2\nVersion:         2.5.2.post3\nBuilder"
-        " version: 7.17.2\nDocs:           "
+        "Type annotations for aiobotocore.Connect 2.5.4\nVersion:         2.5.4\nBuilder version:"
+        " 7.17.2\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_connect//\nBoto3 docs:"
         "     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect\nOther"
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

### Comparing `types-aiobotocore-connect-2.5.2.post3/types_aiobotocore_connect/client.py` & `types-aiobotocore-connect-2.5.4/types_aiobotocore_connect/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -904,24 +904,42 @@
         """
         Deletes a prompt.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.delete_prompt)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_connect/client/#delete_prompt)
         """
 
+    async def delete_queue(self, *, InstanceId: str, QueueId: str) -> EmptyResponseMetadataTypeDef:
+        """
+        Deletes a queue.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.delete_queue)
+        [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_connect/client/#delete_queue)
+        """
+
     async def delete_quick_connect(
         self, *, InstanceId: str, QuickConnectId: str
     ) -> EmptyResponseMetadataTypeDef:
         """
         Deletes a quick connect.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.delete_quick_connect)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_connect/client/#delete_quick_connect)
         """
 
+    async def delete_routing_profile(
+        self, *, InstanceId: str, RoutingProfileId: str
+    ) -> EmptyResponseMetadataTypeDef:
+        """
+        Deletes a routing profile.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.delete_routing_profile)
+        [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_connect/client/#delete_routing_profile)
+        """
+
     async def delete_rule(self, *, InstanceId: str, RuleId: str) -> EmptyResponseMetadataTypeDef:
         """
         Deletes a rule for the specified Amazon Connect instance.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.delete_rule)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_connect/client/#delete_rule)
         """
@@ -2008,15 +2026,15 @@
         InstanceId: str,
         NextToken: str = ...,
         MaxResults: int = ...,
         SearchFilter: QueueSearchFilterTypeDef = ...,
         SearchCriteria: "QueueSearchCriteriaTypeDef" = ...
     ) -> SearchQueuesResponseTypeDef:
         """
-        This API is in preview release for Amazon Connect and is subject to change.
+        Searches queues in an Amazon Connect instance, with optional filtering.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.search_queues)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_connect/client/#search_queues)
         """
 
     async def search_quick_connects(
         self,
@@ -2056,15 +2074,16 @@
         InstanceId: str,
         NextToken: str = ...,
         MaxResults: int = ...,
         SearchFilter: RoutingProfileSearchFilterTypeDef = ...,
         SearchCriteria: "RoutingProfileSearchCriteriaTypeDef" = ...
     ) -> SearchRoutingProfilesResponseTypeDef:
         """
-        This API is in preview release for Amazon Connect and is subject to change.
+        Searches routing profiles in an Amazon Connect instance, with optional
+        filtering.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.search_routing_profiles)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_connect/client/#search_routing_profiles)
         """
 
     async def search_security_profiles(
         self,
@@ -2072,15 +2091,16 @@
         InstanceId: str,
         NextToken: str = ...,
         MaxResults: int = ...,
         SearchCriteria: "SecurityProfileSearchCriteriaTypeDef" = ...,
         SearchFilter: SecurityProfilesSearchFilterTypeDef = ...
     ) -> SearchSecurityProfilesResponseTypeDef:
         """
-        This API is in preview release for Amazon Connect and is subject to change.
+        Searches security profiles in an Amazon Connect instance, with optional
+        filtering.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.search_security_profiles)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_connect/client/#search_security_profiles)
         """
 
     async def search_users(
         self,
```

### Comparing `types-aiobotocore-connect-2.5.2.post3/types_aiobotocore_connect/client.pyi` & `types-aiobotocore-connect-2.5.4/types_aiobotocore_connect/client.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -856,23 +856,39 @@
     ) -> EmptyResponseMetadataTypeDef:
         """
         Deletes a prompt.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.delete_prompt)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_connect/client/#delete_prompt)
         """
+    async def delete_queue(self, *, InstanceId: str, QueueId: str) -> EmptyResponseMetadataTypeDef:
+        """
+        Deletes a queue.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.delete_queue)
+        [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_connect/client/#delete_queue)
+        """
     async def delete_quick_connect(
         self, *, InstanceId: str, QuickConnectId: str
     ) -> EmptyResponseMetadataTypeDef:
         """
         Deletes a quick connect.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.delete_quick_connect)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_connect/client/#delete_quick_connect)
         """
+    async def delete_routing_profile(
+        self, *, InstanceId: str, RoutingProfileId: str
+    ) -> EmptyResponseMetadataTypeDef:
+        """
+        Deletes a routing profile.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.delete_routing_profile)
+        [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_connect/client/#delete_routing_profile)
+        """
     async def delete_rule(self, *, InstanceId: str, RuleId: str) -> EmptyResponseMetadataTypeDef:
         """
         Deletes a rule for the specified Amazon Connect instance.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.delete_rule)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_connect/client/#delete_rule)
         """
@@ -1866,15 +1882,15 @@
         InstanceId: str,
         NextToken: str = ...,
         MaxResults: int = ...,
         SearchFilter: QueueSearchFilterTypeDef = ...,
         SearchCriteria: "QueueSearchCriteriaTypeDef" = ...
     ) -> SearchQueuesResponseTypeDef:
         """
-        This API is in preview release for Amazon Connect and is subject to change.
+        Searches queues in an Amazon Connect instance, with optional filtering.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.search_queues)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_connect/client/#search_queues)
         """
     async def search_quick_connects(
         self,
         *,
@@ -1911,30 +1927,32 @@
         InstanceId: str,
         NextToken: str = ...,
         MaxResults: int = ...,
         SearchFilter: RoutingProfileSearchFilterTypeDef = ...,
         SearchCriteria: "RoutingProfileSearchCriteriaTypeDef" = ...
     ) -> SearchRoutingProfilesResponseTypeDef:
         """
-        This API is in preview release for Amazon Connect and is subject to change.
+        Searches routing profiles in an Amazon Connect instance, with optional
+        filtering.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.search_routing_profiles)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_connect/client/#search_routing_profiles)
         """
     async def search_security_profiles(
         self,
         *,
         InstanceId: str,
         NextToken: str = ...,
         MaxResults: int = ...,
         SearchCriteria: "SecurityProfileSearchCriteriaTypeDef" = ...,
         SearchFilter: SecurityProfilesSearchFilterTypeDef = ...
     ) -> SearchSecurityProfilesResponseTypeDef:
         """
-        This API is in preview release for Amazon Connect and is subject to change.
+        Searches security profiles in an Amazon Connect instance, with optional
+        filtering.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.search_security_profiles)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_connect/client/#search_security_profiles)
         """
     async def search_users(
         self,
         *,
```

### Comparing `types-aiobotocore-connect-2.5.2.post3/types_aiobotocore_connect/literals.py` & `types-aiobotocore-connect-2.5.4/types_aiobotocore_connect/literals.py`

 * *Files 1% similar despite different names*

```diff
@@ -562,15 +562,17 @@
     "WS",
     "YE",
     "YT",
     "ZA",
     "ZM",
     "ZW",
 ]
-PhoneNumberTypeType = Literal["DID", "TOLL_FREE"]
+PhoneNumberTypeType = Literal[
+    "DID", "SHARED", "THIRD_PARTY_DID", "THIRD_PARTY_TF", "TOLL_FREE", "UIFN"
+]
 PhoneNumberWorkflowStatusType = Literal["CLAIMED", "FAILED", "IN_PROGRESS"]
 PhoneTypeType = Literal["DESK_PHONE", "SOFT_PHONE"]
 QueueStatusType = Literal["DISABLED", "ENABLED"]
 QueueTypeType = Literal["AGENT", "STANDARD"]
 QuickConnectTypeType = Literal["PHONE_NUMBER", "QUEUE", "USER"]
 ReferenceStatusType = Literal["APPROVED", "REJECTED"]
 ReferenceTypeType = Literal["ATTACHMENT", "DATE", "EMAIL", "NUMBER", "STRING", "URL"]
@@ -661,14 +663,15 @@
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
@@ -764,14 +767,15 @@
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
@@ -850,26 +854,28 @@
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

### Comparing `types-aiobotocore-connect-2.5.2.post3/types_aiobotocore_connect/literals.pyi` & `types-aiobotocore-connect-2.5.4/types_aiobotocore_connect/literals.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -560,15 +560,17 @@
     "WS",
     "YE",
     "YT",
     "ZA",
     "ZM",
     "ZW",
 ]
-PhoneNumberTypeType = Literal["DID", "TOLL_FREE"]
+PhoneNumberTypeType = Literal[
+    "DID", "SHARED", "THIRD_PARTY_DID", "THIRD_PARTY_TF", "TOLL_FREE", "UIFN"
+]
 PhoneNumberWorkflowStatusType = Literal["CLAIMED", "FAILED", "IN_PROGRESS"]
 PhoneTypeType = Literal["DESK_PHONE", "SOFT_PHONE"]
 QueueStatusType = Literal["DISABLED", "ENABLED"]
 QueueTypeType = Literal["AGENT", "STANDARD"]
 QuickConnectTypeType = Literal["PHONE_NUMBER", "QUEUE", "USER"]
 ReferenceStatusType = Literal["APPROVED", "REJECTED"]
 ReferenceTypeType = Literal["ATTACHMENT", "DATE", "EMAIL", "NUMBER", "STRING", "URL"]
@@ -659,14 +661,15 @@
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
@@ -762,14 +765,15 @@
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
@@ -848,26 +852,28 @@
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

### Comparing `types-aiobotocore-connect-2.5.2.post3/types_aiobotocore_connect/paginator.py` & `types-aiobotocore-connect-2.5.4/types_aiobotocore_connect/paginator.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-connect-2.5.2.post3/types_aiobotocore_connect/paginator.pyi` & `types-aiobotocore-connect-2.5.4/types_aiobotocore_connect/paginator.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-connect-2.5.2.post3/types_aiobotocore_connect/type_defs.py` & `types-aiobotocore-connect-2.5.4/types_aiobotocore_connect/type_defs.py`

 * *Files 0% similar despite different names*

```diff
@@ -150,15 +150,17 @@
     "DeleteContactFlowModuleRequestRequestTypeDef",
     "DeleteContactFlowRequestRequestTypeDef",
     "DeleteEvaluationFormRequestRequestTypeDef",
     "DeleteHoursOfOperationRequestRequestTypeDef",
     "DeleteInstanceRequestRequestTypeDef",
     "DeleteIntegrationAssociationRequestRequestTypeDef",
     "DeletePromptRequestRequestTypeDef",
+    "DeleteQueueRequestRequestTypeDef",
     "DeleteQuickConnectRequestRequestTypeDef",
+    "DeleteRoutingProfileRequestRequestTypeDef",
     "DeleteRuleRequestRequestTypeDef",
     "DeleteSecurityProfileRequestRequestTypeDef",
     "DeleteTaskTemplateRequestRequestTypeDef",
     "DeleteTrafficDistributionGroupRequestRequestTypeDef",
     "DeleteUseCaseRequestRequestTypeDef",
     "DeleteUserHierarchyGroupRequestRequestTypeDef",
     "DeleteUserRequestRequestTypeDef",
@@ -1477,22 +1479,38 @@
     "DeletePromptRequestRequestTypeDef",
     {
         "InstanceId": str,
         "PromptId": str,
     },
 )
 
+DeleteQueueRequestRequestTypeDef = TypedDict(
+    "DeleteQueueRequestRequestTypeDef",
+    {
+        "InstanceId": str,
+        "QueueId": str,
+    },
+)
+
 DeleteQuickConnectRequestRequestTypeDef = TypedDict(
     "DeleteQuickConnectRequestRequestTypeDef",
     {
         "InstanceId": str,
         "QuickConnectId": str,
     },
 )
 
+DeleteRoutingProfileRequestRequestTypeDef = TypedDict(
+    "DeleteRoutingProfileRequestRequestTypeDef",
+    {
+        "InstanceId": str,
+        "RoutingProfileId": str,
+    },
+)
+
 DeleteRuleRequestRequestTypeDef = TypedDict(
     "DeleteRuleRequestRequestTypeDef",
     {
         "InstanceId": str,
         "RuleId": str,
     },
 )
```

### Comparing `types-aiobotocore-connect-2.5.2.post3/types_aiobotocore_connect/type_defs.pyi` & `types-aiobotocore-connect-2.5.4/types_aiobotocore_connect/type_defs.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -149,15 +149,17 @@
     "DeleteContactFlowModuleRequestRequestTypeDef",
     "DeleteContactFlowRequestRequestTypeDef",
     "DeleteEvaluationFormRequestRequestTypeDef",
     "DeleteHoursOfOperationRequestRequestTypeDef",
     "DeleteInstanceRequestRequestTypeDef",
     "DeleteIntegrationAssociationRequestRequestTypeDef",
     "DeletePromptRequestRequestTypeDef",
+    "DeleteQueueRequestRequestTypeDef",
     "DeleteQuickConnectRequestRequestTypeDef",
+    "DeleteRoutingProfileRequestRequestTypeDef",
     "DeleteRuleRequestRequestTypeDef",
     "DeleteSecurityProfileRequestRequestTypeDef",
     "DeleteTaskTemplateRequestRequestTypeDef",
     "DeleteTrafficDistributionGroupRequestRequestTypeDef",
     "DeleteUseCaseRequestRequestTypeDef",
     "DeleteUserHierarchyGroupRequestRequestTypeDef",
     "DeleteUserRequestRequestTypeDef",
@@ -1444,22 +1446,38 @@
     "DeletePromptRequestRequestTypeDef",
     {
         "InstanceId": str,
         "PromptId": str,
     },
 )
 
+DeleteQueueRequestRequestTypeDef = TypedDict(
+    "DeleteQueueRequestRequestTypeDef",
+    {
+        "InstanceId": str,
+        "QueueId": str,
+    },
+)
+
 DeleteQuickConnectRequestRequestTypeDef = TypedDict(
     "DeleteQuickConnectRequestRequestTypeDef",
     {
         "InstanceId": str,
         "QuickConnectId": str,
     },
 )
 
+DeleteRoutingProfileRequestRequestTypeDef = TypedDict(
+    "DeleteRoutingProfileRequestRequestTypeDef",
+    {
+        "InstanceId": str,
+        "RoutingProfileId": str,
+    },
+)
+
 DeleteRuleRequestRequestTypeDef = TypedDict(
     "DeleteRuleRequestRequestTypeDef",
     {
         "InstanceId": str,
         "RuleId": str,
     },
 )
```

### Comparing `types-aiobotocore-connect-2.5.2.post3/types_aiobotocore_connect.egg-info/PKG-INFO` & `types-aiobotocore-connect-2.5.4/types_aiobotocore_connect.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-connect
-Version: 2.5.2.post3
-Summary: Type annotations for aiobotocore.Connect 2.5.2 service generated with mypy-boto3-builder 7.17.2
+Version: 2.5.4
+Summary: Type annotations for aiobotocore.Connect 2.5.4 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_connect/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-connect.svg?color=blue)](https://pypi.org/project/types-aiobotocore-connect)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_connect/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-connect)](https://pepy.tech/project/types-aiobotocore-connect)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.Connect 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect)
+[aiobotocore.Connect 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-connect-2.5.2.post3/types_aiobotocore_connect.egg-info/SOURCES.txt` & `types-aiobotocore-connect-2.5.4/types_aiobotocore_connect.egg-info/SOURCES.txt`

 * *Files identical despite different names*


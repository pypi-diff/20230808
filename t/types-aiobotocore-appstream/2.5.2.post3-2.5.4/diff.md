# Comparing `tmp/types-aiobotocore-appstream-2.5.2.post3.tar.gz` & `tmp/types-aiobotocore-appstream-2.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-appstream-2.5.2.post3.tar", last modified: Fri Aug  4 12:37:18 2023, max compression
+gzip compressed data, was "types-aiobotocore-appstream-2.5.4.tar", last modified: Tue Aug  8 01:23:19 2023, max compression
```

## Comparing `types-aiobotocore-appstream-2.5.2.post3.tar` & `types-aiobotocore-appstream-2.5.4.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:37:18.887225 types-aiobotocore-appstream-2.5.2.post3/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-04 12:18:33.000000 types-aiobotocore-appstream-2.5.2.post3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    15237 2023-08-04 12:37:18.887225 types-aiobotocore-appstream-2.5.2.post3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    13711 2023-08-04 12:18:33.000000 types-aiobotocore-appstream-2.5.2.post3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-04 12:37:18.887225 types-aiobotocore-appstream-2.5.2.post3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2086 2023-08-04 12:18:33.000000 types-aiobotocore-appstream-2.5.2.post3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:37:18.883225 types-aiobotocore-appstream-2.5.2.post3/types_aiobotocore_appstream/
--rw-r--r--   0 runner    (1001) docker     (123)     3011 2023-08-04 12:18:33.000000 types-aiobotocore-appstream-2.5.2.post3/types_aiobotocore_appstream/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3010 2023-08-04 12:18:33.000000 types-aiobotocore-appstream-2.5.2.post3/types_aiobotocore_appstream/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      951 2023-08-04 12:18:33.000000 types-aiobotocore-appstream-2.5.2.post3/types_aiobotocore_appstream/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    53969 2023-08-04 12:18:34.000000 types-aiobotocore-appstream-2.5.2.post3/types_aiobotocore_appstream/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    53883 2023-08-04 12:18:34.000000 types-aiobotocore-appstream-2.5.2.post3/types_aiobotocore_appstream/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    14248 2023-08-04 12:18:34.000000 types-aiobotocore-appstream-2.5.2.post3/types_aiobotocore_appstream/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    14246 2023-08-04 12:18:34.000000 types-aiobotocore-appstream-2.5.2.post3/types_aiobotocore_appstream/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    12871 2023-08-04 12:18:34.000000 types-aiobotocore-appstream-2.5.2.post3/types_aiobotocore_appstream/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)    12859 2023-08-04 12:18:34.000000 types-aiobotocore-appstream-2.5.2.post3/types_aiobotocore_appstream/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 12:18:33.000000 types-aiobotocore-appstream-2.5.2.post3/types_aiobotocore_appstream/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    60881 2023-08-04 12:18:36.000000 types-aiobotocore-appstream-2.5.2.post3/types_aiobotocore_appstream/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    60794 2023-08-04 12:18:35.000000 types-aiobotocore-appstream-2.5.2.post3/types_aiobotocore_appstream/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-04 12:18:33.000000 types-aiobotocore-appstream-2.5.2.post3/types_aiobotocore_appstream/version.py
--rw-r--r--   0 runner    (1001) docker     (123)     2638 2023-08-04 12:18:34.000000 types-aiobotocore-appstream-2.5.2.post3/types_aiobotocore_appstream/waiter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2636 2023-08-04 12:18:34.000000 types-aiobotocore-appstream-2.5.2.post3/types_aiobotocore_appstream/waiter.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:37:18.887225 types-aiobotocore-appstream-2.5.2.post3/types_aiobotocore_appstream.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    15237 2023-08-04 12:37:18.000000 types-aiobotocore-appstream-2.5.2.post3/types_aiobotocore_appstream.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      928 2023-08-04 12:37:18.000000 types-aiobotocore-appstream-2.5.2.post3/types_aiobotocore_appstream.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 12:37:18.000000 types-aiobotocore-appstream-2.5.2.post3/types_aiobotocore_appstream.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 12:37:18.000000 types-aiobotocore-appstream-2.5.2.post3/types_aiobotocore_appstream.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-04 12:37:18.000000 types-aiobotocore-appstream-2.5.2.post3/types_aiobotocore_appstream.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-08-04 12:37:18.000000 types-aiobotocore-appstream-2.5.2.post3/types_aiobotocore_appstream.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:23:19.410526 types-aiobotocore-appstream-2.5.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-08 01:06:20.000000 types-aiobotocore-appstream-2.5.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    15231 2023-08-08 01:23:19.406525 types-aiobotocore-appstream-2.5.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    13711 2023-08-08 01:06:20.000000 types-aiobotocore-appstream-2.5.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-08 01:23:19.410526 types-aiobotocore-appstream-2.5.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2080 2023-08-08 01:06:20.000000 types-aiobotocore-appstream-2.5.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:23:19.406525 types-aiobotocore-appstream-2.5.4/types_aiobotocore_appstream/
+-rw-r--r--   0 runner    (1001) docker     (123)     3011 2023-08-08 01:06:20.000000 types-aiobotocore-appstream-2.5.4/types_aiobotocore_appstream/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3010 2023-08-08 01:06:20.000000 types-aiobotocore-appstream-2.5.4/types_aiobotocore_appstream/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      939 2023-08-08 01:06:20.000000 types-aiobotocore-appstream-2.5.4/types_aiobotocore_appstream/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    60980 2023-08-08 01:06:21.000000 types-aiobotocore-appstream-2.5.4/types_aiobotocore_appstream/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    60884 2023-08-08 01:06:21.000000 types-aiobotocore-appstream-2.5.4/types_aiobotocore_appstream/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    14986 2023-08-08 01:06:22.000000 types-aiobotocore-appstream-2.5.4/types_aiobotocore_appstream/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14984 2023-08-08 01:06:22.000000 types-aiobotocore-appstream-2.5.4/types_aiobotocore_appstream/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    12871 2023-08-08 01:06:21.000000 types-aiobotocore-appstream-2.5.4/types_aiobotocore_appstream/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12859 2023-08-08 01:06:21.000000 types-aiobotocore-appstream-2.5.4/types_aiobotocore_appstream/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 01:06:20.000000 types-aiobotocore-appstream-2.5.4/types_aiobotocore_appstream/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    69611 2023-08-08 01:06:23.000000 types-aiobotocore-appstream-2.5.4/types_aiobotocore_appstream/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    69514 2023-08-08 01:06:22.000000 types-aiobotocore-appstream-2.5.4/types_aiobotocore_appstream/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-08-08 01:06:20.000000 types-aiobotocore-appstream-2.5.4/types_aiobotocore_appstream/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2638 2023-08-08 01:06:21.000000 types-aiobotocore-appstream-2.5.4/types_aiobotocore_appstream/waiter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2636 2023-08-08 01:06:21.000000 types-aiobotocore-appstream-2.5.4/types_aiobotocore_appstream/waiter.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:23:19.406525 types-aiobotocore-appstream-2.5.4/types_aiobotocore_appstream.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    15231 2023-08-08 01:23:19.000000 types-aiobotocore-appstream-2.5.4/types_aiobotocore_appstream.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      928 2023-08-08 01:23:19.000000 types-aiobotocore-appstream-2.5.4/types_aiobotocore_appstream.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 01:23:19.000000 types-aiobotocore-appstream-2.5.4/types_aiobotocore_appstream.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 01:23:19.000000 types-aiobotocore-appstream-2.5.4/types_aiobotocore_appstream.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-08 01:23:19.000000 types-aiobotocore-appstream-2.5.4/types_aiobotocore_appstream.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-08-08 01:23:19.000000 types-aiobotocore-appstream-2.5.4/types_aiobotocore_appstream.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-appstream-2.5.2.post3/LICENSE` & `types-aiobotocore-appstream-2.5.4/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-appstream-2.5.2.post3/PKG-INFO` & `types-aiobotocore-appstream-2.5.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-appstream
-Version: 2.5.2.post3
-Summary: Type annotations for aiobotocore.AppStream 2.5.2 service generated with mypy-boto3-builder 7.17.2
+Version: 2.5.4
+Summary: Type annotations for aiobotocore.AppStream 2.5.4 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appstream/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-appstream.svg?color=blue)](https://pypi.org/project/types-aiobotocore-appstream)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appstream/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-appstream)](https://pepy.tech/project/types-aiobotocore-appstream)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.AppStream 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appstream.html#AppStream)
+[aiobotocore.AppStream 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appstream.html#AppStream)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-appstream-2.5.2.post3/README.md` & `types-aiobotocore-appstream-2.5.4/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-appstream.svg?color=blue)](https://pypi.org/project/types-aiobotocore-appstream)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appstream/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-appstream)](https://pepy.tech/project/types-aiobotocore-appstream)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.AppStream 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appstream.html#AppStream)
+[aiobotocore.AppStream 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appstream.html#AppStream)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-appstream-2.5.2.post3/setup.py` & `types-aiobotocore-appstream-2.5.4/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-appstream",
-    version="2.5.2.post3",
+    version="2.5.4",
     packages=["types_aiobotocore_appstream"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.AppStream 2.5.2 service generated with mypy-boto3-builder"
+        "Type annotations for aiobotocore.AppStream 2.5.4 service generated with mypy-boto3-builder"
         " 7.17.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
```

### Comparing `types-aiobotocore-appstream-2.5.2.post3/types_aiobotocore_appstream/__init__.py` & `types-aiobotocore-appstream-2.5.4/types_aiobotocore_appstream/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-appstream-2.5.2.post3/types_aiobotocore_appstream/__init__.pyi` & `types-aiobotocore-appstream-2.5.4/types_aiobotocore_appstream/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-appstream-2.5.2.post3/types_aiobotocore_appstream/__main__.py` & `types-aiobotocore-appstream-2.5.4/types_aiobotocore_appstream/__main__.py`

 * *Files 27% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.AppStream 2.5.2\nVersion:         2.5.2.post3\nBuilder"
-        " version: 7.17.2\nDocs:           "
+        "Type annotations for aiobotocore.AppStream 2.5.4\nVersion:         2.5.4\nBuilder version:"
+        " 7.17.2\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appstream//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appstream.html#AppStream\nOther"
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

### Comparing `types-aiobotocore-appstream-2.5.2.post3/types_aiobotocore_appstream/client.py` & `types-aiobotocore-appstream-2.5.4/types_aiobotocore_appstream/client.py`

 * *Files 8% similar despite different names*

```diff
@@ -17,20 +17,22 @@
 import sys
 from typing import Any, Dict, Mapping, Sequence, Type, overload
 
 from aiobotocore.client import AioBaseClient
 from botocore.client import ClientMeta
 
 from .literals import (
+    AppBlockBuilderAttributeType,
     ApplicationAttributeType,
     AppVisibilityType,
     AuthenticationTypeType,
     FleetAttributeType,
     FleetTypeType,
     MessageActionType,
+    PackagingTypeType,
     PlatformTypeType,
     StackAttributeType,
     StreamViewType,
     VisibilityTypeType,
 )
 from .paginator import (
     DescribeDirectoryConfigsPaginator,
@@ -43,33 +45,38 @@
     DescribeUserStackAssociationsPaginator,
     ListAssociatedFleetsPaginator,
     ListAssociatedStacksPaginator,
 )
 from .type_defs import (
     AccessEndpointTypeDef,
     ApplicationSettingsTypeDef,
+    AssociateAppBlockBuilderAppBlockResultTypeDef,
     AssociateApplicationFleetResultTypeDef,
     BatchAssociateUserStackResultTypeDef,
     BatchDisassociateUserStackResultTypeDef,
     CertificateBasedAuthPropertiesTypeDef,
     ComputeCapacityTypeDef,
     CopyImageResponseTypeDef,
+    CreateAppBlockBuilderResultTypeDef,
+    CreateAppBlockBuilderStreamingURLResultTypeDef,
     CreateAppBlockResultTypeDef,
     CreateApplicationResultTypeDef,
     CreateDirectoryConfigResultTypeDef,
     CreateEntitlementResultTypeDef,
     CreateFleetResultTypeDef,
     CreateImageBuilderResultTypeDef,
     CreateImageBuilderStreamingURLResultTypeDef,
     CreateStackResultTypeDef,
     CreateStreamingURLResultTypeDef,
     CreateUpdatedImageResultTypeDef,
     CreateUsageReportSubscriptionResultTypeDef,
     DeleteImageBuilderResultTypeDef,
     DeleteImageResultTypeDef,
+    DescribeAppBlockBuilderAppBlockAssociationsResultTypeDef,
+    DescribeAppBlockBuildersResultTypeDef,
     DescribeAppBlocksResultTypeDef,
     DescribeApplicationFleetAssociationsResultTypeDef,
     DescribeApplicationsResultTypeDef,
     DescribeDirectoryConfigsResultTypeDef,
     DescribeEntitlementsResultTypeDef,
     DescribeFleetsResultTypeDef,
     DescribeImageBuildersResultTypeDef,
@@ -86,18 +93,21 @@
     ListAssociatedFleetsResultTypeDef,
     ListAssociatedStacksResultTypeDef,
     ListEntitledApplicationsResultTypeDef,
     ListTagsForResourceResponseTypeDef,
     S3LocationTypeDef,
     ScriptDetailsTypeDef,
     ServiceAccountCredentialsTypeDef,
+    StartAppBlockBuilderResultTypeDef,
     StartImageBuilderResultTypeDef,
+    StopAppBlockBuilderResultTypeDef,
     StopImageBuilderResultTypeDef,
     StorageConnectorTypeDef,
     StreamingExperienceSettingsTypeDef,
+    UpdateAppBlockBuilderResultTypeDef,
     UpdateApplicationResultTypeDef,
     UpdateDirectoryConfigResultTypeDef,
     UpdateEntitlementResultTypeDef,
     UpdateFleetResultTypeDef,
     UpdateStackResultTypeDef,
     UserSettingTypeDef,
     UserStackAssociationTypeDef,
@@ -153,14 +163,24 @@
         """
         AppStreamClient exceptions.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appstream.html#AppStream.Client.exceptions)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appstream/client/#exceptions)
         """
 
+    async def associate_app_block_builder_app_block(
+        self, *, AppBlockArn: str, AppBlockBuilderName: str
+    ) -> AssociateAppBlockBuilderAppBlockResultTypeDef:
+        """
+        Associates the specified app block builder with the specified app block.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appstream.html#AppStream.Client.associate_app_block_builder_app_block)
+        [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appstream/client/#associate_app_block_builder_app_block)
+        """
+
     async def associate_application_fleet(
         self, *, FleetName: str, ApplicationArn: str
     ) -> AssociateApplicationFleetResultTypeDef:
         """
         Associates the specified application with the specified fleet.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appstream.html#AppStream.Client.associate_application_fleet)
@@ -238,26 +258,59 @@
         """
 
     async def create_app_block(
         self,
         *,
         Name: str,
         SourceS3Location: S3LocationTypeDef,
-        SetupScriptDetails: ScriptDetailsTypeDef,
         Description: str = ...,
         DisplayName: str = ...,
-        Tags: Mapping[str, str] = ...
+        SetupScriptDetails: ScriptDetailsTypeDef = ...,
+        Tags: Mapping[str, str] = ...,
+        PostSetupScriptDetails: ScriptDetailsTypeDef = ...,
+        PackagingType: PackagingTypeType = ...
     ) -> CreateAppBlockResultTypeDef:
         """
         Creates an app block.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appstream.html#AppStream.Client.create_app_block)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appstream/client/#create_app_block)
         """
 
+    async def create_app_block_builder(
+        self,
+        *,
+        Name: str,
+        Platform: Literal["WINDOWS_SERVER_2019"],
+        InstanceType: str,
+        VpcConfig: VpcConfigTypeDef,
+        Description: str = ...,
+        DisplayName: str = ...,
+        Tags: Mapping[str, str] = ...,
+        EnableDefaultInternetAccess: bool = ...,
+        IamRoleArn: str = ...,
+        AccessEndpoints: Sequence[AccessEndpointTypeDef] = ...
+    ) -> CreateAppBlockBuilderResultTypeDef:
+        """
+        Creates an app block builder.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appstream.html#AppStream.Client.create_app_block_builder)
+        [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appstream/client/#create_app_block_builder)
+        """
+
+    async def create_app_block_builder_streaming_url(
+        self, *, AppBlockBuilderName: str, Validity: int = ...
+    ) -> CreateAppBlockBuilderStreamingURLResultTypeDef:
+        """
+        Creates a URL to start a create app block builder streaming session.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appstream.html#AppStream.Client.create_app_block_builder_streaming_url)
+        [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appstream/client/#create_app_block_builder_streaming_url)
+        """
+
     async def create_application(
         self,
         *,
         Name: str,
         IconS3Location: S3LocationTypeDef,
         LaunchPath: str,
         Platforms: Sequence[PlatformTypeType],
@@ -460,14 +513,22 @@
         """
         Deletes an app block.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appstream.html#AppStream.Client.delete_app_block)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appstream/client/#delete_app_block)
         """
 
+    async def delete_app_block_builder(self, *, Name: str) -> Dict[str, Any]:
+        """
+        Deletes an app block builder.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appstream.html#AppStream.Client.delete_app_block_builder)
+        [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appstream/client/#delete_app_block_builder)
+        """
+
     async def delete_application(self, *, Name: str) -> Dict[str, Any]:
         """
         Deletes an application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appstream.html#AppStream.Client.delete_application)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appstream/client/#delete_application)
         """
@@ -542,14 +603,39 @@
         """
         Deletes a user from the user pool.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appstream.html#AppStream.Client.delete_user)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appstream/client/#delete_user)
         """
 
+    async def describe_app_block_builder_app_block_associations(
+        self,
+        *,
+        AppBlockArn: str = ...,
+        AppBlockBuilderName: str = ...,
+        MaxResults: int = ...,
+        NextToken: str = ...
+    ) -> DescribeAppBlockBuilderAppBlockAssociationsResultTypeDef:
+        """
+        Retrieves a list that describes one or more app block builder associations.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appstream.html#AppStream.Client.describe_app_block_builder_app_block_associations)
+        [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appstream/client/#describe_app_block_builder_app_block_associations)
+        """
+
+    async def describe_app_block_builders(
+        self, *, Names: Sequence[str] = ..., NextToken: str = ..., MaxResults: int = ...
+    ) -> DescribeAppBlockBuildersResultTypeDef:
+        """
+        Retrieves a list that describes one or more app block builders.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appstream.html#AppStream.Client.describe_app_block_builders)
+        [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appstream/client/#describe_app_block_builders)
+        """
+
     async def describe_app_blocks(
         self, *, Arns: Sequence[str] = ..., NextToken: str = ..., MaxResults: int = ...
     ) -> DescribeAppBlocksResultTypeDef:
         """
         Retrieves a list that describes one or more app blocks.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appstream.html#AppStream.Client.describe_app_blocks)
@@ -732,14 +818,24 @@
         """
         Disables the specified user in the user pool.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appstream.html#AppStream.Client.disable_user)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appstream/client/#disable_user)
         """
 
+    async def disassociate_app_block_builder_app_block(
+        self, *, AppBlockArn: str, AppBlockBuilderName: str
+    ) -> Dict[str, Any]:
+        """
+        Disassociates a specified app block builder from a specified app block.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appstream.html#AppStream.Client.disassociate_app_block_builder_app_block)
+        [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appstream/client/#disassociate_app_block_builder_app_block)
+        """
+
     async def disassociate_application_fleet(
         self, *, FleetName: str, ApplicationArn: str
     ) -> Dict[str, Any]:
         """
         Disassociates the specified application from the fleet.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appstream.html#AppStream.Client.disassociate_application_fleet)
@@ -832,14 +928,22 @@
         """
         Retrieves a list of all tags for the specified AppStream 2.0 resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appstream.html#AppStream.Client.list_tags_for_resource)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appstream/client/#list_tags_for_resource)
         """
 
+    async def start_app_block_builder(self, *, Name: str) -> StartAppBlockBuilderResultTypeDef:
+        """
+        Starts an app block builder.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appstream.html#AppStream.Client.start_app_block_builder)
+        [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appstream/client/#start_app_block_builder)
+        """
+
     async def start_fleet(self, *, Name: str) -> Dict[str, Any]:
         """
         Starts the specified fleet.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appstream.html#AppStream.Client.start_fleet)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appstream/client/#start_fleet)
         """
@@ -850,14 +954,22 @@
         """
         Starts the specified image builder.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appstream.html#AppStream.Client.start_image_builder)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appstream/client/#start_image_builder)
         """
 
+    async def stop_app_block_builder(self, *, Name: str) -> StopAppBlockBuilderResultTypeDef:
+        """
+        Stops an app block builder.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appstream.html#AppStream.Client.stop_app_block_builder)
+        [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appstream/client/#stop_app_block_builder)
+        """
+
     async def stop_fleet(self, *, Name: str) -> Dict[str, Any]:
         """
         Stops the specified fleet.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appstream.html#AppStream.Client.stop_fleet)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appstream/client/#stop_fleet)
         """
@@ -883,14 +995,35 @@
         Disassociates one or more specified tags from the specified AppStream 2.0
         resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appstream.html#AppStream.Client.untag_resource)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appstream/client/#untag_resource)
         """
 
+    async def update_app_block_builder(
+        self,
+        *,
+        Name: str,
+        Description: str = ...,
+        DisplayName: str = ...,
+        Platform: PlatformTypeType = ...,
+        InstanceType: str = ...,
+        VpcConfig: VpcConfigTypeDef = ...,
+        EnableDefaultInternetAccess: bool = ...,
+        IamRoleArn: str = ...,
+        AccessEndpoints: Sequence[AccessEndpointTypeDef] = ...,
+        AttributesToDelete: Sequence[AppBlockBuilderAttributeType] = ...
+    ) -> UpdateAppBlockBuilderResultTypeDef:
+        """
+        Updates an app block builder.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appstream.html#AppStream.Client.update_app_block_builder)
+        [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appstream/client/#update_app_block_builder)
+        """
+
     async def update_application(
         self,
         *,
         Name: str,
         DisplayName: str = ...,
         Description: str = ...,
         IconS3Location: S3LocationTypeDef = ...,
```

### Comparing `types-aiobotocore-appstream-2.5.2.post3/types_aiobotocore_appstream/client.pyi` & `types-aiobotocore-appstream-2.5.4/types_aiobotocore_appstream/client.pyi`

 * *Files 8% similar despite different names*

```diff
@@ -17,20 +17,22 @@
 import sys
 from typing import Any, Dict, Mapping, Sequence, Type, overload
 
 from aiobotocore.client import AioBaseClient
 from botocore.client import ClientMeta
 
 from .literals import (
+    AppBlockBuilderAttributeType,
     ApplicationAttributeType,
     AppVisibilityType,
     AuthenticationTypeType,
     FleetAttributeType,
     FleetTypeType,
     MessageActionType,
+    PackagingTypeType,
     PlatformTypeType,
     StackAttributeType,
     StreamViewType,
     VisibilityTypeType,
 )
 from .paginator import (
     DescribeDirectoryConfigsPaginator,
@@ -43,33 +45,38 @@
     DescribeUserStackAssociationsPaginator,
     ListAssociatedFleetsPaginator,
     ListAssociatedStacksPaginator,
 )
 from .type_defs import (
     AccessEndpointTypeDef,
     ApplicationSettingsTypeDef,
+    AssociateAppBlockBuilderAppBlockResultTypeDef,
     AssociateApplicationFleetResultTypeDef,
     BatchAssociateUserStackResultTypeDef,
     BatchDisassociateUserStackResultTypeDef,
     CertificateBasedAuthPropertiesTypeDef,
     ComputeCapacityTypeDef,
     CopyImageResponseTypeDef,
+    CreateAppBlockBuilderResultTypeDef,
+    CreateAppBlockBuilderStreamingURLResultTypeDef,
     CreateAppBlockResultTypeDef,
     CreateApplicationResultTypeDef,
     CreateDirectoryConfigResultTypeDef,
     CreateEntitlementResultTypeDef,
     CreateFleetResultTypeDef,
     CreateImageBuilderResultTypeDef,
     CreateImageBuilderStreamingURLResultTypeDef,
     CreateStackResultTypeDef,
     CreateStreamingURLResultTypeDef,
     CreateUpdatedImageResultTypeDef,
     CreateUsageReportSubscriptionResultTypeDef,
     DeleteImageBuilderResultTypeDef,
     DeleteImageResultTypeDef,
+    DescribeAppBlockBuilderAppBlockAssociationsResultTypeDef,
+    DescribeAppBlockBuildersResultTypeDef,
     DescribeAppBlocksResultTypeDef,
     DescribeApplicationFleetAssociationsResultTypeDef,
     DescribeApplicationsResultTypeDef,
     DescribeDirectoryConfigsResultTypeDef,
     DescribeEntitlementsResultTypeDef,
     DescribeFleetsResultTypeDef,
     DescribeImageBuildersResultTypeDef,
@@ -86,18 +93,21 @@
     ListAssociatedFleetsResultTypeDef,
     ListAssociatedStacksResultTypeDef,
     ListEntitledApplicationsResultTypeDef,
     ListTagsForResourceResponseTypeDef,
     S3LocationTypeDef,
     ScriptDetailsTypeDef,
     ServiceAccountCredentialsTypeDef,
+    StartAppBlockBuilderResultTypeDef,
     StartImageBuilderResultTypeDef,
+    StopAppBlockBuilderResultTypeDef,
     StopImageBuilderResultTypeDef,
     StorageConnectorTypeDef,
     StreamingExperienceSettingsTypeDef,
+    UpdateAppBlockBuilderResultTypeDef,
     UpdateApplicationResultTypeDef,
     UpdateDirectoryConfigResultTypeDef,
     UpdateEntitlementResultTypeDef,
     UpdateFleetResultTypeDef,
     UpdateStackResultTypeDef,
     UserSettingTypeDef,
     UserStackAssociationTypeDef,
@@ -148,14 +158,23 @@
     def exceptions(self) -> Exceptions:
         """
         AppStreamClient exceptions.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appstream.html#AppStream.Client.exceptions)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appstream/client/#exceptions)
         """
+    async def associate_app_block_builder_app_block(
+        self, *, AppBlockArn: str, AppBlockBuilderName: str
+    ) -> AssociateAppBlockBuilderAppBlockResultTypeDef:
+        """
+        Associates the specified app block builder with the specified app block.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appstream.html#AppStream.Client.associate_app_block_builder_app_block)
+        [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appstream/client/#associate_app_block_builder_app_block)
+        """
     async def associate_application_fleet(
         self, *, FleetName: str, ApplicationArn: str
     ) -> AssociateApplicationFleetResultTypeDef:
         """
         Associates the specified application with the specified fleet.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appstream.html#AppStream.Client.associate_application_fleet)
@@ -225,25 +244,56 @@
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appstream/client/#copy_image)
         """
     async def create_app_block(
         self,
         *,
         Name: str,
         SourceS3Location: S3LocationTypeDef,
-        SetupScriptDetails: ScriptDetailsTypeDef,
         Description: str = ...,
         DisplayName: str = ...,
-        Tags: Mapping[str, str] = ...
+        SetupScriptDetails: ScriptDetailsTypeDef = ...,
+        Tags: Mapping[str, str] = ...,
+        PostSetupScriptDetails: ScriptDetailsTypeDef = ...,
+        PackagingType: PackagingTypeType = ...
     ) -> CreateAppBlockResultTypeDef:
         """
         Creates an app block.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appstream.html#AppStream.Client.create_app_block)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appstream/client/#create_app_block)
         """
+    async def create_app_block_builder(
+        self,
+        *,
+        Name: str,
+        Platform: Literal["WINDOWS_SERVER_2019"],
+        InstanceType: str,
+        VpcConfig: VpcConfigTypeDef,
+        Description: str = ...,
+        DisplayName: str = ...,
+        Tags: Mapping[str, str] = ...,
+        EnableDefaultInternetAccess: bool = ...,
+        IamRoleArn: str = ...,
+        AccessEndpoints: Sequence[AccessEndpointTypeDef] = ...
+    ) -> CreateAppBlockBuilderResultTypeDef:
+        """
+        Creates an app block builder.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appstream.html#AppStream.Client.create_app_block_builder)
+        [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appstream/client/#create_app_block_builder)
+        """
+    async def create_app_block_builder_streaming_url(
+        self, *, AppBlockBuilderName: str, Validity: int = ...
+    ) -> CreateAppBlockBuilderStreamingURLResultTypeDef:
+        """
+        Creates a URL to start a create app block builder streaming session.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appstream.html#AppStream.Client.create_app_block_builder_streaming_url)
+        [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appstream/client/#create_app_block_builder_streaming_url)
+        """
     async def create_application(
         self,
         *,
         Name: str,
         IconS3Location: S3LocationTypeDef,
         LaunchPath: str,
         Platforms: Sequence[PlatformTypeType],
@@ -434,14 +484,21 @@
     async def delete_app_block(self, *, Name: str) -> Dict[str, Any]:
         """
         Deletes an app block.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appstream.html#AppStream.Client.delete_app_block)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appstream/client/#delete_app_block)
         """
+    async def delete_app_block_builder(self, *, Name: str) -> Dict[str, Any]:
+        """
+        Deletes an app block builder.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appstream.html#AppStream.Client.delete_app_block_builder)
+        [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appstream/client/#delete_app_block_builder)
+        """
     async def delete_application(self, *, Name: str) -> Dict[str, Any]:
         """
         Deletes an application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appstream.html#AppStream.Client.delete_application)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appstream/client/#delete_application)
         """
@@ -506,14 +563,37 @@
     ) -> Dict[str, Any]:
         """
         Deletes a user from the user pool.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appstream.html#AppStream.Client.delete_user)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appstream/client/#delete_user)
         """
+    async def describe_app_block_builder_app_block_associations(
+        self,
+        *,
+        AppBlockArn: str = ...,
+        AppBlockBuilderName: str = ...,
+        MaxResults: int = ...,
+        NextToken: str = ...
+    ) -> DescribeAppBlockBuilderAppBlockAssociationsResultTypeDef:
+        """
+        Retrieves a list that describes one or more app block builder associations.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appstream.html#AppStream.Client.describe_app_block_builder_app_block_associations)
+        [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appstream/client/#describe_app_block_builder_app_block_associations)
+        """
+    async def describe_app_block_builders(
+        self, *, Names: Sequence[str] = ..., NextToken: str = ..., MaxResults: int = ...
+    ) -> DescribeAppBlockBuildersResultTypeDef:
+        """
+        Retrieves a list that describes one or more app block builders.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appstream.html#AppStream.Client.describe_app_block_builders)
+        [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appstream/client/#describe_app_block_builders)
+        """
     async def describe_app_blocks(
         self, *, Arns: Sequence[str] = ..., NextToken: str = ..., MaxResults: int = ...
     ) -> DescribeAppBlocksResultTypeDef:
         """
         Retrieves a list that describes one or more app blocks.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appstream.html#AppStream.Client.describe_app_blocks)
@@ -681,14 +761,23 @@
     ) -> Dict[str, Any]:
         """
         Disables the specified user in the user pool.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appstream.html#AppStream.Client.disable_user)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appstream/client/#disable_user)
         """
+    async def disassociate_app_block_builder_app_block(
+        self, *, AppBlockArn: str, AppBlockBuilderName: str
+    ) -> Dict[str, Any]:
+        """
+        Disassociates a specified app block builder from a specified app block.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appstream.html#AppStream.Client.disassociate_app_block_builder_app_block)
+        [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appstream/client/#disassociate_app_block_builder_app_block)
+        """
     async def disassociate_application_fleet(
         self, *, FleetName: str, ApplicationArn: str
     ) -> Dict[str, Any]:
         """
         Disassociates the specified application from the fleet.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appstream.html#AppStream.Client.disassociate_application_fleet)
@@ -771,14 +860,21 @@
     ) -> ListTagsForResourceResponseTypeDef:
         """
         Retrieves a list of all tags for the specified AppStream 2.0 resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appstream.html#AppStream.Client.list_tags_for_resource)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appstream/client/#list_tags_for_resource)
         """
+    async def start_app_block_builder(self, *, Name: str) -> StartAppBlockBuilderResultTypeDef:
+        """
+        Starts an app block builder.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appstream.html#AppStream.Client.start_app_block_builder)
+        [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appstream/client/#start_app_block_builder)
+        """
     async def start_fleet(self, *, Name: str) -> Dict[str, Any]:
         """
         Starts the specified fleet.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appstream.html#AppStream.Client.start_fleet)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appstream/client/#start_fleet)
         """
@@ -787,14 +883,21 @@
     ) -> StartImageBuilderResultTypeDef:
         """
         Starts the specified image builder.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appstream.html#AppStream.Client.start_image_builder)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appstream/client/#start_image_builder)
         """
+    async def stop_app_block_builder(self, *, Name: str) -> StopAppBlockBuilderResultTypeDef:
+        """
+        Stops an app block builder.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appstream.html#AppStream.Client.stop_app_block_builder)
+        [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appstream/client/#stop_app_block_builder)
+        """
     async def stop_fleet(self, *, Name: str) -> Dict[str, Any]:
         """
         Stops the specified fleet.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appstream.html#AppStream.Client.stop_fleet)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appstream/client/#stop_fleet)
         """
@@ -816,14 +919,34 @@
         """
         Disassociates one or more specified tags from the specified AppStream 2.0
         resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appstream.html#AppStream.Client.untag_resource)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appstream/client/#untag_resource)
         """
+    async def update_app_block_builder(
+        self,
+        *,
+        Name: str,
+        Description: str = ...,
+        DisplayName: str = ...,
+        Platform: PlatformTypeType = ...,
+        InstanceType: str = ...,
+        VpcConfig: VpcConfigTypeDef = ...,
+        EnableDefaultInternetAccess: bool = ...,
+        IamRoleArn: str = ...,
+        AccessEndpoints: Sequence[AccessEndpointTypeDef] = ...,
+        AttributesToDelete: Sequence[AppBlockBuilderAttributeType] = ...
+    ) -> UpdateAppBlockBuilderResultTypeDef:
+        """
+        Updates an app block builder.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appstream.html#AppStream.Client.update_app_block_builder)
+        [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appstream/client/#update_app_block_builder)
+        """
     async def update_application(
         self,
         *,
         Name: str,
         DisplayName: str = ...,
         Description: str = ...,
         IconS3Location: S3LocationTypeDef = ...,
```

### Comparing `types-aiobotocore-appstream-2.5.2.post3/types_aiobotocore_appstream/literals.py` & `types-aiobotocore-appstream-2.5.4/types_aiobotocore_appstream/literals.py`

 * *Files 3% similar despite different names*

```diff
@@ -18,14 +18,19 @@
 else:
     from typing_extensions import Literal
 
 
 __all__ = (
     "AccessEndpointTypeType",
     "ActionType",
+    "AppBlockBuilderAttributeType",
+    "AppBlockBuilderPlatformTypeType",
+    "AppBlockBuilderStateChangeReasonCodeType",
+    "AppBlockBuilderStateType",
+    "AppBlockStateType",
     "AppVisibilityType",
     "ApplicationAttributeType",
     "AuthenticationTypeType",
     "CertificateBasedAuthStatusType",
     "DescribeDirectoryConfigsPaginatorName",
     "DescribeFleetsPaginatorName",
     "DescribeImageBuildersPaginatorName",
@@ -43,14 +48,15 @@
     "ImageBuilderStateChangeReasonCodeType",
     "ImageBuilderStateType",
     "ImageStateChangeReasonCodeType",
     "ImageStateType",
     "ListAssociatedFleetsPaginatorName",
     "ListAssociatedStacksPaginatorName",
     "MessageActionType",
+    "PackagingTypeType",
     "PermissionType",
     "PlatformTypeType",
     "PreferredProtocolType",
     "SessionConnectionStateType",
     "SessionStateType",
     "StackAttributeType",
     "StackErrorCodeType",
@@ -75,14 +81,21 @@
     "CLIPBOARD_COPY_TO_LOCAL_DEVICE",
     "DOMAIN_PASSWORD_SIGNIN",
     "DOMAIN_SMART_CARD_SIGNIN",
     "FILE_DOWNLOAD",
     "FILE_UPLOAD",
     "PRINTING_TO_LOCAL_DEVICE",
 ]
+AppBlockBuilderAttributeType = Literal[
+    "ACCESS_ENDPOINTS", "IAM_ROLE_ARN", "VPC_CONFIGURATION_SECURITY_GROUP_IDS"
+]
+AppBlockBuilderPlatformTypeType = Literal["WINDOWS_SERVER_2019"]
+AppBlockBuilderStateChangeReasonCodeType = Literal["INTERNAL_ERROR"]
+AppBlockBuilderStateType = Literal["RUNNING", "STARTING", "STOPPED", "STOPPING"]
+AppBlockStateType = Literal["ACTIVE", "INACTIVE"]
 AppVisibilityType = Literal["ALL", "ASSOCIATED"]
 ApplicationAttributeType = Literal["LAUNCH_PARAMETERS", "WORKING_DIRECTORY"]
 AuthenticationTypeType = Literal["API", "AWS_AD", "SAML", "USERPOOL"]
 CertificateBasedAuthStatusType = Literal[
     "DISABLED", "ENABLED", "ENABLED_NO_DIRECTORY_LOGIN_FALLBACK"
 ]
 DescribeDirectoryConfigsPaginatorName = Literal["describe_directory_configs"]
@@ -156,14 +169,15 @@
 ]
 ImageStateType = Literal[
     "AVAILABLE", "COPYING", "CREATING", "DELETING", "FAILED", "IMPORTING", "PENDING"
 ]
 ListAssociatedFleetsPaginatorName = Literal["list_associated_fleets"]
 ListAssociatedStacksPaginatorName = Literal["list_associated_stacks"]
 MessageActionType = Literal["RESEND", "SUPPRESS"]
+PackagingTypeType = Literal["APPSTREAM2", "CUSTOM"]
 PermissionType = Literal["DISABLED", "ENABLED"]
 PlatformTypeType = Literal["AMAZON_LINUX2", "WINDOWS", "WINDOWS_SERVER_2016", "WINDOWS_SERVER_2019"]
 PreferredProtocolType = Literal["TCP", "UDP"]
 SessionConnectionStateType = Literal["CONNECTED", "NOT_CONNECTED"]
 SessionStateType = Literal["ACTIVE", "EXPIRED", "PENDING"]
 StackAttributeType = Literal[
     "ACCESS_ENDPOINTS",
@@ -202,14 +216,15 @@
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
@@ -305,14 +320,15 @@
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
@@ -391,26 +407,28 @@
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

### Comparing `types-aiobotocore-appstream-2.5.2.post3/types_aiobotocore_appstream/literals.pyi` & `types-aiobotocore-appstream-2.5.4/types_aiobotocore_appstream/literals.pyi`

 * *Files 3% similar despite different names*

```diff
@@ -17,14 +17,19 @@
     from typing import Literal
 else:
     from typing_extensions import Literal
 
 __all__ = (
     "AccessEndpointTypeType",
     "ActionType",
+    "AppBlockBuilderAttributeType",
+    "AppBlockBuilderPlatformTypeType",
+    "AppBlockBuilderStateChangeReasonCodeType",
+    "AppBlockBuilderStateType",
+    "AppBlockStateType",
     "AppVisibilityType",
     "ApplicationAttributeType",
     "AuthenticationTypeType",
     "CertificateBasedAuthStatusType",
     "DescribeDirectoryConfigsPaginatorName",
     "DescribeFleetsPaginatorName",
     "DescribeImageBuildersPaginatorName",
@@ -42,14 +47,15 @@
     "ImageBuilderStateChangeReasonCodeType",
     "ImageBuilderStateType",
     "ImageStateChangeReasonCodeType",
     "ImageStateType",
     "ListAssociatedFleetsPaginatorName",
     "ListAssociatedStacksPaginatorName",
     "MessageActionType",
+    "PackagingTypeType",
     "PermissionType",
     "PlatformTypeType",
     "PreferredProtocolType",
     "SessionConnectionStateType",
     "SessionStateType",
     "StackAttributeType",
     "StackErrorCodeType",
@@ -73,14 +79,21 @@
     "CLIPBOARD_COPY_TO_LOCAL_DEVICE",
     "DOMAIN_PASSWORD_SIGNIN",
     "DOMAIN_SMART_CARD_SIGNIN",
     "FILE_DOWNLOAD",
     "FILE_UPLOAD",
     "PRINTING_TO_LOCAL_DEVICE",
 ]
+AppBlockBuilderAttributeType = Literal[
+    "ACCESS_ENDPOINTS", "IAM_ROLE_ARN", "VPC_CONFIGURATION_SECURITY_GROUP_IDS"
+]
+AppBlockBuilderPlatformTypeType = Literal["WINDOWS_SERVER_2019"]
+AppBlockBuilderStateChangeReasonCodeType = Literal["INTERNAL_ERROR"]
+AppBlockBuilderStateType = Literal["RUNNING", "STARTING", "STOPPED", "STOPPING"]
+AppBlockStateType = Literal["ACTIVE", "INACTIVE"]
 AppVisibilityType = Literal["ALL", "ASSOCIATED"]
 ApplicationAttributeType = Literal["LAUNCH_PARAMETERS", "WORKING_DIRECTORY"]
 AuthenticationTypeType = Literal["API", "AWS_AD", "SAML", "USERPOOL"]
 CertificateBasedAuthStatusType = Literal[
     "DISABLED", "ENABLED", "ENABLED_NO_DIRECTORY_LOGIN_FALLBACK"
 ]
 DescribeDirectoryConfigsPaginatorName = Literal["describe_directory_configs"]
@@ -154,14 +167,15 @@
 ]
 ImageStateType = Literal[
     "AVAILABLE", "COPYING", "CREATING", "DELETING", "FAILED", "IMPORTING", "PENDING"
 ]
 ListAssociatedFleetsPaginatorName = Literal["list_associated_fleets"]
 ListAssociatedStacksPaginatorName = Literal["list_associated_stacks"]
 MessageActionType = Literal["RESEND", "SUPPRESS"]
+PackagingTypeType = Literal["APPSTREAM2", "CUSTOM"]
 PermissionType = Literal["DISABLED", "ENABLED"]
 PlatformTypeType = Literal["AMAZON_LINUX2", "WINDOWS", "WINDOWS_SERVER_2016", "WINDOWS_SERVER_2019"]
 PreferredProtocolType = Literal["TCP", "UDP"]
 SessionConnectionStateType = Literal["CONNECTED", "NOT_CONNECTED"]
 SessionStateType = Literal["ACTIVE", "EXPIRED", "PENDING"]
 StackAttributeType = Literal[
     "ACCESS_ENDPOINTS",
@@ -200,14 +214,15 @@
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
@@ -303,14 +318,15 @@
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
@@ -389,26 +405,28 @@
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

### Comparing `types-aiobotocore-appstream-2.5.2.post3/types_aiobotocore_appstream/paginator.py` & `types-aiobotocore-appstream-2.5.4/types_aiobotocore_appstream/paginator.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-appstream-2.5.2.post3/types_aiobotocore_appstream/paginator.pyi` & `types-aiobotocore-appstream-2.5.4/types_aiobotocore_appstream/paginator.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-appstream-2.5.2.post3/types_aiobotocore_appstream/type_defs.py` & `types-aiobotocore-appstream-2.5.4/types_aiobotocore_appstream/type_defs.py`

 * *Files 3% similar despite different names*

```diff
@@ -13,27 +13,31 @@
 """
 import sys
 from datetime import datetime
 from typing import Dict, List, Mapping, Sequence
 
 from .literals import (
     ActionType,
+    AppBlockBuilderAttributeType,
+    AppBlockBuilderStateType,
+    AppBlockStateType,
     ApplicationAttributeType,
     AppVisibilityType,
     AuthenticationTypeType,
     CertificateBasedAuthStatusType,
     FleetAttributeType,
     FleetErrorCodeType,
     FleetStateType,
     FleetTypeType,
     ImageBuilderStateChangeReasonCodeType,
     ImageBuilderStateType,
     ImageStateChangeReasonCodeType,
     ImageStateType,
     MessageActionType,
+    PackagingTypeType,
     PermissionType,
     PlatformTypeType,
     PreferredProtocolType,
     SessionConnectionStateType,
     SessionStateType,
     StackAttributeType,
     StackErrorCodeType,
@@ -52,48 +56,57 @@
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 
 __all__ = (
     "AccessEndpointTypeDef",
+    "AppBlockBuilderAppBlockAssociationTypeDef",
+    "AppBlockBuilderStateChangeReasonTypeDef",
+    "ResourceErrorTypeDef",
+    "VpcConfigTypeDef",
+    "ErrorDetailsTypeDef",
     "S3LocationTypeDef",
     "ApplicationFleetAssociationTypeDef",
     "ApplicationSettingsResponseTypeDef",
     "ApplicationSettingsTypeDef",
-    "AssociateApplicationFleetRequestRequestTypeDef",
+    "AssociateAppBlockBuilderAppBlockRequestRequestTypeDef",
     "ResponseMetadataTypeDef",
+    "AssociateApplicationFleetRequestRequestTypeDef",
     "AssociateApplicationToEntitlementRequestRequestTypeDef",
     "AssociateFleetRequestRequestTypeDef",
     "UserStackAssociationTypeDef",
     "CertificateBasedAuthPropertiesTypeDef",
     "ComputeCapacityStatusTypeDef",
     "ComputeCapacityTypeDef",
     "CopyImageRequestRequestTypeDef",
+    "CreateAppBlockBuilderStreamingURLRequestRequestTypeDef",
     "ServiceAccountCredentialsTypeDef",
     "EntitlementAttributeTypeDef",
     "DomainJoinInfoTypeDef",
-    "VpcConfigTypeDef",
     "CreateImageBuilderStreamingURLRequestRequestTypeDef",
     "StorageConnectorTypeDef",
     "StreamingExperienceSettingsTypeDef",
     "UserSettingTypeDef",
     "CreateStreamingURLRequestRequestTypeDef",
     "CreateUpdatedImageRequestRequestTypeDef",
     "CreateUserRequestRequestTypeDef",
+    "DeleteAppBlockBuilderRequestRequestTypeDef",
     "DeleteAppBlockRequestRequestTypeDef",
     "DeleteApplicationRequestRequestTypeDef",
     "DeleteDirectoryConfigRequestRequestTypeDef",
     "DeleteEntitlementRequestRequestTypeDef",
     "DeleteFleetRequestRequestTypeDef",
     "DeleteImageBuilderRequestRequestTypeDef",
     "DeleteImagePermissionsRequestRequestTypeDef",
     "DeleteImageRequestRequestTypeDef",
     "DeleteStackRequestRequestTypeDef",
     "DeleteUserRequestRequestTypeDef",
+    "DescribeAppBlockBuilderAppBlockAssociationsRequestRequestTypeDef",
+    "DescribeAppBlockBuildersRequestRequestTypeDef",
     "DescribeAppBlocksRequestRequestTypeDef",
     "DescribeApplicationFleetAssociationsRequestRequestTypeDef",
     "DescribeApplicationsRequestRequestTypeDef",
     "PaginatorConfigTypeDef",
     "DescribeDirectoryConfigsRequestRequestTypeDef",
     "DescribeEntitlementsRequestRequestTypeDef",
     "WaiterConfigTypeDef",
@@ -104,47 +117,55 @@
     "DescribeSessionsRequestRequestTypeDef",
     "DescribeStacksRequestRequestTypeDef",
     "DescribeUsageReportSubscriptionsRequestRequestTypeDef",
     "DescribeUserStackAssociationsRequestRequestTypeDef",
     "DescribeUsersRequestRequestTypeDef",
     "UserTypeDef",
     "DisableUserRequestRequestTypeDef",
+    "DisassociateAppBlockBuilderAppBlockRequestRequestTypeDef",
     "DisassociateApplicationFleetRequestRequestTypeDef",
     "DisassociateApplicationFromEntitlementRequestRequestTypeDef",
     "DisassociateFleetRequestRequestTypeDef",
     "EnableUserRequestRequestTypeDef",
     "EntitledApplicationTypeDef",
     "ExpireSessionRequestRequestTypeDef",
     "FleetErrorTypeDef",
     "ImageBuilderStateChangeReasonTypeDef",
     "NetworkAccessConfigurationTypeDef",
-    "ResourceErrorTypeDef",
     "ImagePermissionsTypeDef",
     "ImageStateChangeReasonTypeDef",
     "LastReportGenerationExecutionErrorTypeDef",
     "ListAssociatedFleetsRequestRequestTypeDef",
     "ListAssociatedStacksRequestRequestTypeDef",
     "ListEntitledApplicationsRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
     "StackErrorTypeDef",
+    "StartAppBlockBuilderRequestRequestTypeDef",
     "StartFleetRequestRequestTypeDef",
     "StartImageBuilderRequestRequestTypeDef",
+    "StopAppBlockBuilderRequestRequestTypeDef",
     "StopFleetRequestRequestTypeDef",
     "StopImageBuilderRequestRequestTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
+    "AppBlockBuilderTypeDef",
+    "CreateAppBlockBuilderRequestRequestTypeDef",
+    "UpdateAppBlockBuilderRequestRequestTypeDef",
     "ApplicationTypeDef",
     "CreateApplicationRequestRequestTypeDef",
     "ScriptDetailsTypeDef",
     "UpdateApplicationRequestRequestTypeDef",
+    "AssociateAppBlockBuilderAppBlockResultTypeDef",
     "AssociateApplicationFleetResultTypeDef",
     "CopyImageResponseTypeDef",
+    "CreateAppBlockBuilderStreamingURLResultTypeDef",
     "CreateImageBuilderStreamingURLResultTypeDef",
     "CreateStreamingURLResultTypeDef",
     "CreateUsageReportSubscriptionResultTypeDef",
+    "DescribeAppBlockBuilderAppBlockAssociationsResultTypeDef",
     "DescribeApplicationFleetAssociationsResultTypeDef",
     "ListAssociatedFleetsResultTypeDef",
     "ListAssociatedStacksResultTypeDef",
     "ListTagsForResourceResponseTypeDef",
     "BatchAssociateUserStackRequestRequestTypeDef",
     "BatchDisassociateUserStackRequestRequestTypeDef",
     "DescribeUserStackAssociationsResultTypeDef",
@@ -171,20 +192,25 @@
     "ListAssociatedFleetsRequestListAssociatedFleetsPaginateTypeDef",
     "ListAssociatedStacksRequestListAssociatedStacksPaginateTypeDef",
     "DescribeFleetsRequestFleetStartedWaitTypeDef",
     "DescribeFleetsRequestFleetStoppedWaitTypeDef",
     "DescribeUsersResultTypeDef",
     "ListEntitledApplicationsResultTypeDef",
     "FleetTypeDef",
-    "SessionTypeDef",
     "ImageBuilderTypeDef",
+    "SessionTypeDef",
     "SharedImagePermissionsTypeDef",
     "UpdateImagePermissionsRequestRequestTypeDef",
     "UsageReportSubscriptionTypeDef",
     "StackTypeDef",
+    "CreateAppBlockBuilderResultTypeDef",
+    "DescribeAppBlockBuildersResultTypeDef",
+    "StartAppBlockBuilderResultTypeDef",
+    "StopAppBlockBuilderResultTypeDef",
+    "UpdateAppBlockBuilderResultTypeDef",
     "CreateApplicationResultTypeDef",
     "DescribeApplicationsResultTypeDef",
     "ImageTypeDef",
     "UpdateApplicationResultTypeDef",
     "AppBlockTypeDef",
     "CreateAppBlockRequestRequestTypeDef",
     "BatchAssociateUserStackResultTypeDef",
@@ -194,20 +220,20 @@
     "UpdateDirectoryConfigResultTypeDef",
     "CreateEntitlementResultTypeDef",
     "DescribeEntitlementsResultTypeDef",
     "UpdateEntitlementResultTypeDef",
     "CreateFleetResultTypeDef",
     "DescribeFleetsResultTypeDef",
     "UpdateFleetResultTypeDef",
-    "DescribeSessionsResultTypeDef",
     "CreateImageBuilderResultTypeDef",
     "DeleteImageBuilderResultTypeDef",
     "DescribeImageBuildersResultTypeDef",
     "StartImageBuilderResultTypeDef",
     "StopImageBuilderResultTypeDef",
+    "DescribeSessionsResultTypeDef",
     "DescribeImagePermissionsResultTypeDef",
     "DescribeUsageReportSubscriptionsResultTypeDef",
     "CreateStackResultTypeDef",
     "DescribeStacksResultTypeDef",
     "UpdateStackResultTypeDef",
     "CreateUpdatedImageResultTypeDef",
     "DeleteImageResultTypeDef",
@@ -231,22 +257,78 @@
 )
 
 
 class AccessEndpointTypeDef(_RequiredAccessEndpointTypeDef, _OptionalAccessEndpointTypeDef):
     pass
 
 
-S3LocationTypeDef = TypedDict(
-    "S3LocationTypeDef",
+AppBlockBuilderAppBlockAssociationTypeDef = TypedDict(
+    "AppBlockBuilderAppBlockAssociationTypeDef",
+    {
+        "AppBlockArn": str,
+        "AppBlockBuilderName": str,
+    },
+)
+
+AppBlockBuilderStateChangeReasonTypeDef = TypedDict(
+    "AppBlockBuilderStateChangeReasonTypeDef",
+    {
+        "Code": Literal["INTERNAL_ERROR"],
+        "Message": str,
+    },
+    total=False,
+)
+
+ResourceErrorTypeDef = TypedDict(
+    "ResourceErrorTypeDef",
+    {
+        "ErrorCode": FleetErrorCodeType,
+        "ErrorMessage": str,
+        "ErrorTimestamp": datetime,
+    },
+    total=False,
+)
+
+VpcConfigTypeDef = TypedDict(
+    "VpcConfigTypeDef",
+    {
+        "SubnetIds": Sequence[str],
+        "SecurityGroupIds": Sequence[str],
+    },
+    total=False,
+)
+
+ErrorDetailsTypeDef = TypedDict(
+    "ErrorDetailsTypeDef",
+    {
+        "ErrorCode": str,
+        "ErrorMessage": str,
+    },
+    total=False,
+)
+
+_RequiredS3LocationTypeDef = TypedDict(
+    "_RequiredS3LocationTypeDef",
     {
         "S3Bucket": str,
+    },
+)
+_OptionalS3LocationTypeDef = TypedDict(
+    "_OptionalS3LocationTypeDef",
+    {
         "S3Key": str,
     },
+    total=False,
 )
 
+
+class S3LocationTypeDef(_RequiredS3LocationTypeDef, _OptionalS3LocationTypeDef):
+    pass
+
+
 ApplicationFleetAssociationTypeDef = TypedDict(
     "ApplicationFleetAssociationTypeDef",
     {
         "FleetName": str,
         "ApplicationArn": str,
     },
 )
@@ -278,33 +360,41 @@
 
 class ApplicationSettingsTypeDef(
     _RequiredApplicationSettingsTypeDef, _OptionalApplicationSettingsTypeDef
 ):
     pass
 
 
-AssociateApplicationFleetRequestRequestTypeDef = TypedDict(
-    "AssociateApplicationFleetRequestRequestTypeDef",
+AssociateAppBlockBuilderAppBlockRequestRequestTypeDef = TypedDict(
+    "AssociateAppBlockBuilderAppBlockRequestRequestTypeDef",
     {
-        "FleetName": str,
-        "ApplicationArn": str,
+        "AppBlockArn": str,
+        "AppBlockBuilderName": str,
     },
 )
 
 ResponseMetadataTypeDef = TypedDict(
     "ResponseMetadataTypeDef",
     {
         "RequestId": str,
         "HostId": str,
         "HTTPStatusCode": int,
         "HTTPHeaders": Dict[str, str],
         "RetryAttempts": int,
     },
 )
 
+AssociateApplicationFleetRequestRequestTypeDef = TypedDict(
+    "AssociateApplicationFleetRequestRequestTypeDef",
+    {
+        "FleetName": str,
+        "ApplicationArn": str,
+    },
+)
+
 AssociateApplicationToEntitlementRequestRequestTypeDef = TypedDict(
     "AssociateApplicationToEntitlementRequestRequestTypeDef",
     {
         "StackName": str,
         "EntitlementName": str,
         "ApplicationIdentifier": str,
     },
@@ -399,14 +489,36 @@
 
 class CopyImageRequestRequestTypeDef(
     _RequiredCopyImageRequestRequestTypeDef, _OptionalCopyImageRequestRequestTypeDef
 ):
     pass
 
 
+_RequiredCreateAppBlockBuilderStreamingURLRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateAppBlockBuilderStreamingURLRequestRequestTypeDef",
+    {
+        "AppBlockBuilderName": str,
+    },
+)
+_OptionalCreateAppBlockBuilderStreamingURLRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateAppBlockBuilderStreamingURLRequestRequestTypeDef",
+    {
+        "Validity": int,
+    },
+    total=False,
+)
+
+
+class CreateAppBlockBuilderStreamingURLRequestRequestTypeDef(
+    _RequiredCreateAppBlockBuilderStreamingURLRequestRequestTypeDef,
+    _OptionalCreateAppBlockBuilderStreamingURLRequestRequestTypeDef,
+):
+    pass
+
+
 ServiceAccountCredentialsTypeDef = TypedDict(
     "ServiceAccountCredentialsTypeDef",
     {
         "AccountName": str,
         "AccountPassword": str,
     },
 )
@@ -424,23 +536,14 @@
     {
         "DirectoryName": str,
         "OrganizationalUnitDistinguishedName": str,
     },
     total=False,
 )
 
-VpcConfigTypeDef = TypedDict(
-    "VpcConfigTypeDef",
-    {
-        "SubnetIds": Sequence[str],
-        "SecurityGroupIds": Sequence[str],
-    },
-    total=False,
-)
-
 _RequiredCreateImageBuilderStreamingURLRequestRequestTypeDef = TypedDict(
     "_RequiredCreateImageBuilderStreamingURLRequestRequestTypeDef",
     {
         "Name": str,
     },
 )
 _OptionalCreateImageBuilderStreamingURLRequestRequestTypeDef = TypedDict(
@@ -567,14 +670,21 @@
 
 class CreateUserRequestRequestTypeDef(
     _RequiredCreateUserRequestRequestTypeDef, _OptionalCreateUserRequestRequestTypeDef
 ):
     pass
 
 
+DeleteAppBlockBuilderRequestRequestTypeDef = TypedDict(
+    "DeleteAppBlockBuilderRequestRequestTypeDef",
+    {
+        "Name": str,
+    },
+)
+
 DeleteAppBlockRequestRequestTypeDef = TypedDict(
     "DeleteAppBlockRequestRequestTypeDef",
     {
         "Name": str,
     },
 )
 
@@ -640,14 +750,35 @@
     "DeleteUserRequestRequestTypeDef",
     {
         "UserName": str,
         "AuthenticationType": AuthenticationTypeType,
     },
 )
 
+DescribeAppBlockBuilderAppBlockAssociationsRequestRequestTypeDef = TypedDict(
+    "DescribeAppBlockBuilderAppBlockAssociationsRequestRequestTypeDef",
+    {
+        "AppBlockArn": str,
+        "AppBlockBuilderName": str,
+        "MaxResults": int,
+        "NextToken": str,
+    },
+    total=False,
+)
+
+DescribeAppBlockBuildersRequestRequestTypeDef = TypedDict(
+    "DescribeAppBlockBuildersRequestRequestTypeDef",
+    {
+        "Names": Sequence[str],
+        "NextToken": str,
+        "MaxResults": int,
+    },
+    total=False,
+)
+
 DescribeAppBlocksRequestRequestTypeDef = TypedDict(
     "DescribeAppBlocksRequestRequestTypeDef",
     {
         "Arns": Sequence[str],
         "NextToken": str,
         "MaxResults": int,
     },
@@ -889,14 +1020,22 @@
     "DisableUserRequestRequestTypeDef",
     {
         "UserName": str,
         "AuthenticationType": AuthenticationTypeType,
     },
 )
 
+DisassociateAppBlockBuilderAppBlockRequestRequestTypeDef = TypedDict(
+    "DisassociateAppBlockBuilderAppBlockRequestRequestTypeDef",
+    {
+        "AppBlockArn": str,
+        "AppBlockBuilderName": str,
+    },
+)
+
 DisassociateApplicationFleetRequestRequestTypeDef = TypedDict(
     "DisassociateApplicationFleetRequestRequestTypeDef",
     {
         "FleetName": str,
         "ApplicationArn": str,
     },
 )
@@ -963,24 +1102,14 @@
     {
         "EniPrivateIpAddress": str,
         "EniId": str,
     },
     total=False,
 )
 
-ResourceErrorTypeDef = TypedDict(
-    "ResourceErrorTypeDef",
-    {
-        "ErrorCode": FleetErrorCodeType,
-        "ErrorMessage": str,
-        "ErrorTimestamp": datetime,
-    },
-    total=False,
-)
-
 ImagePermissionsTypeDef = TypedDict(
     "ImagePermissionsTypeDef",
     {
         "allowFleet": bool,
         "allowImageBuilder": bool,
     },
     total=False,
@@ -1084,14 +1213,21 @@
     {
         "ErrorCode": StackErrorCodeType,
         "ErrorMessage": str,
     },
     total=False,
 )
 
+StartAppBlockBuilderRequestRequestTypeDef = TypedDict(
+    "StartAppBlockBuilderRequestRequestTypeDef",
+    {
+        "Name": str,
+    },
+)
+
 StartFleetRequestRequestTypeDef = TypedDict(
     "StartFleetRequestRequestTypeDef",
     {
         "Name": str,
     },
 )
 
@@ -1112,14 +1248,21 @@
 
 class StartImageBuilderRequestRequestTypeDef(
     _RequiredStartImageBuilderRequestRequestTypeDef, _OptionalStartImageBuilderRequestRequestTypeDef
 ):
     pass
 
 
+StopAppBlockBuilderRequestRequestTypeDef = TypedDict(
+    "StopAppBlockBuilderRequestRequestTypeDef",
+    {
+        "Name": str,
+    },
+)
+
 StopFleetRequestRequestTypeDef = TypedDict(
     "StopFleetRequestRequestTypeDef",
     {
         "Name": str,
     },
 )
 
@@ -1142,14 +1285,105 @@
     "UntagResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
         "TagKeys": Sequence[str],
     },
 )
 
+_RequiredAppBlockBuilderTypeDef = TypedDict(
+    "_RequiredAppBlockBuilderTypeDef",
+    {
+        "Arn": str,
+        "Name": str,
+        "Platform": Literal["WINDOWS_SERVER_2019"],
+        "InstanceType": str,
+        "VpcConfig": VpcConfigTypeDef,
+        "State": AppBlockBuilderStateType,
+    },
+)
+_OptionalAppBlockBuilderTypeDef = TypedDict(
+    "_OptionalAppBlockBuilderTypeDef",
+    {
+        "DisplayName": str,
+        "Description": str,
+        "EnableDefaultInternetAccess": bool,
+        "IamRoleArn": str,
+        "CreatedTime": datetime,
+        "AppBlockBuilderErrors": List[ResourceErrorTypeDef],
+        "StateChangeReason": AppBlockBuilderStateChangeReasonTypeDef,
+        "AccessEndpoints": List[AccessEndpointTypeDef],
+    },
+    total=False,
+)
+
+
+class AppBlockBuilderTypeDef(_RequiredAppBlockBuilderTypeDef, _OptionalAppBlockBuilderTypeDef):
+    pass
+
+
+_RequiredCreateAppBlockBuilderRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateAppBlockBuilderRequestRequestTypeDef",
+    {
+        "Name": str,
+        "Platform": Literal["WINDOWS_SERVER_2019"],
+        "InstanceType": str,
+        "VpcConfig": VpcConfigTypeDef,
+    },
+)
+_OptionalCreateAppBlockBuilderRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateAppBlockBuilderRequestRequestTypeDef",
+    {
+        "Description": str,
+        "DisplayName": str,
+        "Tags": Mapping[str, str],
+        "EnableDefaultInternetAccess": bool,
+        "IamRoleArn": str,
+        "AccessEndpoints": Sequence[AccessEndpointTypeDef],
+    },
+    total=False,
+)
+
+
+class CreateAppBlockBuilderRequestRequestTypeDef(
+    _RequiredCreateAppBlockBuilderRequestRequestTypeDef,
+    _OptionalCreateAppBlockBuilderRequestRequestTypeDef,
+):
+    pass
+
+
+_RequiredUpdateAppBlockBuilderRequestRequestTypeDef = TypedDict(
+    "_RequiredUpdateAppBlockBuilderRequestRequestTypeDef",
+    {
+        "Name": str,
+    },
+)
+_OptionalUpdateAppBlockBuilderRequestRequestTypeDef = TypedDict(
+    "_OptionalUpdateAppBlockBuilderRequestRequestTypeDef",
+    {
+        "Description": str,
+        "DisplayName": str,
+        "Platform": PlatformTypeType,
+        "InstanceType": str,
+        "VpcConfig": VpcConfigTypeDef,
+        "EnableDefaultInternetAccess": bool,
+        "IamRoleArn": str,
+        "AccessEndpoints": Sequence[AccessEndpointTypeDef],
+        "AttributesToDelete": Sequence[AppBlockBuilderAttributeType],
+    },
+    total=False,
+)
+
+
+class UpdateAppBlockBuilderRequestRequestTypeDef(
+    _RequiredUpdateAppBlockBuilderRequestRequestTypeDef,
+    _OptionalUpdateAppBlockBuilderRequestRequestTypeDef,
+):
+    pass
+
+
 ApplicationTypeDef = TypedDict(
     "ApplicationTypeDef",
     {
         "Name": str,
         "DisplayName": str,
         "IconURL": str,
         "LaunchPath": str,
@@ -1243,14 +1477,22 @@
 
 class UpdateApplicationRequestRequestTypeDef(
     _RequiredUpdateApplicationRequestRequestTypeDef, _OptionalUpdateApplicationRequestRequestTypeDef
 ):
     pass
 
 
+AssociateAppBlockBuilderAppBlockResultTypeDef = TypedDict(
+    "AssociateAppBlockBuilderAppBlockResultTypeDef",
+    {
+        "AppBlockBuilderAppBlockAssociation": AppBlockBuilderAppBlockAssociationTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 AssociateApplicationFleetResultTypeDef = TypedDict(
     "AssociateApplicationFleetResultTypeDef",
     {
         "ApplicationFleetAssociation": ApplicationFleetAssociationTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -1259,14 +1501,23 @@
     "CopyImageResponseTypeDef",
     {
         "DestinationImageName": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+CreateAppBlockBuilderStreamingURLResultTypeDef = TypedDict(
+    "CreateAppBlockBuilderStreamingURLResultTypeDef",
+    {
+        "StreamingURL": str,
+        "Expires": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 CreateImageBuilderStreamingURLResultTypeDef = TypedDict(
     "CreateImageBuilderStreamingURLResultTypeDef",
     {
         "StreamingURL": str,
         "Expires": datetime,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -1286,14 +1537,23 @@
     {
         "S3BucketName": str,
         "Schedule": Literal["DAILY"],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+DescribeAppBlockBuilderAppBlockAssociationsResultTypeDef = TypedDict(
+    "DescribeAppBlockBuilderAppBlockAssociationsResultTypeDef",
+    {
+        "AppBlockBuilderAppBlockAssociations": List[AppBlockBuilderAppBlockAssociationTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 DescribeApplicationFleetAssociationsResultTypeDef = TypedDict(
     "DescribeApplicationFleetAssociationsResultTypeDef",
     {
         "ApplicationFleetAssociations": List[ApplicationFleetAssociationTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -1888,41 +2148,14 @@
 )
 
 
 class FleetTypeDef(_RequiredFleetTypeDef, _OptionalFleetTypeDef):
     pass
 
 
-_RequiredSessionTypeDef = TypedDict(
-    "_RequiredSessionTypeDef",
-    {
-        "Id": str,
-        "UserId": str,
-        "StackName": str,
-        "FleetName": str,
-        "State": SessionStateType,
-    },
-)
-_OptionalSessionTypeDef = TypedDict(
-    "_OptionalSessionTypeDef",
-    {
-        "ConnectionState": SessionConnectionStateType,
-        "StartTime": datetime,
-        "MaxExpirationTime": datetime,
-        "AuthenticationType": AuthenticationTypeType,
-        "NetworkAccessConfiguration": NetworkAccessConfigurationTypeDef,
-    },
-    total=False,
-)
-
-
-class SessionTypeDef(_RequiredSessionTypeDef, _OptionalSessionTypeDef):
-    pass
-
-
 _RequiredImageBuilderTypeDef = TypedDict(
     "_RequiredImageBuilderTypeDef",
     {
         "Name": str,
     },
 )
 _OptionalImageBuilderTypeDef = TypedDict(
@@ -1950,14 +2183,41 @@
 )
 
 
 class ImageBuilderTypeDef(_RequiredImageBuilderTypeDef, _OptionalImageBuilderTypeDef):
     pass
 
 
+_RequiredSessionTypeDef = TypedDict(
+    "_RequiredSessionTypeDef",
+    {
+        "Id": str,
+        "UserId": str,
+        "StackName": str,
+        "FleetName": str,
+        "State": SessionStateType,
+    },
+)
+_OptionalSessionTypeDef = TypedDict(
+    "_OptionalSessionTypeDef",
+    {
+        "ConnectionState": SessionConnectionStateType,
+        "StartTime": datetime,
+        "MaxExpirationTime": datetime,
+        "AuthenticationType": AuthenticationTypeType,
+        "NetworkAccessConfiguration": NetworkAccessConfigurationTypeDef,
+    },
+    total=False,
+)
+
+
+class SessionTypeDef(_RequiredSessionTypeDef, _OptionalSessionTypeDef):
+    pass
+
+
 SharedImagePermissionsTypeDef = TypedDict(
     "SharedImagePermissionsTypeDef",
     {
         "sharedAccountId": str,
         "imagePermissions": ImagePermissionsTypeDef,
     },
 )
@@ -2009,14 +2269,55 @@
 )
 
 
 class StackTypeDef(_RequiredStackTypeDef, _OptionalStackTypeDef):
     pass
 
 
+CreateAppBlockBuilderResultTypeDef = TypedDict(
+    "CreateAppBlockBuilderResultTypeDef",
+    {
+        "AppBlockBuilder": AppBlockBuilderTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeAppBlockBuildersResultTypeDef = TypedDict(
+    "DescribeAppBlockBuildersResultTypeDef",
+    {
+        "AppBlockBuilders": List[AppBlockBuilderTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+StartAppBlockBuilderResultTypeDef = TypedDict(
+    "StartAppBlockBuilderResultTypeDef",
+    {
+        "AppBlockBuilder": AppBlockBuilderTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+StopAppBlockBuilderResultTypeDef = TypedDict(
+    "StopAppBlockBuilderResultTypeDef",
+    {
+        "AppBlockBuilder": AppBlockBuilderTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateAppBlockBuilderResultTypeDef = TypedDict(
+    "UpdateAppBlockBuilderResultTypeDef",
+    {
+        "AppBlockBuilder": AppBlockBuilderTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 CreateApplicationResultTypeDef = TypedDict(
     "CreateApplicationResultTypeDef",
     {
         "Application": ApplicationTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -2073,47 +2374,53 @@
 )
 
 _RequiredAppBlockTypeDef = TypedDict(
     "_RequiredAppBlockTypeDef",
     {
         "Name": str,
         "Arn": str,
-        "SetupScriptDetails": ScriptDetailsTypeDef,
     },
 )
 _OptionalAppBlockTypeDef = TypedDict(
     "_OptionalAppBlockTypeDef",
     {
         "Description": str,
         "DisplayName": str,
         "SourceS3Location": S3LocationTypeDef,
+        "SetupScriptDetails": ScriptDetailsTypeDef,
         "CreatedTime": datetime,
+        "PostSetupScriptDetails": ScriptDetailsTypeDef,
+        "PackagingType": PackagingTypeType,
+        "State": AppBlockStateType,
+        "AppBlockErrors": List[ErrorDetailsTypeDef],
     },
     total=False,
 )
 
 
 class AppBlockTypeDef(_RequiredAppBlockTypeDef, _OptionalAppBlockTypeDef):
     pass
 
 
 _RequiredCreateAppBlockRequestRequestTypeDef = TypedDict(
     "_RequiredCreateAppBlockRequestRequestTypeDef",
     {
         "Name": str,
         "SourceS3Location": S3LocationTypeDef,
-        "SetupScriptDetails": ScriptDetailsTypeDef,
     },
 )
 _OptionalCreateAppBlockRequestRequestTypeDef = TypedDict(
     "_OptionalCreateAppBlockRequestRequestTypeDef",
     {
         "Description": str,
         "DisplayName": str,
+        "SetupScriptDetails": ScriptDetailsTypeDef,
         "Tags": Mapping[str, str],
+        "PostSetupScriptDetails": ScriptDetailsTypeDef,
+        "PackagingType": PackagingTypeType,
     },
     total=False,
 )
 
 
 class CreateAppBlockRequestRequestTypeDef(
     _RequiredCreateAppBlockRequestRequestTypeDef, _OptionalCreateAppBlockRequestRequestTypeDef
@@ -2208,23 +2515,14 @@
     "UpdateFleetResultTypeDef",
     {
         "Fleet": FleetTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-DescribeSessionsResultTypeDef = TypedDict(
-    "DescribeSessionsResultTypeDef",
-    {
-        "Sessions": List[SessionTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 CreateImageBuilderResultTypeDef = TypedDict(
     "CreateImageBuilderResultTypeDef",
     {
         "ImageBuilder": ImageBuilderTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -2258,14 +2556,23 @@
     "StopImageBuilderResultTypeDef",
     {
         "ImageBuilder": ImageBuilderTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+DescribeSessionsResultTypeDef = TypedDict(
+    "DescribeSessionsResultTypeDef",
+    {
+        "Sessions": List[SessionTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 DescribeImagePermissionsResultTypeDef = TypedDict(
     "DescribeImagePermissionsResultTypeDef",
     {
         "Name": str,
         "SharedImagePermissionsList": List[SharedImagePermissionsTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
```

### Comparing `types-aiobotocore-appstream-2.5.2.post3/types_aiobotocore_appstream/type_defs.pyi` & `types-aiobotocore-appstream-2.5.4/types_aiobotocore_appstream/type_defs.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -13,27 +13,31 @@
 """
 import sys
 from datetime import datetime
 from typing import Dict, List, Mapping, Sequence
 
 from .literals import (
     ActionType,
+    AppBlockBuilderAttributeType,
+    AppBlockBuilderStateType,
+    AppBlockStateType,
     ApplicationAttributeType,
     AppVisibilityType,
     AuthenticationTypeType,
     CertificateBasedAuthStatusType,
     FleetAttributeType,
     FleetErrorCodeType,
     FleetStateType,
     FleetTypeType,
     ImageBuilderStateChangeReasonCodeType,
     ImageBuilderStateType,
     ImageStateChangeReasonCodeType,
     ImageStateType,
     MessageActionType,
+    PackagingTypeType,
     PermissionType,
     PlatformTypeType,
     PreferredProtocolType,
     SessionConnectionStateType,
     SessionStateType,
     StackAttributeType,
     StackErrorCodeType,
@@ -51,48 +55,57 @@
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
     "AccessEndpointTypeDef",
+    "AppBlockBuilderAppBlockAssociationTypeDef",
+    "AppBlockBuilderStateChangeReasonTypeDef",
+    "ResourceErrorTypeDef",
+    "VpcConfigTypeDef",
+    "ErrorDetailsTypeDef",
     "S3LocationTypeDef",
     "ApplicationFleetAssociationTypeDef",
     "ApplicationSettingsResponseTypeDef",
     "ApplicationSettingsTypeDef",
-    "AssociateApplicationFleetRequestRequestTypeDef",
+    "AssociateAppBlockBuilderAppBlockRequestRequestTypeDef",
     "ResponseMetadataTypeDef",
+    "AssociateApplicationFleetRequestRequestTypeDef",
     "AssociateApplicationToEntitlementRequestRequestTypeDef",
     "AssociateFleetRequestRequestTypeDef",
     "UserStackAssociationTypeDef",
     "CertificateBasedAuthPropertiesTypeDef",
     "ComputeCapacityStatusTypeDef",
     "ComputeCapacityTypeDef",
     "CopyImageRequestRequestTypeDef",
+    "CreateAppBlockBuilderStreamingURLRequestRequestTypeDef",
     "ServiceAccountCredentialsTypeDef",
     "EntitlementAttributeTypeDef",
     "DomainJoinInfoTypeDef",
-    "VpcConfigTypeDef",
     "CreateImageBuilderStreamingURLRequestRequestTypeDef",
     "StorageConnectorTypeDef",
     "StreamingExperienceSettingsTypeDef",
     "UserSettingTypeDef",
     "CreateStreamingURLRequestRequestTypeDef",
     "CreateUpdatedImageRequestRequestTypeDef",
     "CreateUserRequestRequestTypeDef",
+    "DeleteAppBlockBuilderRequestRequestTypeDef",
     "DeleteAppBlockRequestRequestTypeDef",
     "DeleteApplicationRequestRequestTypeDef",
     "DeleteDirectoryConfigRequestRequestTypeDef",
     "DeleteEntitlementRequestRequestTypeDef",
     "DeleteFleetRequestRequestTypeDef",
     "DeleteImageBuilderRequestRequestTypeDef",
     "DeleteImagePermissionsRequestRequestTypeDef",
     "DeleteImageRequestRequestTypeDef",
     "DeleteStackRequestRequestTypeDef",
     "DeleteUserRequestRequestTypeDef",
+    "DescribeAppBlockBuilderAppBlockAssociationsRequestRequestTypeDef",
+    "DescribeAppBlockBuildersRequestRequestTypeDef",
     "DescribeAppBlocksRequestRequestTypeDef",
     "DescribeApplicationFleetAssociationsRequestRequestTypeDef",
     "DescribeApplicationsRequestRequestTypeDef",
     "PaginatorConfigTypeDef",
     "DescribeDirectoryConfigsRequestRequestTypeDef",
     "DescribeEntitlementsRequestRequestTypeDef",
     "WaiterConfigTypeDef",
@@ -103,47 +116,55 @@
     "DescribeSessionsRequestRequestTypeDef",
     "DescribeStacksRequestRequestTypeDef",
     "DescribeUsageReportSubscriptionsRequestRequestTypeDef",
     "DescribeUserStackAssociationsRequestRequestTypeDef",
     "DescribeUsersRequestRequestTypeDef",
     "UserTypeDef",
     "DisableUserRequestRequestTypeDef",
+    "DisassociateAppBlockBuilderAppBlockRequestRequestTypeDef",
     "DisassociateApplicationFleetRequestRequestTypeDef",
     "DisassociateApplicationFromEntitlementRequestRequestTypeDef",
     "DisassociateFleetRequestRequestTypeDef",
     "EnableUserRequestRequestTypeDef",
     "EntitledApplicationTypeDef",
     "ExpireSessionRequestRequestTypeDef",
     "FleetErrorTypeDef",
     "ImageBuilderStateChangeReasonTypeDef",
     "NetworkAccessConfigurationTypeDef",
-    "ResourceErrorTypeDef",
     "ImagePermissionsTypeDef",
     "ImageStateChangeReasonTypeDef",
     "LastReportGenerationExecutionErrorTypeDef",
     "ListAssociatedFleetsRequestRequestTypeDef",
     "ListAssociatedStacksRequestRequestTypeDef",
     "ListEntitledApplicationsRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
     "StackErrorTypeDef",
+    "StartAppBlockBuilderRequestRequestTypeDef",
     "StartFleetRequestRequestTypeDef",
     "StartImageBuilderRequestRequestTypeDef",
+    "StopAppBlockBuilderRequestRequestTypeDef",
     "StopFleetRequestRequestTypeDef",
     "StopImageBuilderRequestRequestTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
+    "AppBlockBuilderTypeDef",
+    "CreateAppBlockBuilderRequestRequestTypeDef",
+    "UpdateAppBlockBuilderRequestRequestTypeDef",
     "ApplicationTypeDef",
     "CreateApplicationRequestRequestTypeDef",
     "ScriptDetailsTypeDef",
     "UpdateApplicationRequestRequestTypeDef",
+    "AssociateAppBlockBuilderAppBlockResultTypeDef",
     "AssociateApplicationFleetResultTypeDef",
     "CopyImageResponseTypeDef",
+    "CreateAppBlockBuilderStreamingURLResultTypeDef",
     "CreateImageBuilderStreamingURLResultTypeDef",
     "CreateStreamingURLResultTypeDef",
     "CreateUsageReportSubscriptionResultTypeDef",
+    "DescribeAppBlockBuilderAppBlockAssociationsResultTypeDef",
     "DescribeApplicationFleetAssociationsResultTypeDef",
     "ListAssociatedFleetsResultTypeDef",
     "ListAssociatedStacksResultTypeDef",
     "ListTagsForResourceResponseTypeDef",
     "BatchAssociateUserStackRequestRequestTypeDef",
     "BatchDisassociateUserStackRequestRequestTypeDef",
     "DescribeUserStackAssociationsResultTypeDef",
@@ -170,20 +191,25 @@
     "ListAssociatedFleetsRequestListAssociatedFleetsPaginateTypeDef",
     "ListAssociatedStacksRequestListAssociatedStacksPaginateTypeDef",
     "DescribeFleetsRequestFleetStartedWaitTypeDef",
     "DescribeFleetsRequestFleetStoppedWaitTypeDef",
     "DescribeUsersResultTypeDef",
     "ListEntitledApplicationsResultTypeDef",
     "FleetTypeDef",
-    "SessionTypeDef",
     "ImageBuilderTypeDef",
+    "SessionTypeDef",
     "SharedImagePermissionsTypeDef",
     "UpdateImagePermissionsRequestRequestTypeDef",
     "UsageReportSubscriptionTypeDef",
     "StackTypeDef",
+    "CreateAppBlockBuilderResultTypeDef",
+    "DescribeAppBlockBuildersResultTypeDef",
+    "StartAppBlockBuilderResultTypeDef",
+    "StopAppBlockBuilderResultTypeDef",
+    "UpdateAppBlockBuilderResultTypeDef",
     "CreateApplicationResultTypeDef",
     "DescribeApplicationsResultTypeDef",
     "ImageTypeDef",
     "UpdateApplicationResultTypeDef",
     "AppBlockTypeDef",
     "CreateAppBlockRequestRequestTypeDef",
     "BatchAssociateUserStackResultTypeDef",
@@ -193,20 +219,20 @@
     "UpdateDirectoryConfigResultTypeDef",
     "CreateEntitlementResultTypeDef",
     "DescribeEntitlementsResultTypeDef",
     "UpdateEntitlementResultTypeDef",
     "CreateFleetResultTypeDef",
     "DescribeFleetsResultTypeDef",
     "UpdateFleetResultTypeDef",
-    "DescribeSessionsResultTypeDef",
     "CreateImageBuilderResultTypeDef",
     "DeleteImageBuilderResultTypeDef",
     "DescribeImageBuildersResultTypeDef",
     "StartImageBuilderResultTypeDef",
     "StopImageBuilderResultTypeDef",
+    "DescribeSessionsResultTypeDef",
     "DescribeImagePermissionsResultTypeDef",
     "DescribeUsageReportSubscriptionsResultTypeDef",
     "CreateStackResultTypeDef",
     "DescribeStacksResultTypeDef",
     "UpdateStackResultTypeDef",
     "CreateUpdatedImageResultTypeDef",
     "DeleteImageResultTypeDef",
@@ -228,22 +254,76 @@
     },
     total=False,
 )
 
 class AccessEndpointTypeDef(_RequiredAccessEndpointTypeDef, _OptionalAccessEndpointTypeDef):
     pass
 
-S3LocationTypeDef = TypedDict(
-    "S3LocationTypeDef",
+AppBlockBuilderAppBlockAssociationTypeDef = TypedDict(
+    "AppBlockBuilderAppBlockAssociationTypeDef",
+    {
+        "AppBlockArn": str,
+        "AppBlockBuilderName": str,
+    },
+)
+
+AppBlockBuilderStateChangeReasonTypeDef = TypedDict(
+    "AppBlockBuilderStateChangeReasonTypeDef",
+    {
+        "Code": Literal["INTERNAL_ERROR"],
+        "Message": str,
+    },
+    total=False,
+)
+
+ResourceErrorTypeDef = TypedDict(
+    "ResourceErrorTypeDef",
+    {
+        "ErrorCode": FleetErrorCodeType,
+        "ErrorMessage": str,
+        "ErrorTimestamp": datetime,
+    },
+    total=False,
+)
+
+VpcConfigTypeDef = TypedDict(
+    "VpcConfigTypeDef",
+    {
+        "SubnetIds": Sequence[str],
+        "SecurityGroupIds": Sequence[str],
+    },
+    total=False,
+)
+
+ErrorDetailsTypeDef = TypedDict(
+    "ErrorDetailsTypeDef",
+    {
+        "ErrorCode": str,
+        "ErrorMessage": str,
+    },
+    total=False,
+)
+
+_RequiredS3LocationTypeDef = TypedDict(
+    "_RequiredS3LocationTypeDef",
     {
         "S3Bucket": str,
+    },
+)
+_OptionalS3LocationTypeDef = TypedDict(
+    "_OptionalS3LocationTypeDef",
+    {
         "S3Key": str,
     },
+    total=False,
 )
 
+class S3LocationTypeDef(_RequiredS3LocationTypeDef, _OptionalS3LocationTypeDef):
+    pass
+
 ApplicationFleetAssociationTypeDef = TypedDict(
     "ApplicationFleetAssociationTypeDef",
     {
         "FleetName": str,
         "ApplicationArn": str,
     },
 )
@@ -273,33 +353,41 @@
 )
 
 class ApplicationSettingsTypeDef(
     _RequiredApplicationSettingsTypeDef, _OptionalApplicationSettingsTypeDef
 ):
     pass
 
-AssociateApplicationFleetRequestRequestTypeDef = TypedDict(
-    "AssociateApplicationFleetRequestRequestTypeDef",
+AssociateAppBlockBuilderAppBlockRequestRequestTypeDef = TypedDict(
+    "AssociateAppBlockBuilderAppBlockRequestRequestTypeDef",
     {
-        "FleetName": str,
-        "ApplicationArn": str,
+        "AppBlockArn": str,
+        "AppBlockBuilderName": str,
     },
 )
 
 ResponseMetadataTypeDef = TypedDict(
     "ResponseMetadataTypeDef",
     {
         "RequestId": str,
         "HostId": str,
         "HTTPStatusCode": int,
         "HTTPHeaders": Dict[str, str],
         "RetryAttempts": int,
     },
 )
 
+AssociateApplicationFleetRequestRequestTypeDef = TypedDict(
+    "AssociateApplicationFleetRequestRequestTypeDef",
+    {
+        "FleetName": str,
+        "ApplicationArn": str,
+    },
+)
+
 AssociateApplicationToEntitlementRequestRequestTypeDef = TypedDict(
     "AssociateApplicationToEntitlementRequestRequestTypeDef",
     {
         "StackName": str,
         "EntitlementName": str,
         "ApplicationIdentifier": str,
     },
@@ -388,14 +476,34 @@
 )
 
 class CopyImageRequestRequestTypeDef(
     _RequiredCopyImageRequestRequestTypeDef, _OptionalCopyImageRequestRequestTypeDef
 ):
     pass
 
+_RequiredCreateAppBlockBuilderStreamingURLRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateAppBlockBuilderStreamingURLRequestRequestTypeDef",
+    {
+        "AppBlockBuilderName": str,
+    },
+)
+_OptionalCreateAppBlockBuilderStreamingURLRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateAppBlockBuilderStreamingURLRequestRequestTypeDef",
+    {
+        "Validity": int,
+    },
+    total=False,
+)
+
+class CreateAppBlockBuilderStreamingURLRequestRequestTypeDef(
+    _RequiredCreateAppBlockBuilderStreamingURLRequestRequestTypeDef,
+    _OptionalCreateAppBlockBuilderStreamingURLRequestRequestTypeDef,
+):
+    pass
+
 ServiceAccountCredentialsTypeDef = TypedDict(
     "ServiceAccountCredentialsTypeDef",
     {
         "AccountName": str,
         "AccountPassword": str,
     },
 )
@@ -413,23 +521,14 @@
     {
         "DirectoryName": str,
         "OrganizationalUnitDistinguishedName": str,
     },
     total=False,
 )
 
-VpcConfigTypeDef = TypedDict(
-    "VpcConfigTypeDef",
-    {
-        "SubnetIds": Sequence[str],
-        "SecurityGroupIds": Sequence[str],
-    },
-    total=False,
-)
-
 _RequiredCreateImageBuilderStreamingURLRequestRequestTypeDef = TypedDict(
     "_RequiredCreateImageBuilderStreamingURLRequestRequestTypeDef",
     {
         "Name": str,
     },
 )
 _OptionalCreateImageBuilderStreamingURLRequestRequestTypeDef = TypedDict(
@@ -546,14 +645,21 @@
 )
 
 class CreateUserRequestRequestTypeDef(
     _RequiredCreateUserRequestRequestTypeDef, _OptionalCreateUserRequestRequestTypeDef
 ):
     pass
 
+DeleteAppBlockBuilderRequestRequestTypeDef = TypedDict(
+    "DeleteAppBlockBuilderRequestRequestTypeDef",
+    {
+        "Name": str,
+    },
+)
+
 DeleteAppBlockRequestRequestTypeDef = TypedDict(
     "DeleteAppBlockRequestRequestTypeDef",
     {
         "Name": str,
     },
 )
 
@@ -619,14 +725,35 @@
     "DeleteUserRequestRequestTypeDef",
     {
         "UserName": str,
         "AuthenticationType": AuthenticationTypeType,
     },
 )
 
+DescribeAppBlockBuilderAppBlockAssociationsRequestRequestTypeDef = TypedDict(
+    "DescribeAppBlockBuilderAppBlockAssociationsRequestRequestTypeDef",
+    {
+        "AppBlockArn": str,
+        "AppBlockBuilderName": str,
+        "MaxResults": int,
+        "NextToken": str,
+    },
+    total=False,
+)
+
+DescribeAppBlockBuildersRequestRequestTypeDef = TypedDict(
+    "DescribeAppBlockBuildersRequestRequestTypeDef",
+    {
+        "Names": Sequence[str],
+        "NextToken": str,
+        "MaxResults": int,
+    },
+    total=False,
+)
+
 DescribeAppBlocksRequestRequestTypeDef = TypedDict(
     "DescribeAppBlocksRequestRequestTypeDef",
     {
         "Arns": Sequence[str],
         "NextToken": str,
         "MaxResults": int,
     },
@@ -858,14 +985,22 @@
     "DisableUserRequestRequestTypeDef",
     {
         "UserName": str,
         "AuthenticationType": AuthenticationTypeType,
     },
 )
 
+DisassociateAppBlockBuilderAppBlockRequestRequestTypeDef = TypedDict(
+    "DisassociateAppBlockBuilderAppBlockRequestRequestTypeDef",
+    {
+        "AppBlockArn": str,
+        "AppBlockBuilderName": str,
+    },
+)
+
 DisassociateApplicationFleetRequestRequestTypeDef = TypedDict(
     "DisassociateApplicationFleetRequestRequestTypeDef",
     {
         "FleetName": str,
         "ApplicationArn": str,
     },
 )
@@ -932,24 +1067,14 @@
     {
         "EniPrivateIpAddress": str,
         "EniId": str,
     },
     total=False,
 )
 
-ResourceErrorTypeDef = TypedDict(
-    "ResourceErrorTypeDef",
-    {
-        "ErrorCode": FleetErrorCodeType,
-        "ErrorMessage": str,
-        "ErrorTimestamp": datetime,
-    },
-    total=False,
-)
-
 ImagePermissionsTypeDef = TypedDict(
     "ImagePermissionsTypeDef",
     {
         "allowFleet": bool,
         "allowImageBuilder": bool,
     },
     total=False,
@@ -1047,14 +1172,21 @@
     {
         "ErrorCode": StackErrorCodeType,
         "ErrorMessage": str,
     },
     total=False,
 )
 
+StartAppBlockBuilderRequestRequestTypeDef = TypedDict(
+    "StartAppBlockBuilderRequestRequestTypeDef",
+    {
+        "Name": str,
+    },
+)
+
 StartFleetRequestRequestTypeDef = TypedDict(
     "StartFleetRequestRequestTypeDef",
     {
         "Name": str,
     },
 )
 
@@ -1073,14 +1205,21 @@
 )
 
 class StartImageBuilderRequestRequestTypeDef(
     _RequiredStartImageBuilderRequestRequestTypeDef, _OptionalStartImageBuilderRequestRequestTypeDef
 ):
     pass
 
+StopAppBlockBuilderRequestRequestTypeDef = TypedDict(
+    "StopAppBlockBuilderRequestRequestTypeDef",
+    {
+        "Name": str,
+    },
+)
+
 StopFleetRequestRequestTypeDef = TypedDict(
     "StopFleetRequestRequestTypeDef",
     {
         "Name": str,
     },
 )
 
@@ -1103,14 +1242,99 @@
     "UntagResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
         "TagKeys": Sequence[str],
     },
 )
 
+_RequiredAppBlockBuilderTypeDef = TypedDict(
+    "_RequiredAppBlockBuilderTypeDef",
+    {
+        "Arn": str,
+        "Name": str,
+        "Platform": Literal["WINDOWS_SERVER_2019"],
+        "InstanceType": str,
+        "VpcConfig": VpcConfigTypeDef,
+        "State": AppBlockBuilderStateType,
+    },
+)
+_OptionalAppBlockBuilderTypeDef = TypedDict(
+    "_OptionalAppBlockBuilderTypeDef",
+    {
+        "DisplayName": str,
+        "Description": str,
+        "EnableDefaultInternetAccess": bool,
+        "IamRoleArn": str,
+        "CreatedTime": datetime,
+        "AppBlockBuilderErrors": List[ResourceErrorTypeDef],
+        "StateChangeReason": AppBlockBuilderStateChangeReasonTypeDef,
+        "AccessEndpoints": List[AccessEndpointTypeDef],
+    },
+    total=False,
+)
+
+class AppBlockBuilderTypeDef(_RequiredAppBlockBuilderTypeDef, _OptionalAppBlockBuilderTypeDef):
+    pass
+
+_RequiredCreateAppBlockBuilderRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateAppBlockBuilderRequestRequestTypeDef",
+    {
+        "Name": str,
+        "Platform": Literal["WINDOWS_SERVER_2019"],
+        "InstanceType": str,
+        "VpcConfig": VpcConfigTypeDef,
+    },
+)
+_OptionalCreateAppBlockBuilderRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateAppBlockBuilderRequestRequestTypeDef",
+    {
+        "Description": str,
+        "DisplayName": str,
+        "Tags": Mapping[str, str],
+        "EnableDefaultInternetAccess": bool,
+        "IamRoleArn": str,
+        "AccessEndpoints": Sequence[AccessEndpointTypeDef],
+    },
+    total=False,
+)
+
+class CreateAppBlockBuilderRequestRequestTypeDef(
+    _RequiredCreateAppBlockBuilderRequestRequestTypeDef,
+    _OptionalCreateAppBlockBuilderRequestRequestTypeDef,
+):
+    pass
+
+_RequiredUpdateAppBlockBuilderRequestRequestTypeDef = TypedDict(
+    "_RequiredUpdateAppBlockBuilderRequestRequestTypeDef",
+    {
+        "Name": str,
+    },
+)
+_OptionalUpdateAppBlockBuilderRequestRequestTypeDef = TypedDict(
+    "_OptionalUpdateAppBlockBuilderRequestRequestTypeDef",
+    {
+        "Description": str,
+        "DisplayName": str,
+        "Platform": PlatformTypeType,
+        "InstanceType": str,
+        "VpcConfig": VpcConfigTypeDef,
+        "EnableDefaultInternetAccess": bool,
+        "IamRoleArn": str,
+        "AccessEndpoints": Sequence[AccessEndpointTypeDef],
+        "AttributesToDelete": Sequence[AppBlockBuilderAttributeType],
+    },
+    total=False,
+)
+
+class UpdateAppBlockBuilderRequestRequestTypeDef(
+    _RequiredUpdateAppBlockBuilderRequestRequestTypeDef,
+    _OptionalUpdateAppBlockBuilderRequestRequestTypeDef,
+):
+    pass
+
 ApplicationTypeDef = TypedDict(
     "ApplicationTypeDef",
     {
         "Name": str,
         "DisplayName": str,
         "IconURL": str,
         "LaunchPath": str,
@@ -1198,14 +1422,22 @@
 )
 
 class UpdateApplicationRequestRequestTypeDef(
     _RequiredUpdateApplicationRequestRequestTypeDef, _OptionalUpdateApplicationRequestRequestTypeDef
 ):
     pass
 
+AssociateAppBlockBuilderAppBlockResultTypeDef = TypedDict(
+    "AssociateAppBlockBuilderAppBlockResultTypeDef",
+    {
+        "AppBlockBuilderAppBlockAssociation": AppBlockBuilderAppBlockAssociationTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 AssociateApplicationFleetResultTypeDef = TypedDict(
     "AssociateApplicationFleetResultTypeDef",
     {
         "ApplicationFleetAssociation": ApplicationFleetAssociationTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -1214,14 +1446,23 @@
     "CopyImageResponseTypeDef",
     {
         "DestinationImageName": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+CreateAppBlockBuilderStreamingURLResultTypeDef = TypedDict(
+    "CreateAppBlockBuilderStreamingURLResultTypeDef",
+    {
+        "StreamingURL": str,
+        "Expires": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 CreateImageBuilderStreamingURLResultTypeDef = TypedDict(
     "CreateImageBuilderStreamingURLResultTypeDef",
     {
         "StreamingURL": str,
         "Expires": datetime,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -1241,14 +1482,23 @@
     {
         "S3BucketName": str,
         "Schedule": Literal["DAILY"],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+DescribeAppBlockBuilderAppBlockAssociationsResultTypeDef = TypedDict(
+    "DescribeAppBlockBuilderAppBlockAssociationsResultTypeDef",
+    {
+        "AppBlockBuilderAppBlockAssociations": List[AppBlockBuilderAppBlockAssociationTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 DescribeApplicationFleetAssociationsResultTypeDef = TypedDict(
     "DescribeApplicationFleetAssociationsResultTypeDef",
     {
         "ApplicationFleetAssociations": List[ApplicationFleetAssociationTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -1813,39 +2063,14 @@
     },
     total=False,
 )
 
 class FleetTypeDef(_RequiredFleetTypeDef, _OptionalFleetTypeDef):
     pass
 
-_RequiredSessionTypeDef = TypedDict(
-    "_RequiredSessionTypeDef",
-    {
-        "Id": str,
-        "UserId": str,
-        "StackName": str,
-        "FleetName": str,
-        "State": SessionStateType,
-    },
-)
-_OptionalSessionTypeDef = TypedDict(
-    "_OptionalSessionTypeDef",
-    {
-        "ConnectionState": SessionConnectionStateType,
-        "StartTime": datetime,
-        "MaxExpirationTime": datetime,
-        "AuthenticationType": AuthenticationTypeType,
-        "NetworkAccessConfiguration": NetworkAccessConfigurationTypeDef,
-    },
-    total=False,
-)
-
-class SessionTypeDef(_RequiredSessionTypeDef, _OptionalSessionTypeDef):
-    pass
-
 _RequiredImageBuilderTypeDef = TypedDict(
     "_RequiredImageBuilderTypeDef",
     {
         "Name": str,
     },
 )
 _OptionalImageBuilderTypeDef = TypedDict(
@@ -1871,14 +2096,39 @@
     },
     total=False,
 )
 
 class ImageBuilderTypeDef(_RequiredImageBuilderTypeDef, _OptionalImageBuilderTypeDef):
     pass
 
+_RequiredSessionTypeDef = TypedDict(
+    "_RequiredSessionTypeDef",
+    {
+        "Id": str,
+        "UserId": str,
+        "StackName": str,
+        "FleetName": str,
+        "State": SessionStateType,
+    },
+)
+_OptionalSessionTypeDef = TypedDict(
+    "_OptionalSessionTypeDef",
+    {
+        "ConnectionState": SessionConnectionStateType,
+        "StartTime": datetime,
+        "MaxExpirationTime": datetime,
+        "AuthenticationType": AuthenticationTypeType,
+        "NetworkAccessConfiguration": NetworkAccessConfigurationTypeDef,
+    },
+    total=False,
+)
+
+class SessionTypeDef(_RequiredSessionTypeDef, _OptionalSessionTypeDef):
+    pass
+
 SharedImagePermissionsTypeDef = TypedDict(
     "SharedImagePermissionsTypeDef",
     {
         "sharedAccountId": str,
         "imagePermissions": ImagePermissionsTypeDef,
     },
 )
@@ -1928,14 +2178,55 @@
     },
     total=False,
 )
 
 class StackTypeDef(_RequiredStackTypeDef, _OptionalStackTypeDef):
     pass
 
+CreateAppBlockBuilderResultTypeDef = TypedDict(
+    "CreateAppBlockBuilderResultTypeDef",
+    {
+        "AppBlockBuilder": AppBlockBuilderTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeAppBlockBuildersResultTypeDef = TypedDict(
+    "DescribeAppBlockBuildersResultTypeDef",
+    {
+        "AppBlockBuilders": List[AppBlockBuilderTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+StartAppBlockBuilderResultTypeDef = TypedDict(
+    "StartAppBlockBuilderResultTypeDef",
+    {
+        "AppBlockBuilder": AppBlockBuilderTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+StopAppBlockBuilderResultTypeDef = TypedDict(
+    "StopAppBlockBuilderResultTypeDef",
+    {
+        "AppBlockBuilder": AppBlockBuilderTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateAppBlockBuilderResultTypeDef = TypedDict(
+    "UpdateAppBlockBuilderResultTypeDef",
+    {
+        "AppBlockBuilder": AppBlockBuilderTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 CreateApplicationResultTypeDef = TypedDict(
     "CreateApplicationResultTypeDef",
     {
         "Application": ApplicationTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -1990,45 +2281,51 @@
 )
 
 _RequiredAppBlockTypeDef = TypedDict(
     "_RequiredAppBlockTypeDef",
     {
         "Name": str,
         "Arn": str,
-        "SetupScriptDetails": ScriptDetailsTypeDef,
     },
 )
 _OptionalAppBlockTypeDef = TypedDict(
     "_OptionalAppBlockTypeDef",
     {
         "Description": str,
         "DisplayName": str,
         "SourceS3Location": S3LocationTypeDef,
+        "SetupScriptDetails": ScriptDetailsTypeDef,
         "CreatedTime": datetime,
+        "PostSetupScriptDetails": ScriptDetailsTypeDef,
+        "PackagingType": PackagingTypeType,
+        "State": AppBlockStateType,
+        "AppBlockErrors": List[ErrorDetailsTypeDef],
     },
     total=False,
 )
 
 class AppBlockTypeDef(_RequiredAppBlockTypeDef, _OptionalAppBlockTypeDef):
     pass
 
 _RequiredCreateAppBlockRequestRequestTypeDef = TypedDict(
     "_RequiredCreateAppBlockRequestRequestTypeDef",
     {
         "Name": str,
         "SourceS3Location": S3LocationTypeDef,
-        "SetupScriptDetails": ScriptDetailsTypeDef,
     },
 )
 _OptionalCreateAppBlockRequestRequestTypeDef = TypedDict(
     "_OptionalCreateAppBlockRequestRequestTypeDef",
     {
         "Description": str,
         "DisplayName": str,
+        "SetupScriptDetails": ScriptDetailsTypeDef,
         "Tags": Mapping[str, str],
+        "PostSetupScriptDetails": ScriptDetailsTypeDef,
+        "PackagingType": PackagingTypeType,
     },
     total=False,
 )
 
 class CreateAppBlockRequestRequestTypeDef(
     _RequiredCreateAppBlockRequestRequestTypeDef, _OptionalCreateAppBlockRequestRequestTypeDef
 ):
@@ -2121,23 +2418,14 @@
     "UpdateFleetResultTypeDef",
     {
         "Fleet": FleetTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-DescribeSessionsResultTypeDef = TypedDict(
-    "DescribeSessionsResultTypeDef",
-    {
-        "Sessions": List[SessionTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 CreateImageBuilderResultTypeDef = TypedDict(
     "CreateImageBuilderResultTypeDef",
     {
         "ImageBuilder": ImageBuilderTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -2171,14 +2459,23 @@
     "StopImageBuilderResultTypeDef",
     {
         "ImageBuilder": ImageBuilderTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+DescribeSessionsResultTypeDef = TypedDict(
+    "DescribeSessionsResultTypeDef",
+    {
+        "Sessions": List[SessionTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 DescribeImagePermissionsResultTypeDef = TypedDict(
     "DescribeImagePermissionsResultTypeDef",
     {
         "Name": str,
         "SharedImagePermissionsList": List[SharedImagePermissionsTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
```

### Comparing `types-aiobotocore-appstream-2.5.2.post3/types_aiobotocore_appstream/waiter.py` & `types-aiobotocore-appstream-2.5.4/types_aiobotocore_appstream/waiter.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-appstream-2.5.2.post3/types_aiobotocore_appstream/waiter.pyi` & `types-aiobotocore-appstream-2.5.4/types_aiobotocore_appstream/waiter.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-appstream-2.5.2.post3/types_aiobotocore_appstream.egg-info/PKG-INFO` & `types-aiobotocore-appstream-2.5.4/types_aiobotocore_appstream.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-appstream
-Version: 2.5.2.post3
-Summary: Type annotations for aiobotocore.AppStream 2.5.2 service generated with mypy-boto3-builder 7.17.2
+Version: 2.5.4
+Summary: Type annotations for aiobotocore.AppStream 2.5.4 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appstream/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-appstream.svg?color=blue)](https://pypi.org/project/types-aiobotocore-appstream)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appstream/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-appstream)](https://pepy.tech/project/types-aiobotocore-appstream)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.AppStream 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appstream.html#AppStream)
+[aiobotocore.AppStream 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appstream.html#AppStream)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-appstream-2.5.2.post3/types_aiobotocore_appstream.egg-info/SOURCES.txt` & `types-aiobotocore-appstream-2.5.4/types_aiobotocore_appstream.egg-info/SOURCES.txt`

 * *Files identical despite different names*


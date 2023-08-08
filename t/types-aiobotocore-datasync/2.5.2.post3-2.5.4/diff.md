# Comparing `tmp/types-aiobotocore-datasync-2.5.2.post3.tar.gz` & `tmp/types-aiobotocore-datasync-2.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-datasync-2.5.2.post3.tar", last modified: Fri Aug  4 12:37:34 2023, max compression
+gzip compressed data, was "types-aiobotocore-datasync-2.5.4.tar", last modified: Tue Aug  8 01:23:35 2023, max compression
```

## Comparing `types-aiobotocore-datasync-2.5.2.post3.tar` & `types-aiobotocore-datasync-2.5.4.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:37:34.235588 types-aiobotocore-datasync-2.5.2.post3/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-04 12:21:14.000000 types-aiobotocore-datasync-2.5.2.post3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    14035 2023-08-04 12:37:34.235588 types-aiobotocore-datasync-2.5.2.post3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    12513 2023-08-04 12:21:14.000000 types-aiobotocore-datasync-2.5.2.post3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-04 12:37:34.235588 types-aiobotocore-datasync-2.5.2.post3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2079 2023-08-04 12:21:14.000000 types-aiobotocore-datasync-2.5.2.post3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:37:34.227588 types-aiobotocore-datasync-2.5.2.post3/types_aiobotocore_datasync/
--rw-r--r--   0 runner    (1001) docker     (123)     2193 2023-08-04 12:21:14.000000 types-aiobotocore-datasync-2.5.2.post3/types_aiobotocore_datasync/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2192 2023-08-04 12:21:14.000000 types-aiobotocore-datasync-2.5.2.post3/types_aiobotocore_datasync/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      947 2023-08-04 12:21:14.000000 types-aiobotocore-datasync-2.5.2.post3/types_aiobotocore_datasync/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    47714 2023-08-04 12:21:15.000000 types-aiobotocore-datasync-2.5.2.post3/types_aiobotocore_datasync/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    47640 2023-08-04 12:21:14.000000 types-aiobotocore-datasync-2.5.2.post3/types_aiobotocore_datasync/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    12834 2023-08-04 12:21:15.000000 types-aiobotocore-datasync-2.5.2.post3/types_aiobotocore_datasync/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    12832 2023-08-04 12:21:15.000000 types-aiobotocore-datasync-2.5.2.post3/types_aiobotocore_datasync/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    10352 2023-08-04 12:21:15.000000 types-aiobotocore-datasync-2.5.2.post3/types_aiobotocore_datasync/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)    10342 2023-08-04 12:21:15.000000 types-aiobotocore-datasync-2.5.2.post3/types_aiobotocore_datasync/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 12:21:14.000000 types-aiobotocore-datasync-2.5.2.post3/types_aiobotocore_datasync/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    55303 2023-08-04 12:21:17.000000 types-aiobotocore-datasync-2.5.2.post3/types_aiobotocore_datasync/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    55242 2023-08-04 12:21:16.000000 types-aiobotocore-datasync-2.5.2.post3/types_aiobotocore_datasync/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-04 12:21:14.000000 types-aiobotocore-datasync-2.5.2.post3/types_aiobotocore_datasync/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:37:34.235588 types-aiobotocore-datasync-2.5.2.post3/types_aiobotocore_datasync.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    14035 2023-08-04 12:37:34.000000 types-aiobotocore-datasync-2.5.2.post3/types_aiobotocore_datasync.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      832 2023-08-04 12:37:34.000000 types-aiobotocore-datasync-2.5.2.post3/types_aiobotocore_datasync.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 12:37:34.000000 types-aiobotocore-datasync-2.5.2.post3/types_aiobotocore_datasync.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 12:37:34.000000 types-aiobotocore-datasync-2.5.2.post3/types_aiobotocore_datasync.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-04 12:37:34.000000 types-aiobotocore-datasync-2.5.2.post3/types_aiobotocore_datasync.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-08-04 12:37:34.000000 types-aiobotocore-datasync-2.5.2.post3/types_aiobotocore_datasync.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:23:35.262680 types-aiobotocore-datasync-2.5.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-08 01:08:50.000000 types-aiobotocore-datasync-2.5.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    14029 2023-08-08 01:23:35.262680 types-aiobotocore-datasync-2.5.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    12513 2023-08-08 01:08:50.000000 types-aiobotocore-datasync-2.5.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-08 01:23:35.262680 types-aiobotocore-datasync-2.5.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2073 2023-08-08 01:08:50.000000 types-aiobotocore-datasync-2.5.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:23:35.258680 types-aiobotocore-datasync-2.5.4/types_aiobotocore_datasync/
+-rw-r--r--   0 runner    (1001) docker     (123)     2193 2023-08-08 01:08:50.000000 types-aiobotocore-datasync-2.5.4/types_aiobotocore_datasync/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2192 2023-08-08 01:08:50.000000 types-aiobotocore-datasync-2.5.4/types_aiobotocore_datasync/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      935 2023-08-08 01:08:50.000000 types-aiobotocore-datasync-2.5.4/types_aiobotocore_datasync/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    50346 2023-08-08 01:08:50.000000 types-aiobotocore-datasync-2.5.4/types_aiobotocore_datasync/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    50269 2023-08-08 01:08:50.000000 types-aiobotocore-datasync-2.5.4/types_aiobotocore_datasync/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    13162 2023-08-08 01:08:51.000000 types-aiobotocore-datasync-2.5.4/types_aiobotocore_datasync/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13160 2023-08-08 01:08:51.000000 types-aiobotocore-datasync-2.5.4/types_aiobotocore_datasync/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    10352 2023-08-08 01:08:51.000000 types-aiobotocore-datasync-2.5.4/types_aiobotocore_datasync/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10342 2023-08-08 01:08:51.000000 types-aiobotocore-datasync-2.5.4/types_aiobotocore_datasync/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 01:08:50.000000 types-aiobotocore-datasync-2.5.4/types_aiobotocore_datasync/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    58182 2023-08-08 01:08:53.000000 types-aiobotocore-datasync-2.5.4/types_aiobotocore_datasync/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    58117 2023-08-08 01:08:52.000000 types-aiobotocore-datasync-2.5.4/types_aiobotocore_datasync/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-08-08 01:08:50.000000 types-aiobotocore-datasync-2.5.4/types_aiobotocore_datasync/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:23:35.262680 types-aiobotocore-datasync-2.5.4/types_aiobotocore_datasync.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    14029 2023-08-08 01:23:35.000000 types-aiobotocore-datasync-2.5.4/types_aiobotocore_datasync.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      832 2023-08-08 01:23:35.000000 types-aiobotocore-datasync-2.5.4/types_aiobotocore_datasync.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 01:23:35.000000 types-aiobotocore-datasync-2.5.4/types_aiobotocore_datasync.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 01:23:35.000000 types-aiobotocore-datasync-2.5.4/types_aiobotocore_datasync.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-08 01:23:35.000000 types-aiobotocore-datasync-2.5.4/types_aiobotocore_datasync.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-08-08 01:23:35.000000 types-aiobotocore-datasync-2.5.4/types_aiobotocore_datasync.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-datasync-2.5.2.post3/LICENSE` & `types-aiobotocore-datasync-2.5.4/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-datasync-2.5.2.post3/PKG-INFO` & `types-aiobotocore-datasync-2.5.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-datasync
-Version: 2.5.2.post3
-Summary: Type annotations for aiobotocore.DataSync 2.5.2 service generated with mypy-boto3-builder 7.17.2
+Version: 2.5.4
+Summary: Type annotations for aiobotocore.DataSync 2.5.4 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_datasync/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-datasync.svg?color=blue)](https://pypi.org/project/types-aiobotocore-datasync)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_datasync/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-datasync)](https://pepy.tech/project/types-aiobotocore-datasync)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.DataSync 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync.html#DataSync)
+[aiobotocore.DataSync 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync.html#DataSync)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-datasync-2.5.2.post3/README.md` & `types-aiobotocore-datasync-2.5.4/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-datasync.svg?color=blue)](https://pypi.org/project/types-aiobotocore-datasync)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_datasync/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-datasync)](https://pepy.tech/project/types-aiobotocore-datasync)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.DataSync 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync.html#DataSync)
+[aiobotocore.DataSync 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync.html#DataSync)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-datasync-2.5.2.post3/setup.py` & `types-aiobotocore-datasync-2.5.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-datasync",
-    version="2.5.2.post3",
+    version="2.5.4",
     packages=["types_aiobotocore_datasync"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.DataSync 2.5.2 service generated with mypy-boto3-builder"
+        "Type annotations for aiobotocore.DataSync 2.5.4 service generated with mypy-boto3-builder"
         " 7.17.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
```

### Comparing `types-aiobotocore-datasync-2.5.2.post3/types_aiobotocore_datasync/__init__.py` & `types-aiobotocore-datasync-2.5.4/types_aiobotocore_datasync/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-datasync-2.5.2.post3/types_aiobotocore_datasync/__init__.pyi` & `types-aiobotocore-datasync-2.5.4/types_aiobotocore_datasync/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-datasync-2.5.2.post3/types_aiobotocore_datasync/__main__.py` & `types-aiobotocore-datasync-2.5.4/types_aiobotocore_datasync/__main__.py`

 * *Files 26% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.DataSync 2.5.2\nVersion:         2.5.2.post3\nBuilder"
-        " version: 7.17.2\nDocs:           "
+        "Type annotations for aiobotocore.DataSync 2.5.4\nVersion:         2.5.4\nBuilder version:"
+        " 7.17.2\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_datasync//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync.html#DataSync\nOther"
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

### Comparing `types-aiobotocore-datasync-2.5.2.post3/types_aiobotocore_datasync/client.py` & `types-aiobotocore-datasync-2.5.4/types_aiobotocore_datasync/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,14 +17,15 @@
 import sys
 from typing import Any, Dict, Mapping, Sequence, Type, overload
 
 from aiobotocore.client import AioBaseClient
 from botocore.client import ClientMeta
 
 from .literals import (
+    AzureAccessTierType,
     DiscoveryResourceTypeType,
     EfsInTransitEncryptionType,
     HdfsAuthenticationTypeType,
     ObjectStorageServerProtocolType,
     S3StorageClassType,
 )
 from .paginator import (
@@ -35,30 +36,33 @@
     ListStorageSystemsPaginator,
     ListTagsForResourcePaginator,
     ListTaskExecutionsPaginator,
     ListTasksPaginator,
 )
 from .type_defs import (
     AddStorageSystemResponseTypeDef,
+    AzureBlobSasConfigurationTypeDef,
     BlobTypeDef,
     CreateAgentResponseTypeDef,
+    CreateLocationAzureBlobResponseTypeDef,
     CreateLocationEfsResponseTypeDef,
     CreateLocationFsxLustreResponseTypeDef,
     CreateLocationFsxOntapResponseTypeDef,
     CreateLocationFsxOpenZfsResponseTypeDef,
     CreateLocationFsxWindowsResponseTypeDef,
     CreateLocationHdfsResponseTypeDef,
     CreateLocationNfsResponseTypeDef,
     CreateLocationObjectStorageResponseTypeDef,
     CreateLocationS3ResponseTypeDef,
     CreateLocationSmbResponseTypeDef,
     CreateTaskResponseTypeDef,
     CredentialsTypeDef,
     DescribeAgentResponseTypeDef,
     DescribeDiscoveryJobResponseTypeDef,
+    DescribeLocationAzureBlobResponseTypeDef,
     DescribeLocationEfsResponseTypeDef,
     DescribeLocationFsxLustreResponseTypeDef,
     DescribeLocationFsxOntapResponseTypeDef,
     DescribeLocationFsxOpenZfsResponseTypeDef,
     DescribeLocationFsxWindowsResponseTypeDef,
     DescribeLocationHdfsResponseTypeDef,
     DescribeLocationNfsResponseTypeDef,
@@ -188,20 +192,40 @@
         AgentName: str = ...,
         Tags: Sequence[TagListEntryTypeDef] = ...,
         VpcEndpointId: str = ...,
         SubnetArns: Sequence[str] = ...,
         SecurityGroupArns: Sequence[str] = ...
     ) -> CreateAgentResponseTypeDef:
         """
-        Activates an DataSync agent that you have deployed in your storage environment.
+        Activates an DataSync agent that you've deployed in your storage environment.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync.html#DataSync.Client.create_agent)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_datasync/client/#create_agent)
         """
 
+    async def create_location_azure_blob(
+        self,
+        *,
+        ContainerUrl: str,
+        AuthenticationType: Literal["SAS"],
+        AgentArns: Sequence[str],
+        SasConfiguration: AzureBlobSasConfigurationTypeDef = ...,
+        BlobType: Literal["BLOCK"] = ...,
+        AccessTier: AzureAccessTierType = ...,
+        Subdirectory: str = ...,
+        Tags: Sequence[TagListEntryTypeDef] = ...
+    ) -> CreateLocationAzureBlobResponseTypeDef:
+        """
+        Creates an endpoint for a Microsoft Azure Blob Storage container that DataSync
+        can use as a transfer source or destination.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync.html#DataSync.Client.create_location_azure_blob)
+        [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_datasync/client/#create_location_azure_blob)
+        """
+
     async def create_location_efs(
         self,
         *,
         EfsFilesystemArn: str,
         Ec2Config: Ec2ConfigTypeDef,
         Subdirectory: str = ...,
         Tags: Sequence[TagListEntryTypeDef] = ...,
@@ -314,16 +338,16 @@
         Subdirectory: str,
         ServerHostname: str,
         OnPremConfig: OnPremConfigTypeDef,
         MountOptions: NfsMountOptionsTypeDef = ...,
         Tags: Sequence[TagListEntryTypeDef] = ...
     ) -> CreateLocationNfsResponseTypeDef:
         """
-        Defines a file system on a Network File System (NFS) server that can be read
-        from or written to.
+        Creates an endpoint for an Network File System (NFS) file server that DataSync
+        can use for a data transfer.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync.html#DataSync.Client.create_location_nfs)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_datasync/client/#create_location_nfs)
         """
 
     async def create_location_object_storage(
         self,
@@ -374,15 +398,15 @@
         AgentArns: Sequence[str],
         Domain: str = ...,
         MountOptions: SmbMountOptionsTypeDef = ...,
         Tags: Sequence[TagListEntryTypeDef] = ...
     ) -> CreateLocationSmbResponseTypeDef:
         """
         Creates an endpoint for a Server Message Block (SMB) file server that DataSync
-        can access for a transfer.
+        can use for a data transfer.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync.html#DataSync.Client.create_location_smb)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_datasync/client/#create_location_smb)
         """
 
     async def create_task(
         self,
@@ -443,14 +467,25 @@
         """
         Returns information about a DataSync discovery job.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync.html#DataSync.Client.describe_discovery_job)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_datasync/client/#describe_discovery_job)
         """
 
+    async def describe_location_azure_blob(
+        self, *, LocationArn: str
+    ) -> DescribeLocationAzureBlobResponseTypeDef:
+        """
+        Provides details about how an DataSync transfer location for Microsoft Azure
+        Blob Storage is configured.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync.html#DataSync.Client.describe_location_azure_blob)
+        [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_datasync/client/#describe_location_azure_blob)
+        """
+
     async def describe_location_efs(
         self, *, LocationArn: str
     ) -> DescribeLocationEfsResponseTypeDef:
         """
         Returns metadata about your DataSync location for an Amazon EFS file system.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync.html#DataSync.Client.describe_location_efs)
@@ -597,25 +632,25 @@
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync.html#DataSync.Client.describe_storage_system_resources)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_datasync/client/#describe_storage_system_resources)
         """
 
     async def describe_task(self, *, TaskArn: str) -> DescribeTaskResponseTypeDef:
         """
-        Returns metadata about a task.
+        Provides information about an DataSync transfer task.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync.html#DataSync.Client.describe_task)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_datasync/client/#describe_task)
         """
 
     async def describe_task_execution(
         self, *, TaskExecutionArn: str
     ) -> DescribeTaskExecutionResponseTypeDef:
         """
-        Returns detailed metadata about a task that is being executed.
+        Provides information about an DataSync transfer task that's running.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync.html#DataSync.Client.describe_task_execution)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_datasync/client/#describe_task_execution)
         """
 
     async def generate_presigned_url(
         self,
@@ -806,14 +841,33 @@
         """
         Edits a DataSync discovery job configuration.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync.html#DataSync.Client.update_discovery_job)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_datasync/client/#update_discovery_job)
         """
 
+    async def update_location_azure_blob(
+        self,
+        *,
+        LocationArn: str,
+        Subdirectory: str = ...,
+        AuthenticationType: Literal["SAS"] = ...,
+        SasConfiguration: AzureBlobSasConfigurationTypeDef = ...,
+        BlobType: Literal["BLOCK"] = ...,
+        AccessTier: AzureAccessTierType = ...,
+        AgentArns: Sequence[str] = ...
+    ) -> Dict[str, Any]:
+        """
+        Modifies some configurations of the Microsoft Azure Blob Storage transfer
+        location that you're using with DataSync.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync.html#DataSync.Client.update_location_azure_blob)
+        [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_datasync/client/#update_location_azure_blob)
+        """
+
     async def update_location_hdfs(
         self,
         *,
         LocationArn: str,
         Subdirectory: str = ...,
         NameNodes: Sequence[HdfsNameNodeTypeDef] = ...,
         BlockSize: int = ...,
```

### Comparing `types-aiobotocore-datasync-2.5.2.post3/types_aiobotocore_datasync/client.pyi` & `types-aiobotocore-datasync-2.5.4/types_aiobotocore_datasync/client.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -17,14 +17,15 @@
 import sys
 from typing import Any, Dict, Mapping, Sequence, Type, overload
 
 from aiobotocore.client import AioBaseClient
 from botocore.client import ClientMeta
 
 from .literals import (
+    AzureAccessTierType,
     DiscoveryResourceTypeType,
     EfsInTransitEncryptionType,
     HdfsAuthenticationTypeType,
     ObjectStorageServerProtocolType,
     S3StorageClassType,
 )
 from .paginator import (
@@ -35,30 +36,33 @@
     ListStorageSystemsPaginator,
     ListTagsForResourcePaginator,
     ListTaskExecutionsPaginator,
     ListTasksPaginator,
 )
 from .type_defs import (
     AddStorageSystemResponseTypeDef,
+    AzureBlobSasConfigurationTypeDef,
     BlobTypeDef,
     CreateAgentResponseTypeDef,
+    CreateLocationAzureBlobResponseTypeDef,
     CreateLocationEfsResponseTypeDef,
     CreateLocationFsxLustreResponseTypeDef,
     CreateLocationFsxOntapResponseTypeDef,
     CreateLocationFsxOpenZfsResponseTypeDef,
     CreateLocationFsxWindowsResponseTypeDef,
     CreateLocationHdfsResponseTypeDef,
     CreateLocationNfsResponseTypeDef,
     CreateLocationObjectStorageResponseTypeDef,
     CreateLocationS3ResponseTypeDef,
     CreateLocationSmbResponseTypeDef,
     CreateTaskResponseTypeDef,
     CredentialsTypeDef,
     DescribeAgentResponseTypeDef,
     DescribeDiscoveryJobResponseTypeDef,
+    DescribeLocationAzureBlobResponseTypeDef,
     DescribeLocationEfsResponseTypeDef,
     DescribeLocationFsxLustreResponseTypeDef,
     DescribeLocationFsxOntapResponseTypeDef,
     DescribeLocationFsxOpenZfsResponseTypeDef,
     DescribeLocationFsxWindowsResponseTypeDef,
     DescribeLocationHdfsResponseTypeDef,
     DescribeLocationNfsResponseTypeDef,
@@ -179,19 +183,38 @@
         AgentName: str = ...,
         Tags: Sequence[TagListEntryTypeDef] = ...,
         VpcEndpointId: str = ...,
         SubnetArns: Sequence[str] = ...,
         SecurityGroupArns: Sequence[str] = ...
     ) -> CreateAgentResponseTypeDef:
         """
-        Activates an DataSync agent that you have deployed in your storage environment.
+        Activates an DataSync agent that you've deployed in your storage environment.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync.html#DataSync.Client.create_agent)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_datasync/client/#create_agent)
         """
+    async def create_location_azure_blob(
+        self,
+        *,
+        ContainerUrl: str,
+        AuthenticationType: Literal["SAS"],
+        AgentArns: Sequence[str],
+        SasConfiguration: AzureBlobSasConfigurationTypeDef = ...,
+        BlobType: Literal["BLOCK"] = ...,
+        AccessTier: AzureAccessTierType = ...,
+        Subdirectory: str = ...,
+        Tags: Sequence[TagListEntryTypeDef] = ...
+    ) -> CreateLocationAzureBlobResponseTypeDef:
+        """
+        Creates an endpoint for a Microsoft Azure Blob Storage container that DataSync
+        can use as a transfer source or destination.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync.html#DataSync.Client.create_location_azure_blob)
+        [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_datasync/client/#create_location_azure_blob)
+        """
     async def create_location_efs(
         self,
         *,
         EfsFilesystemArn: str,
         Ec2Config: Ec2ConfigTypeDef,
         Subdirectory: str = ...,
         Tags: Sequence[TagListEntryTypeDef] = ...,
@@ -298,16 +321,16 @@
         Subdirectory: str,
         ServerHostname: str,
         OnPremConfig: OnPremConfigTypeDef,
         MountOptions: NfsMountOptionsTypeDef = ...,
         Tags: Sequence[TagListEntryTypeDef] = ...
     ) -> CreateLocationNfsResponseTypeDef:
         """
-        Defines a file system on a Network File System (NFS) server that can be read
-        from or written to.
+        Creates an endpoint for an Network File System (NFS) file server that DataSync
+        can use for a data transfer.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync.html#DataSync.Client.create_location_nfs)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_datasync/client/#create_location_nfs)
         """
     async def create_location_object_storage(
         self,
         *,
@@ -355,15 +378,15 @@
         AgentArns: Sequence[str],
         Domain: str = ...,
         MountOptions: SmbMountOptionsTypeDef = ...,
         Tags: Sequence[TagListEntryTypeDef] = ...
     ) -> CreateLocationSmbResponseTypeDef:
         """
         Creates an endpoint for a Server Message Block (SMB) file server that DataSync
-        can access for a transfer.
+        can use for a data transfer.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync.html#DataSync.Client.create_location_smb)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_datasync/client/#create_location_smb)
         """
     async def create_task(
         self,
         *,
@@ -417,14 +440,24 @@
     ) -> DescribeDiscoveryJobResponseTypeDef:
         """
         Returns information about a DataSync discovery job.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync.html#DataSync.Client.describe_discovery_job)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_datasync/client/#describe_discovery_job)
         """
+    async def describe_location_azure_blob(
+        self, *, LocationArn: str
+    ) -> DescribeLocationAzureBlobResponseTypeDef:
+        """
+        Provides details about how an DataSync transfer location for Microsoft Azure
+        Blob Storage is configured.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync.html#DataSync.Client.describe_location_azure_blob)
+        [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_datasync/client/#describe_location_azure_blob)
+        """
     async def describe_location_efs(
         self, *, LocationArn: str
     ) -> DescribeLocationEfsResponseTypeDef:
         """
         Returns metadata about your DataSync location for an Amazon EFS file system.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync.html#DataSync.Client.describe_location_efs)
@@ -558,24 +591,24 @@
         premises storage system.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync.html#DataSync.Client.describe_storage_system_resources)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_datasync/client/#describe_storage_system_resources)
         """
     async def describe_task(self, *, TaskArn: str) -> DescribeTaskResponseTypeDef:
         """
-        Returns metadata about a task.
+        Provides information about an DataSync transfer task.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync.html#DataSync.Client.describe_task)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_datasync/client/#describe_task)
         """
     async def describe_task_execution(
         self, *, TaskExecutionArn: str
     ) -> DescribeTaskExecutionResponseTypeDef:
         """
-        Returns detailed metadata about a task that is being executed.
+        Provides information about an DataSync transfer task that's running.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync.html#DataSync.Client.describe_task_execution)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_datasync/client/#describe_task_execution)
         """
     async def generate_presigned_url(
         self,
         ClientMethod: str,
@@ -748,14 +781,32 @@
     ) -> Dict[str, Any]:
         """
         Edits a DataSync discovery job configuration.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync.html#DataSync.Client.update_discovery_job)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_datasync/client/#update_discovery_job)
         """
+    async def update_location_azure_blob(
+        self,
+        *,
+        LocationArn: str,
+        Subdirectory: str = ...,
+        AuthenticationType: Literal["SAS"] = ...,
+        SasConfiguration: AzureBlobSasConfigurationTypeDef = ...,
+        BlobType: Literal["BLOCK"] = ...,
+        AccessTier: AzureAccessTierType = ...,
+        AgentArns: Sequence[str] = ...
+    ) -> Dict[str, Any]:
+        """
+        Modifies some configurations of the Microsoft Azure Blob Storage transfer
+        location that you're using with DataSync.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync.html#DataSync.Client.update_location_azure_blob)
+        [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_datasync/client/#update_location_azure_blob)
+        """
     async def update_location_hdfs(
         self,
         *,
         LocationArn: str,
         Subdirectory: str = ...,
         NameNodes: Sequence[HdfsNameNodeTypeDef] = ...,
         BlockSize: int = ...,
```

### Comparing `types-aiobotocore-datasync-2.5.2.post3/types_aiobotocore_datasync/literals.py` & `types-aiobotocore-datasync-2.5.4/types_aiobotocore_datasync/literals.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,14 +18,17 @@
 else:
     from typing_extensions import Literal
 
 
 __all__ = (
     "AgentStatusType",
     "AtimeType",
+    "AzureAccessTierType",
+    "AzureBlobAuthenticationTypeType",
+    "AzureBlobTypeType",
     "DescribeStorageSystemResourceMetricsPaginatorName",
     "DiscoveryJobStatusType",
     "DiscoveryResourceFilterType",
     "DiscoveryResourceTypeType",
     "DiscoverySystemTypeType",
     "EfsInTransitEncryptionType",
     "EndpointTypeType",
@@ -71,14 +74,17 @@
     "PaginatorName",
     "RegionName",
 )
 
 
 AgentStatusType = Literal["OFFLINE", "ONLINE"]
 AtimeType = Literal["BEST_EFFORT", "NONE"]
+AzureAccessTierType = Literal["ARCHIVE", "COOL", "HOT"]
+AzureBlobAuthenticationTypeType = Literal["SAS"]
+AzureBlobTypeType = Literal["BLOCK"]
 DescribeStorageSystemResourceMetricsPaginatorName = Literal[
     "describe_storage_system_resource_metrics"
 ]
 DiscoveryJobStatusType = Literal[
     "COMPLETED", "COMPLETED_WITH_ISSUES", "FAILED", "RUNNING", "STOPPED", "TERMINATED", "WARNING"
 ]
 DiscoveryResourceFilterType = Literal["SVM"]
@@ -156,14 +162,15 @@
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
@@ -259,14 +266,15 @@
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
@@ -345,26 +353,28 @@
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

### Comparing `types-aiobotocore-datasync-2.5.2.post3/types_aiobotocore_datasync/literals.pyi` & `types-aiobotocore-datasync-2.5.4/types_aiobotocore_datasync/literals.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -17,14 +17,17 @@
     from typing import Literal
 else:
     from typing_extensions import Literal
 
 __all__ = (
     "AgentStatusType",
     "AtimeType",
+    "AzureAccessTierType",
+    "AzureBlobAuthenticationTypeType",
+    "AzureBlobTypeType",
     "DescribeStorageSystemResourceMetricsPaginatorName",
     "DiscoveryJobStatusType",
     "DiscoveryResourceFilterType",
     "DiscoveryResourceTypeType",
     "DiscoverySystemTypeType",
     "EfsInTransitEncryptionType",
     "EndpointTypeType",
@@ -69,14 +72,17 @@
     "ResourceServiceName",
     "PaginatorName",
     "RegionName",
 )
 
 AgentStatusType = Literal["OFFLINE", "ONLINE"]
 AtimeType = Literal["BEST_EFFORT", "NONE"]
+AzureAccessTierType = Literal["ARCHIVE", "COOL", "HOT"]
+AzureBlobAuthenticationTypeType = Literal["SAS"]
+AzureBlobTypeType = Literal["BLOCK"]
 DescribeStorageSystemResourceMetricsPaginatorName = Literal[
     "describe_storage_system_resource_metrics"
 ]
 DiscoveryJobStatusType = Literal[
     "COMPLETED", "COMPLETED_WITH_ISSUES", "FAILED", "RUNNING", "STOPPED", "TERMINATED", "WARNING"
 ]
 DiscoveryResourceFilterType = Literal["SVM"]
@@ -154,14 +160,15 @@
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
@@ -257,14 +264,15 @@
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
@@ -343,26 +351,28 @@
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

### Comparing `types-aiobotocore-datasync-2.5.2.post3/types_aiobotocore_datasync/paginator.py` & `types-aiobotocore-datasync-2.5.4/types_aiobotocore_datasync/paginator.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-datasync-2.5.2.post3/types_aiobotocore_datasync/paginator.pyi` & `types-aiobotocore-datasync-2.5.4/types_aiobotocore_datasync/paginator.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-datasync-2.5.2.post3/types_aiobotocore_datasync/type_defs.py` & `types-aiobotocore-datasync-2.5.4/types_aiobotocore_datasync/type_defs.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 from typing import IO, Any, Dict, List, Mapping, Sequence, Union
 
 from aiobotocore.response import StreamingBody
 
 from .literals import (
     AgentStatusType,
     AtimeType,
+    AzureAccessTierType,
     DiscoveryJobStatusType,
     DiscoveryResourceTypeType,
     EfsInTransitEncryptionType,
     EndpointTypeType,
     GidType,
     HdfsAuthenticationTypeType,
     HdfsDataTransferProtectionType,
@@ -66,14 +67,15 @@
 
 __all__ = (
     "CredentialsTypeDef",
     "DiscoveryServerConfigurationTypeDef",
     "TagListEntryTypeDef",
     "ResponseMetadataTypeDef",
     "AgentListEntryTypeDef",
+    "AzureBlobSasConfigurationTypeDef",
     "BlobTypeDef",
     "CancelTaskExecutionRequestRequestTypeDef",
     "CapacityTypeDef",
     "Ec2ConfigTypeDef",
     "HdfsNameNodeTypeDef",
     "QopConfigurationTypeDef",
     "NfsMountOptionsTypeDef",
@@ -85,14 +87,15 @@
     "TaskScheduleTypeDef",
     "DeleteAgentRequestRequestTypeDef",
     "DeleteLocationRequestRequestTypeDef",
     "DeleteTaskRequestRequestTypeDef",
     "DescribeAgentRequestRequestTypeDef",
     "PrivateLinkConfigTypeDef",
     "DescribeDiscoveryJobRequestRequestTypeDef",
+    "DescribeLocationAzureBlobRequestRequestTypeDef",
     "DescribeLocationEfsRequestRequestTypeDef",
     "DescribeLocationFsxLustreRequestRequestTypeDef",
     "DescribeLocationFsxOntapRequestRequestTypeDef",
     "DescribeLocationFsxOpenZfsRequestRequestTypeDef",
     "DescribeLocationFsxWindowsRequestRequestTypeDef",
     "DescribeLocationHdfsRequestRequestTypeDef",
     "DescribeLocationNfsRequestRequestTypeDef",
@@ -134,34 +137,38 @@
     "CreateAgentRequestRequestTypeDef",
     "CreateLocationFsxLustreRequestRequestTypeDef",
     "CreateLocationFsxWindowsRequestRequestTypeDef",
     "StartDiscoveryJobRequestRequestTypeDef",
     "TagResourceRequestRequestTypeDef",
     "AddStorageSystemResponseTypeDef",
     "CreateAgentResponseTypeDef",
+    "CreateLocationAzureBlobResponseTypeDef",
     "CreateLocationEfsResponseTypeDef",
     "CreateLocationFsxLustreResponseTypeDef",
     "CreateLocationFsxOntapResponseTypeDef",
     "CreateLocationFsxOpenZfsResponseTypeDef",
     "CreateLocationFsxWindowsResponseTypeDef",
     "CreateLocationHdfsResponseTypeDef",
     "CreateLocationNfsResponseTypeDef",
     "CreateLocationObjectStorageResponseTypeDef",
     "CreateLocationS3ResponseTypeDef",
     "CreateLocationSmbResponseTypeDef",
     "CreateTaskResponseTypeDef",
     "DescribeDiscoveryJobResponseTypeDef",
+    "DescribeLocationAzureBlobResponseTypeDef",
     "DescribeLocationFsxLustreResponseTypeDef",
     "DescribeLocationFsxWindowsResponseTypeDef",
     "DescribeLocationObjectStorageResponseTypeDef",
     "DescribeStorageSystemResponseTypeDef",
     "ListTagsForResourceResponseTypeDef",
     "StartDiscoveryJobResponseTypeDef",
     "StartTaskExecutionResponseTypeDef",
     "ListAgentsResponseTypeDef",
+    "CreateLocationAzureBlobRequestRequestTypeDef",
+    "UpdateLocationAzureBlobRequestRequestTypeDef",
     "CreateLocationObjectStorageRequestRequestTypeDef",
     "UpdateLocationObjectStorageRequestRequestTypeDef",
     "CreateLocationEfsRequestRequestTypeDef",
     "DescribeLocationEfsResponseTypeDef",
     "CreateLocationHdfsRequestRequestTypeDef",
     "DescribeLocationHdfsResponseTypeDef",
     "UpdateLocationHdfsRequestRequestTypeDef",
@@ -278,14 +285,21 @@
         "AgentArn": str,
         "Name": str,
         "Status": AgentStatusType,
     },
     total=False,
 )
 
+AzureBlobSasConfigurationTypeDef = TypedDict(
+    "AzureBlobSasConfigurationTypeDef",
+    {
+        "Token": str,
+    },
+)
+
 BlobTypeDef = Union[str, bytes, IO[Any], StreamingBody]
 CancelTaskExecutionRequestRequestTypeDef = TypedDict(
     "CancelTaskExecutionRequestRequestTypeDef",
     {
         "TaskExecutionArn": str,
     },
 )
@@ -435,14 +449,21 @@
 DescribeDiscoveryJobRequestRequestTypeDef = TypedDict(
     "DescribeDiscoveryJobRequestRequestTypeDef",
     {
         "DiscoveryJobArn": str,
     },
 )
 
+DescribeLocationAzureBlobRequestRequestTypeDef = TypedDict(
+    "DescribeLocationAzureBlobRequestRequestTypeDef",
+    {
+        "LocationArn": str,
+    },
+)
+
 DescribeLocationEfsRequestRequestTypeDef = TypedDict(
     "DescribeLocationEfsRequestRequestTypeDef",
     {
         "LocationArn": str,
     },
 )
 
@@ -1000,14 +1021,22 @@
     "CreateAgentResponseTypeDef",
     {
         "AgentArn": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+CreateLocationAzureBlobResponseTypeDef = TypedDict(
+    "CreateLocationAzureBlobResponseTypeDef",
+    {
+        "LocationArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 CreateLocationEfsResponseTypeDef = TypedDict(
     "CreateLocationEfsResponseTypeDef",
     {
         "LocationArn": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -1101,14 +1130,28 @@
         "Status": DiscoveryJobStatusType,
         "JobStartTime": datetime,
         "JobEndTime": datetime,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+DescribeLocationAzureBlobResponseTypeDef = TypedDict(
+    "DescribeLocationAzureBlobResponseTypeDef",
+    {
+        "LocationArn": str,
+        "LocationUri": str,
+        "AuthenticationType": Literal["SAS"],
+        "BlobType": Literal["BLOCK"],
+        "AccessTier": AzureAccessTierType,
+        "AgentArns": List[str],
+        "CreationTime": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 DescribeLocationFsxLustreResponseTypeDef = TypedDict(
     "DescribeLocationFsxLustreResponseTypeDef",
     {
         "LocationArn": str,
         "LocationUri": str,
         "SecurityGroupArns": List[str],
         "CreationTime": datetime,
@@ -1191,14 +1234,69 @@
     {
         "Agents": List[AgentListEntryTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+_RequiredCreateLocationAzureBlobRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateLocationAzureBlobRequestRequestTypeDef",
+    {
+        "ContainerUrl": str,
+        "AuthenticationType": Literal["SAS"],
+        "AgentArns": Sequence[str],
+    },
+)
+_OptionalCreateLocationAzureBlobRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateLocationAzureBlobRequestRequestTypeDef",
+    {
+        "SasConfiguration": AzureBlobSasConfigurationTypeDef,
+        "BlobType": Literal["BLOCK"],
+        "AccessTier": AzureAccessTierType,
+        "Subdirectory": str,
+        "Tags": Sequence[TagListEntryTypeDef],
+    },
+    total=False,
+)
+
+
+class CreateLocationAzureBlobRequestRequestTypeDef(
+    _RequiredCreateLocationAzureBlobRequestRequestTypeDef,
+    _OptionalCreateLocationAzureBlobRequestRequestTypeDef,
+):
+    pass
+
+
+_RequiredUpdateLocationAzureBlobRequestRequestTypeDef = TypedDict(
+    "_RequiredUpdateLocationAzureBlobRequestRequestTypeDef",
+    {
+        "LocationArn": str,
+    },
+)
+_OptionalUpdateLocationAzureBlobRequestRequestTypeDef = TypedDict(
+    "_OptionalUpdateLocationAzureBlobRequestRequestTypeDef",
+    {
+        "Subdirectory": str,
+        "AuthenticationType": Literal["SAS"],
+        "SasConfiguration": AzureBlobSasConfigurationTypeDef,
+        "BlobType": Literal["BLOCK"],
+        "AccessTier": AzureAccessTierType,
+        "AgentArns": Sequence[str],
+    },
+    total=False,
+)
+
+
+class UpdateLocationAzureBlobRequestRequestTypeDef(
+    _RequiredUpdateLocationAzureBlobRequestRequestTypeDef,
+    _OptionalUpdateLocationAzureBlobRequestRequestTypeDef,
+):
+    pass
+
+
 _RequiredCreateLocationObjectStorageRequestRequestTypeDef = TypedDict(
     "_RequiredCreateLocationObjectStorageRequestRequestTypeDef",
     {
         "ServerHostname": str,
         "BucketName": str,
         "AgentArns": Sequence[str],
     },
@@ -1916,14 +2014,15 @@
         "ClusterName": str,
         "MaxP95Performance": MaxP95PerformanceTypeDef,
         "ClusterBlockStorageSize": int,
         "ClusterBlockStorageUsed": int,
         "ClusterBlockStorageLogicalUsed": int,
         "Recommendations": List[RecommendationTypeDef],
         "RecommendationStatus": RecommendationStatusType,
+        "LunCount": int,
     },
     total=False,
 )
 
 NetAppONTAPSVMTypeDef = TypedDict(
     "NetAppONTAPSVMTypeDef",
     {
@@ -1936,14 +2035,15 @@
         "TotalCapacityProvisioned": int,
         "TotalLogicalCapacityUsed": int,
         "MaxP95Performance": MaxP95PerformanceTypeDef,
         "Recommendations": List[RecommendationTypeDef],
         "NfsExportedVolumes": int,
         "RecommendationStatus": RecommendationStatusType,
         "TotalSnapshotCapacityUsed": int,
+        "LunCount": int,
     },
     total=False,
 )
 
 NetAppONTAPVolumeTypeDef = TypedDict(
     "NetAppONTAPVolumeTypeDef",
     {
@@ -1957,14 +2057,15 @@
         "CapacityProvisioned": int,
         "LogicalCapacityUsed": int,
         "NfsExported": bool,
         "SnapshotCapacityUsed": int,
         "MaxP95Performance": MaxP95PerformanceTypeDef,
         "Recommendations": List[RecommendationTypeDef],
         "RecommendationStatus": RecommendationStatusType,
+        "LunCount": int,
     },
     total=False,
 )
 
 P95MetricsTypeDef = TypedDict(
     "P95MetricsTypeDef",
     {
```

### Comparing `types-aiobotocore-datasync-2.5.2.post3/types_aiobotocore_datasync/type_defs.pyi` & `types-aiobotocore-datasync-2.5.4/types_aiobotocore_datasync/type_defs.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 from typing import IO, Any, Dict, List, Mapping, Sequence, Union
 
 from aiobotocore.response import StreamingBody
 
 from .literals import (
     AgentStatusType,
     AtimeType,
+    AzureAccessTierType,
     DiscoveryJobStatusType,
     DiscoveryResourceTypeType,
     EfsInTransitEncryptionType,
     EndpointTypeType,
     GidType,
     HdfsAuthenticationTypeType,
     HdfsDataTransferProtectionType,
@@ -65,14 +66,15 @@
 
 __all__ = (
     "CredentialsTypeDef",
     "DiscoveryServerConfigurationTypeDef",
     "TagListEntryTypeDef",
     "ResponseMetadataTypeDef",
     "AgentListEntryTypeDef",
+    "AzureBlobSasConfigurationTypeDef",
     "BlobTypeDef",
     "CancelTaskExecutionRequestRequestTypeDef",
     "CapacityTypeDef",
     "Ec2ConfigTypeDef",
     "HdfsNameNodeTypeDef",
     "QopConfigurationTypeDef",
     "NfsMountOptionsTypeDef",
@@ -84,14 +86,15 @@
     "TaskScheduleTypeDef",
     "DeleteAgentRequestRequestTypeDef",
     "DeleteLocationRequestRequestTypeDef",
     "DeleteTaskRequestRequestTypeDef",
     "DescribeAgentRequestRequestTypeDef",
     "PrivateLinkConfigTypeDef",
     "DescribeDiscoveryJobRequestRequestTypeDef",
+    "DescribeLocationAzureBlobRequestRequestTypeDef",
     "DescribeLocationEfsRequestRequestTypeDef",
     "DescribeLocationFsxLustreRequestRequestTypeDef",
     "DescribeLocationFsxOntapRequestRequestTypeDef",
     "DescribeLocationFsxOpenZfsRequestRequestTypeDef",
     "DescribeLocationFsxWindowsRequestRequestTypeDef",
     "DescribeLocationHdfsRequestRequestTypeDef",
     "DescribeLocationNfsRequestRequestTypeDef",
@@ -133,34 +136,38 @@
     "CreateAgentRequestRequestTypeDef",
     "CreateLocationFsxLustreRequestRequestTypeDef",
     "CreateLocationFsxWindowsRequestRequestTypeDef",
     "StartDiscoveryJobRequestRequestTypeDef",
     "TagResourceRequestRequestTypeDef",
     "AddStorageSystemResponseTypeDef",
     "CreateAgentResponseTypeDef",
+    "CreateLocationAzureBlobResponseTypeDef",
     "CreateLocationEfsResponseTypeDef",
     "CreateLocationFsxLustreResponseTypeDef",
     "CreateLocationFsxOntapResponseTypeDef",
     "CreateLocationFsxOpenZfsResponseTypeDef",
     "CreateLocationFsxWindowsResponseTypeDef",
     "CreateLocationHdfsResponseTypeDef",
     "CreateLocationNfsResponseTypeDef",
     "CreateLocationObjectStorageResponseTypeDef",
     "CreateLocationS3ResponseTypeDef",
     "CreateLocationSmbResponseTypeDef",
     "CreateTaskResponseTypeDef",
     "DescribeDiscoveryJobResponseTypeDef",
+    "DescribeLocationAzureBlobResponseTypeDef",
     "DescribeLocationFsxLustreResponseTypeDef",
     "DescribeLocationFsxWindowsResponseTypeDef",
     "DescribeLocationObjectStorageResponseTypeDef",
     "DescribeStorageSystemResponseTypeDef",
     "ListTagsForResourceResponseTypeDef",
     "StartDiscoveryJobResponseTypeDef",
     "StartTaskExecutionResponseTypeDef",
     "ListAgentsResponseTypeDef",
+    "CreateLocationAzureBlobRequestRequestTypeDef",
+    "UpdateLocationAzureBlobRequestRequestTypeDef",
     "CreateLocationObjectStorageRequestRequestTypeDef",
     "UpdateLocationObjectStorageRequestRequestTypeDef",
     "CreateLocationEfsRequestRequestTypeDef",
     "DescribeLocationEfsResponseTypeDef",
     "CreateLocationHdfsRequestRequestTypeDef",
     "DescribeLocationHdfsResponseTypeDef",
     "UpdateLocationHdfsRequestRequestTypeDef",
@@ -273,14 +280,21 @@
         "AgentArn": str,
         "Name": str,
         "Status": AgentStatusType,
     },
     total=False,
 )
 
+AzureBlobSasConfigurationTypeDef = TypedDict(
+    "AzureBlobSasConfigurationTypeDef",
+    {
+        "Token": str,
+    },
+)
+
 BlobTypeDef = Union[str, bytes, IO[Any], StreamingBody]
 CancelTaskExecutionRequestRequestTypeDef = TypedDict(
     "CancelTaskExecutionRequestRequestTypeDef",
     {
         "TaskExecutionArn": str,
     },
 )
@@ -430,14 +444,21 @@
 DescribeDiscoveryJobRequestRequestTypeDef = TypedDict(
     "DescribeDiscoveryJobRequestRequestTypeDef",
     {
         "DiscoveryJobArn": str,
     },
 )
 
+DescribeLocationAzureBlobRequestRequestTypeDef = TypedDict(
+    "DescribeLocationAzureBlobRequestRequestTypeDef",
+    {
+        "LocationArn": str,
+    },
+)
+
 DescribeLocationEfsRequestRequestTypeDef = TypedDict(
     "DescribeLocationEfsRequestRequestTypeDef",
     {
         "LocationArn": str,
     },
 )
 
@@ -977,14 +998,22 @@
     "CreateAgentResponseTypeDef",
     {
         "AgentArn": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+CreateLocationAzureBlobResponseTypeDef = TypedDict(
+    "CreateLocationAzureBlobResponseTypeDef",
+    {
+        "LocationArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 CreateLocationEfsResponseTypeDef = TypedDict(
     "CreateLocationEfsResponseTypeDef",
     {
         "LocationArn": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -1078,14 +1107,28 @@
         "Status": DiscoveryJobStatusType,
         "JobStartTime": datetime,
         "JobEndTime": datetime,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+DescribeLocationAzureBlobResponseTypeDef = TypedDict(
+    "DescribeLocationAzureBlobResponseTypeDef",
+    {
+        "LocationArn": str,
+        "LocationUri": str,
+        "AuthenticationType": Literal["SAS"],
+        "BlobType": Literal["BLOCK"],
+        "AccessTier": AzureAccessTierType,
+        "AgentArns": List[str],
+        "CreationTime": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 DescribeLocationFsxLustreResponseTypeDef = TypedDict(
     "DescribeLocationFsxLustreResponseTypeDef",
     {
         "LocationArn": str,
         "LocationUri": str,
         "SecurityGroupArns": List[str],
         "CreationTime": datetime,
@@ -1168,14 +1211,65 @@
     {
         "Agents": List[AgentListEntryTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+_RequiredCreateLocationAzureBlobRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateLocationAzureBlobRequestRequestTypeDef",
+    {
+        "ContainerUrl": str,
+        "AuthenticationType": Literal["SAS"],
+        "AgentArns": Sequence[str],
+    },
+)
+_OptionalCreateLocationAzureBlobRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateLocationAzureBlobRequestRequestTypeDef",
+    {
+        "SasConfiguration": AzureBlobSasConfigurationTypeDef,
+        "BlobType": Literal["BLOCK"],
+        "AccessTier": AzureAccessTierType,
+        "Subdirectory": str,
+        "Tags": Sequence[TagListEntryTypeDef],
+    },
+    total=False,
+)
+
+class CreateLocationAzureBlobRequestRequestTypeDef(
+    _RequiredCreateLocationAzureBlobRequestRequestTypeDef,
+    _OptionalCreateLocationAzureBlobRequestRequestTypeDef,
+):
+    pass
+
+_RequiredUpdateLocationAzureBlobRequestRequestTypeDef = TypedDict(
+    "_RequiredUpdateLocationAzureBlobRequestRequestTypeDef",
+    {
+        "LocationArn": str,
+    },
+)
+_OptionalUpdateLocationAzureBlobRequestRequestTypeDef = TypedDict(
+    "_OptionalUpdateLocationAzureBlobRequestRequestTypeDef",
+    {
+        "Subdirectory": str,
+        "AuthenticationType": Literal["SAS"],
+        "SasConfiguration": AzureBlobSasConfigurationTypeDef,
+        "BlobType": Literal["BLOCK"],
+        "AccessTier": AzureAccessTierType,
+        "AgentArns": Sequence[str],
+    },
+    total=False,
+)
+
+class UpdateLocationAzureBlobRequestRequestTypeDef(
+    _RequiredUpdateLocationAzureBlobRequestRequestTypeDef,
+    _OptionalUpdateLocationAzureBlobRequestRequestTypeDef,
+):
+    pass
+
 _RequiredCreateLocationObjectStorageRequestRequestTypeDef = TypedDict(
     "_RequiredCreateLocationObjectStorageRequestRequestTypeDef",
     {
         "ServerHostname": str,
         "BucketName": str,
         "AgentArns": Sequence[str],
     },
@@ -1859,14 +1953,15 @@
         "ClusterName": str,
         "MaxP95Performance": MaxP95PerformanceTypeDef,
         "ClusterBlockStorageSize": int,
         "ClusterBlockStorageUsed": int,
         "ClusterBlockStorageLogicalUsed": int,
         "Recommendations": List[RecommendationTypeDef],
         "RecommendationStatus": RecommendationStatusType,
+        "LunCount": int,
     },
     total=False,
 )
 
 NetAppONTAPSVMTypeDef = TypedDict(
     "NetAppONTAPSVMTypeDef",
     {
@@ -1879,14 +1974,15 @@
         "TotalCapacityProvisioned": int,
         "TotalLogicalCapacityUsed": int,
         "MaxP95Performance": MaxP95PerformanceTypeDef,
         "Recommendations": List[RecommendationTypeDef],
         "NfsExportedVolumes": int,
         "RecommendationStatus": RecommendationStatusType,
         "TotalSnapshotCapacityUsed": int,
+        "LunCount": int,
     },
     total=False,
 )
 
 NetAppONTAPVolumeTypeDef = TypedDict(
     "NetAppONTAPVolumeTypeDef",
     {
@@ -1900,14 +1996,15 @@
         "CapacityProvisioned": int,
         "LogicalCapacityUsed": int,
         "NfsExported": bool,
         "SnapshotCapacityUsed": int,
         "MaxP95Performance": MaxP95PerformanceTypeDef,
         "Recommendations": List[RecommendationTypeDef],
         "RecommendationStatus": RecommendationStatusType,
+        "LunCount": int,
     },
     total=False,
 )
 
 P95MetricsTypeDef = TypedDict(
     "P95MetricsTypeDef",
     {
```

### Comparing `types-aiobotocore-datasync-2.5.2.post3/types_aiobotocore_datasync.egg-info/PKG-INFO` & `types-aiobotocore-datasync-2.5.4/types_aiobotocore_datasync.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-datasync
-Version: 2.5.2.post3
-Summary: Type annotations for aiobotocore.DataSync 2.5.2 service generated with mypy-boto3-builder 7.17.2
+Version: 2.5.4
+Summary: Type annotations for aiobotocore.DataSync 2.5.4 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_datasync/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-datasync.svg?color=blue)](https://pypi.org/project/types-aiobotocore-datasync)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_datasync/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-datasync)](https://pepy.tech/project/types-aiobotocore-datasync)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.DataSync 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync.html#DataSync)
+[aiobotocore.DataSync 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync.html#DataSync)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-datasync-2.5.2.post3/types_aiobotocore_datasync.egg-info/SOURCES.txt` & `types-aiobotocore-datasync-2.5.4/types_aiobotocore_datasync.egg-info/SOURCES.txt`

 * *Files identical despite different names*


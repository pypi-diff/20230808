# Comparing `tmp/types-aiobotocore-fsx-2.5.2.post3.tar.gz` & `tmp/types-aiobotocore-fsx-2.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-fsx-2.5.2.post3.tar", last modified: Fri Aug  4 12:37:45 2023, max compression
+gzip compressed data, was "types-aiobotocore-fsx-2.5.4.tar", last modified: Tue Aug  8 01:23:45 2023, max compression
```

## Comparing `types-aiobotocore-fsx-2.5.2.post3.tar` & `types-aiobotocore-fsx-2.5.4.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:37:45.387850 types-aiobotocore-fsx-2.5.2.post3/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-04 12:24:04.000000 types-aiobotocore-fsx-2.5.2.post3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    13394 2023-08-04 12:37:45.387850 types-aiobotocore-fsx-2.5.2.post3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    11892 2023-08-04 12:24:04.000000 types-aiobotocore-fsx-2.5.2.post3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-04 12:37:45.387850 types-aiobotocore-fsx-2.5.2.post3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2020 2023-08-04 12:24:04.000000 types-aiobotocore-fsx-2.5.2.post3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:37:45.367850 types-aiobotocore-fsx-2.5.2.post3/types_aiobotocore_fsx/
--rw-r--r--   0 runner    (1001) docker     (123)     1577 2023-08-04 12:24:04.000000 types-aiobotocore-fsx-2.5.2.post3/types_aiobotocore_fsx/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1576 2023-08-04 12:24:04.000000 types-aiobotocore-fsx-2.5.2.post3/types_aiobotocore_fsx/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      916 2023-08-04 12:24:04.000000 types-aiobotocore-fsx-2.5.2.post3/types_aiobotocore_fsx/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    40811 2023-08-04 12:24:04.000000 types-aiobotocore-fsx-2.5.2.post3/types_aiobotocore_fsx/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    40756 2023-08-04 12:24:04.000000 types-aiobotocore-fsx-2.5.2.post3/types_aiobotocore_fsx/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    14870 2023-08-04 12:24:05.000000 types-aiobotocore-fsx-2.5.2.post3/types_aiobotocore_fsx/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    14868 2023-08-04 12:24:05.000000 types-aiobotocore-fsx-2.5.2.post3/types_aiobotocore_fsx/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     6930 2023-08-04 12:24:05.000000 types-aiobotocore-fsx-2.5.2.post3/types_aiobotocore_fsx/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     6923 2023-08-04 12:24:05.000000 types-aiobotocore-fsx-2.5.2.post3/types_aiobotocore_fsx/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 12:24:04.000000 types-aiobotocore-fsx-2.5.2.post3/types_aiobotocore_fsx/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    79330 2023-08-04 12:24:08.000000 types-aiobotocore-fsx-2.5.2.post3/types_aiobotocore_fsx/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    79233 2023-08-04 12:24:07.000000 types-aiobotocore-fsx-2.5.2.post3/types_aiobotocore_fsx/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-04 12:24:04.000000 types-aiobotocore-fsx-2.5.2.post3/types_aiobotocore_fsx/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:37:45.387850 types-aiobotocore-fsx-2.5.2.post3/types_aiobotocore_fsx.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    13394 2023-08-04 12:37:45.000000 types-aiobotocore-fsx-2.5.2.post3/types_aiobotocore_fsx.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      737 2023-08-04 12:37:45.000000 types-aiobotocore-fsx-2.5.2.post3/types_aiobotocore_fsx.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 12:37:45.000000 types-aiobotocore-fsx-2.5.2.post3/types_aiobotocore_fsx.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 12:37:45.000000 types-aiobotocore-fsx-2.5.2.post3/types_aiobotocore_fsx.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-04 12:37:45.000000 types-aiobotocore-fsx-2.5.2.post3/types_aiobotocore_fsx.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-08-04 12:37:45.000000 types-aiobotocore-fsx-2.5.2.post3/types_aiobotocore_fsx.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:23:45.754721 types-aiobotocore-fsx-2.5.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-08 01:11:27.000000 types-aiobotocore-fsx-2.5.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    13388 2023-08-08 01:23:45.754721 types-aiobotocore-fsx-2.5.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    11892 2023-08-08 01:11:27.000000 types-aiobotocore-fsx-2.5.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-08 01:23:45.754721 types-aiobotocore-fsx-2.5.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2014 2023-08-08 01:11:27.000000 types-aiobotocore-fsx-2.5.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:23:45.754721 types-aiobotocore-fsx-2.5.4/types_aiobotocore_fsx/
+-rw-r--r--   0 runner    (1001) docker     (123)     1577 2023-08-08 01:11:27.000000 types-aiobotocore-fsx-2.5.4/types_aiobotocore_fsx/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1576 2023-08-08 01:11:27.000000 types-aiobotocore-fsx-2.5.4/types_aiobotocore_fsx/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      904 2023-08-08 01:11:27.000000 types-aiobotocore-fsx-2.5.4/types_aiobotocore_fsx/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40811 2023-08-08 01:11:28.000000 types-aiobotocore-fsx-2.5.4/types_aiobotocore_fsx/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40756 2023-08-08 01:11:28.000000 types-aiobotocore-fsx-2.5.4/types_aiobotocore_fsx/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    15428 2023-08-08 01:11:28.000000 types-aiobotocore-fsx-2.5.4/types_aiobotocore_fsx/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15426 2023-08-08 01:11:28.000000 types-aiobotocore-fsx-2.5.4/types_aiobotocore_fsx/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     6930 2023-08-08 01:11:28.000000 types-aiobotocore-fsx-2.5.4/types_aiobotocore_fsx/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6923 2023-08-08 01:11:28.000000 types-aiobotocore-fsx-2.5.4/types_aiobotocore_fsx/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 01:11:27.000000 types-aiobotocore-fsx-2.5.4/types_aiobotocore_fsx/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    82381 2023-08-08 01:11:31.000000 types-aiobotocore-fsx-2.5.4/types_aiobotocore_fsx/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    82278 2023-08-08 01:11:30.000000 types-aiobotocore-fsx-2.5.4/types_aiobotocore_fsx/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-08-08 01:11:27.000000 types-aiobotocore-fsx-2.5.4/types_aiobotocore_fsx/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:23:45.754721 types-aiobotocore-fsx-2.5.4/types_aiobotocore_fsx.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    13388 2023-08-08 01:23:45.000000 types-aiobotocore-fsx-2.5.4/types_aiobotocore_fsx.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      737 2023-08-08 01:23:45.000000 types-aiobotocore-fsx-2.5.4/types_aiobotocore_fsx.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 01:23:45.000000 types-aiobotocore-fsx-2.5.4/types_aiobotocore_fsx.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 01:23:45.000000 types-aiobotocore-fsx-2.5.4/types_aiobotocore_fsx.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-08 01:23:45.000000 types-aiobotocore-fsx-2.5.4/types_aiobotocore_fsx.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-08-08 01:23:45.000000 types-aiobotocore-fsx-2.5.4/types_aiobotocore_fsx.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-fsx-2.5.2.post3/LICENSE` & `types-aiobotocore-fsx-2.5.4/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-fsx-2.5.2.post3/PKG-INFO` & `types-aiobotocore-fsx-2.5.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-fsx
-Version: 2.5.2.post3
-Summary: Type annotations for aiobotocore.FSx 2.5.2 service generated with mypy-boto3-builder 7.17.2
+Version: 2.5.4
+Summary: Type annotations for aiobotocore.FSx 2.5.4 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_fsx/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-fsx.svg?color=blue)](https://pypi.org/project/types-aiobotocore-fsx)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_fsx/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-fsx)](https://pepy.tech/project/types-aiobotocore-fsx)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.FSx 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fsx.html#FSx)
+[aiobotocore.FSx 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fsx.html#FSx)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-fsx-2.5.2.post3/README.md` & `types-aiobotocore-fsx-2.5.4/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-fsx.svg?color=blue)](https://pypi.org/project/types-aiobotocore-fsx)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_fsx/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-fsx)](https://pepy.tech/project/types-aiobotocore-fsx)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.FSx 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fsx.html#FSx)
+[aiobotocore.FSx 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fsx.html#FSx)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-fsx-2.5.2.post3/setup.py` & `types-aiobotocore-fsx-2.5.4/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-fsx",
-    version="2.5.2.post3",
+    version="2.5.4",
     packages=["types_aiobotocore_fsx"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.FSx 2.5.2 service generated with mypy-boto3-builder"
+        "Type annotations for aiobotocore.FSx 2.5.4 service generated with mypy-boto3-builder"
         " 7.17.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
```

### Comparing `types-aiobotocore-fsx-2.5.2.post3/types_aiobotocore_fsx/__init__.py` & `types-aiobotocore-fsx-2.5.4/types_aiobotocore_fsx/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-fsx-2.5.2.post3/types_aiobotocore_fsx/__init__.pyi` & `types-aiobotocore-fsx-2.5.4/types_aiobotocore_fsx/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-fsx-2.5.2.post3/types_aiobotocore_fsx/__main__.py` & `types-aiobotocore-fsx-2.5.4/types_aiobotocore_fsx/__main__.py`

 * *Files 13% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.FSx 2.5.2\nVersion:         2.5.2.post3\nBuilder version:"
+        "Type annotations for aiobotocore.FSx 2.5.4\nVersion:         2.5.4\nBuilder version:"
         " 7.17.2\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_fsx//\nBoto3 docs:    "
         "  https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fsx.html#FSx\nOther"
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

### Comparing `types-aiobotocore-fsx-2.5.2.post3/types_aiobotocore_fsx/client.py` & `types-aiobotocore-fsx-2.5.4/types_aiobotocore_fsx/client.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-fsx-2.5.2.post3/types_aiobotocore_fsx/client.pyi` & `types-aiobotocore-fsx-2.5.4/types_aiobotocore_fsx/client.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-fsx-2.5.2.post3/types_aiobotocore_fsx/literals.py` & `types-aiobotocore-fsx-2.5.4/types_aiobotocore_fsx/literals.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,14 +19,15 @@
     from typing_extensions import Literal
 
 
 __all__ = (
     "AdministrativeActionTypeType",
     "AliasLifecycleType",
     "AutoImportPolicyTypeType",
+    "AutocommitPeriodTypeType",
     "BackupLifecycleType",
     "BackupTypeType",
     "DataCompressionTypeType",
     "DataRepositoryLifecycleType",
     "DataRepositoryTaskFilterNameType",
     "DataRepositoryTaskLifecycleType",
     "DataRepositoryTaskTypeType",
@@ -54,19 +55,22 @@
     "NfsVersionType",
     "OntapDeploymentTypeType",
     "OntapVolumeTypeType",
     "OpenZFSCopyStrategyType",
     "OpenZFSDataCompressionTypeType",
     "OpenZFSDeploymentTypeType",
     "OpenZFSQuotaTypeType",
+    "PrivilegedDeleteType",
     "ReportFormatType",
     "ReportScopeType",
     "ResourceTypeType",
     "RestoreOpenZFSVolumeOptionType",
+    "RetentionPeriodTypeType",
     "SecurityStyleType",
+    "SnaplockTypeType",
     "SnapshotFilterNameType",
     "SnapshotLifecycleType",
     "StatusType",
     "StorageTypeType",
     "StorageVirtualMachineFilterNameType",
     "StorageVirtualMachineLifecycleType",
     "StorageVirtualMachineRootVolumeSecurityStyleType",
@@ -93,14 +97,15 @@
     "SNAPSHOT_UPDATE",
     "STORAGE_OPTIMIZATION",
     "VOLUME_RESTORE",
     "VOLUME_UPDATE",
 ]
 AliasLifecycleType = Literal["AVAILABLE", "CREATE_FAILED", "CREATING", "DELETE_FAILED", "DELETING"]
 AutoImportPolicyTypeType = Literal["NEW", "NEW_CHANGED", "NEW_CHANGED_DELETED", "NONE"]
+AutocommitPeriodTypeType = Literal["DAYS", "HOURS", "MINUTES", "MONTHS", "NONE", "YEARS"]
 BackupLifecycleType = Literal[
     "AVAILABLE", "COPYING", "CREATING", "DELETED", "FAILED", "PENDING", "TRANSFERRING"
 ]
 BackupTypeType = Literal["AUTOMATIC", "AWS_BACKUP", "USER_INITIATED"]
 DataCompressionTypeType = Literal["LZ4", "NONE"]
 DataRepositoryLifecycleType = Literal[
     "AVAILABLE", "CREATING", "DELETING", "FAILED", "MISCONFIGURED", "UPDATING"
@@ -157,19 +162,24 @@
 NfsVersionType = Literal["NFS3"]
 OntapDeploymentTypeType = Literal["MULTI_AZ_1", "SINGLE_AZ_1"]
 OntapVolumeTypeType = Literal["DP", "LS", "RW"]
 OpenZFSCopyStrategyType = Literal["CLONE", "FULL_COPY"]
 OpenZFSDataCompressionTypeType = Literal["LZ4", "NONE", "ZSTD"]
 OpenZFSDeploymentTypeType = Literal["SINGLE_AZ_1", "SINGLE_AZ_2"]
 OpenZFSQuotaTypeType = Literal["GROUP", "USER"]
+PrivilegedDeleteType = Literal["DISABLED", "ENABLED", "PERMANENTLY_DISABLED"]
 ReportFormatType = Literal["REPORT_CSV_20191124"]
 ReportScopeType = Literal["FAILED_FILES_ONLY"]
 ResourceTypeType = Literal["FILE_SYSTEM", "VOLUME"]
 RestoreOpenZFSVolumeOptionType = Literal["DELETE_CLONED_VOLUMES", "DELETE_INTERMEDIATE_SNAPSHOTS"]
+RetentionPeriodTypeType = Literal[
+    "DAYS", "HOURS", "INFINITE", "MINUTES", "MONTHS", "SECONDS", "UNSPECIFIED", "YEARS"
+]
 SecurityStyleType = Literal["MIXED", "NTFS", "UNIX"]
+SnaplockTypeType = Literal["COMPLIANCE", "ENTERPRISE"]
 SnapshotFilterNameType = Literal["file-system-id", "volume-id"]
 SnapshotLifecycleType = Literal["AVAILABLE", "CREATING", "DELETING", "PENDING"]
 StatusType = Literal["COMPLETED", "FAILED", "IN_PROGRESS", "PENDING", "UPDATED_OPTIMIZING"]
 StorageTypeType = Literal["HDD", "SSD"]
 StorageVirtualMachineFilterNameType = Literal["file-system-id"]
 StorageVirtualMachineLifecycleType = Literal[
     "CREATED", "CREATING", "DELETING", "FAILED", "MISCONFIGURED", "PENDING"
@@ -200,14 +210,15 @@
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
@@ -303,14 +314,15 @@
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
@@ -389,26 +401,28 @@
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

### Comparing `types-aiobotocore-fsx-2.5.2.post3/types_aiobotocore_fsx/literals.pyi` & `types-aiobotocore-fsx-2.5.4/types_aiobotocore_fsx/literals.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -18,14 +18,15 @@
 else:
     from typing_extensions import Literal
 
 __all__ = (
     "AdministrativeActionTypeType",
     "AliasLifecycleType",
     "AutoImportPolicyTypeType",
+    "AutocommitPeriodTypeType",
     "BackupLifecycleType",
     "BackupTypeType",
     "DataCompressionTypeType",
     "DataRepositoryLifecycleType",
     "DataRepositoryTaskFilterNameType",
     "DataRepositoryTaskLifecycleType",
     "DataRepositoryTaskTypeType",
@@ -53,19 +54,22 @@
     "NfsVersionType",
     "OntapDeploymentTypeType",
     "OntapVolumeTypeType",
     "OpenZFSCopyStrategyType",
     "OpenZFSDataCompressionTypeType",
     "OpenZFSDeploymentTypeType",
     "OpenZFSQuotaTypeType",
+    "PrivilegedDeleteType",
     "ReportFormatType",
     "ReportScopeType",
     "ResourceTypeType",
     "RestoreOpenZFSVolumeOptionType",
+    "RetentionPeriodTypeType",
     "SecurityStyleType",
+    "SnaplockTypeType",
     "SnapshotFilterNameType",
     "SnapshotLifecycleType",
     "StatusType",
     "StorageTypeType",
     "StorageVirtualMachineFilterNameType",
     "StorageVirtualMachineLifecycleType",
     "StorageVirtualMachineRootVolumeSecurityStyleType",
@@ -91,14 +95,15 @@
     "SNAPSHOT_UPDATE",
     "STORAGE_OPTIMIZATION",
     "VOLUME_RESTORE",
     "VOLUME_UPDATE",
 ]
 AliasLifecycleType = Literal["AVAILABLE", "CREATE_FAILED", "CREATING", "DELETE_FAILED", "DELETING"]
 AutoImportPolicyTypeType = Literal["NEW", "NEW_CHANGED", "NEW_CHANGED_DELETED", "NONE"]
+AutocommitPeriodTypeType = Literal["DAYS", "HOURS", "MINUTES", "MONTHS", "NONE", "YEARS"]
 BackupLifecycleType = Literal[
     "AVAILABLE", "COPYING", "CREATING", "DELETED", "FAILED", "PENDING", "TRANSFERRING"
 ]
 BackupTypeType = Literal["AUTOMATIC", "AWS_BACKUP", "USER_INITIATED"]
 DataCompressionTypeType = Literal["LZ4", "NONE"]
 DataRepositoryLifecycleType = Literal[
     "AVAILABLE", "CREATING", "DELETING", "FAILED", "MISCONFIGURED", "UPDATING"
@@ -155,19 +160,24 @@
 NfsVersionType = Literal["NFS3"]
 OntapDeploymentTypeType = Literal["MULTI_AZ_1", "SINGLE_AZ_1"]
 OntapVolumeTypeType = Literal["DP", "LS", "RW"]
 OpenZFSCopyStrategyType = Literal["CLONE", "FULL_COPY"]
 OpenZFSDataCompressionTypeType = Literal["LZ4", "NONE", "ZSTD"]
 OpenZFSDeploymentTypeType = Literal["SINGLE_AZ_1", "SINGLE_AZ_2"]
 OpenZFSQuotaTypeType = Literal["GROUP", "USER"]
+PrivilegedDeleteType = Literal["DISABLED", "ENABLED", "PERMANENTLY_DISABLED"]
 ReportFormatType = Literal["REPORT_CSV_20191124"]
 ReportScopeType = Literal["FAILED_FILES_ONLY"]
 ResourceTypeType = Literal["FILE_SYSTEM", "VOLUME"]
 RestoreOpenZFSVolumeOptionType = Literal["DELETE_CLONED_VOLUMES", "DELETE_INTERMEDIATE_SNAPSHOTS"]
+RetentionPeriodTypeType = Literal[
+    "DAYS", "HOURS", "INFINITE", "MINUTES", "MONTHS", "SECONDS", "UNSPECIFIED", "YEARS"
+]
 SecurityStyleType = Literal["MIXED", "NTFS", "UNIX"]
+SnaplockTypeType = Literal["COMPLIANCE", "ENTERPRISE"]
 SnapshotFilterNameType = Literal["file-system-id", "volume-id"]
 SnapshotLifecycleType = Literal["AVAILABLE", "CREATING", "DELETING", "PENDING"]
 StatusType = Literal["COMPLETED", "FAILED", "IN_PROGRESS", "PENDING", "UPDATED_OPTIMIZING"]
 StorageTypeType = Literal["HDD", "SSD"]
 StorageVirtualMachineFilterNameType = Literal["file-system-id"]
 StorageVirtualMachineLifecycleType = Literal[
     "CREATED", "CREATING", "DELETING", "FAILED", "MISCONFIGURED", "PENDING"
@@ -198,14 +208,15 @@
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
@@ -301,14 +312,15 @@
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
@@ -387,26 +399,28 @@
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

### Comparing `types-aiobotocore-fsx-2.5.2.post3/types_aiobotocore_fsx/paginator.py` & `types-aiobotocore-fsx-2.5.4/types_aiobotocore_fsx/paginator.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-fsx-2.5.2.post3/types_aiobotocore_fsx/paginator.pyi` & `types-aiobotocore-fsx-2.5.4/types_aiobotocore_fsx/paginator.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-fsx-2.5.2.post3/types_aiobotocore_fsx/type_defs.py` & `types-aiobotocore-fsx-2.5.4/types_aiobotocore_fsx/type_defs.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 import sys
 from datetime import datetime
 from typing import Any, Dict, List, Sequence
 
 from .literals import (
     AdministrativeActionTypeType,
     AliasLifecycleType,
+    AutocommitPeriodTypeType,
     AutoImportPolicyTypeType,
     BackupLifecycleType,
     BackupTypeType,
     DataCompressionTypeType,
     DataRepositoryLifecycleType,
     DataRepositoryTaskFilterNameType,
     DataRepositoryTaskLifecycleType,
@@ -40,17 +41,20 @@
     LustreDeploymentTypeType,
     OntapDeploymentTypeType,
     OntapVolumeTypeType,
     OpenZFSCopyStrategyType,
     OpenZFSDataCompressionTypeType,
     OpenZFSDeploymentTypeType,
     OpenZFSQuotaTypeType,
+    PrivilegedDeleteType,
     ResourceTypeType,
     RestoreOpenZFSVolumeOptionType,
+    RetentionPeriodTypeType,
     SecurityStyleType,
+    SnaplockTypeType,
     SnapshotFilterNameType,
     SnapshotLifecycleType,
     StatusType,
     StorageTypeType,
     StorageVirtualMachineLifecycleType,
     StorageVirtualMachineRootVolumeSecurityStyleType,
     StorageVirtualMachineSubtypeType,
@@ -67,23 +71,23 @@
 else:
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "ActiveDirectoryBackupAttributesTypeDef",
     "AdministrativeActionFailureDetailsTypeDef",
     "AliasTypeDef",
     "AssociateFileSystemAliasesRequestRequestTypeDef",
     "ResponseMetadataTypeDef",
     "AutoExportPolicyTypeDef",
     "AutoImportPolicyTypeDef",
+    "AutocommitPeriodTypeDef",
     "BackupFailureDetailsTypeDef",
     "TagTypeDef",
     "CancelDataRepositoryTaskRequestRequestTypeDef",
     "CompletionReportTypeDef",
     "FileCacheLustreMetadataConfigurationTypeDef",
     "LustreLogCreateConfigurationTypeDef",
     "LustreRootSquashConfigurationTypeDef",
@@ -119,14 +123,15 @@
     "FileSystemFailureDetailsTypeDef",
     "LifecycleTransitionReasonTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
     "OpenZFSClientConfigurationTypeDef",
     "OpenZFSOriginSnapshotConfigurationTypeDef",
     "ReleaseFileSystemNfsV3LocksRequestRequestTypeDef",
     "RestoreVolumeFromSnapshotRequestRequestTypeDef",
+    "RetentionPeriodTypeDef",
     "SelfManagedActiveDirectoryAttributesTypeDef",
     "SelfManagedActiveDirectoryConfigurationUpdatesTypeDef",
     "SvmEndpointTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateFileCacheLustreConfigurationTypeDef",
     "UpdateSnapshotRequestRequestTypeDef",
     "WindowsAuditLogConfigurationTypeDef",
@@ -166,17 +171,14 @@
     "UpdateFileSystemLustreConfigurationTypeDef",
     "CreateFileSystemOntapConfigurationTypeDef",
     "OpenZFSFileSystemConfigurationTypeDef",
     "UpdateFileSystemOntapConfigurationTypeDef",
     "UpdateFileSystemOpenZFSConfigurationTypeDef",
     "CreateSvmActiveDirectoryConfigurationTypeDef",
     "CreateFileSystemWindowsConfigurationTypeDef",
-    "CreateOntapVolumeConfigurationTypeDef",
-    "OntapVolumeConfigurationTypeDef",
-    "UpdateOntapVolumeConfigurationTypeDef",
     "DataRepositoryConfigurationTypeDef",
     "DescribeDataRepositoryTasksRequestRequestTypeDef",
     "DataRepositoryTaskTypeDef",
     "DescribeBackupsRequestRequestTypeDef",
     "DescribeDataRepositoryAssociationsRequestRequestTypeDef",
     "DescribeBackupsRequestDescribeBackupsPaginateTypeDef",
     "DescribeFileSystemsRequestDescribeFileSystemsPaginateTypeDef",
@@ -187,62 +189,69 @@
     "DescribeVolumesRequestDescribeVolumesPaginateTypeDef",
     "DescribeVolumesRequestRequestTypeDef",
     "FileCacheDataRepositoryAssociationTypeDef",
     "FileCacheLustreConfigurationTypeDef",
     "FileSystemEndpointsTypeDef",
     "SnapshotTypeDef",
     "OpenZFSNfsExportTypeDef",
+    "SnaplockRetentionPeriodTypeDef",
     "SvmActiveDirectoryConfigurationTypeDef",
     "UpdateFileSystemWindowsConfigurationTypeDef",
     "UpdateSvmActiveDirectoryConfigurationTypeDef",
     "SvmEndpointsTypeDef",
     "UpdateFileCacheRequestRequestTypeDef",
     "WindowsFileSystemConfigurationTypeDef",
     "CreateDataRepositoryAssociationRequestRequestTypeDef",
     "DataRepositoryAssociationTypeDef",
     "UpdateDataRepositoryAssociationRequestRequestTypeDef",
     "DeleteFileSystemRequestRequestTypeDef",
     "DeleteFileSystemResponseTypeDef",
     "DeleteVolumeRequestRequestTypeDef",
     "DeleteVolumeResponseTypeDef",
     "CreateStorageVirtualMachineRequestRequestTypeDef",
-    "CreateVolumeFromBackupRequestRequestTypeDef",
     "LustreFileSystemConfigurationTypeDef",
     "CreateDataRepositoryTaskResponseTypeDef",
     "DescribeDataRepositoryTasksResponseTypeDef",
     "CreateFileCacheRequestRequestTypeDef",
     "FileCacheCreatingTypeDef",
     "FileCacheTypeDef",
     "OntapFileSystemConfigurationTypeDef",
     "CreateSnapshotResponseTypeDef",
     "DescribeSnapshotsResponseTypeDef",
     "UpdateSnapshotResponseTypeDef",
     "CreateOpenZFSVolumeConfigurationTypeDef",
     "OpenZFSCreateRootVolumeConfigurationTypeDef",
     "OpenZFSVolumeConfigurationTypeDef",
     "UpdateOpenZFSVolumeConfigurationTypeDef",
+    "CreateSnaplockConfigurationTypeDef",
+    "SnaplockConfigurationTypeDef",
+    "UpdateSnaplockConfigurationTypeDef",
     "UpdateFileSystemRequestRequestTypeDef",
     "UpdateStorageVirtualMachineRequestRequestTypeDef",
     "StorageVirtualMachineTypeDef",
     "CreateDataRepositoryAssociationResponseTypeDef",
     "DescribeDataRepositoryAssociationsResponseTypeDef",
     "UpdateDataRepositoryAssociationResponseTypeDef",
     "CreateFileCacheResponseTypeDef",
     "DescribeFileCachesResponseTypeDef",
     "UpdateFileCacheResponseTypeDef",
     "FileSystemTypeDef",
-    "CreateVolumeRequestRequestTypeDef",
     "CreateFileSystemOpenZFSConfigurationTypeDef",
-    "VolumeTypeDef",
-    "UpdateVolumeRequestRequestTypeDef",
+    "CreateOntapVolumeConfigurationTypeDef",
+    "OntapVolumeConfigurationTypeDef",
+    "UpdateOntapVolumeConfigurationTypeDef",
     "CreateStorageVirtualMachineResponseTypeDef",
     "DescribeStorageVirtualMachinesResponseTypeDef",
     "UpdateStorageVirtualMachineResponseTypeDef",
     "CreateFileSystemFromBackupRequestRequestTypeDef",
     "CreateFileSystemRequestRequestTypeDef",
+    "CreateVolumeFromBackupRequestRequestTypeDef",
+    "CreateVolumeRequestRequestTypeDef",
+    "VolumeTypeDef",
+    "UpdateVolumeRequestRequestTypeDef",
     "AdministrativeActionTypeDef",
     "BackupTypeDef",
     "CreateVolumeFromBackupResponseTypeDef",
     "CreateVolumeResponseTypeDef",
     "DescribeVolumesResponseTypeDef",
     "UpdateVolumeResponseTypeDef",
     "CopyBackupResponseTypeDef",
@@ -288,22 +297,20 @@
     "_OptionalAssociateFileSystemAliasesRequestRequestTypeDef",
     {
         "ClientRequestToken": str,
     },
     total=False,
 )
 
-
 class AssociateFileSystemAliasesRequestRequestTypeDef(
     _RequiredAssociateFileSystemAliasesRequestRequestTypeDef,
     _OptionalAssociateFileSystemAliasesRequestRequestTypeDef,
 ):
     pass
 
-
 ResponseMetadataTypeDef = TypedDict(
     "ResponseMetadataTypeDef",
     {
         "RequestId": str,
         "HostId": str,
         "HTTPStatusCode": int,
         "HTTPHeaders": Dict[str, str],
@@ -323,14 +330,31 @@
     "AutoImportPolicyTypeDef",
     {
         "Events": Sequence[EventTypeType],
     },
     total=False,
 )
 
+_RequiredAutocommitPeriodTypeDef = TypedDict(
+    "_RequiredAutocommitPeriodTypeDef",
+    {
+        "Type": AutocommitPeriodTypeType,
+    },
+)
+_OptionalAutocommitPeriodTypeDef = TypedDict(
+    "_OptionalAutocommitPeriodTypeDef",
+    {
+        "Value": int,
+    },
+    total=False,
+)
+
+class AutocommitPeriodTypeDef(_RequiredAutocommitPeriodTypeDef, _OptionalAutocommitPeriodTypeDef):
+    pass
+
 BackupFailureDetailsTypeDef = TypedDict(
     "BackupFailureDetailsTypeDef",
     {
         "Message": str,
     },
     total=False,
 )
@@ -362,19 +386,17 @@
         "Path": str,
         "Format": Literal["REPORT_CSV_20191124"],
         "Scope": Literal["FAILED_FILES_ONLY"],
     },
     total=False,
 )
 
-
 class CompletionReportTypeDef(_RequiredCompletionReportTypeDef, _OptionalCompletionReportTypeDef):
     pass
 
-
 FileCacheLustreMetadataConfigurationTypeDef = TypedDict(
     "FileCacheLustreMetadataConfigurationTypeDef",
     {
         "StorageCapacity": int,
     },
 )
 
@@ -388,21 +410,19 @@
     "_OptionalLustreLogCreateConfigurationTypeDef",
     {
         "Destination": str,
     },
     total=False,
 )
 
-
 class LustreLogCreateConfigurationTypeDef(
     _RequiredLustreLogCreateConfigurationTypeDef, _OptionalLustreLogCreateConfigurationTypeDef
 ):
     pass
 
-
 LustreRootSquashConfigurationTypeDef = TypedDict(
     "LustreRootSquashConfigurationTypeDef",
     {
         "RootSquash": str,
         "NoSquashNids": List[str],
     },
     total=False,
@@ -431,22 +451,20 @@
     {
         "OrganizationalUnitDistinguishedName": str,
         "FileSystemAdministratorsGroup": str,
     },
     total=False,
 )
 
-
 class SelfManagedActiveDirectoryConfigurationTypeDef(
     _RequiredSelfManagedActiveDirectoryConfigurationTypeDef,
     _OptionalSelfManagedActiveDirectoryConfigurationTypeDef,
 ):
     pass
 
-
 _RequiredWindowsAuditLogCreateConfigurationTypeDef = TypedDict(
     "_RequiredWindowsAuditLogCreateConfigurationTypeDef",
     {
         "FileAccessAuditLogLevel": WindowsAccessAuditLogLevelType,
         "FileShareAccessAuditLogLevel": WindowsAccessAuditLogLevelType,
     },
 )
@@ -454,22 +472,20 @@
     "_OptionalWindowsAuditLogCreateConfigurationTypeDef",
     {
         "AuditLogDestination": str,
     },
     total=False,
 )
 
-
 class WindowsAuditLogCreateConfigurationTypeDef(
     _RequiredWindowsAuditLogCreateConfigurationTypeDef,
     _OptionalWindowsAuditLogCreateConfigurationTypeDef,
 ):
     pass
 
-
 TieringPolicyTypeDef = TypedDict(
     "TieringPolicyTypeDef",
     {
         "CoolingPeriod": int,
         "Name": TieringPolicyNameType,
     },
     total=False,
@@ -539,21 +555,19 @@
     "_OptionalDeleteBackupRequestRequestTypeDef",
     {
         "ClientRequestToken": str,
     },
     total=False,
 )
 
-
 class DeleteBackupRequestRequestTypeDef(
     _RequiredDeleteBackupRequestRequestTypeDef, _OptionalDeleteBackupRequestRequestTypeDef
 ):
     pass
 
-
 _RequiredDeleteDataRepositoryAssociationRequestRequestTypeDef = TypedDict(
     "_RequiredDeleteDataRepositoryAssociationRequestRequestTypeDef",
     {
         "AssociationId": str,
     },
 )
 _OptionalDeleteDataRepositoryAssociationRequestRequestTypeDef = TypedDict(
@@ -561,86 +575,78 @@
     {
         "ClientRequestToken": str,
         "DeleteDataInFileSystem": bool,
     },
     total=False,
 )
 
-
 class DeleteDataRepositoryAssociationRequestRequestTypeDef(
     _RequiredDeleteDataRepositoryAssociationRequestRequestTypeDef,
     _OptionalDeleteDataRepositoryAssociationRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredDeleteFileCacheRequestRequestTypeDef = TypedDict(
     "_RequiredDeleteFileCacheRequestRequestTypeDef",
     {
         "FileCacheId": str,
     },
 )
 _OptionalDeleteFileCacheRequestRequestTypeDef = TypedDict(
     "_OptionalDeleteFileCacheRequestRequestTypeDef",
     {
         "ClientRequestToken": str,
     },
     total=False,
 )
 
-
 class DeleteFileCacheRequestRequestTypeDef(
     _RequiredDeleteFileCacheRequestRequestTypeDef, _OptionalDeleteFileCacheRequestRequestTypeDef
 ):
     pass
 
-
 _RequiredDeleteSnapshotRequestRequestTypeDef = TypedDict(
     "_RequiredDeleteSnapshotRequestRequestTypeDef",
     {
         "SnapshotId": str,
     },
 )
 _OptionalDeleteSnapshotRequestRequestTypeDef = TypedDict(
     "_OptionalDeleteSnapshotRequestRequestTypeDef",
     {
         "ClientRequestToken": str,
     },
     total=False,
 )
 
-
 class DeleteSnapshotRequestRequestTypeDef(
     _RequiredDeleteSnapshotRequestRequestTypeDef, _OptionalDeleteSnapshotRequestRequestTypeDef
 ):
     pass
 
-
 _RequiredDeleteStorageVirtualMachineRequestRequestTypeDef = TypedDict(
     "_RequiredDeleteStorageVirtualMachineRequestRequestTypeDef",
     {
         "StorageVirtualMachineId": str,
     },
 )
 _OptionalDeleteStorageVirtualMachineRequestRequestTypeDef = TypedDict(
     "_OptionalDeleteStorageVirtualMachineRequestRequestTypeDef",
     {
         "ClientRequestToken": str,
     },
     total=False,
 )
 
-
 class DeleteStorageVirtualMachineRequestRequestTypeDef(
     _RequiredDeleteStorageVirtualMachineRequestRequestTypeDef,
     _OptionalDeleteStorageVirtualMachineRequestRequestTypeDef,
 ):
     pass
 
-
 DeleteVolumeOpenZFSConfigurationTypeDef = TypedDict(
     "DeleteVolumeOpenZFSConfigurationTypeDef",
     {
         "Options": Sequence[Literal["DELETE_CHILD_VOLUMES_AND_SNAPSHOTS"]],
     },
     total=False,
 )
@@ -686,22 +692,20 @@
         "ClientRequestToken": str,
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
-
 class DescribeFileSystemAliasesRequestRequestTypeDef(
     _RequiredDescribeFileSystemAliasesRequestRequestTypeDef,
     _OptionalDescribeFileSystemAliasesRequestRequestTypeDef,
 ):
     pass
 
-
 DescribeFileSystemsRequestRequestTypeDef = TypedDict(
     "DescribeFileSystemsRequestRequestTypeDef",
     {
         "FileSystemIds": Sequence[str],
         "MaxResults": int,
         "NextToken": str,
     },
@@ -746,22 +750,20 @@
     "_OptionalDisassociateFileSystemAliasesRequestRequestTypeDef",
     {
         "ClientRequestToken": str,
     },
     total=False,
 )
 
-
 class DisassociateFileSystemAliasesRequestRequestTypeDef(
     _RequiredDisassociateFileSystemAliasesRequestRequestTypeDef,
     _OptionalDisassociateFileSystemAliasesRequestRequestTypeDef,
 ):
     pass
 
-
 FileCacheFailureDetailsTypeDef = TypedDict(
     "FileCacheFailureDetailsTypeDef",
     {
         "Message": str,
     },
     total=False,
 )
@@ -776,42 +778,38 @@
     "_OptionalFileCacheNFSConfigurationTypeDef",
     {
         "DnsIps": Sequence[str],
     },
     total=False,
 )
 
-
 class FileCacheNFSConfigurationTypeDef(
     _RequiredFileCacheNFSConfigurationTypeDef, _OptionalFileCacheNFSConfigurationTypeDef
 ):
     pass
 
-
 _RequiredLustreLogConfigurationTypeDef = TypedDict(
     "_RequiredLustreLogConfigurationTypeDef",
     {
         "Level": LustreAccessAuditLogLevelType,
     },
 )
 _OptionalLustreLogConfigurationTypeDef = TypedDict(
     "_OptionalLustreLogConfigurationTypeDef",
     {
         "Destination": str,
     },
     total=False,
 )
 
-
 class LustreLogConfigurationTypeDef(
     _RequiredLustreLogConfigurationTypeDef, _OptionalLustreLogConfigurationTypeDef
 ):
     pass
 
-
 FileSystemEndpointTypeDef = TypedDict(
     "FileSystemEndpointTypeDef",
     {
         "DNSName": str,
         "IpAddresses": List[str],
     },
     total=False,
@@ -844,22 +842,20 @@
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
-
 class ListTagsForResourceRequestRequestTypeDef(
     _RequiredListTagsForResourceRequestRequestTypeDef,
     _OptionalListTagsForResourceRequestRequestTypeDef,
 ):
     pass
 
-
 OpenZFSClientConfigurationTypeDef = TypedDict(
     "OpenZFSClientConfigurationTypeDef",
     {
         "Clients": str,
         "Options": List[str],
     },
 )
@@ -883,22 +879,20 @@
     "_OptionalReleaseFileSystemNfsV3LocksRequestRequestTypeDef",
     {
         "ClientRequestToken": str,
     },
     total=False,
 )
 
-
 class ReleaseFileSystemNfsV3LocksRequestRequestTypeDef(
     _RequiredReleaseFileSystemNfsV3LocksRequestRequestTypeDef,
     _OptionalReleaseFileSystemNfsV3LocksRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredRestoreVolumeFromSnapshotRequestRequestTypeDef = TypedDict(
     "_RequiredRestoreVolumeFromSnapshotRequestRequestTypeDef",
     {
         "VolumeId": str,
         "SnapshotId": str,
     },
 )
@@ -907,21 +901,36 @@
     {
         "ClientRequestToken": str,
         "Options": Sequence[RestoreOpenZFSVolumeOptionType],
     },
     total=False,
 )
 
-
 class RestoreVolumeFromSnapshotRequestRequestTypeDef(
     _RequiredRestoreVolumeFromSnapshotRequestRequestTypeDef,
     _OptionalRestoreVolumeFromSnapshotRequestRequestTypeDef,
 ):
     pass
 
+_RequiredRetentionPeriodTypeDef = TypedDict(
+    "_RequiredRetentionPeriodTypeDef",
+    {
+        "Type": RetentionPeriodTypeType,
+    },
+)
+_OptionalRetentionPeriodTypeDef = TypedDict(
+    "_OptionalRetentionPeriodTypeDef",
+    {
+        "Value": int,
+    },
+    total=False,
+)
+
+class RetentionPeriodTypeDef(_RequiredRetentionPeriodTypeDef, _OptionalRetentionPeriodTypeDef):
+    pass
 
 SelfManagedActiveDirectoryAttributesTypeDef = TypedDict(
     "SelfManagedActiveDirectoryAttributesTypeDef",
     {
         "DomainName": str,
         "OrganizationalUnitDistinguishedName": str,
         "FileSystemAdministratorsGroup": str,
@@ -980,21 +989,19 @@
     "_OptionalUpdateSnapshotRequestRequestTypeDef",
     {
         "ClientRequestToken": str,
     },
     total=False,
 )
 
-
 class UpdateSnapshotRequestRequestTypeDef(
     _RequiredUpdateSnapshotRequestRequestTypeDef, _OptionalUpdateSnapshotRequestRequestTypeDef
 ):
     pass
 
-
 _RequiredWindowsAuditLogConfigurationTypeDef = TypedDict(
     "_RequiredWindowsAuditLogConfigurationTypeDef",
     {
         "FileAccessAuditLogLevel": WindowsAccessAuditLogLevelType,
         "FileShareAccessAuditLogLevel": WindowsAccessAuditLogLevelType,
     },
 )
@@ -1002,21 +1009,19 @@
     "_OptionalWindowsAuditLogConfigurationTypeDef",
     {
         "AuditLogDestination": str,
     },
     total=False,
 )
 
-
 class WindowsAuditLogConfigurationTypeDef(
     _RequiredWindowsAuditLogConfigurationTypeDef, _OptionalWindowsAuditLogConfigurationTypeDef
 ):
     pass
 
-
 AssociateFileSystemAliasesResponseTypeDef = TypedDict(
     "AssociateFileSystemAliasesResponseTypeDef",
     {
         "Aliases": List[AliasTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -1155,21 +1160,19 @@
     {
         "DnsIps": List[str],
         "AutoExportPolicy": AutoExportPolicyTypeDef,
     },
     total=False,
 )
 
-
 class NFSDataRepositoryConfigurationTypeDef(
     _RequiredNFSDataRepositoryConfigurationTypeDef, _OptionalNFSDataRepositoryConfigurationTypeDef
 ):
     pass
 
-
 S3DataRepositoryConfigurationTypeDef = TypedDict(
     "S3DataRepositoryConfigurationTypeDef",
     {
         "AutoImportPolicy": AutoImportPolicyTypeDef,
         "AutoExportPolicy": AutoExportPolicyTypeDef,
     },
     total=False,
@@ -1189,21 +1192,19 @@
         "KmsKeyId": str,
         "CopyTags": bool,
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
-
 class CopyBackupRequestRequestTypeDef(
     _RequiredCopyBackupRequestRequestTypeDef, _OptionalCopyBackupRequestRequestTypeDef
 ):
     pass
 
-
 CreateBackupRequestRequestTypeDef = TypedDict(
     "CreateBackupRequestRequestTypeDef",
     {
         "FileSystemId": str,
         "ClientRequestToken": str,
         "Tags": Sequence[TagTypeDef],
         "VolumeId": str,
@@ -1223,21 +1224,19 @@
     {
         "ClientRequestToken": str,
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
-
 class CreateSnapshotRequestRequestTypeDef(
     _RequiredCreateSnapshotRequestRequestTypeDef, _OptionalCreateSnapshotRequestRequestTypeDef
 ):
     pass
 
-
 DeleteFileSystemLustreConfigurationTypeDef = TypedDict(
     "DeleteFileSystemLustreConfigurationTypeDef",
     {
         "SkipFinalBackup": bool,
         "FinalBackupTags": Sequence[TagTypeDef],
     },
     total=False,
@@ -1290,14 +1289,15 @@
 )
 
 DeleteVolumeOntapConfigurationTypeDef = TypedDict(
     "DeleteVolumeOntapConfigurationTypeDef",
     {
         "SkipFinalBackup": bool,
         "FinalBackupTags": Sequence[TagTypeDef],
+        "BypassSnaplockEnterpriseRetention": bool,
     },
     total=False,
 )
 
 DeleteVolumeOntapResponseTypeDef = TypedDict(
     "DeleteVolumeOntapResponseTypeDef",
     {
@@ -1339,22 +1339,20 @@
         "ClientRequestToken": str,
         "Tags": Sequence[TagTypeDef],
         "CapacityToRelease": int,
     },
     total=False,
 )
 
-
 class CreateDataRepositoryTaskRequestRequestTypeDef(
     _RequiredCreateDataRepositoryTaskRequestRequestTypeDef,
     _OptionalCreateDataRepositoryTaskRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredCreateFileCacheLustreConfigurationTypeDef = TypedDict(
     "_RequiredCreateFileCacheLustreConfigurationTypeDef",
     {
         "PerUnitStorageThroughput": int,
         "DeploymentType": Literal["CACHE_1"],
         "MetadataConfiguration": FileCacheLustreMetadataConfigurationTypeDef,
     },
@@ -1363,22 +1361,20 @@
     "_OptionalCreateFileCacheLustreConfigurationTypeDef",
     {
         "WeeklyMaintenanceStartTime": str,
     },
     total=False,
 )
 
-
 class CreateFileCacheLustreConfigurationTypeDef(
     _RequiredCreateFileCacheLustreConfigurationTypeDef,
     _OptionalCreateFileCacheLustreConfigurationTypeDef,
 ):
     pass
 
-
 CreateFileSystemLustreConfigurationTypeDef = TypedDict(
     "CreateFileSystemLustreConfigurationTypeDef",
     {
         "WeeklyMaintenanceStartTime": str,
         "ImportPath": str,
         "ExportPath": str,
         "ImportedFileChunkSize": int,
@@ -1428,22 +1424,20 @@
         "PreferredSubnetId": str,
         "RouteTableIds": Sequence[str],
         "WeeklyMaintenanceStartTime": str,
     },
     total=False,
 )
 
-
 class CreateFileSystemOntapConfigurationTypeDef(
     _RequiredCreateFileSystemOntapConfigurationTypeDef,
     _OptionalCreateFileSystemOntapConfigurationTypeDef,
 ):
     pass
 
-
 OpenZFSFileSystemConfigurationTypeDef = TypedDict(
     "OpenZFSFileSystemConfigurationTypeDef",
     {
         "AutomaticBackupRetentionDays": int,
         "CopyTagsToBackups": bool,
         "CopyTagsToVolumes": bool,
         "DailyAutomaticBackupStartTime": str,
@@ -1495,22 +1489,20 @@
     "_OptionalCreateSvmActiveDirectoryConfigurationTypeDef",
     {
         "SelfManagedActiveDirectoryConfiguration": SelfManagedActiveDirectoryConfigurationTypeDef,
     },
     total=False,
 )
 
-
 class CreateSvmActiveDirectoryConfigurationTypeDef(
     _RequiredCreateSvmActiveDirectoryConfigurationTypeDef,
     _OptionalCreateSvmActiveDirectoryConfigurationTypeDef,
 ):
     pass
 
-
 _RequiredCreateFileSystemWindowsConfigurationTypeDef = TypedDict(
     "_RequiredCreateFileSystemWindowsConfigurationTypeDef",
     {
         "ThroughputCapacity": int,
     },
 )
 _OptionalCreateFileSystemWindowsConfigurationTypeDef = TypedDict(
@@ -1526,83 +1518,20 @@
         "CopyTagsToBackups": bool,
         "Aliases": Sequence[str],
         "AuditLogConfiguration": WindowsAuditLogCreateConfigurationTypeDef,
     },
     total=False,
 )
 
-
 class CreateFileSystemWindowsConfigurationTypeDef(
     _RequiredCreateFileSystemWindowsConfigurationTypeDef,
     _OptionalCreateFileSystemWindowsConfigurationTypeDef,
 ):
     pass
 
-
-_RequiredCreateOntapVolumeConfigurationTypeDef = TypedDict(
-    "_RequiredCreateOntapVolumeConfigurationTypeDef",
-    {
-        "SizeInMegabytes": int,
-        "StorageVirtualMachineId": str,
-    },
-)
-_OptionalCreateOntapVolumeConfigurationTypeDef = TypedDict(
-    "_OptionalCreateOntapVolumeConfigurationTypeDef",
-    {
-        "JunctionPath": str,
-        "SecurityStyle": SecurityStyleType,
-        "StorageEfficiencyEnabled": bool,
-        "TieringPolicy": TieringPolicyTypeDef,
-        "OntapVolumeType": InputOntapVolumeTypeType,
-        "SnapshotPolicy": str,
-        "CopyTagsToBackups": bool,
-    },
-    total=False,
-)
-
-
-class CreateOntapVolumeConfigurationTypeDef(
-    _RequiredCreateOntapVolumeConfigurationTypeDef, _OptionalCreateOntapVolumeConfigurationTypeDef
-):
-    pass
-
-
-OntapVolumeConfigurationTypeDef = TypedDict(
-    "OntapVolumeConfigurationTypeDef",
-    {
-        "FlexCacheEndpointType": FlexCacheEndpointTypeType,
-        "JunctionPath": str,
-        "SecurityStyle": SecurityStyleType,
-        "SizeInMegabytes": int,
-        "StorageEfficiencyEnabled": bool,
-        "StorageVirtualMachineId": str,
-        "StorageVirtualMachineRoot": bool,
-        "TieringPolicy": TieringPolicyTypeDef,
-        "UUID": str,
-        "OntapVolumeType": OntapVolumeTypeType,
-        "SnapshotPolicy": str,
-        "CopyTagsToBackups": bool,
-    },
-    total=False,
-)
-
-UpdateOntapVolumeConfigurationTypeDef = TypedDict(
-    "UpdateOntapVolumeConfigurationTypeDef",
-    {
-        "JunctionPath": str,
-        "SecurityStyle": SecurityStyleType,
-        "SizeInMegabytes": int,
-        "StorageEfficiencyEnabled": bool,
-        "TieringPolicy": TieringPolicyTypeDef,
-        "SnapshotPolicy": str,
-        "CopyTagsToBackups": bool,
-    },
-    total=False,
-)
-
 DataRepositoryConfigurationTypeDef = TypedDict(
     "DataRepositoryConfigurationTypeDef",
     {
         "Lifecycle": DataRepositoryLifecycleType,
         "ImportPath": str,
         "ExportPath": str,
         "ImportedFileChunkSize": int,
@@ -1646,21 +1575,19 @@
         "Report": CompletionReportTypeDef,
         "CapacityToRelease": int,
         "FileCacheId": str,
     },
     total=False,
 )
 
-
 class DataRepositoryTaskTypeDef(
     _RequiredDataRepositoryTaskTypeDef, _OptionalDataRepositoryTaskTypeDef
 ):
     pass
 
-
 DescribeBackupsRequestRequestTypeDef = TypedDict(
     "DescribeBackupsRequestRequestTypeDef",
     {
         "BackupIds": Sequence[str],
         "Filters": Sequence[FilterTypeDef],
         "MaxResults": int,
         "NextToken": str,
@@ -1708,22 +1635,20 @@
     "_OptionalListTagsForResourceRequestListTagsForResourcePaginateTypeDef",
     {
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-
 class ListTagsForResourceRequestListTagsForResourcePaginateTypeDef(
     _RequiredListTagsForResourceRequestListTagsForResourcePaginateTypeDef,
     _OptionalListTagsForResourceRequestListTagsForResourcePaginateTypeDef,
 ):
     pass
 
-
 DescribeSnapshotsRequestRequestTypeDef = TypedDict(
     "DescribeSnapshotsRequestRequestTypeDef",
     {
         "SnapshotIds": Sequence[str],
         "Filters": Sequence[SnapshotFilterTypeDef],
         "MaxResults": int,
         "NextToken": str,
@@ -1785,22 +1710,20 @@
     {
         "DataRepositorySubdirectories": Sequence[str],
         "NFS": FileCacheNFSConfigurationTypeDef,
     },
     total=False,
 )
 
-
 class FileCacheDataRepositoryAssociationTypeDef(
     _RequiredFileCacheDataRepositoryAssociationTypeDef,
     _OptionalFileCacheDataRepositoryAssociationTypeDef,
 ):
     pass
 
-
 FileCacheLustreConfigurationTypeDef = TypedDict(
     "FileCacheLustreConfigurationTypeDef",
     {
         "PerUnitStorageThroughput": int,
         "DeploymentType": Literal["CACHE_1"],
         "MountName": str,
         "WeeklyMaintenanceStartTime": str,
@@ -1838,14 +1761,23 @@
 OpenZFSNfsExportTypeDef = TypedDict(
     "OpenZFSNfsExportTypeDef",
     {
         "ClientConfigurations": List[OpenZFSClientConfigurationTypeDef],
     },
 )
 
+SnaplockRetentionPeriodTypeDef = TypedDict(
+    "SnaplockRetentionPeriodTypeDef",
+    {
+        "DefaultRetention": RetentionPeriodTypeDef,
+        "MinimumRetention": RetentionPeriodTypeDef,
+        "MaximumRetention": RetentionPeriodTypeDef,
+    },
+)
+
 SvmActiveDirectoryConfigurationTypeDef = TypedDict(
     "SvmActiveDirectoryConfigurationTypeDef",
     {
         "NetBiosName": str,
         "SelfManagedActiveDirectoryConfiguration": SelfManagedActiveDirectoryAttributesTypeDef,
     },
     total=False,
@@ -1899,21 +1831,19 @@
     {
         "ClientRequestToken": str,
         "LustreConfiguration": UpdateFileCacheLustreConfigurationTypeDef,
     },
     total=False,
 )
 
-
 class UpdateFileCacheRequestRequestTypeDef(
     _RequiredUpdateFileCacheRequestRequestTypeDef, _OptionalUpdateFileCacheRequestRequestTypeDef
 ):
     pass
 
-
 WindowsFileSystemConfigurationTypeDef = TypedDict(
     "WindowsFileSystemConfigurationTypeDef",
     {
         "ActiveDirectoryId": str,
         "SelfManagedActiveDirectoryConfiguration": SelfManagedActiveDirectoryAttributesTypeDef,
         "DeploymentType": WindowsDeploymentTypeType,
         "RemoteAdministrationEndpoint": str,
@@ -1947,22 +1877,20 @@
         "S3": S3DataRepositoryConfigurationTypeDef,
         "ClientRequestToken": str,
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
-
 class CreateDataRepositoryAssociationRequestRequestTypeDef(
     _RequiredCreateDataRepositoryAssociationRequestRequestTypeDef,
     _OptionalCreateDataRepositoryAssociationRequestRequestTypeDef,
 ):
     pass
 
-
 DataRepositoryAssociationTypeDef = TypedDict(
     "DataRepositoryAssociationTypeDef",
     {
         "AssociationId": str,
         "ResourceARN": str,
         "FileSystemId": str,
         "Lifecycle": DataRepositoryLifecycleType,
@@ -1994,22 +1922,20 @@
         "ClientRequestToken": str,
         "ImportedFileChunkSize": int,
         "S3": S3DataRepositoryConfigurationTypeDef,
     },
     total=False,
 )
 
-
 class UpdateDataRepositoryAssociationRequestRequestTypeDef(
     _RequiredUpdateDataRepositoryAssociationRequestRequestTypeDef,
     _OptionalUpdateDataRepositoryAssociationRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredDeleteFileSystemRequestRequestTypeDef = TypedDict(
     "_RequiredDeleteFileSystemRequestRequestTypeDef",
     {
         "FileSystemId": str,
     },
 )
 _OptionalDeleteFileSystemRequestRequestTypeDef = TypedDict(
@@ -2019,21 +1945,19 @@
         "WindowsConfiguration": DeleteFileSystemWindowsConfigurationTypeDef,
         "LustreConfiguration": DeleteFileSystemLustreConfigurationTypeDef,
         "OpenZFSConfiguration": DeleteFileSystemOpenZFSConfigurationTypeDef,
     },
     total=False,
 )
 
-
 class DeleteFileSystemRequestRequestTypeDef(
     _RequiredDeleteFileSystemRequestRequestTypeDef, _OptionalDeleteFileSystemRequestRequestTypeDef
 ):
     pass
 
-
 DeleteFileSystemResponseTypeDef = TypedDict(
     "DeleteFileSystemResponseTypeDef",
     {
         "FileSystemId": str,
         "Lifecycle": FileSystemLifecycleType,
         "WindowsResponse": DeleteFileSystemWindowsResponseTypeDef,
         "LustreResponse": DeleteFileSystemLustreResponseTypeDef,
@@ -2054,21 +1978,19 @@
         "ClientRequestToken": str,
         "OntapConfiguration": DeleteVolumeOntapConfigurationTypeDef,
         "OpenZFSConfiguration": DeleteVolumeOpenZFSConfigurationTypeDef,
     },
     total=False,
 )
 
-
 class DeleteVolumeRequestRequestTypeDef(
     _RequiredDeleteVolumeRequestRequestTypeDef, _OptionalDeleteVolumeRequestRequestTypeDef
 ):
     pass
 
-
 DeleteVolumeResponseTypeDef = TypedDict(
     "DeleteVolumeResponseTypeDef",
     {
         "VolumeId": str,
         "Lifecycle": VolumeLifecycleType,
         "OntapResponse": DeleteVolumeOntapResponseTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
@@ -2090,47 +2012,20 @@
         "SvmAdminPassword": str,
         "Tags": Sequence[TagTypeDef],
         "RootVolumeSecurityStyle": StorageVirtualMachineRootVolumeSecurityStyleType,
     },
     total=False,
 )
 
-
 class CreateStorageVirtualMachineRequestRequestTypeDef(
     _RequiredCreateStorageVirtualMachineRequestRequestTypeDef,
     _OptionalCreateStorageVirtualMachineRequestRequestTypeDef,
 ):
     pass
 
-
-_RequiredCreateVolumeFromBackupRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateVolumeFromBackupRequestRequestTypeDef",
-    {
-        "BackupId": str,
-        "Name": str,
-    },
-)
-_OptionalCreateVolumeFromBackupRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateVolumeFromBackupRequestRequestTypeDef",
-    {
-        "ClientRequestToken": str,
-        "OntapConfiguration": CreateOntapVolumeConfigurationTypeDef,
-        "Tags": Sequence[TagTypeDef],
-    },
-    total=False,
-)
-
-
-class CreateVolumeFromBackupRequestRequestTypeDef(
-    _RequiredCreateVolumeFromBackupRequestRequestTypeDef,
-    _OptionalCreateVolumeFromBackupRequestRequestTypeDef,
-):
-    pass
-
-
 LustreFileSystemConfigurationTypeDef = TypedDict(
     "LustreFileSystemConfigurationTypeDef",
     {
         "WeeklyMaintenanceStartTime": str,
         "DataRepositoryConfiguration": DataRepositoryConfigurationTypeDef,
         "DeploymentType": LustreDeploymentTypeType,
         "PerUnitStorageThroughput": int,
@@ -2182,21 +2077,19 @@
         "KmsKeyId": str,
         "LustreConfiguration": CreateFileCacheLustreConfigurationTypeDef,
         "DataRepositoryAssociations": Sequence[FileCacheDataRepositoryAssociationTypeDef],
     },
     total=False,
 )
 
-
 class CreateFileCacheRequestRequestTypeDef(
     _RequiredCreateFileCacheRequestRequestTypeDef, _OptionalCreateFileCacheRequestRequestTypeDef
 ):
     pass
 
-
 FileCacheCreatingTypeDef = TypedDict(
     "FileCacheCreatingTypeDef",
     {
         "OwnerId": str,
         "CreationTime": datetime,
         "FileCacheId": str,
         "FileCacheType": Literal["LUSTRE"],
@@ -2302,22 +2195,20 @@
         "ReadOnly": bool,
         "NfsExports": Sequence[OpenZFSNfsExportTypeDef],
         "UserAndGroupQuotas": Sequence[OpenZFSUserOrGroupQuotaTypeDef],
     },
     total=False,
 )
 
-
 class CreateOpenZFSVolumeConfigurationTypeDef(
     _RequiredCreateOpenZFSVolumeConfigurationTypeDef,
     _OptionalCreateOpenZFSVolumeConfigurationTypeDef,
 ):
     pass
 
-
 OpenZFSCreateRootVolumeConfigurationTypeDef = TypedDict(
     "OpenZFSCreateRootVolumeConfigurationTypeDef",
     {
         "RecordSizeKiB": int,
         "DataCompressionType": OpenZFSDataCompressionTypeType,
         "NfsExports": Sequence[OpenZFSNfsExportTypeDef],
         "UserAndGroupQuotas": Sequence[OpenZFSUserOrGroupQuotaTypeDef],
@@ -2358,14 +2249,62 @@
         "NfsExports": Sequence[OpenZFSNfsExportTypeDef],
         "UserAndGroupQuotas": Sequence[OpenZFSUserOrGroupQuotaTypeDef],
         "ReadOnly": bool,
     },
     total=False,
 )
 
+_RequiredCreateSnaplockConfigurationTypeDef = TypedDict(
+    "_RequiredCreateSnaplockConfigurationTypeDef",
+    {
+        "SnaplockType": SnaplockTypeType,
+    },
+)
+_OptionalCreateSnaplockConfigurationTypeDef = TypedDict(
+    "_OptionalCreateSnaplockConfigurationTypeDef",
+    {
+        "AuditLogVolume": bool,
+        "AutocommitPeriod": AutocommitPeriodTypeDef,
+        "PrivilegedDelete": PrivilegedDeleteType,
+        "RetentionPeriod": SnaplockRetentionPeriodTypeDef,
+        "VolumeAppendModeEnabled": bool,
+    },
+    total=False,
+)
+
+class CreateSnaplockConfigurationTypeDef(
+    _RequiredCreateSnaplockConfigurationTypeDef, _OptionalCreateSnaplockConfigurationTypeDef
+):
+    pass
+
+SnaplockConfigurationTypeDef = TypedDict(
+    "SnaplockConfigurationTypeDef",
+    {
+        "AuditLogVolume": bool,
+        "AutocommitPeriod": AutocommitPeriodTypeDef,
+        "PrivilegedDelete": PrivilegedDeleteType,
+        "RetentionPeriod": SnaplockRetentionPeriodTypeDef,
+        "SnaplockType": SnaplockTypeType,
+        "VolumeAppendModeEnabled": bool,
+    },
+    total=False,
+)
+
+UpdateSnaplockConfigurationTypeDef = TypedDict(
+    "UpdateSnaplockConfigurationTypeDef",
+    {
+        "AuditLogVolume": bool,
+        "AutocommitPeriod": AutocommitPeriodTypeDef,
+        "PrivilegedDelete": PrivilegedDeleteType,
+        "RetentionPeriod": SnaplockRetentionPeriodTypeDef,
+        "VolumeAppendModeEnabled": bool,
+    },
+    total=False,
+)
+
 _RequiredUpdateFileSystemRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateFileSystemRequestRequestTypeDef",
     {
         "FileSystemId": str,
     },
 )
 _OptionalUpdateFileSystemRequestRequestTypeDef = TypedDict(
@@ -2377,21 +2316,19 @@
         "LustreConfiguration": UpdateFileSystemLustreConfigurationTypeDef,
         "OntapConfiguration": UpdateFileSystemOntapConfigurationTypeDef,
         "OpenZFSConfiguration": UpdateFileSystemOpenZFSConfigurationTypeDef,
     },
     total=False,
 )
 
-
 class UpdateFileSystemRequestRequestTypeDef(
     _RequiredUpdateFileSystemRequestRequestTypeDef, _OptionalUpdateFileSystemRequestRequestTypeDef
 ):
     pass
 
-
 _RequiredUpdateStorageVirtualMachineRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateStorageVirtualMachineRequestRequestTypeDef",
     {
         "StorageVirtualMachineId": str,
     },
 )
 _OptionalUpdateStorageVirtualMachineRequestRequestTypeDef = TypedDict(
@@ -2400,22 +2337,20 @@
         "ActiveDirectoryConfiguration": UpdateSvmActiveDirectoryConfigurationTypeDef,
         "ClientRequestToken": str,
         "SvmAdminPassword": str,
     },
     total=False,
 )
 
-
 class UpdateStorageVirtualMachineRequestRequestTypeDef(
     _RequiredUpdateStorageVirtualMachineRequestRequestTypeDef,
     _OptionalUpdateStorageVirtualMachineRequestRequestTypeDef,
 ):
     pass
 
-
 StorageVirtualMachineTypeDef = TypedDict(
     "StorageVirtualMachineTypeDef",
     {
         "ActiveDirectoryConfiguration": SvmActiveDirectoryConfigurationTypeDef,
         "CreationTime": datetime,
         "Endpoints": SvmEndpointsTypeDef,
         "FileSystemId": str,
@@ -2498,47 +2433,22 @@
         "NetworkInterfaceIds": List[str],
         "DNSName": str,
         "KmsKeyId": str,
         "ResourceARN": str,
         "Tags": List[TagTypeDef],
         "WindowsConfiguration": WindowsFileSystemConfigurationTypeDef,
         "LustreConfiguration": LustreFileSystemConfigurationTypeDef,
-        "AdministrativeActions": List["AdministrativeActionTypeDef"],
+        "AdministrativeActions": List[Dict[str, Any]],
         "OntapConfiguration": OntapFileSystemConfigurationTypeDef,
         "FileSystemTypeVersion": str,
         "OpenZFSConfiguration": OpenZFSFileSystemConfigurationTypeDef,
     },
     total=False,
 )
 
-_RequiredCreateVolumeRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateVolumeRequestRequestTypeDef",
-    {
-        "VolumeType": VolumeTypeType,
-        "Name": str,
-    },
-)
-_OptionalCreateVolumeRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateVolumeRequestRequestTypeDef",
-    {
-        "ClientRequestToken": str,
-        "OntapConfiguration": CreateOntapVolumeConfigurationTypeDef,
-        "Tags": Sequence[TagTypeDef],
-        "OpenZFSConfiguration": CreateOpenZFSVolumeConfigurationTypeDef,
-    },
-    total=False,
-)
-
-
-class CreateVolumeRequestRequestTypeDef(
-    _RequiredCreateVolumeRequestRequestTypeDef, _OptionalCreateVolumeRequestRequestTypeDef
-):
-    pass
-
-
 _RequiredCreateFileSystemOpenZFSConfigurationTypeDef = TypedDict(
     "_RequiredCreateFileSystemOpenZFSConfigurationTypeDef",
     {
         "DeploymentType": OpenZFSDeploymentTypeType,
         "ThroughputCapacity": int,
     },
 )
@@ -2552,65 +2462,82 @@
         "WeeklyMaintenanceStartTime": str,
         "DiskIopsConfiguration": DiskIopsConfigurationTypeDef,
         "RootVolumeConfiguration": OpenZFSCreateRootVolumeConfigurationTypeDef,
     },
     total=False,
 )
 
-
 class CreateFileSystemOpenZFSConfigurationTypeDef(
     _RequiredCreateFileSystemOpenZFSConfigurationTypeDef,
     _OptionalCreateFileSystemOpenZFSConfigurationTypeDef,
 ):
     pass
 
-
-VolumeTypeDef = TypedDict(
-    "VolumeTypeDef",
+_RequiredCreateOntapVolumeConfigurationTypeDef = TypedDict(
+    "_RequiredCreateOntapVolumeConfigurationTypeDef",
     {
-        "CreationTime": datetime,
-        "FileSystemId": str,
-        "Lifecycle": VolumeLifecycleType,
-        "Name": str,
-        "OntapConfiguration": OntapVolumeConfigurationTypeDef,
-        "ResourceARN": str,
-        "Tags": List[TagTypeDef],
-        "VolumeId": str,
-        "VolumeType": VolumeTypeType,
-        "LifecycleTransitionReason": LifecycleTransitionReasonTypeDef,
-        "AdministrativeActions": List[Dict[str, Any]],
-        "OpenZFSConfiguration": OpenZFSVolumeConfigurationTypeDef,
+        "SizeInMegabytes": int,
+        "StorageVirtualMachineId": str,
+    },
+)
+_OptionalCreateOntapVolumeConfigurationTypeDef = TypedDict(
+    "_OptionalCreateOntapVolumeConfigurationTypeDef",
+    {
+        "JunctionPath": str,
+        "SecurityStyle": SecurityStyleType,
+        "StorageEfficiencyEnabled": bool,
+        "TieringPolicy": TieringPolicyTypeDef,
+        "OntapVolumeType": InputOntapVolumeTypeType,
+        "SnapshotPolicy": str,
+        "CopyTagsToBackups": bool,
+        "SnaplockConfiguration": CreateSnaplockConfigurationTypeDef,
     },
     total=False,
 )
 
-_RequiredUpdateVolumeRequestRequestTypeDef = TypedDict(
-    "_RequiredUpdateVolumeRequestRequestTypeDef",
+class CreateOntapVolumeConfigurationTypeDef(
+    _RequiredCreateOntapVolumeConfigurationTypeDef, _OptionalCreateOntapVolumeConfigurationTypeDef
+):
+    pass
+
+OntapVolumeConfigurationTypeDef = TypedDict(
+    "OntapVolumeConfigurationTypeDef",
     {
-        "VolumeId": str,
+        "FlexCacheEndpointType": FlexCacheEndpointTypeType,
+        "JunctionPath": str,
+        "SecurityStyle": SecurityStyleType,
+        "SizeInMegabytes": int,
+        "StorageEfficiencyEnabled": bool,
+        "StorageVirtualMachineId": str,
+        "StorageVirtualMachineRoot": bool,
+        "TieringPolicy": TieringPolicyTypeDef,
+        "UUID": str,
+        "OntapVolumeType": OntapVolumeTypeType,
+        "SnapshotPolicy": str,
+        "CopyTagsToBackups": bool,
+        "SnaplockConfiguration": SnaplockConfigurationTypeDef,
     },
+    total=False,
 )
-_OptionalUpdateVolumeRequestRequestTypeDef = TypedDict(
-    "_OptionalUpdateVolumeRequestRequestTypeDef",
+
+UpdateOntapVolumeConfigurationTypeDef = TypedDict(
+    "UpdateOntapVolumeConfigurationTypeDef",
     {
-        "ClientRequestToken": str,
-        "OntapConfiguration": UpdateOntapVolumeConfigurationTypeDef,
-        "Name": str,
-        "OpenZFSConfiguration": UpdateOpenZFSVolumeConfigurationTypeDef,
+        "JunctionPath": str,
+        "SecurityStyle": SecurityStyleType,
+        "SizeInMegabytes": int,
+        "StorageEfficiencyEnabled": bool,
+        "TieringPolicy": TieringPolicyTypeDef,
+        "SnapshotPolicy": str,
+        "CopyTagsToBackups": bool,
+        "SnaplockConfiguration": UpdateSnaplockConfigurationTypeDef,
     },
     total=False,
 )
 
-
-class UpdateVolumeRequestRequestTypeDef(
-    _RequiredUpdateVolumeRequestRequestTypeDef, _OptionalUpdateVolumeRequestRequestTypeDef
-):
-    pass
-
-
 CreateStorageVirtualMachineResponseTypeDef = TypedDict(
     "CreateStorageVirtualMachineResponseTypeDef",
     {
         "StorageVirtualMachine": StorageVirtualMachineTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -2652,22 +2579,20 @@
         "FileSystemTypeVersion": str,
         "OpenZFSConfiguration": CreateFileSystemOpenZFSConfigurationTypeDef,
         "StorageCapacity": int,
     },
     total=False,
 )
 
-
 class CreateFileSystemFromBackupRequestRequestTypeDef(
     _RequiredCreateFileSystemFromBackupRequestRequestTypeDef,
     _OptionalCreateFileSystemFromBackupRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredCreateFileSystemRequestRequestTypeDef = TypedDict(
     "_RequiredCreateFileSystemRequestRequestTypeDef",
     {
         "FileSystemType": FileSystemTypeType,
         "StorageCapacity": int,
         "SubnetIds": Sequence[str],
     },
@@ -2685,20 +2610,105 @@
         "OntapConfiguration": CreateFileSystemOntapConfigurationTypeDef,
         "FileSystemTypeVersion": str,
         "OpenZFSConfiguration": CreateFileSystemOpenZFSConfigurationTypeDef,
     },
     total=False,
 )
 
-
 class CreateFileSystemRequestRequestTypeDef(
     _RequiredCreateFileSystemRequestRequestTypeDef, _OptionalCreateFileSystemRequestRequestTypeDef
 ):
     pass
 
+_RequiredCreateVolumeFromBackupRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateVolumeFromBackupRequestRequestTypeDef",
+    {
+        "BackupId": str,
+        "Name": str,
+    },
+)
+_OptionalCreateVolumeFromBackupRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateVolumeFromBackupRequestRequestTypeDef",
+    {
+        "ClientRequestToken": str,
+        "OntapConfiguration": CreateOntapVolumeConfigurationTypeDef,
+        "Tags": Sequence[TagTypeDef],
+    },
+    total=False,
+)
+
+class CreateVolumeFromBackupRequestRequestTypeDef(
+    _RequiredCreateVolumeFromBackupRequestRequestTypeDef,
+    _OptionalCreateVolumeFromBackupRequestRequestTypeDef,
+):
+    pass
+
+_RequiredCreateVolumeRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateVolumeRequestRequestTypeDef",
+    {
+        "VolumeType": VolumeTypeType,
+        "Name": str,
+    },
+)
+_OptionalCreateVolumeRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateVolumeRequestRequestTypeDef",
+    {
+        "ClientRequestToken": str,
+        "OntapConfiguration": CreateOntapVolumeConfigurationTypeDef,
+        "Tags": Sequence[TagTypeDef],
+        "OpenZFSConfiguration": CreateOpenZFSVolumeConfigurationTypeDef,
+    },
+    total=False,
+)
+
+class CreateVolumeRequestRequestTypeDef(
+    _RequiredCreateVolumeRequestRequestTypeDef, _OptionalCreateVolumeRequestRequestTypeDef
+):
+    pass
+
+VolumeTypeDef = TypedDict(
+    "VolumeTypeDef",
+    {
+        "CreationTime": datetime,
+        "FileSystemId": str,
+        "Lifecycle": VolumeLifecycleType,
+        "Name": str,
+        "OntapConfiguration": OntapVolumeConfigurationTypeDef,
+        "ResourceARN": str,
+        "Tags": List[TagTypeDef],
+        "VolumeId": str,
+        "VolumeType": VolumeTypeType,
+        "LifecycleTransitionReason": LifecycleTransitionReasonTypeDef,
+        "AdministrativeActions": List["AdministrativeActionTypeDef"],
+        "OpenZFSConfiguration": OpenZFSVolumeConfigurationTypeDef,
+    },
+    total=False,
+)
+
+_RequiredUpdateVolumeRequestRequestTypeDef = TypedDict(
+    "_RequiredUpdateVolumeRequestRequestTypeDef",
+    {
+        "VolumeId": str,
+    },
+)
+_OptionalUpdateVolumeRequestRequestTypeDef = TypedDict(
+    "_OptionalUpdateVolumeRequestRequestTypeDef",
+    {
+        "ClientRequestToken": str,
+        "OntapConfiguration": UpdateOntapVolumeConfigurationTypeDef,
+        "Name": str,
+        "OpenZFSConfiguration": UpdateOpenZFSVolumeConfigurationTypeDef,
+    },
+    total=False,
+)
+
+class UpdateVolumeRequestRequestTypeDef(
+    _RequiredUpdateVolumeRequestRequestTypeDef, _OptionalUpdateVolumeRequestRequestTypeDef
+):
+    pass
 
 AdministrativeActionTypeDef = TypedDict(
     "AdministrativeActionTypeDef",
     {
         "AdministrativeActionType": AdministrativeActionTypeType,
         "ProgressPercent": int,
         "RequestTime": datetime,
@@ -2735,19 +2745,17 @@
         "SourceBackupRegion": str,
         "ResourceType": ResourceTypeType,
         "Volume": VolumeTypeDef,
     },
     total=False,
 )
 
-
 class BackupTypeDef(_RequiredBackupTypeDef, _OptionalBackupTypeDef):
     pass
 
-
 CreateVolumeFromBackupResponseTypeDef = TypedDict(
     "CreateVolumeFromBackupResponseTypeDef",
     {
         "Volume": VolumeTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `types-aiobotocore-fsx-2.5.2.post3/types_aiobotocore_fsx/type_defs.pyi` & `types-aiobotocore-fsx-2.5.4/types_aiobotocore_fsx/type_defs.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 import sys
 from datetime import datetime
 from typing import Any, Dict, List, Sequence
 
 from .literals import (
     AdministrativeActionTypeType,
     AliasLifecycleType,
+    AutocommitPeriodTypeType,
     AutoImportPolicyTypeType,
     BackupLifecycleType,
     BackupTypeType,
     DataCompressionTypeType,
     DataRepositoryLifecycleType,
     DataRepositoryTaskFilterNameType,
     DataRepositoryTaskLifecycleType,
@@ -40,17 +41,20 @@
     LustreDeploymentTypeType,
     OntapDeploymentTypeType,
     OntapVolumeTypeType,
     OpenZFSCopyStrategyType,
     OpenZFSDataCompressionTypeType,
     OpenZFSDeploymentTypeType,
     OpenZFSQuotaTypeType,
+    PrivilegedDeleteType,
     ResourceTypeType,
     RestoreOpenZFSVolumeOptionType,
+    RetentionPeriodTypeType,
     SecurityStyleType,
+    SnaplockTypeType,
     SnapshotFilterNameType,
     SnapshotLifecycleType,
     StatusType,
     StorageTypeType,
     StorageVirtualMachineLifecycleType,
     StorageVirtualMachineRootVolumeSecurityStyleType,
     StorageVirtualMachineSubtypeType,
@@ -67,22 +71,24 @@
 else:
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
+
 __all__ = (
     "ActiveDirectoryBackupAttributesTypeDef",
     "AdministrativeActionFailureDetailsTypeDef",
     "AliasTypeDef",
     "AssociateFileSystemAliasesRequestRequestTypeDef",
     "ResponseMetadataTypeDef",
     "AutoExportPolicyTypeDef",
     "AutoImportPolicyTypeDef",
+    "AutocommitPeriodTypeDef",
     "BackupFailureDetailsTypeDef",
     "TagTypeDef",
     "CancelDataRepositoryTaskRequestRequestTypeDef",
     "CompletionReportTypeDef",
     "FileCacheLustreMetadataConfigurationTypeDef",
     "LustreLogCreateConfigurationTypeDef",
     "LustreRootSquashConfigurationTypeDef",
@@ -118,14 +124,15 @@
     "FileSystemFailureDetailsTypeDef",
     "LifecycleTransitionReasonTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
     "OpenZFSClientConfigurationTypeDef",
     "OpenZFSOriginSnapshotConfigurationTypeDef",
     "ReleaseFileSystemNfsV3LocksRequestRequestTypeDef",
     "RestoreVolumeFromSnapshotRequestRequestTypeDef",
+    "RetentionPeriodTypeDef",
     "SelfManagedActiveDirectoryAttributesTypeDef",
     "SelfManagedActiveDirectoryConfigurationUpdatesTypeDef",
     "SvmEndpointTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateFileCacheLustreConfigurationTypeDef",
     "UpdateSnapshotRequestRequestTypeDef",
     "WindowsAuditLogConfigurationTypeDef",
@@ -165,17 +172,14 @@
     "UpdateFileSystemLustreConfigurationTypeDef",
     "CreateFileSystemOntapConfigurationTypeDef",
     "OpenZFSFileSystemConfigurationTypeDef",
     "UpdateFileSystemOntapConfigurationTypeDef",
     "UpdateFileSystemOpenZFSConfigurationTypeDef",
     "CreateSvmActiveDirectoryConfigurationTypeDef",
     "CreateFileSystemWindowsConfigurationTypeDef",
-    "CreateOntapVolumeConfigurationTypeDef",
-    "OntapVolumeConfigurationTypeDef",
-    "UpdateOntapVolumeConfigurationTypeDef",
     "DataRepositoryConfigurationTypeDef",
     "DescribeDataRepositoryTasksRequestRequestTypeDef",
     "DataRepositoryTaskTypeDef",
     "DescribeBackupsRequestRequestTypeDef",
     "DescribeDataRepositoryAssociationsRequestRequestTypeDef",
     "DescribeBackupsRequestDescribeBackupsPaginateTypeDef",
     "DescribeFileSystemsRequestDescribeFileSystemsPaginateTypeDef",
@@ -186,62 +190,69 @@
     "DescribeVolumesRequestDescribeVolumesPaginateTypeDef",
     "DescribeVolumesRequestRequestTypeDef",
     "FileCacheDataRepositoryAssociationTypeDef",
     "FileCacheLustreConfigurationTypeDef",
     "FileSystemEndpointsTypeDef",
     "SnapshotTypeDef",
     "OpenZFSNfsExportTypeDef",
+    "SnaplockRetentionPeriodTypeDef",
     "SvmActiveDirectoryConfigurationTypeDef",
     "UpdateFileSystemWindowsConfigurationTypeDef",
     "UpdateSvmActiveDirectoryConfigurationTypeDef",
     "SvmEndpointsTypeDef",
     "UpdateFileCacheRequestRequestTypeDef",
     "WindowsFileSystemConfigurationTypeDef",
     "CreateDataRepositoryAssociationRequestRequestTypeDef",
     "DataRepositoryAssociationTypeDef",
     "UpdateDataRepositoryAssociationRequestRequestTypeDef",
     "DeleteFileSystemRequestRequestTypeDef",
     "DeleteFileSystemResponseTypeDef",
     "DeleteVolumeRequestRequestTypeDef",
     "DeleteVolumeResponseTypeDef",
     "CreateStorageVirtualMachineRequestRequestTypeDef",
-    "CreateVolumeFromBackupRequestRequestTypeDef",
     "LustreFileSystemConfigurationTypeDef",
     "CreateDataRepositoryTaskResponseTypeDef",
     "DescribeDataRepositoryTasksResponseTypeDef",
     "CreateFileCacheRequestRequestTypeDef",
     "FileCacheCreatingTypeDef",
     "FileCacheTypeDef",
     "OntapFileSystemConfigurationTypeDef",
     "CreateSnapshotResponseTypeDef",
     "DescribeSnapshotsResponseTypeDef",
     "UpdateSnapshotResponseTypeDef",
     "CreateOpenZFSVolumeConfigurationTypeDef",
     "OpenZFSCreateRootVolumeConfigurationTypeDef",
     "OpenZFSVolumeConfigurationTypeDef",
     "UpdateOpenZFSVolumeConfigurationTypeDef",
+    "CreateSnaplockConfigurationTypeDef",
+    "SnaplockConfigurationTypeDef",
+    "UpdateSnaplockConfigurationTypeDef",
     "UpdateFileSystemRequestRequestTypeDef",
     "UpdateStorageVirtualMachineRequestRequestTypeDef",
     "StorageVirtualMachineTypeDef",
     "CreateDataRepositoryAssociationResponseTypeDef",
     "DescribeDataRepositoryAssociationsResponseTypeDef",
     "UpdateDataRepositoryAssociationResponseTypeDef",
     "CreateFileCacheResponseTypeDef",
     "DescribeFileCachesResponseTypeDef",
     "UpdateFileCacheResponseTypeDef",
     "FileSystemTypeDef",
-    "CreateVolumeRequestRequestTypeDef",
     "CreateFileSystemOpenZFSConfigurationTypeDef",
-    "VolumeTypeDef",
-    "UpdateVolumeRequestRequestTypeDef",
+    "CreateOntapVolumeConfigurationTypeDef",
+    "OntapVolumeConfigurationTypeDef",
+    "UpdateOntapVolumeConfigurationTypeDef",
     "CreateStorageVirtualMachineResponseTypeDef",
     "DescribeStorageVirtualMachinesResponseTypeDef",
     "UpdateStorageVirtualMachineResponseTypeDef",
     "CreateFileSystemFromBackupRequestRequestTypeDef",
     "CreateFileSystemRequestRequestTypeDef",
+    "CreateVolumeFromBackupRequestRequestTypeDef",
+    "CreateVolumeRequestRequestTypeDef",
+    "VolumeTypeDef",
+    "UpdateVolumeRequestRequestTypeDef",
     "AdministrativeActionTypeDef",
     "BackupTypeDef",
     "CreateVolumeFromBackupResponseTypeDef",
     "CreateVolumeResponseTypeDef",
     "DescribeVolumesResponseTypeDef",
     "UpdateVolumeResponseTypeDef",
     "CopyBackupResponseTypeDef",
@@ -287,20 +298,22 @@
     "_OptionalAssociateFileSystemAliasesRequestRequestTypeDef",
     {
         "ClientRequestToken": str,
     },
     total=False,
 )
 
+
 class AssociateFileSystemAliasesRequestRequestTypeDef(
     _RequiredAssociateFileSystemAliasesRequestRequestTypeDef,
     _OptionalAssociateFileSystemAliasesRequestRequestTypeDef,
 ):
     pass
 
+
 ResponseMetadataTypeDef = TypedDict(
     "ResponseMetadataTypeDef",
     {
         "RequestId": str,
         "HostId": str,
         "HTTPStatusCode": int,
         "HTTPHeaders": Dict[str, str],
@@ -320,14 +333,33 @@
     "AutoImportPolicyTypeDef",
     {
         "Events": Sequence[EventTypeType],
     },
     total=False,
 )
 
+_RequiredAutocommitPeriodTypeDef = TypedDict(
+    "_RequiredAutocommitPeriodTypeDef",
+    {
+        "Type": AutocommitPeriodTypeType,
+    },
+)
+_OptionalAutocommitPeriodTypeDef = TypedDict(
+    "_OptionalAutocommitPeriodTypeDef",
+    {
+        "Value": int,
+    },
+    total=False,
+)
+
+
+class AutocommitPeriodTypeDef(_RequiredAutocommitPeriodTypeDef, _OptionalAutocommitPeriodTypeDef):
+    pass
+
+
 BackupFailureDetailsTypeDef = TypedDict(
     "BackupFailureDetailsTypeDef",
     {
         "Message": str,
     },
     total=False,
 )
@@ -359,17 +391,19 @@
         "Path": str,
         "Format": Literal["REPORT_CSV_20191124"],
         "Scope": Literal["FAILED_FILES_ONLY"],
     },
     total=False,
 )
 
+
 class CompletionReportTypeDef(_RequiredCompletionReportTypeDef, _OptionalCompletionReportTypeDef):
     pass
 
+
 FileCacheLustreMetadataConfigurationTypeDef = TypedDict(
     "FileCacheLustreMetadataConfigurationTypeDef",
     {
         "StorageCapacity": int,
     },
 )
 
@@ -383,19 +417,21 @@
     "_OptionalLustreLogCreateConfigurationTypeDef",
     {
         "Destination": str,
     },
     total=False,
 )
 
+
 class LustreLogCreateConfigurationTypeDef(
     _RequiredLustreLogCreateConfigurationTypeDef, _OptionalLustreLogCreateConfigurationTypeDef
 ):
     pass
 
+
 LustreRootSquashConfigurationTypeDef = TypedDict(
     "LustreRootSquashConfigurationTypeDef",
     {
         "RootSquash": str,
         "NoSquashNids": List[str],
     },
     total=False,
@@ -424,20 +460,22 @@
     {
         "OrganizationalUnitDistinguishedName": str,
         "FileSystemAdministratorsGroup": str,
     },
     total=False,
 )
 
+
 class SelfManagedActiveDirectoryConfigurationTypeDef(
     _RequiredSelfManagedActiveDirectoryConfigurationTypeDef,
     _OptionalSelfManagedActiveDirectoryConfigurationTypeDef,
 ):
     pass
 
+
 _RequiredWindowsAuditLogCreateConfigurationTypeDef = TypedDict(
     "_RequiredWindowsAuditLogCreateConfigurationTypeDef",
     {
         "FileAccessAuditLogLevel": WindowsAccessAuditLogLevelType,
         "FileShareAccessAuditLogLevel": WindowsAccessAuditLogLevelType,
     },
 )
@@ -445,20 +483,22 @@
     "_OptionalWindowsAuditLogCreateConfigurationTypeDef",
     {
         "AuditLogDestination": str,
     },
     total=False,
 )
 
+
 class WindowsAuditLogCreateConfigurationTypeDef(
     _RequiredWindowsAuditLogCreateConfigurationTypeDef,
     _OptionalWindowsAuditLogCreateConfigurationTypeDef,
 ):
     pass
 
+
 TieringPolicyTypeDef = TypedDict(
     "TieringPolicyTypeDef",
     {
         "CoolingPeriod": int,
         "Name": TieringPolicyNameType,
     },
     total=False,
@@ -528,19 +568,21 @@
     "_OptionalDeleteBackupRequestRequestTypeDef",
     {
         "ClientRequestToken": str,
     },
     total=False,
 )
 
+
 class DeleteBackupRequestRequestTypeDef(
     _RequiredDeleteBackupRequestRequestTypeDef, _OptionalDeleteBackupRequestRequestTypeDef
 ):
     pass
 
+
 _RequiredDeleteDataRepositoryAssociationRequestRequestTypeDef = TypedDict(
     "_RequiredDeleteDataRepositoryAssociationRequestRequestTypeDef",
     {
         "AssociationId": str,
     },
 )
 _OptionalDeleteDataRepositoryAssociationRequestRequestTypeDef = TypedDict(
@@ -548,78 +590,86 @@
     {
         "ClientRequestToken": str,
         "DeleteDataInFileSystem": bool,
     },
     total=False,
 )
 
+
 class DeleteDataRepositoryAssociationRequestRequestTypeDef(
     _RequiredDeleteDataRepositoryAssociationRequestRequestTypeDef,
     _OptionalDeleteDataRepositoryAssociationRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredDeleteFileCacheRequestRequestTypeDef = TypedDict(
     "_RequiredDeleteFileCacheRequestRequestTypeDef",
     {
         "FileCacheId": str,
     },
 )
 _OptionalDeleteFileCacheRequestRequestTypeDef = TypedDict(
     "_OptionalDeleteFileCacheRequestRequestTypeDef",
     {
         "ClientRequestToken": str,
     },
     total=False,
 )
 
+
 class DeleteFileCacheRequestRequestTypeDef(
     _RequiredDeleteFileCacheRequestRequestTypeDef, _OptionalDeleteFileCacheRequestRequestTypeDef
 ):
     pass
 
+
 _RequiredDeleteSnapshotRequestRequestTypeDef = TypedDict(
     "_RequiredDeleteSnapshotRequestRequestTypeDef",
     {
         "SnapshotId": str,
     },
 )
 _OptionalDeleteSnapshotRequestRequestTypeDef = TypedDict(
     "_OptionalDeleteSnapshotRequestRequestTypeDef",
     {
         "ClientRequestToken": str,
     },
     total=False,
 )
 
+
 class DeleteSnapshotRequestRequestTypeDef(
     _RequiredDeleteSnapshotRequestRequestTypeDef, _OptionalDeleteSnapshotRequestRequestTypeDef
 ):
     pass
 
+
 _RequiredDeleteStorageVirtualMachineRequestRequestTypeDef = TypedDict(
     "_RequiredDeleteStorageVirtualMachineRequestRequestTypeDef",
     {
         "StorageVirtualMachineId": str,
     },
 )
 _OptionalDeleteStorageVirtualMachineRequestRequestTypeDef = TypedDict(
     "_OptionalDeleteStorageVirtualMachineRequestRequestTypeDef",
     {
         "ClientRequestToken": str,
     },
     total=False,
 )
 
+
 class DeleteStorageVirtualMachineRequestRequestTypeDef(
     _RequiredDeleteStorageVirtualMachineRequestRequestTypeDef,
     _OptionalDeleteStorageVirtualMachineRequestRequestTypeDef,
 ):
     pass
 
+
 DeleteVolumeOpenZFSConfigurationTypeDef = TypedDict(
     "DeleteVolumeOpenZFSConfigurationTypeDef",
     {
         "Options": Sequence[Literal["DELETE_CHILD_VOLUMES_AND_SNAPSHOTS"]],
     },
     total=False,
 )
@@ -665,20 +715,22 @@
         "ClientRequestToken": str,
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
+
 class DescribeFileSystemAliasesRequestRequestTypeDef(
     _RequiredDescribeFileSystemAliasesRequestRequestTypeDef,
     _OptionalDescribeFileSystemAliasesRequestRequestTypeDef,
 ):
     pass
 
+
 DescribeFileSystemsRequestRequestTypeDef = TypedDict(
     "DescribeFileSystemsRequestRequestTypeDef",
     {
         "FileSystemIds": Sequence[str],
         "MaxResults": int,
         "NextToken": str,
     },
@@ -723,20 +775,22 @@
     "_OptionalDisassociateFileSystemAliasesRequestRequestTypeDef",
     {
         "ClientRequestToken": str,
     },
     total=False,
 )
 
+
 class DisassociateFileSystemAliasesRequestRequestTypeDef(
     _RequiredDisassociateFileSystemAliasesRequestRequestTypeDef,
     _OptionalDisassociateFileSystemAliasesRequestRequestTypeDef,
 ):
     pass
 
+
 FileCacheFailureDetailsTypeDef = TypedDict(
     "FileCacheFailureDetailsTypeDef",
     {
         "Message": str,
     },
     total=False,
 )
@@ -751,38 +805,42 @@
     "_OptionalFileCacheNFSConfigurationTypeDef",
     {
         "DnsIps": Sequence[str],
     },
     total=False,
 )
 
+
 class FileCacheNFSConfigurationTypeDef(
     _RequiredFileCacheNFSConfigurationTypeDef, _OptionalFileCacheNFSConfigurationTypeDef
 ):
     pass
 
+
 _RequiredLustreLogConfigurationTypeDef = TypedDict(
     "_RequiredLustreLogConfigurationTypeDef",
     {
         "Level": LustreAccessAuditLogLevelType,
     },
 )
 _OptionalLustreLogConfigurationTypeDef = TypedDict(
     "_OptionalLustreLogConfigurationTypeDef",
     {
         "Destination": str,
     },
     total=False,
 )
 
+
 class LustreLogConfigurationTypeDef(
     _RequiredLustreLogConfigurationTypeDef, _OptionalLustreLogConfigurationTypeDef
 ):
     pass
 
+
 FileSystemEndpointTypeDef = TypedDict(
     "FileSystemEndpointTypeDef",
     {
         "DNSName": str,
         "IpAddresses": List[str],
     },
     total=False,
@@ -815,20 +873,22 @@
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
+
 class ListTagsForResourceRequestRequestTypeDef(
     _RequiredListTagsForResourceRequestRequestTypeDef,
     _OptionalListTagsForResourceRequestRequestTypeDef,
 ):
     pass
 
+
 OpenZFSClientConfigurationTypeDef = TypedDict(
     "OpenZFSClientConfigurationTypeDef",
     {
         "Clients": str,
         "Options": List[str],
     },
 )
@@ -852,20 +912,22 @@
     "_OptionalReleaseFileSystemNfsV3LocksRequestRequestTypeDef",
     {
         "ClientRequestToken": str,
     },
     total=False,
 )
 
+
 class ReleaseFileSystemNfsV3LocksRequestRequestTypeDef(
     _RequiredReleaseFileSystemNfsV3LocksRequestRequestTypeDef,
     _OptionalReleaseFileSystemNfsV3LocksRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredRestoreVolumeFromSnapshotRequestRequestTypeDef = TypedDict(
     "_RequiredRestoreVolumeFromSnapshotRequestRequestTypeDef",
     {
         "VolumeId": str,
         "SnapshotId": str,
     },
 )
@@ -874,20 +936,41 @@
     {
         "ClientRequestToken": str,
         "Options": Sequence[RestoreOpenZFSVolumeOptionType],
     },
     total=False,
 )
 
+
 class RestoreVolumeFromSnapshotRequestRequestTypeDef(
     _RequiredRestoreVolumeFromSnapshotRequestRequestTypeDef,
     _OptionalRestoreVolumeFromSnapshotRequestRequestTypeDef,
 ):
     pass
 
+
+_RequiredRetentionPeriodTypeDef = TypedDict(
+    "_RequiredRetentionPeriodTypeDef",
+    {
+        "Type": RetentionPeriodTypeType,
+    },
+)
+_OptionalRetentionPeriodTypeDef = TypedDict(
+    "_OptionalRetentionPeriodTypeDef",
+    {
+        "Value": int,
+    },
+    total=False,
+)
+
+
+class RetentionPeriodTypeDef(_RequiredRetentionPeriodTypeDef, _OptionalRetentionPeriodTypeDef):
+    pass
+
+
 SelfManagedActiveDirectoryAttributesTypeDef = TypedDict(
     "SelfManagedActiveDirectoryAttributesTypeDef",
     {
         "DomainName": str,
         "OrganizationalUnitDistinguishedName": str,
         "FileSystemAdministratorsGroup": str,
         "UserName": str,
@@ -945,19 +1028,21 @@
     "_OptionalUpdateSnapshotRequestRequestTypeDef",
     {
         "ClientRequestToken": str,
     },
     total=False,
 )
 
+
 class UpdateSnapshotRequestRequestTypeDef(
     _RequiredUpdateSnapshotRequestRequestTypeDef, _OptionalUpdateSnapshotRequestRequestTypeDef
 ):
     pass
 
+
 _RequiredWindowsAuditLogConfigurationTypeDef = TypedDict(
     "_RequiredWindowsAuditLogConfigurationTypeDef",
     {
         "FileAccessAuditLogLevel": WindowsAccessAuditLogLevelType,
         "FileShareAccessAuditLogLevel": WindowsAccessAuditLogLevelType,
     },
 )
@@ -965,19 +1050,21 @@
     "_OptionalWindowsAuditLogConfigurationTypeDef",
     {
         "AuditLogDestination": str,
     },
     total=False,
 )
 
+
 class WindowsAuditLogConfigurationTypeDef(
     _RequiredWindowsAuditLogConfigurationTypeDef, _OptionalWindowsAuditLogConfigurationTypeDef
 ):
     pass
 
+
 AssociateFileSystemAliasesResponseTypeDef = TypedDict(
     "AssociateFileSystemAliasesResponseTypeDef",
     {
         "Aliases": List[AliasTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -1116,19 +1203,21 @@
     {
         "DnsIps": List[str],
         "AutoExportPolicy": AutoExportPolicyTypeDef,
     },
     total=False,
 )
 
+
 class NFSDataRepositoryConfigurationTypeDef(
     _RequiredNFSDataRepositoryConfigurationTypeDef, _OptionalNFSDataRepositoryConfigurationTypeDef
 ):
     pass
 
+
 S3DataRepositoryConfigurationTypeDef = TypedDict(
     "S3DataRepositoryConfigurationTypeDef",
     {
         "AutoImportPolicy": AutoImportPolicyTypeDef,
         "AutoExportPolicy": AutoExportPolicyTypeDef,
     },
     total=False,
@@ -1148,19 +1237,21 @@
         "KmsKeyId": str,
         "CopyTags": bool,
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
+
 class CopyBackupRequestRequestTypeDef(
     _RequiredCopyBackupRequestRequestTypeDef, _OptionalCopyBackupRequestRequestTypeDef
 ):
     pass
 
+
 CreateBackupRequestRequestTypeDef = TypedDict(
     "CreateBackupRequestRequestTypeDef",
     {
         "FileSystemId": str,
         "ClientRequestToken": str,
         "Tags": Sequence[TagTypeDef],
         "VolumeId": str,
@@ -1180,19 +1271,21 @@
     {
         "ClientRequestToken": str,
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
+
 class CreateSnapshotRequestRequestTypeDef(
     _RequiredCreateSnapshotRequestRequestTypeDef, _OptionalCreateSnapshotRequestRequestTypeDef
 ):
     pass
 
+
 DeleteFileSystemLustreConfigurationTypeDef = TypedDict(
     "DeleteFileSystemLustreConfigurationTypeDef",
     {
         "SkipFinalBackup": bool,
         "FinalBackupTags": Sequence[TagTypeDef],
     },
     total=False,
@@ -1245,14 +1338,15 @@
 )
 
 DeleteVolumeOntapConfigurationTypeDef = TypedDict(
     "DeleteVolumeOntapConfigurationTypeDef",
     {
         "SkipFinalBackup": bool,
         "FinalBackupTags": Sequence[TagTypeDef],
+        "BypassSnaplockEnterpriseRetention": bool,
     },
     total=False,
 )
 
 DeleteVolumeOntapResponseTypeDef = TypedDict(
     "DeleteVolumeOntapResponseTypeDef",
     {
@@ -1294,20 +1388,22 @@
         "ClientRequestToken": str,
         "Tags": Sequence[TagTypeDef],
         "CapacityToRelease": int,
     },
     total=False,
 )
 
+
 class CreateDataRepositoryTaskRequestRequestTypeDef(
     _RequiredCreateDataRepositoryTaskRequestRequestTypeDef,
     _OptionalCreateDataRepositoryTaskRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredCreateFileCacheLustreConfigurationTypeDef = TypedDict(
     "_RequiredCreateFileCacheLustreConfigurationTypeDef",
     {
         "PerUnitStorageThroughput": int,
         "DeploymentType": Literal["CACHE_1"],
         "MetadataConfiguration": FileCacheLustreMetadataConfigurationTypeDef,
     },
@@ -1316,20 +1412,22 @@
     "_OptionalCreateFileCacheLustreConfigurationTypeDef",
     {
         "WeeklyMaintenanceStartTime": str,
     },
     total=False,
 )
 
+
 class CreateFileCacheLustreConfigurationTypeDef(
     _RequiredCreateFileCacheLustreConfigurationTypeDef,
     _OptionalCreateFileCacheLustreConfigurationTypeDef,
 ):
     pass
 
+
 CreateFileSystemLustreConfigurationTypeDef = TypedDict(
     "CreateFileSystemLustreConfigurationTypeDef",
     {
         "WeeklyMaintenanceStartTime": str,
         "ImportPath": str,
         "ExportPath": str,
         "ImportedFileChunkSize": int,
@@ -1379,20 +1477,22 @@
         "PreferredSubnetId": str,
         "RouteTableIds": Sequence[str],
         "WeeklyMaintenanceStartTime": str,
     },
     total=False,
 )
 
+
 class CreateFileSystemOntapConfigurationTypeDef(
     _RequiredCreateFileSystemOntapConfigurationTypeDef,
     _OptionalCreateFileSystemOntapConfigurationTypeDef,
 ):
     pass
 
+
 OpenZFSFileSystemConfigurationTypeDef = TypedDict(
     "OpenZFSFileSystemConfigurationTypeDef",
     {
         "AutomaticBackupRetentionDays": int,
         "CopyTagsToBackups": bool,
         "CopyTagsToVolumes": bool,
         "DailyAutomaticBackupStartTime": str,
@@ -1444,20 +1544,22 @@
     "_OptionalCreateSvmActiveDirectoryConfigurationTypeDef",
     {
         "SelfManagedActiveDirectoryConfiguration": SelfManagedActiveDirectoryConfigurationTypeDef,
     },
     total=False,
 )
 
+
 class CreateSvmActiveDirectoryConfigurationTypeDef(
     _RequiredCreateSvmActiveDirectoryConfigurationTypeDef,
     _OptionalCreateSvmActiveDirectoryConfigurationTypeDef,
 ):
     pass
 
+
 _RequiredCreateFileSystemWindowsConfigurationTypeDef = TypedDict(
     "_RequiredCreateFileSystemWindowsConfigurationTypeDef",
     {
         "ThroughputCapacity": int,
     },
 )
 _OptionalCreateFileSystemWindowsConfigurationTypeDef = TypedDict(
@@ -1473,78 +1575,21 @@
         "CopyTagsToBackups": bool,
         "Aliases": Sequence[str],
         "AuditLogConfiguration": WindowsAuditLogCreateConfigurationTypeDef,
     },
     total=False,
 )
 
+
 class CreateFileSystemWindowsConfigurationTypeDef(
     _RequiredCreateFileSystemWindowsConfigurationTypeDef,
     _OptionalCreateFileSystemWindowsConfigurationTypeDef,
 ):
     pass
 
-_RequiredCreateOntapVolumeConfigurationTypeDef = TypedDict(
-    "_RequiredCreateOntapVolumeConfigurationTypeDef",
-    {
-        "SizeInMegabytes": int,
-        "StorageVirtualMachineId": str,
-    },
-)
-_OptionalCreateOntapVolumeConfigurationTypeDef = TypedDict(
-    "_OptionalCreateOntapVolumeConfigurationTypeDef",
-    {
-        "JunctionPath": str,
-        "SecurityStyle": SecurityStyleType,
-        "StorageEfficiencyEnabled": bool,
-        "TieringPolicy": TieringPolicyTypeDef,
-        "OntapVolumeType": InputOntapVolumeTypeType,
-        "SnapshotPolicy": str,
-        "CopyTagsToBackups": bool,
-    },
-    total=False,
-)
-
-class CreateOntapVolumeConfigurationTypeDef(
-    _RequiredCreateOntapVolumeConfigurationTypeDef, _OptionalCreateOntapVolumeConfigurationTypeDef
-):
-    pass
-
-OntapVolumeConfigurationTypeDef = TypedDict(
-    "OntapVolumeConfigurationTypeDef",
-    {
-        "FlexCacheEndpointType": FlexCacheEndpointTypeType,
-        "JunctionPath": str,
-        "SecurityStyle": SecurityStyleType,
-        "SizeInMegabytes": int,
-        "StorageEfficiencyEnabled": bool,
-        "StorageVirtualMachineId": str,
-        "StorageVirtualMachineRoot": bool,
-        "TieringPolicy": TieringPolicyTypeDef,
-        "UUID": str,
-        "OntapVolumeType": OntapVolumeTypeType,
-        "SnapshotPolicy": str,
-        "CopyTagsToBackups": bool,
-    },
-    total=False,
-)
-
-UpdateOntapVolumeConfigurationTypeDef = TypedDict(
-    "UpdateOntapVolumeConfigurationTypeDef",
-    {
-        "JunctionPath": str,
-        "SecurityStyle": SecurityStyleType,
-        "SizeInMegabytes": int,
-        "StorageEfficiencyEnabled": bool,
-        "TieringPolicy": TieringPolicyTypeDef,
-        "SnapshotPolicy": str,
-        "CopyTagsToBackups": bool,
-    },
-    total=False,
-)
 
 DataRepositoryConfigurationTypeDef = TypedDict(
     "DataRepositoryConfigurationTypeDef",
     {
         "Lifecycle": DataRepositoryLifecycleType,
         "ImportPath": str,
         "ExportPath": str,
@@ -1589,19 +1634,21 @@
         "Report": CompletionReportTypeDef,
         "CapacityToRelease": int,
         "FileCacheId": str,
     },
     total=False,
 )
 
+
 class DataRepositoryTaskTypeDef(
     _RequiredDataRepositoryTaskTypeDef, _OptionalDataRepositoryTaskTypeDef
 ):
     pass
 
+
 DescribeBackupsRequestRequestTypeDef = TypedDict(
     "DescribeBackupsRequestRequestTypeDef",
     {
         "BackupIds": Sequence[str],
         "Filters": Sequence[FilterTypeDef],
         "MaxResults": int,
         "NextToken": str,
@@ -1649,20 +1696,22 @@
     "_OptionalListTagsForResourceRequestListTagsForResourcePaginateTypeDef",
     {
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
+
 class ListTagsForResourceRequestListTagsForResourcePaginateTypeDef(
     _RequiredListTagsForResourceRequestListTagsForResourcePaginateTypeDef,
     _OptionalListTagsForResourceRequestListTagsForResourcePaginateTypeDef,
 ):
     pass
 
+
 DescribeSnapshotsRequestRequestTypeDef = TypedDict(
     "DescribeSnapshotsRequestRequestTypeDef",
     {
         "SnapshotIds": Sequence[str],
         "Filters": Sequence[SnapshotFilterTypeDef],
         "MaxResults": int,
         "NextToken": str,
@@ -1724,20 +1773,22 @@
     {
         "DataRepositorySubdirectories": Sequence[str],
         "NFS": FileCacheNFSConfigurationTypeDef,
     },
     total=False,
 )
 
+
 class FileCacheDataRepositoryAssociationTypeDef(
     _RequiredFileCacheDataRepositoryAssociationTypeDef,
     _OptionalFileCacheDataRepositoryAssociationTypeDef,
 ):
     pass
 
+
 FileCacheLustreConfigurationTypeDef = TypedDict(
     "FileCacheLustreConfigurationTypeDef",
     {
         "PerUnitStorageThroughput": int,
         "DeploymentType": Literal["CACHE_1"],
         "MountName": str,
         "WeeklyMaintenanceStartTime": str,
@@ -1775,14 +1826,23 @@
 OpenZFSNfsExportTypeDef = TypedDict(
     "OpenZFSNfsExportTypeDef",
     {
         "ClientConfigurations": List[OpenZFSClientConfigurationTypeDef],
     },
 )
 
+SnaplockRetentionPeriodTypeDef = TypedDict(
+    "SnaplockRetentionPeriodTypeDef",
+    {
+        "DefaultRetention": RetentionPeriodTypeDef,
+        "MinimumRetention": RetentionPeriodTypeDef,
+        "MaximumRetention": RetentionPeriodTypeDef,
+    },
+)
+
 SvmActiveDirectoryConfigurationTypeDef = TypedDict(
     "SvmActiveDirectoryConfigurationTypeDef",
     {
         "NetBiosName": str,
         "SelfManagedActiveDirectoryConfiguration": SelfManagedActiveDirectoryAttributesTypeDef,
     },
     total=False,
@@ -1836,19 +1896,21 @@
     {
         "ClientRequestToken": str,
         "LustreConfiguration": UpdateFileCacheLustreConfigurationTypeDef,
     },
     total=False,
 )
 
+
 class UpdateFileCacheRequestRequestTypeDef(
     _RequiredUpdateFileCacheRequestRequestTypeDef, _OptionalUpdateFileCacheRequestRequestTypeDef
 ):
     pass
 
+
 WindowsFileSystemConfigurationTypeDef = TypedDict(
     "WindowsFileSystemConfigurationTypeDef",
     {
         "ActiveDirectoryId": str,
         "SelfManagedActiveDirectoryConfiguration": SelfManagedActiveDirectoryAttributesTypeDef,
         "DeploymentType": WindowsDeploymentTypeType,
         "RemoteAdministrationEndpoint": str,
@@ -1882,20 +1944,22 @@
         "S3": S3DataRepositoryConfigurationTypeDef,
         "ClientRequestToken": str,
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
+
 class CreateDataRepositoryAssociationRequestRequestTypeDef(
     _RequiredCreateDataRepositoryAssociationRequestRequestTypeDef,
     _OptionalCreateDataRepositoryAssociationRequestRequestTypeDef,
 ):
     pass
 
+
 DataRepositoryAssociationTypeDef = TypedDict(
     "DataRepositoryAssociationTypeDef",
     {
         "AssociationId": str,
         "ResourceARN": str,
         "FileSystemId": str,
         "Lifecycle": DataRepositoryLifecycleType,
@@ -1927,20 +1991,22 @@
         "ClientRequestToken": str,
         "ImportedFileChunkSize": int,
         "S3": S3DataRepositoryConfigurationTypeDef,
     },
     total=False,
 )
 
+
 class UpdateDataRepositoryAssociationRequestRequestTypeDef(
     _RequiredUpdateDataRepositoryAssociationRequestRequestTypeDef,
     _OptionalUpdateDataRepositoryAssociationRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredDeleteFileSystemRequestRequestTypeDef = TypedDict(
     "_RequiredDeleteFileSystemRequestRequestTypeDef",
     {
         "FileSystemId": str,
     },
 )
 _OptionalDeleteFileSystemRequestRequestTypeDef = TypedDict(
@@ -1950,19 +2016,21 @@
         "WindowsConfiguration": DeleteFileSystemWindowsConfigurationTypeDef,
         "LustreConfiguration": DeleteFileSystemLustreConfigurationTypeDef,
         "OpenZFSConfiguration": DeleteFileSystemOpenZFSConfigurationTypeDef,
     },
     total=False,
 )
 
+
 class DeleteFileSystemRequestRequestTypeDef(
     _RequiredDeleteFileSystemRequestRequestTypeDef, _OptionalDeleteFileSystemRequestRequestTypeDef
 ):
     pass
 
+
 DeleteFileSystemResponseTypeDef = TypedDict(
     "DeleteFileSystemResponseTypeDef",
     {
         "FileSystemId": str,
         "Lifecycle": FileSystemLifecycleType,
         "WindowsResponse": DeleteFileSystemWindowsResponseTypeDef,
         "LustreResponse": DeleteFileSystemLustreResponseTypeDef,
@@ -1983,19 +2051,21 @@
         "ClientRequestToken": str,
         "OntapConfiguration": DeleteVolumeOntapConfigurationTypeDef,
         "OpenZFSConfiguration": DeleteVolumeOpenZFSConfigurationTypeDef,
     },
     total=False,
 )
 
+
 class DeleteVolumeRequestRequestTypeDef(
     _RequiredDeleteVolumeRequestRequestTypeDef, _OptionalDeleteVolumeRequestRequestTypeDef
 ):
     pass
 
+
 DeleteVolumeResponseTypeDef = TypedDict(
     "DeleteVolumeResponseTypeDef",
     {
         "VolumeId": str,
         "Lifecycle": VolumeLifecycleType,
         "OntapResponse": DeleteVolumeOntapResponseTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
@@ -2017,42 +2087,21 @@
         "SvmAdminPassword": str,
         "Tags": Sequence[TagTypeDef],
         "RootVolumeSecurityStyle": StorageVirtualMachineRootVolumeSecurityStyleType,
     },
     total=False,
 )
 
+
 class CreateStorageVirtualMachineRequestRequestTypeDef(
     _RequiredCreateStorageVirtualMachineRequestRequestTypeDef,
     _OptionalCreateStorageVirtualMachineRequestRequestTypeDef,
 ):
     pass
 
-_RequiredCreateVolumeFromBackupRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateVolumeFromBackupRequestRequestTypeDef",
-    {
-        "BackupId": str,
-        "Name": str,
-    },
-)
-_OptionalCreateVolumeFromBackupRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateVolumeFromBackupRequestRequestTypeDef",
-    {
-        "ClientRequestToken": str,
-        "OntapConfiguration": CreateOntapVolumeConfigurationTypeDef,
-        "Tags": Sequence[TagTypeDef],
-    },
-    total=False,
-)
-
-class CreateVolumeFromBackupRequestRequestTypeDef(
-    _RequiredCreateVolumeFromBackupRequestRequestTypeDef,
-    _OptionalCreateVolumeFromBackupRequestRequestTypeDef,
-):
-    pass
 
 LustreFileSystemConfigurationTypeDef = TypedDict(
     "LustreFileSystemConfigurationTypeDef",
     {
         "WeeklyMaintenanceStartTime": str,
         "DataRepositoryConfiguration": DataRepositoryConfigurationTypeDef,
         "DeploymentType": LustreDeploymentTypeType,
@@ -2105,19 +2154,21 @@
         "KmsKeyId": str,
         "LustreConfiguration": CreateFileCacheLustreConfigurationTypeDef,
         "DataRepositoryAssociations": Sequence[FileCacheDataRepositoryAssociationTypeDef],
     },
     total=False,
 )
 
+
 class CreateFileCacheRequestRequestTypeDef(
     _RequiredCreateFileCacheRequestRequestTypeDef, _OptionalCreateFileCacheRequestRequestTypeDef
 ):
     pass
 
+
 FileCacheCreatingTypeDef = TypedDict(
     "FileCacheCreatingTypeDef",
     {
         "OwnerId": str,
         "CreationTime": datetime,
         "FileCacheId": str,
         "FileCacheType": Literal["LUSTRE"],
@@ -2223,20 +2274,22 @@
         "ReadOnly": bool,
         "NfsExports": Sequence[OpenZFSNfsExportTypeDef],
         "UserAndGroupQuotas": Sequence[OpenZFSUserOrGroupQuotaTypeDef],
     },
     total=False,
 )
 
+
 class CreateOpenZFSVolumeConfigurationTypeDef(
     _RequiredCreateOpenZFSVolumeConfigurationTypeDef,
     _OptionalCreateOpenZFSVolumeConfigurationTypeDef,
 ):
     pass
 
+
 OpenZFSCreateRootVolumeConfigurationTypeDef = TypedDict(
     "OpenZFSCreateRootVolumeConfigurationTypeDef",
     {
         "RecordSizeKiB": int,
         "DataCompressionType": OpenZFSDataCompressionTypeType,
         "NfsExports": Sequence[OpenZFSNfsExportTypeDef],
         "UserAndGroupQuotas": Sequence[OpenZFSUserOrGroupQuotaTypeDef],
@@ -2277,14 +2330,64 @@
         "NfsExports": Sequence[OpenZFSNfsExportTypeDef],
         "UserAndGroupQuotas": Sequence[OpenZFSUserOrGroupQuotaTypeDef],
         "ReadOnly": bool,
     },
     total=False,
 )
 
+_RequiredCreateSnaplockConfigurationTypeDef = TypedDict(
+    "_RequiredCreateSnaplockConfigurationTypeDef",
+    {
+        "SnaplockType": SnaplockTypeType,
+    },
+)
+_OptionalCreateSnaplockConfigurationTypeDef = TypedDict(
+    "_OptionalCreateSnaplockConfigurationTypeDef",
+    {
+        "AuditLogVolume": bool,
+        "AutocommitPeriod": AutocommitPeriodTypeDef,
+        "PrivilegedDelete": PrivilegedDeleteType,
+        "RetentionPeriod": SnaplockRetentionPeriodTypeDef,
+        "VolumeAppendModeEnabled": bool,
+    },
+    total=False,
+)
+
+
+class CreateSnaplockConfigurationTypeDef(
+    _RequiredCreateSnaplockConfigurationTypeDef, _OptionalCreateSnaplockConfigurationTypeDef
+):
+    pass
+
+
+SnaplockConfigurationTypeDef = TypedDict(
+    "SnaplockConfigurationTypeDef",
+    {
+        "AuditLogVolume": bool,
+        "AutocommitPeriod": AutocommitPeriodTypeDef,
+        "PrivilegedDelete": PrivilegedDeleteType,
+        "RetentionPeriod": SnaplockRetentionPeriodTypeDef,
+        "SnaplockType": SnaplockTypeType,
+        "VolumeAppendModeEnabled": bool,
+    },
+    total=False,
+)
+
+UpdateSnaplockConfigurationTypeDef = TypedDict(
+    "UpdateSnaplockConfigurationTypeDef",
+    {
+        "AuditLogVolume": bool,
+        "AutocommitPeriod": AutocommitPeriodTypeDef,
+        "PrivilegedDelete": PrivilegedDeleteType,
+        "RetentionPeriod": SnaplockRetentionPeriodTypeDef,
+        "VolumeAppendModeEnabled": bool,
+    },
+    total=False,
+)
+
 _RequiredUpdateFileSystemRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateFileSystemRequestRequestTypeDef",
     {
         "FileSystemId": str,
     },
 )
 _OptionalUpdateFileSystemRequestRequestTypeDef = TypedDict(
@@ -2296,19 +2399,21 @@
         "LustreConfiguration": UpdateFileSystemLustreConfigurationTypeDef,
         "OntapConfiguration": UpdateFileSystemOntapConfigurationTypeDef,
         "OpenZFSConfiguration": UpdateFileSystemOpenZFSConfigurationTypeDef,
     },
     total=False,
 )
 
+
 class UpdateFileSystemRequestRequestTypeDef(
     _RequiredUpdateFileSystemRequestRequestTypeDef, _OptionalUpdateFileSystemRequestRequestTypeDef
 ):
     pass
 
+
 _RequiredUpdateStorageVirtualMachineRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateStorageVirtualMachineRequestRequestTypeDef",
     {
         "StorageVirtualMachineId": str,
     },
 )
 _OptionalUpdateStorageVirtualMachineRequestRequestTypeDef = TypedDict(
@@ -2317,20 +2422,22 @@
         "ActiveDirectoryConfiguration": UpdateSvmActiveDirectoryConfigurationTypeDef,
         "ClientRequestToken": str,
         "SvmAdminPassword": str,
     },
     total=False,
 )
 
+
 class UpdateStorageVirtualMachineRequestRequestTypeDef(
     _RequiredUpdateStorageVirtualMachineRequestRequestTypeDef,
     _OptionalUpdateStorageVirtualMachineRequestRequestTypeDef,
 ):
     pass
 
+
 StorageVirtualMachineTypeDef = TypedDict(
     "StorageVirtualMachineTypeDef",
     {
         "ActiveDirectoryConfiguration": SvmActiveDirectoryConfigurationTypeDef,
         "CreationTime": datetime,
         "Endpoints": SvmEndpointsTypeDef,
         "FileSystemId": str,
@@ -2413,45 +2520,22 @@
         "NetworkInterfaceIds": List[str],
         "DNSName": str,
         "KmsKeyId": str,
         "ResourceARN": str,
         "Tags": List[TagTypeDef],
         "WindowsConfiguration": WindowsFileSystemConfigurationTypeDef,
         "LustreConfiguration": LustreFileSystemConfigurationTypeDef,
-        "AdministrativeActions": List["AdministrativeActionTypeDef"],
+        "AdministrativeActions": List[Dict[str, Any]],
         "OntapConfiguration": OntapFileSystemConfigurationTypeDef,
         "FileSystemTypeVersion": str,
         "OpenZFSConfiguration": OpenZFSFileSystemConfigurationTypeDef,
     },
     total=False,
 )
 
-_RequiredCreateVolumeRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateVolumeRequestRequestTypeDef",
-    {
-        "VolumeType": VolumeTypeType,
-        "Name": str,
-    },
-)
-_OptionalCreateVolumeRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateVolumeRequestRequestTypeDef",
-    {
-        "ClientRequestToken": str,
-        "OntapConfiguration": CreateOntapVolumeConfigurationTypeDef,
-        "Tags": Sequence[TagTypeDef],
-        "OpenZFSConfiguration": CreateOpenZFSVolumeConfigurationTypeDef,
-    },
-    total=False,
-)
-
-class CreateVolumeRequestRequestTypeDef(
-    _RequiredCreateVolumeRequestRequestTypeDef, _OptionalCreateVolumeRequestRequestTypeDef
-):
-    pass
-
 _RequiredCreateFileSystemOpenZFSConfigurationTypeDef = TypedDict(
     "_RequiredCreateFileSystemOpenZFSConfigurationTypeDef",
     {
         "DeploymentType": OpenZFSDeploymentTypeType,
         "ThroughputCapacity": int,
     },
 )
@@ -2465,61 +2549,86 @@
         "WeeklyMaintenanceStartTime": str,
         "DiskIopsConfiguration": DiskIopsConfigurationTypeDef,
         "RootVolumeConfiguration": OpenZFSCreateRootVolumeConfigurationTypeDef,
     },
     total=False,
 )
 
+
 class CreateFileSystemOpenZFSConfigurationTypeDef(
     _RequiredCreateFileSystemOpenZFSConfigurationTypeDef,
     _OptionalCreateFileSystemOpenZFSConfigurationTypeDef,
 ):
     pass
 
-VolumeTypeDef = TypedDict(
-    "VolumeTypeDef",
+
+_RequiredCreateOntapVolumeConfigurationTypeDef = TypedDict(
+    "_RequiredCreateOntapVolumeConfigurationTypeDef",
     {
-        "CreationTime": datetime,
-        "FileSystemId": str,
-        "Lifecycle": VolumeLifecycleType,
-        "Name": str,
-        "OntapConfiguration": OntapVolumeConfigurationTypeDef,
-        "ResourceARN": str,
-        "Tags": List[TagTypeDef],
-        "VolumeId": str,
-        "VolumeType": VolumeTypeType,
-        "LifecycleTransitionReason": LifecycleTransitionReasonTypeDef,
-        "AdministrativeActions": List[Dict[str, Any]],
-        "OpenZFSConfiguration": OpenZFSVolumeConfigurationTypeDef,
+        "SizeInMegabytes": int,
+        "StorageVirtualMachineId": str,
+    },
+)
+_OptionalCreateOntapVolumeConfigurationTypeDef = TypedDict(
+    "_OptionalCreateOntapVolumeConfigurationTypeDef",
+    {
+        "JunctionPath": str,
+        "SecurityStyle": SecurityStyleType,
+        "StorageEfficiencyEnabled": bool,
+        "TieringPolicy": TieringPolicyTypeDef,
+        "OntapVolumeType": InputOntapVolumeTypeType,
+        "SnapshotPolicy": str,
+        "CopyTagsToBackups": bool,
+        "SnaplockConfiguration": CreateSnaplockConfigurationTypeDef,
     },
     total=False,
 )
 
-_RequiredUpdateVolumeRequestRequestTypeDef = TypedDict(
-    "_RequiredUpdateVolumeRequestRequestTypeDef",
+
+class CreateOntapVolumeConfigurationTypeDef(
+    _RequiredCreateOntapVolumeConfigurationTypeDef, _OptionalCreateOntapVolumeConfigurationTypeDef
+):
+    pass
+
+
+OntapVolumeConfigurationTypeDef = TypedDict(
+    "OntapVolumeConfigurationTypeDef",
     {
-        "VolumeId": str,
+        "FlexCacheEndpointType": FlexCacheEndpointTypeType,
+        "JunctionPath": str,
+        "SecurityStyle": SecurityStyleType,
+        "SizeInMegabytes": int,
+        "StorageEfficiencyEnabled": bool,
+        "StorageVirtualMachineId": str,
+        "StorageVirtualMachineRoot": bool,
+        "TieringPolicy": TieringPolicyTypeDef,
+        "UUID": str,
+        "OntapVolumeType": OntapVolumeTypeType,
+        "SnapshotPolicy": str,
+        "CopyTagsToBackups": bool,
+        "SnaplockConfiguration": SnaplockConfigurationTypeDef,
     },
+    total=False,
 )
-_OptionalUpdateVolumeRequestRequestTypeDef = TypedDict(
-    "_OptionalUpdateVolumeRequestRequestTypeDef",
+
+UpdateOntapVolumeConfigurationTypeDef = TypedDict(
+    "UpdateOntapVolumeConfigurationTypeDef",
     {
-        "ClientRequestToken": str,
-        "OntapConfiguration": UpdateOntapVolumeConfigurationTypeDef,
-        "Name": str,
-        "OpenZFSConfiguration": UpdateOpenZFSVolumeConfigurationTypeDef,
+        "JunctionPath": str,
+        "SecurityStyle": SecurityStyleType,
+        "SizeInMegabytes": int,
+        "StorageEfficiencyEnabled": bool,
+        "TieringPolicy": TieringPolicyTypeDef,
+        "SnapshotPolicy": str,
+        "CopyTagsToBackups": bool,
+        "SnaplockConfiguration": UpdateSnaplockConfigurationTypeDef,
     },
     total=False,
 )
 
-class UpdateVolumeRequestRequestTypeDef(
-    _RequiredUpdateVolumeRequestRequestTypeDef, _OptionalUpdateVolumeRequestRequestTypeDef
-):
-    pass
-
 CreateStorageVirtualMachineResponseTypeDef = TypedDict(
     "CreateStorageVirtualMachineResponseTypeDef",
     {
         "StorageVirtualMachine": StorageVirtualMachineTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -2561,20 +2670,22 @@
         "FileSystemTypeVersion": str,
         "OpenZFSConfiguration": CreateFileSystemOpenZFSConfigurationTypeDef,
         "StorageCapacity": int,
     },
     total=False,
 )
 
+
 class CreateFileSystemFromBackupRequestRequestTypeDef(
     _RequiredCreateFileSystemFromBackupRequestRequestTypeDef,
     _OptionalCreateFileSystemFromBackupRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredCreateFileSystemRequestRequestTypeDef = TypedDict(
     "_RequiredCreateFileSystemRequestRequestTypeDef",
     {
         "FileSystemType": FileSystemTypeType,
         "StorageCapacity": int,
         "SubnetIds": Sequence[str],
     },
@@ -2592,19 +2703,114 @@
         "OntapConfiguration": CreateFileSystemOntapConfigurationTypeDef,
         "FileSystemTypeVersion": str,
         "OpenZFSConfiguration": CreateFileSystemOpenZFSConfigurationTypeDef,
     },
     total=False,
 )
 
+
 class CreateFileSystemRequestRequestTypeDef(
     _RequiredCreateFileSystemRequestRequestTypeDef, _OptionalCreateFileSystemRequestRequestTypeDef
 ):
     pass
 
+
+_RequiredCreateVolumeFromBackupRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateVolumeFromBackupRequestRequestTypeDef",
+    {
+        "BackupId": str,
+        "Name": str,
+    },
+)
+_OptionalCreateVolumeFromBackupRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateVolumeFromBackupRequestRequestTypeDef",
+    {
+        "ClientRequestToken": str,
+        "OntapConfiguration": CreateOntapVolumeConfigurationTypeDef,
+        "Tags": Sequence[TagTypeDef],
+    },
+    total=False,
+)
+
+
+class CreateVolumeFromBackupRequestRequestTypeDef(
+    _RequiredCreateVolumeFromBackupRequestRequestTypeDef,
+    _OptionalCreateVolumeFromBackupRequestRequestTypeDef,
+):
+    pass
+
+
+_RequiredCreateVolumeRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateVolumeRequestRequestTypeDef",
+    {
+        "VolumeType": VolumeTypeType,
+        "Name": str,
+    },
+)
+_OptionalCreateVolumeRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateVolumeRequestRequestTypeDef",
+    {
+        "ClientRequestToken": str,
+        "OntapConfiguration": CreateOntapVolumeConfigurationTypeDef,
+        "Tags": Sequence[TagTypeDef],
+        "OpenZFSConfiguration": CreateOpenZFSVolumeConfigurationTypeDef,
+    },
+    total=False,
+)
+
+
+class CreateVolumeRequestRequestTypeDef(
+    _RequiredCreateVolumeRequestRequestTypeDef, _OptionalCreateVolumeRequestRequestTypeDef
+):
+    pass
+
+
+VolumeTypeDef = TypedDict(
+    "VolumeTypeDef",
+    {
+        "CreationTime": datetime,
+        "FileSystemId": str,
+        "Lifecycle": VolumeLifecycleType,
+        "Name": str,
+        "OntapConfiguration": OntapVolumeConfigurationTypeDef,
+        "ResourceARN": str,
+        "Tags": List[TagTypeDef],
+        "VolumeId": str,
+        "VolumeType": VolumeTypeType,
+        "LifecycleTransitionReason": LifecycleTransitionReasonTypeDef,
+        "AdministrativeActions": List["AdministrativeActionTypeDef"],
+        "OpenZFSConfiguration": OpenZFSVolumeConfigurationTypeDef,
+    },
+    total=False,
+)
+
+_RequiredUpdateVolumeRequestRequestTypeDef = TypedDict(
+    "_RequiredUpdateVolumeRequestRequestTypeDef",
+    {
+        "VolumeId": str,
+    },
+)
+_OptionalUpdateVolumeRequestRequestTypeDef = TypedDict(
+    "_OptionalUpdateVolumeRequestRequestTypeDef",
+    {
+        "ClientRequestToken": str,
+        "OntapConfiguration": UpdateOntapVolumeConfigurationTypeDef,
+        "Name": str,
+        "OpenZFSConfiguration": UpdateOpenZFSVolumeConfigurationTypeDef,
+    },
+    total=False,
+)
+
+
+class UpdateVolumeRequestRequestTypeDef(
+    _RequiredUpdateVolumeRequestRequestTypeDef, _OptionalUpdateVolumeRequestRequestTypeDef
+):
+    pass
+
+
 AdministrativeActionTypeDef = TypedDict(
     "AdministrativeActionTypeDef",
     {
         "AdministrativeActionType": AdministrativeActionTypeType,
         "ProgressPercent": int,
         "RequestTime": datetime,
         "Status": StatusType,
@@ -2640,17 +2846,19 @@
         "SourceBackupRegion": str,
         "ResourceType": ResourceTypeType,
         "Volume": VolumeTypeDef,
     },
     total=False,
 )
 
+
 class BackupTypeDef(_RequiredBackupTypeDef, _OptionalBackupTypeDef):
     pass
 
+
 CreateVolumeFromBackupResponseTypeDef = TypedDict(
     "CreateVolumeFromBackupResponseTypeDef",
     {
         "Volume": VolumeTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `types-aiobotocore-fsx-2.5.2.post3/types_aiobotocore_fsx.egg-info/PKG-INFO` & `types-aiobotocore-fsx-2.5.4/types_aiobotocore_fsx.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-fsx
-Version: 2.5.2.post3
-Summary: Type annotations for aiobotocore.FSx 2.5.2 service generated with mypy-boto3-builder 7.17.2
+Version: 2.5.4
+Summary: Type annotations for aiobotocore.FSx 2.5.4 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_fsx/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-fsx.svg?color=blue)](https://pypi.org/project/types-aiobotocore-fsx)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_fsx/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-fsx)](https://pepy.tech/project/types-aiobotocore-fsx)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.FSx 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fsx.html#FSx)
+[aiobotocore.FSx 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fsx.html#FSx)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-fsx-2.5.2.post3/types_aiobotocore_fsx.egg-info/SOURCES.txt` & `types-aiobotocore-fsx-2.5.4/types_aiobotocore_fsx.egg-info/SOURCES.txt`

 * *Files identical despite different names*


# Comparing `tmp/types-aiobotocore-healthlake-2.5.2.post2.tar.gz` & `tmp/types-aiobotocore-healthlake-2.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-healthlake-2.5.2.post2.tar", last modified: Fri Aug  4 12:37:48 2023, max compression
+gzip compressed data, was "types-aiobotocore-healthlake-2.5.4.tar", last modified: Tue Aug  8 01:23:48 2023, max compression
```

## Comparing `types-aiobotocore-healthlake-2.5.2.post2.tar` & `types-aiobotocore-healthlake-2.5.4.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:37:48.591925 types-aiobotocore-healthlake-2.5.2.post2/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-04 12:24:53.000000 types-aiobotocore-healthlake-2.5.2.post2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    12391 2023-08-04 12:37:48.591925 types-aiobotocore-healthlake-2.5.2.post2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    10861 2023-08-04 12:24:53.000000 types-aiobotocore-healthlake-2.5.2.post2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-04 12:37:48.591925 types-aiobotocore-healthlake-2.5.2.post2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2093 2023-08-04 12:24:53.000000 types-aiobotocore-healthlake-2.5.2.post2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:37:48.587925 types-aiobotocore-healthlake-2.5.2.post2/types_aiobotocore_healthlake/
--rw-r--r--   0 runner    (1001) docker     (123)      466 2023-08-04 12:24:53.000000 types-aiobotocore-healthlake-2.5.2.post2/types_aiobotocore_healthlake/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      465 2023-08-04 12:24:53.000000 types-aiobotocore-healthlake-2.5.2.post2/types_aiobotocore_healthlake/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      955 2023-08-04 12:24:53.000000 types-aiobotocore-healthlake-2.5.2.post2/types_aiobotocore_healthlake/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13403 2023-08-04 12:24:54.000000 types-aiobotocore-healthlake-2.5.2.post2/types_aiobotocore_healthlake/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    13381 2023-08-04 12:24:53.000000 types-aiobotocore-healthlake-2.5.2.post2/types_aiobotocore_healthlake/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8300 2023-08-04 12:24:54.000000 types-aiobotocore-healthlake-2.5.2.post2/types_aiobotocore_healthlake/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     8298 2023-08-04 12:24:54.000000 types-aiobotocore-healthlake-2.5.2.post2/types_aiobotocore_healthlake/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 12:24:53.000000 types-aiobotocore-healthlake-2.5.2.post2/types_aiobotocore_healthlake/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    14241 2023-08-04 12:24:54.000000 types-aiobotocore-healthlake-2.5.2.post2/types_aiobotocore_healthlake/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    14220 2023-08-04 12:24:54.000000 types-aiobotocore-healthlake-2.5.2.post2/types_aiobotocore_healthlake/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-04 12:24:53.000000 types-aiobotocore-healthlake-2.5.2.post2/types_aiobotocore_healthlake/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:37:48.591925 types-aiobotocore-healthlake-2.5.2.post2/types_aiobotocore_healthlake.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    12391 2023-08-04 12:37:48.000000 types-aiobotocore-healthlake-2.5.2.post2/types_aiobotocore_healthlake.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      785 2023-08-04 12:37:48.000000 types-aiobotocore-healthlake-2.5.2.post2/types_aiobotocore_healthlake.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 12:37:48.000000 types-aiobotocore-healthlake-2.5.2.post2/types_aiobotocore_healthlake.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 12:37:48.000000 types-aiobotocore-healthlake-2.5.2.post2/types_aiobotocore_healthlake.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-04 12:37:48.000000 types-aiobotocore-healthlake-2.5.2.post2/types_aiobotocore_healthlake.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-08-04 12:37:48.000000 types-aiobotocore-healthlake-2.5.2.post2/types_aiobotocore_healthlake.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:23:48.298728 types-aiobotocore-healthlake-2.5.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-08 01:12:12.000000 types-aiobotocore-healthlake-2.5.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    12385 2023-08-08 01:23:48.298728 types-aiobotocore-healthlake-2.5.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10861 2023-08-08 01:12:12.000000 types-aiobotocore-healthlake-2.5.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-08 01:23:48.298728 types-aiobotocore-healthlake-2.5.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2087 2023-08-08 01:12:12.000000 types-aiobotocore-healthlake-2.5.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:23:48.294728 types-aiobotocore-healthlake-2.5.4/types_aiobotocore_healthlake/
+-rw-r--r--   0 runner    (1001) docker     (123)      466 2023-08-08 01:12:12.000000 types-aiobotocore-healthlake-2.5.4/types_aiobotocore_healthlake/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      465 2023-08-08 01:12:12.000000 types-aiobotocore-healthlake-2.5.4/types_aiobotocore_healthlake/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      943 2023-08-08 01:12:12.000000 types-aiobotocore-healthlake-2.5.4/types_aiobotocore_healthlake/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13430 2023-08-08 01:12:12.000000 types-aiobotocore-healthlake-2.5.4/types_aiobotocore_healthlake/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13408 2023-08-08 01:12:12.000000 types-aiobotocore-healthlake-2.5.4/types_aiobotocore_healthlake/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8395 2023-08-08 01:12:12.000000 types-aiobotocore-healthlake-2.5.4/types_aiobotocore_healthlake/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8393 2023-08-08 01:12:12.000000 types-aiobotocore-healthlake-2.5.4/types_aiobotocore_healthlake/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 01:12:12.000000 types-aiobotocore-healthlake-2.5.4/types_aiobotocore_healthlake/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    14241 2023-08-08 01:12:12.000000 types-aiobotocore-healthlake-2.5.4/types_aiobotocore_healthlake/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14220 2023-08-08 01:12:12.000000 types-aiobotocore-healthlake-2.5.4/types_aiobotocore_healthlake/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-08-08 01:12:12.000000 types-aiobotocore-healthlake-2.5.4/types_aiobotocore_healthlake/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:23:48.298728 types-aiobotocore-healthlake-2.5.4/types_aiobotocore_healthlake.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    12385 2023-08-08 01:23:48.000000 types-aiobotocore-healthlake-2.5.4/types_aiobotocore_healthlake.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      785 2023-08-08 01:23:48.000000 types-aiobotocore-healthlake-2.5.4/types_aiobotocore_healthlake.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 01:23:48.000000 types-aiobotocore-healthlake-2.5.4/types_aiobotocore_healthlake.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 01:23:48.000000 types-aiobotocore-healthlake-2.5.4/types_aiobotocore_healthlake.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-08 01:23:48.000000 types-aiobotocore-healthlake-2.5.4/types_aiobotocore_healthlake.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-08-08 01:23:48.000000 types-aiobotocore-healthlake-2.5.4/types_aiobotocore_healthlake.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-healthlake-2.5.2.post2/LICENSE` & `types-aiobotocore-healthlake-2.5.4/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-healthlake-2.5.2.post2/PKG-INFO` & `types-aiobotocore-healthlake-2.5.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-healthlake
-Version: 2.5.2.post2
-Summary: Type annotations for aiobotocore.HealthLake 2.5.2 service generated with mypy-boto3-builder 7.17.2
+Version: 2.5.4
+Summary: Type annotations for aiobotocore.HealthLake 2.5.4 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_healthlake/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-healthlake.svg?color=blue)](https://pypi.org/project/types-aiobotocore-healthlake)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_healthlake/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-healthlake)](https://pepy.tech/project/types-aiobotocore-healthlake)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.HealthLake 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/healthlake.html#HealthLake)
+[aiobotocore.HealthLake 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/healthlake.html#HealthLake)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-healthlake-2.5.2.post2/README.md` & `types-aiobotocore-healthlake-2.5.4/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-healthlake.svg?color=blue)](https://pypi.org/project/types-aiobotocore-healthlake)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_healthlake/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-healthlake)](https://pepy.tech/project/types-aiobotocore-healthlake)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.HealthLake 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/healthlake.html#HealthLake)
+[aiobotocore.HealthLake 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/healthlake.html#HealthLake)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-healthlake-2.5.2.post2/setup.py` & `types-aiobotocore-healthlake-2.5.4/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-healthlake",
-    version="2.5.2.post2",
+    version="2.5.4",
     packages=["types_aiobotocore_healthlake"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.HealthLake 2.5.2 service generated with"
+        "Type annotations for aiobotocore.HealthLake 2.5.4 service generated with"
         " mypy-boto3-builder 7.17.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
```

### Comparing `types-aiobotocore-healthlake-2.5.2.post2/types_aiobotocore_healthlake/__main__.py` & `types-aiobotocore-healthlake-2.5.4/types_aiobotocore_healthlake/__main__.py`

 * *Files 15% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.HealthLake 2.5.2\nVersion:         2.5.2.post2\nBuilder"
+        "Type annotations for aiobotocore.HealthLake 2.5.4\nVersion:         2.5.4\nBuilder"
         " version: 7.17.2\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_healthlake//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/healthlake.html#HealthLake\nOther"
         " services:  https://pypi.org/project/boto3-stubs/\nChangelog:      "
         " https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("2.5.2.post2")
+    print("2.5.4")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `types-aiobotocore-healthlake-2.5.2.post2/types_aiobotocore_healthlake/client.py` & `types-aiobotocore-healthlake-2.5.4/types_aiobotocore_healthlake/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -111,37 +111,37 @@
         SseConfiguration: SseConfigurationTypeDef = ...,
         PreloadDataConfig: PreloadDataConfigTypeDef = ...,
         ClientToken: str = ...,
         Tags: Sequence[TagTypeDef] = ...,
         IdentityProviderConfiguration: IdentityProviderConfigurationTypeDef = ...
     ) -> CreateFHIRDatastoreResponseTypeDef:
         """
-        Creates a Data Store that can ingest and export FHIR formatted data.
+        Creates a data store that can ingest and export FHIR formatted data.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/healthlake.html#HealthLake.Client.create_fhir_datastore)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_healthlake/client/#create_fhir_datastore)
         """
 
     async def delete_fhir_datastore(
         self, *, DatastoreId: str
     ) -> DeleteFHIRDatastoreResponseTypeDef:
         """
-        Deletes a Data Store.
+        Deletes a data store.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/healthlake.html#HealthLake.Client.delete_fhir_datastore)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_healthlake/client/#delete_fhir_datastore)
         """
 
     async def describe_fhir_datastore(
         self, *, DatastoreId: str
     ) -> DescribeFHIRDatastoreResponseTypeDef:
         """
-        Gets the properties associated with the FHIR Data Store, including the Data
-        Store ID, Data Store ARN, Data Store name, Data Store status, created at, Data
-        Store type version, and Data Store endpoint.
+        Gets the properties associated with the FHIR data store, including the data
+        store ID, data store ARN, data store name, data store status, when the data
+        store was created, data store type version, and the data store's endpoint.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/healthlake.html#HealthLake.Client.describe_fhir_datastore)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_healthlake/client/#describe_fhir_datastore)
         """
 
     async def describe_fhir_export_job(
         self, *, DatastoreId: str, JobId: str
@@ -179,16 +179,16 @@
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_healthlake/client/#generate_presigned_url)
         """
 
     async def list_fhir_datastores(
         self, *, Filter: DatastoreFilterTypeDef = ..., NextToken: str = ..., MaxResults: int = ...
     ) -> ListFHIRDatastoresResponseTypeDef:
         """
-        Lists all FHIR Data Stores that are in the user’s account, regardless of Data
-        Store status.
+        Lists all FHIR data stores that are in the user’s account, regardless of data
+        store status.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/healthlake.html#HealthLake.Client.list_fhir_datastores)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_healthlake/client/#list_fhir_datastores)
         """
 
     async def list_fhir_export_jobs(
         self,
@@ -226,15 +226,15 @@
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_healthlake/client/#list_fhir_import_jobs)
         """
 
     async def list_tags_for_resource(
         self, *, ResourceARN: str
     ) -> ListTagsForResourceResponseTypeDef:
         """
-        Returns a list of all existing tags associated with a Data Store.
+        Returns a list of all existing tags associated with a data store.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/healthlake.html#HealthLake.Client.list_tags_for_resource)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_healthlake/client/#list_tags_for_resource)
         """
 
     async def start_fhir_export_job(
         self,
@@ -267,23 +267,23 @@
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/healthlake.html#HealthLake.Client.start_fhir_import_job)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_healthlake/client/#start_fhir_import_job)
         """
 
     async def tag_resource(self, *, ResourceARN: str, Tags: Sequence[TagTypeDef]) -> Dict[str, Any]:
         """
-        Adds a user specified key and value tag to a Data Store.
+        Adds a user specified key and value tag to a data store.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/healthlake.html#HealthLake.Client.tag_resource)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_healthlake/client/#tag_resource)
         """
 
     async def untag_resource(self, *, ResourceARN: str, TagKeys: Sequence[str]) -> Dict[str, Any]:
         """
-        Removes tags from a Data Store.
+        Removes tags from a data store.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/healthlake.html#HealthLake.Client.untag_resource)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_healthlake/client/#untag_resource)
         """
 
     async def __aenter__(self) -> "HealthLakeClient":
         """
```

### Comparing `types-aiobotocore-healthlake-2.5.2.post2/types_aiobotocore_healthlake/client.pyi` & `types-aiobotocore-healthlake-2.5.4/types_aiobotocore_healthlake/client.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -104,35 +104,35 @@
         SseConfiguration: SseConfigurationTypeDef = ...,
         PreloadDataConfig: PreloadDataConfigTypeDef = ...,
         ClientToken: str = ...,
         Tags: Sequence[TagTypeDef] = ...,
         IdentityProviderConfiguration: IdentityProviderConfigurationTypeDef = ...
     ) -> CreateFHIRDatastoreResponseTypeDef:
         """
-        Creates a Data Store that can ingest and export FHIR formatted data.
+        Creates a data store that can ingest and export FHIR formatted data.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/healthlake.html#HealthLake.Client.create_fhir_datastore)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_healthlake/client/#create_fhir_datastore)
         """
     async def delete_fhir_datastore(
         self, *, DatastoreId: str
     ) -> DeleteFHIRDatastoreResponseTypeDef:
         """
-        Deletes a Data Store.
+        Deletes a data store.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/healthlake.html#HealthLake.Client.delete_fhir_datastore)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_healthlake/client/#delete_fhir_datastore)
         """
     async def describe_fhir_datastore(
         self, *, DatastoreId: str
     ) -> DescribeFHIRDatastoreResponseTypeDef:
         """
-        Gets the properties associated with the FHIR Data Store, including the Data
-        Store ID, Data Store ARN, Data Store name, Data Store status, created at, Data
-        Store type version, and Data Store endpoint.
+        Gets the properties associated with the FHIR data store, including the data
+        store ID, data store ARN, data store name, data store status, when the data
+        store was created, data store type version, and the data store's endpoint.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/healthlake.html#HealthLake.Client.describe_fhir_datastore)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_healthlake/client/#describe_fhir_datastore)
         """
     async def describe_fhir_export_job(
         self, *, DatastoreId: str, JobId: str
     ) -> DescribeFHIRExportJobResponseTypeDef:
@@ -166,16 +166,16 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/healthlake.html#HealthLake.Client.generate_presigned_url)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_healthlake/client/#generate_presigned_url)
         """
     async def list_fhir_datastores(
         self, *, Filter: DatastoreFilterTypeDef = ..., NextToken: str = ..., MaxResults: int = ...
     ) -> ListFHIRDatastoresResponseTypeDef:
         """
-        Lists all FHIR Data Stores that are in the user’s account, regardless of Data
-        Store status.
+        Lists all FHIR data stores that are in the user’s account, regardless of data
+        store status.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/healthlake.html#HealthLake.Client.list_fhir_datastores)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_healthlake/client/#list_fhir_datastores)
         """
     async def list_fhir_export_jobs(
         self,
         *,
@@ -210,15 +210,15 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/healthlake.html#HealthLake.Client.list_fhir_import_jobs)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_healthlake/client/#list_fhir_import_jobs)
         """
     async def list_tags_for_resource(
         self, *, ResourceARN: str
     ) -> ListTagsForResourceResponseTypeDef:
         """
-        Returns a list of all existing tags associated with a Data Store.
+        Returns a list of all existing tags associated with a data store.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/healthlake.html#HealthLake.Client.list_tags_for_resource)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_healthlake/client/#list_tags_for_resource)
         """
     async def start_fhir_export_job(
         self,
         *,
@@ -248,22 +248,22 @@
         Begins a FHIR Import job.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/healthlake.html#HealthLake.Client.start_fhir_import_job)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_healthlake/client/#start_fhir_import_job)
         """
     async def tag_resource(self, *, ResourceARN: str, Tags: Sequence[TagTypeDef]) -> Dict[str, Any]:
         """
-        Adds a user specified key and value tag to a Data Store.
+        Adds a user specified key and value tag to a data store.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/healthlake.html#HealthLake.Client.tag_resource)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_healthlake/client/#tag_resource)
         """
     async def untag_resource(self, *, ResourceARN: str, TagKeys: Sequence[str]) -> Dict[str, Any]:
         """
-        Removes tags from a Data Store.
+        Removes tags from a data store.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/healthlake.html#HealthLake.Client.untag_resource)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_healthlake/client/#untag_resource)
         """
     async def __aenter__(self) -> "HealthLakeClient":
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/healthlake.html#HealthLake.Client)
```

### Comparing `types-aiobotocore-healthlake-2.5.2.post2/types_aiobotocore_healthlake/literals.py` & `types-aiobotocore-healthlake-2.5.4/types_aiobotocore_healthlake/literals.py`

 * *Files 1% similar despite different names*

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

### Comparing `types-aiobotocore-healthlake-2.5.2.post2/types_aiobotocore_healthlake/literals.pyi` & `types-aiobotocore-healthlake-2.5.4/types_aiobotocore_healthlake/literals.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -59,14 +59,15 @@
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
@@ -162,14 +163,15 @@
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
@@ -248,26 +250,28 @@
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

### Comparing `types-aiobotocore-healthlake-2.5.2.post2/types_aiobotocore_healthlake/type_defs.py` & `types-aiobotocore-healthlake-2.5.4/types_aiobotocore_healthlake/type_defs.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-healthlake-2.5.2.post2/types_aiobotocore_healthlake/type_defs.pyi` & `types-aiobotocore-healthlake-2.5.4/types_aiobotocore_healthlake/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-healthlake-2.5.2.post2/types_aiobotocore_healthlake.egg-info/PKG-INFO` & `types-aiobotocore-healthlake-2.5.4/types_aiobotocore_healthlake.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-healthlake
-Version: 2.5.2.post2
-Summary: Type annotations for aiobotocore.HealthLake 2.5.2 service generated with mypy-boto3-builder 7.17.2
+Version: 2.5.4
+Summary: Type annotations for aiobotocore.HealthLake 2.5.4 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_healthlake/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-healthlake.svg?color=blue)](https://pypi.org/project/types-aiobotocore-healthlake)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_healthlake/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-healthlake)](https://pepy.tech/project/types-aiobotocore-healthlake)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.HealthLake 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/healthlake.html#HealthLake)
+[aiobotocore.HealthLake 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/healthlake.html#HealthLake)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-healthlake-2.5.2.post2/types_aiobotocore_healthlake.egg-info/SOURCES.txt` & `types-aiobotocore-healthlake-2.5.4/types_aiobotocore_healthlake.egg-info/SOURCES.txt`

 * *Files identical despite different names*


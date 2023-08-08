# Comparing `tmp/types-aiobotocore-emr-serverless-2.5.2.post3.tar.gz` & `tmp/types-aiobotocore-emr-serverless-2.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-emr-serverless-2.5.2.post3.tar", last modified: Fri Aug  4 12:37:42 2023, max compression
+gzip compressed data, was "types-aiobotocore-emr-serverless-2.5.4.tar", last modified: Tue Aug  8 01:23:42 2023, max compression
```

## Comparing `types-aiobotocore-emr-serverless-2.5.2.post3.tar` & `types-aiobotocore-emr-serverless-2.5.4.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:37:42.015771 types-aiobotocore-emr-serverless-2.5.2.post3/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-04 12:23:32.000000 types-aiobotocore-emr-serverless-2.5.2.post3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    13460 2023-08-04 12:37:42.015771 types-aiobotocore-emr-serverless-2.5.2.post3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    11915 2023-08-04 12:23:32.000000 types-aiobotocore-emr-serverless-2.5.2.post3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-04 12:37:42.015771 types-aiobotocore-emr-serverless-2.5.2.post3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2120 2023-08-04 12:23:32.000000 types-aiobotocore-emr-serverless-2.5.2.post3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:37:42.011771 types-aiobotocore-emr-serverless-2.5.2.post3/types_aiobotocore_emr_serverless/
--rw-r--r--   0 runner    (1001) docker     (123)      876 2023-08-04 12:23:32.000000 types-aiobotocore-emr-serverless-2.5.2.post3/types_aiobotocore_emr_serverless/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      875 2023-08-04 12:23:32.000000 types-aiobotocore-emr-serverless-2.5.2.post3/types_aiobotocore_emr_serverless/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      969 2023-08-04 12:23:32.000000 types-aiobotocore-emr-serverless-2.5.2.post3/types_aiobotocore_emr_serverless/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15541 2023-08-04 12:23:32.000000 types-aiobotocore-emr-serverless-2.5.2.post3/types_aiobotocore_emr_serverless/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    15515 2023-08-04 12:23:32.000000 types-aiobotocore-emr-serverless-2.5.2.post3/types_aiobotocore_emr_serverless/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8575 2023-08-04 12:23:32.000000 types-aiobotocore-emr-serverless-2.5.2.post3/types_aiobotocore_emr_serverless/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     8573 2023-08-04 12:23:32.000000 types-aiobotocore-emr-serverless-2.5.2.post3/types_aiobotocore_emr_serverless/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     3514 2023-08-04 12:23:32.000000 types-aiobotocore-emr-serverless-2.5.2.post3/types_aiobotocore_emr_serverless/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     3510 2023-08-04 12:23:32.000000 types-aiobotocore-emr-serverless-2.5.2.post3/types_aiobotocore_emr_serverless/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 12:23:32.000000 types-aiobotocore-emr-serverless-2.5.2.post3/types_aiobotocore_emr_serverless/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    19974 2023-08-04 12:23:32.000000 types-aiobotocore-emr-serverless-2.5.2.post3/types_aiobotocore_emr_serverless/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    19941 2023-08-04 12:23:32.000000 types-aiobotocore-emr-serverless-2.5.2.post3/types_aiobotocore_emr_serverless/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-04 12:23:32.000000 types-aiobotocore-emr-serverless-2.5.2.post3/types_aiobotocore_emr_serverless/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:37:42.015771 types-aiobotocore-emr-serverless-2.5.2.post3/types_aiobotocore_emr_serverless.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    13460 2023-08-04 12:37:41.000000 types-aiobotocore-emr-serverless-2.5.2.post3/types_aiobotocore_emr_serverless.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      946 2023-08-04 12:37:41.000000 types-aiobotocore-emr-serverless-2.5.2.post3/types_aiobotocore_emr_serverless.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 12:37:41.000000 types-aiobotocore-emr-serverless-2.5.2.post3/types_aiobotocore_emr_serverless.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 12:37:41.000000 types-aiobotocore-emr-serverless-2.5.2.post3/types_aiobotocore_emr_serverless.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-04 12:37:41.000000 types-aiobotocore-emr-serverless-2.5.2.post3/types_aiobotocore_emr_serverless.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-08-04 12:37:41.000000 types-aiobotocore-emr-serverless-2.5.2.post3/types_aiobotocore_emr_serverless.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:23:42.962713 types-aiobotocore-emr-serverless-2.5.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-08 01:10:55.000000 types-aiobotocore-emr-serverless-2.5.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    13454 2023-08-08 01:23:42.958713 types-aiobotocore-emr-serverless-2.5.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    11915 2023-08-08 01:10:55.000000 types-aiobotocore-emr-serverless-2.5.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-08 01:23:42.962713 types-aiobotocore-emr-serverless-2.5.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2114 2023-08-08 01:10:55.000000 types-aiobotocore-emr-serverless-2.5.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:23:42.954713 types-aiobotocore-emr-serverless-2.5.4/types_aiobotocore_emr_serverless/
+-rw-r--r--   0 runner    (1001) docker     (123)      876 2023-08-08 01:10:55.000000 types-aiobotocore-emr-serverless-2.5.4/types_aiobotocore_emr_serverless/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      875 2023-08-08 01:10:55.000000 types-aiobotocore-emr-serverless-2.5.4/types_aiobotocore_emr_serverless/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      957 2023-08-08 01:10:56.000000 types-aiobotocore-emr-serverless-2.5.4/types_aiobotocore_emr_serverless/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15623 2023-08-08 01:10:56.000000 types-aiobotocore-emr-serverless-2.5.4/types_aiobotocore_emr_serverless/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15597 2023-08-08 01:10:56.000000 types-aiobotocore-emr-serverless-2.5.4/types_aiobotocore_emr_serverless/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8670 2023-08-08 01:10:57.000000 types-aiobotocore-emr-serverless-2.5.4/types_aiobotocore_emr_serverless/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8668 2023-08-08 01:10:57.000000 types-aiobotocore-emr-serverless-2.5.4/types_aiobotocore_emr_serverless/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     3514 2023-08-08 01:10:56.000000 types-aiobotocore-emr-serverless-2.5.4/types_aiobotocore_emr_serverless/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3510 2023-08-08 01:10:56.000000 types-aiobotocore-emr-serverless-2.5.4/types_aiobotocore_emr_serverless/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 01:10:56.000000 types-aiobotocore-emr-serverless-2.5.4/types_aiobotocore_emr_serverless/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    20729 2023-08-08 01:10:57.000000 types-aiobotocore-emr-serverless-2.5.4/types_aiobotocore_emr_serverless/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20694 2023-08-08 01:10:57.000000 types-aiobotocore-emr-serverless-2.5.4/types_aiobotocore_emr_serverless/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-08-08 01:10:55.000000 types-aiobotocore-emr-serverless-2.5.4/types_aiobotocore_emr_serverless/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:23:42.958713 types-aiobotocore-emr-serverless-2.5.4/types_aiobotocore_emr_serverless.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    13454 2023-08-08 01:23:42.000000 types-aiobotocore-emr-serverless-2.5.4/types_aiobotocore_emr_serverless.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      946 2023-08-08 01:23:42.000000 types-aiobotocore-emr-serverless-2.5.4/types_aiobotocore_emr_serverless.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 01:23:42.000000 types-aiobotocore-emr-serverless-2.5.4/types_aiobotocore_emr_serverless.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 01:23:42.000000 types-aiobotocore-emr-serverless-2.5.4/types_aiobotocore_emr_serverless.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-08 01:23:42.000000 types-aiobotocore-emr-serverless-2.5.4/types_aiobotocore_emr_serverless.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-08-08 01:23:42.000000 types-aiobotocore-emr-serverless-2.5.4/types_aiobotocore_emr_serverless.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-emr-serverless-2.5.2.post3/LICENSE` & `types-aiobotocore-emr-serverless-2.5.4/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-emr-serverless-2.5.2.post3/PKG-INFO` & `types-aiobotocore-emr-serverless-2.5.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-emr-serverless
-Version: 2.5.2.post3
-Summary: Type annotations for aiobotocore.EMRServerless 2.5.2 service generated with mypy-boto3-builder 7.17.2
+Version: 2.5.4
+Summary: Type annotations for aiobotocore.EMRServerless 2.5.4 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_emr_serverless/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-emr-serverless.svg?color=blue)](https://pypi.org/project/types-aiobotocore-emr-serverless)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_emr_serverless/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-emr-serverless)](https://pepy.tech/project/types-aiobotocore-emr-serverless)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.EMRServerless 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr-serverless.html#EMRServerless)
+[aiobotocore.EMRServerless 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr-serverless.html#EMRServerless)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-emr-serverless-2.5.2.post3/README.md` & `types-aiobotocore-emr-serverless-2.5.4/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-emr-serverless.svg?color=blue)](https://pypi.org/project/types-aiobotocore-emr-serverless)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_emr_serverless/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-emr-serverless)](https://pepy.tech/project/types-aiobotocore-emr-serverless)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.EMRServerless 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr-serverless.html#EMRServerless)
+[aiobotocore.EMRServerless 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr-serverless.html#EMRServerless)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-emr-serverless-2.5.2.post3/setup.py` & `types-aiobotocore-emr-serverless-2.5.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-emr-serverless",
-    version="2.5.2.post3",
+    version="2.5.4",
     packages=["types_aiobotocore_emr_serverless"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.EMRServerless 2.5.2 service generated with"
+        "Type annotations for aiobotocore.EMRServerless 2.5.4 service generated with"
         " mypy-boto3-builder 7.17.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
```

### Comparing `types-aiobotocore-emr-serverless-2.5.2.post3/types_aiobotocore_emr_serverless/__init__.py` & `types-aiobotocore-emr-serverless-2.5.4/types_aiobotocore_emr_serverless/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-emr-serverless-2.5.2.post3/types_aiobotocore_emr_serverless/__init__.pyi` & `types-aiobotocore-emr-serverless-2.5.4/types_aiobotocore_emr_serverless/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-emr-serverless-2.5.2.post3/types_aiobotocore_emr_serverless/__main__.py` & `types-aiobotocore-emr-serverless-2.5.4/types_aiobotocore_emr_serverless/__main__.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.EMRServerless 2.5.2\nVersion:        "
-        " 2.5.2.post3\nBuilder version: 7.17.2\nDocs:           "
+        "Type annotations for aiobotocore.EMRServerless 2.5.4\nVersion:         2.5.4\nBuilder"
+        " version: 7.17.2\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_emr_serverless//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr-serverless.html#EMRServerless\nOther"
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

### Comparing `types-aiobotocore-emr-serverless-2.5.2.post3/types_aiobotocore_emr_serverless/client.py` & `types-aiobotocore-emr-serverless-2.5.4/types_aiobotocore_emr_serverless/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -168,15 +168,16 @@
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_emr_serverless/client/#get_application)
         """
 
     async def get_dashboard_for_job_run(
         self, *, applicationId: str, jobRunId: str
     ) -> GetDashboardForJobRunResponseTypeDef:
         """
-        Returns a URL to access the job run dashboard.
+        Creates and returns a URL that you can use to access the application UIs for a
+        job run.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr-serverless.html#EMRServerless.Client.get_dashboard_for_job_run)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_emr_serverless/client/#get_dashboard_for_job_run)
         """
 
     async def get_job_run(self, *, applicationId: str, jobRunId: str) -> GetJobRunResponseTypeDef:
         """
@@ -286,15 +287,16 @@
         initialCapacity: Mapping[str, InitialCapacityConfigTypeDef] = ...,
         maximumCapacity: MaximumAllowedResourcesTypeDef = ...,
         autoStartConfiguration: AutoStartConfigTypeDef = ...,
         autoStopConfiguration: AutoStopConfigTypeDef = ...,
         networkConfiguration: NetworkConfigurationTypeDef = ...,
         architecture: ArchitectureType = ...,
         imageConfiguration: ImageConfigurationInputTypeDef = ...,
-        workerTypeSpecifications: Mapping[str, WorkerTypeSpecificationInputTypeDef] = ...
+        workerTypeSpecifications: Mapping[str, WorkerTypeSpecificationInputTypeDef] = ...,
+        releaseLabel: str = ...
     ) -> UpdateApplicationResponseTypeDef:
         """
         Updates a specified application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr-serverless.html#EMRServerless.Client.update_application)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_emr_serverless/client/#update_application)
         """
```

### Comparing `types-aiobotocore-emr-serverless-2.5.2.post3/types_aiobotocore_emr_serverless/client.pyi` & `types-aiobotocore-emr-serverless-2.5.4/types_aiobotocore_emr_serverless/client.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -156,15 +156,16 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr-serverless.html#EMRServerless.Client.get_application)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_emr_serverless/client/#get_application)
         """
     async def get_dashboard_for_job_run(
         self, *, applicationId: str, jobRunId: str
     ) -> GetDashboardForJobRunResponseTypeDef:
         """
-        Returns a URL to access the job run dashboard.
+        Creates and returns a URL that you can use to access the application UIs for a
+        job run.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr-serverless.html#EMRServerless.Client.get_dashboard_for_job_run)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_emr_serverless/client/#get_dashboard_for_job_run)
         """
     async def get_job_run(self, *, applicationId: str, jobRunId: str) -> GetJobRunResponseTypeDef:
         """
         Displays detailed information about a job run.
@@ -264,15 +265,16 @@
         initialCapacity: Mapping[str, InitialCapacityConfigTypeDef] = ...,
         maximumCapacity: MaximumAllowedResourcesTypeDef = ...,
         autoStartConfiguration: AutoStartConfigTypeDef = ...,
         autoStopConfiguration: AutoStopConfigTypeDef = ...,
         networkConfiguration: NetworkConfigurationTypeDef = ...,
         architecture: ArchitectureType = ...,
         imageConfiguration: ImageConfigurationInputTypeDef = ...,
-        workerTypeSpecifications: Mapping[str, WorkerTypeSpecificationInputTypeDef] = ...
+        workerTypeSpecifications: Mapping[str, WorkerTypeSpecificationInputTypeDef] = ...,
+        releaseLabel: str = ...
     ) -> UpdateApplicationResponseTypeDef:
         """
         Updates a specified application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr-serverless.html#EMRServerless.Client.update_application)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_emr_serverless/client/#update_application)
         """
```

### Comparing `types-aiobotocore-emr-serverless-2.5.2.post3/types_aiobotocore_emr_serverless/literals.py` & `types-aiobotocore-emr-serverless-2.5.4/types_aiobotocore_emr_serverless/literals.py`

 * *Files 2% similar despite different names*

```diff
@@ -54,14 +54,15 @@
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
@@ -157,14 +158,15 @@
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
@@ -243,26 +245,28 @@
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

### Comparing `types-aiobotocore-emr-serverless-2.5.2.post3/types_aiobotocore_emr_serverless/literals.pyi` & `types-aiobotocore-emr-serverless-2.5.4/types_aiobotocore_emr_serverless/literals.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -52,14 +52,15 @@
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
@@ -155,14 +156,15 @@
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
@@ -241,26 +243,28 @@
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

### Comparing `types-aiobotocore-emr-serverless-2.5.2.post3/types_aiobotocore_emr_serverless/paginator.py` & `types-aiobotocore-emr-serverless-2.5.4/types_aiobotocore_emr_serverless/paginator.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-emr-serverless-2.5.2.post3/types_aiobotocore_emr_serverless/paginator.pyi` & `types-aiobotocore-emr-serverless-2.5.4/types_aiobotocore_emr_serverless/paginator.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-emr-serverless-2.5.2.post3/types_aiobotocore_emr_serverless/type_defs.py` & `types-aiobotocore-emr-serverless-2.5.4/types_aiobotocore_emr_serverless/type_defs.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,14 +28,15 @@
     "AutoStartConfigTypeDef",
     "AutoStopConfigTypeDef",
     "ImageConfigurationTypeDef",
     "MaximumAllowedResourcesTypeDef",
     "NetworkConfigurationTypeDef",
     "CancelJobRunRequestRequestTypeDef",
     "ResponseMetadataTypeDef",
+    "CloudWatchLoggingConfigurationTypeDef",
     "ConfigurationTypeDef",
     "ImageConfigurationInputTypeDef",
     "DeleteApplicationRequestRequestTypeDef",
     "GetApplicationRequestRequestTypeDef",
     "GetDashboardForJobRunRequestRequestTypeDef",
     "GetJobRunRequestRequestTypeDef",
     "HiveTypeDef",
@@ -193,14 +194,38 @@
         "HostId": str,
         "HTTPStatusCode": int,
         "HTTPHeaders": Dict[str, str],
         "RetryAttempts": int,
     },
 )
 
+_RequiredCloudWatchLoggingConfigurationTypeDef = TypedDict(
+    "_RequiredCloudWatchLoggingConfigurationTypeDef",
+    {
+        "enabled": bool,
+    },
+)
+_OptionalCloudWatchLoggingConfigurationTypeDef = TypedDict(
+    "_OptionalCloudWatchLoggingConfigurationTypeDef",
+    {
+        "logGroupName": str,
+        "logStreamNamePrefix": str,
+        "encryptionKeyArn": str,
+        "logTypes": Dict[str, List[str]],
+    },
+    total=False,
+)
+
+
+class CloudWatchLoggingConfigurationTypeDef(
+    _RequiredCloudWatchLoggingConfigurationTypeDef, _OptionalCloudWatchLoggingConfigurationTypeDef
+):
+    pass
+
+
 _RequiredConfigurationTypeDef = TypedDict(
     "_RequiredConfigurationTypeDef",
     {
         "classification": str,
     },
 )
 _OptionalConfigurationTypeDef = TypedDict(
@@ -613,14 +638,15 @@
 MonitoringConfigurationTypeDef = TypedDict(
     "MonitoringConfigurationTypeDef",
     {
         "s3MonitoringConfiguration": S3MonitoringConfigurationTypeDef,
         "managedPersistenceMonitoringConfiguration": (
             ManagedPersistenceMonitoringConfigurationTypeDef
         ),
+        "cloudWatchLoggingConfiguration": CloudWatchLoggingConfigurationTypeDef,
     },
     total=False,
 )
 
 _RequiredApplicationTypeDef = TypedDict(
     "_RequiredApplicationTypeDef",
     {
@@ -702,14 +728,15 @@
         "maximumCapacity": MaximumAllowedResourcesTypeDef,
         "autoStartConfiguration": AutoStartConfigTypeDef,
         "autoStopConfiguration": AutoStopConfigTypeDef,
         "networkConfiguration": NetworkConfigurationTypeDef,
         "architecture": ArchitectureType,
         "imageConfiguration": ImageConfigurationInputTypeDef,
         "workerTypeSpecifications": Mapping[str, WorkerTypeSpecificationInputTypeDef],
+        "releaseLabel": str,
     },
     total=False,
 )
 
 
 class UpdateApplicationRequestRequestTypeDef(
     _RequiredUpdateApplicationRequestRequestTypeDef, _OptionalUpdateApplicationRequestRequestTypeDef
```

### Comparing `types-aiobotocore-emr-serverless-2.5.2.post3/types_aiobotocore_emr_serverless/type_defs.pyi` & `types-aiobotocore-emr-serverless-2.5.4/types_aiobotocore_emr_serverless/type_defs.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -27,14 +27,15 @@
     "AutoStartConfigTypeDef",
     "AutoStopConfigTypeDef",
     "ImageConfigurationTypeDef",
     "MaximumAllowedResourcesTypeDef",
     "NetworkConfigurationTypeDef",
     "CancelJobRunRequestRequestTypeDef",
     "ResponseMetadataTypeDef",
+    "CloudWatchLoggingConfigurationTypeDef",
     "ConfigurationTypeDef",
     "ImageConfigurationInputTypeDef",
     "DeleteApplicationRequestRequestTypeDef",
     "GetApplicationRequestRequestTypeDef",
     "GetDashboardForJobRunRequestRequestTypeDef",
     "GetJobRunRequestRequestTypeDef",
     "HiveTypeDef",
@@ -186,14 +187,36 @@
         "HostId": str,
         "HTTPStatusCode": int,
         "HTTPHeaders": Dict[str, str],
         "RetryAttempts": int,
     },
 )
 
+_RequiredCloudWatchLoggingConfigurationTypeDef = TypedDict(
+    "_RequiredCloudWatchLoggingConfigurationTypeDef",
+    {
+        "enabled": bool,
+    },
+)
+_OptionalCloudWatchLoggingConfigurationTypeDef = TypedDict(
+    "_OptionalCloudWatchLoggingConfigurationTypeDef",
+    {
+        "logGroupName": str,
+        "logStreamNamePrefix": str,
+        "encryptionKeyArn": str,
+        "logTypes": Dict[str, List[str]],
+    },
+    total=False,
+)
+
+class CloudWatchLoggingConfigurationTypeDef(
+    _RequiredCloudWatchLoggingConfigurationTypeDef, _OptionalCloudWatchLoggingConfigurationTypeDef
+):
+    pass
+
 _RequiredConfigurationTypeDef = TypedDict(
     "_RequiredConfigurationTypeDef",
     {
         "classification": str,
     },
 )
 _OptionalConfigurationTypeDef = TypedDict(
@@ -590,14 +613,15 @@
 MonitoringConfigurationTypeDef = TypedDict(
     "MonitoringConfigurationTypeDef",
     {
         "s3MonitoringConfiguration": S3MonitoringConfigurationTypeDef,
         "managedPersistenceMonitoringConfiguration": (
             ManagedPersistenceMonitoringConfigurationTypeDef
         ),
+        "cloudWatchLoggingConfiguration": CloudWatchLoggingConfigurationTypeDef,
     },
     total=False,
 )
 
 _RequiredApplicationTypeDef = TypedDict(
     "_RequiredApplicationTypeDef",
     {
@@ -675,14 +699,15 @@
         "maximumCapacity": MaximumAllowedResourcesTypeDef,
         "autoStartConfiguration": AutoStartConfigTypeDef,
         "autoStopConfiguration": AutoStopConfigTypeDef,
         "networkConfiguration": NetworkConfigurationTypeDef,
         "architecture": ArchitectureType,
         "imageConfiguration": ImageConfigurationInputTypeDef,
         "workerTypeSpecifications": Mapping[str, WorkerTypeSpecificationInputTypeDef],
+        "releaseLabel": str,
     },
     total=False,
 )
 
 class UpdateApplicationRequestRequestTypeDef(
     _RequiredUpdateApplicationRequestRequestTypeDef, _OptionalUpdateApplicationRequestRequestTypeDef
 ):
```

### Comparing `types-aiobotocore-emr-serverless-2.5.2.post3/types_aiobotocore_emr_serverless.egg-info/PKG-INFO` & `types-aiobotocore-emr-serverless-2.5.4/types_aiobotocore_emr_serverless.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-emr-serverless
-Version: 2.5.2.post3
-Summary: Type annotations for aiobotocore.EMRServerless 2.5.2 service generated with mypy-boto3-builder 7.17.2
+Version: 2.5.4
+Summary: Type annotations for aiobotocore.EMRServerless 2.5.4 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_emr_serverless/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-emr-serverless.svg?color=blue)](https://pypi.org/project/types-aiobotocore-emr-serverless)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_emr_serverless/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-emr-serverless)](https://pepy.tech/project/types-aiobotocore-emr-serverless)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.EMRServerless 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr-serverless.html#EMRServerless)
+[aiobotocore.EMRServerless 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr-serverless.html#EMRServerless)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-emr-serverless-2.5.2.post3/types_aiobotocore_emr_serverless.egg-info/SOURCES.txt` & `types-aiobotocore-emr-serverless-2.5.4/types_aiobotocore_emr_serverless.egg-info/SOURCES.txt`

 * *Files identical despite different names*


# Comparing `tmp/types-aiobotocore-codeguru-security-2.5.2.post3.tar.gz` & `tmp/types-aiobotocore-codeguru-security-2.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-codeguru-security-2.5.2.post3.tar", last modified: Fri Aug  4 12:37:28 2023, max compression
+gzip compressed data, was "types-aiobotocore-codeguru-security-2.5.4.tar", last modified: Tue Aug  8 01:23:29 2023, max compression
```

## Comparing `types-aiobotocore-codeguru-security-2.5.2.post3.tar` & `types-aiobotocore-codeguru-security-2.5.4.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:37:28.879455 types-aiobotocore-codeguru-security-2.5.2.post3/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-04 12:20:17.000000 types-aiobotocore-codeguru-security-2.5.2.post3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    13771 2023-08-04 12:37:28.879455 types-aiobotocore-codeguru-security-2.5.2.post3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    12214 2023-08-04 12:20:17.000000 types-aiobotocore-codeguru-security-2.5.2.post3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-04 12:37:28.879455 types-aiobotocore-codeguru-security-2.5.2.post3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2141 2023-08-04 12:20:17.000000 types-aiobotocore-codeguru-security-2.5.2.post3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:37:28.875455 types-aiobotocore-codeguru-security-2.5.2.post3/types_aiobotocore_codeguru_security/
--rw-r--r--   0 runner    (1001) docker     (123)     1093 2023-08-04 12:20:17.000000 types-aiobotocore-codeguru-security-2.5.2.post3/types_aiobotocore_codeguru_security/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1092 2023-08-04 12:20:17.000000 types-aiobotocore-codeguru-security-2.5.2.post3/types_aiobotocore_codeguru_security/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      981 2023-08-04 12:20:17.000000 types-aiobotocore-codeguru-security-2.5.2.post3/types_aiobotocore_codeguru_security/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14227 2023-08-04 12:20:17.000000 types-aiobotocore-codeguru-security-2.5.2.post3/types_aiobotocore_codeguru_security/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    14202 2023-08-04 12:20:17.000000 types-aiobotocore-codeguru-security-2.5.2.post3/types_aiobotocore_codeguru_security/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8485 2023-08-04 12:20:17.000000 types-aiobotocore-codeguru-security-2.5.2.post3/types_aiobotocore_codeguru_security/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     8483 2023-08-04 12:20:17.000000 types-aiobotocore-codeguru-security-2.5.2.post3/types_aiobotocore_codeguru_security/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     4523 2023-08-04 12:20:17.000000 types-aiobotocore-codeguru-security-2.5.2.post3/types_aiobotocore_codeguru_security/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     4518 2023-08-04 12:20:17.000000 types-aiobotocore-codeguru-security-2.5.2.post3/types_aiobotocore_codeguru_security/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 12:20:17.000000 types-aiobotocore-codeguru-security-2.5.2.post3/types_aiobotocore_codeguru_security/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    14789 2023-08-04 12:20:17.000000 types-aiobotocore-codeguru-security-2.5.2.post3/types_aiobotocore_codeguru_security/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    14774 2023-08-04 12:20:17.000000 types-aiobotocore-codeguru-security-2.5.2.post3/types_aiobotocore_codeguru_security/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-04 12:20:17.000000 types-aiobotocore-codeguru-security-2.5.2.post3/types_aiobotocore_codeguru_security/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:37:28.879455 types-aiobotocore-codeguru-security-2.5.2.post3/types_aiobotocore_codeguru_security.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    13771 2023-08-04 12:37:28.000000 types-aiobotocore-codeguru-security-2.5.2.post3/types_aiobotocore_codeguru_security.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1003 2023-08-04 12:37:28.000000 types-aiobotocore-codeguru-security-2.5.2.post3/types_aiobotocore_codeguru_security.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 12:37:28.000000 types-aiobotocore-codeguru-security-2.5.2.post3/types_aiobotocore_codeguru_security.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 12:37:28.000000 types-aiobotocore-codeguru-security-2.5.2.post3/types_aiobotocore_codeguru_security.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-04 12:37:28.000000 types-aiobotocore-codeguru-security-2.5.2.post3/types_aiobotocore_codeguru_security.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-08-04 12:37:28.000000 types-aiobotocore-codeguru-security-2.5.2.post3/types_aiobotocore_codeguru_security.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:23:29.030646 types-aiobotocore-codeguru-security-2.5.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-08 01:07:55.000000 types-aiobotocore-codeguru-security-2.5.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    13765 2023-08-08 01:23:29.030646 types-aiobotocore-codeguru-security-2.5.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    12214 2023-08-08 01:07:55.000000 types-aiobotocore-codeguru-security-2.5.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-08 01:23:29.030646 types-aiobotocore-codeguru-security-2.5.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2135 2023-08-08 01:07:55.000000 types-aiobotocore-codeguru-security-2.5.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:23:29.030646 types-aiobotocore-codeguru-security-2.5.4/types_aiobotocore_codeguru_security/
+-rw-r--r--   0 runner    (1001) docker     (123)     1093 2023-08-08 01:07:55.000000 types-aiobotocore-codeguru-security-2.5.4/types_aiobotocore_codeguru_security/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1092 2023-08-08 01:07:55.000000 types-aiobotocore-codeguru-security-2.5.4/types_aiobotocore_codeguru_security/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      969 2023-08-08 01:07:55.000000 types-aiobotocore-codeguru-security-2.5.4/types_aiobotocore_codeguru_security/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14236 2023-08-08 01:07:55.000000 types-aiobotocore-codeguru-security-2.5.4/types_aiobotocore_codeguru_security/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14211 2023-08-08 01:07:55.000000 types-aiobotocore-codeguru-security-2.5.4/types_aiobotocore_codeguru_security/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8580 2023-08-08 01:07:56.000000 types-aiobotocore-codeguru-security-2.5.4/types_aiobotocore_codeguru_security/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8578 2023-08-08 01:07:56.000000 types-aiobotocore-codeguru-security-2.5.4/types_aiobotocore_codeguru_security/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     4523 2023-08-08 01:07:55.000000 types-aiobotocore-codeguru-security-2.5.4/types_aiobotocore_codeguru_security/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4518 2023-08-08 01:07:55.000000 types-aiobotocore-codeguru-security-2.5.4/types_aiobotocore_codeguru_security/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 01:07:55.000000 types-aiobotocore-codeguru-security-2.5.4/types_aiobotocore_codeguru_security/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    14789 2023-08-08 01:07:57.000000 types-aiobotocore-codeguru-security-2.5.4/types_aiobotocore_codeguru_security/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14774 2023-08-08 01:07:56.000000 types-aiobotocore-codeguru-security-2.5.4/types_aiobotocore_codeguru_security/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-08-08 01:07:55.000000 types-aiobotocore-codeguru-security-2.5.4/types_aiobotocore_codeguru_security/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:23:29.030646 types-aiobotocore-codeguru-security-2.5.4/types_aiobotocore_codeguru_security.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    13765 2023-08-08 01:23:28.000000 types-aiobotocore-codeguru-security-2.5.4/types_aiobotocore_codeguru_security.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1003 2023-08-08 01:23:28.000000 types-aiobotocore-codeguru-security-2.5.4/types_aiobotocore_codeguru_security.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 01:23:28.000000 types-aiobotocore-codeguru-security-2.5.4/types_aiobotocore_codeguru_security.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 01:23:28.000000 types-aiobotocore-codeguru-security-2.5.4/types_aiobotocore_codeguru_security.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-08 01:23:28.000000 types-aiobotocore-codeguru-security-2.5.4/types_aiobotocore_codeguru_security.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-08-08 01:23:28.000000 types-aiobotocore-codeguru-security-2.5.4/types_aiobotocore_codeguru_security.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-codeguru-security-2.5.2.post3/LICENSE` & `types-aiobotocore-codeguru-security-2.5.4/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-codeguru-security-2.5.2.post3/PKG-INFO` & `types-aiobotocore-codeguru-security-2.5.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-codeguru-security
-Version: 2.5.2.post3
-Summary: Type annotations for aiobotocore.CodeGuruSecurity 2.5.2 service generated with mypy-boto3-builder 7.17.2
+Version: 2.5.4
+Summary: Type annotations for aiobotocore.CodeGuruSecurity 2.5.4 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codeguru_security/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-codeguru-security.svg?color=blue)](https://pypi.org/project/types-aiobotocore-codeguru-security)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codeguru_security/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-codeguru-security)](https://pepy.tech/project/types-aiobotocore-codeguru-security)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.CodeGuruSecurity 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeguru-security.html#CodeGuruSecurity)
+[aiobotocore.CodeGuruSecurity 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeguru-security.html#CodeGuruSecurity)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-codeguru-security-2.5.2.post3/README.md` & `types-aiobotocore-codeguru-security-2.5.4/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-codeguru-security.svg?color=blue)](https://pypi.org/project/types-aiobotocore-codeguru-security)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codeguru_security/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-codeguru-security)](https://pepy.tech/project/types-aiobotocore-codeguru-security)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.CodeGuruSecurity 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeguru-security.html#CodeGuruSecurity)
+[aiobotocore.CodeGuruSecurity 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeguru-security.html#CodeGuruSecurity)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-codeguru-security-2.5.2.post3/setup.py` & `types-aiobotocore-codeguru-security-2.5.4/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-codeguru-security",
-    version="2.5.2.post3",
+    version="2.5.4",
     packages=["types_aiobotocore_codeguru_security"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.CodeGuruSecurity 2.5.2 service generated with"
+        "Type annotations for aiobotocore.CodeGuruSecurity 2.5.4 service generated with"
         " mypy-boto3-builder 7.17.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
```

### Comparing `types-aiobotocore-codeguru-security-2.5.2.post3/types_aiobotocore_codeguru_security/__init__.py` & `types-aiobotocore-codeguru-security-2.5.4/types_aiobotocore_codeguru_security/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-codeguru-security-2.5.2.post3/types_aiobotocore_codeguru_security/__init__.pyi` & `types-aiobotocore-codeguru-security-2.5.4/types_aiobotocore_codeguru_security/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-codeguru-security-2.5.2.post3/types_aiobotocore_codeguru_security/__main__.py` & `types-aiobotocore-codeguru-security-2.5.4/types_aiobotocore_codeguru_security/__main__.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.CodeGuruSecurity 2.5.2\nVersion:        "
-        " 2.5.2.post3\nBuilder version: 7.17.2\nDocs:           "
+        "Type annotations for aiobotocore.CodeGuruSecurity 2.5.4\nVersion:         2.5.4\nBuilder"
+        " version: 7.17.2\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codeguru_security//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeguru-security.html#CodeGuruSecurity\nOther"
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

### Comparing `types-aiobotocore-codeguru-security-2.5.2.post3/types_aiobotocore_codeguru_security/client.py` & `types-aiobotocore-codeguru-security-2.5.4/types_aiobotocore_codeguru_security/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -207,15 +207,15 @@
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codeguru_security/client/#list_findings_metrics)
         """
 
     async def list_scans(
         self, *, maxResults: int = ..., nextToken: str = ...
     ) -> ListScansResponseTypeDef:
         """
-        Returns a list of all the scans in an account.
+        Returns a list of all the standard scans in an account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeguru-security.html#CodeGuruSecurity.Client.list_scans)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codeguru_security/client/#list_scans)
         """
 
     async def list_tags_for_resource(
         self, *, resourceArn: str
```

### Comparing `types-aiobotocore-codeguru-security-2.5.2.post3/types_aiobotocore_codeguru_security/client.pyi` & `types-aiobotocore-codeguru-security-2.5.4/types_aiobotocore_codeguru_security/client.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -191,15 +191,15 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeguru-security.html#CodeGuruSecurity.Client.list_findings_metrics)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codeguru_security/client/#list_findings_metrics)
         """
     async def list_scans(
         self, *, maxResults: int = ..., nextToken: str = ...
     ) -> ListScansResponseTypeDef:
         """
-        Returns a list of all the scans in an account.
+        Returns a list of all the standard scans in an account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeguru-security.html#CodeGuruSecurity.Client.list_scans)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codeguru_security/client/#list_scans)
         """
     async def list_tags_for_resource(
         self, *, resourceArn: str
     ) -> ListTagsForResourceResponseTypeDef:
```

### Comparing `types-aiobotocore-codeguru-security-2.5.2.post3/types_aiobotocore_codeguru_security/literals.py` & `types-aiobotocore-codeguru-security-2.5.4/types_aiobotocore_codeguru_security/literals.pyi`

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
     "AnalysisTypeType",
     "ErrorCodeType",
     "GetFindingsPaginatorName",
     "ListFindingsMetricsPaginatorName",
     "ListScansPaginatorName",
     "ScanStateType",
@@ -31,15 +30,14 @@
     "StatusType",
     "CodeGuruSecurityServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
 )
 
-
 AnalysisTypeType = Literal["All", "Security"]
 ErrorCodeType = Literal[
     "DUPLICATE_IDENTIFIER",
     "INTERNAL_ERROR",
     "INVALID_FINDING_ID",
     "INVALID_SCAN_NAME",
     "ITEM_DOES_NOT_EXIST",
@@ -63,14 +61,15 @@
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
@@ -166,14 +165,15 @@
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
@@ -252,26 +252,28 @@
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

### Comparing `types-aiobotocore-codeguru-security-2.5.2.post3/types_aiobotocore_codeguru_security/literals.pyi` & `types-aiobotocore-codeguru-security-2.5.4/types_aiobotocore_codeguru_security/literals.py`

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
     "AnalysisTypeType",
     "ErrorCodeType",
     "GetFindingsPaginatorName",
     "ListFindingsMetricsPaginatorName",
     "ListScansPaginatorName",
     "ScanStateType",
@@ -30,14 +31,15 @@
     "StatusType",
     "CodeGuruSecurityServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
 )
 
+
 AnalysisTypeType = Literal["All", "Security"]
 ErrorCodeType = Literal[
     "DUPLICATE_IDENTIFIER",
     "INTERNAL_ERROR",
     "INVALID_FINDING_ID",
     "INVALID_SCAN_NAME",
     "ITEM_DOES_NOT_EXIST",
@@ -61,14 +63,15 @@
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
@@ -164,14 +167,15 @@
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
@@ -250,26 +254,28 @@
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

### Comparing `types-aiobotocore-codeguru-security-2.5.2.post3/types_aiobotocore_codeguru_security/paginator.py` & `types-aiobotocore-codeguru-security-2.5.4/types_aiobotocore_codeguru_security/paginator.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-codeguru-security-2.5.2.post3/types_aiobotocore_codeguru_security/paginator.pyi` & `types-aiobotocore-codeguru-security-2.5.4/types_aiobotocore_codeguru_security/paginator.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-codeguru-security-2.5.2.post3/types_aiobotocore_codeguru_security/type_defs.py` & `types-aiobotocore-codeguru-security-2.5.4/types_aiobotocore_codeguru_security/type_defs.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-codeguru-security-2.5.2.post3/types_aiobotocore_codeguru_security/type_defs.pyi` & `types-aiobotocore-codeguru-security-2.5.4/types_aiobotocore_codeguru_security/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-codeguru-security-2.5.2.post3/types_aiobotocore_codeguru_security.egg-info/PKG-INFO` & `types-aiobotocore-codeguru-security-2.5.4/types_aiobotocore_codeguru_security.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-codeguru-security
-Version: 2.5.2.post3
-Summary: Type annotations for aiobotocore.CodeGuruSecurity 2.5.2 service generated with mypy-boto3-builder 7.17.2
+Version: 2.5.4
+Summary: Type annotations for aiobotocore.CodeGuruSecurity 2.5.4 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codeguru_security/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-codeguru-security.svg?color=blue)](https://pypi.org/project/types-aiobotocore-codeguru-security)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codeguru_security/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-codeguru-security)](https://pepy.tech/project/types-aiobotocore-codeguru-security)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.CodeGuruSecurity 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeguru-security.html#CodeGuruSecurity)
+[aiobotocore.CodeGuruSecurity 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeguru-security.html#CodeGuruSecurity)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-codeguru-security-2.5.2.post3/types_aiobotocore_codeguru_security.egg-info/SOURCES.txt` & `types-aiobotocore-codeguru-security-2.5.4/types_aiobotocore_codeguru_security.egg-info/SOURCES.txt`

 * *Files identical despite different names*


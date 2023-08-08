# Comparing `tmp/types-aiobotocore-migrationhuborchestrator-2.5.2.post2.tar.gz` & `tmp/types-aiobotocore-migrationhuborchestrator-2.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-migrationhuborchestrator-2.5.2.post2.tar", last modified: Fri Aug  4 13:59:19 2023, max compression
+gzip compressed data, was "types-aiobotocore-migrationhuborchestrator-2.5.4.tar", last modified: Tue Aug  8 01:24:08 2023, max compression
```

## Comparing `types-aiobotocore-migrationhuborchestrator-2.5.2.post2.tar` & `types-aiobotocore-migrationhuborchestrator-2.5.4.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:19.076643 types-aiobotocore-migrationhuborchestrator-2.5.2.post2/
--rw-r--r--   0 vlad      (1000) vlad      (1000)     1070 2023-08-04 13:45:08.000000 types-aiobotocore-migrationhuborchestrator-2.5.2.post2/LICENSE
--rw-r--r--   0 vlad      (1000) vlad      (1000)    14781 2023-08-04 13:59:19.076643 types-aiobotocore-migrationhuborchestrator-2.5.2.post2/PKG-INFO
--rw-r--r--   0 vlad      (1000) vlad      (1000)    13195 2023-08-04 13:45:08.000000 types-aiobotocore-migrationhuborchestrator-2.5.2.post2/README.md
--rw-r--r--   0 vlad      (1000) vlad      (1000)       38 2023-08-04 13:59:19.076643 types-aiobotocore-migrationhuborchestrator-2.5.2.post2/setup.cfg
--rw-r--r--   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:58:46.126642 types-aiobotocore-migrationhuborchestrator-2.5.2.post2/setup.py
-drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:19.076643 types-aiobotocore-migrationhuborchestrator-2.5.2.post2/types_aiobotocore_migrationhuborchestrator/
--rw-r--r--   0 vlad      (1000) vlad      (1000)     2061 2023-08-04 13:45:08.000000 types-aiobotocore-migrationhuborchestrator-2.5.2.post2/types_aiobotocore_migrationhuborchestrator/__init__.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)     2060 2023-08-04 13:45:08.000000 types-aiobotocore-migrationhuborchestrator-2.5.2.post2/types_aiobotocore_migrationhuborchestrator/__init__.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)     1011 2023-08-04 13:45:08.000000 types-aiobotocore-migrationhuborchestrator-2.5.2.post2/types_aiobotocore_migrationhuborchestrator/__main__.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)    27081 2023-08-04 13:45:09.000000 types-aiobotocore-migrationhuborchestrator-2.5.2.post2/types_aiobotocore_migrationhuborchestrator/client.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)    27037 2023-08-04 13:45:08.000000 types-aiobotocore-migrationhuborchestrator-2.5.2.post2/types_aiobotocore_migrationhuborchestrator/client.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)    10083 2023-08-04 13:45:09.000000 types-aiobotocore-migrationhuborchestrator-2.5.2.post2/types_aiobotocore_migrationhuborchestrator/literals.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)    10081 2023-08-04 13:45:09.000000 types-aiobotocore-migrationhuborchestrator-2.5.2.post2/types_aiobotocore_migrationhuborchestrator/literals.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)     9801 2023-08-04 13:45:09.000000 types-aiobotocore-migrationhuborchestrator-2.5.2.post2/types_aiobotocore_migrationhuborchestrator/paginator.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)     9792 2023-08-04 13:45:09.000000 types-aiobotocore-migrationhuborchestrator-2.5.2.post2/types_aiobotocore_migrationhuborchestrator/paginator.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:45:08.000000 types-aiobotocore-migrationhuborchestrator-2.5.2.post2/types_aiobotocore_migrationhuborchestrator/py.typed
--rw-r--r--   0 vlad      (1000) vlad      (1000)    31838 2023-08-04 13:45:10.000000 types-aiobotocore-migrationhuborchestrator-2.5.2.post2/types_aiobotocore_migrationhuborchestrator/type_defs.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)    31810 2023-08-04 13:45:09.000000 types-aiobotocore-migrationhuborchestrator-2.5.2.post2/types_aiobotocore_migrationhuborchestrator/type_defs.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)       65 2023-08-04 13:45:08.000000 types-aiobotocore-migrationhuborchestrator-2.5.2.post2/types_aiobotocore_migrationhuborchestrator/version.py
-drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:19.076643 types-aiobotocore-migrationhuborchestrator-2.5.2.post2/types_aiobotocore_migrationhuborchestrator.egg-info/
--rw-r--r--   0 vlad      (1000) vlad      (1000)    14781 2023-08-04 13:59:18.000000 types-aiobotocore-migrationhuborchestrator-2.5.2.post2/types_aiobotocore_migrationhuborchestrator.egg-info/PKG-INFO
--rw-r--r--   0 vlad      (1000) vlad      (1000)     1136 2023-08-04 13:59:19.000000 types-aiobotocore-migrationhuborchestrator-2.5.2.post2/types_aiobotocore_migrationhuborchestrator.egg-info/SOURCES.txt
--rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:18.000000 types-aiobotocore-migrationhuborchestrator-2.5.2.post2/types_aiobotocore_migrationhuborchestrator.egg-info/dependency_links.txt
--rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:18.000000 types-aiobotocore-migrationhuborchestrator-2.5.2.post2/types_aiobotocore_migrationhuborchestrator.egg-info/not-zip-safe
--rw-r--r--   0 vlad      (1000) vlad      (1000)       52 2023-08-04 13:59:18.000000 types-aiobotocore-migrationhuborchestrator-2.5.2.post2/types_aiobotocore_migrationhuborchestrator.egg-info/requires.txt
--rw-r--r--   0 vlad      (1000) vlad      (1000)       43 2023-08-04 13:59:19.000000 types-aiobotocore-migrationhuborchestrator-2.5.2.post2/types_aiobotocore_migrationhuborchestrator.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:24:08.586739 types-aiobotocore-migrationhuborchestrator-2.5.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-08 01:15:36.000000 types-aiobotocore-migrationhuborchestrator-2.5.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    14775 2023-08-08 01:24:08.586739 types-aiobotocore-migrationhuborchestrator-2.5.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    13195 2023-08-08 01:15:36.000000 types-aiobotocore-migrationhuborchestrator-2.5.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-08 01:24:08.586739 types-aiobotocore-migrationhuborchestrator-2.5.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2177 2023-08-08 01:15:36.000000 types-aiobotocore-migrationhuborchestrator-2.5.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:24:08.570739 types-aiobotocore-migrationhuborchestrator-2.5.4/types_aiobotocore_migrationhuborchestrator/
+-rw-r--r--   0 runner    (1001) docker     (123)     2061 2023-08-08 01:15:36.000000 types-aiobotocore-migrationhuborchestrator-2.5.4/types_aiobotocore_migrationhuborchestrator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2060 2023-08-08 01:15:36.000000 types-aiobotocore-migrationhuborchestrator-2.5.4/types_aiobotocore_migrationhuborchestrator/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      999 2023-08-08 01:15:36.000000 types-aiobotocore-migrationhuborchestrator-2.5.4/types_aiobotocore_migrationhuborchestrator/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27081 2023-08-08 01:15:36.000000 types-aiobotocore-migrationhuborchestrator-2.5.4/types_aiobotocore_migrationhuborchestrator/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27037 2023-08-08 01:15:36.000000 types-aiobotocore-migrationhuborchestrator-2.5.4/types_aiobotocore_migrationhuborchestrator/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    10083 2023-08-08 01:15:36.000000 types-aiobotocore-migrationhuborchestrator-2.5.4/types_aiobotocore_migrationhuborchestrator/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10081 2023-08-08 01:15:36.000000 types-aiobotocore-migrationhuborchestrator-2.5.4/types_aiobotocore_migrationhuborchestrator/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9801 2023-08-08 01:15:36.000000 types-aiobotocore-migrationhuborchestrator-2.5.4/types_aiobotocore_migrationhuborchestrator/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9792 2023-08-08 01:15:36.000000 types-aiobotocore-migrationhuborchestrator-2.5.4/types_aiobotocore_migrationhuborchestrator/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 01:15:36.000000 types-aiobotocore-migrationhuborchestrator-2.5.4/types_aiobotocore_migrationhuborchestrator/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    31838 2023-08-08 01:15:37.000000 types-aiobotocore-migrationhuborchestrator-2.5.4/types_aiobotocore_migrationhuborchestrator/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31810 2023-08-08 01:15:36.000000 types-aiobotocore-migrationhuborchestrator-2.5.4/types_aiobotocore_migrationhuborchestrator/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-08-08 01:15:36.000000 types-aiobotocore-migrationhuborchestrator-2.5.4/types_aiobotocore_migrationhuborchestrator/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:24:08.586739 types-aiobotocore-migrationhuborchestrator-2.5.4/types_aiobotocore_migrationhuborchestrator.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    14775 2023-08-08 01:24:08.000000 types-aiobotocore-migrationhuborchestrator-2.5.4/types_aiobotocore_migrationhuborchestrator.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1136 2023-08-08 01:24:08.000000 types-aiobotocore-migrationhuborchestrator-2.5.4/types_aiobotocore_migrationhuborchestrator.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 01:24:08.000000 types-aiobotocore-migrationhuborchestrator-2.5.4/types_aiobotocore_migrationhuborchestrator.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 01:24:08.000000 types-aiobotocore-migrationhuborchestrator-2.5.4/types_aiobotocore_migrationhuborchestrator.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-08 01:24:08.000000 types-aiobotocore-migrationhuborchestrator-2.5.4/types_aiobotocore_migrationhuborchestrator.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-08-08 01:24:08.000000 types-aiobotocore-migrationhuborchestrator-2.5.4/types_aiobotocore_migrationhuborchestrator.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-migrationhuborchestrator-2.5.2.post2/LICENSE` & `types-aiobotocore-migrationhuborchestrator-2.5.4/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-migrationhuborchestrator-2.5.2.post2/PKG-INFO` & `types-aiobotocore-migrationhuborchestrator-2.5.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-migrationhuborchestrator
-Version: 2.5.2.post2
-Summary: Type annotations for aiobotocore.MigrationHubOrchestrator 2.5.2 service generated with mypy-boto3-builder 7.17.2
+Version: 2.5.4
+Summary: Type annotations for aiobotocore.MigrationHubOrchestrator 2.5.4 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_migrationhuborchestrator/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-migrationhuborchestrator.svg?color=blue)](https://pypi.org/project/types-aiobotocore-migrationhuborchestrator)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_migrationhuborchestrator/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-migrationhuborchestrator)](https://pepy.tech/project/types-aiobotocore-migrationhuborchestrator)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.MigrationHubOrchestrator 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migrationhuborchestrator.html#MigrationHubOrchestrator)
+[aiobotocore.MigrationHubOrchestrator 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migrationhuborchestrator.html#MigrationHubOrchestrator)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-migrationhuborchestrator-2.5.2.post2/README.md` & `types-aiobotocore-migrationhuborchestrator-2.5.4/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-migrationhuborchestrator.svg?color=blue)](https://pypi.org/project/types-aiobotocore-migrationhuborchestrator)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_migrationhuborchestrator/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-migrationhuborchestrator)](https://pepy.tech/project/types-aiobotocore-migrationhuborchestrator)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.MigrationHubOrchestrator 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migrationhuborchestrator.html#MigrationHubOrchestrator)
+[aiobotocore.MigrationHubOrchestrator 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migrationhuborchestrator.html#MigrationHubOrchestrator)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-migrationhuborchestrator-2.5.2.post2/types_aiobotocore_migrationhuborchestrator/__init__.py` & `types-aiobotocore-migrationhuborchestrator-2.5.4/types_aiobotocore_migrationhuborchestrator/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-migrationhuborchestrator-2.5.2.post2/types_aiobotocore_migrationhuborchestrator/__init__.pyi` & `types-aiobotocore-migrationhuborchestrator-2.5.4/types_aiobotocore_migrationhuborchestrator/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-migrationhuborchestrator-2.5.2.post2/types_aiobotocore_migrationhuborchestrator/__main__.py` & `types-aiobotocore-migrationhuborchestrator-2.5.4/types_aiobotocore_migrationhuborchestrator/__main__.py`

 * *Files 7% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.MigrationHubOrchestrator 2.5.2\nVersion:        "
-        " 2.5.2.post2\nBuilder version: 7.17.2\nDocs:           "
+        "Type annotations for aiobotocore.MigrationHubOrchestrator 2.5.4\nVersion:        "
+        " 2.5.4\nBuilder version: 7.17.2\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_migrationhuborchestrator//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migrationhuborchestrator.html#MigrationHubOrchestrator\nOther"
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

### Comparing `types-aiobotocore-migrationhuborchestrator-2.5.2.post2/types_aiobotocore_migrationhuborchestrator/client.py` & `types-aiobotocore-migrationhuborchestrator-2.5.4/types_aiobotocore_migrationhuborchestrator/client.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-migrationhuborchestrator-2.5.2.post2/types_aiobotocore_migrationhuborchestrator/client.pyi` & `types-aiobotocore-migrationhuborchestrator-2.5.4/types_aiobotocore_migrationhuborchestrator/client.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-migrationhuborchestrator-2.5.2.post2/types_aiobotocore_migrationhuborchestrator/literals.py` & `types-aiobotocore-migrationhuborchestrator-2.5.4/types_aiobotocore_migrationhuborchestrator/literals.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-migrationhuborchestrator-2.5.2.post2/types_aiobotocore_migrationhuborchestrator/literals.pyi` & `types-aiobotocore-migrationhuborchestrator-2.5.4/types_aiobotocore_migrationhuborchestrator/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-migrationhuborchestrator-2.5.2.post2/types_aiobotocore_migrationhuborchestrator/paginator.py` & `types-aiobotocore-migrationhuborchestrator-2.5.4/types_aiobotocore_migrationhuborchestrator/paginator.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-migrationhuborchestrator-2.5.2.post2/types_aiobotocore_migrationhuborchestrator/paginator.pyi` & `types-aiobotocore-migrationhuborchestrator-2.5.4/types_aiobotocore_migrationhuborchestrator/paginator.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-migrationhuborchestrator-2.5.2.post2/types_aiobotocore_migrationhuborchestrator/type_defs.py` & `types-aiobotocore-migrationhuborchestrator-2.5.4/types_aiobotocore_migrationhuborchestrator/type_defs.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-migrationhuborchestrator-2.5.2.post2/types_aiobotocore_migrationhuborchestrator/type_defs.pyi` & `types-aiobotocore-migrationhuborchestrator-2.5.4/types_aiobotocore_migrationhuborchestrator/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-migrationhuborchestrator-2.5.2.post2/types_aiobotocore_migrationhuborchestrator.egg-info/PKG-INFO` & `types-aiobotocore-migrationhuborchestrator-2.5.4/types_aiobotocore_migrationhuborchestrator.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-migrationhuborchestrator
-Version: 2.5.2.post2
-Summary: Type annotations for aiobotocore.MigrationHubOrchestrator 2.5.2 service generated with mypy-boto3-builder 7.17.2
+Version: 2.5.4
+Summary: Type annotations for aiobotocore.MigrationHubOrchestrator 2.5.4 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_migrationhuborchestrator/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-migrationhuborchestrator.svg?color=blue)](https://pypi.org/project/types-aiobotocore-migrationhuborchestrator)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_migrationhuborchestrator/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-migrationhuborchestrator)](https://pepy.tech/project/types-aiobotocore-migrationhuborchestrator)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.MigrationHubOrchestrator 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migrationhuborchestrator.html#MigrationHubOrchestrator)
+[aiobotocore.MigrationHubOrchestrator 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migrationhuborchestrator.html#MigrationHubOrchestrator)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-migrationhuborchestrator-2.5.2.post2/types_aiobotocore_migrationhuborchestrator.egg-info/SOURCES.txt` & `types-aiobotocore-migrationhuborchestrator-2.5.4/types_aiobotocore_migrationhuborchestrator.egg-info/SOURCES.txt`

 * *Files identical despite different names*


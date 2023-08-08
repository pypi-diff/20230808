# Comparing `tmp/types-aiobotocore-migration-hub-refactor-spaces-2.5.2.post2.tar.gz` & `tmp/types-aiobotocore-migration-hub-refactor-spaces-2.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-migration-hub-refactor-spaces-2.5.2.post2.tar", last modified: Fri Aug  4 13:59:18 2023, max compression
+gzip compressed data, was "types-aiobotocore-migration-hub-refactor-spaces-2.5.4.tar", last modified: Tue Aug  8 01:24:07 2023, max compression
```

## Comparing `types-aiobotocore-migration-hub-refactor-spaces-2.5.2.post2.tar` & `types-aiobotocore-migration-hub-refactor-spaces-2.5.4.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:18.566643 types-aiobotocore-migration-hub-refactor-spaces-2.5.2.post2/
--rw-r--r--   0 vlad      (1000) vlad      (1000)     1070 2023-08-04 13:45:03.000000 types-aiobotocore-migration-hub-refactor-spaces-2.5.2.post2/LICENSE
--rw-r--r--   0 vlad      (1000) vlad      (1000)    14769 2023-08-04 13:59:18.556643 types-aiobotocore-migration-hub-refactor-spaces-2.5.2.post2/PKG-INFO
--rw-r--r--   0 vlad      (1000) vlad      (1000)    13166 2023-08-04 13:45:03.000000 types-aiobotocore-migration-hub-refactor-spaces-2.5.2.post2/README.md
--rw-r--r--   0 vlad      (1000) vlad      (1000)       38 2023-08-04 13:59:18.566643 types-aiobotocore-migration-hub-refactor-spaces-2.5.2.post2/setup.cfg
--rw-r--r--   0 vlad      (1000) vlad      (1000)     2226 2023-08-04 13:45:03.000000 types-aiobotocore-migration-hub-refactor-spaces-2.5.2.post2/setup.py
-drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:18.556643 types-aiobotocore-migration-hub-refactor-spaces-2.5.2.post2/types_aiobotocore_migration_hub_refactor_spaces/
--rw-r--r--   0 vlad      (1000) vlad      (1000)     1612 2023-08-04 13:45:03.000000 types-aiobotocore-migration-hub-refactor-spaces-2.5.2.post2/types_aiobotocore_migration_hub_refactor_spaces/__init__.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)     1611 2023-08-04 13:45:03.000000 types-aiobotocore-migration-hub-refactor-spaces-2.5.2.post2/types_aiobotocore_migration_hub_refactor_spaces/__init__.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)     1025 2023-08-04 13:45:03.000000 types-aiobotocore-migration-hub-refactor-spaces-2.5.2.post2/types_aiobotocore_migration_hub_refactor_spaces/__main__.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)    24605 2023-08-04 13:45:04.000000 types-aiobotocore-migration-hub-refactor-spaces-2.5.2.post2/types_aiobotocore_migration_hub_refactor_spaces/client.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)    24567 2023-08-04 13:45:03.000000 types-aiobotocore-migration-hub-refactor-spaces-2.5.2.post2/types_aiobotocore_migration_hub_refactor_spaces/client.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)    10271 2023-08-04 13:45:04.000000 types-aiobotocore-migration-hub-refactor-spaces-2.5.2.post2/types_aiobotocore_migration_hub_refactor_spaces/literals.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)    10269 2023-08-04 13:45:04.000000 types-aiobotocore-migration-hub-refactor-spaces-2.5.2.post2/types_aiobotocore_migration_hub_refactor_spaces/literals.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)     7278 2023-08-04 13:45:04.000000 types-aiobotocore-migration-hub-refactor-spaces-2.5.2.post2/types_aiobotocore_migration_hub_refactor_spaces/paginator.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)     7271 2023-08-04 13:45:04.000000 types-aiobotocore-migration-hub-refactor-spaces-2.5.2.post2/types_aiobotocore_migration_hub_refactor_spaces/paginator.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:45:03.000000 types-aiobotocore-migration-hub-refactor-spaces-2.5.2.post2/types_aiobotocore_migration_hub_refactor_spaces/py.typed
--rw-r--r--   0 vlad      (1000) vlad      (1000)    28376 2023-08-04 13:45:05.000000 types-aiobotocore-migration-hub-refactor-spaces-2.5.2.post2/types_aiobotocore_migration_hub_refactor_spaces/type_defs.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)    28347 2023-08-04 13:45:04.000000 types-aiobotocore-migration-hub-refactor-spaces-2.5.2.post2/types_aiobotocore_migration_hub_refactor_spaces/type_defs.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)       65 2023-08-04 13:45:03.000000 types-aiobotocore-migration-hub-refactor-spaces-2.5.2.post2/types_aiobotocore_migration_hub_refactor_spaces/version.py
-drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:18.556643 types-aiobotocore-migration-hub-refactor-spaces-2.5.2.post2/types_aiobotocore_migration_hub_refactor_spaces.egg-info/
--rw-r--r--   0 vlad      (1000) vlad      (1000)    14769 2023-08-04 13:59:18.000000 types-aiobotocore-migration-hub-refactor-spaces-2.5.2.post2/types_aiobotocore_migration_hub_refactor_spaces.egg-info/PKG-INFO
--rw-r--r--   0 vlad      (1000) vlad      (1000)     1231 2023-08-04 13:59:18.000000 types-aiobotocore-migration-hub-refactor-spaces-2.5.2.post2/types_aiobotocore_migration_hub_refactor_spaces.egg-info/SOURCES.txt
--rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:18.000000 types-aiobotocore-migration-hub-refactor-spaces-2.5.2.post2/types_aiobotocore_migration_hub_refactor_spaces.egg-info/dependency_links.txt
--rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:18.000000 types-aiobotocore-migration-hub-refactor-spaces-2.5.2.post2/types_aiobotocore_migration_hub_refactor_spaces.egg-info/not-zip-safe
--rw-r--r--   0 vlad      (1000) vlad      (1000)       52 2023-08-04 13:59:18.000000 types-aiobotocore-migration-hub-refactor-spaces-2.5.2.post2/types_aiobotocore_migration_hub_refactor_spaces.egg-info/requires.txt
--rw-r--r--   0 vlad      (1000) vlad      (1000)       48 2023-08-04 13:59:18.000000 types-aiobotocore-migration-hub-refactor-spaces-2.5.2.post2/types_aiobotocore_migration_hub_refactor_spaces.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:24:07.178736 types-aiobotocore-migration-hub-refactor-spaces-2.5.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-08 01:15:34.000000 types-aiobotocore-migration-hub-refactor-spaces-2.5.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    14763 2023-08-08 01:24:07.174736 types-aiobotocore-migration-hub-refactor-spaces-2.5.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    13166 2023-08-08 01:15:34.000000 types-aiobotocore-migration-hub-refactor-spaces-2.5.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-08 01:24:07.178736 types-aiobotocore-migration-hub-refactor-spaces-2.5.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2220 2023-08-08 01:15:34.000000 types-aiobotocore-migration-hub-refactor-spaces-2.5.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:24:07.174736 types-aiobotocore-migration-hub-refactor-spaces-2.5.4/types_aiobotocore_migration_hub_refactor_spaces/
+-rw-r--r--   0 runner    (1001) docker     (123)     1612 2023-08-08 01:15:34.000000 types-aiobotocore-migration-hub-refactor-spaces-2.5.4/types_aiobotocore_migration_hub_refactor_spaces/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1611 2023-08-08 01:15:34.000000 types-aiobotocore-migration-hub-refactor-spaces-2.5.4/types_aiobotocore_migration_hub_refactor_spaces/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1013 2023-08-08 01:15:34.000000 types-aiobotocore-migration-hub-refactor-spaces-2.5.4/types_aiobotocore_migration_hub_refactor_spaces/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24605 2023-08-08 01:15:34.000000 types-aiobotocore-migration-hub-refactor-spaces-2.5.4/types_aiobotocore_migration_hub_refactor_spaces/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24567 2023-08-08 01:15:34.000000 types-aiobotocore-migration-hub-refactor-spaces-2.5.4/types_aiobotocore_migration_hub_refactor_spaces/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    10271 2023-08-08 01:15:34.000000 types-aiobotocore-migration-hub-refactor-spaces-2.5.4/types_aiobotocore_migration_hub_refactor_spaces/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10269 2023-08-08 01:15:34.000000 types-aiobotocore-migration-hub-refactor-spaces-2.5.4/types_aiobotocore_migration_hub_refactor_spaces/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     7278 2023-08-08 01:15:34.000000 types-aiobotocore-migration-hub-refactor-spaces-2.5.4/types_aiobotocore_migration_hub_refactor_spaces/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7271 2023-08-08 01:15:34.000000 types-aiobotocore-migration-hub-refactor-spaces-2.5.4/types_aiobotocore_migration_hub_refactor_spaces/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 01:15:34.000000 types-aiobotocore-migration-hub-refactor-spaces-2.5.4/types_aiobotocore_migration_hub_refactor_spaces/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    28376 2023-08-08 01:15:35.000000 types-aiobotocore-migration-hub-refactor-spaces-2.5.4/types_aiobotocore_migration_hub_refactor_spaces/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28347 2023-08-08 01:15:35.000000 types-aiobotocore-migration-hub-refactor-spaces-2.5.4/types_aiobotocore_migration_hub_refactor_spaces/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-08-08 01:15:34.000000 types-aiobotocore-migration-hub-refactor-spaces-2.5.4/types_aiobotocore_migration_hub_refactor_spaces/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:24:07.174736 types-aiobotocore-migration-hub-refactor-spaces-2.5.4/types_aiobotocore_migration_hub_refactor_spaces.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    14763 2023-08-08 01:24:07.000000 types-aiobotocore-migration-hub-refactor-spaces-2.5.4/types_aiobotocore_migration_hub_refactor_spaces.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1231 2023-08-08 01:24:07.000000 types-aiobotocore-migration-hub-refactor-spaces-2.5.4/types_aiobotocore_migration_hub_refactor_spaces.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 01:24:07.000000 types-aiobotocore-migration-hub-refactor-spaces-2.5.4/types_aiobotocore_migration_hub_refactor_spaces.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 01:24:07.000000 types-aiobotocore-migration-hub-refactor-spaces-2.5.4/types_aiobotocore_migration_hub_refactor_spaces.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-08 01:24:07.000000 types-aiobotocore-migration-hub-refactor-spaces-2.5.4/types_aiobotocore_migration_hub_refactor_spaces.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-08-08 01:24:07.000000 types-aiobotocore-migration-hub-refactor-spaces-2.5.4/types_aiobotocore_migration_hub_refactor_spaces.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-migration-hub-refactor-spaces-2.5.2.post2/LICENSE` & `types-aiobotocore-migration-hub-refactor-spaces-2.5.4/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-migration-hub-refactor-spaces-2.5.2.post2/PKG-INFO` & `types-aiobotocore-migration-hub-refactor-spaces-2.5.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-migration-hub-refactor-spaces
-Version: 2.5.2.post2
-Summary: Type annotations for aiobotocore.MigrationHubRefactorSpaces 2.5.2 service generated with mypy-boto3-builder 7.17.2
+Version: 2.5.4
+Summary: Type annotations for aiobotocore.MigrationHubRefactorSpaces 2.5.4 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_migration_hub_refactor_spaces/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-migration-hub-refactor-spaces.svg?color=blue)](https://pypi.org/project/types-aiobotocore-migration-hub-refactor-spaces)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_migration_hub_refactor_spaces/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-migration-hub-refactor-spaces)](https://pepy.tech/project/types-aiobotocore-migration-hub-refactor-spaces)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.MigrationHubRefactorSpaces 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migration-hub-refactor-spaces.html#MigrationHubRefactorSpaces)
+[aiobotocore.MigrationHubRefactorSpaces 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migration-hub-refactor-spaces.html#MigrationHubRefactorSpaces)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-migration-hub-refactor-spaces-2.5.2.post2/README.md` & `types-aiobotocore-migration-hub-refactor-spaces-2.5.4/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-migration-hub-refactor-spaces.svg?color=blue)](https://pypi.org/project/types-aiobotocore-migration-hub-refactor-spaces)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_migration_hub_refactor_spaces/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-migration-hub-refactor-spaces)](https://pepy.tech/project/types-aiobotocore-migration-hub-refactor-spaces)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.MigrationHubRefactorSpaces 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migration-hub-refactor-spaces.html#MigrationHubRefactorSpaces)
+[aiobotocore.MigrationHubRefactorSpaces 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migration-hub-refactor-spaces.html#MigrationHubRefactorSpaces)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-migration-hub-refactor-spaces-2.5.2.post2/setup.py` & `types-aiobotocore-migration-hub-refactor-spaces-2.5.4/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-migration-hub-refactor-spaces",
-    version="2.5.2.post2",
+    version="2.5.4",
     packages=["types_aiobotocore_migration_hub_refactor_spaces"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.MigrationHubRefactorSpaces 2.5.2 service generated with"
+        "Type annotations for aiobotocore.MigrationHubRefactorSpaces 2.5.4 service generated with"
         " mypy-boto3-builder 7.17.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
```

### Comparing `types-aiobotocore-migration-hub-refactor-spaces-2.5.2.post2/types_aiobotocore_migration_hub_refactor_spaces/__init__.py` & `types-aiobotocore-migration-hub-refactor-spaces-2.5.4/types_aiobotocore_migration_hub_refactor_spaces/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-migration-hub-refactor-spaces-2.5.2.post2/types_aiobotocore_migration_hub_refactor_spaces/__init__.pyi` & `types-aiobotocore-migration-hub-refactor-spaces-2.5.4/types_aiobotocore_migration_hub_refactor_spaces/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-migration-hub-refactor-spaces-2.5.2.post2/types_aiobotocore_migration_hub_refactor_spaces/__main__.py` & `types-aiobotocore-migration-hub-refactor-spaces-2.5.4/types_aiobotocore_migration_hub_refactor_spaces/__main__.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.MigrationHubRefactorSpaces 2.5.2\nVersion:        "
-        " 2.5.2.post2\nBuilder version: 7.17.2\nDocs:           "
+        "Type annotations for aiobotocore.MigrationHubRefactorSpaces 2.5.4\nVersion:        "
+        " 2.5.4\nBuilder version: 7.17.2\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_migration_hub_refactor_spaces//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migration-hub-refactor-spaces.html#MigrationHubRefactorSpaces\nOther"
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

### Comparing `types-aiobotocore-migration-hub-refactor-spaces-2.5.2.post2/types_aiobotocore_migration_hub_refactor_spaces/client.py` & `types-aiobotocore-migration-hub-refactor-spaces-2.5.4/types_aiobotocore_migration_hub_refactor_spaces/client.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-migration-hub-refactor-spaces-2.5.2.post2/types_aiobotocore_migration_hub_refactor_spaces/client.pyi` & `types-aiobotocore-migration-hub-refactor-spaces-2.5.4/types_aiobotocore_migration_hub_refactor_spaces/client.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-migration-hub-refactor-spaces-2.5.2.post2/types_aiobotocore_migration_hub_refactor_spaces/literals.py` & `types-aiobotocore-migration-hub-refactor-spaces-2.5.4/types_aiobotocore_migration_hub_refactor_spaces/literals.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-migration-hub-refactor-spaces-2.5.2.post2/types_aiobotocore_migration_hub_refactor_spaces/literals.pyi` & `types-aiobotocore-migration-hub-refactor-spaces-2.5.4/types_aiobotocore_migration_hub_refactor_spaces/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-migration-hub-refactor-spaces-2.5.2.post2/types_aiobotocore_migration_hub_refactor_spaces/paginator.py` & `types-aiobotocore-migration-hub-refactor-spaces-2.5.4/types_aiobotocore_migration_hub_refactor_spaces/paginator.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-migration-hub-refactor-spaces-2.5.2.post2/types_aiobotocore_migration_hub_refactor_spaces/paginator.pyi` & `types-aiobotocore-migration-hub-refactor-spaces-2.5.4/types_aiobotocore_migration_hub_refactor_spaces/paginator.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-migration-hub-refactor-spaces-2.5.2.post2/types_aiobotocore_migration_hub_refactor_spaces/type_defs.py` & `types-aiobotocore-migration-hub-refactor-spaces-2.5.4/types_aiobotocore_migration_hub_refactor_spaces/type_defs.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-migration-hub-refactor-spaces-2.5.2.post2/types_aiobotocore_migration_hub_refactor_spaces/type_defs.pyi` & `types-aiobotocore-migration-hub-refactor-spaces-2.5.4/types_aiobotocore_migration_hub_refactor_spaces/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-migration-hub-refactor-spaces-2.5.2.post2/types_aiobotocore_migration_hub_refactor_spaces.egg-info/PKG-INFO` & `types-aiobotocore-migration-hub-refactor-spaces-2.5.4/types_aiobotocore_migration_hub_refactor_spaces.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-migration-hub-refactor-spaces
-Version: 2.5.2.post2
-Summary: Type annotations for aiobotocore.MigrationHubRefactorSpaces 2.5.2 service generated with mypy-boto3-builder 7.17.2
+Version: 2.5.4
+Summary: Type annotations for aiobotocore.MigrationHubRefactorSpaces 2.5.4 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_migration_hub_refactor_spaces/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-migration-hub-refactor-spaces.svg?color=blue)](https://pypi.org/project/types-aiobotocore-migration-hub-refactor-spaces)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_migration_hub_refactor_spaces/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-migration-hub-refactor-spaces)](https://pepy.tech/project/types-aiobotocore-migration-hub-refactor-spaces)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.MigrationHubRefactorSpaces 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migration-hub-refactor-spaces.html#MigrationHubRefactorSpaces)
+[aiobotocore.MigrationHubRefactorSpaces 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migration-hub-refactor-spaces.html#MigrationHubRefactorSpaces)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-migration-hub-refactor-spaces-2.5.2.post2/types_aiobotocore_migration_hub_refactor_spaces.egg-info/SOURCES.txt` & `types-aiobotocore-migration-hub-refactor-spaces-2.5.4/types_aiobotocore_migration_hub_refactor_spaces.egg-info/SOURCES.txt`

 * *Files identical despite different names*


# Comparing `tmp/types-aiobotocore-migrationhub-config-2.5.2.post2.tar.gz` & `tmp/types-aiobotocore-migrationhub-config-2.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-migrationhub-config-2.5.2.post2.tar", last modified: Fri Aug  4 13:59:18 2023, max compression
+gzip compressed data, was "types-aiobotocore-migrationhub-config-2.5.4.tar", last modified: Tue Aug  8 01:24:07 2023, max compression
```

## Comparing `types-aiobotocore-migrationhub-config-2.5.2.post2.tar` & `types-aiobotocore-migrationhub-config-2.5.4.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:18.736643 types-aiobotocore-migrationhub-config-2.5.2.post2/
--rw-r--r--   0 vlad      (1000) vlad      (1000)     1070 2023-08-04 13:45:06.000000 types-aiobotocore-migrationhub-config-2.5.2.post2/LICENSE
--rw-r--r--   0 vlad      (1000) vlad      (1000)    12791 2023-08-04 13:59:18.736643 types-aiobotocore-migrationhub-config-2.5.2.post2/PKG-INFO
--rw-r--r--   0 vlad      (1000) vlad      (1000)    11226 2023-08-04 13:45:06.000000 types-aiobotocore-migrationhub-config-2.5.2.post2/README.md
--rw-r--r--   0 vlad      (1000) vlad      (1000)       38 2023-08-04 13:59:18.736643 types-aiobotocore-migrationhub-config-2.5.2.post2/setup.cfg
--rw-r--r--   0 vlad      (1000) vlad      (1000)     2131 2023-08-04 13:45:05.000000 types-aiobotocore-migrationhub-config-2.5.2.post2/setup.py
-drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:18.736643 types-aiobotocore-migrationhub-config-2.5.2.post2/types_aiobotocore_migrationhub_config/
--rw-r--r--   0 vlad      (1000) vlad      (1000)      533 2023-08-04 13:45:06.000000 types-aiobotocore-migrationhub-config-2.5.2.post2/types_aiobotocore_migrationhub_config/__init__.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)      532 2023-08-04 13:45:06.000000 types-aiobotocore-migrationhub-config-2.5.2.post2/types_aiobotocore_migrationhub_config/__init__.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)      989 2023-08-04 13:45:06.000000 types-aiobotocore-migrationhub-config-2.5.2.post2/types_aiobotocore_migrationhub_config/__main__.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)     6471 2023-08-04 13:45:06.000000 types-aiobotocore-migrationhub-config-2.5.2.post2/types_aiobotocore_migrationhub_config/client.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)     6460 2023-08-04 13:45:06.000000 types-aiobotocore-migrationhub-config-2.5.2.post2/types_aiobotocore_migrationhub_config/client.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)     7716 2023-08-04 13:45:06.000000 types-aiobotocore-migrationhub-config-2.5.2.post2/types_aiobotocore_migrationhub_config/literals.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)     7714 2023-08-04 13:45:06.000000 types-aiobotocore-migrationhub-config-2.5.2.post2/types_aiobotocore_migrationhub_config/literals.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:45:06.000000 types-aiobotocore-migrationhub-config-2.5.2.post2/types_aiobotocore_migrationhub_config/py.typed
--rw-r--r--   0 vlad      (1000) vlad      (1000)     3244 2023-08-04 13:45:06.000000 types-aiobotocore-migrationhub-config-2.5.2.post2/types_aiobotocore_migrationhub_config/type_defs.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)     3239 2023-08-04 13:45:06.000000 types-aiobotocore-migrationhub-config-2.5.2.post2/types_aiobotocore_migrationhub_config/type_defs.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)       65 2023-08-04 13:45:06.000000 types-aiobotocore-migrationhub-config-2.5.2.post2/types_aiobotocore_migrationhub_config/version.py
-drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:18.736643 types-aiobotocore-migrationhub-config-2.5.2.post2/types_aiobotocore_migrationhub_config.egg-info/
--rw-r--r--   0 vlad      (1000) vlad      (1000)    12791 2023-08-04 13:59:18.000000 types-aiobotocore-migrationhub-config-2.5.2.post2/types_aiobotocore_migrationhub_config.egg-info/PKG-INFO
--rw-r--r--   0 vlad      (1000) vlad      (1000)      938 2023-08-04 13:59:18.000000 types-aiobotocore-migrationhub-config-2.5.2.post2/types_aiobotocore_migrationhub_config.egg-info/SOURCES.txt
--rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:18.000000 types-aiobotocore-migrationhub-config-2.5.2.post2/types_aiobotocore_migrationhub_config.egg-info/dependency_links.txt
--rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:18.000000 types-aiobotocore-migrationhub-config-2.5.2.post2/types_aiobotocore_migrationhub_config.egg-info/not-zip-safe
--rw-r--r--   0 vlad      (1000) vlad      (1000)       52 2023-08-04 13:59:18.000000 types-aiobotocore-migrationhub-config-2.5.2.post2/types_aiobotocore_migrationhub_config.egg-info/requires.txt
--rw-r--r--   0 vlad      (1000) vlad      (1000)       38 2023-08-04 13:59:18.000000 types-aiobotocore-migrationhub-config-2.5.2.post2/types_aiobotocore_migrationhub_config.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:24:07.870738 types-aiobotocore-migrationhub-config-2.5.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-08 01:15:35.000000 types-aiobotocore-migrationhub-config-2.5.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    12785 2023-08-08 01:24:07.870738 types-aiobotocore-migrationhub-config-2.5.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    11226 2023-08-08 01:15:35.000000 types-aiobotocore-migrationhub-config-2.5.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-08 01:24:07.870738 types-aiobotocore-migrationhub-config-2.5.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2125 2023-08-08 01:15:35.000000 types-aiobotocore-migrationhub-config-2.5.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:24:07.870738 types-aiobotocore-migrationhub-config-2.5.4/types_aiobotocore_migrationhub_config/
+-rw-r--r--   0 runner    (1001) docker     (123)      533 2023-08-08 01:15:35.000000 types-aiobotocore-migrationhub-config-2.5.4/types_aiobotocore_migrationhub_config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      532 2023-08-08 01:15:35.000000 types-aiobotocore-migrationhub-config-2.5.4/types_aiobotocore_migrationhub_config/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      977 2023-08-08 01:15:35.000000 types-aiobotocore-migrationhub-config-2.5.4/types_aiobotocore_migrationhub_config/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6471 2023-08-08 01:15:35.000000 types-aiobotocore-migrationhub-config-2.5.4/types_aiobotocore_migrationhub_config/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6460 2023-08-08 01:15:35.000000 types-aiobotocore-migrationhub-config-2.5.4/types_aiobotocore_migrationhub_config/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     7716 2023-08-08 01:15:35.000000 types-aiobotocore-migrationhub-config-2.5.4/types_aiobotocore_migrationhub_config/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7714 2023-08-08 01:15:35.000000 types-aiobotocore-migrationhub-config-2.5.4/types_aiobotocore_migrationhub_config/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 01:15:35.000000 types-aiobotocore-migrationhub-config-2.5.4/types_aiobotocore_migrationhub_config/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     3244 2023-08-08 01:15:35.000000 types-aiobotocore-migrationhub-config-2.5.4/types_aiobotocore_migrationhub_config/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3239 2023-08-08 01:15:35.000000 types-aiobotocore-migrationhub-config-2.5.4/types_aiobotocore_migrationhub_config/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-08-08 01:15:35.000000 types-aiobotocore-migrationhub-config-2.5.4/types_aiobotocore_migrationhub_config/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:24:07.870738 types-aiobotocore-migrationhub-config-2.5.4/types_aiobotocore_migrationhub_config.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    12785 2023-08-08 01:24:07.000000 types-aiobotocore-migrationhub-config-2.5.4/types_aiobotocore_migrationhub_config.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      938 2023-08-08 01:24:07.000000 types-aiobotocore-migrationhub-config-2.5.4/types_aiobotocore_migrationhub_config.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 01:24:07.000000 types-aiobotocore-migrationhub-config-2.5.4/types_aiobotocore_migrationhub_config.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 01:24:07.000000 types-aiobotocore-migrationhub-config-2.5.4/types_aiobotocore_migrationhub_config.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-08 01:24:07.000000 types-aiobotocore-migrationhub-config-2.5.4/types_aiobotocore_migrationhub_config.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-08 01:24:07.000000 types-aiobotocore-migrationhub-config-2.5.4/types_aiobotocore_migrationhub_config.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-migrationhub-config-2.5.2.post2/LICENSE` & `types-aiobotocore-migrationhub-config-2.5.4/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-migrationhub-config-2.5.2.post2/PKG-INFO` & `types-aiobotocore-migrationhub-config-2.5.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-migrationhub-config
-Version: 2.5.2.post2
-Summary: Type annotations for aiobotocore.MigrationHubConfig 2.5.2 service generated with mypy-boto3-builder 7.17.2
+Version: 2.5.4
+Summary: Type annotations for aiobotocore.MigrationHubConfig 2.5.4 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_migrationhub_config/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-migrationhub-config.svg?color=blue)](https://pypi.org/project/types-aiobotocore-migrationhub-config)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_migrationhub_config/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-migrationhub-config)](https://pepy.tech/project/types-aiobotocore-migrationhub-config)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.MigrationHubConfig 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migrationhub-config.html#MigrationHubConfig)
+[aiobotocore.MigrationHubConfig 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migrationhub-config.html#MigrationHubConfig)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-migrationhub-config-2.5.2.post2/README.md` & `types-aiobotocore-migrationhub-config-2.5.4/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-migrationhub-config.svg?color=blue)](https://pypi.org/project/types-aiobotocore-migrationhub-config)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_migrationhub_config/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-migrationhub-config)](https://pepy.tech/project/types-aiobotocore-migrationhub-config)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.MigrationHubConfig 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migrationhub-config.html#MigrationHubConfig)
+[aiobotocore.MigrationHubConfig 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migrationhub-config.html#MigrationHubConfig)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-migrationhub-config-2.5.2.post2/setup.py` & `types-aiobotocore-migrationhub-config-2.5.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-migrationhub-config",
-    version="2.5.2.post2",
+    version="2.5.4",
     packages=["types_aiobotocore_migrationhub_config"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.MigrationHubConfig 2.5.2 service generated with"
+        "Type annotations for aiobotocore.MigrationHubConfig 2.5.4 service generated with"
         " mypy-boto3-builder 7.17.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
```

### Comparing `types-aiobotocore-migrationhub-config-2.5.2.post2/types_aiobotocore_migrationhub_config/__init__.py` & `types-aiobotocore-migrationhub-config-2.5.4/types_aiobotocore_migrationhub_config/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-migrationhub-config-2.5.2.post2/types_aiobotocore_migrationhub_config/__init__.pyi` & `types-aiobotocore-migrationhub-config-2.5.4/types_aiobotocore_migrationhub_config/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-migrationhub-config-2.5.2.post2/types_aiobotocore_migrationhub_config/__main__.py` & `types-aiobotocore-migrationhub-config-2.5.4/types_aiobotocore_migrationhub_config/__main__.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.MigrationHubConfig 2.5.2\nVersion:        "
-        " 2.5.2.post2\nBuilder version: 7.17.2\nDocs:           "
+        "Type annotations for aiobotocore.MigrationHubConfig 2.5.4\nVersion:         2.5.4\nBuilder"
+        " version: 7.17.2\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_migrationhub_config//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migrationhub-config.html#MigrationHubConfig\nOther"
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

### Comparing `types-aiobotocore-migrationhub-config-2.5.2.post2/types_aiobotocore_migrationhub_config/client.py` & `types-aiobotocore-migrationhub-config-2.5.4/types_aiobotocore_migrationhub_config/client.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-migrationhub-config-2.5.2.post2/types_aiobotocore_migrationhub_config/client.pyi` & `types-aiobotocore-migrationhub-config-2.5.4/types_aiobotocore_migrationhub_config/client.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-migrationhub-config-2.5.2.post2/types_aiobotocore_migrationhub_config/literals.py` & `types-aiobotocore-migrationhub-config-2.5.4/types_aiobotocore_migrationhub_config/literals.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-migrationhub-config-2.5.2.post2/types_aiobotocore_migrationhub_config/literals.pyi` & `types-aiobotocore-migrationhub-config-2.5.4/types_aiobotocore_migrationhub_config/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-migrationhub-config-2.5.2.post2/types_aiobotocore_migrationhub_config/type_defs.py` & `types-aiobotocore-migrationhub-config-2.5.4/types_aiobotocore_migrationhub_config/type_defs.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-migrationhub-config-2.5.2.post2/types_aiobotocore_migrationhub_config/type_defs.pyi` & `types-aiobotocore-migrationhub-config-2.5.4/types_aiobotocore_migrationhub_config/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-migrationhub-config-2.5.2.post2/types_aiobotocore_migrationhub_config.egg-info/PKG-INFO` & `types-aiobotocore-migrationhub-config-2.5.4/types_aiobotocore_migrationhub_config.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-migrationhub-config
-Version: 2.5.2.post2
-Summary: Type annotations for aiobotocore.MigrationHubConfig 2.5.2 service generated with mypy-boto3-builder 7.17.2
+Version: 2.5.4
+Summary: Type annotations for aiobotocore.MigrationHubConfig 2.5.4 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_migrationhub_config/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-migrationhub-config.svg?color=blue)](https://pypi.org/project/types-aiobotocore-migrationhub-config)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_migrationhub_config/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-migrationhub-config)](https://pepy.tech/project/types-aiobotocore-migrationhub-config)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.MigrationHubConfig 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migrationhub-config.html#MigrationHubConfig)
+[aiobotocore.MigrationHubConfig 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migrationhub-config.html#MigrationHubConfig)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-migrationhub-config-2.5.2.post2/types_aiobotocore_migrationhub_config.egg-info/SOURCES.txt` & `types-aiobotocore-migrationhub-config-2.5.4/types_aiobotocore_migrationhub_config.egg-info/SOURCES.txt`

 * *Files identical despite different names*


# Comparing `tmp/types-aiobotocore-mgh-2.5.2.post2.tar.gz` & `tmp/types-aiobotocore-mgh-2.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-mgh-2.5.2.post2.tar", last modified: Fri Aug  4 13:59:18 2023, max compression
+gzip compressed data, was "types-aiobotocore-mgh-2.5.4.tar", last modified: Tue Aug  8 01:24:06 2023, max compression
```

## Comparing `types-aiobotocore-mgh-2.5.2.post2.tar` & `types-aiobotocore-mgh-2.5.4.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:18.466643 types-aiobotocore-mgh-2.5.2.post2/
--rw-r--r--   0 vlad      (1000) vlad      (1000)     1070 2023-08-04 13:44:54.000000 types-aiobotocore-mgh-2.5.2.post2/LICENSE
--rw-r--r--   0 vlad      (1000) vlad      (1000)    13515 2023-08-04 13:59:18.466643 types-aiobotocore-mgh-2.5.2.post2/PKG-INFO
--rw-r--r--   0 vlad      (1000) vlad      (1000)    12004 2023-08-04 13:44:54.000000 types-aiobotocore-mgh-2.5.2.post2/README.md
--rw-r--r--   0 vlad      (1000) vlad      (1000)       38 2023-08-04 13:59:18.466643 types-aiobotocore-mgh-2.5.2.post2/setup.cfg
--rw-r--r--   0 vlad      (1000) vlad      (1000)     2029 2023-08-04 13:44:54.000000 types-aiobotocore-mgh-2.5.2.post2/setup.py
-drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:18.466643 types-aiobotocore-mgh-2.5.2.post2/types_aiobotocore_mgh/
--rw-r--r--   0 vlad      (1000) vlad      (1000)     1678 2023-08-04 13:44:54.000000 types-aiobotocore-mgh-2.5.2.post2/types_aiobotocore_mgh/__init__.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)     1677 2023-08-04 13:44:54.000000 types-aiobotocore-mgh-2.5.2.post2/types_aiobotocore_mgh/__init__.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)      934 2023-08-04 13:44:54.000000 types-aiobotocore-mgh-2.5.2.post2/types_aiobotocore_mgh/__main__.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)    18634 2023-08-04 13:44:54.000000 types-aiobotocore-mgh-2.5.2.post2/types_aiobotocore_mgh/client.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)    18603 2023-08-04 13:44:54.000000 types-aiobotocore-mgh-2.5.2.post2/types_aiobotocore_mgh/client.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)     9047 2023-08-04 13:44:56.000000 types-aiobotocore-mgh-2.5.2.post2/types_aiobotocore_mgh/literals.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)     9045 2023-08-04 13:44:54.000000 types-aiobotocore-mgh-2.5.2.post2/types_aiobotocore_mgh/literals.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)     6864 2023-08-04 13:44:54.000000 types-aiobotocore-mgh-2.5.2.post2/types_aiobotocore_mgh/paginator.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)     6857 2023-08-04 13:44:54.000000 types-aiobotocore-mgh-2.5.2.post2/types_aiobotocore_mgh/paginator.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:44:54.000000 types-aiobotocore-mgh-2.5.2.post2/types_aiobotocore_mgh/py.typed
--rw-r--r--   0 vlad      (1000) vlad      (1000)    17738 2023-08-04 13:44:56.000000 types-aiobotocore-mgh-2.5.2.post2/types_aiobotocore_mgh/type_defs.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)    17703 2023-08-04 13:44:56.000000 types-aiobotocore-mgh-2.5.2.post2/types_aiobotocore_mgh/type_defs.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)       65 2023-08-04 13:44:54.000000 types-aiobotocore-mgh-2.5.2.post2/types_aiobotocore_mgh/version.py
-drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:18.466643 types-aiobotocore-mgh-2.5.2.post2/types_aiobotocore_mgh.egg-info/
--rw-r--r--   0 vlad      (1000) vlad      (1000)    13515 2023-08-04 13:59:18.000000 types-aiobotocore-mgh-2.5.2.post2/types_aiobotocore_mgh.egg-info/PKG-INFO
--rw-r--r--   0 vlad      (1000) vlad      (1000)      737 2023-08-04 13:59:18.000000 types-aiobotocore-mgh-2.5.2.post2/types_aiobotocore_mgh.egg-info/SOURCES.txt
--rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:18.000000 types-aiobotocore-mgh-2.5.2.post2/types_aiobotocore_mgh.egg-info/dependency_links.txt
--rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:18.000000 types-aiobotocore-mgh-2.5.2.post2/types_aiobotocore_mgh.egg-info/not-zip-safe
--rw-r--r--   0 vlad      (1000) vlad      (1000)       52 2023-08-04 13:59:18.000000 types-aiobotocore-mgh-2.5.2.post2/types_aiobotocore_mgh.egg-info/requires.txt
--rw-r--r--   0 vlad      (1000) vlad      (1000)       22 2023-08-04 13:59:18.000000 types-aiobotocore-mgh-2.5.2.post2/types_aiobotocore_mgh.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:24:06.978736 types-aiobotocore-mgh-2.5.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-08 01:15:28.000000 types-aiobotocore-mgh-2.5.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    13509 2023-08-08 01:24:06.978736 types-aiobotocore-mgh-2.5.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    12004 2023-08-08 01:15:28.000000 types-aiobotocore-mgh-2.5.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-08 01:24:06.978736 types-aiobotocore-mgh-2.5.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2023 2023-08-08 01:15:28.000000 types-aiobotocore-mgh-2.5.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:24:06.966736 types-aiobotocore-mgh-2.5.4/types_aiobotocore_mgh/
+-rw-r--r--   0 runner    (1001) docker     (123)     1678 2023-08-08 01:15:28.000000 types-aiobotocore-mgh-2.5.4/types_aiobotocore_mgh/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1677 2023-08-08 01:15:28.000000 types-aiobotocore-mgh-2.5.4/types_aiobotocore_mgh/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      922 2023-08-08 01:15:28.000000 types-aiobotocore-mgh-2.5.4/types_aiobotocore_mgh/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18634 2023-08-08 01:15:28.000000 types-aiobotocore-mgh-2.5.4/types_aiobotocore_mgh/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18603 2023-08-08 01:15:28.000000 types-aiobotocore-mgh-2.5.4/types_aiobotocore_mgh/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9047 2023-08-08 01:15:28.000000 types-aiobotocore-mgh-2.5.4/types_aiobotocore_mgh/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9045 2023-08-08 01:15:28.000000 types-aiobotocore-mgh-2.5.4/types_aiobotocore_mgh/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     6864 2023-08-08 01:15:28.000000 types-aiobotocore-mgh-2.5.4/types_aiobotocore_mgh/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6857 2023-08-08 01:15:28.000000 types-aiobotocore-mgh-2.5.4/types_aiobotocore_mgh/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 01:15:28.000000 types-aiobotocore-mgh-2.5.4/types_aiobotocore_mgh/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    17738 2023-08-08 01:15:29.000000 types-aiobotocore-mgh-2.5.4/types_aiobotocore_mgh/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17703 2023-08-08 01:15:28.000000 types-aiobotocore-mgh-2.5.4/types_aiobotocore_mgh/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-08-08 01:15:28.000000 types-aiobotocore-mgh-2.5.4/types_aiobotocore_mgh/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:24:06.978736 types-aiobotocore-mgh-2.5.4/types_aiobotocore_mgh.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    13509 2023-08-08 01:24:06.000000 types-aiobotocore-mgh-2.5.4/types_aiobotocore_mgh.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      737 2023-08-08 01:24:06.000000 types-aiobotocore-mgh-2.5.4/types_aiobotocore_mgh.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 01:24:06.000000 types-aiobotocore-mgh-2.5.4/types_aiobotocore_mgh.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 01:24:06.000000 types-aiobotocore-mgh-2.5.4/types_aiobotocore_mgh.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-08 01:24:06.000000 types-aiobotocore-mgh-2.5.4/types_aiobotocore_mgh.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-08-08 01:24:06.000000 types-aiobotocore-mgh-2.5.4/types_aiobotocore_mgh.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-mgh-2.5.2.post2/LICENSE` & `types-aiobotocore-mgh-2.5.4/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-mgh-2.5.2.post2/PKG-INFO` & `types-aiobotocore-mgh-2.5.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-mgh
-Version: 2.5.2.post2
-Summary: Type annotations for aiobotocore.MigrationHub 2.5.2 service generated with mypy-boto3-builder 7.17.2
+Version: 2.5.4
+Summary: Type annotations for aiobotocore.MigrationHub 2.5.4 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mgh/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-mgh.svg?color=blue)](https://pypi.org/project/types-aiobotocore-mgh)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mgh/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-mgh)](https://pepy.tech/project/types-aiobotocore-mgh)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.MigrationHub 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgh.html#MigrationHub)
+[aiobotocore.MigrationHub 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgh.html#MigrationHub)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-mgh-2.5.2.post2/README.md` & `types-aiobotocore-mgh-2.5.4/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-mgh.svg?color=blue)](https://pypi.org/project/types-aiobotocore-mgh)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mgh/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-mgh)](https://pepy.tech/project/types-aiobotocore-mgh)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.MigrationHub 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgh.html#MigrationHub)
+[aiobotocore.MigrationHub 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgh.html#MigrationHub)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-mgh-2.5.2.post2/setup.py` & `types-aiobotocore-mgh-2.5.4/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-mgh",
-    version="2.5.2.post2",
+    version="2.5.4",
     packages=["types_aiobotocore_mgh"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.MigrationHub 2.5.2 service generated with"
+        "Type annotations for aiobotocore.MigrationHub 2.5.4 service generated with"
         " mypy-boto3-builder 7.17.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
```

### Comparing `types-aiobotocore-mgh-2.5.2.post2/types_aiobotocore_mgh/__init__.py` & `types-aiobotocore-mgh-2.5.4/types_aiobotocore_mgh/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-mgh-2.5.2.post2/types_aiobotocore_mgh/__init__.pyi` & `types-aiobotocore-mgh-2.5.4/types_aiobotocore_mgh/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-mgh-2.5.2.post2/types_aiobotocore_mgh/__main__.py` & `types-aiobotocore-mgh-2.5.4/types_aiobotocore_mgh/__main__.py`

 * *Files 22% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.MigrationHub 2.5.2\nVersion:         2.5.2.post2\nBuilder"
+        "Type annotations for aiobotocore.MigrationHub 2.5.4\nVersion:         2.5.4\nBuilder"
         " version: 7.17.2\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mgh//\nBoto3 docs:    "
         "  https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgh.html#MigrationHub\nOther"
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

### Comparing `types-aiobotocore-mgh-2.5.2.post2/types_aiobotocore_mgh/client.py` & `types-aiobotocore-mgh-2.5.4/types_aiobotocore_mgh/client.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-mgh-2.5.2.post2/types_aiobotocore_mgh/client.pyi` & `types-aiobotocore-mgh-2.5.4/types_aiobotocore_mgh/client.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-mgh-2.5.2.post2/types_aiobotocore_mgh/literals.py` & `types-aiobotocore-mgh-2.5.4/types_aiobotocore_mgh/literals.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-mgh-2.5.2.post2/types_aiobotocore_mgh/literals.pyi` & `types-aiobotocore-mgh-2.5.4/types_aiobotocore_mgh/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-mgh-2.5.2.post2/types_aiobotocore_mgh/paginator.py` & `types-aiobotocore-mgh-2.5.4/types_aiobotocore_mgh/paginator.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-mgh-2.5.2.post2/types_aiobotocore_mgh/paginator.pyi` & `types-aiobotocore-mgh-2.5.4/types_aiobotocore_mgh/paginator.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-mgh-2.5.2.post2/types_aiobotocore_mgh/type_defs.py` & `types-aiobotocore-mgh-2.5.4/types_aiobotocore_mgh/type_defs.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-mgh-2.5.2.post2/types_aiobotocore_mgh/type_defs.pyi` & `types-aiobotocore-mgh-2.5.4/types_aiobotocore_mgh/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-mgh-2.5.2.post2/types_aiobotocore_mgh.egg-info/PKG-INFO` & `types-aiobotocore-mgh-2.5.4/types_aiobotocore_mgh.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-mgh
-Version: 2.5.2.post2
-Summary: Type annotations for aiobotocore.MigrationHub 2.5.2 service generated with mypy-boto3-builder 7.17.2
+Version: 2.5.4
+Summary: Type annotations for aiobotocore.MigrationHub 2.5.4 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mgh/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-mgh.svg?color=blue)](https://pypi.org/project/types-aiobotocore-mgh)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mgh/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-mgh)](https://pepy.tech/project/types-aiobotocore-mgh)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.MigrationHub 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgh.html#MigrationHub)
+[aiobotocore.MigrationHub 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgh.html#MigrationHub)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-mgh-2.5.2.post2/types_aiobotocore_mgh.egg-info/SOURCES.txt` & `types-aiobotocore-mgh-2.5.4/types_aiobotocore_mgh.egg-info/SOURCES.txt`

 * *Files identical despite different names*


# Comparing `tmp/types-aiobotocore-rolesanywhere-2.5.2.post2.tar.gz` & `tmp/types-aiobotocore-rolesanywhere-2.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-rolesanywhere-2.5.2.post2.tar", last modified: Fri Aug  4 13:59:23 2023, max compression
+gzip compressed data, was "types-aiobotocore-rolesanywhere-2.5.4.tar", last modified: Tue Aug  8 01:24:20 2023, max compression
```

## Comparing `types-aiobotocore-rolesanywhere-2.5.2.post2.tar` & `types-aiobotocore-rolesanywhere-2.5.4.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:23.826643 types-aiobotocore-rolesanywhere-2.5.2.post2/
--rw-r--r--   0 vlad      (1000) vlad      (1000)     1070 2023-08-04 13:50:57.000000 types-aiobotocore-rolesanywhere-2.5.2.post2/LICENSE
--rw-r--r--   0 vlad      (1000) vlad      (1000)    13643 2023-08-04 13:59:23.826643 types-aiobotocore-rolesanywhere-2.5.2.post2/PKG-INFO
--rw-r--r--   0 vlad      (1000) vlad      (1000)    12098 2023-08-04 13:50:57.000000 types-aiobotocore-rolesanywhere-2.5.2.post2/README.md
--rw-r--r--   0 vlad      (1000) vlad      (1000)       38 2023-08-04 13:59:23.826643 types-aiobotocore-rolesanywhere-2.5.2.post2/setup.cfg
--rw-r--r--   0 vlad      (1000) vlad      (1000)     2117 2023-08-04 13:50:57.000000 types-aiobotocore-rolesanywhere-2.5.2.post2/setup.py
-drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:23.816643 types-aiobotocore-rolesanywhere-2.5.2.post2/types_aiobotocore_rolesanywhere/
--rw-r--r--   0 vlad      (1000) vlad      (1000)     1258 2023-08-04 13:50:57.000000 types-aiobotocore-rolesanywhere-2.5.2.post2/types_aiobotocore_rolesanywhere/__init__.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)     1257 2023-08-04 13:50:57.000000 types-aiobotocore-rolesanywhere-2.5.2.post2/types_aiobotocore_rolesanywhere/__init__.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)      973 2023-08-04 13:50:57.000000 types-aiobotocore-rolesanywhere-2.5.2.post2/types_aiobotocore_rolesanywhere/__main__.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)    22225 2023-08-04 13:50:58.000000 types-aiobotocore-rolesanywhere-2.5.2.post2/types_aiobotocore_rolesanywhere/client.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)    22184 2023-08-04 13:50:58.000000 types-aiobotocore-rolesanywhere-2.5.2.post2/types_aiobotocore_rolesanywhere/client.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)     8892 2023-08-04 13:50:58.000000 types-aiobotocore-rolesanywhere-2.5.2.post2/types_aiobotocore_rolesanywhere/literals.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)     8890 2023-08-04 13:50:58.000000 types-aiobotocore-rolesanywhere-2.5.2.post2/types_aiobotocore_rolesanywhere/literals.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)     5378 2023-08-04 13:50:58.000000 types-aiobotocore-rolesanywhere-2.5.2.post2/types_aiobotocore_rolesanywhere/paginator.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)     5372 2023-08-04 13:50:58.000000 types-aiobotocore-rolesanywhere-2.5.2.post2/types_aiobotocore_rolesanywhere/paginator.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:50:57.000000 types-aiobotocore-rolesanywhere-2.5.2.post2/types_aiobotocore_rolesanywhere/py.typed
--rw-r--r--   0 vlad      (1000) vlad      (1000)    15346 2023-08-04 13:50:58.000000 types-aiobotocore-rolesanywhere-2.5.2.post2/types_aiobotocore_rolesanywhere/type_defs.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)    15327 2023-08-04 13:50:58.000000 types-aiobotocore-rolesanywhere-2.5.2.post2/types_aiobotocore_rolesanywhere/type_defs.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)       65 2023-08-04 13:50:57.000000 types-aiobotocore-rolesanywhere-2.5.2.post2/types_aiobotocore_rolesanywhere/version.py
-drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:23.826643 types-aiobotocore-rolesanywhere-2.5.2.post2/types_aiobotocore_rolesanywhere.egg-info/
--rw-r--r--   0 vlad      (1000) vlad      (1000)    13643 2023-08-04 13:59:23.000000 types-aiobotocore-rolesanywhere-2.5.2.post2/types_aiobotocore_rolesanywhere.egg-info/PKG-INFO
--rw-r--r--   0 vlad      (1000) vlad      (1000)      927 2023-08-04 13:59:23.000000 types-aiobotocore-rolesanywhere-2.5.2.post2/types_aiobotocore_rolesanywhere.egg-info/SOURCES.txt
--rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:23.000000 types-aiobotocore-rolesanywhere-2.5.2.post2/types_aiobotocore_rolesanywhere.egg-info/dependency_links.txt
--rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:23.000000 types-aiobotocore-rolesanywhere-2.5.2.post2/types_aiobotocore_rolesanywhere.egg-info/not-zip-safe
--rw-r--r--   0 vlad      (1000) vlad      (1000)       52 2023-08-04 13:59:23.000000 types-aiobotocore-rolesanywhere-2.5.2.post2/types_aiobotocore_rolesanywhere.egg-info/requires.txt
--rw-r--r--   0 vlad      (1000) vlad      (1000)       32 2023-08-04 13:59:23.000000 types-aiobotocore-rolesanywhere-2.5.2.post2/types_aiobotocore_rolesanywhere.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:24:20.042765 types-aiobotocore-rolesanywhere-2.5.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-08 01:19:31.000000 types-aiobotocore-rolesanywhere-2.5.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    13637 2023-08-08 01:24:20.042765 types-aiobotocore-rolesanywhere-2.5.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    12098 2023-08-08 01:19:31.000000 types-aiobotocore-rolesanywhere-2.5.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-08 01:24:20.042765 types-aiobotocore-rolesanywhere-2.5.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2111 2023-08-08 01:19:31.000000 types-aiobotocore-rolesanywhere-2.5.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:24:20.042765 types-aiobotocore-rolesanywhere-2.5.4/types_aiobotocore_rolesanywhere/
+-rw-r--r--   0 runner    (1001) docker     (123)     1258 2023-08-08 01:19:31.000000 types-aiobotocore-rolesanywhere-2.5.4/types_aiobotocore_rolesanywhere/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1257 2023-08-08 01:19:31.000000 types-aiobotocore-rolesanywhere-2.5.4/types_aiobotocore_rolesanywhere/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      961 2023-08-08 01:19:31.000000 types-aiobotocore-rolesanywhere-2.5.4/types_aiobotocore_rolesanywhere/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22225 2023-08-08 01:19:31.000000 types-aiobotocore-rolesanywhere-2.5.4/types_aiobotocore_rolesanywhere/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22184 2023-08-08 01:19:31.000000 types-aiobotocore-rolesanywhere-2.5.4/types_aiobotocore_rolesanywhere/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8892 2023-08-08 01:19:31.000000 types-aiobotocore-rolesanywhere-2.5.4/types_aiobotocore_rolesanywhere/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8890 2023-08-08 01:19:31.000000 types-aiobotocore-rolesanywhere-2.5.4/types_aiobotocore_rolesanywhere/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     5378 2023-08-08 01:19:31.000000 types-aiobotocore-rolesanywhere-2.5.4/types_aiobotocore_rolesanywhere/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5372 2023-08-08 01:19:31.000000 types-aiobotocore-rolesanywhere-2.5.4/types_aiobotocore_rolesanywhere/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 01:19:31.000000 types-aiobotocore-rolesanywhere-2.5.4/types_aiobotocore_rolesanywhere/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    15346 2023-08-08 01:19:32.000000 types-aiobotocore-rolesanywhere-2.5.4/types_aiobotocore_rolesanywhere/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15327 2023-08-08 01:19:32.000000 types-aiobotocore-rolesanywhere-2.5.4/types_aiobotocore_rolesanywhere/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-08-08 01:19:31.000000 types-aiobotocore-rolesanywhere-2.5.4/types_aiobotocore_rolesanywhere/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:24:20.042765 types-aiobotocore-rolesanywhere-2.5.4/types_aiobotocore_rolesanywhere.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    13637 2023-08-08 01:24:19.000000 types-aiobotocore-rolesanywhere-2.5.4/types_aiobotocore_rolesanywhere.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      927 2023-08-08 01:24:19.000000 types-aiobotocore-rolesanywhere-2.5.4/types_aiobotocore_rolesanywhere.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 01:24:19.000000 types-aiobotocore-rolesanywhere-2.5.4/types_aiobotocore_rolesanywhere.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 01:24:19.000000 types-aiobotocore-rolesanywhere-2.5.4/types_aiobotocore_rolesanywhere.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-08 01:24:19.000000 types-aiobotocore-rolesanywhere-2.5.4/types_aiobotocore_rolesanywhere.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-08-08 01:24:19.000000 types-aiobotocore-rolesanywhere-2.5.4/types_aiobotocore_rolesanywhere.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-rolesanywhere-2.5.2.post2/LICENSE` & `types-aiobotocore-rolesanywhere-2.5.4/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-rolesanywhere-2.5.2.post2/PKG-INFO` & `types-aiobotocore-rolesanywhere-2.5.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-rolesanywhere
-Version: 2.5.2.post2
-Summary: Type annotations for aiobotocore.IAMRolesAnywhere 2.5.2 service generated with mypy-boto3-builder 7.17.2
+Version: 2.5.4
+Summary: Type annotations for aiobotocore.IAMRolesAnywhere 2.5.4 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rolesanywhere/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-rolesanywhere.svg?color=blue)](https://pypi.org/project/types-aiobotocore-rolesanywhere)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rolesanywhere/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-rolesanywhere)](https://pepy.tech/project/types-aiobotocore-rolesanywhere)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.IAMRolesAnywhere 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rolesanywhere.html#IAMRolesAnywhere)
+[aiobotocore.IAMRolesAnywhere 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rolesanywhere.html#IAMRolesAnywhere)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-rolesanywhere-2.5.2.post2/README.md` & `types-aiobotocore-rolesanywhere-2.5.4/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-rolesanywhere.svg?color=blue)](https://pypi.org/project/types-aiobotocore-rolesanywhere)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rolesanywhere/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-rolesanywhere)](https://pepy.tech/project/types-aiobotocore-rolesanywhere)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.IAMRolesAnywhere 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rolesanywhere.html#IAMRolesAnywhere)
+[aiobotocore.IAMRolesAnywhere 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rolesanywhere.html#IAMRolesAnywhere)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-rolesanywhere-2.5.2.post2/setup.py` & `types-aiobotocore-rolesanywhere-2.5.4/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-rolesanywhere",
-    version="2.5.2.post2",
+    version="2.5.4",
     packages=["types_aiobotocore_rolesanywhere"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.IAMRolesAnywhere 2.5.2 service generated with"
+        "Type annotations for aiobotocore.IAMRolesAnywhere 2.5.4 service generated with"
         " mypy-boto3-builder 7.17.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
```

### Comparing `types-aiobotocore-rolesanywhere-2.5.2.post2/types_aiobotocore_rolesanywhere/__init__.py` & `types-aiobotocore-rolesanywhere-2.5.4/types_aiobotocore_rolesanywhere/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-rolesanywhere-2.5.2.post2/types_aiobotocore_rolesanywhere/__init__.pyi` & `types-aiobotocore-rolesanywhere-2.5.4/types_aiobotocore_rolesanywhere/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-rolesanywhere-2.5.2.post2/types_aiobotocore_rolesanywhere/__main__.py` & `types-aiobotocore-rolesanywhere-2.5.4/types_aiobotocore_rolesanywhere/__main__.py`

 * *Files 26% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.IAMRolesAnywhere 2.5.2\nVersion:        "
-        " 2.5.2.post2\nBuilder version: 7.17.2\nDocs:           "
+        "Type annotations for aiobotocore.IAMRolesAnywhere 2.5.4\nVersion:         2.5.4\nBuilder"
+        " version: 7.17.2\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rolesanywhere//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rolesanywhere.html#IAMRolesAnywhere\nOther"
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

### Comparing `types-aiobotocore-rolesanywhere-2.5.2.post2/types_aiobotocore_rolesanywhere/client.py` & `types-aiobotocore-rolesanywhere-2.5.4/types_aiobotocore_rolesanywhere/client.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-rolesanywhere-2.5.2.post2/types_aiobotocore_rolesanywhere/client.pyi` & `types-aiobotocore-rolesanywhere-2.5.4/types_aiobotocore_rolesanywhere/client.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-rolesanywhere-2.5.2.post2/types_aiobotocore_rolesanywhere/literals.py` & `types-aiobotocore-rolesanywhere-2.5.4/types_aiobotocore_rolesanywhere/literals.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-rolesanywhere-2.5.2.post2/types_aiobotocore_rolesanywhere/literals.pyi` & `types-aiobotocore-rolesanywhere-2.5.4/types_aiobotocore_rolesanywhere/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-rolesanywhere-2.5.2.post2/types_aiobotocore_rolesanywhere/paginator.py` & `types-aiobotocore-rolesanywhere-2.5.4/types_aiobotocore_rolesanywhere/paginator.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-rolesanywhere-2.5.2.post2/types_aiobotocore_rolesanywhere/paginator.pyi` & `types-aiobotocore-rolesanywhere-2.5.4/types_aiobotocore_rolesanywhere/paginator.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-rolesanywhere-2.5.2.post2/types_aiobotocore_rolesanywhere/type_defs.py` & `types-aiobotocore-rolesanywhere-2.5.4/types_aiobotocore_rolesanywhere/type_defs.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-rolesanywhere-2.5.2.post2/types_aiobotocore_rolesanywhere/type_defs.pyi` & `types-aiobotocore-rolesanywhere-2.5.4/types_aiobotocore_rolesanywhere/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-rolesanywhere-2.5.2.post2/types_aiobotocore_rolesanywhere.egg-info/PKG-INFO` & `types-aiobotocore-rolesanywhere-2.5.4/types_aiobotocore_rolesanywhere.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-rolesanywhere
-Version: 2.5.2.post2
-Summary: Type annotations for aiobotocore.IAMRolesAnywhere 2.5.2 service generated with mypy-boto3-builder 7.17.2
+Version: 2.5.4
+Summary: Type annotations for aiobotocore.IAMRolesAnywhere 2.5.4 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rolesanywhere/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-rolesanywhere.svg?color=blue)](https://pypi.org/project/types-aiobotocore-rolesanywhere)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rolesanywhere/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-rolesanywhere)](https://pepy.tech/project/types-aiobotocore-rolesanywhere)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.IAMRolesAnywhere 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rolesanywhere.html#IAMRolesAnywhere)
+[aiobotocore.IAMRolesAnywhere 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rolesanywhere.html#IAMRolesAnywhere)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-rolesanywhere-2.5.2.post2/types_aiobotocore_rolesanywhere.egg-info/SOURCES.txt` & `types-aiobotocore-rolesanywhere-2.5.4/types_aiobotocore_rolesanywhere.egg-info/SOURCES.txt`

 * *Files identical despite different names*


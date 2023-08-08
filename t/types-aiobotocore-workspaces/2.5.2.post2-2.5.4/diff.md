# Comparing `tmp/types-aiobotocore-workspaces-2.5.2.post2.tar.gz` & `tmp/types-aiobotocore-workspaces-2.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-workspaces-2.5.2.post2.tar", last modified: Fri Aug  4 13:59:30 2023, max compression
+gzip compressed data, was "types-aiobotocore-workspaces-2.5.4.tar", last modified: Tue Aug  8 01:24:36 2023, max compression
```

## Comparing `types-aiobotocore-workspaces-2.5.2.post2.tar` & `types-aiobotocore-workspaces-2.5.4.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:30.446643 types-aiobotocore-workspaces-2.5.2.post2/
--rw-r--r--   0 vlad      (1000) vlad      (1000)     1070 2023-08-04 13:56:19.000000 types-aiobotocore-workspaces-2.5.2.post2/LICENSE
--rw-r--r--   0 vlad      (1000) vlad      (1000)    14495 2023-08-04 13:59:30.446643 types-aiobotocore-workspaces-2.5.2.post2/PKG-INFO
--rw-r--r--   0 vlad      (1000) vlad      (1000)    12965 2023-08-04 13:56:19.000000 types-aiobotocore-workspaces-2.5.2.post2/README.md
--rw-r--r--   0 vlad      (1000) vlad      (1000)       38 2023-08-04 13:59:30.446643 types-aiobotocore-workspaces-2.5.2.post2/setup.cfg
--rw-r--r--   0 vlad      (1000) vlad      (1000)     2093 2023-08-04 13:56:19.000000 types-aiobotocore-workspaces-2.5.2.post2/setup.py
-drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:30.446643 types-aiobotocore-workspaces-2.5.2.post2/types_aiobotocore_workspaces/
--rw-r--r--   0 vlad      (1000) vlad      (1000)     2597 2023-08-04 13:56:19.000000 types-aiobotocore-workspaces-2.5.2.post2/types_aiobotocore_workspaces/__init__.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)     2596 2023-08-04 13:56:19.000000 types-aiobotocore-workspaces-2.5.2.post2/types_aiobotocore_workspaces/__init__.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)      955 2023-08-04 13:56:19.000000 types-aiobotocore-workspaces-2.5.2.post2/types_aiobotocore_workspaces/__main__.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)    50842 2023-08-04 13:56:19.000000 types-aiobotocore-workspaces-2.5.2.post2/types_aiobotocore_workspaces/client.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)    50760 2023-08-04 13:56:19.000000 types-aiobotocore-workspaces-2.5.2.post2/types_aiobotocore_workspaces/client.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)    13374 2023-08-04 13:56:20.000000 types-aiobotocore-workspaces-2.5.2.post2/types_aiobotocore_workspaces/literals.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)    13372 2023-08-04 13:56:19.000000 types-aiobotocore-workspaces-2.5.2.post2/types_aiobotocore_workspaces/literals.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)    11220 2023-08-04 13:56:19.000000 types-aiobotocore-workspaces-2.5.2.post2/types_aiobotocore_workspaces/paginator.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)    11210 2023-08-04 13:56:19.000000 types-aiobotocore-workspaces-2.5.2.post2/types_aiobotocore_workspaces/paginator.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:56:19.000000 types-aiobotocore-workspaces-2.5.2.post2/types_aiobotocore_workspaces/py.typed
--rw-r--r--   0 vlad      (1000) vlad      (1000)    53880 2023-08-04 13:56:21.000000 types-aiobotocore-workspaces-2.5.2.post2/types_aiobotocore_workspaces/type_defs.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)    53839 2023-08-04 13:56:20.000000 types-aiobotocore-workspaces-2.5.2.post2/types_aiobotocore_workspaces/type_defs.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)       65 2023-08-04 13:56:19.000000 types-aiobotocore-workspaces-2.5.2.post2/types_aiobotocore_workspaces/version.py
-drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:30.446643 types-aiobotocore-workspaces-2.5.2.post2/types_aiobotocore_workspaces.egg-info/
--rw-r--r--   0 vlad      (1000) vlad      (1000)    14495 2023-08-04 13:59:30.000000 types-aiobotocore-workspaces-2.5.2.post2/types_aiobotocore_workspaces.egg-info/PKG-INFO
--rw-r--r--   0 vlad      (1000) vlad      (1000)      870 2023-08-04 13:59:30.000000 types-aiobotocore-workspaces-2.5.2.post2/types_aiobotocore_workspaces.egg-info/SOURCES.txt
--rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:30.000000 types-aiobotocore-workspaces-2.5.2.post2/types_aiobotocore_workspaces.egg-info/dependency_links.txt
--rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:30.000000 types-aiobotocore-workspaces-2.5.2.post2/types_aiobotocore_workspaces.egg-info/not-zip-safe
--rw-r--r--   0 vlad      (1000) vlad      (1000)       52 2023-08-04 13:59:30.000000 types-aiobotocore-workspaces-2.5.2.post2/types_aiobotocore_workspaces.egg-info/requires.txt
--rw-r--r--   0 vlad      (1000) vlad      (1000)       29 2023-08-04 13:59:30.000000 types-aiobotocore-workspaces-2.5.2.post2/types_aiobotocore_workspaces.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:24:36.814806 types-aiobotocore-workspaces-2.5.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-08 01:22:46.000000 types-aiobotocore-workspaces-2.5.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    14489 2023-08-08 01:24:36.810806 types-aiobotocore-workspaces-2.5.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    12965 2023-08-08 01:22:46.000000 types-aiobotocore-workspaces-2.5.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-08 01:24:36.814806 types-aiobotocore-workspaces-2.5.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2087 2023-08-08 01:22:46.000000 types-aiobotocore-workspaces-2.5.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:24:36.810806 types-aiobotocore-workspaces-2.5.4/types_aiobotocore_workspaces/
+-rw-r--r--   0 runner    (1001) docker     (123)     2597 2023-08-08 01:22:46.000000 types-aiobotocore-workspaces-2.5.4/types_aiobotocore_workspaces/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2596 2023-08-08 01:22:46.000000 types-aiobotocore-workspaces-2.5.4/types_aiobotocore_workspaces/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      943 2023-08-08 01:22:46.000000 types-aiobotocore-workspaces-2.5.4/types_aiobotocore_workspaces/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    50842 2023-08-08 01:22:46.000000 types-aiobotocore-workspaces-2.5.4/types_aiobotocore_workspaces/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    50760 2023-08-08 01:22:46.000000 types-aiobotocore-workspaces-2.5.4/types_aiobotocore_workspaces/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    13374 2023-08-08 01:22:47.000000 types-aiobotocore-workspaces-2.5.4/types_aiobotocore_workspaces/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13372 2023-08-08 01:22:46.000000 types-aiobotocore-workspaces-2.5.4/types_aiobotocore_workspaces/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    11220 2023-08-08 01:22:46.000000 types-aiobotocore-workspaces-2.5.4/types_aiobotocore_workspaces/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11210 2023-08-08 01:22:46.000000 types-aiobotocore-workspaces-2.5.4/types_aiobotocore_workspaces/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 01:22:46.000000 types-aiobotocore-workspaces-2.5.4/types_aiobotocore_workspaces/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    53880 2023-08-08 01:22:48.000000 types-aiobotocore-workspaces-2.5.4/types_aiobotocore_workspaces/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    53839 2023-08-08 01:22:47.000000 types-aiobotocore-workspaces-2.5.4/types_aiobotocore_workspaces/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-08-08 01:22:46.000000 types-aiobotocore-workspaces-2.5.4/types_aiobotocore_workspaces/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:24:36.810806 types-aiobotocore-workspaces-2.5.4/types_aiobotocore_workspaces.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    14489 2023-08-08 01:24:36.000000 types-aiobotocore-workspaces-2.5.4/types_aiobotocore_workspaces.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      870 2023-08-08 01:24:36.000000 types-aiobotocore-workspaces-2.5.4/types_aiobotocore_workspaces.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 01:24:36.000000 types-aiobotocore-workspaces-2.5.4/types_aiobotocore_workspaces.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 01:24:36.000000 types-aiobotocore-workspaces-2.5.4/types_aiobotocore_workspaces.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-08 01:24:36.000000 types-aiobotocore-workspaces-2.5.4/types_aiobotocore_workspaces.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-08-08 01:24:36.000000 types-aiobotocore-workspaces-2.5.4/types_aiobotocore_workspaces.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-workspaces-2.5.2.post2/LICENSE` & `types-aiobotocore-workspaces-2.5.4/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-workspaces-2.5.2.post2/PKG-INFO` & `types-aiobotocore-workspaces-2.5.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-workspaces
-Version: 2.5.2.post2
-Summary: Type annotations for aiobotocore.WorkSpaces 2.5.2 service generated with mypy-boto3-builder 7.17.2
+Version: 2.5.4
+Summary: Type annotations for aiobotocore.WorkSpaces 2.5.4 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_workspaces/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-workspaces.svg?color=blue)](https://pypi.org/project/types-aiobotocore-workspaces)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_workspaces/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-workspaces)](https://pepy.tech/project/types-aiobotocore-workspaces)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.WorkSpaces 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces.html#WorkSpaces)
+[aiobotocore.WorkSpaces 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces.html#WorkSpaces)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-workspaces-2.5.2.post2/README.md` & `types-aiobotocore-workspaces-2.5.4/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-workspaces.svg?color=blue)](https://pypi.org/project/types-aiobotocore-workspaces)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_workspaces/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-workspaces)](https://pepy.tech/project/types-aiobotocore-workspaces)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.WorkSpaces 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces.html#WorkSpaces)
+[aiobotocore.WorkSpaces 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces.html#WorkSpaces)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-workspaces-2.5.2.post2/setup.py` & `types-aiobotocore-workspaces-2.5.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-workspaces",
-    version="2.5.2.post2",
+    version="2.5.4",
     packages=["types_aiobotocore_workspaces"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.WorkSpaces 2.5.2 service generated with"
+        "Type annotations for aiobotocore.WorkSpaces 2.5.4 service generated with"
         " mypy-boto3-builder 7.17.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
```

### Comparing `types-aiobotocore-workspaces-2.5.2.post2/types_aiobotocore_workspaces/__init__.py` & `types-aiobotocore-workspaces-2.5.4/types_aiobotocore_workspaces/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-workspaces-2.5.2.post2/types_aiobotocore_workspaces/__init__.pyi` & `types-aiobotocore-workspaces-2.5.4/types_aiobotocore_workspaces/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-workspaces-2.5.2.post2/types_aiobotocore_workspaces/__main__.py` & `types-aiobotocore-workspaces-2.5.4/types_aiobotocore_workspaces/__main__.py`

 * *Files 25% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.WorkSpaces 2.5.2\nVersion:         2.5.2.post2\nBuilder"
+        "Type annotations for aiobotocore.WorkSpaces 2.5.4\nVersion:         2.5.4\nBuilder"
         " version: 7.17.2\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_workspaces//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces.html#WorkSpaces\nOther"
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

### Comparing `types-aiobotocore-workspaces-2.5.2.post2/types_aiobotocore_workspaces/client.py` & `types-aiobotocore-workspaces-2.5.4/types_aiobotocore_workspaces/client.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-workspaces-2.5.2.post2/types_aiobotocore_workspaces/client.pyi` & `types-aiobotocore-workspaces-2.5.4/types_aiobotocore_workspaces/client.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-workspaces-2.5.2.post2/types_aiobotocore_workspaces/literals.py` & `types-aiobotocore-workspaces-2.5.4/types_aiobotocore_workspaces/literals.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-workspaces-2.5.2.post2/types_aiobotocore_workspaces/literals.pyi` & `types-aiobotocore-workspaces-2.5.4/types_aiobotocore_workspaces/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-workspaces-2.5.2.post2/types_aiobotocore_workspaces/paginator.py` & `types-aiobotocore-workspaces-2.5.4/types_aiobotocore_workspaces/paginator.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-workspaces-2.5.2.post2/types_aiobotocore_workspaces/paginator.pyi` & `types-aiobotocore-workspaces-2.5.4/types_aiobotocore_workspaces/paginator.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-workspaces-2.5.2.post2/types_aiobotocore_workspaces/type_defs.py` & `types-aiobotocore-workspaces-2.5.4/types_aiobotocore_workspaces/type_defs.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-workspaces-2.5.2.post2/types_aiobotocore_workspaces/type_defs.pyi` & `types-aiobotocore-workspaces-2.5.4/types_aiobotocore_workspaces/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-workspaces-2.5.2.post2/types_aiobotocore_workspaces.egg-info/PKG-INFO` & `types-aiobotocore-workspaces-2.5.4/types_aiobotocore_workspaces.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-workspaces
-Version: 2.5.2.post2
-Summary: Type annotations for aiobotocore.WorkSpaces 2.5.2 service generated with mypy-boto3-builder 7.17.2
+Version: 2.5.4
+Summary: Type annotations for aiobotocore.WorkSpaces 2.5.4 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_workspaces/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-workspaces.svg?color=blue)](https://pypi.org/project/types-aiobotocore-workspaces)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_workspaces/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-workspaces)](https://pepy.tech/project/types-aiobotocore-workspaces)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.WorkSpaces 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces.html#WorkSpaces)
+[aiobotocore.WorkSpaces 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces.html#WorkSpaces)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-workspaces-2.5.2.post2/types_aiobotocore_workspaces.egg-info/SOURCES.txt` & `types-aiobotocore-workspaces-2.5.4/types_aiobotocore_workspaces.egg-info/SOURCES.txt`

 * *Files identical despite different names*


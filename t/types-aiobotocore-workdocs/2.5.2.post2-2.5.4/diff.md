# Comparing `tmp/types-aiobotocore-workdocs-2.5.2.post2.tar.gz` & `tmp/types-aiobotocore-workdocs-2.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-workdocs-2.5.2.post2.tar", last modified: Fri Aug  4 13:59:30 2023, max compression
+gzip compressed data, was "types-aiobotocore-workdocs-2.5.4.tar", last modified: Tue Aug  8 01:24:36 2023, max compression
```

## Comparing `types-aiobotocore-workdocs-2.5.2.post2.tar` & `types-aiobotocore-workdocs-2.5.4.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:30.166643 types-aiobotocore-workdocs-2.5.2.post2/
--rw-r--r--   0 vlad      (1000) vlad      (1000)     1070 2023-08-04 13:56:05.000000 types-aiobotocore-workdocs-2.5.2.post2/LICENSE
--rw-r--r--   0 vlad      (1000) vlad      (1000)    14505 2023-08-04 13:59:30.166643 types-aiobotocore-workdocs-2.5.2.post2/PKG-INFO
--rw-r--r--   0 vlad      (1000) vlad      (1000)    12983 2023-08-04 13:56:05.000000 types-aiobotocore-workdocs-2.5.2.post2/README.md
--rw-r--r--   0 vlad      (1000) vlad      (1000)       38 2023-08-04 13:59:30.166643 types-aiobotocore-workdocs-2.5.2.post2/setup.cfg
--rw-r--r--   0 vlad      (1000) vlad      (1000)     2079 2023-08-04 13:56:05.000000 types-aiobotocore-workdocs-2.5.2.post2/setup.py
-drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:30.156643 types-aiobotocore-workdocs-2.5.2.post2/types_aiobotocore_workdocs/
--rw-r--r--   0 vlad      (1000) vlad      (1000)     2765 2023-08-04 13:56:05.000000 types-aiobotocore-workdocs-2.5.2.post2/types_aiobotocore_workdocs/__init__.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)     2764 2023-08-04 13:56:05.000000 types-aiobotocore-workdocs-2.5.2.post2/types_aiobotocore_workdocs/__init__.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)      947 2023-08-04 13:56:05.000000 types-aiobotocore-workdocs-2.5.2.post2/types_aiobotocore_workdocs/__main__.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)    40851 2023-08-04 13:56:05.000000 types-aiobotocore-workdocs-2.5.2.post2/types_aiobotocore_workdocs/client.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)    40788 2023-08-04 13:56:05.000000 types-aiobotocore-workdocs-2.5.2.post2/types_aiobotocore_workdocs/client.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)    13900 2023-08-04 13:56:06.000000 types-aiobotocore-workdocs-2.5.2.post2/types_aiobotocore_workdocs/literals.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)    13898 2023-08-04 13:56:05.000000 types-aiobotocore-workdocs-2.5.2.post2/types_aiobotocore_workdocs/literals.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)    14406 2023-08-04 13:56:05.000000 types-aiobotocore-workdocs-2.5.2.post2/types_aiobotocore_workdocs/paginator.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)    14393 2023-08-04 13:56:05.000000 types-aiobotocore-workdocs-2.5.2.post2/types_aiobotocore_workdocs/paginator.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:56:05.000000 types-aiobotocore-workdocs-2.5.2.post2/types_aiobotocore_workdocs/py.typed
--rw-r--r--   0 vlad      (1000) vlad      (1000)    50590 2023-08-04 13:56:10.000000 types-aiobotocore-workdocs-2.5.2.post2/types_aiobotocore_workdocs/type_defs.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)    50499 2023-08-04 13:56:06.000000 types-aiobotocore-workdocs-2.5.2.post2/types_aiobotocore_workdocs/type_defs.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)       65 2023-08-04 13:56:05.000000 types-aiobotocore-workdocs-2.5.2.post2/types_aiobotocore_workdocs/version.py
-drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:30.166643 types-aiobotocore-workdocs-2.5.2.post2/types_aiobotocore_workdocs.egg-info/
--rw-r--r--   0 vlad      (1000) vlad      (1000)    14505 2023-08-04 13:59:30.000000 types-aiobotocore-workdocs-2.5.2.post2/types_aiobotocore_workdocs.egg-info/PKG-INFO
--rw-r--r--   0 vlad      (1000) vlad      (1000)      832 2023-08-04 13:59:30.000000 types-aiobotocore-workdocs-2.5.2.post2/types_aiobotocore_workdocs.egg-info/SOURCES.txt
--rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:30.000000 types-aiobotocore-workdocs-2.5.2.post2/types_aiobotocore_workdocs.egg-info/dependency_links.txt
--rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:30.000000 types-aiobotocore-workdocs-2.5.2.post2/types_aiobotocore_workdocs.egg-info/not-zip-safe
--rw-r--r--   0 vlad      (1000) vlad      (1000)       52 2023-08-04 13:59:30.000000 types-aiobotocore-workdocs-2.5.2.post2/types_aiobotocore_workdocs.egg-info/requires.txt
--rw-r--r--   0 vlad      (1000) vlad      (1000)       27 2023-08-04 13:59:30.000000 types-aiobotocore-workdocs-2.5.2.post2/types_aiobotocore_workdocs.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:24:36.234804 types-aiobotocore-workdocs-2.5.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-08 01:22:36.000000 types-aiobotocore-workdocs-2.5.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    14499 2023-08-08 01:24:36.234804 types-aiobotocore-workdocs-2.5.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    12983 2023-08-08 01:22:36.000000 types-aiobotocore-workdocs-2.5.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-08 01:24:36.234804 types-aiobotocore-workdocs-2.5.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2073 2023-08-08 01:22:36.000000 types-aiobotocore-workdocs-2.5.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:24:36.226804 types-aiobotocore-workdocs-2.5.4/types_aiobotocore_workdocs/
+-rw-r--r--   0 runner    (1001) docker     (123)     2765 2023-08-08 01:22:36.000000 types-aiobotocore-workdocs-2.5.4/types_aiobotocore_workdocs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2764 2023-08-08 01:22:36.000000 types-aiobotocore-workdocs-2.5.4/types_aiobotocore_workdocs/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      935 2023-08-08 01:22:36.000000 types-aiobotocore-workdocs-2.5.4/types_aiobotocore_workdocs/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40851 2023-08-08 01:22:37.000000 types-aiobotocore-workdocs-2.5.4/types_aiobotocore_workdocs/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40788 2023-08-08 01:22:37.000000 types-aiobotocore-workdocs-2.5.4/types_aiobotocore_workdocs/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    13900 2023-08-08 01:22:37.000000 types-aiobotocore-workdocs-2.5.4/types_aiobotocore_workdocs/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13898 2023-08-08 01:22:37.000000 types-aiobotocore-workdocs-2.5.4/types_aiobotocore_workdocs/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    14406 2023-08-08 01:22:37.000000 types-aiobotocore-workdocs-2.5.4/types_aiobotocore_workdocs/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14393 2023-08-08 01:22:37.000000 types-aiobotocore-workdocs-2.5.4/types_aiobotocore_workdocs/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 01:22:36.000000 types-aiobotocore-workdocs-2.5.4/types_aiobotocore_workdocs/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    50590 2023-08-08 01:22:41.000000 types-aiobotocore-workdocs-2.5.4/types_aiobotocore_workdocs/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    50499 2023-08-08 01:22:38.000000 types-aiobotocore-workdocs-2.5.4/types_aiobotocore_workdocs/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-08-08 01:22:36.000000 types-aiobotocore-workdocs-2.5.4/types_aiobotocore_workdocs/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:24:36.230804 types-aiobotocore-workdocs-2.5.4/types_aiobotocore_workdocs.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    14499 2023-08-08 01:24:36.000000 types-aiobotocore-workdocs-2.5.4/types_aiobotocore_workdocs.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      832 2023-08-08 01:24:36.000000 types-aiobotocore-workdocs-2.5.4/types_aiobotocore_workdocs.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 01:24:36.000000 types-aiobotocore-workdocs-2.5.4/types_aiobotocore_workdocs.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 01:24:36.000000 types-aiobotocore-workdocs-2.5.4/types_aiobotocore_workdocs.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-08 01:24:36.000000 types-aiobotocore-workdocs-2.5.4/types_aiobotocore_workdocs.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-08-08 01:24:36.000000 types-aiobotocore-workdocs-2.5.4/types_aiobotocore_workdocs.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-workdocs-2.5.2.post2/LICENSE` & `types-aiobotocore-workdocs-2.5.4/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-workdocs-2.5.2.post2/PKG-INFO` & `types-aiobotocore-workdocs-2.5.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-workdocs
-Version: 2.5.2.post2
-Summary: Type annotations for aiobotocore.WorkDocs 2.5.2 service generated with mypy-boto3-builder 7.17.2
+Version: 2.5.4
+Summary: Type annotations for aiobotocore.WorkDocs 2.5.4 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_workdocs/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-workdocs.svg?color=blue)](https://pypi.org/project/types-aiobotocore-workdocs)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_workdocs/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-workdocs)](https://pepy.tech/project/types-aiobotocore-workdocs)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.WorkDocs 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workdocs.html#WorkDocs)
+[aiobotocore.WorkDocs 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workdocs.html#WorkDocs)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-workdocs-2.5.2.post2/README.md` & `types-aiobotocore-workdocs-2.5.4/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-workdocs.svg?color=blue)](https://pypi.org/project/types-aiobotocore-workdocs)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_workdocs/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-workdocs)](https://pepy.tech/project/types-aiobotocore-workdocs)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.WorkDocs 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workdocs.html#WorkDocs)
+[aiobotocore.WorkDocs 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workdocs.html#WorkDocs)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-workdocs-2.5.2.post2/setup.py` & `types-aiobotocore-workdocs-2.5.4/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-workdocs",
-    version="2.5.2.post2",
+    version="2.5.4",
     packages=["types_aiobotocore_workdocs"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.WorkDocs 2.5.2 service generated with mypy-boto3-builder"
+        "Type annotations for aiobotocore.WorkDocs 2.5.4 service generated with mypy-boto3-builder"
         " 7.17.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
```

### Comparing `types-aiobotocore-workdocs-2.5.2.post2/types_aiobotocore_workdocs/__init__.py` & `types-aiobotocore-workdocs-2.5.4/types_aiobotocore_workdocs/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-workdocs-2.5.2.post2/types_aiobotocore_workdocs/__init__.pyi` & `types-aiobotocore-workdocs-2.5.4/types_aiobotocore_workdocs/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-workdocs-2.5.2.post2/types_aiobotocore_workdocs/__main__.py` & `types-aiobotocore-workdocs-2.5.4/types_aiobotocore_workdocs/__main__.py`

 * *Files 15% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.WorkDocs 2.5.2\nVersion:         2.5.2.post2\nBuilder"
-        " version: 7.17.2\nDocs:           "
+        "Type annotations for aiobotocore.WorkDocs 2.5.4\nVersion:         2.5.4\nBuilder version:"
+        " 7.17.2\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_workdocs//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workdocs.html#WorkDocs\nOther"
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

### Comparing `types-aiobotocore-workdocs-2.5.2.post2/types_aiobotocore_workdocs/client.py` & `types-aiobotocore-workdocs-2.5.4/types_aiobotocore_workdocs/client.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-workdocs-2.5.2.post2/types_aiobotocore_workdocs/client.pyi` & `types-aiobotocore-workdocs-2.5.4/types_aiobotocore_workdocs/client.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-workdocs-2.5.2.post2/types_aiobotocore_workdocs/literals.py` & `types-aiobotocore-workdocs-2.5.4/types_aiobotocore_workdocs/literals.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-workdocs-2.5.2.post2/types_aiobotocore_workdocs/literals.pyi` & `types-aiobotocore-workdocs-2.5.4/types_aiobotocore_workdocs/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-workdocs-2.5.2.post2/types_aiobotocore_workdocs/paginator.py` & `types-aiobotocore-workdocs-2.5.4/types_aiobotocore_workdocs/paginator.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-workdocs-2.5.2.post2/types_aiobotocore_workdocs/paginator.pyi` & `types-aiobotocore-workdocs-2.5.4/types_aiobotocore_workdocs/paginator.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-workdocs-2.5.2.post2/types_aiobotocore_workdocs/type_defs.py` & `types-aiobotocore-workdocs-2.5.4/types_aiobotocore_workdocs/type_defs.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-workdocs-2.5.2.post2/types_aiobotocore_workdocs/type_defs.pyi` & `types-aiobotocore-workdocs-2.5.4/types_aiobotocore_workdocs/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-workdocs-2.5.2.post2/types_aiobotocore_workdocs.egg-info/PKG-INFO` & `types-aiobotocore-workdocs-2.5.4/types_aiobotocore_workdocs.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-workdocs
-Version: 2.5.2.post2
-Summary: Type annotations for aiobotocore.WorkDocs 2.5.2 service generated with mypy-boto3-builder 7.17.2
+Version: 2.5.4
+Summary: Type annotations for aiobotocore.WorkDocs 2.5.4 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_workdocs/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-workdocs.svg?color=blue)](https://pypi.org/project/types-aiobotocore-workdocs)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_workdocs/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-workdocs)](https://pepy.tech/project/types-aiobotocore-workdocs)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.WorkDocs 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workdocs.html#WorkDocs)
+[aiobotocore.WorkDocs 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workdocs.html#WorkDocs)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-workdocs-2.5.2.post2/types_aiobotocore_workdocs.egg-info/SOURCES.txt` & `types-aiobotocore-workdocs-2.5.4/types_aiobotocore_workdocs.egg-info/SOURCES.txt`

 * *Files identical despite different names*


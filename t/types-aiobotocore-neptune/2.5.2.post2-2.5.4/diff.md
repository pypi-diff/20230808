# Comparing `tmp/types-aiobotocore-neptune-2.5.2.post2.tar.gz` & `tmp/types-aiobotocore-neptune-2.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-neptune-2.5.2.post2.tar", last modified: Fri Aug  4 13:59:19 2023, max compression
+gzip compressed data, was "types-aiobotocore-neptune-2.5.4.tar", last modified: Tue Aug  8 01:24:09 2023, max compression
```

## Comparing `types-aiobotocore-neptune-2.5.2.post2.tar` & `types-aiobotocore-neptune-2.5.4.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:19.306643 types-aiobotocore-neptune-2.5.2.post2/
--rw-r--r--   0 vlad      (1000) vlad      (1000)     1070 2023-08-04 13:45:25.000000 types-aiobotocore-neptune-2.5.2.post2/LICENSE
--rw-r--r--   0 vlad      (1000) vlad      (1000)    16653 2023-08-04 13:59:19.306643 types-aiobotocore-neptune-2.5.2.post2/PKG-INFO
--rw-r--r--   0 vlad      (1000) vlad      (1000)    15135 2023-08-04 13:45:25.000000 types-aiobotocore-neptune-2.5.2.post2/README.md
--rw-r--r--   0 vlad      (1000) vlad      (1000)       38 2023-08-04 13:59:19.306643 types-aiobotocore-neptune-2.5.2.post2/setup.cfg
--rw-r--r--   0 vlad      (1000) vlad      (1000)     2072 2023-08-04 13:45:25.000000 types-aiobotocore-neptune-2.5.2.post2/setup.py
-drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:19.306643 types-aiobotocore-neptune-2.5.2.post2/types_aiobotocore_neptune/
--rw-r--r--   0 vlad      (1000) vlad      (1000)     5033 2023-08-04 13:45:25.000000 types-aiobotocore-neptune-2.5.2.post2/types_aiobotocore_neptune/__init__.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)     5032 2023-08-04 13:45:25.000000 types-aiobotocore-neptune-2.5.2.post2/types_aiobotocore_neptune/__init__.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)      943 2023-08-04 13:45:25.000000 types-aiobotocore-neptune-2.5.2.post2/types_aiobotocore_neptune/__main__.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)    70608 2023-08-04 13:45:27.000000 types-aiobotocore-neptune-2.5.2.post2/types_aiobotocore_neptune/client.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)    70512 2023-08-04 13:45:26.000000 types-aiobotocore-neptune-2.5.2.post2/types_aiobotocore_neptune/client.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)    11377 2023-08-04 13:45:28.000000 types-aiobotocore-neptune-2.5.2.post2/types_aiobotocore_neptune/literals.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)    11375 2023-08-04 13:45:28.000000 types-aiobotocore-neptune-2.5.2.post2/types_aiobotocore_neptune/literals.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)    22183 2023-08-04 13:45:28.000000 types-aiobotocore-neptune-2.5.2.post2/types_aiobotocore_neptune/paginator.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)    22165 2023-08-04 13:45:27.000000 types-aiobotocore-neptune-2.5.2.post2/types_aiobotocore_neptune/paginator.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:45:25.000000 types-aiobotocore-neptune-2.5.2.post2/types_aiobotocore_neptune/py.typed
--rw-r--r--   0 vlad      (1000) vlad      (1000)    84484 2023-08-04 13:45:30.000000 types-aiobotocore-neptune-2.5.2.post2/types_aiobotocore_neptune/type_defs.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)    84407 2023-08-04 13:45:29.000000 types-aiobotocore-neptune-2.5.2.post2/types_aiobotocore_neptune/type_defs.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)       65 2023-08-04 13:45:25.000000 types-aiobotocore-neptune-2.5.2.post2/types_aiobotocore_neptune/version.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)     2901 2023-08-04 13:45:28.000000 types-aiobotocore-neptune-2.5.2.post2/types_aiobotocore_neptune/waiter.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)     2899 2023-08-04 13:45:28.000000 types-aiobotocore-neptune-2.5.2.post2/types_aiobotocore_neptune/waiter.pyi
-drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:19.306643 types-aiobotocore-neptune-2.5.2.post2/types_aiobotocore_neptune.egg-info/
--rw-r--r--   0 vlad      (1000) vlad      (1000)    16653 2023-08-04 13:59:19.000000 types-aiobotocore-neptune-2.5.2.post2/types_aiobotocore_neptune.egg-info/PKG-INFO
--rw-r--r--   0 vlad      (1000) vlad      (1000)      886 2023-08-04 13:59:19.000000 types-aiobotocore-neptune-2.5.2.post2/types_aiobotocore_neptune.egg-info/SOURCES.txt
--rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:19.000000 types-aiobotocore-neptune-2.5.2.post2/types_aiobotocore_neptune.egg-info/dependency_links.txt
--rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:19.000000 types-aiobotocore-neptune-2.5.2.post2/types_aiobotocore_neptune.egg-info/not-zip-safe
--rw-r--r--   0 vlad      (1000) vlad      (1000)       52 2023-08-04 13:59:19.000000 types-aiobotocore-neptune-2.5.2.post2/types_aiobotocore_neptune.egg-info/requires.txt
--rw-r--r--   0 vlad      (1000) vlad      (1000)       26 2023-08-04 13:59:19.000000 types-aiobotocore-neptune-2.5.2.post2/types_aiobotocore_neptune.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:24:09.174740 types-aiobotocore-neptune-2.5.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-08 01:15:45.000000 types-aiobotocore-neptune-2.5.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    16647 2023-08-08 01:24:09.174740 types-aiobotocore-neptune-2.5.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    15135 2023-08-08 01:15:45.000000 types-aiobotocore-neptune-2.5.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-08 01:24:09.174740 types-aiobotocore-neptune-2.5.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2066 2023-08-08 01:15:45.000000 types-aiobotocore-neptune-2.5.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:24:09.174740 types-aiobotocore-neptune-2.5.4/types_aiobotocore_neptune/
+-rw-r--r--   0 runner    (1001) docker     (123)     5033 2023-08-08 01:15:45.000000 types-aiobotocore-neptune-2.5.4/types_aiobotocore_neptune/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5032 2023-08-08 01:15:45.000000 types-aiobotocore-neptune-2.5.4/types_aiobotocore_neptune/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      931 2023-08-08 01:15:45.000000 types-aiobotocore-neptune-2.5.4/types_aiobotocore_neptune/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    70608 2023-08-08 01:15:46.000000 types-aiobotocore-neptune-2.5.4/types_aiobotocore_neptune/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    70512 2023-08-08 01:15:46.000000 types-aiobotocore-neptune-2.5.4/types_aiobotocore_neptune/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    11377 2023-08-08 01:15:48.000000 types-aiobotocore-neptune-2.5.4/types_aiobotocore_neptune/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11375 2023-08-08 01:15:48.000000 types-aiobotocore-neptune-2.5.4/types_aiobotocore_neptune/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    22183 2023-08-08 01:15:48.000000 types-aiobotocore-neptune-2.5.4/types_aiobotocore_neptune/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22165 2023-08-08 01:15:46.000000 types-aiobotocore-neptune-2.5.4/types_aiobotocore_neptune/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 01:15:45.000000 types-aiobotocore-neptune-2.5.4/types_aiobotocore_neptune/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    84484 2023-08-08 01:15:50.000000 types-aiobotocore-neptune-2.5.4/types_aiobotocore_neptune/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    84407 2023-08-08 01:15:49.000000 types-aiobotocore-neptune-2.5.4/types_aiobotocore_neptune/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-08-08 01:15:45.000000 types-aiobotocore-neptune-2.5.4/types_aiobotocore_neptune/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2901 2023-08-08 01:15:48.000000 types-aiobotocore-neptune-2.5.4/types_aiobotocore_neptune/waiter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2899 2023-08-08 01:15:48.000000 types-aiobotocore-neptune-2.5.4/types_aiobotocore_neptune/waiter.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:24:09.174740 types-aiobotocore-neptune-2.5.4/types_aiobotocore_neptune.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    16647 2023-08-08 01:24:08.000000 types-aiobotocore-neptune-2.5.4/types_aiobotocore_neptune.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      886 2023-08-08 01:24:09.000000 types-aiobotocore-neptune-2.5.4/types_aiobotocore_neptune.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 01:24:08.000000 types-aiobotocore-neptune-2.5.4/types_aiobotocore_neptune.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 01:24:08.000000 types-aiobotocore-neptune-2.5.4/types_aiobotocore_neptune.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-08 01:24:08.000000 types-aiobotocore-neptune-2.5.4/types_aiobotocore_neptune.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-08-08 01:24:08.000000 types-aiobotocore-neptune-2.5.4/types_aiobotocore_neptune.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-neptune-2.5.2.post2/LICENSE` & `types-aiobotocore-neptune-2.5.4/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-neptune-2.5.2.post2/PKG-INFO` & `types-aiobotocore-neptune-2.5.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-neptune
-Version: 2.5.2.post2
-Summary: Type annotations for aiobotocore.Neptune 2.5.2 service generated with mypy-boto3-builder 7.17.2
+Version: 2.5.4
+Summary: Type annotations for aiobotocore.Neptune 2.5.4 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_neptune/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-neptune.svg?color=blue)](https://pypi.org/project/types-aiobotocore-neptune)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_neptune/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-neptune)](https://pepy.tech/project/types-aiobotocore-neptune)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.Neptune 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/neptune.html#Neptune)
+[aiobotocore.Neptune 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/neptune.html#Neptune)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-neptune-2.5.2.post2/README.md` & `types-aiobotocore-neptune-2.5.4/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-neptune.svg?color=blue)](https://pypi.org/project/types-aiobotocore-neptune)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_neptune/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-neptune)](https://pepy.tech/project/types-aiobotocore-neptune)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.Neptune 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/neptune.html#Neptune)
+[aiobotocore.Neptune 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/neptune.html#Neptune)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-neptune-2.5.2.post2/setup.py` & `types-aiobotocore-neptune-2.5.4/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-neptune",
-    version="2.5.2.post2",
+    version="2.5.4",
     packages=["types_aiobotocore_neptune"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.Neptune 2.5.2 service generated with mypy-boto3-builder"
+        "Type annotations for aiobotocore.Neptune 2.5.4 service generated with mypy-boto3-builder"
         " 7.17.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
```

### Comparing `types-aiobotocore-neptune-2.5.2.post2/types_aiobotocore_neptune/__init__.py` & `types-aiobotocore-neptune-2.5.4/types_aiobotocore_neptune/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-neptune-2.5.2.post2/types_aiobotocore_neptune/__init__.pyi` & `types-aiobotocore-neptune-2.5.4/types_aiobotocore_neptune/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-neptune-2.5.2.post2/types_aiobotocore_neptune/__main__.py` & `types-aiobotocore-neptune-2.5.4/types_aiobotocore_neptune/__main__.py`

 * *Files 15% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.Neptune 2.5.2\nVersion:         2.5.2.post2\nBuilder"
-        " version: 7.17.2\nDocs:           "
+        "Type annotations for aiobotocore.Neptune 2.5.4\nVersion:         2.5.4\nBuilder version:"
+        " 7.17.2\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_neptune//\nBoto3 docs:"
         "     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/neptune.html#Neptune\nOther"
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

### Comparing `types-aiobotocore-neptune-2.5.2.post2/types_aiobotocore_neptune/client.py` & `types-aiobotocore-neptune-2.5.4/types_aiobotocore_neptune/client.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-neptune-2.5.2.post2/types_aiobotocore_neptune/client.pyi` & `types-aiobotocore-neptune-2.5.4/types_aiobotocore_neptune/client.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-neptune-2.5.2.post2/types_aiobotocore_neptune/literals.py` & `types-aiobotocore-neptune-2.5.4/types_aiobotocore_neptune/literals.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-neptune-2.5.2.post2/types_aiobotocore_neptune/literals.pyi` & `types-aiobotocore-neptune-2.5.4/types_aiobotocore_neptune/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-neptune-2.5.2.post2/types_aiobotocore_neptune/paginator.py` & `types-aiobotocore-neptune-2.5.4/types_aiobotocore_neptune/paginator.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-neptune-2.5.2.post2/types_aiobotocore_neptune/paginator.pyi` & `types-aiobotocore-neptune-2.5.4/types_aiobotocore_neptune/paginator.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-neptune-2.5.2.post2/types_aiobotocore_neptune/type_defs.py` & `types-aiobotocore-neptune-2.5.4/types_aiobotocore_neptune/type_defs.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-neptune-2.5.2.post2/types_aiobotocore_neptune/type_defs.pyi` & `types-aiobotocore-neptune-2.5.4/types_aiobotocore_neptune/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-neptune-2.5.2.post2/types_aiobotocore_neptune/waiter.py` & `types-aiobotocore-neptune-2.5.4/types_aiobotocore_neptune/waiter.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-neptune-2.5.2.post2/types_aiobotocore_neptune/waiter.pyi` & `types-aiobotocore-neptune-2.5.4/types_aiobotocore_neptune/waiter.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-neptune-2.5.2.post2/types_aiobotocore_neptune.egg-info/PKG-INFO` & `types-aiobotocore-neptune-2.5.4/types_aiobotocore_neptune.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-neptune
-Version: 2.5.2.post2
-Summary: Type annotations for aiobotocore.Neptune 2.5.2 service generated with mypy-boto3-builder 7.17.2
+Version: 2.5.4
+Summary: Type annotations for aiobotocore.Neptune 2.5.4 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_neptune/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-neptune.svg?color=blue)](https://pypi.org/project/types-aiobotocore-neptune)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_neptune/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-neptune)](https://pepy.tech/project/types-aiobotocore-neptune)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.Neptune 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/neptune.html#Neptune)
+[aiobotocore.Neptune 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/neptune.html#Neptune)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-neptune-2.5.2.post2/types_aiobotocore_neptune.egg-info/SOURCES.txt` & `types-aiobotocore-neptune-2.5.4/types_aiobotocore_neptune.egg-info/SOURCES.txt`

 * *Files identical despite different names*


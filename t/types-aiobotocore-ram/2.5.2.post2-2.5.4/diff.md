# Comparing `tmp/types-aiobotocore-ram-2.5.2.post2.tar.gz` & `tmp/types-aiobotocore-ram-2.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-ram-2.5.2.post2.tar", last modified: Fri Aug  4 13:59:22 2023, max compression
+gzip compressed data, was "types-aiobotocore-ram-2.5.4.tar", last modified: Tue Aug  8 01:24:16 2023, max compression
```

## Comparing `types-aiobotocore-ram-2.5.2.post2.tar` & `types-aiobotocore-ram-2.5.4.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:22.076643 types-aiobotocore-ram-2.5.2.post2/
--rw-r--r--   0 vlad      (1000) vlad      (1000)     1070 2023-08-04 13:49:49.000000 types-aiobotocore-ram-2.5.2.post2/LICENSE
--rw-r--r--   0 vlad      (1000) vlad      (1000)    13594 2023-08-04 13:59:22.076643 types-aiobotocore-ram-2.5.2.post2/PKG-INFO
--rw-r--r--   0 vlad      (1000) vlad      (1000)    12092 2023-08-04 13:49:49.000000 types-aiobotocore-ram-2.5.2.post2/README.md
--rw-r--r--   0 vlad      (1000) vlad      (1000)       38 2023-08-04 13:59:22.076643 types-aiobotocore-ram-2.5.2.post2/setup.cfg
--rw-r--r--   0 vlad      (1000) vlad      (1000)     2020 2023-08-04 13:49:48.000000 types-aiobotocore-ram-2.5.2.post2/setup.py
-drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:22.076643 types-aiobotocore-ram-2.5.2.post2/types_aiobotocore_ram/
--rw-r--r--   0 vlad      (1000) vlad      (1000)     1805 2023-08-04 13:49:49.000000 types-aiobotocore-ram-2.5.2.post2/types_aiobotocore_ram/__init__.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)     1804 2023-08-04 13:49:49.000000 types-aiobotocore-ram-2.5.2.post2/types_aiobotocore_ram/__init__.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)      916 2023-08-04 13:49:49.000000 types-aiobotocore-ram-2.5.2.post2/types_aiobotocore_ram/__main__.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)    33737 2023-08-04 13:49:52.000000 types-aiobotocore-ram-2.5.2.post2/types_aiobotocore_ram/client.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)    33688 2023-08-04 13:49:52.000000 types-aiobotocore-ram-2.5.2.post2/types_aiobotocore_ram/client.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)    10754 2023-08-04 13:49:52.000000 types-aiobotocore-ram-2.5.2.post2/types_aiobotocore_ram/literals.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)    10752 2023-08-04 13:49:52.000000 types-aiobotocore-ram-2.5.2.post2/types_aiobotocore_ram/literals.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)     9025 2023-08-04 13:49:52.000000 types-aiobotocore-ram-2.5.2.post2/types_aiobotocore_ram/paginator.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)     9017 2023-08-04 13:49:52.000000 types-aiobotocore-ram-2.5.2.post2/types_aiobotocore_ram/paginator.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:49:49.000000 types-aiobotocore-ram-2.5.2.post2/types_aiobotocore_ram/py.typed
--rw-r--r--   0 vlad      (1000) vlad      (1000)    41115 2023-08-04 13:49:53.000000 types-aiobotocore-ram-2.5.2.post2/types_aiobotocore_ram/type_defs.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)    41050 2023-08-04 13:49:53.000000 types-aiobotocore-ram-2.5.2.post2/types_aiobotocore_ram/type_defs.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)       65 2023-08-04 13:49:49.000000 types-aiobotocore-ram-2.5.2.post2/types_aiobotocore_ram/version.py
-drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:22.076643 types-aiobotocore-ram-2.5.2.post2/types_aiobotocore_ram.egg-info/
--rw-r--r--   0 vlad      (1000) vlad      (1000)    13594 2023-08-04 13:59:21.000000 types-aiobotocore-ram-2.5.2.post2/types_aiobotocore_ram.egg-info/PKG-INFO
--rw-r--r--   0 vlad      (1000) vlad      (1000)      737 2023-08-04 13:59:22.000000 types-aiobotocore-ram-2.5.2.post2/types_aiobotocore_ram.egg-info/SOURCES.txt
--rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:21.000000 types-aiobotocore-ram-2.5.2.post2/types_aiobotocore_ram.egg-info/dependency_links.txt
--rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:21.000000 types-aiobotocore-ram-2.5.2.post2/types_aiobotocore_ram.egg-info/not-zip-safe
--rw-r--r--   0 vlad      (1000) vlad      (1000)       52 2023-08-04 13:59:21.000000 types-aiobotocore-ram-2.5.2.post2/types_aiobotocore_ram.egg-info/requires.txt
--rw-r--r--   0 vlad      (1000) vlad      (1000)       22 2023-08-04 13:59:21.000000 types-aiobotocore-ram-2.5.2.post2/types_aiobotocore_ram.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:24:16.242755 types-aiobotocore-ram-2.5.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-08 01:18:49.000000 types-aiobotocore-ram-2.5.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    13588 2023-08-08 01:24:16.242755 types-aiobotocore-ram-2.5.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    12092 2023-08-08 01:18:49.000000 types-aiobotocore-ram-2.5.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-08 01:24:16.242755 types-aiobotocore-ram-2.5.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2014 2023-08-08 01:18:49.000000 types-aiobotocore-ram-2.5.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:24:16.242755 types-aiobotocore-ram-2.5.4/types_aiobotocore_ram/
+-rw-r--r--   0 runner    (1001) docker     (123)     1805 2023-08-08 01:18:49.000000 types-aiobotocore-ram-2.5.4/types_aiobotocore_ram/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1804 2023-08-08 01:18:49.000000 types-aiobotocore-ram-2.5.4/types_aiobotocore_ram/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      904 2023-08-08 01:18:49.000000 types-aiobotocore-ram-2.5.4/types_aiobotocore_ram/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33737 2023-08-08 01:18:49.000000 types-aiobotocore-ram-2.5.4/types_aiobotocore_ram/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33688 2023-08-08 01:18:49.000000 types-aiobotocore-ram-2.5.4/types_aiobotocore_ram/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    10754 2023-08-08 01:18:49.000000 types-aiobotocore-ram-2.5.4/types_aiobotocore_ram/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10752 2023-08-08 01:18:49.000000 types-aiobotocore-ram-2.5.4/types_aiobotocore_ram/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9025 2023-08-08 01:18:49.000000 types-aiobotocore-ram-2.5.4/types_aiobotocore_ram/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9017 2023-08-08 01:18:49.000000 types-aiobotocore-ram-2.5.4/types_aiobotocore_ram/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 01:18:49.000000 types-aiobotocore-ram-2.5.4/types_aiobotocore_ram/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    41115 2023-08-08 01:18:50.000000 types-aiobotocore-ram-2.5.4/types_aiobotocore_ram/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41050 2023-08-08 01:18:50.000000 types-aiobotocore-ram-2.5.4/types_aiobotocore_ram/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-08-08 01:18:49.000000 types-aiobotocore-ram-2.5.4/types_aiobotocore_ram/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:24:16.242755 types-aiobotocore-ram-2.5.4/types_aiobotocore_ram.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    13588 2023-08-08 01:24:16.000000 types-aiobotocore-ram-2.5.4/types_aiobotocore_ram.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      737 2023-08-08 01:24:16.000000 types-aiobotocore-ram-2.5.4/types_aiobotocore_ram.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 01:24:16.000000 types-aiobotocore-ram-2.5.4/types_aiobotocore_ram.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 01:24:16.000000 types-aiobotocore-ram-2.5.4/types_aiobotocore_ram.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-08 01:24:16.000000 types-aiobotocore-ram-2.5.4/types_aiobotocore_ram.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-08-08 01:24:16.000000 types-aiobotocore-ram-2.5.4/types_aiobotocore_ram.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-ram-2.5.2.post2/LICENSE` & `types-aiobotocore-ram-2.5.4/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-ram-2.5.2.post2/PKG-INFO` & `types-aiobotocore-ram-2.5.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-ram
-Version: 2.5.2.post2
-Summary: Type annotations for aiobotocore.RAM 2.5.2 service generated with mypy-boto3-builder 7.17.2
+Version: 2.5.4
+Summary: Type annotations for aiobotocore.RAM 2.5.4 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ram/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-ram.svg?color=blue)](https://pypi.org/project/types-aiobotocore-ram)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ram/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-ram)](https://pepy.tech/project/types-aiobotocore-ram)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.RAM 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ram.html#RAM)
+[aiobotocore.RAM 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ram.html#RAM)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-ram-2.5.2.post2/README.md` & `types-aiobotocore-ram-2.5.4/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-ram.svg?color=blue)](https://pypi.org/project/types-aiobotocore-ram)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ram/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-ram)](https://pepy.tech/project/types-aiobotocore-ram)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.RAM 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ram.html#RAM)
+[aiobotocore.RAM 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ram.html#RAM)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-ram-2.5.2.post2/setup.py` & `types-aiobotocore-ram-2.5.4/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-ram",
-    version="2.5.2.post2",
+    version="2.5.4",
     packages=["types_aiobotocore_ram"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.RAM 2.5.2 service generated with mypy-boto3-builder"
+        "Type annotations for aiobotocore.RAM 2.5.4 service generated with mypy-boto3-builder"
         " 7.17.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
```

### Comparing `types-aiobotocore-ram-2.5.2.post2/types_aiobotocore_ram/__init__.py` & `types-aiobotocore-ram-2.5.4/types_aiobotocore_ram/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-ram-2.5.2.post2/types_aiobotocore_ram/__init__.pyi` & `types-aiobotocore-ram-2.5.4/types_aiobotocore_ram/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-ram-2.5.2.post2/types_aiobotocore_ram/__main__.py` & `types-aiobotocore-ram-2.5.4/types_aiobotocore_ram/__main__.py`

 * *Files 7% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.RAM 2.5.2\nVersion:         2.5.2.post2\nBuilder version:"
+        "Type annotations for aiobotocore.RAM 2.5.4\nVersion:         2.5.4\nBuilder version:"
         " 7.17.2\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ram//\nBoto3 docs:    "
         "  https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ram.html#RAM\nOther"
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

### Comparing `types-aiobotocore-ram-2.5.2.post2/types_aiobotocore_ram/client.py` & `types-aiobotocore-ram-2.5.4/types_aiobotocore_ram/client.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-ram-2.5.2.post2/types_aiobotocore_ram/client.pyi` & `types-aiobotocore-ram-2.5.4/types_aiobotocore_ram/client.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-ram-2.5.2.post2/types_aiobotocore_ram/literals.py` & `types-aiobotocore-ram-2.5.4/types_aiobotocore_ram/literals.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-ram-2.5.2.post2/types_aiobotocore_ram/literals.pyi` & `types-aiobotocore-ram-2.5.4/types_aiobotocore_ram/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-ram-2.5.2.post2/types_aiobotocore_ram/paginator.py` & `types-aiobotocore-ram-2.5.4/types_aiobotocore_ram/paginator.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-ram-2.5.2.post2/types_aiobotocore_ram/paginator.pyi` & `types-aiobotocore-ram-2.5.4/types_aiobotocore_ram/paginator.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-ram-2.5.2.post2/types_aiobotocore_ram/type_defs.py` & `types-aiobotocore-ram-2.5.4/types_aiobotocore_ram/type_defs.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-ram-2.5.2.post2/types_aiobotocore_ram/type_defs.pyi` & `types-aiobotocore-ram-2.5.4/types_aiobotocore_ram/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-ram-2.5.2.post2/types_aiobotocore_ram.egg-info/PKG-INFO` & `types-aiobotocore-ram-2.5.4/types_aiobotocore_ram.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-ram
-Version: 2.5.2.post2
-Summary: Type annotations for aiobotocore.RAM 2.5.2 service generated with mypy-boto3-builder 7.17.2
+Version: 2.5.4
+Summary: Type annotations for aiobotocore.RAM 2.5.4 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ram/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-ram.svg?color=blue)](https://pypi.org/project/types-aiobotocore-ram)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ram/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-ram)](https://pepy.tech/project/types-aiobotocore-ram)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.RAM 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ram.html#RAM)
+[aiobotocore.RAM 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ram.html#RAM)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-ram-2.5.2.post2/types_aiobotocore_ram.egg-info/SOURCES.txt` & `types-aiobotocore-ram-2.5.4/types_aiobotocore_ram.egg-info/SOURCES.txt`

 * *Files identical despite different names*


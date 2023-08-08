# Comparing `tmp/types-aiobotocore-support-2.5.2.post2.tar.gz` & `tmp/types-aiobotocore-support-2.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-support-2.5.2.post2.tar", last modified: Fri Aug  4 13:59:28 2023, max compression
+gzip compressed data, was "types-aiobotocore-support-2.5.4.tar", last modified: Tue Aug  8 01:24:31 2023, max compression
```

## Comparing `types-aiobotocore-support-2.5.2.post2.tar` & `types-aiobotocore-support-2.5.4.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:28.406643 types-aiobotocore-support-2.5.2.post2/
--rw-r--r--   0 vlad      (1000) vlad      (1000)     1070 2023-08-04 13:54:48.000000 types-aiobotocore-support-2.5.2.post2/LICENSE
--rw-r--r--   0 vlad      (1000) vlad      (1000)    13096 2023-08-04 13:59:28.406643 types-aiobotocore-support-2.5.2.post2/PKG-INFO
--rw-r--r--   0 vlad      (1000) vlad      (1000)    11578 2023-08-04 13:54:48.000000 types-aiobotocore-support-2.5.2.post2/README.md
--rw-r--r--   0 vlad      (1000) vlad      (1000)       38 2023-08-04 13:59:28.406643 types-aiobotocore-support-2.5.2.post2/setup.cfg
--rw-r--r--   0 vlad      (1000) vlad      (1000)     2072 2023-08-04 13:54:48.000000 types-aiobotocore-support-2.5.2.post2/setup.py
-drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:28.396643 types-aiobotocore-support-2.5.2.post2/types_aiobotocore_support/
--rw-r--r--   0 vlad      (1000) vlad      (1000)      871 2023-08-04 13:54:48.000000 types-aiobotocore-support-2.5.2.post2/types_aiobotocore_support/__init__.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)      870 2023-08-04 13:54:48.000000 types-aiobotocore-support-2.5.2.post2/types_aiobotocore_support/__init__.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)      943 2023-08-04 13:54:48.000000 types-aiobotocore-support-2.5.2.post2/types_aiobotocore_support/__main__.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)    16246 2023-08-04 13:54:48.000000 types-aiobotocore-support-2.5.2.post2/types_aiobotocore_support/client.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)    16219 2023-08-04 13:54:48.000000 types-aiobotocore-support-2.5.2.post2/types_aiobotocore_support/client.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)     7933 2023-08-04 13:54:48.000000 types-aiobotocore-support-2.5.2.post2/types_aiobotocore_support/literals.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)     7931 2023-08-04 13:54:48.000000 types-aiobotocore-support-2.5.2.post2/types_aiobotocore_support/literals.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)     3499 2023-08-04 13:54:48.000000 types-aiobotocore-support-2.5.2.post2/types_aiobotocore_support/paginator.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)     3495 2023-08-04 13:54:48.000000 types-aiobotocore-support-2.5.2.post2/types_aiobotocore_support/paginator.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:54:48.000000 types-aiobotocore-support-2.5.2.post2/types_aiobotocore_support/py.typed
--rw-r--r--   0 vlad      (1000) vlad      (1000)    18653 2023-08-04 13:54:49.000000 types-aiobotocore-support-2.5.2.post2/types_aiobotocore_support/type_defs.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)    18636 2023-08-04 13:54:48.000000 types-aiobotocore-support-2.5.2.post2/types_aiobotocore_support/type_defs.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)       65 2023-08-04 13:54:48.000000 types-aiobotocore-support-2.5.2.post2/types_aiobotocore_support/version.py
-drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:28.406643 types-aiobotocore-support-2.5.2.post2/types_aiobotocore_support.egg-info/
--rw-r--r--   0 vlad      (1000) vlad      (1000)    13096 2023-08-04 13:59:28.000000 types-aiobotocore-support-2.5.2.post2/types_aiobotocore_support.egg-info/PKG-INFO
--rw-r--r--   0 vlad      (1000) vlad      (1000)      813 2023-08-04 13:59:28.000000 types-aiobotocore-support-2.5.2.post2/types_aiobotocore_support.egg-info/SOURCES.txt
--rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:28.000000 types-aiobotocore-support-2.5.2.post2/types_aiobotocore_support.egg-info/dependency_links.txt
--rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:28.000000 types-aiobotocore-support-2.5.2.post2/types_aiobotocore_support.egg-info/not-zip-safe
--rw-r--r--   0 vlad      (1000) vlad      (1000)       52 2023-08-04 13:59:28.000000 types-aiobotocore-support-2.5.2.post2/types_aiobotocore_support.egg-info/requires.txt
--rw-r--r--   0 vlad      (1000) vlad      (1000)       26 2023-08-04 13:59:28.000000 types-aiobotocore-support-2.5.2.post2/types_aiobotocore_support.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:24:31.918794 types-aiobotocore-support-2.5.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-08 01:21:49.000000 types-aiobotocore-support-2.5.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    13090 2023-08-08 01:24:31.918794 types-aiobotocore-support-2.5.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    11578 2023-08-08 01:21:49.000000 types-aiobotocore-support-2.5.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-08 01:24:31.918794 types-aiobotocore-support-2.5.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2066 2023-08-08 01:21:49.000000 types-aiobotocore-support-2.5.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:24:31.918794 types-aiobotocore-support-2.5.4/types_aiobotocore_support/
+-rw-r--r--   0 runner    (1001) docker     (123)      871 2023-08-08 01:21:49.000000 types-aiobotocore-support-2.5.4/types_aiobotocore_support/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      870 2023-08-08 01:21:49.000000 types-aiobotocore-support-2.5.4/types_aiobotocore_support/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      931 2023-08-08 01:21:49.000000 types-aiobotocore-support-2.5.4/types_aiobotocore_support/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16246 2023-08-08 01:21:50.000000 types-aiobotocore-support-2.5.4/types_aiobotocore_support/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16219 2023-08-08 01:21:49.000000 types-aiobotocore-support-2.5.4/types_aiobotocore_support/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     7933 2023-08-08 01:21:50.000000 types-aiobotocore-support-2.5.4/types_aiobotocore_support/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7931 2023-08-08 01:21:50.000000 types-aiobotocore-support-2.5.4/types_aiobotocore_support/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     3499 2023-08-08 01:21:50.000000 types-aiobotocore-support-2.5.4/types_aiobotocore_support/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3495 2023-08-08 01:21:50.000000 types-aiobotocore-support-2.5.4/types_aiobotocore_support/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 01:21:49.000000 types-aiobotocore-support-2.5.4/types_aiobotocore_support/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    18653 2023-08-08 01:21:53.000000 types-aiobotocore-support-2.5.4/types_aiobotocore_support/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18636 2023-08-08 01:21:50.000000 types-aiobotocore-support-2.5.4/types_aiobotocore_support/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-08-08 01:21:49.000000 types-aiobotocore-support-2.5.4/types_aiobotocore_support/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:24:31.918794 types-aiobotocore-support-2.5.4/types_aiobotocore_support.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    13090 2023-08-08 01:24:31.000000 types-aiobotocore-support-2.5.4/types_aiobotocore_support.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      813 2023-08-08 01:24:31.000000 types-aiobotocore-support-2.5.4/types_aiobotocore_support.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 01:24:31.000000 types-aiobotocore-support-2.5.4/types_aiobotocore_support.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 01:24:31.000000 types-aiobotocore-support-2.5.4/types_aiobotocore_support.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-08 01:24:31.000000 types-aiobotocore-support-2.5.4/types_aiobotocore_support.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-08-08 01:24:31.000000 types-aiobotocore-support-2.5.4/types_aiobotocore_support.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-support-2.5.2.post2/LICENSE` & `types-aiobotocore-support-2.5.4/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-support-2.5.2.post2/PKG-INFO` & `types-aiobotocore-support-2.5.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-support
-Version: 2.5.2.post2
-Summary: Type annotations for aiobotocore.Support 2.5.2 service generated with mypy-boto3-builder 7.17.2
+Version: 2.5.4
+Summary: Type annotations for aiobotocore.Support 2.5.4 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_support/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-support.svg?color=blue)](https://pypi.org/project/types-aiobotocore-support)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_support/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-support)](https://pepy.tech/project/types-aiobotocore-support)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.Support 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/support.html#Support)
+[aiobotocore.Support 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/support.html#Support)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-support-2.5.2.post2/README.md` & `types-aiobotocore-support-2.5.4/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-support.svg?color=blue)](https://pypi.org/project/types-aiobotocore-support)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_support/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-support)](https://pepy.tech/project/types-aiobotocore-support)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.Support 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/support.html#Support)
+[aiobotocore.Support 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/support.html#Support)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-support-2.5.2.post2/setup.py` & `types-aiobotocore-support-2.5.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-support",
-    version="2.5.2.post2",
+    version="2.5.4",
     packages=["types_aiobotocore_support"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.Support 2.5.2 service generated with mypy-boto3-builder"
+        "Type annotations for aiobotocore.Support 2.5.4 service generated with mypy-boto3-builder"
         " 7.17.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
```

### Comparing `types-aiobotocore-support-2.5.2.post2/types_aiobotocore_support/__init__.py` & `types-aiobotocore-support-2.5.4/types_aiobotocore_support/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-support-2.5.2.post2/types_aiobotocore_support/__init__.pyi` & `types-aiobotocore-support-2.5.4/types_aiobotocore_support/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-support-2.5.2.post2/types_aiobotocore_support/__main__.py` & `types-aiobotocore-support-2.5.4/types_aiobotocore_support/__main__.py`

 * *Files 15% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.Support 2.5.2\nVersion:         2.5.2.post2\nBuilder"
-        " version: 7.17.2\nDocs:           "
+        "Type annotations for aiobotocore.Support 2.5.4\nVersion:         2.5.4\nBuilder version:"
+        " 7.17.2\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_support//\nBoto3 docs:"
         "     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/support.html#Support\nOther"
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

### Comparing `types-aiobotocore-support-2.5.2.post2/types_aiobotocore_support/client.py` & `types-aiobotocore-support-2.5.4/types_aiobotocore_support/client.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-support-2.5.2.post2/types_aiobotocore_support/client.pyi` & `types-aiobotocore-support-2.5.4/types_aiobotocore_support/client.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-support-2.5.2.post2/types_aiobotocore_support/literals.py` & `types-aiobotocore-support-2.5.4/types_aiobotocore_support/literals.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-support-2.5.2.post2/types_aiobotocore_support/literals.pyi` & `types-aiobotocore-support-2.5.4/types_aiobotocore_support/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-support-2.5.2.post2/types_aiobotocore_support/paginator.py` & `types-aiobotocore-support-2.5.4/types_aiobotocore_support/paginator.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-support-2.5.2.post2/types_aiobotocore_support/paginator.pyi` & `types-aiobotocore-support-2.5.4/types_aiobotocore_support/paginator.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-support-2.5.2.post2/types_aiobotocore_support/type_defs.py` & `types-aiobotocore-support-2.5.4/types_aiobotocore_support/type_defs.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-support-2.5.2.post2/types_aiobotocore_support/type_defs.pyi` & `types-aiobotocore-support-2.5.4/types_aiobotocore_support/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-support-2.5.2.post2/types_aiobotocore_support.egg-info/PKG-INFO` & `types-aiobotocore-support-2.5.4/types_aiobotocore_support.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-support
-Version: 2.5.2.post2
-Summary: Type annotations for aiobotocore.Support 2.5.2 service generated with mypy-boto3-builder 7.17.2
+Version: 2.5.4
+Summary: Type annotations for aiobotocore.Support 2.5.4 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_support/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-support.svg?color=blue)](https://pypi.org/project/types-aiobotocore-support)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_support/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-support)](https://pepy.tech/project/types-aiobotocore-support)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.Support 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/support.html#Support)
+[aiobotocore.Support 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/support.html#Support)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-support-2.5.2.post2/types_aiobotocore_support.egg-info/SOURCES.txt` & `types-aiobotocore-support-2.5.4/types_aiobotocore_support.egg-info/SOURCES.txt`

 * *Files identical despite different names*


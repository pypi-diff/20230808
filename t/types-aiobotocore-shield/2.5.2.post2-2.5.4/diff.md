# Comparing `tmp/types-aiobotocore-shield-2.5.2.post2.tar.gz` & `tmp/types-aiobotocore-shield-2.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-shield-2.5.2.post2.tar", last modified: Fri Aug  4 13:59:26 2023, max compression
+gzip compressed data, was "types-aiobotocore-shield-2.5.4.tar", last modified: Tue Aug  8 01:24:27 2023, max compression
```

## Comparing `types-aiobotocore-shield-2.5.2.post2.tar` & `types-aiobotocore-shield-2.5.4.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:26.636643 types-aiobotocore-shield-2.5.2.post2/
--rw-r--r--   0 vlad      (1000) vlad      (1000)     1070 2023-08-04 13:53:37.000000 types-aiobotocore-shield-2.5.2.post2/LICENSE
--rw-r--r--   0 vlad      (1000) vlad      (1000)    13004 2023-08-04 13:59:26.636643 types-aiobotocore-shield-2.5.2.post2/PKG-INFO
--rw-r--r--   0 vlad      (1000) vlad      (1000)    11490 2023-08-04 13:53:37.000000 types-aiobotocore-shield-2.5.2.post2/README.md
--rw-r--r--   0 vlad      (1000) vlad      (1000)       38 2023-08-04 13:59:26.636643 types-aiobotocore-shield-2.5.2.post2/setup.cfg
--rw-r--r--   0 vlad      (1000) vlad      (1000)     2065 2023-08-04 13:53:37.000000 types-aiobotocore-shield-2.5.2.post2/setup.py
-drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:26.636643 types-aiobotocore-shield-2.5.2.post2/types_aiobotocore_shield/
--rw-r--r--   0 vlad      (1000) vlad      (1000)      809 2023-08-04 13:53:37.000000 types-aiobotocore-shield-2.5.2.post2/types_aiobotocore_shield/__init__.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)      808 2023-08-04 13:53:37.000000 types-aiobotocore-shield-2.5.2.post2/types_aiobotocore_shield/__init__.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)      928 2023-08-04 13:53:37.000000 types-aiobotocore-shield-2.5.2.post2/types_aiobotocore_shield/__main__.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)    27481 2023-08-04 13:53:38.000000 types-aiobotocore-shield-2.5.2.post2/types_aiobotocore_shield/client.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)    27434 2023-08-04 13:53:37.000000 types-aiobotocore-shield-2.5.2.post2/types_aiobotocore_shield/client.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)     9265 2023-08-04 13:53:38.000000 types-aiobotocore-shield-2.5.2.post2/types_aiobotocore_shield/literals.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)     9263 2023-08-04 13:53:38.000000 types-aiobotocore-shield-2.5.2.post2/types_aiobotocore_shield/literals.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)     3299 2023-08-04 13:53:38.000000 types-aiobotocore-shield-2.5.2.post2/types_aiobotocore_shield/paginator.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)     3295 2023-08-04 13:53:38.000000 types-aiobotocore-shield-2.5.2.post2/types_aiobotocore_shield/paginator.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:53:37.000000 types-aiobotocore-shield-2.5.2.post2/types_aiobotocore_shield/py.typed
--rw-r--r--   0 vlad      (1000) vlad      (1000)    22173 2023-08-04 13:53:42.000000 types-aiobotocore-shield-2.5.2.post2/types_aiobotocore_shield/type_defs.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)    22154 2023-08-04 13:53:38.000000 types-aiobotocore-shield-2.5.2.post2/types_aiobotocore_shield/type_defs.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)       65 2023-08-04 13:53:37.000000 types-aiobotocore-shield-2.5.2.post2/types_aiobotocore_shield/version.py
-drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:26.636643 types-aiobotocore-shield-2.5.2.post2/types_aiobotocore_shield.egg-info/
--rw-r--r--   0 vlad      (1000) vlad      (1000)    13004 2023-08-04 13:59:26.000000 types-aiobotocore-shield-2.5.2.post2/types_aiobotocore_shield.egg-info/PKG-INFO
--rw-r--r--   0 vlad      (1000) vlad      (1000)      794 2023-08-04 13:59:26.000000 types-aiobotocore-shield-2.5.2.post2/types_aiobotocore_shield.egg-info/SOURCES.txt
--rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:26.000000 types-aiobotocore-shield-2.5.2.post2/types_aiobotocore_shield.egg-info/dependency_links.txt
--rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:26.000000 types-aiobotocore-shield-2.5.2.post2/types_aiobotocore_shield.egg-info/not-zip-safe
--rw-r--r--   0 vlad      (1000) vlad      (1000)       52 2023-08-04 13:59:26.000000 types-aiobotocore-shield-2.5.2.post2/types_aiobotocore_shield.egg-info/requires.txt
--rw-r--r--   0 vlad      (1000) vlad      (1000)       25 2023-08-04 13:59:26.000000 types-aiobotocore-shield-2.5.2.post2/types_aiobotocore_shield.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:24:27.230783 types-aiobotocore-shield-2.5.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-08 01:21:10.000000 types-aiobotocore-shield-2.5.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    12998 2023-08-08 01:24:27.230783 types-aiobotocore-shield-2.5.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    11490 2023-08-08 01:21:10.000000 types-aiobotocore-shield-2.5.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-08 01:24:27.230783 types-aiobotocore-shield-2.5.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2059 2023-08-08 01:21:09.000000 types-aiobotocore-shield-2.5.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:24:27.230783 types-aiobotocore-shield-2.5.4/types_aiobotocore_shield/
+-rw-r--r--   0 runner    (1001) docker     (123)      809 2023-08-08 01:21:10.000000 types-aiobotocore-shield-2.5.4/types_aiobotocore_shield/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      808 2023-08-08 01:21:10.000000 types-aiobotocore-shield-2.5.4/types_aiobotocore_shield/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      916 2023-08-08 01:21:10.000000 types-aiobotocore-shield-2.5.4/types_aiobotocore_shield/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27481 2023-08-08 01:21:10.000000 types-aiobotocore-shield-2.5.4/types_aiobotocore_shield/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27434 2023-08-08 01:21:10.000000 types-aiobotocore-shield-2.5.4/types_aiobotocore_shield/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9265 2023-08-08 01:21:10.000000 types-aiobotocore-shield-2.5.4/types_aiobotocore_shield/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9263 2023-08-08 01:21:10.000000 types-aiobotocore-shield-2.5.4/types_aiobotocore_shield/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     3299 2023-08-08 01:21:10.000000 types-aiobotocore-shield-2.5.4/types_aiobotocore_shield/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3295 2023-08-08 01:21:10.000000 types-aiobotocore-shield-2.5.4/types_aiobotocore_shield/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 01:21:10.000000 types-aiobotocore-shield-2.5.4/types_aiobotocore_shield/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    22173 2023-08-08 01:21:10.000000 types-aiobotocore-shield-2.5.4/types_aiobotocore_shield/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22154 2023-08-08 01:21:10.000000 types-aiobotocore-shield-2.5.4/types_aiobotocore_shield/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-08-08 01:21:10.000000 types-aiobotocore-shield-2.5.4/types_aiobotocore_shield/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:24:27.230783 types-aiobotocore-shield-2.5.4/types_aiobotocore_shield.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    12998 2023-08-08 01:24:27.000000 types-aiobotocore-shield-2.5.4/types_aiobotocore_shield.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      794 2023-08-08 01:24:27.000000 types-aiobotocore-shield-2.5.4/types_aiobotocore_shield.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 01:24:27.000000 types-aiobotocore-shield-2.5.4/types_aiobotocore_shield.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 01:24:27.000000 types-aiobotocore-shield-2.5.4/types_aiobotocore_shield.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-08 01:24:27.000000 types-aiobotocore-shield-2.5.4/types_aiobotocore_shield.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-08-08 01:24:27.000000 types-aiobotocore-shield-2.5.4/types_aiobotocore_shield.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-shield-2.5.2.post2/LICENSE` & `types-aiobotocore-shield-2.5.4/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-shield-2.5.2.post2/PKG-INFO` & `types-aiobotocore-shield-2.5.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-shield
-Version: 2.5.2.post2
-Summary: Type annotations for aiobotocore.Shield 2.5.2 service generated with mypy-boto3-builder 7.17.2
+Version: 2.5.4
+Summary: Type annotations for aiobotocore.Shield 2.5.4 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_shield/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-shield.svg?color=blue)](https://pypi.org/project/types-aiobotocore-shield)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_shield/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-shield)](https://pepy.tech/project/types-aiobotocore-shield)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.Shield 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/shield.html#Shield)
+[aiobotocore.Shield 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/shield.html#Shield)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-shield-2.5.2.post2/README.md` & `types-aiobotocore-shield-2.5.4/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-shield.svg?color=blue)](https://pypi.org/project/types-aiobotocore-shield)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_shield/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-shield)](https://pepy.tech/project/types-aiobotocore-shield)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.Shield 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/shield.html#Shield)
+[aiobotocore.Shield 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/shield.html#Shield)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-shield-2.5.2.post2/setup.py` & `types-aiobotocore-shield-2.5.4/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-shield",
-    version="2.5.2.post2",
+    version="2.5.4",
     packages=["types_aiobotocore_shield"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.Shield 2.5.2 service generated with mypy-boto3-builder"
+        "Type annotations for aiobotocore.Shield 2.5.4 service generated with mypy-boto3-builder"
         " 7.17.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
```

### Comparing `types-aiobotocore-shield-2.5.2.post2/types_aiobotocore_shield/__init__.py` & `types-aiobotocore-shield-2.5.4/types_aiobotocore_shield/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-shield-2.5.2.post2/types_aiobotocore_shield/__init__.pyi` & `types-aiobotocore-shield-2.5.4/types_aiobotocore_shield/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-shield-2.5.2.post2/types_aiobotocore_shield/__main__.py` & `types-aiobotocore-shield-2.5.4/types_aiobotocore_shield/__main__.py`

 * *Files 22% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.Shield 2.5.2\nVersion:         2.5.2.post2\nBuilder"
-        " version: 7.17.2\nDocs:           "
+        "Type annotations for aiobotocore.Shield 2.5.4\nVersion:         2.5.4\nBuilder version:"
+        " 7.17.2\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_shield//\nBoto3 docs: "
         "     https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/shield.html#Shield\nOther"
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

### Comparing `types-aiobotocore-shield-2.5.2.post2/types_aiobotocore_shield/client.py` & `types-aiobotocore-shield-2.5.4/types_aiobotocore_shield/client.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-shield-2.5.2.post2/types_aiobotocore_shield/client.pyi` & `types-aiobotocore-shield-2.5.4/types_aiobotocore_shield/client.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-shield-2.5.2.post2/types_aiobotocore_shield/literals.py` & `types-aiobotocore-shield-2.5.4/types_aiobotocore_shield/literals.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-shield-2.5.2.post2/types_aiobotocore_shield/literals.pyi` & `types-aiobotocore-shield-2.5.4/types_aiobotocore_shield/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-shield-2.5.2.post2/types_aiobotocore_shield/paginator.py` & `types-aiobotocore-shield-2.5.4/types_aiobotocore_shield/paginator.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-shield-2.5.2.post2/types_aiobotocore_shield/paginator.pyi` & `types-aiobotocore-shield-2.5.4/types_aiobotocore_shield/paginator.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-shield-2.5.2.post2/types_aiobotocore_shield/type_defs.py` & `types-aiobotocore-shield-2.5.4/types_aiobotocore_shield/type_defs.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-shield-2.5.2.post2/types_aiobotocore_shield/type_defs.pyi` & `types-aiobotocore-shield-2.5.4/types_aiobotocore_shield/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-shield-2.5.2.post2/types_aiobotocore_shield.egg-info/PKG-INFO` & `types-aiobotocore-shield-2.5.4/types_aiobotocore_shield.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-shield
-Version: 2.5.2.post2
-Summary: Type annotations for aiobotocore.Shield 2.5.2 service generated with mypy-boto3-builder 7.17.2
+Version: 2.5.4
+Summary: Type annotations for aiobotocore.Shield 2.5.4 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_shield/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-shield.svg?color=blue)](https://pypi.org/project/types-aiobotocore-shield)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_shield/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-shield)](https://pepy.tech/project/types-aiobotocore-shield)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.Shield 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/shield.html#Shield)
+[aiobotocore.Shield 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/shield.html#Shield)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-shield-2.5.2.post2/types_aiobotocore_shield.egg-info/SOURCES.txt` & `types-aiobotocore-shield-2.5.4/types_aiobotocore_shield.egg-info/SOURCES.txt`

 * *Files identical despite different names*


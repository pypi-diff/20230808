# Comparing `tmp/types-aiobotocore-internetmonitor-2.5.2.post2.tar.gz` & `tmp/types-aiobotocore-internetmonitor-2.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-internetmonitor-2.5.2.post2.tar", last modified: Fri Aug  4 13:59:11 2023, max compression
+gzip compressed data, was "types-aiobotocore-internetmonitor-2.5.4.tar", last modified: Tue Aug  8 01:23:50 2023, max compression
```

## Comparing `types-aiobotocore-internetmonitor-2.5.2.post2.tar` & `types-aiobotocore-internetmonitor-2.5.4.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:11.156643 types-aiobotocore-internetmonitor-2.5.2.post2/
--rw-r--r--   0 vlad      (1000) vlad      (1000)     1070 2023-08-04 13:40:26.000000 types-aiobotocore-internetmonitor-2.5.2.post2/LICENSE
--rw-r--r--   0 vlad      (1000) vlad      (1000)    13664 2023-08-04 13:59:11.156643 types-aiobotocore-internetmonitor-2.5.2.post2/PKG-INFO
--rw-r--r--   0 vlad      (1000) vlad      (1000)    12104 2023-08-04 13:40:26.000000 types-aiobotocore-internetmonitor-2.5.2.post2/README.md
--rw-r--r--   0 vlad      (1000) vlad      (1000)       38 2023-08-04 13:59:11.156643 types-aiobotocore-internetmonitor-2.5.2.post2/setup.cfg
--rw-r--r--   0 vlad      (1000) vlad      (1000)     2138 2023-08-04 13:40:26.000000 types-aiobotocore-internetmonitor-2.5.2.post2/setup.py
-drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:11.156643 types-aiobotocore-internetmonitor-2.5.2.post2/types_aiobotocore_internetmonitor/
--rw-r--r--   0 vlad      (1000) vlad      (1000)      964 2023-08-04 13:40:26.000000 types-aiobotocore-internetmonitor-2.5.2.post2/types_aiobotocore_internetmonitor/__init__.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)      963 2023-08-04 13:40:26.000000 types-aiobotocore-internetmonitor-2.5.2.post2/types_aiobotocore_internetmonitor/__init__.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)      995 2023-08-04 13:40:26.000000 types-aiobotocore-internetmonitor-2.5.2.post2/types_aiobotocore_internetmonitor/__main__.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)    12756 2023-08-04 13:40:27.000000 types-aiobotocore-internetmonitor-2.5.2.post2/types_aiobotocore_internetmonitor/client.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)    12735 2023-08-04 13:40:26.000000 types-aiobotocore-internetmonitor-2.5.2.post2/types_aiobotocore_internetmonitor/client.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)     9375 2023-08-04 13:40:27.000000 types-aiobotocore-internetmonitor-2.5.2.post2/types_aiobotocore_internetmonitor/literals.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)     9373 2023-08-04 13:40:27.000000 types-aiobotocore-internetmonitor-2.5.2.post2/types_aiobotocore_internetmonitor/literals.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)     3519 2023-08-04 13:40:27.000000 types-aiobotocore-internetmonitor-2.5.2.post2/types_aiobotocore_internetmonitor/paginator.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)     3515 2023-08-04 13:40:27.000000 types-aiobotocore-internetmonitor-2.5.2.post2/types_aiobotocore_internetmonitor/paginator.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:40:26.000000 types-aiobotocore-internetmonitor-2.5.2.post2/types_aiobotocore_internetmonitor/py.typed
--rw-r--r--   0 vlad      (1000) vlad      (1000)    13136 2023-08-04 13:40:27.000000 types-aiobotocore-internetmonitor-2.5.2.post2/types_aiobotocore_internetmonitor/type_defs.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)    13121 2023-08-04 13:40:27.000000 types-aiobotocore-internetmonitor-2.5.2.post2/types_aiobotocore_internetmonitor/type_defs.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)       65 2023-08-04 13:40:26.000000 types-aiobotocore-internetmonitor-2.5.2.post2/types_aiobotocore_internetmonitor/version.py
-drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:11.156643 types-aiobotocore-internetmonitor-2.5.2.post2/types_aiobotocore_internetmonitor.egg-info/
--rw-r--r--   0 vlad      (1000) vlad      (1000)    13664 2023-08-04 13:59:11.000000 types-aiobotocore-internetmonitor-2.5.2.post2/types_aiobotocore_internetmonitor.egg-info/PKG-INFO
--rw-r--r--   0 vlad      (1000) vlad      (1000)      965 2023-08-04 13:59:11.000000 types-aiobotocore-internetmonitor-2.5.2.post2/types_aiobotocore_internetmonitor.egg-info/SOURCES.txt
--rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:11.000000 types-aiobotocore-internetmonitor-2.5.2.post2/types_aiobotocore_internetmonitor.egg-info/dependency_links.txt
--rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:11.000000 types-aiobotocore-internetmonitor-2.5.2.post2/types_aiobotocore_internetmonitor.egg-info/not-zip-safe
--rw-r--r--   0 vlad      (1000) vlad      (1000)       52 2023-08-04 13:59:11.000000 types-aiobotocore-internetmonitor-2.5.2.post2/types_aiobotocore_internetmonitor.egg-info/requires.txt
--rw-r--r--   0 vlad      (1000) vlad      (1000)       34 2023-08-04 13:59:11.000000 types-aiobotocore-internetmonitor-2.5.2.post2/types_aiobotocore_internetmonitor.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:23:50.406734 types-aiobotocore-internetmonitor-2.5.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-08 01:12:35.000000 types-aiobotocore-internetmonitor-2.5.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    13658 2023-08-08 01:23:50.406734 types-aiobotocore-internetmonitor-2.5.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    12104 2023-08-08 01:12:35.000000 types-aiobotocore-internetmonitor-2.5.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-08 01:23:50.406734 types-aiobotocore-internetmonitor-2.5.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2132 2023-08-08 01:12:35.000000 types-aiobotocore-internetmonitor-2.5.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:23:50.402734 types-aiobotocore-internetmonitor-2.5.4/types_aiobotocore_internetmonitor/
+-rw-r--r--   0 runner    (1001) docker     (123)      964 2023-08-08 01:12:35.000000 types-aiobotocore-internetmonitor-2.5.4/types_aiobotocore_internetmonitor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      963 2023-08-08 01:12:35.000000 types-aiobotocore-internetmonitor-2.5.4/types_aiobotocore_internetmonitor/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      983 2023-08-08 01:12:35.000000 types-aiobotocore-internetmonitor-2.5.4/types_aiobotocore_internetmonitor/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12756 2023-08-08 01:12:35.000000 types-aiobotocore-internetmonitor-2.5.4/types_aiobotocore_internetmonitor/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12735 2023-08-08 01:12:35.000000 types-aiobotocore-internetmonitor-2.5.4/types_aiobotocore_internetmonitor/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9375 2023-08-08 01:12:35.000000 types-aiobotocore-internetmonitor-2.5.4/types_aiobotocore_internetmonitor/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9373 2023-08-08 01:12:35.000000 types-aiobotocore-internetmonitor-2.5.4/types_aiobotocore_internetmonitor/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     3519 2023-08-08 01:12:35.000000 types-aiobotocore-internetmonitor-2.5.4/types_aiobotocore_internetmonitor/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3515 2023-08-08 01:12:35.000000 types-aiobotocore-internetmonitor-2.5.4/types_aiobotocore_internetmonitor/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 01:12:35.000000 types-aiobotocore-internetmonitor-2.5.4/types_aiobotocore_internetmonitor/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    13136 2023-08-08 01:12:36.000000 types-aiobotocore-internetmonitor-2.5.4/types_aiobotocore_internetmonitor/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13121 2023-08-08 01:12:35.000000 types-aiobotocore-internetmonitor-2.5.4/types_aiobotocore_internetmonitor/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-08-08 01:12:35.000000 types-aiobotocore-internetmonitor-2.5.4/types_aiobotocore_internetmonitor/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:23:50.406734 types-aiobotocore-internetmonitor-2.5.4/types_aiobotocore_internetmonitor.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    13658 2023-08-08 01:23:50.000000 types-aiobotocore-internetmonitor-2.5.4/types_aiobotocore_internetmonitor.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      965 2023-08-08 01:23:50.000000 types-aiobotocore-internetmonitor-2.5.4/types_aiobotocore_internetmonitor.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 01:23:50.000000 types-aiobotocore-internetmonitor-2.5.4/types_aiobotocore_internetmonitor.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 01:23:50.000000 types-aiobotocore-internetmonitor-2.5.4/types_aiobotocore_internetmonitor.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-08 01:23:50.000000 types-aiobotocore-internetmonitor-2.5.4/types_aiobotocore_internetmonitor.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-08-08 01:23:50.000000 types-aiobotocore-internetmonitor-2.5.4/types_aiobotocore_internetmonitor.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-internetmonitor-2.5.2.post2/LICENSE` & `types-aiobotocore-internetmonitor-2.5.4/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-internetmonitor-2.5.2.post2/PKG-INFO` & `types-aiobotocore-internetmonitor-2.5.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-internetmonitor
-Version: 2.5.2.post2
-Summary: Type annotations for aiobotocore.CloudWatchInternetMonitor 2.5.2 service generated with mypy-boto3-builder 7.17.2
+Version: 2.5.4
+Summary: Type annotations for aiobotocore.CloudWatchInternetMonitor 2.5.4 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_internetmonitor/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-internetmonitor.svg?color=blue)](https://pypi.org/project/types-aiobotocore-internetmonitor)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_internetmonitor/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-internetmonitor)](https://pepy.tech/project/types-aiobotocore-internetmonitor)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.CloudWatchInternetMonitor 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/internetmonitor.html#CloudWatchInternetMonitor)
+[aiobotocore.CloudWatchInternetMonitor 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/internetmonitor.html#CloudWatchInternetMonitor)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-internetmonitor-2.5.2.post2/README.md` & `types-aiobotocore-internetmonitor-2.5.4/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-internetmonitor.svg?color=blue)](https://pypi.org/project/types-aiobotocore-internetmonitor)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_internetmonitor/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-internetmonitor)](https://pepy.tech/project/types-aiobotocore-internetmonitor)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.CloudWatchInternetMonitor 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/internetmonitor.html#CloudWatchInternetMonitor)
+[aiobotocore.CloudWatchInternetMonitor 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/internetmonitor.html#CloudWatchInternetMonitor)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-internetmonitor-2.5.2.post2/setup.py` & `types-aiobotocore-internetmonitor-2.5.4/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-internetmonitor",
-    version="2.5.2.post2",
+    version="2.5.4",
     packages=["types_aiobotocore_internetmonitor"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.CloudWatchInternetMonitor 2.5.2 service generated with"
+        "Type annotations for aiobotocore.CloudWatchInternetMonitor 2.5.4 service generated with"
         " mypy-boto3-builder 7.17.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
```

### Comparing `types-aiobotocore-internetmonitor-2.5.2.post2/types_aiobotocore_internetmonitor/__init__.py` & `types-aiobotocore-internetmonitor-2.5.4/types_aiobotocore_internetmonitor/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-internetmonitor-2.5.2.post2/types_aiobotocore_internetmonitor/__init__.pyi` & `types-aiobotocore-internetmonitor-2.5.4/types_aiobotocore_internetmonitor/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-internetmonitor-2.5.2.post2/types_aiobotocore_internetmonitor/__main__.py` & `types-aiobotocore-internetmonitor-2.5.4/types_aiobotocore_internetmonitor/__main__.py`

 * *Files 20% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.CloudWatchInternetMonitor 2.5.2\nVersion:        "
-        " 2.5.2.post2\nBuilder version: 7.17.2\nDocs:           "
+        "Type annotations for aiobotocore.CloudWatchInternetMonitor 2.5.4\nVersion:        "
+        " 2.5.4\nBuilder version: 7.17.2\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_internetmonitor//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/internetmonitor.html#CloudWatchInternetMonitor\nOther"
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

### Comparing `types-aiobotocore-internetmonitor-2.5.2.post2/types_aiobotocore_internetmonitor/client.py` & `types-aiobotocore-internetmonitor-2.5.4/types_aiobotocore_internetmonitor/client.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-internetmonitor-2.5.2.post2/types_aiobotocore_internetmonitor/client.pyi` & `types-aiobotocore-internetmonitor-2.5.4/types_aiobotocore_internetmonitor/client.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-internetmonitor-2.5.2.post2/types_aiobotocore_internetmonitor/literals.py` & `types-aiobotocore-internetmonitor-2.5.4/types_aiobotocore_internetmonitor/literals.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-internetmonitor-2.5.2.post2/types_aiobotocore_internetmonitor/literals.pyi` & `types-aiobotocore-internetmonitor-2.5.4/types_aiobotocore_internetmonitor/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-internetmonitor-2.5.2.post2/types_aiobotocore_internetmonitor/paginator.py` & `types-aiobotocore-internetmonitor-2.5.4/types_aiobotocore_internetmonitor/paginator.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-internetmonitor-2.5.2.post2/types_aiobotocore_internetmonitor/paginator.pyi` & `types-aiobotocore-internetmonitor-2.5.4/types_aiobotocore_internetmonitor/paginator.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-internetmonitor-2.5.2.post2/types_aiobotocore_internetmonitor/type_defs.py` & `types-aiobotocore-internetmonitor-2.5.4/types_aiobotocore_internetmonitor/type_defs.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-internetmonitor-2.5.2.post2/types_aiobotocore_internetmonitor/type_defs.pyi` & `types-aiobotocore-internetmonitor-2.5.4/types_aiobotocore_internetmonitor/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-internetmonitor-2.5.2.post2/types_aiobotocore_internetmonitor.egg-info/PKG-INFO` & `types-aiobotocore-internetmonitor-2.5.4/types_aiobotocore_internetmonitor.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-internetmonitor
-Version: 2.5.2.post2
-Summary: Type annotations for aiobotocore.CloudWatchInternetMonitor 2.5.2 service generated with mypy-boto3-builder 7.17.2
+Version: 2.5.4
+Summary: Type annotations for aiobotocore.CloudWatchInternetMonitor 2.5.4 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_internetmonitor/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-internetmonitor.svg?color=blue)](https://pypi.org/project/types-aiobotocore-internetmonitor)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_internetmonitor/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-internetmonitor)](https://pepy.tech/project/types-aiobotocore-internetmonitor)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.CloudWatchInternetMonitor 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/internetmonitor.html#CloudWatchInternetMonitor)
+[aiobotocore.CloudWatchInternetMonitor 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/internetmonitor.html#CloudWatchInternetMonitor)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-internetmonitor-2.5.2.post2/types_aiobotocore_internetmonitor.egg-info/SOURCES.txt` & `types-aiobotocore-internetmonitor-2.5.4/types_aiobotocore_internetmonitor.egg-info/SOURCES.txt`

 * *Files identical despite different names*


# Comparing `tmp/types-aiobotocore-logs-2.5.2.post2.tar.gz` & `tmp/types-aiobotocore-logs-2.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-logs-2.5.2.post2.tar", last modified: Fri Aug  4 13:59:16 2023, max compression
+gzip compressed data, was "types-aiobotocore-logs-2.5.4.tar", last modified: Tue Aug  8 01:24:01 2023, max compression
```

## Comparing `types-aiobotocore-logs-2.5.2.post2.tar` & `types-aiobotocore-logs-2.5.4.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:16.136643 types-aiobotocore-logs-2.5.2.post2/
--rw-r--r--   0 vlad      (1000) vlad      (1000)     1070 2023-08-04 13:43:19.000000 types-aiobotocore-logs-2.5.2.post2/LICENSE
--rw-r--r--   0 vlad      (1000) vlad      (1000)    14185 2023-08-04 13:59:16.136643 types-aiobotocore-logs-2.5.2.post2/PKG-INFO
--rw-r--r--   0 vlad      (1000) vlad      (1000)    12669 2023-08-04 13:43:19.000000 types-aiobotocore-logs-2.5.2.post2/README.md
--rw-r--r--   0 vlad      (1000) vlad      (1000)       38 2023-08-04 13:59:16.136643 types-aiobotocore-logs-2.5.2.post2/setup.cfg
--rw-r--r--   0 vlad      (1000) vlad      (1000)     2037 2023-08-04 13:43:19.000000 types-aiobotocore-logs-2.5.2.post2/setup.py
-drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:16.136643 types-aiobotocore-logs-2.5.2.post2/types_aiobotocore_logs/
--rw-r--r--   0 vlad      (1000) vlad      (1000)     2531 2023-08-04 13:43:19.000000 types-aiobotocore-logs-2.5.2.post2/types_aiobotocore_logs/__init__.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)     2530 2023-08-04 13:43:19.000000 types-aiobotocore-logs-2.5.2.post2/types_aiobotocore_logs/__init__.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)      940 2023-08-04 13:43:19.000000 types-aiobotocore-logs-2.5.2.post2/types_aiobotocore_logs/__main__.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)    40743 2023-08-04 13:43:21.000000 types-aiobotocore-logs-2.5.2.post2/types_aiobotocore_logs/client.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)    40674 2023-08-04 13:43:20.000000 types-aiobotocore-logs-2.5.2.post2/types_aiobotocore_logs/client.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)    10812 2023-08-04 13:43:21.000000 types-aiobotocore-logs-2.5.2.post2/types_aiobotocore_logs/literals.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)    10810 2023-08-04 13:43:21.000000 types-aiobotocore-logs-2.5.2.post2/types_aiobotocore_logs/literals.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)    12339 2023-08-04 13:43:21.000000 types-aiobotocore-logs-2.5.2.post2/types_aiobotocore_logs/paginator.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)    12328 2023-08-04 13:43:21.000000 types-aiobotocore-logs-2.5.2.post2/types_aiobotocore_logs/paginator.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:43:19.000000 types-aiobotocore-logs-2.5.2.post2/types_aiobotocore_logs/py.typed
--rw-r--r--   0 vlad      (1000) vlad      (1000)    37094 2023-08-04 13:43:22.000000 types-aiobotocore-logs-2.5.2.post2/types_aiobotocore_logs/type_defs.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)    37061 2023-08-04 13:43:22.000000 types-aiobotocore-logs-2.5.2.post2/types_aiobotocore_logs/type_defs.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)       65 2023-08-04 13:43:19.000000 types-aiobotocore-logs-2.5.2.post2/types_aiobotocore_logs/version.py
-drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:16.136643 types-aiobotocore-logs-2.5.2.post2/types_aiobotocore_logs.egg-info/
--rw-r--r--   0 vlad      (1000) vlad      (1000)    14185 2023-08-04 13:59:15.000000 types-aiobotocore-logs-2.5.2.post2/types_aiobotocore_logs.egg-info/PKG-INFO
--rw-r--r--   0 vlad      (1000) vlad      (1000)      756 2023-08-04 13:59:16.000000 types-aiobotocore-logs-2.5.2.post2/types_aiobotocore_logs.egg-info/SOURCES.txt
--rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:15.000000 types-aiobotocore-logs-2.5.2.post2/types_aiobotocore_logs.egg-info/dependency_links.txt
--rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:15.000000 types-aiobotocore-logs-2.5.2.post2/types_aiobotocore_logs.egg-info/not-zip-safe
--rw-r--r--   0 vlad      (1000) vlad      (1000)       52 2023-08-04 13:59:15.000000 types-aiobotocore-logs-2.5.2.post2/types_aiobotocore_logs.egg-info/requires.txt
--rw-r--r--   0 vlad      (1000) vlad      (1000)       23 2023-08-04 13:59:15.000000 types-aiobotocore-logs-2.5.2.post2/types_aiobotocore_logs.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:24:01.874724 types-aiobotocore-logs-2.5.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-08 01:14:27.000000 types-aiobotocore-logs-2.5.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    14179 2023-08-08 01:24:01.874724 types-aiobotocore-logs-2.5.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    12669 2023-08-08 01:14:27.000000 types-aiobotocore-logs-2.5.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-08 01:24:01.874724 types-aiobotocore-logs-2.5.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2031 2023-08-08 01:14:27.000000 types-aiobotocore-logs-2.5.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:24:01.870724 types-aiobotocore-logs-2.5.4/types_aiobotocore_logs/
+-rw-r--r--   0 runner    (1001) docker     (123)     2531 2023-08-08 01:14:27.000000 types-aiobotocore-logs-2.5.4/types_aiobotocore_logs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2530 2023-08-08 01:14:27.000000 types-aiobotocore-logs-2.5.4/types_aiobotocore_logs/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      928 2023-08-08 01:14:27.000000 types-aiobotocore-logs-2.5.4/types_aiobotocore_logs/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40743 2023-08-08 01:14:28.000000 types-aiobotocore-logs-2.5.4/types_aiobotocore_logs/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40674 2023-08-08 01:14:28.000000 types-aiobotocore-logs-2.5.4/types_aiobotocore_logs/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    10812 2023-08-08 01:14:28.000000 types-aiobotocore-logs-2.5.4/types_aiobotocore_logs/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10810 2023-08-08 01:14:28.000000 types-aiobotocore-logs-2.5.4/types_aiobotocore_logs/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    12339 2023-08-08 01:14:28.000000 types-aiobotocore-logs-2.5.4/types_aiobotocore_logs/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12328 2023-08-08 01:14:28.000000 types-aiobotocore-logs-2.5.4/types_aiobotocore_logs/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 01:14:27.000000 types-aiobotocore-logs-2.5.4/types_aiobotocore_logs/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    37094 2023-08-08 01:14:29.000000 types-aiobotocore-logs-2.5.4/types_aiobotocore_logs/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37061 2023-08-08 01:14:28.000000 types-aiobotocore-logs-2.5.4/types_aiobotocore_logs/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-08-08 01:14:27.000000 types-aiobotocore-logs-2.5.4/types_aiobotocore_logs/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:24:01.874724 types-aiobotocore-logs-2.5.4/types_aiobotocore_logs.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    14179 2023-08-08 01:24:01.000000 types-aiobotocore-logs-2.5.4/types_aiobotocore_logs.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      756 2023-08-08 01:24:01.000000 types-aiobotocore-logs-2.5.4/types_aiobotocore_logs.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 01:24:01.000000 types-aiobotocore-logs-2.5.4/types_aiobotocore_logs.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 01:24:01.000000 types-aiobotocore-logs-2.5.4/types_aiobotocore_logs.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-08 01:24:01.000000 types-aiobotocore-logs-2.5.4/types_aiobotocore_logs.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-08-08 01:24:01.000000 types-aiobotocore-logs-2.5.4/types_aiobotocore_logs.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-logs-2.5.2.post2/LICENSE` & `types-aiobotocore-logs-2.5.4/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-logs-2.5.2.post2/PKG-INFO` & `types-aiobotocore-logs-2.5.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-logs
-Version: 2.5.2.post2
-Summary: Type annotations for aiobotocore.CloudWatchLogs 2.5.2 service generated with mypy-boto3-builder 7.17.2
+Version: 2.5.4
+Summary: Type annotations for aiobotocore.CloudWatchLogs 2.5.4 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_logs/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-logs.svg?color=blue)](https://pypi.org/project/types-aiobotocore-logs)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_logs/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-logs)](https://pepy.tech/project/types-aiobotocore-logs)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.CloudWatchLogs 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/logs.html#CloudWatchLogs)
+[aiobotocore.CloudWatchLogs 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/logs.html#CloudWatchLogs)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-logs-2.5.2.post2/README.md` & `types-aiobotocore-logs-2.5.4/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-logs.svg?color=blue)](https://pypi.org/project/types-aiobotocore-logs)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_logs/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-logs)](https://pepy.tech/project/types-aiobotocore-logs)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.CloudWatchLogs 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/logs.html#CloudWatchLogs)
+[aiobotocore.CloudWatchLogs 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/logs.html#CloudWatchLogs)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-logs-2.5.2.post2/setup.py` & `types-aiobotocore-logs-2.5.4/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-logs",
-    version="2.5.2.post2",
+    version="2.5.4",
     packages=["types_aiobotocore_logs"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.CloudWatchLogs 2.5.2 service generated with"
+        "Type annotations for aiobotocore.CloudWatchLogs 2.5.4 service generated with"
         " mypy-boto3-builder 7.17.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
```

### Comparing `types-aiobotocore-logs-2.5.2.post2/types_aiobotocore_logs/__init__.py` & `types-aiobotocore-logs-2.5.4/types_aiobotocore_logs/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-logs-2.5.2.post2/types_aiobotocore_logs/__init__.pyi` & `types-aiobotocore-logs-2.5.4/types_aiobotocore_logs/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-logs-2.5.2.post2/types_aiobotocore_logs/__main__.py` & `types-aiobotocore-logs-2.5.4/types_aiobotocore_logs/__main__.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.CloudWatchLogs 2.5.2\nVersion:        "
-        " 2.5.2.post2\nBuilder version: 7.17.2\nDocs:           "
+        "Type annotations for aiobotocore.CloudWatchLogs 2.5.4\nVersion:         2.5.4\nBuilder"
+        " version: 7.17.2\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_logs//\nBoto3 docs:   "
         "   https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/logs.html#CloudWatchLogs\nOther"
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

### Comparing `types-aiobotocore-logs-2.5.2.post2/types_aiobotocore_logs/client.py` & `types-aiobotocore-logs-2.5.4/types_aiobotocore_logs/client.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-logs-2.5.2.post2/types_aiobotocore_logs/client.pyi` & `types-aiobotocore-logs-2.5.4/types_aiobotocore_logs/client.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-logs-2.5.2.post2/types_aiobotocore_logs/literals.py` & `types-aiobotocore-logs-2.5.4/types_aiobotocore_logs/literals.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-logs-2.5.2.post2/types_aiobotocore_logs/literals.pyi` & `types-aiobotocore-logs-2.5.4/types_aiobotocore_logs/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-logs-2.5.2.post2/types_aiobotocore_logs/paginator.py` & `types-aiobotocore-logs-2.5.4/types_aiobotocore_logs/paginator.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-logs-2.5.2.post2/types_aiobotocore_logs/paginator.pyi` & `types-aiobotocore-logs-2.5.4/types_aiobotocore_logs/paginator.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-logs-2.5.2.post2/types_aiobotocore_logs/type_defs.py` & `types-aiobotocore-logs-2.5.4/types_aiobotocore_logs/type_defs.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-logs-2.5.2.post2/types_aiobotocore_logs/type_defs.pyi` & `types-aiobotocore-logs-2.5.4/types_aiobotocore_logs/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-logs-2.5.2.post2/types_aiobotocore_logs.egg-info/PKG-INFO` & `types-aiobotocore-logs-2.5.4/types_aiobotocore_logs.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-logs
-Version: 2.5.2.post2
-Summary: Type annotations for aiobotocore.CloudWatchLogs 2.5.2 service generated with mypy-boto3-builder 7.17.2
+Version: 2.5.4
+Summary: Type annotations for aiobotocore.CloudWatchLogs 2.5.4 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_logs/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-logs.svg?color=blue)](https://pypi.org/project/types-aiobotocore-logs)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_logs/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-logs)](https://pepy.tech/project/types-aiobotocore-logs)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.CloudWatchLogs 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/logs.html#CloudWatchLogs)
+[aiobotocore.CloudWatchLogs 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/logs.html#CloudWatchLogs)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-logs-2.5.2.post2/types_aiobotocore_logs.egg-info/SOURCES.txt` & `types-aiobotocore-logs-2.5.4/types_aiobotocore_logs.egg-info/SOURCES.txt`

 * *Files identical despite different names*


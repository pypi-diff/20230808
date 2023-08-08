# Comparing `tmp/types-aiobotocore-scheduler-2.5.2.post2.tar.gz` & `tmp/types-aiobotocore-scheduler-2.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-scheduler-2.5.2.post2.tar", last modified: Fri Aug  4 13:59:25 2023, max compression
+gzip compressed data, was "types-aiobotocore-scheduler-2.5.4.tar", last modified: Tue Aug  8 01:24:24 2023, max compression
```

## Comparing `types-aiobotocore-scheduler-2.5.2.post2.tar` & `types-aiobotocore-scheduler-2.5.4.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:25.686643 types-aiobotocore-scheduler-2.5.2.post2/
--rw-r--r--   0 vlad      (1000) vlad      (1000)     1070 2023-08-04 13:52:34.000000 types-aiobotocore-scheduler-2.5.2.post2/LICENSE
--rw-r--r--   0 vlad      (1000) vlad      (1000)    13325 2023-08-04 13:59:25.676643 types-aiobotocore-scheduler-2.5.2.post2/PKG-INFO
--rw-r--r--   0 vlad      (1000) vlad      (1000)    11788 2023-08-04 13:52:34.000000 types-aiobotocore-scheduler-2.5.2.post2/README.md
--rw-r--r--   0 vlad      (1000) vlad      (1000)       38 2023-08-04 13:59:25.686643 types-aiobotocore-scheduler-2.5.2.post2/setup.cfg
--rw-r--r--   0 vlad      (1000) vlad      (1000)     2097 2023-08-04 13:52:34.000000 types-aiobotocore-scheduler-2.5.2.post2/setup.py
-drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:25.676643 types-aiobotocore-scheduler-2.5.2.post2/types_aiobotocore_scheduler/
--rw-r--r--   0 vlad      (1000) vlad      (1000)      939 2023-08-04 13:52:34.000000 types-aiobotocore-scheduler-2.5.2.post2/types_aiobotocore_scheduler/__init__.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)      938 2023-08-04 13:52:34.000000 types-aiobotocore-scheduler-2.5.2.post2/types_aiobotocore_scheduler/__init__.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)      973 2023-08-04 13:52:34.000000 types-aiobotocore-scheduler-2.5.2.post2/types_aiobotocore_scheduler/__main__.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)    13255 2023-08-04 13:52:34.000000 types-aiobotocore-scheduler-2.5.2.post2/types_aiobotocore_scheduler/client.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)    13232 2023-08-04 13:52:34.000000 types-aiobotocore-scheduler-2.5.2.post2/types_aiobotocore_scheduler/client.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)     9268 2023-08-04 13:52:34.000000 types-aiobotocore-scheduler-2.5.2.post2/types_aiobotocore_scheduler/literals.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)     9266 2023-08-04 13:52:34.000000 types-aiobotocore-scheduler-2.5.2.post2/types_aiobotocore_scheduler/literals.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)     3359 2023-08-04 13:52:34.000000 types-aiobotocore-scheduler-2.5.2.post2/types_aiobotocore_scheduler/paginator.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)     3355 2023-08-04 13:52:34.000000 types-aiobotocore-scheduler-2.5.2.post2/types_aiobotocore_scheduler/paginator.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:52:34.000000 types-aiobotocore-scheduler-2.5.2.post2/types_aiobotocore_scheduler/py.typed
--rw-r--r--   0 vlad      (1000) vlad      (1000)    15803 2023-08-04 13:52:38.000000 types-aiobotocore-scheduler-2.5.2.post2/types_aiobotocore_scheduler/type_defs.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)    15781 2023-08-04 13:52:38.000000 types-aiobotocore-scheduler-2.5.2.post2/types_aiobotocore_scheduler/type_defs.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)       65 2023-08-04 13:52:34.000000 types-aiobotocore-scheduler-2.5.2.post2/types_aiobotocore_scheduler/version.py
-drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:25.676643 types-aiobotocore-scheduler-2.5.2.post2/types_aiobotocore_scheduler.egg-info/
--rw-r--r--   0 vlad      (1000) vlad      (1000)    13325 2023-08-04 13:59:25.000000 types-aiobotocore-scheduler-2.5.2.post2/types_aiobotocore_scheduler.egg-info/PKG-INFO
--rw-r--r--   0 vlad      (1000) vlad      (1000)      851 2023-08-04 13:59:25.000000 types-aiobotocore-scheduler-2.5.2.post2/types_aiobotocore_scheduler.egg-info/SOURCES.txt
--rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:25.000000 types-aiobotocore-scheduler-2.5.2.post2/types_aiobotocore_scheduler.egg-info/dependency_links.txt
--rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:25.000000 types-aiobotocore-scheduler-2.5.2.post2/types_aiobotocore_scheduler.egg-info/not-zip-safe
--rw-r--r--   0 vlad      (1000) vlad      (1000)       52 2023-08-04 13:59:25.000000 types-aiobotocore-scheduler-2.5.2.post2/types_aiobotocore_scheduler.egg-info/requires.txt
--rw-r--r--   0 vlad      (1000) vlad      (1000)       28 2023-08-04 13:59:25.000000 types-aiobotocore-scheduler-2.5.2.post2/types_aiobotocore_scheduler.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:24:24.566776 types-aiobotocore-scheduler-2.5.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-08 01:20:33.000000 types-aiobotocore-scheduler-2.5.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    13319 2023-08-08 01:24:24.558776 types-aiobotocore-scheduler-2.5.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    11788 2023-08-08 01:20:33.000000 types-aiobotocore-scheduler-2.5.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-08 01:24:24.566776 types-aiobotocore-scheduler-2.5.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2091 2023-08-08 01:20:33.000000 types-aiobotocore-scheduler-2.5.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:24:24.550776 types-aiobotocore-scheduler-2.5.4/types_aiobotocore_scheduler/
+-rw-r--r--   0 runner    (1001) docker     (123)      939 2023-08-08 01:20:33.000000 types-aiobotocore-scheduler-2.5.4/types_aiobotocore_scheduler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      938 2023-08-08 01:20:33.000000 types-aiobotocore-scheduler-2.5.4/types_aiobotocore_scheduler/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      961 2023-08-08 01:20:33.000000 types-aiobotocore-scheduler-2.5.4/types_aiobotocore_scheduler/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13255 2023-08-08 01:20:33.000000 types-aiobotocore-scheduler-2.5.4/types_aiobotocore_scheduler/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13232 2023-08-08 01:20:33.000000 types-aiobotocore-scheduler-2.5.4/types_aiobotocore_scheduler/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9268 2023-08-08 01:20:33.000000 types-aiobotocore-scheduler-2.5.4/types_aiobotocore_scheduler/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9266 2023-08-08 01:20:33.000000 types-aiobotocore-scheduler-2.5.4/types_aiobotocore_scheduler/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     3359 2023-08-08 01:20:33.000000 types-aiobotocore-scheduler-2.5.4/types_aiobotocore_scheduler/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3355 2023-08-08 01:20:33.000000 types-aiobotocore-scheduler-2.5.4/types_aiobotocore_scheduler/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 01:20:33.000000 types-aiobotocore-scheduler-2.5.4/types_aiobotocore_scheduler/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    15803 2023-08-08 01:20:34.000000 types-aiobotocore-scheduler-2.5.4/types_aiobotocore_scheduler/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15781 2023-08-08 01:20:33.000000 types-aiobotocore-scheduler-2.5.4/types_aiobotocore_scheduler/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-08-08 01:20:33.000000 types-aiobotocore-scheduler-2.5.4/types_aiobotocore_scheduler/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:24:24.558776 types-aiobotocore-scheduler-2.5.4/types_aiobotocore_scheduler.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    13319 2023-08-08 01:24:24.000000 types-aiobotocore-scheduler-2.5.4/types_aiobotocore_scheduler.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      851 2023-08-08 01:24:24.000000 types-aiobotocore-scheduler-2.5.4/types_aiobotocore_scheduler.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 01:24:24.000000 types-aiobotocore-scheduler-2.5.4/types_aiobotocore_scheduler.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 01:24:24.000000 types-aiobotocore-scheduler-2.5.4/types_aiobotocore_scheduler.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-08 01:24:24.000000 types-aiobotocore-scheduler-2.5.4/types_aiobotocore_scheduler.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-08-08 01:24:24.000000 types-aiobotocore-scheduler-2.5.4/types_aiobotocore_scheduler.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-scheduler-2.5.2.post2/LICENSE` & `types-aiobotocore-scheduler-2.5.4/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-scheduler-2.5.2.post2/PKG-INFO` & `types-aiobotocore-scheduler-2.5.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-scheduler
-Version: 2.5.2.post2
-Summary: Type annotations for aiobotocore.EventBridgeScheduler 2.5.2 service generated with mypy-boto3-builder 7.17.2
+Version: 2.5.4
+Summary: Type annotations for aiobotocore.EventBridgeScheduler 2.5.4 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_scheduler/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-scheduler.svg?color=blue)](https://pypi.org/project/types-aiobotocore-scheduler)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_scheduler/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-scheduler)](https://pepy.tech/project/types-aiobotocore-scheduler)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.EventBridgeScheduler 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/scheduler.html#EventBridgeScheduler)
+[aiobotocore.EventBridgeScheduler 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/scheduler.html#EventBridgeScheduler)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-scheduler-2.5.2.post2/README.md` & `types-aiobotocore-scheduler-2.5.4/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-scheduler.svg?color=blue)](https://pypi.org/project/types-aiobotocore-scheduler)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_scheduler/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-scheduler)](https://pepy.tech/project/types-aiobotocore-scheduler)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.EventBridgeScheduler 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/scheduler.html#EventBridgeScheduler)
+[aiobotocore.EventBridgeScheduler 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/scheduler.html#EventBridgeScheduler)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-scheduler-2.5.2.post2/setup.py` & `types-aiobotocore-scheduler-2.5.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-scheduler",
-    version="2.5.2.post2",
+    version="2.5.4",
     packages=["types_aiobotocore_scheduler"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.EventBridgeScheduler 2.5.2 service generated with"
+        "Type annotations for aiobotocore.EventBridgeScheduler 2.5.4 service generated with"
         " mypy-boto3-builder 7.17.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
```

### Comparing `types-aiobotocore-scheduler-2.5.2.post2/types_aiobotocore_scheduler/__init__.py` & `types-aiobotocore-scheduler-2.5.4/types_aiobotocore_scheduler/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-scheduler-2.5.2.post2/types_aiobotocore_scheduler/__init__.pyi` & `types-aiobotocore-scheduler-2.5.4/types_aiobotocore_scheduler/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-scheduler-2.5.2.post2/types_aiobotocore_scheduler/__main__.py` & `types-aiobotocore-scheduler-2.5.4/types_aiobotocore_scheduler/__main__.py`

 * *Files 9% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.EventBridgeScheduler 2.5.2\nVersion:        "
-        " 2.5.2.post2\nBuilder version: 7.17.2\nDocs:           "
+        "Type annotations for aiobotocore.EventBridgeScheduler 2.5.4\nVersion:        "
+        " 2.5.4\nBuilder version: 7.17.2\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_scheduler//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/scheduler.html#EventBridgeScheduler\nOther"
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

### Comparing `types-aiobotocore-scheduler-2.5.2.post2/types_aiobotocore_scheduler/client.py` & `types-aiobotocore-scheduler-2.5.4/types_aiobotocore_scheduler/client.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-scheduler-2.5.2.post2/types_aiobotocore_scheduler/client.pyi` & `types-aiobotocore-scheduler-2.5.4/types_aiobotocore_scheduler/client.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-scheduler-2.5.2.post2/types_aiobotocore_scheduler/literals.py` & `types-aiobotocore-scheduler-2.5.4/types_aiobotocore_scheduler/literals.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-scheduler-2.5.2.post2/types_aiobotocore_scheduler/literals.pyi` & `types-aiobotocore-scheduler-2.5.4/types_aiobotocore_scheduler/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-scheduler-2.5.2.post2/types_aiobotocore_scheduler/paginator.py` & `types-aiobotocore-scheduler-2.5.4/types_aiobotocore_scheduler/paginator.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-scheduler-2.5.2.post2/types_aiobotocore_scheduler/paginator.pyi` & `types-aiobotocore-scheduler-2.5.4/types_aiobotocore_scheduler/paginator.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-scheduler-2.5.2.post2/types_aiobotocore_scheduler/type_defs.py` & `types-aiobotocore-scheduler-2.5.4/types_aiobotocore_scheduler/type_defs.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-scheduler-2.5.2.post2/types_aiobotocore_scheduler/type_defs.pyi` & `types-aiobotocore-scheduler-2.5.4/types_aiobotocore_scheduler/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-scheduler-2.5.2.post2/types_aiobotocore_scheduler.egg-info/PKG-INFO` & `types-aiobotocore-scheduler-2.5.4/types_aiobotocore_scheduler.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-scheduler
-Version: 2.5.2.post2
-Summary: Type annotations for aiobotocore.EventBridgeScheduler 2.5.2 service generated with mypy-boto3-builder 7.17.2
+Version: 2.5.4
+Summary: Type annotations for aiobotocore.EventBridgeScheduler 2.5.4 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_scheduler/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-scheduler.svg?color=blue)](https://pypi.org/project/types-aiobotocore-scheduler)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_scheduler/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-scheduler)](https://pepy.tech/project/types-aiobotocore-scheduler)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.EventBridgeScheduler 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/scheduler.html#EventBridgeScheduler)
+[aiobotocore.EventBridgeScheduler 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/scheduler.html#EventBridgeScheduler)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-scheduler-2.5.2.post2/types_aiobotocore_scheduler.egg-info/SOURCES.txt` & `types-aiobotocore-scheduler-2.5.4/types_aiobotocore_scheduler.egg-info/SOURCES.txt`

 * *Files identical despite different names*


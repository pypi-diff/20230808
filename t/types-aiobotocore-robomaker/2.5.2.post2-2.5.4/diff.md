# Comparing `tmp/types-aiobotocore-robomaker-2.5.2.post2.tar.gz` & `tmp/types-aiobotocore-robomaker-2.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-robomaker-2.5.2.post2.tar", last modified: Fri Aug  4 13:59:23 2023, max compression
+gzip compressed data, was "types-aiobotocore-robomaker-2.5.4.tar", last modified: Tue Aug  8 01:24:19 2023, max compression
```

## Comparing `types-aiobotocore-robomaker-2.5.2.post2.tar` & `types-aiobotocore-robomaker-2.5.4.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:23.816643 types-aiobotocore-robomaker-2.5.2.post2/
--rw-r--r--   0 vlad      (1000) vlad      (1000)     1070 2023-08-04 13:50:54.000000 types-aiobotocore-robomaker-2.5.2.post2/LICENSE
--rw-r--r--   0 vlad      (1000) vlad      (1000)    14624 2023-08-04 13:59:23.806643 types-aiobotocore-robomaker-2.5.2.post2/PKG-INFO
--rw-r--r--   0 vlad      (1000) vlad      (1000)    13098 2023-08-04 13:50:54.000000 types-aiobotocore-robomaker-2.5.2.post2/README.md
--rw-r--r--   0 vlad      (1000) vlad      (1000)       38 2023-08-04 13:59:23.816643 types-aiobotocore-robomaker-2.5.2.post2/setup.cfg
--rw-r--r--   0 vlad      (1000) vlad      (1000)     2086 2023-08-04 13:50:54.000000 types-aiobotocore-robomaker-2.5.2.post2/setup.py
-drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:23.806643 types-aiobotocore-robomaker-2.5.2.post2/types_aiobotocore_robomaker/
--rw-r--r--   0 vlad      (1000) vlad      (1000)     2867 2023-08-04 13:50:54.000000 types-aiobotocore-robomaker-2.5.2.post2/types_aiobotocore_robomaker/__init__.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)     2866 2023-08-04 13:50:54.000000 types-aiobotocore-robomaker-2.5.2.post2/types_aiobotocore_robomaker/__init__.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)      951 2023-08-04 13:50:54.000000 types-aiobotocore-robomaker-2.5.2.post2/types_aiobotocore_robomaker/__main__.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)    44856 2023-08-04 13:50:54.000000 types-aiobotocore-robomaker-2.5.2.post2/types_aiobotocore_robomaker/client.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)    44779 2023-08-04 13:50:54.000000 types-aiobotocore-robomaker-2.5.2.post2/types_aiobotocore_robomaker/client.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)    13941 2023-08-04 13:50:55.000000 types-aiobotocore-robomaker-2.5.2.post2/types_aiobotocore_robomaker/literals.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)    13939 2023-08-04 13:50:55.000000 types-aiobotocore-robomaker-2.5.2.post2/types_aiobotocore_robomaker/literals.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)    14005 2023-08-04 13:50:55.000000 types-aiobotocore-robomaker-2.5.2.post2/types_aiobotocore_robomaker/paginator.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)    13992 2023-08-04 13:50:54.000000 types-aiobotocore-robomaker-2.5.2.post2/types_aiobotocore_robomaker/paginator.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:50:54.000000 types-aiobotocore-robomaker-2.5.2.post2/types_aiobotocore_robomaker/py.typed
--rw-r--r--   0 vlad      (1000) vlad      (1000)    63517 2023-08-04 13:50:56.000000 types-aiobotocore-robomaker-2.5.2.post2/types_aiobotocore_robomaker/type_defs.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)    63462 2023-08-04 13:50:56.000000 types-aiobotocore-robomaker-2.5.2.post2/types_aiobotocore_robomaker/type_defs.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)       65 2023-08-04 13:50:54.000000 types-aiobotocore-robomaker-2.5.2.post2/types_aiobotocore_robomaker/version.py
-drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:23.806643 types-aiobotocore-robomaker-2.5.2.post2/types_aiobotocore_robomaker.egg-info/
--rw-r--r--   0 vlad      (1000) vlad      (1000)    14624 2023-08-04 13:59:23.000000 types-aiobotocore-robomaker-2.5.2.post2/types_aiobotocore_robomaker.egg-info/PKG-INFO
--rw-r--r--   0 vlad      (1000) vlad      (1000)      851 2023-08-04 13:59:23.000000 types-aiobotocore-robomaker-2.5.2.post2/types_aiobotocore_robomaker.egg-info/SOURCES.txt
--rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:23.000000 types-aiobotocore-robomaker-2.5.2.post2/types_aiobotocore_robomaker.egg-info/dependency_links.txt
--rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:23.000000 types-aiobotocore-robomaker-2.5.2.post2/types_aiobotocore_robomaker.egg-info/not-zip-safe
--rw-r--r--   0 vlad      (1000) vlad      (1000)       52 2023-08-04 13:59:23.000000 types-aiobotocore-robomaker-2.5.2.post2/types_aiobotocore_robomaker.egg-info/requires.txt
--rw-r--r--   0 vlad      (1000) vlad      (1000)       28 2023-08-04 13:59:23.000000 types-aiobotocore-robomaker-2.5.2.post2/types_aiobotocore_robomaker.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:24:19.866764 types-aiobotocore-robomaker-2.5.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-08 01:19:29.000000 types-aiobotocore-robomaker-2.5.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    14618 2023-08-08 01:24:19.858764 types-aiobotocore-robomaker-2.5.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    13098 2023-08-08 01:19:29.000000 types-aiobotocore-robomaker-2.5.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-08 01:24:19.866764 types-aiobotocore-robomaker-2.5.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2080 2023-08-08 01:19:29.000000 types-aiobotocore-robomaker-2.5.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:24:19.854764 types-aiobotocore-robomaker-2.5.4/types_aiobotocore_robomaker/
+-rw-r--r--   0 runner    (1001) docker     (123)     2867 2023-08-08 01:19:29.000000 types-aiobotocore-robomaker-2.5.4/types_aiobotocore_robomaker/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2866 2023-08-08 01:19:29.000000 types-aiobotocore-robomaker-2.5.4/types_aiobotocore_robomaker/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      939 2023-08-08 01:19:29.000000 types-aiobotocore-robomaker-2.5.4/types_aiobotocore_robomaker/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    44856 2023-08-08 01:19:29.000000 types-aiobotocore-robomaker-2.5.4/types_aiobotocore_robomaker/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    44779 2023-08-08 01:19:29.000000 types-aiobotocore-robomaker-2.5.4/types_aiobotocore_robomaker/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    13941 2023-08-08 01:19:29.000000 types-aiobotocore-robomaker-2.5.4/types_aiobotocore_robomaker/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13939 2023-08-08 01:19:29.000000 types-aiobotocore-robomaker-2.5.4/types_aiobotocore_robomaker/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    14005 2023-08-08 01:19:29.000000 types-aiobotocore-robomaker-2.5.4/types_aiobotocore_robomaker/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13992 2023-08-08 01:19:29.000000 types-aiobotocore-robomaker-2.5.4/types_aiobotocore_robomaker/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 01:19:29.000000 types-aiobotocore-robomaker-2.5.4/types_aiobotocore_robomaker/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    63517 2023-08-08 01:19:31.000000 types-aiobotocore-robomaker-2.5.4/types_aiobotocore_robomaker/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    63462 2023-08-08 01:19:30.000000 types-aiobotocore-robomaker-2.5.4/types_aiobotocore_robomaker/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-08-08 01:19:29.000000 types-aiobotocore-robomaker-2.5.4/types_aiobotocore_robomaker/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:24:19.858764 types-aiobotocore-robomaker-2.5.4/types_aiobotocore_robomaker.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    14618 2023-08-08 01:24:19.000000 types-aiobotocore-robomaker-2.5.4/types_aiobotocore_robomaker.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      851 2023-08-08 01:24:19.000000 types-aiobotocore-robomaker-2.5.4/types_aiobotocore_robomaker.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 01:24:19.000000 types-aiobotocore-robomaker-2.5.4/types_aiobotocore_robomaker.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 01:24:19.000000 types-aiobotocore-robomaker-2.5.4/types_aiobotocore_robomaker.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-08 01:24:19.000000 types-aiobotocore-robomaker-2.5.4/types_aiobotocore_robomaker.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-08-08 01:24:19.000000 types-aiobotocore-robomaker-2.5.4/types_aiobotocore_robomaker.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-robomaker-2.5.2.post2/LICENSE` & `types-aiobotocore-robomaker-2.5.4/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-robomaker-2.5.2.post2/PKG-INFO` & `types-aiobotocore-robomaker-2.5.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-robomaker
-Version: 2.5.2.post2
-Summary: Type annotations for aiobotocore.RoboMaker 2.5.2 service generated with mypy-boto3-builder 7.17.2
+Version: 2.5.4
+Summary: Type annotations for aiobotocore.RoboMaker 2.5.4 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_robomaker/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-robomaker.svg?color=blue)](https://pypi.org/project/types-aiobotocore-robomaker)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_robomaker/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-robomaker)](https://pepy.tech/project/types-aiobotocore-robomaker)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.RoboMaker 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/robomaker.html#RoboMaker)
+[aiobotocore.RoboMaker 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/robomaker.html#RoboMaker)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-robomaker-2.5.2.post2/README.md` & `types-aiobotocore-robomaker-2.5.4/README.md`

 * *Files identical despite different names*

```diff
@@ -6,15 +6,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-robomaker.svg?color=blue)](https://pypi.org/project/types-aiobotocore-robomaker)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_robomaker/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-robomaker)](https://pepy.tech/project/types-aiobotocore-robomaker)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.RoboMaker 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/robomaker.html#RoboMaker)
+[aiobotocore.RoboMaker 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/robomaker.html#RoboMaker)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-robomaker-2.5.2.post2/setup.py` & `types-aiobotocore-robomaker-2.5.4/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-robomaker",
-    version="2.5.2.post2",
+    version="2.5.4",
     packages=["types_aiobotocore_robomaker"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.RoboMaker 2.5.2 service generated with mypy-boto3-builder"
+        "Type annotations for aiobotocore.RoboMaker 2.5.4 service generated with mypy-boto3-builder"
         " 7.17.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
```

### Comparing `types-aiobotocore-robomaker-2.5.2.post2/types_aiobotocore_robomaker/__init__.py` & `types-aiobotocore-robomaker-2.5.4/types_aiobotocore_robomaker/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-robomaker-2.5.2.post2/types_aiobotocore_robomaker/__init__.pyi` & `types-aiobotocore-robomaker-2.5.4/types_aiobotocore_robomaker/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-robomaker-2.5.2.post2/types_aiobotocore_robomaker/__main__.py` & `types-aiobotocore-robomaker-2.5.4/types_aiobotocore_robomaker/__main__.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.RoboMaker 2.5.2\nVersion:         2.5.2.post2\nBuilder"
-        " version: 7.17.2\nDocs:           "
+        "Type annotations for aiobotocore.RoboMaker 2.5.4\nVersion:         2.5.4\nBuilder version:"
+        " 7.17.2\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_robomaker//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/robomaker.html#RoboMaker\nOther"
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

### Comparing `types-aiobotocore-robomaker-2.5.2.post2/types_aiobotocore_robomaker/client.py` & `types-aiobotocore-robomaker-2.5.4/types_aiobotocore_robomaker/client.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-robomaker-2.5.2.post2/types_aiobotocore_robomaker/client.pyi` & `types-aiobotocore-robomaker-2.5.4/types_aiobotocore_robomaker/client.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-robomaker-2.5.2.post2/types_aiobotocore_robomaker/literals.py` & `types-aiobotocore-robomaker-2.5.4/types_aiobotocore_robomaker/literals.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-robomaker-2.5.2.post2/types_aiobotocore_robomaker/literals.pyi` & `types-aiobotocore-robomaker-2.5.4/types_aiobotocore_robomaker/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-robomaker-2.5.2.post2/types_aiobotocore_robomaker/paginator.py` & `types-aiobotocore-robomaker-2.5.4/types_aiobotocore_robomaker/paginator.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-robomaker-2.5.2.post2/types_aiobotocore_robomaker/paginator.pyi` & `types-aiobotocore-robomaker-2.5.4/types_aiobotocore_robomaker/paginator.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-robomaker-2.5.2.post2/types_aiobotocore_robomaker/type_defs.py` & `types-aiobotocore-robomaker-2.5.4/types_aiobotocore_robomaker/type_defs.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-robomaker-2.5.2.post2/types_aiobotocore_robomaker/type_defs.pyi` & `types-aiobotocore-robomaker-2.5.4/types_aiobotocore_robomaker/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-robomaker-2.5.2.post2/types_aiobotocore_robomaker.egg-info/PKG-INFO` & `types-aiobotocore-robomaker-2.5.4/types_aiobotocore_robomaker.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-robomaker
-Version: 2.5.2.post2
-Summary: Type annotations for aiobotocore.RoboMaker 2.5.2 service generated with mypy-boto3-builder 7.17.2
+Version: 2.5.4
+Summary: Type annotations for aiobotocore.RoboMaker 2.5.4 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_robomaker/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-robomaker.svg?color=blue)](https://pypi.org/project/types-aiobotocore-robomaker)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_robomaker/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-robomaker)](https://pepy.tech/project/types-aiobotocore-robomaker)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.RoboMaker 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/robomaker.html#RoboMaker)
+[aiobotocore.RoboMaker 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/robomaker.html#RoboMaker)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-robomaker-2.5.2.post2/types_aiobotocore_robomaker.egg-info/SOURCES.txt` & `types-aiobotocore-robomaker-2.5.4/types_aiobotocore_robomaker.egg-info/SOURCES.txt`

 * *Files identical despite different names*


# Comparing `tmp/types-aiobotocore-pipes-2.5.2.post2.tar.gz` & `tmp/types-aiobotocore-pipes-2.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-pipes-2.5.2.post2.tar", last modified: Fri Aug  4 13:59:21 2023, max compression
+gzip compressed data, was "types-aiobotocore-pipes-2.5.4.tar", last modified: Tue Aug  8 01:24:15 2023, max compression
```

## Comparing `types-aiobotocore-pipes-2.5.2.post2.tar` & `types-aiobotocore-pipes-2.5.4.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:21.696643 types-aiobotocore-pipes-2.5.2.post2/
--rw-r--r--   0 vlad      (1000) vlad      (1000)     1070 2023-08-04 13:47:03.000000 types-aiobotocore-pipes-2.5.2.post2/LICENSE
--rw-r--r--   0 vlad      (1000) vlad      (1000)    12890 2023-08-04 13:59:21.696643 types-aiobotocore-pipes-2.5.2.post2/PKG-INFO
--rw-r--r--   0 vlad      (1000) vlad      (1000)    11369 2023-08-04 13:47:03.000000 types-aiobotocore-pipes-2.5.2.post2/README.md
--rw-r--r--   0 vlad      (1000) vlad      (1000)       38 2023-08-04 13:59:21.696643 types-aiobotocore-pipes-2.5.2.post2/setup.cfg
--rw-r--r--   0 vlad      (1000) vlad      (1000)     2069 2023-08-04 13:47:03.000000 types-aiobotocore-pipes-2.5.2.post2/setup.py
-drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:21.696643 types-aiobotocore-pipes-2.5.2.post2/types_aiobotocore_pipes/
--rw-r--r--   0 vlad      (1000) vlad      (1000)      656 2023-08-04 13:47:03.000000 types-aiobotocore-pipes-2.5.2.post2/types_aiobotocore_pipes/__init__.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)      655 2023-08-04 13:47:03.000000 types-aiobotocore-pipes-2.5.2.post2/types_aiobotocore_pipes/__init__.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)      946 2023-08-04 13:47:03.000000 types-aiobotocore-pipes-2.5.2.post2/types_aiobotocore_pipes/__main__.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)    10880 2023-08-04 13:47:03.000000 types-aiobotocore-pipes-2.5.2.post2/types_aiobotocore_pipes/client.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)    10860 2023-08-04 13:47:03.000000 types-aiobotocore-pipes-2.5.2.post2/types_aiobotocore_pipes/client.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)    10162 2023-08-04 13:47:03.000000 types-aiobotocore-pipes-2.5.2.post2/types_aiobotocore_pipes/literals.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)    10160 2023-08-04 13:47:03.000000 types-aiobotocore-pipes-2.5.2.post2/types_aiobotocore_pipes/literals.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)     2205 2023-08-04 13:47:03.000000 types-aiobotocore-pipes-2.5.2.post2/types_aiobotocore_pipes/paginator.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)     2202 2023-08-04 13:47:03.000000 types-aiobotocore-pipes-2.5.2.post2/types_aiobotocore_pipes/paginator.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:47:03.000000 types-aiobotocore-pipes-2.5.2.post2/types_aiobotocore_pipes/py.typed
--rw-r--r--   0 vlad      (1000) vlad      (1000)    31941 2023-08-04 13:47:04.000000 types-aiobotocore-pipes-2.5.2.post2/types_aiobotocore_pipes/type_defs.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)    31911 2023-08-04 13:47:04.000000 types-aiobotocore-pipes-2.5.2.post2/types_aiobotocore_pipes/type_defs.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)       65 2023-08-04 13:47:03.000000 types-aiobotocore-pipes-2.5.2.post2/types_aiobotocore_pipes/version.py
-drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:21.696643 types-aiobotocore-pipes-2.5.2.post2/types_aiobotocore_pipes.egg-info/
--rw-r--r--   0 vlad      (1000) vlad      (1000)    12890 2023-08-04 13:59:21.000000 types-aiobotocore-pipes-2.5.2.post2/types_aiobotocore_pipes.egg-info/PKG-INFO
--rw-r--r--   0 vlad      (1000) vlad      (1000)      775 2023-08-04 13:59:21.000000 types-aiobotocore-pipes-2.5.2.post2/types_aiobotocore_pipes.egg-info/SOURCES.txt
--rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:21.000000 types-aiobotocore-pipes-2.5.2.post2/types_aiobotocore_pipes.egg-info/dependency_links.txt
--rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:21.000000 types-aiobotocore-pipes-2.5.2.post2/types_aiobotocore_pipes.egg-info/not-zip-safe
--rw-r--r--   0 vlad      (1000) vlad      (1000)       52 2023-08-04 13:59:21.000000 types-aiobotocore-pipes-2.5.2.post2/types_aiobotocore_pipes.egg-info/requires.txt
--rw-r--r--   0 vlad      (1000) vlad      (1000)       24 2023-08-04 13:59:21.000000 types-aiobotocore-pipes-2.5.2.post2/types_aiobotocore_pipes.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:24:15.266753 types-aiobotocore-pipes-2.5.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-08 01:16:49.000000 types-aiobotocore-pipes-2.5.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    12884 2023-08-08 01:24:15.266753 types-aiobotocore-pipes-2.5.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    11369 2023-08-08 01:16:49.000000 types-aiobotocore-pipes-2.5.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-08 01:24:15.266753 types-aiobotocore-pipes-2.5.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2063 2023-08-08 01:16:49.000000 types-aiobotocore-pipes-2.5.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:24:15.254753 types-aiobotocore-pipes-2.5.4/types_aiobotocore_pipes/
+-rw-r--r--   0 runner    (1001) docker     (123)      656 2023-08-08 01:16:49.000000 types-aiobotocore-pipes-2.5.4/types_aiobotocore_pipes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      655 2023-08-08 01:16:49.000000 types-aiobotocore-pipes-2.5.4/types_aiobotocore_pipes/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      934 2023-08-08 01:16:49.000000 types-aiobotocore-pipes-2.5.4/types_aiobotocore_pipes/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10880 2023-08-08 01:16:49.000000 types-aiobotocore-pipes-2.5.4/types_aiobotocore_pipes/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10860 2023-08-08 01:16:49.000000 types-aiobotocore-pipes-2.5.4/types_aiobotocore_pipes/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    10162 2023-08-08 01:16:50.000000 types-aiobotocore-pipes-2.5.4/types_aiobotocore_pipes/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10160 2023-08-08 01:16:49.000000 types-aiobotocore-pipes-2.5.4/types_aiobotocore_pipes/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2205 2023-08-08 01:16:49.000000 types-aiobotocore-pipes-2.5.4/types_aiobotocore_pipes/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2202 2023-08-08 01:16:49.000000 types-aiobotocore-pipes-2.5.4/types_aiobotocore_pipes/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 01:16:49.000000 types-aiobotocore-pipes-2.5.4/types_aiobotocore_pipes/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    31941 2023-08-08 01:16:50.000000 types-aiobotocore-pipes-2.5.4/types_aiobotocore_pipes/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31911 2023-08-08 01:16:50.000000 types-aiobotocore-pipes-2.5.4/types_aiobotocore_pipes/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-08-08 01:16:49.000000 types-aiobotocore-pipes-2.5.4/types_aiobotocore_pipes/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:24:15.266753 types-aiobotocore-pipes-2.5.4/types_aiobotocore_pipes.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    12884 2023-08-08 01:24:15.000000 types-aiobotocore-pipes-2.5.4/types_aiobotocore_pipes.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      775 2023-08-08 01:24:15.000000 types-aiobotocore-pipes-2.5.4/types_aiobotocore_pipes.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 01:24:15.000000 types-aiobotocore-pipes-2.5.4/types_aiobotocore_pipes.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 01:24:15.000000 types-aiobotocore-pipes-2.5.4/types_aiobotocore_pipes.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-08 01:24:15.000000 types-aiobotocore-pipes-2.5.4/types_aiobotocore_pipes.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-08-08 01:24:15.000000 types-aiobotocore-pipes-2.5.4/types_aiobotocore_pipes.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-pipes-2.5.2.post2/LICENSE` & `types-aiobotocore-pipes-2.5.4/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-pipes-2.5.2.post2/PKG-INFO` & `types-aiobotocore-pipes-2.5.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-pipes
-Version: 2.5.2.post2
-Summary: Type annotations for aiobotocore.EventBridgePipes 2.5.2 service generated with mypy-boto3-builder 7.17.2
+Version: 2.5.4
+Summary: Type annotations for aiobotocore.EventBridgePipes 2.5.4 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_pipes/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-pipes.svg?color=blue)](https://pypi.org/project/types-aiobotocore-pipes)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_pipes/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-pipes)](https://pepy.tech/project/types-aiobotocore-pipes)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.EventBridgePipes 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pipes.html#EventBridgePipes)
+[aiobotocore.EventBridgePipes 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pipes.html#EventBridgePipes)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-pipes-2.5.2.post2/README.md` & `types-aiobotocore-pipes-2.5.4/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-pipes.svg?color=blue)](https://pypi.org/project/types-aiobotocore-pipes)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_pipes/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-pipes)](https://pepy.tech/project/types-aiobotocore-pipes)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.EventBridgePipes 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pipes.html#EventBridgePipes)
+[aiobotocore.EventBridgePipes 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pipes.html#EventBridgePipes)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-pipes-2.5.2.post2/setup.py` & `types-aiobotocore-pipes-2.5.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-pipes",
-    version="2.5.2.post2",
+    version="2.5.4",
     packages=["types_aiobotocore_pipes"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.EventBridgePipes 2.5.2 service generated with"
+        "Type annotations for aiobotocore.EventBridgePipes 2.5.4 service generated with"
         " mypy-boto3-builder 7.17.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
```

### Comparing `types-aiobotocore-pipes-2.5.2.post2/types_aiobotocore_pipes/__init__.py` & `types-aiobotocore-pipes-2.5.4/types_aiobotocore_pipes/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-pipes-2.5.2.post2/types_aiobotocore_pipes/__init__.pyi` & `types-aiobotocore-pipes-2.5.4/types_aiobotocore_pipes/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-pipes-2.5.2.post2/types_aiobotocore_pipes/__main__.py` & `types-aiobotocore-pipes-2.5.4/types_aiobotocore_pipes/__main__.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.EventBridgePipes 2.5.2\nVersion:        "
-        " 2.5.2.post2\nBuilder version: 7.17.2\nDocs:           "
+        "Type annotations for aiobotocore.EventBridgePipes 2.5.4\nVersion:         2.5.4\nBuilder"
+        " version: 7.17.2\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_pipes//\nBoto3 docs:  "
         "    https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pipes.html#EventBridgePipes\nOther"
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

### Comparing `types-aiobotocore-pipes-2.5.2.post2/types_aiobotocore_pipes/client.py` & `types-aiobotocore-pipes-2.5.4/types_aiobotocore_pipes/client.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-pipes-2.5.2.post2/types_aiobotocore_pipes/client.pyi` & `types-aiobotocore-pipes-2.5.4/types_aiobotocore_pipes/client.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-pipes-2.5.2.post2/types_aiobotocore_pipes/literals.py` & `types-aiobotocore-pipes-2.5.4/types_aiobotocore_pipes/literals.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-pipes-2.5.2.post2/types_aiobotocore_pipes/literals.pyi` & `types-aiobotocore-pipes-2.5.4/types_aiobotocore_pipes/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-pipes-2.5.2.post2/types_aiobotocore_pipes/paginator.py` & `types-aiobotocore-pipes-2.5.4/types_aiobotocore_pipes/paginator.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-pipes-2.5.2.post2/types_aiobotocore_pipes/paginator.pyi` & `types-aiobotocore-pipes-2.5.4/types_aiobotocore_pipes/paginator.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-pipes-2.5.2.post2/types_aiobotocore_pipes/type_defs.py` & `types-aiobotocore-pipes-2.5.4/types_aiobotocore_pipes/type_defs.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-pipes-2.5.2.post2/types_aiobotocore_pipes/type_defs.pyi` & `types-aiobotocore-pipes-2.5.4/types_aiobotocore_pipes/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-pipes-2.5.2.post2/types_aiobotocore_pipes.egg-info/PKG-INFO` & `types-aiobotocore-pipes-2.5.4/types_aiobotocore_pipes.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-pipes
-Version: 2.5.2.post2
-Summary: Type annotations for aiobotocore.EventBridgePipes 2.5.2 service generated with mypy-boto3-builder 7.17.2
+Version: 2.5.4
+Summary: Type annotations for aiobotocore.EventBridgePipes 2.5.4 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_pipes/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-pipes.svg?color=blue)](https://pypi.org/project/types-aiobotocore-pipes)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_pipes/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-pipes)](https://pepy.tech/project/types-aiobotocore-pipes)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.EventBridgePipes 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pipes.html#EventBridgePipes)
+[aiobotocore.EventBridgePipes 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pipes.html#EventBridgePipes)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-pipes-2.5.2.post2/types_aiobotocore_pipes.egg-info/SOURCES.txt` & `types-aiobotocore-pipes-2.5.4/types_aiobotocore_pipes.egg-info/SOURCES.txt`

 * *Files identical despite different names*


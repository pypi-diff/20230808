# Comparing `tmp/types-aiobotocore-serverlessrepo-2.5.2.post2.tar.gz` & `tmp/types-aiobotocore-serverlessrepo-2.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-serverlessrepo-2.5.2.post2.tar", last modified: Fri Aug  4 13:59:25 2023, max compression
+gzip compressed data, was "types-aiobotocore-serverlessrepo-2.5.4.tar", last modified: Tue Aug  8 01:24:25 2023, max compression
```

## Comparing `types-aiobotocore-serverlessrepo-2.5.2.post2.tar` & `types-aiobotocore-serverlessrepo-2.5.4.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:25.906643 types-aiobotocore-serverlessrepo-2.5.2.post2/
--rw-r--r--   0 vlad      (1000) vlad      (1000)     1070 2023-08-04 13:53:10.000000 types-aiobotocore-serverlessrepo-2.5.2.post2/LICENSE
--rw-r--r--   0 vlad      (1000) vlad      (1000)    13924 2023-08-04 13:59:25.906643 types-aiobotocore-serverlessrepo-2.5.2.post2/PKG-INFO
--rw-r--r--   0 vlad      (1000) vlad      (1000)    12361 2023-08-04 13:53:10.000000 types-aiobotocore-serverlessrepo-2.5.2.post2/README.md
--rw-r--r--   0 vlad      (1000) vlad      (1000)       38 2023-08-04 13:59:25.906643 types-aiobotocore-serverlessrepo-2.5.2.post2/setup.cfg
--rw-r--r--   0 vlad      (1000) vlad      (1000)     2138 2023-08-04 13:53:09.000000 types-aiobotocore-serverlessrepo-2.5.2.post2/setup.py
-drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:25.906643 types-aiobotocore-serverlessrepo-2.5.2.post2/types_aiobotocore_serverlessrepo/
--rw-r--r--   0 vlad      (1000) vlad      (1000)     1340 2023-08-04 13:53:10.000000 types-aiobotocore-serverlessrepo-2.5.2.post2/types_aiobotocore_serverlessrepo/__init__.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)     1339 2023-08-04 13:53:10.000000 types-aiobotocore-serverlessrepo-2.5.2.post2/types_aiobotocore_serverlessrepo/__init__.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)     1005 2023-08-04 13:53:10.000000 types-aiobotocore-serverlessrepo-2.5.2.post2/types_aiobotocore_serverlessrepo/__main__.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)    16558 2023-08-04 13:53:10.000000 types-aiobotocore-serverlessrepo-2.5.2.post2/types_aiobotocore_serverlessrepo/client.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)    16532 2023-08-04 13:53:10.000000 types-aiobotocore-serverlessrepo-2.5.2.post2/types_aiobotocore_serverlessrepo/client.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)     8783 2023-08-04 13:53:10.000000 types-aiobotocore-serverlessrepo-2.5.2.post2/types_aiobotocore_serverlessrepo/literals.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)     8781 2023-08-04 13:53:10.000000 types-aiobotocore-serverlessrepo-2.5.2.post2/types_aiobotocore_serverlessrepo/literals.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)     4817 2023-08-04 13:53:10.000000 types-aiobotocore-serverlessrepo-2.5.2.post2/types_aiobotocore_serverlessrepo/paginator.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)     4812 2023-08-04 13:53:10.000000 types-aiobotocore-serverlessrepo-2.5.2.post2/types_aiobotocore_serverlessrepo/paginator.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:53:10.000000 types-aiobotocore-serverlessrepo-2.5.2.post2/types_aiobotocore_serverlessrepo/py.typed
--rw-r--r--   0 vlad      (1000) vlad      (1000)    19293 2023-08-04 13:53:14.000000 types-aiobotocore-serverlessrepo-2.5.2.post2/types_aiobotocore_serverlessrepo/type_defs.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)    19263 2023-08-04 13:53:10.000000 types-aiobotocore-serverlessrepo-2.5.2.post2/types_aiobotocore_serverlessrepo/type_defs.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)       65 2023-08-04 13:53:10.000000 types-aiobotocore-serverlessrepo-2.5.2.post2/types_aiobotocore_serverlessrepo/version.py
-drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:25.906643 types-aiobotocore-serverlessrepo-2.5.2.post2/types_aiobotocore_serverlessrepo.egg-info/
--rw-r--r--   0 vlad      (1000) vlad      (1000)    13924 2023-08-04 13:59:25.000000 types-aiobotocore-serverlessrepo-2.5.2.post2/types_aiobotocore_serverlessrepo.egg-info/PKG-INFO
--rw-r--r--   0 vlad      (1000) vlad      (1000)      946 2023-08-04 13:59:25.000000 types-aiobotocore-serverlessrepo-2.5.2.post2/types_aiobotocore_serverlessrepo.egg-info/SOURCES.txt
--rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:25.000000 types-aiobotocore-serverlessrepo-2.5.2.post2/types_aiobotocore_serverlessrepo.egg-info/dependency_links.txt
--rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:25.000000 types-aiobotocore-serverlessrepo-2.5.2.post2/types_aiobotocore_serverlessrepo.egg-info/not-zip-safe
--rw-r--r--   0 vlad      (1000) vlad      (1000)       52 2023-08-04 13:59:25.000000 types-aiobotocore-serverlessrepo-2.5.2.post2/types_aiobotocore_serverlessrepo.egg-info/requires.txt
--rw-r--r--   0 vlad      (1000) vlad      (1000)       33 2023-08-04 13:59:25.000000 types-aiobotocore-serverlessrepo-2.5.2.post2/types_aiobotocore_serverlessrepo.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:24:25.318778 types-aiobotocore-serverlessrepo-2.5.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-08 01:20:54.000000 types-aiobotocore-serverlessrepo-2.5.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    13918 2023-08-08 01:24:25.318778 types-aiobotocore-serverlessrepo-2.5.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    12361 2023-08-08 01:20:54.000000 types-aiobotocore-serverlessrepo-2.5.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-08 01:24:25.318778 types-aiobotocore-serverlessrepo-2.5.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2132 2023-08-08 01:20:54.000000 types-aiobotocore-serverlessrepo-2.5.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:24:25.318778 types-aiobotocore-serverlessrepo-2.5.4/types_aiobotocore_serverlessrepo/
+-rw-r--r--   0 runner    (1001) docker     (123)     1340 2023-08-08 01:20:54.000000 types-aiobotocore-serverlessrepo-2.5.4/types_aiobotocore_serverlessrepo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1339 2023-08-08 01:20:54.000000 types-aiobotocore-serverlessrepo-2.5.4/types_aiobotocore_serverlessrepo/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      993 2023-08-08 01:20:54.000000 types-aiobotocore-serverlessrepo-2.5.4/types_aiobotocore_serverlessrepo/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16558 2023-08-08 01:20:54.000000 types-aiobotocore-serverlessrepo-2.5.4/types_aiobotocore_serverlessrepo/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16532 2023-08-08 01:20:54.000000 types-aiobotocore-serverlessrepo-2.5.4/types_aiobotocore_serverlessrepo/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8783 2023-08-08 01:20:54.000000 types-aiobotocore-serverlessrepo-2.5.4/types_aiobotocore_serverlessrepo/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8781 2023-08-08 01:20:54.000000 types-aiobotocore-serverlessrepo-2.5.4/types_aiobotocore_serverlessrepo/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     4817 2023-08-08 01:20:54.000000 types-aiobotocore-serverlessrepo-2.5.4/types_aiobotocore_serverlessrepo/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4812 2023-08-08 01:20:54.000000 types-aiobotocore-serverlessrepo-2.5.4/types_aiobotocore_serverlessrepo/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 01:20:54.000000 types-aiobotocore-serverlessrepo-2.5.4/types_aiobotocore_serverlessrepo/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    19293 2023-08-08 01:20:55.000000 types-aiobotocore-serverlessrepo-2.5.4/types_aiobotocore_serverlessrepo/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19263 2023-08-08 01:20:55.000000 types-aiobotocore-serverlessrepo-2.5.4/types_aiobotocore_serverlessrepo/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-08-08 01:20:54.000000 types-aiobotocore-serverlessrepo-2.5.4/types_aiobotocore_serverlessrepo/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:24:25.318778 types-aiobotocore-serverlessrepo-2.5.4/types_aiobotocore_serverlessrepo.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    13918 2023-08-08 01:24:25.000000 types-aiobotocore-serverlessrepo-2.5.4/types_aiobotocore_serverlessrepo.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      946 2023-08-08 01:24:25.000000 types-aiobotocore-serverlessrepo-2.5.4/types_aiobotocore_serverlessrepo.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 01:24:25.000000 types-aiobotocore-serverlessrepo-2.5.4/types_aiobotocore_serverlessrepo.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 01:24:25.000000 types-aiobotocore-serverlessrepo-2.5.4/types_aiobotocore_serverlessrepo.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-08 01:24:25.000000 types-aiobotocore-serverlessrepo-2.5.4/types_aiobotocore_serverlessrepo.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-08-08 01:24:25.000000 types-aiobotocore-serverlessrepo-2.5.4/types_aiobotocore_serverlessrepo.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-serverlessrepo-2.5.2.post2/LICENSE` & `types-aiobotocore-serverlessrepo-2.5.4/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-serverlessrepo-2.5.2.post2/PKG-INFO` & `types-aiobotocore-serverlessrepo-2.5.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-serverlessrepo
-Version: 2.5.2.post2
-Summary: Type annotations for aiobotocore.ServerlessApplicationRepository 2.5.2 service generated with mypy-boto3-builder 7.17.2
+Version: 2.5.4
+Summary: Type annotations for aiobotocore.ServerlessApplicationRepository 2.5.4 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_serverlessrepo/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-serverlessrepo.svg?color=blue)](https://pypi.org/project/types-aiobotocore-serverlessrepo)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_serverlessrepo/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-serverlessrepo)](https://pepy.tech/project/types-aiobotocore-serverlessrepo)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.ServerlessApplicationRepository 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/serverlessrepo.html#ServerlessApplicationRepository)
+[aiobotocore.ServerlessApplicationRepository 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/serverlessrepo.html#ServerlessApplicationRepository)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-serverlessrepo-2.5.2.post2/README.md` & `types-aiobotocore-serverlessrepo-2.5.4/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-serverlessrepo.svg?color=blue)](https://pypi.org/project/types-aiobotocore-serverlessrepo)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_serverlessrepo/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-serverlessrepo)](https://pepy.tech/project/types-aiobotocore-serverlessrepo)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.ServerlessApplicationRepository 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/serverlessrepo.html#ServerlessApplicationRepository)
+[aiobotocore.ServerlessApplicationRepository 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/serverlessrepo.html#ServerlessApplicationRepository)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-serverlessrepo-2.5.2.post2/setup.py` & `types-aiobotocore-serverlessrepo-2.5.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-serverlessrepo",
-    version="2.5.2.post2",
+    version="2.5.4",
     packages=["types_aiobotocore_serverlessrepo"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.ServerlessApplicationRepository 2.5.2 service generated"
+        "Type annotations for aiobotocore.ServerlessApplicationRepository 2.5.4 service generated"
         " with mypy-boto3-builder 7.17.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
```

### Comparing `types-aiobotocore-serverlessrepo-2.5.2.post2/types_aiobotocore_serverlessrepo/__init__.py` & `types-aiobotocore-serverlessrepo-2.5.4/types_aiobotocore_serverlessrepo/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-serverlessrepo-2.5.2.post2/types_aiobotocore_serverlessrepo/__init__.pyi` & `types-aiobotocore-serverlessrepo-2.5.4/types_aiobotocore_serverlessrepo/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-serverlessrepo-2.5.2.post2/types_aiobotocore_serverlessrepo/__main__.py` & `types-aiobotocore-serverlessrepo-2.5.4/types_aiobotocore_serverlessrepo/__main__.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.ServerlessApplicationRepository 2.5.2\nVersion:        "
-        " 2.5.2.post2\nBuilder version: 7.17.2\nDocs:           "
+        "Type annotations for aiobotocore.ServerlessApplicationRepository 2.5.4\nVersion:        "
+        " 2.5.4\nBuilder version: 7.17.2\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_serverlessrepo//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/serverlessrepo.html#ServerlessApplicationRepository\nOther"
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

### Comparing `types-aiobotocore-serverlessrepo-2.5.2.post2/types_aiobotocore_serverlessrepo/client.py` & `types-aiobotocore-serverlessrepo-2.5.4/types_aiobotocore_serverlessrepo/client.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-serverlessrepo-2.5.2.post2/types_aiobotocore_serverlessrepo/client.pyi` & `types-aiobotocore-serverlessrepo-2.5.4/types_aiobotocore_serverlessrepo/client.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-serverlessrepo-2.5.2.post2/types_aiobotocore_serverlessrepo/literals.py` & `types-aiobotocore-serverlessrepo-2.5.4/types_aiobotocore_serverlessrepo/literals.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-serverlessrepo-2.5.2.post2/types_aiobotocore_serverlessrepo/literals.pyi` & `types-aiobotocore-serverlessrepo-2.5.4/types_aiobotocore_serverlessrepo/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-serverlessrepo-2.5.2.post2/types_aiobotocore_serverlessrepo/paginator.py` & `types-aiobotocore-serverlessrepo-2.5.4/types_aiobotocore_serverlessrepo/paginator.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-serverlessrepo-2.5.2.post2/types_aiobotocore_serverlessrepo/paginator.pyi` & `types-aiobotocore-serverlessrepo-2.5.4/types_aiobotocore_serverlessrepo/paginator.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-serverlessrepo-2.5.2.post2/types_aiobotocore_serverlessrepo/type_defs.py` & `types-aiobotocore-serverlessrepo-2.5.4/types_aiobotocore_serverlessrepo/type_defs.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-serverlessrepo-2.5.2.post2/types_aiobotocore_serverlessrepo/type_defs.pyi` & `types-aiobotocore-serverlessrepo-2.5.4/types_aiobotocore_serverlessrepo/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-serverlessrepo-2.5.2.post2/types_aiobotocore_serverlessrepo.egg-info/PKG-INFO` & `types-aiobotocore-serverlessrepo-2.5.4/types_aiobotocore_serverlessrepo.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-serverlessrepo
-Version: 2.5.2.post2
-Summary: Type annotations for aiobotocore.ServerlessApplicationRepository 2.5.2 service generated with mypy-boto3-builder 7.17.2
+Version: 2.5.4
+Summary: Type annotations for aiobotocore.ServerlessApplicationRepository 2.5.4 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_serverlessrepo/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-serverlessrepo.svg?color=blue)](https://pypi.org/project/types-aiobotocore-serverlessrepo)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_serverlessrepo/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-serverlessrepo)](https://pepy.tech/project/types-aiobotocore-serverlessrepo)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.ServerlessApplicationRepository 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/serverlessrepo.html#ServerlessApplicationRepository)
+[aiobotocore.ServerlessApplicationRepository 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/serverlessrepo.html#ServerlessApplicationRepository)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-serverlessrepo-2.5.2.post2/types_aiobotocore_serverlessrepo.egg-info/SOURCES.txt` & `types-aiobotocore-serverlessrepo-2.5.4/types_aiobotocore_serverlessrepo.egg-info/SOURCES.txt`

 * *Files identical despite different names*


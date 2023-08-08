# Comparing `tmp/types-aiobotocore-privatenetworks-2.5.2.post2.tar.gz` & `tmp/types-aiobotocore-privatenetworks-2.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-privatenetworks-2.5.2.post2.tar", last modified: Fri Aug  4 13:59:21 2023, max compression
+gzip compressed data, was "types-aiobotocore-privatenetworks-2.5.4.tar", last modified: Tue Aug  8 01:24:15 2023, max compression
```

## Comparing `types-aiobotocore-privatenetworks-2.5.2.post2.tar` & `types-aiobotocore-privatenetworks-2.5.4.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:21.886643 types-aiobotocore-privatenetworks-2.5.2.post2/
--rw-r--r--   0 vlad      (1000) vlad      (1000)     1070 2023-08-04 13:47:10.000000 types-aiobotocore-privatenetworks-2.5.2.post2/LICENSE
--rw-r--r--   0 vlad      (1000) vlad      (1000)    13960 2023-08-04 13:59:21.886643 types-aiobotocore-privatenetworks-2.5.2.post2/PKG-INFO
--rw-r--r--   0 vlad      (1000) vlad      (1000)    12416 2023-08-04 13:47:10.000000 types-aiobotocore-privatenetworks-2.5.2.post2/README.md
--rw-r--r--   0 vlad      (1000) vlad      (1000)       38 2023-08-04 13:59:21.886643 types-aiobotocore-privatenetworks-2.5.2.post2/setup.cfg
--rw-r--r--   0 vlad      (1000) vlad      (1000)     2122 2023-08-04 13:47:10.000000 types-aiobotocore-privatenetworks-2.5.2.post2/setup.py
-drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:21.886643 types-aiobotocore-privatenetworks-2.5.2.post2/types_aiobotocore_privatenetworks/
--rw-r--r--   0 vlad      (1000) vlad      (1000)     1525 2023-08-04 13:47:10.000000 types-aiobotocore-privatenetworks-2.5.2.post2/types_aiobotocore_privatenetworks/__init__.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)     1524 2023-08-04 13:47:10.000000 types-aiobotocore-privatenetworks-2.5.2.post2/types_aiobotocore_privatenetworks/__init__.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)      963 2023-08-04 13:47:10.000000 types-aiobotocore-privatenetworks-2.5.2.post2/types_aiobotocore_privatenetworks/__main__.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)    23100 2023-08-04 13:47:10.000000 types-aiobotocore-privatenetworks-2.5.2.post2/types_aiobotocore_privatenetworks/client.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)    23060 2023-08-04 13:47:10.000000 types-aiobotocore-privatenetworks-2.5.2.post2/types_aiobotocore_privatenetworks/client.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)    10088 2023-08-04 13:47:10.000000 types-aiobotocore-privatenetworks-2.5.2.post2/types_aiobotocore_privatenetworks/literals.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)    10086 2023-08-04 13:47:10.000000 types-aiobotocore-privatenetworks-2.5.2.post2/types_aiobotocore_privatenetworks/literals.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)     7369 2023-08-04 13:47:10.000000 types-aiobotocore-privatenetworks-2.5.2.post2/types_aiobotocore_privatenetworks/paginator.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)     7361 2023-08-04 13:47:10.000000 types-aiobotocore-privatenetworks-2.5.2.post2/types_aiobotocore_privatenetworks/paginator.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:47:10.000000 types-aiobotocore-privatenetworks-2.5.2.post2/types_aiobotocore_privatenetworks/py.typed
--rw-r--r--   0 vlad      (1000) vlad      (1000)    28972 2023-08-04 13:47:11.000000 types-aiobotocore-privatenetworks-2.5.2.post2/types_aiobotocore_privatenetworks/type_defs.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)    28919 2023-08-04 13:47:11.000000 types-aiobotocore-privatenetworks-2.5.2.post2/types_aiobotocore_privatenetworks/type_defs.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)       65 2023-08-04 13:47:10.000000 types-aiobotocore-privatenetworks-2.5.2.post2/types_aiobotocore_privatenetworks/version.py
-drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:21.886643 types-aiobotocore-privatenetworks-2.5.2.post2/types_aiobotocore_privatenetworks.egg-info/
--rw-r--r--   0 vlad      (1000) vlad      (1000)    13960 2023-08-04 13:59:21.000000 types-aiobotocore-privatenetworks-2.5.2.post2/types_aiobotocore_privatenetworks.egg-info/PKG-INFO
--rw-r--r--   0 vlad      (1000) vlad      (1000)      965 2023-08-04 13:59:21.000000 types-aiobotocore-privatenetworks-2.5.2.post2/types_aiobotocore_privatenetworks.egg-info/SOURCES.txt
--rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:21.000000 types-aiobotocore-privatenetworks-2.5.2.post2/types_aiobotocore_privatenetworks.egg-info/dependency_links.txt
--rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:21.000000 types-aiobotocore-privatenetworks-2.5.2.post2/types_aiobotocore_privatenetworks.egg-info/not-zip-safe
--rw-r--r--   0 vlad      (1000) vlad      (1000)       52 2023-08-04 13:59:21.000000 types-aiobotocore-privatenetworks-2.5.2.post2/types_aiobotocore_privatenetworks.egg-info/requires.txt
--rw-r--r--   0 vlad      (1000) vlad      (1000)       34 2023-08-04 13:59:21.000000 types-aiobotocore-privatenetworks-2.5.2.post2/types_aiobotocore_privatenetworks.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:24:15.598754 types-aiobotocore-privatenetworks-2.5.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-08 01:16:52.000000 types-aiobotocore-privatenetworks-2.5.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    13954 2023-08-08 01:24:15.598754 types-aiobotocore-privatenetworks-2.5.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    12416 2023-08-08 01:16:52.000000 types-aiobotocore-privatenetworks-2.5.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-08 01:24:15.598754 types-aiobotocore-privatenetworks-2.5.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2116 2023-08-08 01:16:52.000000 types-aiobotocore-privatenetworks-2.5.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:24:15.594754 types-aiobotocore-privatenetworks-2.5.4/types_aiobotocore_privatenetworks/
+-rw-r--r--   0 runner    (1001) docker     (123)     1525 2023-08-08 01:16:52.000000 types-aiobotocore-privatenetworks-2.5.4/types_aiobotocore_privatenetworks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1524 2023-08-08 01:16:52.000000 types-aiobotocore-privatenetworks-2.5.4/types_aiobotocore_privatenetworks/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      951 2023-08-08 01:16:52.000000 types-aiobotocore-privatenetworks-2.5.4/types_aiobotocore_privatenetworks/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23100 2023-08-08 01:16:52.000000 types-aiobotocore-privatenetworks-2.5.4/types_aiobotocore_privatenetworks/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23060 2023-08-08 01:16:52.000000 types-aiobotocore-privatenetworks-2.5.4/types_aiobotocore_privatenetworks/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    10088 2023-08-08 01:16:52.000000 types-aiobotocore-privatenetworks-2.5.4/types_aiobotocore_privatenetworks/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10086 2023-08-08 01:16:52.000000 types-aiobotocore-privatenetworks-2.5.4/types_aiobotocore_privatenetworks/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     7369 2023-08-08 01:16:52.000000 types-aiobotocore-privatenetworks-2.5.4/types_aiobotocore_privatenetworks/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7361 2023-08-08 01:16:52.000000 types-aiobotocore-privatenetworks-2.5.4/types_aiobotocore_privatenetworks/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 01:16:52.000000 types-aiobotocore-privatenetworks-2.5.4/types_aiobotocore_privatenetworks/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    28972 2023-08-08 01:16:53.000000 types-aiobotocore-privatenetworks-2.5.4/types_aiobotocore_privatenetworks/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28919 2023-08-08 01:16:53.000000 types-aiobotocore-privatenetworks-2.5.4/types_aiobotocore_privatenetworks/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-08-08 01:16:52.000000 types-aiobotocore-privatenetworks-2.5.4/types_aiobotocore_privatenetworks/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:24:15.598754 types-aiobotocore-privatenetworks-2.5.4/types_aiobotocore_privatenetworks.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    13954 2023-08-08 01:24:15.000000 types-aiobotocore-privatenetworks-2.5.4/types_aiobotocore_privatenetworks.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      965 2023-08-08 01:24:15.000000 types-aiobotocore-privatenetworks-2.5.4/types_aiobotocore_privatenetworks.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 01:24:15.000000 types-aiobotocore-privatenetworks-2.5.4/types_aiobotocore_privatenetworks.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 01:24:15.000000 types-aiobotocore-privatenetworks-2.5.4/types_aiobotocore_privatenetworks.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-08 01:24:15.000000 types-aiobotocore-privatenetworks-2.5.4/types_aiobotocore_privatenetworks.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-08-08 01:24:15.000000 types-aiobotocore-privatenetworks-2.5.4/types_aiobotocore_privatenetworks.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-privatenetworks-2.5.2.post2/LICENSE` & `types-aiobotocore-privatenetworks-2.5.4/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-privatenetworks-2.5.2.post2/PKG-INFO` & `types-aiobotocore-privatenetworks-2.5.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-privatenetworks
-Version: 2.5.2.post2
-Summary: Type annotations for aiobotocore.Private5G 2.5.2 service generated with mypy-boto3-builder 7.17.2
+Version: 2.5.4
+Summary: Type annotations for aiobotocore.Private5G 2.5.4 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_privatenetworks/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-privatenetworks.svg?color=blue)](https://pypi.org/project/types-aiobotocore-privatenetworks)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_privatenetworks/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-privatenetworks)](https://pepy.tech/project/types-aiobotocore-privatenetworks)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.Private5G 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/privatenetworks.html#Private5G)
+[aiobotocore.Private5G 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/privatenetworks.html#Private5G)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-privatenetworks-2.5.2.post2/README.md` & `types-aiobotocore-privatenetworks-2.5.4/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-privatenetworks.svg?color=blue)](https://pypi.org/project/types-aiobotocore-privatenetworks)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_privatenetworks/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-privatenetworks)](https://pepy.tech/project/types-aiobotocore-privatenetworks)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.Private5G 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/privatenetworks.html#Private5G)
+[aiobotocore.Private5G 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/privatenetworks.html#Private5G)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-privatenetworks-2.5.2.post2/setup.py` & `types-aiobotocore-privatenetworks-2.5.4/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-privatenetworks",
-    version="2.5.2.post2",
+    version="2.5.4",
     packages=["types_aiobotocore_privatenetworks"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.Private5G 2.5.2 service generated with mypy-boto3-builder"
+        "Type annotations for aiobotocore.Private5G 2.5.4 service generated with mypy-boto3-builder"
         " 7.17.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
```

### Comparing `types-aiobotocore-privatenetworks-2.5.2.post2/types_aiobotocore_privatenetworks/__init__.py` & `types-aiobotocore-privatenetworks-2.5.4/types_aiobotocore_privatenetworks/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-privatenetworks-2.5.2.post2/types_aiobotocore_privatenetworks/__init__.pyi` & `types-aiobotocore-privatenetworks-2.5.4/types_aiobotocore_privatenetworks/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-privatenetworks-2.5.2.post2/types_aiobotocore_privatenetworks/__main__.py` & `types-aiobotocore-privatenetworks-2.5.4/types_aiobotocore_privatenetworks/__main__.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.Private5G 2.5.2\nVersion:         2.5.2.post2\nBuilder"
-        " version: 7.17.2\nDocs:           "
+        "Type annotations for aiobotocore.Private5G 2.5.4\nVersion:         2.5.4\nBuilder version:"
+        " 7.17.2\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_privatenetworks//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/privatenetworks.html#Private5G\nOther"
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

### Comparing `types-aiobotocore-privatenetworks-2.5.2.post2/types_aiobotocore_privatenetworks/client.py` & `types-aiobotocore-privatenetworks-2.5.4/types_aiobotocore_privatenetworks/client.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-privatenetworks-2.5.2.post2/types_aiobotocore_privatenetworks/client.pyi` & `types-aiobotocore-privatenetworks-2.5.4/types_aiobotocore_privatenetworks/client.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-privatenetworks-2.5.2.post2/types_aiobotocore_privatenetworks/literals.py` & `types-aiobotocore-privatenetworks-2.5.4/types_aiobotocore_privatenetworks/literals.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-privatenetworks-2.5.2.post2/types_aiobotocore_privatenetworks/literals.pyi` & `types-aiobotocore-privatenetworks-2.5.4/types_aiobotocore_privatenetworks/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-privatenetworks-2.5.2.post2/types_aiobotocore_privatenetworks/paginator.py` & `types-aiobotocore-privatenetworks-2.5.4/types_aiobotocore_privatenetworks/paginator.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-privatenetworks-2.5.2.post2/types_aiobotocore_privatenetworks/paginator.pyi` & `types-aiobotocore-privatenetworks-2.5.4/types_aiobotocore_privatenetworks/paginator.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-privatenetworks-2.5.2.post2/types_aiobotocore_privatenetworks/type_defs.py` & `types-aiobotocore-privatenetworks-2.5.4/types_aiobotocore_privatenetworks/type_defs.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-privatenetworks-2.5.2.post2/types_aiobotocore_privatenetworks/type_defs.pyi` & `types-aiobotocore-privatenetworks-2.5.4/types_aiobotocore_privatenetworks/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-privatenetworks-2.5.2.post2/types_aiobotocore_privatenetworks.egg-info/PKG-INFO` & `types-aiobotocore-privatenetworks-2.5.4/types_aiobotocore_privatenetworks.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-privatenetworks
-Version: 2.5.2.post2
-Summary: Type annotations for aiobotocore.Private5G 2.5.2 service generated with mypy-boto3-builder 7.17.2
+Version: 2.5.4
+Summary: Type annotations for aiobotocore.Private5G 2.5.4 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_privatenetworks/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-privatenetworks.svg?color=blue)](https://pypi.org/project/types-aiobotocore-privatenetworks)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_privatenetworks/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-privatenetworks)](https://pepy.tech/project/types-aiobotocore-privatenetworks)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.Private5G 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/privatenetworks.html#Private5G)
+[aiobotocore.Private5G 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/privatenetworks.html#Private5G)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-privatenetworks-2.5.2.post2/types_aiobotocore_privatenetworks.egg-info/SOURCES.txt` & `types-aiobotocore-privatenetworks-2.5.4/types_aiobotocore_privatenetworks.egg-info/SOURCES.txt`

 * *Files identical despite different names*


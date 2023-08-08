# Comparing `tmp/types-aiobotocore-proton-2.5.2.post2.tar.gz` & `tmp/types-aiobotocore-proton-2.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-proton-2.5.2.post2.tar", last modified: Fri Aug  4 13:59:21 2023, max compression
+gzip compressed data, was "types-aiobotocore-proton-2.5.4.tar", last modified: Tue Aug  8 01:24:15 2023, max compression
```

## Comparing `types-aiobotocore-proton-2.5.2.post2.tar` & `types-aiobotocore-proton-2.5.4.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:21.946643 types-aiobotocore-proton-2.5.2.post2/
--rw-r--r--   0 vlad      (1000) vlad      (1000)     1070 2023-08-04 13:47:13.000000 types-aiobotocore-proton-2.5.2.post2/LICENSE
--rw-r--r--   0 vlad      (1000) vlad      (1000)    18715 2023-08-04 13:59:21.946643 types-aiobotocore-proton-2.5.2.post2/PKG-INFO
--rw-r--r--   0 vlad      (1000) vlad      (1000)    17201 2023-08-04 13:47:13.000000 types-aiobotocore-proton-2.5.2.post2/README.md
--rw-r--r--   0 vlad      (1000) vlad      (1000)       38 2023-08-04 13:59:21.946643 types-aiobotocore-proton-2.5.2.post2/setup.cfg
--rw-r--r--   0 vlad      (1000) vlad      (1000)     2065 2023-08-04 13:47:13.000000 types-aiobotocore-proton-2.5.2.post2/setup.py
-drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:21.936643 types-aiobotocore-proton-2.5.2.post2/types_aiobotocore_proton/
--rw-r--r--   0 vlad      (1000) vlad      (1000)     8018 2023-08-04 13:47:13.000000 types-aiobotocore-proton-2.5.2.post2/types_aiobotocore_proton/__init__.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)     8017 2023-08-04 13:47:13.000000 types-aiobotocore-proton-2.5.2.post2/types_aiobotocore_proton/__init__.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)      928 2023-08-04 13:47:13.000000 types-aiobotocore-proton-2.5.2.post2/types_aiobotocore_proton/__main__.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)    78108 2023-08-04 13:47:14.000000 types-aiobotocore-proton-2.5.2.post2/types_aiobotocore_proton/client.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)    77981 2023-08-04 13:47:13.000000 types-aiobotocore-proton-2.5.2.post2/types_aiobotocore_proton/client.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)    15953 2023-08-04 13:47:16.000000 types-aiobotocore-proton-2.5.2.post2/types_aiobotocore_proton/literals.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)    15951 2023-08-04 13:47:14.000000 types-aiobotocore-proton-2.5.2.post2/types_aiobotocore_proton/literals.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)    27543 2023-08-04 13:47:14.000000 types-aiobotocore-proton-2.5.2.post2/types_aiobotocore_proton/paginator.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)    27520 2023-08-04 13:47:14.000000 types-aiobotocore-proton-2.5.2.post2/types_aiobotocore_proton/paginator.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:47:13.000000 types-aiobotocore-proton-2.5.2.post2/types_aiobotocore_proton/py.typed
--rw-r--r--   0 vlad      (1000) vlad      (1000)   112775 2023-08-04 13:47:19.000000 types-aiobotocore-proton-2.5.2.post2/types_aiobotocore_proton/type_defs.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)   112590 2023-08-04 13:47:17.000000 types-aiobotocore-proton-2.5.2.post2/types_aiobotocore_proton/type_defs.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)       65 2023-08-04 13:47:13.000000 types-aiobotocore-proton-2.5.2.post2/types_aiobotocore_proton/version.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)    10765 2023-08-04 13:47:14.000000 types-aiobotocore-proton-2.5.2.post2/types_aiobotocore_proton/waiter.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)    10755 2023-08-04 13:47:14.000000 types-aiobotocore-proton-2.5.2.post2/types_aiobotocore_proton/waiter.pyi
-drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:21.946643 types-aiobotocore-proton-2.5.2.post2/types_aiobotocore_proton.egg-info/
--rw-r--r--   0 vlad      (1000) vlad      (1000)    18715 2023-08-04 13:59:21.000000 types-aiobotocore-proton-2.5.2.post2/types_aiobotocore_proton.egg-info/PKG-INFO
--rw-r--r--   0 vlad      (1000) vlad      (1000)      865 2023-08-04 13:59:21.000000 types-aiobotocore-proton-2.5.2.post2/types_aiobotocore_proton.egg-info/SOURCES.txt
--rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:21.000000 types-aiobotocore-proton-2.5.2.post2/types_aiobotocore_proton.egg-info/dependency_links.txt
--rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:21.000000 types-aiobotocore-proton-2.5.2.post2/types_aiobotocore_proton.egg-info/not-zip-safe
--rw-r--r--   0 vlad      (1000) vlad      (1000)       52 2023-08-04 13:59:21.000000 types-aiobotocore-proton-2.5.2.post2/types_aiobotocore_proton.egg-info/requires.txt
--rw-r--r--   0 vlad      (1000) vlad      (1000)       25 2023-08-04 13:59:21.000000 types-aiobotocore-proton-2.5.2.post2/types_aiobotocore_proton.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:24:15.750754 types-aiobotocore-proton-2.5.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-08 01:16:56.000000 types-aiobotocore-proton-2.5.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    18709 2023-08-08 01:24:15.750754 types-aiobotocore-proton-2.5.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    17201 2023-08-08 01:16:56.000000 types-aiobotocore-proton-2.5.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-08 01:24:15.750754 types-aiobotocore-proton-2.5.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2059 2023-08-08 01:16:56.000000 types-aiobotocore-proton-2.5.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:24:15.738754 types-aiobotocore-proton-2.5.4/types_aiobotocore_proton/
+-rw-r--r--   0 runner    (1001) docker     (123)     8018 2023-08-08 01:16:56.000000 types-aiobotocore-proton-2.5.4/types_aiobotocore_proton/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8017 2023-08-08 01:16:56.000000 types-aiobotocore-proton-2.5.4/types_aiobotocore_proton/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      916 2023-08-08 01:16:56.000000 types-aiobotocore-proton-2.5.4/types_aiobotocore_proton/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    78108 2023-08-08 01:16:56.000000 types-aiobotocore-proton-2.5.4/types_aiobotocore_proton/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    77981 2023-08-08 01:16:56.000000 types-aiobotocore-proton-2.5.4/types_aiobotocore_proton/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    15953 2023-08-08 01:16:57.000000 types-aiobotocore-proton-2.5.4/types_aiobotocore_proton/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15951 2023-08-08 01:16:57.000000 types-aiobotocore-proton-2.5.4/types_aiobotocore_proton/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    27543 2023-08-08 01:16:57.000000 types-aiobotocore-proton-2.5.4/types_aiobotocore_proton/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27520 2023-08-08 01:16:57.000000 types-aiobotocore-proton-2.5.4/types_aiobotocore_proton/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 01:16:56.000000 types-aiobotocore-proton-2.5.4/types_aiobotocore_proton/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)   112775 2023-08-08 01:16:59.000000 types-aiobotocore-proton-2.5.4/types_aiobotocore_proton/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)   112590 2023-08-08 01:16:58.000000 types-aiobotocore-proton-2.5.4/types_aiobotocore_proton/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-08-08 01:16:56.000000 types-aiobotocore-proton-2.5.4/types_aiobotocore_proton/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10765 2023-08-08 01:16:57.000000 types-aiobotocore-proton-2.5.4/types_aiobotocore_proton/waiter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10755 2023-08-08 01:16:57.000000 types-aiobotocore-proton-2.5.4/types_aiobotocore_proton/waiter.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:24:15.750754 types-aiobotocore-proton-2.5.4/types_aiobotocore_proton.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    18709 2023-08-08 01:24:15.000000 types-aiobotocore-proton-2.5.4/types_aiobotocore_proton.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      865 2023-08-08 01:24:15.000000 types-aiobotocore-proton-2.5.4/types_aiobotocore_proton.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 01:24:15.000000 types-aiobotocore-proton-2.5.4/types_aiobotocore_proton.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 01:24:15.000000 types-aiobotocore-proton-2.5.4/types_aiobotocore_proton.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-08 01:24:15.000000 types-aiobotocore-proton-2.5.4/types_aiobotocore_proton.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-08-08 01:24:15.000000 types-aiobotocore-proton-2.5.4/types_aiobotocore_proton.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-proton-2.5.2.post2/LICENSE` & `types-aiobotocore-proton-2.5.4/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-proton-2.5.2.post2/PKG-INFO` & `types-aiobotocore-proton-2.5.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-proton
-Version: 2.5.2.post2
-Summary: Type annotations for aiobotocore.Proton 2.5.2 service generated with mypy-boto3-builder 7.17.2
+Version: 2.5.4
+Summary: Type annotations for aiobotocore.Proton 2.5.4 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_proton/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-proton.svg?color=blue)](https://pypi.org/project/types-aiobotocore-proton)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_proton/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-proton)](https://pepy.tech/project/types-aiobotocore-proton)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.Proton 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton)
+[aiobotocore.Proton 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-proton-2.5.2.post2/README.md` & `types-aiobotocore-proton-2.5.4/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-proton.svg?color=blue)](https://pypi.org/project/types-aiobotocore-proton)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_proton/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-proton)](https://pepy.tech/project/types-aiobotocore-proton)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.Proton 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton)
+[aiobotocore.Proton 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-proton-2.5.2.post2/setup.py` & `types-aiobotocore-proton-2.5.4/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-proton",
-    version="2.5.2.post2",
+    version="2.5.4",
     packages=["types_aiobotocore_proton"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.Proton 2.5.2 service generated with mypy-boto3-builder"
+        "Type annotations for aiobotocore.Proton 2.5.4 service generated with mypy-boto3-builder"
         " 7.17.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
```

### Comparing `types-aiobotocore-proton-2.5.2.post2/types_aiobotocore_proton/__init__.py` & `types-aiobotocore-proton-2.5.4/types_aiobotocore_proton/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-proton-2.5.2.post2/types_aiobotocore_proton/__init__.pyi` & `types-aiobotocore-proton-2.5.4/types_aiobotocore_proton/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-proton-2.5.2.post2/types_aiobotocore_proton/__main__.py` & `types-aiobotocore-proton-2.5.4/types_aiobotocore_proton/__main__.py`

 * *Files 17% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.Proton 2.5.2\nVersion:         2.5.2.post2\nBuilder"
-        " version: 7.17.2\nDocs:           "
+        "Type annotations for aiobotocore.Proton 2.5.4\nVersion:         2.5.4\nBuilder version:"
+        " 7.17.2\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_proton//\nBoto3 docs: "
         "     https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton\nOther"
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

### Comparing `types-aiobotocore-proton-2.5.2.post2/types_aiobotocore_proton/client.py` & `types-aiobotocore-proton-2.5.4/types_aiobotocore_proton/client.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-proton-2.5.2.post2/types_aiobotocore_proton/client.pyi` & `types-aiobotocore-proton-2.5.4/types_aiobotocore_proton/client.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-proton-2.5.2.post2/types_aiobotocore_proton/literals.py` & `types-aiobotocore-proton-2.5.4/types_aiobotocore_proton/literals.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-proton-2.5.2.post2/types_aiobotocore_proton/literals.pyi` & `types-aiobotocore-proton-2.5.4/types_aiobotocore_proton/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-proton-2.5.2.post2/types_aiobotocore_proton/paginator.py` & `types-aiobotocore-proton-2.5.4/types_aiobotocore_proton/paginator.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-proton-2.5.2.post2/types_aiobotocore_proton/paginator.pyi` & `types-aiobotocore-proton-2.5.4/types_aiobotocore_proton/paginator.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-proton-2.5.2.post2/types_aiobotocore_proton/type_defs.py` & `types-aiobotocore-proton-2.5.4/types_aiobotocore_proton/type_defs.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-proton-2.5.2.post2/types_aiobotocore_proton/type_defs.pyi` & `types-aiobotocore-proton-2.5.4/types_aiobotocore_proton/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-proton-2.5.2.post2/types_aiobotocore_proton/waiter.py` & `types-aiobotocore-proton-2.5.4/types_aiobotocore_proton/waiter.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-proton-2.5.2.post2/types_aiobotocore_proton/waiter.pyi` & `types-aiobotocore-proton-2.5.4/types_aiobotocore_proton/waiter.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-proton-2.5.2.post2/types_aiobotocore_proton.egg-info/PKG-INFO` & `types-aiobotocore-proton-2.5.4/types_aiobotocore_proton.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-proton
-Version: 2.5.2.post2
-Summary: Type annotations for aiobotocore.Proton 2.5.2 service generated with mypy-boto3-builder 7.17.2
+Version: 2.5.4
+Summary: Type annotations for aiobotocore.Proton 2.5.4 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_proton/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-proton.svg?color=blue)](https://pypi.org/project/types-aiobotocore-proton)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_proton/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-proton)](https://pepy.tech/project/types-aiobotocore-proton)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.Proton 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton)
+[aiobotocore.Proton 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-proton-2.5.2.post2/types_aiobotocore_proton.egg-info/SOURCES.txt` & `types-aiobotocore-proton-2.5.4/types_aiobotocore_proton.egg-info/SOURCES.txt`

 * *Files identical despite different names*


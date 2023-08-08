# Comparing `tmp/types-aiobotocore-redshift-serverless-2.5.2.post2.tar.gz` & `tmp/types-aiobotocore-redshift-serverless-2.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-redshift-serverless-2.5.2.post2.tar", last modified: Fri Aug  4 13:59:22 2023, max compression
+gzip compressed data, was "types-aiobotocore-redshift-serverless-2.5.4.tar", last modified: Tue Aug  8 01:24:18 2023, max compression
```

## Comparing `types-aiobotocore-redshift-serverless-2.5.2.post2.tar` & `types-aiobotocore-redshift-serverless-2.5.4.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:22.906643 types-aiobotocore-redshift-serverless-2.5.2.post2/
--rw-r--r--   0 vlad      (1000) vlad      (1000)     1070 2023-08-04 13:50:30.000000 types-aiobotocore-redshift-serverless-2.5.2.post2/LICENSE
--rw-r--r--   0 vlad      (1000) vlad      (1000)    14519 2023-08-04 13:59:22.906643 types-aiobotocore-redshift-serverless-2.5.2.post2/PKG-INFO
--rw-r--r--   0 vlad      (1000) vlad      (1000)    12954 2023-08-04 13:50:30.000000 types-aiobotocore-redshift-serverless-2.5.2.post2/README.md
--rw-r--r--   0 vlad      (1000) vlad      (1000)       38 2023-08-04 13:59:22.906643 types-aiobotocore-redshift-serverless-2.5.2.post2/setup.cfg
--rw-r--r--   0 vlad      (1000) vlad      (1000)     2131 2023-08-04 13:50:30.000000 types-aiobotocore-redshift-serverless-2.5.2.post2/setup.py
-drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:22.906643 types-aiobotocore-redshift-serverless-2.5.2.post2/types_aiobotocore_redshift_serverless/
--rw-r--r--   0 vlad      (1000) vlad      (1000)     2008 2023-08-04 13:50:30.000000 types-aiobotocore-redshift-serverless-2.5.2.post2/types_aiobotocore_redshift_serverless/__init__.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)     2007 2023-08-04 13:50:30.000000 types-aiobotocore-redshift-serverless-2.5.2.post2/types_aiobotocore_redshift_serverless/__init__.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)      989 2023-08-04 13:50:30.000000 types-aiobotocore-redshift-serverless-2.5.2.post2/types_aiobotocore_redshift_serverless/__main__.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)    35136 2023-08-04 13:50:30.000000 types-aiobotocore-redshift-serverless-2.5.2.post2/types_aiobotocore_redshift_serverless/client.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)    35080 2023-08-04 13:50:30.000000 types-aiobotocore-redshift-serverless-2.5.2.post2/types_aiobotocore_redshift_serverless/client.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)     9706 2023-08-04 13:50:31.000000 types-aiobotocore-redshift-serverless-2.5.2.post2/types_aiobotocore_redshift_serverless/literals.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)     9704 2023-08-04 13:50:31.000000 types-aiobotocore-redshift-serverless-2.5.2.post2/types_aiobotocore_redshift_serverless/literals.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)     9813 2023-08-04 13:50:30.000000 types-aiobotocore-redshift-serverless-2.5.2.post2/types_aiobotocore_redshift_serverless/paginator.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)     9804 2023-08-04 13:50:30.000000 types-aiobotocore-redshift-serverless-2.5.2.post2/types_aiobotocore_redshift_serverless/paginator.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:50:30.000000 types-aiobotocore-redshift-serverless-2.5.2.post2/types_aiobotocore_redshift_serverless/py.typed
--rw-r--r--   0 vlad      (1000) vlad      (1000)    33772 2023-08-04 13:50:32.000000 types-aiobotocore-redshift-serverless-2.5.2.post2/types_aiobotocore_redshift_serverless/type_defs.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)    33741 2023-08-04 13:50:31.000000 types-aiobotocore-redshift-serverless-2.5.2.post2/types_aiobotocore_redshift_serverless/type_defs.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)       65 2023-08-04 13:50:30.000000 types-aiobotocore-redshift-serverless-2.5.2.post2/types_aiobotocore_redshift_serverless/version.py
-drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:22.906643 types-aiobotocore-redshift-serverless-2.5.2.post2/types_aiobotocore_redshift_serverless.egg-info/
--rw-r--r--   0 vlad      (1000) vlad      (1000)    14519 2023-08-04 13:59:22.000000 types-aiobotocore-redshift-serverless-2.5.2.post2/types_aiobotocore_redshift_serverless.egg-info/PKG-INFO
--rw-r--r--   0 vlad      (1000) vlad      (1000)     1041 2023-08-04 13:59:22.000000 types-aiobotocore-redshift-serverless-2.5.2.post2/types_aiobotocore_redshift_serverless.egg-info/SOURCES.txt
--rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:22.000000 types-aiobotocore-redshift-serverless-2.5.2.post2/types_aiobotocore_redshift_serverless.egg-info/dependency_links.txt
--rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:22.000000 types-aiobotocore-redshift-serverless-2.5.2.post2/types_aiobotocore_redshift_serverless.egg-info/not-zip-safe
--rw-r--r--   0 vlad      (1000) vlad      (1000)       52 2023-08-04 13:59:22.000000 types-aiobotocore-redshift-serverless-2.5.2.post2/types_aiobotocore_redshift_serverless.egg-info/requires.txt
--rw-r--r--   0 vlad      (1000) vlad      (1000)       38 2023-08-04 13:59:22.000000 types-aiobotocore-redshift-serverless-2.5.2.post2/types_aiobotocore_redshift_serverless.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:24:18.014760 types-aiobotocore-redshift-serverless-2.5.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-08 01:19:15.000000 types-aiobotocore-redshift-serverless-2.5.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    14513 2023-08-08 01:24:18.010760 types-aiobotocore-redshift-serverless-2.5.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    12954 2023-08-08 01:19:15.000000 types-aiobotocore-redshift-serverless-2.5.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-08 01:24:18.014760 types-aiobotocore-redshift-serverless-2.5.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2125 2023-08-08 01:19:15.000000 types-aiobotocore-redshift-serverless-2.5.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:24:18.010760 types-aiobotocore-redshift-serverless-2.5.4/types_aiobotocore_redshift_serverless/
+-rw-r--r--   0 runner    (1001) docker     (123)     2008 2023-08-08 01:19:15.000000 types-aiobotocore-redshift-serverless-2.5.4/types_aiobotocore_redshift_serverless/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2007 2023-08-08 01:19:15.000000 types-aiobotocore-redshift-serverless-2.5.4/types_aiobotocore_redshift_serverless/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      977 2023-08-08 01:19:15.000000 types-aiobotocore-redshift-serverless-2.5.4/types_aiobotocore_redshift_serverless/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35136 2023-08-08 01:19:16.000000 types-aiobotocore-redshift-serverless-2.5.4/types_aiobotocore_redshift_serverless/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35080 2023-08-08 01:19:15.000000 types-aiobotocore-redshift-serverless-2.5.4/types_aiobotocore_redshift_serverless/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9706 2023-08-08 01:19:16.000000 types-aiobotocore-redshift-serverless-2.5.4/types_aiobotocore_redshift_serverless/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9704 2023-08-08 01:19:16.000000 types-aiobotocore-redshift-serverless-2.5.4/types_aiobotocore_redshift_serverless/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9813 2023-08-08 01:19:16.000000 types-aiobotocore-redshift-serverless-2.5.4/types_aiobotocore_redshift_serverless/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9804 2023-08-08 01:19:16.000000 types-aiobotocore-redshift-serverless-2.5.4/types_aiobotocore_redshift_serverless/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 01:19:15.000000 types-aiobotocore-redshift-serverless-2.5.4/types_aiobotocore_redshift_serverless/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    33772 2023-08-08 01:19:16.000000 types-aiobotocore-redshift-serverless-2.5.4/types_aiobotocore_redshift_serverless/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33741 2023-08-08 01:19:16.000000 types-aiobotocore-redshift-serverless-2.5.4/types_aiobotocore_redshift_serverless/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-08-08 01:19:15.000000 types-aiobotocore-redshift-serverless-2.5.4/types_aiobotocore_redshift_serverless/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:24:18.010760 types-aiobotocore-redshift-serverless-2.5.4/types_aiobotocore_redshift_serverless.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    14513 2023-08-08 01:24:17.000000 types-aiobotocore-redshift-serverless-2.5.4/types_aiobotocore_redshift_serverless.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1041 2023-08-08 01:24:17.000000 types-aiobotocore-redshift-serverless-2.5.4/types_aiobotocore_redshift_serverless.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 01:24:17.000000 types-aiobotocore-redshift-serverless-2.5.4/types_aiobotocore_redshift_serverless.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 01:24:17.000000 types-aiobotocore-redshift-serverless-2.5.4/types_aiobotocore_redshift_serverless.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-08 01:24:17.000000 types-aiobotocore-redshift-serverless-2.5.4/types_aiobotocore_redshift_serverless.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-08 01:24:17.000000 types-aiobotocore-redshift-serverless-2.5.4/types_aiobotocore_redshift_serverless.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-redshift-serverless-2.5.2.post2/LICENSE` & `types-aiobotocore-redshift-serverless-2.5.4/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-redshift-serverless-2.5.2.post2/PKG-INFO` & `types-aiobotocore-redshift-serverless-2.5.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-redshift-serverless
-Version: 2.5.2.post2
-Summary: Type annotations for aiobotocore.RedshiftServerless 2.5.2 service generated with mypy-boto3-builder 7.17.2
+Version: 2.5.4
+Summary: Type annotations for aiobotocore.RedshiftServerless 2.5.4 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift_serverless/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-redshift-serverless.svg?color=blue)](https://pypi.org/project/types-aiobotocore-redshift-serverless)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift_serverless/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-redshift-serverless)](https://pepy.tech/project/types-aiobotocore-redshift-serverless)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.RedshiftServerless 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift-serverless.html#RedshiftServerless)
+[aiobotocore.RedshiftServerless 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift-serverless.html#RedshiftServerless)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-redshift-serverless-2.5.2.post2/README.md` & `types-aiobotocore-redshift-serverless-2.5.4/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-redshift-serverless.svg?color=blue)](https://pypi.org/project/types-aiobotocore-redshift-serverless)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift_serverless/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-redshift-serverless)](https://pepy.tech/project/types-aiobotocore-redshift-serverless)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.RedshiftServerless 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift-serverless.html#RedshiftServerless)
+[aiobotocore.RedshiftServerless 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift-serverless.html#RedshiftServerless)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-redshift-serverless-2.5.2.post2/setup.py` & `types-aiobotocore-redshift-serverless-2.5.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-redshift-serverless",
-    version="2.5.2.post2",
+    version="2.5.4",
     packages=["types_aiobotocore_redshift_serverless"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.RedshiftServerless 2.5.2 service generated with"
+        "Type annotations for aiobotocore.RedshiftServerless 2.5.4 service generated with"
         " mypy-boto3-builder 7.17.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
```

### Comparing `types-aiobotocore-redshift-serverless-2.5.2.post2/types_aiobotocore_redshift_serverless/__init__.py` & `types-aiobotocore-redshift-serverless-2.5.4/types_aiobotocore_redshift_serverless/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-redshift-serverless-2.5.2.post2/types_aiobotocore_redshift_serverless/__init__.pyi` & `types-aiobotocore-redshift-serverless-2.5.4/types_aiobotocore_redshift_serverless/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-redshift-serverless-2.5.2.post2/types_aiobotocore_redshift_serverless/__main__.py` & `types-aiobotocore-redshift-serverless-2.5.4/types_aiobotocore_redshift_serverless/__main__.py`

 * *Files 13% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.RedshiftServerless 2.5.2\nVersion:        "
-        " 2.5.2.post2\nBuilder version: 7.17.2\nDocs:           "
+        "Type annotations for aiobotocore.RedshiftServerless 2.5.4\nVersion:         2.5.4\nBuilder"
+        " version: 7.17.2\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift_serverless//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift-serverless.html#RedshiftServerless\nOther"
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

### Comparing `types-aiobotocore-redshift-serverless-2.5.2.post2/types_aiobotocore_redshift_serverless/client.py` & `types-aiobotocore-redshift-serverless-2.5.4/types_aiobotocore_redshift_serverless/client.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-redshift-serverless-2.5.2.post2/types_aiobotocore_redshift_serverless/client.pyi` & `types-aiobotocore-redshift-serverless-2.5.4/types_aiobotocore_redshift_serverless/client.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-redshift-serverless-2.5.2.post2/types_aiobotocore_redshift_serverless/literals.py` & `types-aiobotocore-redshift-serverless-2.5.4/types_aiobotocore_redshift_serverless/literals.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-redshift-serverless-2.5.2.post2/types_aiobotocore_redshift_serverless/literals.pyi` & `types-aiobotocore-redshift-serverless-2.5.4/types_aiobotocore_redshift_serverless/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-redshift-serverless-2.5.2.post2/types_aiobotocore_redshift_serverless/paginator.py` & `types-aiobotocore-redshift-serverless-2.5.4/types_aiobotocore_redshift_serverless/paginator.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-redshift-serverless-2.5.2.post2/types_aiobotocore_redshift_serverless/paginator.pyi` & `types-aiobotocore-redshift-serverless-2.5.4/types_aiobotocore_redshift_serverless/paginator.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-redshift-serverless-2.5.2.post2/types_aiobotocore_redshift_serverless/type_defs.py` & `types-aiobotocore-redshift-serverless-2.5.4/types_aiobotocore_redshift_serverless/type_defs.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-redshift-serverless-2.5.2.post2/types_aiobotocore_redshift_serverless/type_defs.pyi` & `types-aiobotocore-redshift-serverless-2.5.4/types_aiobotocore_redshift_serverless/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-redshift-serverless-2.5.2.post2/types_aiobotocore_redshift_serverless.egg-info/PKG-INFO` & `types-aiobotocore-redshift-serverless-2.5.4/types_aiobotocore_redshift_serverless.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-redshift-serverless
-Version: 2.5.2.post2
-Summary: Type annotations for aiobotocore.RedshiftServerless 2.5.2 service generated with mypy-boto3-builder 7.17.2
+Version: 2.5.4
+Summary: Type annotations for aiobotocore.RedshiftServerless 2.5.4 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift_serverless/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-redshift-serverless.svg?color=blue)](https://pypi.org/project/types-aiobotocore-redshift-serverless)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift_serverless/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-redshift-serverless)](https://pepy.tech/project/types-aiobotocore-redshift-serverless)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.RedshiftServerless 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift-serverless.html#RedshiftServerless)
+[aiobotocore.RedshiftServerless 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift-serverless.html#RedshiftServerless)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-redshift-serverless-2.5.2.post2/types_aiobotocore_redshift_serverless.egg-info/SOURCES.txt` & `types-aiobotocore-redshift-serverless-2.5.4/types_aiobotocore_redshift_serverless.egg-info/SOURCES.txt`

 * *Files identical despite different names*

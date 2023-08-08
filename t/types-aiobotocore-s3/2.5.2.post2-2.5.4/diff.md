# Comparing `tmp/types-aiobotocore-s3-2.5.2.post2.tar.gz` & `tmp/types-aiobotocore-s3-2.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-s3-2.5.2.post2.tar", last modified: Fri Aug  4 13:59:24 2023, max compression
+gzip compressed data, was "types-aiobotocore-s3-2.5.4.tar", last modified: Tue Aug  8 01:24:21 2023, max compression
```

## Comparing `types-aiobotocore-s3-2.5.2.post2.tar` & `types-aiobotocore-s3-2.5.4.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:24.456643 types-aiobotocore-s3-2.5.2.post2/
--rw-r--r--   0 vlad      (1000) vlad      (1000)     1070 2023-08-04 13:51:27.000000 types-aiobotocore-s3-2.5.2.post2/LICENSE
--rw-r--r--   0 vlad      (1000) vlad      (1000)    17692 2023-08-04 13:59:24.446643 types-aiobotocore-s3-2.5.2.post2/PKG-INFO
--rw-r--r--   0 vlad      (1000) vlad      (1000)    16194 2023-08-04 13:51:27.000000 types-aiobotocore-s3-2.5.2.post2/README.md
--rw-r--r--   0 vlad      (1000) vlad      (1000)       38 2023-08-04 13:59:24.456643 types-aiobotocore-s3-2.5.2.post2/setup.cfg
--rw-r--r--   0 vlad      (1000) vlad      (1000)     2002 2023-08-04 13:51:27.000000 types-aiobotocore-s3-2.5.2.post2/setup.py
-drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:24.426643 types-aiobotocore-s3-2.5.2.post2/types_aiobotocore_s3/
--rw-r--r--   0 vlad      (1000) vlad      (1000)     2294 2023-08-04 13:51:27.000000 types-aiobotocore-s3-2.5.2.post2/types_aiobotocore_s3/__init__.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)     2292 2023-08-04 13:51:27.000000 types-aiobotocore-s3-2.5.2.post2/types_aiobotocore_s3/__init__.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)      912 2023-08-04 13:51:27.000000 types-aiobotocore-s3-2.5.2.post2/types_aiobotocore_s3/__main__.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)    87379 2023-08-04 13:51:31.000000 types-aiobotocore-s3-2.5.2.post2/types_aiobotocore_s3/client.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)    87258 2023-08-04 13:51:30.000000 types-aiobotocore-s3-2.5.2.post2/types_aiobotocore_s3/client.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)    16722 2023-08-04 13:51:33.000000 types-aiobotocore-s3-2.5.2.post2/types_aiobotocore_s3/literals.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)    16720 2023-08-04 13:51:32.000000 types-aiobotocore-s3-2.5.2.post2/types_aiobotocore_s3/literals.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)     7661 2023-08-04 13:51:32.000000 types-aiobotocore-s3-2.5.2.post2/types_aiobotocore_s3/paginator.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)     7653 2023-08-04 13:51:32.000000 types-aiobotocore-s3-2.5.2.post2/types_aiobotocore_s3/paginator.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:51:27.000000 types-aiobotocore-s3-2.5.2.post2/types_aiobotocore_s3/py.typed
--rw-r--r--   0 vlad      (1000) vlad      (1000)   124985 2023-08-04 13:51:32.000000 types-aiobotocore-s3-2.5.2.post2/types_aiobotocore_s3/service_resource.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)   124764 2023-08-04 13:51:31.000000 types-aiobotocore-s3-2.5.2.post2/types_aiobotocore_s3/service_resource.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)   194181 2023-08-04 13:51:40.000000 types-aiobotocore-s3-2.5.2.post2/types_aiobotocore_s3/type_defs.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)   193855 2023-08-04 13:51:35.000000 types-aiobotocore-s3-2.5.2.post2/types_aiobotocore_s3/type_defs.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)       65 2023-08-04 13:51:27.000000 types-aiobotocore-s3-2.5.2.post2/types_aiobotocore_s3/version.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)     5561 2023-08-04 13:51:32.000000 types-aiobotocore-s3-2.5.2.post2/types_aiobotocore_s3/waiter.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)     5556 2023-08-04 13:51:32.000000 types-aiobotocore-s3-2.5.2.post2/types_aiobotocore_s3/waiter.pyi
-drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:24.446643 types-aiobotocore-s3-2.5.2.post2/types_aiobotocore_s3.egg-info/
--rw-r--r--   0 vlad      (1000) vlad      (1000)    17692 2023-08-04 13:59:24.000000 types-aiobotocore-s3-2.5.2.post2/types_aiobotocore_s3.egg-info/PKG-INFO
--rw-r--r--   0 vlad      (1000) vlad      (1000)      864 2023-08-04 13:59:24.000000 types-aiobotocore-s3-2.5.2.post2/types_aiobotocore_s3.egg-info/SOURCES.txt
--rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:24.000000 types-aiobotocore-s3-2.5.2.post2/types_aiobotocore_s3.egg-info/dependency_links.txt
--rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:24.000000 types-aiobotocore-s3-2.5.2.post2/types_aiobotocore_s3.egg-info/not-zip-safe
--rw-r--r--   0 vlad      (1000) vlad      (1000)       52 2023-08-04 13:59:24.000000 types-aiobotocore-s3-2.5.2.post2/types_aiobotocore_s3.egg-info/requires.txt
--rw-r--r--   0 vlad      (1000) vlad      (1000)       21 2023-08-04 13:59:24.000000 types-aiobotocore-s3-2.5.2.post2/types_aiobotocore_s3.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:24:21.406768 types-aiobotocore-s3-2.5.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-08 01:19:50.000000 types-aiobotocore-s3-2.5.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    17686 2023-08-08 01:24:21.398768 types-aiobotocore-s3-2.5.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    16194 2023-08-08 01:19:50.000000 types-aiobotocore-s3-2.5.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-08 01:24:21.406768 types-aiobotocore-s3-2.5.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1996 2023-08-08 01:19:50.000000 types-aiobotocore-s3-2.5.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:24:21.398768 types-aiobotocore-s3-2.5.4/types_aiobotocore_s3/
+-rw-r--r--   0 runner    (1001) docker     (123)     2294 2023-08-08 01:19:50.000000 types-aiobotocore-s3-2.5.4/types_aiobotocore_s3/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2292 2023-08-08 01:19:50.000000 types-aiobotocore-s3-2.5.4/types_aiobotocore_s3/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      900 2023-08-08 01:19:50.000000 types-aiobotocore-s3-2.5.4/types_aiobotocore_s3/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    87379 2023-08-08 01:19:51.000000 types-aiobotocore-s3-2.5.4/types_aiobotocore_s3/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    87258 2023-08-08 01:19:51.000000 types-aiobotocore-s3-2.5.4/types_aiobotocore_s3/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    16722 2023-08-08 01:19:53.000000 types-aiobotocore-s3-2.5.4/types_aiobotocore_s3/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16720 2023-08-08 01:19:52.000000 types-aiobotocore-s3-2.5.4/types_aiobotocore_s3/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     7661 2023-08-08 01:19:52.000000 types-aiobotocore-s3-2.5.4/types_aiobotocore_s3/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7653 2023-08-08 01:19:52.000000 types-aiobotocore-s3-2.5.4/types_aiobotocore_s3/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 01:19:50.000000 types-aiobotocore-s3-2.5.4/types_aiobotocore_s3/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)   124985 2023-08-08 01:19:52.000000 types-aiobotocore-s3-2.5.4/types_aiobotocore_s3/service_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)   124764 2023-08-08 01:19:52.000000 types-aiobotocore-s3-2.5.4/types_aiobotocore_s3/service_resource.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)   194181 2023-08-08 01:19:59.000000 types-aiobotocore-s3-2.5.4/types_aiobotocore_s3/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)   193855 2023-08-08 01:19:54.000000 types-aiobotocore-s3-2.5.4/types_aiobotocore_s3/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-08-08 01:19:50.000000 types-aiobotocore-s3-2.5.4/types_aiobotocore_s3/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5561 2023-08-08 01:19:52.000000 types-aiobotocore-s3-2.5.4/types_aiobotocore_s3/waiter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5556 2023-08-08 01:19:52.000000 types-aiobotocore-s3-2.5.4/types_aiobotocore_s3/waiter.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:24:21.398768 types-aiobotocore-s3-2.5.4/types_aiobotocore_s3.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    17686 2023-08-08 01:24:21.000000 types-aiobotocore-s3-2.5.4/types_aiobotocore_s3.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      864 2023-08-08 01:24:21.000000 types-aiobotocore-s3-2.5.4/types_aiobotocore_s3.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 01:24:21.000000 types-aiobotocore-s3-2.5.4/types_aiobotocore_s3.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 01:24:21.000000 types-aiobotocore-s3-2.5.4/types_aiobotocore_s3.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-08 01:24:21.000000 types-aiobotocore-s3-2.5.4/types_aiobotocore_s3.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-08-08 01:24:21.000000 types-aiobotocore-s3-2.5.4/types_aiobotocore_s3.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-s3-2.5.2.post2/LICENSE` & `types-aiobotocore-s3-2.5.4/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-s3-2.5.2.post2/PKG-INFO` & `types-aiobotocore-s3-2.5.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-s3
-Version: 2.5.2.post2
-Summary: Type annotations for aiobotocore.S3 2.5.2 service generated with mypy-boto3-builder 7.17.2
+Version: 2.5.4
+Summary: Type annotations for aiobotocore.S3 2.5.4 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-s3.svg?color=blue)](https://pypi.org/project/types-aiobotocore-s3)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-s3)](https://pepy.tech/project/types-aiobotocore-s3)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.S3 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3)
+[aiobotocore.S3 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-s3-2.5.2.post2/README.md` & `types-aiobotocore-s3-2.5.4/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-s3.svg?color=blue)](https://pypi.org/project/types-aiobotocore-s3)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-s3)](https://pepy.tech/project/types-aiobotocore-s3)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.S3 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3)
+[aiobotocore.S3 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-s3-2.5.2.post2/setup.py` & `types-aiobotocore-s3-2.5.4/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-s3",
-    version="2.5.2.post2",
+    version="2.5.4",
     packages=["types_aiobotocore_s3"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.S3 2.5.2 service generated with mypy-boto3-builder 7.17.2"
+        "Type annotations for aiobotocore.S3 2.5.4 service generated with mypy-boto3-builder 7.17.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

### Comparing `types-aiobotocore-s3-2.5.2.post2/types_aiobotocore_s3/__init__.py` & `types-aiobotocore-s3-2.5.4/types_aiobotocore_s3/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-s3-2.5.2.post2/types_aiobotocore_s3/__init__.pyi` & `types-aiobotocore-s3-2.5.4/types_aiobotocore_s3/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-s3-2.5.2.post2/types_aiobotocore_s3/__main__.py` & `types-aiobotocore-s3-2.5.4/types_aiobotocore_s3/__main__.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.S3 2.5.2\nVersion:         2.5.2.post2\nBuilder version:"
+        "Type annotations for aiobotocore.S3 2.5.4\nVersion:         2.5.4\nBuilder version:"
         " 7.17.2\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3\nOther"
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

### Comparing `types-aiobotocore-s3-2.5.2.post2/types_aiobotocore_s3/client.py` & `types-aiobotocore-s3-2.5.4/types_aiobotocore_s3/client.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-s3-2.5.2.post2/types_aiobotocore_s3/client.pyi` & `types-aiobotocore-s3-2.5.4/types_aiobotocore_s3/client.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-s3-2.5.2.post2/types_aiobotocore_s3/literals.py` & `types-aiobotocore-s3-2.5.4/types_aiobotocore_s3/literals.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-s3-2.5.2.post2/types_aiobotocore_s3/literals.pyi` & `types-aiobotocore-s3-2.5.4/types_aiobotocore_s3/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-s3-2.5.2.post2/types_aiobotocore_s3/paginator.py` & `types-aiobotocore-s3-2.5.4/types_aiobotocore_s3/paginator.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-s3-2.5.2.post2/types_aiobotocore_s3/paginator.pyi` & `types-aiobotocore-s3-2.5.4/types_aiobotocore_s3/paginator.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-s3-2.5.2.post2/types_aiobotocore_s3/service_resource.py` & `types-aiobotocore-s3-2.5.4/types_aiobotocore_s3/service_resource.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-s3-2.5.2.post2/types_aiobotocore_s3/service_resource.pyi` & `types-aiobotocore-s3-2.5.4/types_aiobotocore_s3/service_resource.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-s3-2.5.2.post2/types_aiobotocore_s3/type_defs.py` & `types-aiobotocore-s3-2.5.4/types_aiobotocore_s3/type_defs.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-s3-2.5.2.post2/types_aiobotocore_s3/type_defs.pyi` & `types-aiobotocore-s3-2.5.4/types_aiobotocore_s3/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-s3-2.5.2.post2/types_aiobotocore_s3/waiter.py` & `types-aiobotocore-s3-2.5.4/types_aiobotocore_s3/waiter.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-s3-2.5.2.post2/types_aiobotocore_s3/waiter.pyi` & `types-aiobotocore-s3-2.5.4/types_aiobotocore_s3/waiter.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-s3-2.5.2.post2/types_aiobotocore_s3.egg-info/PKG-INFO` & `types-aiobotocore-s3-2.5.4/types_aiobotocore_s3.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-s3
-Version: 2.5.2.post2
-Summary: Type annotations for aiobotocore.S3 2.5.2 service generated with mypy-boto3-builder 7.17.2
+Version: 2.5.4
+Summary: Type annotations for aiobotocore.S3 2.5.4 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-s3.svg?color=blue)](https://pypi.org/project/types-aiobotocore-s3)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-s3)](https://pepy.tech/project/types-aiobotocore-s3)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.S3 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3)
+[aiobotocore.S3 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-s3-2.5.2.post2/types_aiobotocore_s3.egg-info/SOURCES.txt` & `types-aiobotocore-s3-2.5.4/types_aiobotocore_s3.egg-info/SOURCES.txt`

 * *Files identical despite different names*


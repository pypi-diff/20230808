# Comparing `tmp/types-aiobotocore-s3control-2.5.2.post2.tar.gz` & `tmp/types-aiobotocore-s3control-2.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-s3control-2.5.2.post2.tar", last modified: Fri Aug  4 13:59:24 2023, max compression
+gzip compressed data, was "types-aiobotocore-s3control-2.5.4.tar", last modified: Tue Aug  8 01:24:22 2023, max compression
```

## Comparing `types-aiobotocore-s3control-2.5.2.post2.tar` & `types-aiobotocore-s3control-2.5.4.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:24.836643 types-aiobotocore-s3control-2.5.2.post2/
--rw-r--r--   0 vlad      (1000) vlad      (1000)     1070 2023-08-04 13:51:42.000000 types-aiobotocore-s3control-2.5.2.post2/LICENSE
--rw-r--r--   0 vlad      (1000) vlad      (1000)    13149 2023-08-04 13:59:24.836643 types-aiobotocore-s3control-2.5.2.post2/PKG-INFO
--rw-r--r--   0 vlad      (1000) vlad      (1000)    11623 2023-08-04 13:51:42.000000 types-aiobotocore-s3control-2.5.2.post2/README.md
--rw-r--r--   0 vlad      (1000) vlad      (1000)       38 2023-08-04 13:59:24.836643 types-aiobotocore-s3control-2.5.2.post2/setup.cfg
--rw-r--r--   0 vlad      (1000) vlad      (1000)     2086 2023-08-04 13:51:42.000000 types-aiobotocore-s3control-2.5.2.post2/setup.py
-drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:24.836643 types-aiobotocore-s3control-2.5.2.post2/types_aiobotocore_s3control/
--rw-r--r--   0 vlad      (1000) vlad      (1000)      773 2023-08-04 13:51:42.000000 types-aiobotocore-s3control-2.5.2.post2/types_aiobotocore_s3control/__init__.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)      772 2023-08-04 13:51:42.000000 types-aiobotocore-s3control-2.5.2.post2/types_aiobotocore_s3control/__init__.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)      951 2023-08-04 13:51:42.000000 types-aiobotocore-s3control-2.5.2.post2/types_aiobotocore_s3control/__main__.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)    45691 2023-08-04 13:51:42.000000 types-aiobotocore-s3control-2.5.2.post2/types_aiobotocore_s3control/client.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)    45617 2023-08-04 13:51:42.000000 types-aiobotocore-s3control-2.5.2.post2/types_aiobotocore_s3control/client.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)    13714 2023-08-04 13:51:42.000000 types-aiobotocore-s3control-2.5.2.post2/types_aiobotocore_s3control/literals.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)    13712 2023-08-04 13:51:42.000000 types-aiobotocore-s3control-2.5.2.post2/types_aiobotocore_s3control/literals.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)     2229 2023-08-04 13:51:42.000000 types-aiobotocore-s3control-2.5.2.post2/types_aiobotocore_s3control/paginator.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)     2226 2023-08-04 13:51:42.000000 types-aiobotocore-s3control-2.5.2.post2/types_aiobotocore_s3control/paginator.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:51:42.000000 types-aiobotocore-s3control-2.5.2.post2/types_aiobotocore_s3control/py.typed
--rw-r--r--   0 vlad      (1000) vlad      (1000)    70218 2023-08-04 13:51:44.000000 types-aiobotocore-s3control-2.5.2.post2/types_aiobotocore_s3control/type_defs.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)    70141 2023-08-04 13:51:43.000000 types-aiobotocore-s3control-2.5.2.post2/types_aiobotocore_s3control/type_defs.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)       65 2023-08-04 13:51:42.000000 types-aiobotocore-s3control-2.5.2.post2/types_aiobotocore_s3control/version.py
-drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:24.836643 types-aiobotocore-s3control-2.5.2.post2/types_aiobotocore_s3control.egg-info/
--rw-r--r--   0 vlad      (1000) vlad      (1000)    13149 2023-08-04 13:59:24.000000 types-aiobotocore-s3control-2.5.2.post2/types_aiobotocore_s3control.egg-info/PKG-INFO
--rw-r--r--   0 vlad      (1000) vlad      (1000)      851 2023-08-04 13:59:24.000000 types-aiobotocore-s3control-2.5.2.post2/types_aiobotocore_s3control.egg-info/SOURCES.txt
--rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:24.000000 types-aiobotocore-s3control-2.5.2.post2/types_aiobotocore_s3control.egg-info/dependency_links.txt
--rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:24.000000 types-aiobotocore-s3control-2.5.2.post2/types_aiobotocore_s3control.egg-info/not-zip-safe
--rw-r--r--   0 vlad      (1000) vlad      (1000)       52 2023-08-04 13:59:24.000000 types-aiobotocore-s3control-2.5.2.post2/types_aiobotocore_s3control.egg-info/requires.txt
--rw-r--r--   0 vlad      (1000) vlad      (1000)       28 2023-08-04 13:59:24.000000 types-aiobotocore-s3control-2.5.2.post2/types_aiobotocore_s3control.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:24:22.226770 types-aiobotocore-s3control-2.5.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-08 01:19:59.000000 types-aiobotocore-s3control-2.5.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    13143 2023-08-08 01:24:22.226770 types-aiobotocore-s3control-2.5.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    11623 2023-08-08 01:19:59.000000 types-aiobotocore-s3control-2.5.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-08 01:24:22.226770 types-aiobotocore-s3control-2.5.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2080 2023-08-08 01:19:59.000000 types-aiobotocore-s3control-2.5.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:24:22.226770 types-aiobotocore-s3control-2.5.4/types_aiobotocore_s3control/
+-rw-r--r--   0 runner    (1001) docker     (123)      773 2023-08-08 01:19:59.000000 types-aiobotocore-s3control-2.5.4/types_aiobotocore_s3control/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      772 2023-08-08 01:19:59.000000 types-aiobotocore-s3control-2.5.4/types_aiobotocore_s3control/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      939 2023-08-08 01:19:59.000000 types-aiobotocore-s3control-2.5.4/types_aiobotocore_s3control/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    45691 2023-08-08 01:20:00.000000 types-aiobotocore-s3control-2.5.4/types_aiobotocore_s3control/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    45617 2023-08-08 01:19:59.000000 types-aiobotocore-s3control-2.5.4/types_aiobotocore_s3control/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    13714 2023-08-08 01:20:00.000000 types-aiobotocore-s3control-2.5.4/types_aiobotocore_s3control/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13712 2023-08-08 01:20:00.000000 types-aiobotocore-s3control-2.5.4/types_aiobotocore_s3control/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2229 2023-08-08 01:20:00.000000 types-aiobotocore-s3control-2.5.4/types_aiobotocore_s3control/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2226 2023-08-08 01:20:00.000000 types-aiobotocore-s3control-2.5.4/types_aiobotocore_s3control/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 01:19:59.000000 types-aiobotocore-s3control-2.5.4/types_aiobotocore_s3control/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    70218 2023-08-08 01:20:01.000000 types-aiobotocore-s3control-2.5.4/types_aiobotocore_s3control/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    70141 2023-08-08 01:20:01.000000 types-aiobotocore-s3control-2.5.4/types_aiobotocore_s3control/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-08-08 01:19:59.000000 types-aiobotocore-s3control-2.5.4/types_aiobotocore_s3control/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:24:22.226770 types-aiobotocore-s3control-2.5.4/types_aiobotocore_s3control.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    13143 2023-08-08 01:24:22.000000 types-aiobotocore-s3control-2.5.4/types_aiobotocore_s3control.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      851 2023-08-08 01:24:22.000000 types-aiobotocore-s3control-2.5.4/types_aiobotocore_s3control.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 01:24:22.000000 types-aiobotocore-s3control-2.5.4/types_aiobotocore_s3control.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 01:24:22.000000 types-aiobotocore-s3control-2.5.4/types_aiobotocore_s3control.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-08 01:24:22.000000 types-aiobotocore-s3control-2.5.4/types_aiobotocore_s3control.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-08-08 01:24:22.000000 types-aiobotocore-s3control-2.5.4/types_aiobotocore_s3control.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-s3control-2.5.2.post2/LICENSE` & `types-aiobotocore-s3control-2.5.4/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-s3control-2.5.2.post2/PKG-INFO` & `types-aiobotocore-s3control-2.5.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-s3control
-Version: 2.5.2.post2
-Summary: Type annotations for aiobotocore.S3Control 2.5.2 service generated with mypy-boto3-builder 7.17.2
+Version: 2.5.4
+Summary: Type annotations for aiobotocore.S3Control 2.5.4 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3control/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-s3control.svg?color=blue)](https://pypi.org/project/types-aiobotocore-s3control)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3control/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-s3control)](https://pepy.tech/project/types-aiobotocore-s3control)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.S3Control 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3control.html#S3Control)
+[aiobotocore.S3Control 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3control.html#S3Control)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-s3control-2.5.2.post2/README.md` & `types-aiobotocore-s3control-2.5.4/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-s3control.svg?color=blue)](https://pypi.org/project/types-aiobotocore-s3control)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3control/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-s3control)](https://pepy.tech/project/types-aiobotocore-s3control)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.S3Control 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3control.html#S3Control)
+[aiobotocore.S3Control 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3control.html#S3Control)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-s3control-2.5.2.post2/setup.py` & `types-aiobotocore-s3control-2.5.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-s3control",
-    version="2.5.2.post2",
+    version="2.5.4",
     packages=["types_aiobotocore_s3control"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.S3Control 2.5.2 service generated with mypy-boto3-builder"
+        "Type annotations for aiobotocore.S3Control 2.5.4 service generated with mypy-boto3-builder"
         " 7.17.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
```

### Comparing `types-aiobotocore-s3control-2.5.2.post2/types_aiobotocore_s3control/__init__.py` & `types-aiobotocore-s3control-2.5.4/types_aiobotocore_s3control/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-s3control-2.5.2.post2/types_aiobotocore_s3control/__init__.pyi` & `types-aiobotocore-s3control-2.5.4/types_aiobotocore_s3control/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-s3control-2.5.2.post2/types_aiobotocore_s3control/__main__.py` & `types-aiobotocore-s3control-2.5.4/types_aiobotocore_s3control/__main__.py`

 * *Files 24% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.S3Control 2.5.2\nVersion:         2.5.2.post2\nBuilder"
-        " version: 7.17.2\nDocs:           "
+        "Type annotations for aiobotocore.S3Control 2.5.4\nVersion:         2.5.4\nBuilder version:"
+        " 7.17.2\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3control//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3control.html#S3Control\nOther"
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

### Comparing `types-aiobotocore-s3control-2.5.2.post2/types_aiobotocore_s3control/client.py` & `types-aiobotocore-s3control-2.5.4/types_aiobotocore_s3control/client.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-s3control-2.5.2.post2/types_aiobotocore_s3control/client.pyi` & `types-aiobotocore-s3control-2.5.4/types_aiobotocore_s3control/client.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-s3control-2.5.2.post2/types_aiobotocore_s3control/literals.py` & `types-aiobotocore-s3control-2.5.4/types_aiobotocore_s3control/literals.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-s3control-2.5.2.post2/types_aiobotocore_s3control/literals.pyi` & `types-aiobotocore-s3control-2.5.4/types_aiobotocore_s3control/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-s3control-2.5.2.post2/types_aiobotocore_s3control/paginator.py` & `types-aiobotocore-s3control-2.5.4/types_aiobotocore_s3control/paginator.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-s3control-2.5.2.post2/types_aiobotocore_s3control/paginator.pyi` & `types-aiobotocore-s3control-2.5.4/types_aiobotocore_s3control/paginator.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-s3control-2.5.2.post2/types_aiobotocore_s3control/type_defs.py` & `types-aiobotocore-s3control-2.5.4/types_aiobotocore_s3control/type_defs.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-s3control-2.5.2.post2/types_aiobotocore_s3control/type_defs.pyi` & `types-aiobotocore-s3control-2.5.4/types_aiobotocore_s3control/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-s3control-2.5.2.post2/types_aiobotocore_s3control.egg-info/PKG-INFO` & `types-aiobotocore-s3control-2.5.4/types_aiobotocore_s3control.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-s3control
-Version: 2.5.2.post2
-Summary: Type annotations for aiobotocore.S3Control 2.5.2 service generated with mypy-boto3-builder 7.17.2
+Version: 2.5.4
+Summary: Type annotations for aiobotocore.S3Control 2.5.4 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3control/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-s3control.svg?color=blue)](https://pypi.org/project/types-aiobotocore-s3control)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3control/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-s3control)](https://pepy.tech/project/types-aiobotocore-s3control)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.S3Control 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3control.html#S3Control)
+[aiobotocore.S3Control 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3control.html#S3Control)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-s3control-2.5.2.post2/types_aiobotocore_s3control.egg-info/SOURCES.txt` & `types-aiobotocore-s3control-2.5.4/types_aiobotocore_s3control.egg-info/SOURCES.txt`

 * *Files identical despite different names*


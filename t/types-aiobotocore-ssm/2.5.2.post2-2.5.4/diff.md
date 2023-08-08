# Comparing `tmp/types-aiobotocore-ssm-2.5.2.post2.tar.gz` & `tmp/types-aiobotocore-ssm-2.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-ssm-2.5.2.post2.tar", last modified: Fri Aug  4 13:59:27 2023, max compression
+gzip compressed data, was "types-aiobotocore-ssm-2.5.4.tar", last modified: Tue Aug  8 01:24:29 2023, max compression
```

## Comparing `types-aiobotocore-ssm-2.5.2.post2.tar` & `types-aiobotocore-ssm-2.5.4.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:27.626643 types-aiobotocore-ssm-2.5.2.post2/
--rw-r--r--   0 vlad      (1000) vlad      (1000)     1070 2023-08-04 13:54:06.000000 types-aiobotocore-ssm-2.5.2.post2/LICENSE
--rw-r--r--   0 vlad      (1000) vlad      (1000)    21973 2023-08-04 13:59:27.626643 types-aiobotocore-ssm-2.5.2.post2/PKG-INFO
--rw-r--r--   0 vlad      (1000) vlad      (1000)    20471 2023-08-04 13:54:06.000000 types-aiobotocore-ssm-2.5.2.post2/README.md
--rw-r--r--   0 vlad      (1000) vlad      (1000)       38 2023-08-04 13:59:27.626643 types-aiobotocore-ssm-2.5.2.post2/setup.cfg
--rw-r--r--   0 vlad      (1000) vlad      (1000)     2020 2023-08-04 13:54:06.000000 types-aiobotocore-ssm-2.5.2.post2/setup.py
-drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:27.626643 types-aiobotocore-ssm-2.5.2.post2/types_aiobotocore_ssm/
--rw-r--r--   0 vlad      (1000) vlad      (1000)    12771 2023-08-04 13:54:06.000000 types-aiobotocore-ssm-2.5.2.post2/types_aiobotocore_ssm/__init__.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)    12770 2023-08-04 13:54:06.000000 types-aiobotocore-ssm-2.5.2.post2/types_aiobotocore_ssm/__init__.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)      916 2023-08-04 13:54:06.000000 types-aiobotocore-ssm-2.5.2.post2/types_aiobotocore_ssm/__main__.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)   136556 2023-08-04 13:54:08.000000 types-aiobotocore-ssm-2.5.2.post2/types_aiobotocore_ssm/client.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)   136361 2023-08-04 13:54:07.000000 types-aiobotocore-ssm-2.5.2.post2/types_aiobotocore_ssm/client.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)    28212 2023-08-04 13:54:12.000000 types-aiobotocore-ssm-2.5.2.post2/types_aiobotocore_ssm/literals.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)    28210 2023-08-04 13:54:12.000000 types-aiobotocore-ssm-2.5.2.post2/types_aiobotocore_ssm/literals.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)    61421 2023-08-04 13:54:12.000000 types-aiobotocore-ssm-2.5.2.post2/types_aiobotocore_ssm/paginator.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)    61372 2023-08-04 13:54:08.000000 types-aiobotocore-ssm-2.5.2.post2/types_aiobotocore_ssm/paginator.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:54:06.000000 types-aiobotocore-ssm-2.5.2.post2/types_aiobotocore_ssm/py.typed
--rw-r--r--   0 vlad      (1000) vlad      (1000)   204193 2023-08-04 13:54:17.000000 types-aiobotocore-ssm-2.5.2.post2/types_aiobotocore_ssm/type_defs.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)   203965 2023-08-04 13:54:15.000000 types-aiobotocore-ssm-2.5.2.post2/types_aiobotocore_ssm/type_defs.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)       65 2023-08-04 13:54:06.000000 types-aiobotocore-ssm-2.5.2.post2/types_aiobotocore_ssm/version.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)     1571 2023-08-04 13:54:12.000000 types-aiobotocore-ssm-2.5.2.post2/types_aiobotocore_ssm/waiter.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)     1570 2023-08-04 13:54:12.000000 types-aiobotocore-ssm-2.5.2.post2/types_aiobotocore_ssm/waiter.pyi
-drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:27.626643 types-aiobotocore-ssm-2.5.2.post2/types_aiobotocore_ssm.egg-info/
--rw-r--r--   0 vlad      (1000) vlad      (1000)    21973 2023-08-04 13:59:27.000000 types-aiobotocore-ssm-2.5.2.post2/types_aiobotocore_ssm.egg-info/PKG-INFO
--rw-r--r--   0 vlad      (1000) vlad      (1000)      802 2023-08-04 13:59:27.000000 types-aiobotocore-ssm-2.5.2.post2/types_aiobotocore_ssm.egg-info/SOURCES.txt
--rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:27.000000 types-aiobotocore-ssm-2.5.2.post2/types_aiobotocore_ssm.egg-info/dependency_links.txt
--rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:27.000000 types-aiobotocore-ssm-2.5.2.post2/types_aiobotocore_ssm.egg-info/not-zip-safe
--rw-r--r--   0 vlad      (1000) vlad      (1000)       52 2023-08-04 13:59:27.000000 types-aiobotocore-ssm-2.5.2.post2/types_aiobotocore_ssm.egg-info/requires.txt
--rw-r--r--   0 vlad      (1000) vlad      (1000)       22 2023-08-04 13:59:27.000000 types-aiobotocore-ssm-2.5.2.post2/types_aiobotocore_ssm.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:24:29.846789 types-aiobotocore-ssm-2.5.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-08 01:21:25.000000 types-aiobotocore-ssm-2.5.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    21967 2023-08-08 01:24:29.830789 types-aiobotocore-ssm-2.5.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    20471 2023-08-08 01:21:25.000000 types-aiobotocore-ssm-2.5.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-08 01:24:29.846789 types-aiobotocore-ssm-2.5.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2014 2023-08-08 01:21:25.000000 types-aiobotocore-ssm-2.5.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:24:29.830789 types-aiobotocore-ssm-2.5.4/types_aiobotocore_ssm/
+-rw-r--r--   0 runner    (1001) docker     (123)    12771 2023-08-08 01:21:25.000000 types-aiobotocore-ssm-2.5.4/types_aiobotocore_ssm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12770 2023-08-08 01:21:25.000000 types-aiobotocore-ssm-2.5.4/types_aiobotocore_ssm/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      904 2023-08-08 01:21:25.000000 types-aiobotocore-ssm-2.5.4/types_aiobotocore_ssm/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   136556 2023-08-08 01:21:29.000000 types-aiobotocore-ssm-2.5.4/types_aiobotocore_ssm/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)   136361 2023-08-08 01:21:29.000000 types-aiobotocore-ssm-2.5.4/types_aiobotocore_ssm/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    28212 2023-08-08 01:21:30.000000 types-aiobotocore-ssm-2.5.4/types_aiobotocore_ssm/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28210 2023-08-08 01:21:30.000000 types-aiobotocore-ssm-2.5.4/types_aiobotocore_ssm/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    61421 2023-08-08 01:21:29.000000 types-aiobotocore-ssm-2.5.4/types_aiobotocore_ssm/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    61372 2023-08-08 01:21:29.000000 types-aiobotocore-ssm-2.5.4/types_aiobotocore_ssm/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 01:21:25.000000 types-aiobotocore-ssm-2.5.4/types_aiobotocore_ssm/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)   204193 2023-08-08 01:21:34.000000 types-aiobotocore-ssm-2.5.4/types_aiobotocore_ssm/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)   203965 2023-08-08 01:21:32.000000 types-aiobotocore-ssm-2.5.4/types_aiobotocore_ssm/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-08-08 01:21:25.000000 types-aiobotocore-ssm-2.5.4/types_aiobotocore_ssm/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1571 2023-08-08 01:21:30.000000 types-aiobotocore-ssm-2.5.4/types_aiobotocore_ssm/waiter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1570 2023-08-08 01:21:30.000000 types-aiobotocore-ssm-2.5.4/types_aiobotocore_ssm/waiter.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:24:29.830789 types-aiobotocore-ssm-2.5.4/types_aiobotocore_ssm.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    21967 2023-08-08 01:24:29.000000 types-aiobotocore-ssm-2.5.4/types_aiobotocore_ssm.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      802 2023-08-08 01:24:29.000000 types-aiobotocore-ssm-2.5.4/types_aiobotocore_ssm.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 01:24:29.000000 types-aiobotocore-ssm-2.5.4/types_aiobotocore_ssm.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 01:24:29.000000 types-aiobotocore-ssm-2.5.4/types_aiobotocore_ssm.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-08 01:24:29.000000 types-aiobotocore-ssm-2.5.4/types_aiobotocore_ssm.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-08-08 01:24:29.000000 types-aiobotocore-ssm-2.5.4/types_aiobotocore_ssm.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-ssm-2.5.2.post2/LICENSE` & `types-aiobotocore-ssm-2.5.4/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-ssm-2.5.2.post2/PKG-INFO` & `types-aiobotocore-ssm-2.5.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-ssm
-Version: 2.5.2.post2
-Summary: Type annotations for aiobotocore.SSM 2.5.2 service generated with mypy-boto3-builder 7.17.2
+Version: 2.5.4
+Summary: Type annotations for aiobotocore.SSM 2.5.4 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-ssm.svg?color=blue)](https://pypi.org/project/types-aiobotocore-ssm)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-ssm)](https://pepy.tech/project/types-aiobotocore-ssm)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.SSM 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM)
+[aiobotocore.SSM 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-ssm-2.5.2.post2/README.md` & `types-aiobotocore-ssm-2.5.4/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-ssm.svg?color=blue)](https://pypi.org/project/types-aiobotocore-ssm)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-ssm)](https://pepy.tech/project/types-aiobotocore-ssm)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.SSM 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM)
+[aiobotocore.SSM 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-ssm-2.5.2.post2/setup.py` & `types-aiobotocore-ssm-2.5.4/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-ssm",
-    version="2.5.2.post2",
+    version="2.5.4",
     packages=["types_aiobotocore_ssm"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.SSM 2.5.2 service generated with mypy-boto3-builder"
+        "Type annotations for aiobotocore.SSM 2.5.4 service generated with mypy-boto3-builder"
         " 7.17.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
```

### Comparing `types-aiobotocore-ssm-2.5.2.post2/types_aiobotocore_ssm/__init__.py` & `types-aiobotocore-ssm-2.5.4/types_aiobotocore_ssm/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-ssm-2.5.2.post2/types_aiobotocore_ssm/__init__.pyi` & `types-aiobotocore-ssm-2.5.4/types_aiobotocore_ssm/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-ssm-2.5.2.post2/types_aiobotocore_ssm/__main__.py` & `types-aiobotocore-ssm-2.5.4/types_aiobotocore_ssm/__main__.py`

 * *Files 7% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.SSM 2.5.2\nVersion:         2.5.2.post2\nBuilder version:"
+        "Type annotations for aiobotocore.SSM 2.5.4\nVersion:         2.5.4\nBuilder version:"
         " 7.17.2\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm//\nBoto3 docs:    "
         "  https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM\nOther"
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

### Comparing `types-aiobotocore-ssm-2.5.2.post2/types_aiobotocore_ssm/client.py` & `types-aiobotocore-ssm-2.5.4/types_aiobotocore_ssm/client.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-ssm-2.5.2.post2/types_aiobotocore_ssm/client.pyi` & `types-aiobotocore-ssm-2.5.4/types_aiobotocore_ssm/client.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-ssm-2.5.2.post2/types_aiobotocore_ssm/literals.py` & `types-aiobotocore-ssm-2.5.4/types_aiobotocore_ssm/literals.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-ssm-2.5.2.post2/types_aiobotocore_ssm/literals.pyi` & `types-aiobotocore-ssm-2.5.4/types_aiobotocore_ssm/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-ssm-2.5.2.post2/types_aiobotocore_ssm/paginator.py` & `types-aiobotocore-ssm-2.5.4/types_aiobotocore_ssm/paginator.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-ssm-2.5.2.post2/types_aiobotocore_ssm/paginator.pyi` & `types-aiobotocore-ssm-2.5.4/types_aiobotocore_ssm/paginator.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-ssm-2.5.2.post2/types_aiobotocore_ssm/type_defs.py` & `types-aiobotocore-ssm-2.5.4/types_aiobotocore_ssm/type_defs.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-ssm-2.5.2.post2/types_aiobotocore_ssm/type_defs.pyi` & `types-aiobotocore-ssm-2.5.4/types_aiobotocore_ssm/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-ssm-2.5.2.post2/types_aiobotocore_ssm/waiter.py` & `types-aiobotocore-ssm-2.5.4/types_aiobotocore_ssm/waiter.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-ssm-2.5.2.post2/types_aiobotocore_ssm/waiter.pyi` & `types-aiobotocore-ssm-2.5.4/types_aiobotocore_ssm/waiter.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-ssm-2.5.2.post2/types_aiobotocore_ssm.egg-info/PKG-INFO` & `types-aiobotocore-ssm-2.5.4/types_aiobotocore_ssm.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-ssm
-Version: 2.5.2.post2
-Summary: Type annotations for aiobotocore.SSM 2.5.2 service generated with mypy-boto3-builder 7.17.2
+Version: 2.5.4
+Summary: Type annotations for aiobotocore.SSM 2.5.4 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-ssm.svg?color=blue)](https://pypi.org/project/types-aiobotocore-ssm)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-ssm)](https://pepy.tech/project/types-aiobotocore-ssm)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.SSM 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM)
+[aiobotocore.SSM 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-ssm-2.5.2.post2/types_aiobotocore_ssm.egg-info/SOURCES.txt` & `types-aiobotocore-ssm-2.5.4/types_aiobotocore_ssm.egg-info/SOURCES.txt`

 * *Files identical despite different names*


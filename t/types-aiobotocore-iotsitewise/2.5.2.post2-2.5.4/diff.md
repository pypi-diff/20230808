# Comparing `tmp/types-aiobotocore-iotsitewise-2.5.2.post2.tar.gz` & `tmp/types-aiobotocore-iotsitewise-2.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-iotsitewise-2.5.2.post2.tar", last modified: Fri Aug  4 13:59:13 2023, max compression
+gzip compressed data, was "types-aiobotocore-iotsitewise-2.5.4.tar", last modified: Tue Aug  8 01:23:53 2023, max compression
```

## Comparing `types-aiobotocore-iotsitewise-2.5.2.post2.tar` & `types-aiobotocore-iotsitewise-2.5.4.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:13.056643 types-aiobotocore-iotsitewise-2.5.2.post2/
--rw-r--r--   0 vlad      (1000) vlad      (1000)     1070 2023-08-04 13:41:12.000000 types-aiobotocore-iotsitewise-2.5.2.post2/LICENSE
--rw-r--r--   0 vlad      (1000) vlad      (1000)    16974 2023-08-04 13:59:13.056643 types-aiobotocore-iotsitewise-2.5.2.post2/PKG-INFO
--rw-r--r--   0 vlad      (1000) vlad      (1000)    15440 2023-08-04 13:41:12.000000 types-aiobotocore-iotsitewise-2.5.2.post2/README.md
--rw-r--r--   0 vlad      (1000) vlad      (1000)       38 2023-08-04 13:59:13.056643 types-aiobotocore-iotsitewise-2.5.2.post2/setup.cfg
--rw-r--r--   0 vlad      (1000) vlad      (1000)     2100 2023-08-04 13:41:12.000000 types-aiobotocore-iotsitewise-2.5.2.post2/setup.py
-drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:13.056643 types-aiobotocore-iotsitewise-2.5.2.post2/types_aiobotocore_iotsitewise/
--rw-r--r--   0 vlad      (1000) vlad      (1000)     5322 2023-08-04 13:41:12.000000 types-aiobotocore-iotsitewise-2.5.2.post2/types_aiobotocore_iotsitewise/__init__.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)     5321 2023-08-04 13:41:12.000000 types-aiobotocore-iotsitewise-2.5.2.post2/types_aiobotocore_iotsitewise/__init__.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)      959 2023-08-04 13:41:12.000000 types-aiobotocore-iotsitewise-2.5.2.post2/types_aiobotocore_iotsitewise/__main__.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)    65807 2023-08-04 13:41:13.000000 types-aiobotocore-iotsitewise-2.5.2.post2/types_aiobotocore_iotsitewise/client.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)    65702 2023-08-04 13:41:12.000000 types-aiobotocore-iotsitewise-2.5.2.post2/types_aiobotocore_iotsitewise/client.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)    15491 2023-08-04 13:41:14.000000 types-aiobotocore-iotsitewise-2.5.2.post2/types_aiobotocore_iotsitewise/literals.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)    15489 2023-08-04 13:41:13.000000 types-aiobotocore-iotsitewise-2.5.2.post2/types_aiobotocore_iotsitewise/literals.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)    22753 2023-08-04 13:41:13.000000 types-aiobotocore-iotsitewise-2.5.2.post2/types_aiobotocore_iotsitewise/paginator.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)    22733 2023-08-04 13:41:13.000000 types-aiobotocore-iotsitewise-2.5.2.post2/types_aiobotocore_iotsitewise/paginator.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:41:12.000000 types-aiobotocore-iotsitewise-2.5.2.post2/types_aiobotocore_iotsitewise/py.typed
--rw-r--r--   0 vlad      (1000) vlad      (1000)   105809 2023-08-04 13:41:17.000000 types-aiobotocore-iotsitewise-2.5.2.post2/types_aiobotocore_iotsitewise/type_defs.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)   105608 2023-08-04 13:41:15.000000 types-aiobotocore-iotsitewise-2.5.2.post2/types_aiobotocore_iotsitewise/type_defs.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)       65 2023-08-04 13:41:12.000000 types-aiobotocore-iotsitewise-2.5.2.post2/types_aiobotocore_iotsitewise/version.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)     6730 2023-08-04 13:41:13.000000 types-aiobotocore-iotsitewise-2.5.2.post2/types_aiobotocore_iotsitewise/waiter.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)     6724 2023-08-04 13:41:13.000000 types-aiobotocore-iotsitewise-2.5.2.post2/types_aiobotocore_iotsitewise/waiter.pyi
-drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:13.056643 types-aiobotocore-iotsitewise-2.5.2.post2/types_aiobotocore_iotsitewise.egg-info/
--rw-r--r--   0 vlad      (1000) vlad      (1000)    16974 2023-08-04 13:59:12.000000 types-aiobotocore-iotsitewise-2.5.2.post2/types_aiobotocore_iotsitewise.egg-info/PKG-INFO
--rw-r--r--   0 vlad      (1000) vlad      (1000)      970 2023-08-04 13:59:12.000000 types-aiobotocore-iotsitewise-2.5.2.post2/types_aiobotocore_iotsitewise.egg-info/SOURCES.txt
--rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:12.000000 types-aiobotocore-iotsitewise-2.5.2.post2/types_aiobotocore_iotsitewise.egg-info/dependency_links.txt
--rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:12.000000 types-aiobotocore-iotsitewise-2.5.2.post2/types_aiobotocore_iotsitewise.egg-info/not-zip-safe
--rw-r--r--   0 vlad      (1000) vlad      (1000)       52 2023-08-04 13:59:12.000000 types-aiobotocore-iotsitewise-2.5.2.post2/types_aiobotocore_iotsitewise.egg-info/requires.txt
--rw-r--r--   0 vlad      (1000) vlad      (1000)       30 2023-08-04 13:59:12.000000 types-aiobotocore-iotsitewise-2.5.2.post2/types_aiobotocore_iotsitewise.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:23:53.690708 types-aiobotocore-iotsitewise-2.5.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-08 01:13:04.000000 types-aiobotocore-iotsitewise-2.5.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    16968 2023-08-08 01:23:53.690708 types-aiobotocore-iotsitewise-2.5.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    15440 2023-08-08 01:13:04.000000 types-aiobotocore-iotsitewise-2.5.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-08 01:23:53.690708 types-aiobotocore-iotsitewise-2.5.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2094 2023-08-08 01:13:04.000000 types-aiobotocore-iotsitewise-2.5.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:23:53.690708 types-aiobotocore-iotsitewise-2.5.4/types_aiobotocore_iotsitewise/
+-rw-r--r--   0 runner    (1001) docker     (123)     5322 2023-08-08 01:13:04.000000 types-aiobotocore-iotsitewise-2.5.4/types_aiobotocore_iotsitewise/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5321 2023-08-08 01:13:04.000000 types-aiobotocore-iotsitewise-2.5.4/types_aiobotocore_iotsitewise/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      947 2023-08-08 01:13:04.000000 types-aiobotocore-iotsitewise-2.5.4/types_aiobotocore_iotsitewise/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    65807 2023-08-08 01:13:05.000000 types-aiobotocore-iotsitewise-2.5.4/types_aiobotocore_iotsitewise/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    65702 2023-08-08 01:13:05.000000 types-aiobotocore-iotsitewise-2.5.4/types_aiobotocore_iotsitewise/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    15491 2023-08-08 01:13:05.000000 types-aiobotocore-iotsitewise-2.5.4/types_aiobotocore_iotsitewise/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15489 2023-08-08 01:13:05.000000 types-aiobotocore-iotsitewise-2.5.4/types_aiobotocore_iotsitewise/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    22753 2023-08-08 01:13:05.000000 types-aiobotocore-iotsitewise-2.5.4/types_aiobotocore_iotsitewise/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22733 2023-08-08 01:13:05.000000 types-aiobotocore-iotsitewise-2.5.4/types_aiobotocore_iotsitewise/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 01:13:04.000000 types-aiobotocore-iotsitewise-2.5.4/types_aiobotocore_iotsitewise/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)   105809 2023-08-08 01:13:07.000000 types-aiobotocore-iotsitewise-2.5.4/types_aiobotocore_iotsitewise/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)   105608 2023-08-08 01:13:06.000000 types-aiobotocore-iotsitewise-2.5.4/types_aiobotocore_iotsitewise/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-08-08 01:13:04.000000 types-aiobotocore-iotsitewise-2.5.4/types_aiobotocore_iotsitewise/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6730 2023-08-08 01:13:05.000000 types-aiobotocore-iotsitewise-2.5.4/types_aiobotocore_iotsitewise/waiter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6724 2023-08-08 01:13:05.000000 types-aiobotocore-iotsitewise-2.5.4/types_aiobotocore_iotsitewise/waiter.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:23:53.690708 types-aiobotocore-iotsitewise-2.5.4/types_aiobotocore_iotsitewise.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    16968 2023-08-08 01:23:53.000000 types-aiobotocore-iotsitewise-2.5.4/types_aiobotocore_iotsitewise.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      970 2023-08-08 01:23:53.000000 types-aiobotocore-iotsitewise-2.5.4/types_aiobotocore_iotsitewise.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 01:23:53.000000 types-aiobotocore-iotsitewise-2.5.4/types_aiobotocore_iotsitewise.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 01:23:53.000000 types-aiobotocore-iotsitewise-2.5.4/types_aiobotocore_iotsitewise.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-08 01:23:53.000000 types-aiobotocore-iotsitewise-2.5.4/types_aiobotocore_iotsitewise.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-08-08 01:23:53.000000 types-aiobotocore-iotsitewise-2.5.4/types_aiobotocore_iotsitewise.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-iotsitewise-2.5.2.post2/LICENSE` & `types-aiobotocore-iotsitewise-2.5.4/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-iotsitewise-2.5.2.post2/PKG-INFO` & `types-aiobotocore-iotsitewise-2.5.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-iotsitewise
-Version: 2.5.2.post2
-Summary: Type annotations for aiobotocore.IoTSiteWise 2.5.2 service generated with mypy-boto3-builder 7.17.2
+Version: 2.5.4
+Summary: Type annotations for aiobotocore.IoTSiteWise 2.5.4 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotsitewise/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-iotsitewise.svg?color=blue)](https://pypi.org/project/types-aiobotocore-iotsitewise)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotsitewise/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-iotsitewise)](https://pepy.tech/project/types-aiobotocore-iotsitewise)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.IoTSiteWise 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotsitewise.html#IoTSiteWise)
+[aiobotocore.IoTSiteWise 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotsitewise.html#IoTSiteWise)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-iotsitewise-2.5.2.post2/README.md` & `types-aiobotocore-iotsitewise-2.5.4/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-iotsitewise.svg?color=blue)](https://pypi.org/project/types-aiobotocore-iotsitewise)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotsitewise/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-iotsitewise)](https://pepy.tech/project/types-aiobotocore-iotsitewise)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.IoTSiteWise 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotsitewise.html#IoTSiteWise)
+[aiobotocore.IoTSiteWise 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotsitewise.html#IoTSiteWise)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-iotsitewise-2.5.2.post2/setup.py` & `types-aiobotocore-iotsitewise-2.5.4/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-iotsitewise",
-    version="2.5.2.post2",
+    version="2.5.4",
     packages=["types_aiobotocore_iotsitewise"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.IoTSiteWise 2.5.2 service generated with"
+        "Type annotations for aiobotocore.IoTSiteWise 2.5.4 service generated with"
         " mypy-boto3-builder 7.17.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
```

### Comparing `types-aiobotocore-iotsitewise-2.5.2.post2/types_aiobotocore_iotsitewise/__init__.py` & `types-aiobotocore-iotsitewise-2.5.4/types_aiobotocore_iotsitewise/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-iotsitewise-2.5.2.post2/types_aiobotocore_iotsitewise/__init__.pyi` & `types-aiobotocore-iotsitewise-2.5.4/types_aiobotocore_iotsitewise/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-iotsitewise-2.5.2.post2/types_aiobotocore_iotsitewise/__main__.py` & `types-aiobotocore-iotsitewise-2.5.4/types_aiobotocore_iotsitewise/__main__.py`

 * *Files 10% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.IoTSiteWise 2.5.2\nVersion:         2.5.2.post2\nBuilder"
+        "Type annotations for aiobotocore.IoTSiteWise 2.5.4\nVersion:         2.5.4\nBuilder"
         " version: 7.17.2\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotsitewise//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotsitewise.html#IoTSiteWise\nOther"
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

### Comparing `types-aiobotocore-iotsitewise-2.5.2.post2/types_aiobotocore_iotsitewise/client.py` & `types-aiobotocore-iotsitewise-2.5.4/types_aiobotocore_iotsitewise/client.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-iotsitewise-2.5.2.post2/types_aiobotocore_iotsitewise/client.pyi` & `types-aiobotocore-iotsitewise-2.5.4/types_aiobotocore_iotsitewise/client.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-iotsitewise-2.5.2.post2/types_aiobotocore_iotsitewise/literals.py` & `types-aiobotocore-iotsitewise-2.5.4/types_aiobotocore_iotsitewise/literals.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-iotsitewise-2.5.2.post2/types_aiobotocore_iotsitewise/literals.pyi` & `types-aiobotocore-iotsitewise-2.5.4/types_aiobotocore_iotsitewise/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-iotsitewise-2.5.2.post2/types_aiobotocore_iotsitewise/paginator.py` & `types-aiobotocore-iotsitewise-2.5.4/types_aiobotocore_iotsitewise/paginator.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-iotsitewise-2.5.2.post2/types_aiobotocore_iotsitewise/paginator.pyi` & `types-aiobotocore-iotsitewise-2.5.4/types_aiobotocore_iotsitewise/paginator.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-iotsitewise-2.5.2.post2/types_aiobotocore_iotsitewise/type_defs.py` & `types-aiobotocore-iotsitewise-2.5.4/types_aiobotocore_iotsitewise/type_defs.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-iotsitewise-2.5.2.post2/types_aiobotocore_iotsitewise/type_defs.pyi` & `types-aiobotocore-iotsitewise-2.5.4/types_aiobotocore_iotsitewise/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-iotsitewise-2.5.2.post2/types_aiobotocore_iotsitewise/waiter.py` & `types-aiobotocore-iotsitewise-2.5.4/types_aiobotocore_iotsitewise/waiter.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-iotsitewise-2.5.2.post2/types_aiobotocore_iotsitewise/waiter.pyi` & `types-aiobotocore-iotsitewise-2.5.4/types_aiobotocore_iotsitewise/waiter.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-iotsitewise-2.5.2.post2/types_aiobotocore_iotsitewise.egg-info/PKG-INFO` & `types-aiobotocore-iotsitewise-2.5.4/types_aiobotocore_iotsitewise.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-iotsitewise
-Version: 2.5.2.post2
-Summary: Type annotations for aiobotocore.IoTSiteWise 2.5.2 service generated with mypy-boto3-builder 7.17.2
+Version: 2.5.4
+Summary: Type annotations for aiobotocore.IoTSiteWise 2.5.4 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotsitewise/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-iotsitewise.svg?color=blue)](https://pypi.org/project/types-aiobotocore-iotsitewise)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotsitewise/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-iotsitewise)](https://pepy.tech/project/types-aiobotocore-iotsitewise)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.IoTSiteWise 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotsitewise.html#IoTSiteWise)
+[aiobotocore.IoTSiteWise 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotsitewise.html#IoTSiteWise)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-iotsitewise-2.5.2.post2/types_aiobotocore_iotsitewise.egg-info/SOURCES.txt` & `types-aiobotocore-iotsitewise-2.5.4/types_aiobotocore_iotsitewise.egg-info/SOURCES.txt`

 * *Files identical despite different names*


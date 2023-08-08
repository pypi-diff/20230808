# Comparing `tmp/types-aiobotocore-transfer-2.5.2.post2.tar.gz` & `tmp/types-aiobotocore-transfer-2.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-transfer-2.5.2.post2.tar", last modified: Fri Aug  4 13:59:29 2023, max compression
+gzip compressed data, was "types-aiobotocore-transfer-2.5.4.tar", last modified: Tue Aug  8 01:24:33 2023, max compression
```

## Comparing `types-aiobotocore-transfer-2.5.2.post2.tar` & `types-aiobotocore-transfer-2.5.4.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:29.206643 types-aiobotocore-transfer-2.5.2.post2/
--rw-r--r--   0 vlad      (1000) vlad      (1000)     1070 2023-08-04 13:55:17.000000 types-aiobotocore-transfer-2.5.2.post2/LICENSE
--rw-r--r--   0 vlad      (1000) vlad      (1000)    15082 2023-08-04 13:59:29.206643 types-aiobotocore-transfer-2.5.2.post2/PKG-INFO
--rw-r--r--   0 vlad      (1000) vlad      (1000)    13560 2023-08-04 13:55:17.000000 types-aiobotocore-transfer-2.5.2.post2/README.md
--rw-r--r--   0 vlad      (1000) vlad      (1000)       38 2023-08-04 13:59:29.206643 types-aiobotocore-transfer-2.5.2.post2/setup.cfg
--rw-r--r--   0 vlad      (1000) vlad      (1000)     2079 2023-08-04 13:55:17.000000 types-aiobotocore-transfer-2.5.2.post2/setup.py
-drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:29.206643 types-aiobotocore-transfer-2.5.2.post2/types_aiobotocore_transfer/
--rw-r--r--   0 vlad      (1000) vlad      (1000)     2923 2023-08-04 13:55:17.000000 types-aiobotocore-transfer-2.5.2.post2/types_aiobotocore_transfer/__init__.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)     2922 2023-08-04 13:55:17.000000 types-aiobotocore-transfer-2.5.2.post2/types_aiobotocore_transfer/__init__.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)      947 2023-08-04 13:55:17.000000 types-aiobotocore-transfer-2.5.2.post2/types_aiobotocore_transfer/__main__.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)    49822 2023-08-04 13:55:18.000000 types-aiobotocore-transfer-2.5.2.post2/types_aiobotocore_transfer/client.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)    49741 2023-08-04 13:55:17.000000 types-aiobotocore-transfer-2.5.2.post2/types_aiobotocore_transfer/client.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)    12293 2023-08-04 13:55:18.000000 types-aiobotocore-transfer-2.5.2.post2/types_aiobotocore_transfer/literals.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)    12291 2023-08-04 13:55:18.000000 types-aiobotocore-transfer-2.5.2.post2/types_aiobotocore_transfer/literals.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)    12803 2023-08-04 13:55:18.000000 types-aiobotocore-transfer-2.5.2.post2/types_aiobotocore_transfer/paginator.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)    12790 2023-08-04 13:55:18.000000 types-aiobotocore-transfer-2.5.2.post2/types_aiobotocore_transfer/paginator.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:55:17.000000 types-aiobotocore-transfer-2.5.2.post2/types_aiobotocore_transfer/py.typed
--rw-r--r--   0 vlad      (1000) vlad      (1000)    60425 2023-08-04 13:55:20.000000 types-aiobotocore-transfer-2.5.2.post2/types_aiobotocore_transfer/type_defs.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)    60334 2023-08-04 13:55:19.000000 types-aiobotocore-transfer-2.5.2.post2/types_aiobotocore_transfer/type_defs.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)       65 2023-08-04 13:55:17.000000 types-aiobotocore-transfer-2.5.2.post2/types_aiobotocore_transfer/version.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)     2438 2023-08-04 13:55:18.000000 types-aiobotocore-transfer-2.5.2.post2/types_aiobotocore_transfer/waiter.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)     2436 2023-08-04 13:55:18.000000 types-aiobotocore-transfer-2.5.2.post2/types_aiobotocore_transfer/waiter.pyi
-drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:29.206643 types-aiobotocore-transfer-2.5.2.post2/types_aiobotocore_transfer.egg-info/
--rw-r--r--   0 vlad      (1000) vlad      (1000)    15082 2023-08-04 13:59:29.000000 types-aiobotocore-transfer-2.5.2.post2/types_aiobotocore_transfer.egg-info/PKG-INFO
--rw-r--r--   0 vlad      (1000) vlad      (1000)      907 2023-08-04 13:59:29.000000 types-aiobotocore-transfer-2.5.2.post2/types_aiobotocore_transfer.egg-info/SOURCES.txt
--rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:29.000000 types-aiobotocore-transfer-2.5.2.post2/types_aiobotocore_transfer.egg-info/dependency_links.txt
--rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:29.000000 types-aiobotocore-transfer-2.5.2.post2/types_aiobotocore_transfer.egg-info/not-zip-safe
--rw-r--r--   0 vlad      (1000) vlad      (1000)       52 2023-08-04 13:59:29.000000 types-aiobotocore-transfer-2.5.2.post2/types_aiobotocore_transfer.egg-info/requires.txt
--rw-r--r--   0 vlad      (1000) vlad      (1000)       27 2023-08-04 13:59:29.000000 types-aiobotocore-transfer-2.5.2.post2/types_aiobotocore_transfer.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:24:33.874799 types-aiobotocore-transfer-2.5.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-08 01:22:08.000000 types-aiobotocore-transfer-2.5.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    15076 2023-08-08 01:24:33.874799 types-aiobotocore-transfer-2.5.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    13560 2023-08-08 01:22:08.000000 types-aiobotocore-transfer-2.5.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-08 01:24:33.874799 types-aiobotocore-transfer-2.5.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2073 2023-08-08 01:22:08.000000 types-aiobotocore-transfer-2.5.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:24:33.874799 types-aiobotocore-transfer-2.5.4/types_aiobotocore_transfer/
+-rw-r--r--   0 runner    (1001) docker     (123)     2923 2023-08-08 01:22:08.000000 types-aiobotocore-transfer-2.5.4/types_aiobotocore_transfer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2922 2023-08-08 01:22:08.000000 types-aiobotocore-transfer-2.5.4/types_aiobotocore_transfer/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      935 2023-08-08 01:22:08.000000 types-aiobotocore-transfer-2.5.4/types_aiobotocore_transfer/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    49822 2023-08-08 01:22:08.000000 types-aiobotocore-transfer-2.5.4/types_aiobotocore_transfer/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    49741 2023-08-08 01:22:08.000000 types-aiobotocore-transfer-2.5.4/types_aiobotocore_transfer/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    12293 2023-08-08 01:22:09.000000 types-aiobotocore-transfer-2.5.4/types_aiobotocore_transfer/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12291 2023-08-08 01:22:08.000000 types-aiobotocore-transfer-2.5.4/types_aiobotocore_transfer/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    12803 2023-08-08 01:22:08.000000 types-aiobotocore-transfer-2.5.4/types_aiobotocore_transfer/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12790 2023-08-08 01:22:08.000000 types-aiobotocore-transfer-2.5.4/types_aiobotocore_transfer/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 01:22:08.000000 types-aiobotocore-transfer-2.5.4/types_aiobotocore_transfer/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    60425 2023-08-08 01:22:10.000000 types-aiobotocore-transfer-2.5.4/types_aiobotocore_transfer/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    60334 2023-08-08 01:22:09.000000 types-aiobotocore-transfer-2.5.4/types_aiobotocore_transfer/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-08-08 01:22:08.000000 types-aiobotocore-transfer-2.5.4/types_aiobotocore_transfer/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2438 2023-08-08 01:22:08.000000 types-aiobotocore-transfer-2.5.4/types_aiobotocore_transfer/waiter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2436 2023-08-08 01:22:08.000000 types-aiobotocore-transfer-2.5.4/types_aiobotocore_transfer/waiter.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:24:33.874799 types-aiobotocore-transfer-2.5.4/types_aiobotocore_transfer.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    15076 2023-08-08 01:24:33.000000 types-aiobotocore-transfer-2.5.4/types_aiobotocore_transfer.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      907 2023-08-08 01:24:33.000000 types-aiobotocore-transfer-2.5.4/types_aiobotocore_transfer.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 01:24:33.000000 types-aiobotocore-transfer-2.5.4/types_aiobotocore_transfer.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 01:24:33.000000 types-aiobotocore-transfer-2.5.4/types_aiobotocore_transfer.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-08 01:24:33.000000 types-aiobotocore-transfer-2.5.4/types_aiobotocore_transfer.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-08-08 01:24:33.000000 types-aiobotocore-transfer-2.5.4/types_aiobotocore_transfer.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-transfer-2.5.2.post2/LICENSE` & `types-aiobotocore-transfer-2.5.4/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-transfer-2.5.2.post2/PKG-INFO` & `types-aiobotocore-transfer-2.5.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-transfer
-Version: 2.5.2.post2
-Summary: Type annotations for aiobotocore.Transfer 2.5.2 service generated with mypy-boto3-builder 7.17.2
+Version: 2.5.4
+Summary: Type annotations for aiobotocore.Transfer 2.5.4 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_transfer/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-transfer.svg?color=blue)](https://pypi.org/project/types-aiobotocore-transfer)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_transfer/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-transfer)](https://pepy.tech/project/types-aiobotocore-transfer)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.Transfer 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transfer.html#Transfer)
+[aiobotocore.Transfer 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transfer.html#Transfer)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-transfer-2.5.2.post2/README.md` & `types-aiobotocore-transfer-2.5.4/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-transfer.svg?color=blue)](https://pypi.org/project/types-aiobotocore-transfer)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_transfer/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-transfer)](https://pepy.tech/project/types-aiobotocore-transfer)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.Transfer 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transfer.html#Transfer)
+[aiobotocore.Transfer 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transfer.html#Transfer)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-transfer-2.5.2.post2/setup.py` & `types-aiobotocore-transfer-2.5.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-transfer",
-    version="2.5.2.post2",
+    version="2.5.4",
     packages=["types_aiobotocore_transfer"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.Transfer 2.5.2 service generated with mypy-boto3-builder"
+        "Type annotations for aiobotocore.Transfer 2.5.4 service generated with mypy-boto3-builder"
         " 7.17.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
```

### Comparing `types-aiobotocore-transfer-2.5.2.post2/types_aiobotocore_transfer/__init__.py` & `types-aiobotocore-transfer-2.5.4/types_aiobotocore_transfer/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-transfer-2.5.2.post2/types_aiobotocore_transfer/__init__.pyi` & `types-aiobotocore-transfer-2.5.4/types_aiobotocore_transfer/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-transfer-2.5.2.post2/types_aiobotocore_transfer/__main__.py` & `types-aiobotocore-transfer-2.5.4/types_aiobotocore_transfer/__main__.py`

 * *Files 24% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.Transfer 2.5.2\nVersion:         2.5.2.post2\nBuilder"
-        " version: 7.17.2\nDocs:           "
+        "Type annotations for aiobotocore.Transfer 2.5.4\nVersion:         2.5.4\nBuilder version:"
+        " 7.17.2\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_transfer//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transfer.html#Transfer\nOther"
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

### Comparing `types-aiobotocore-transfer-2.5.2.post2/types_aiobotocore_transfer/client.py` & `types-aiobotocore-transfer-2.5.4/types_aiobotocore_transfer/client.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-transfer-2.5.2.post2/types_aiobotocore_transfer/client.pyi` & `types-aiobotocore-transfer-2.5.4/types_aiobotocore_transfer/client.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-transfer-2.5.2.post2/types_aiobotocore_transfer/literals.py` & `types-aiobotocore-transfer-2.5.4/types_aiobotocore_transfer/literals.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-transfer-2.5.2.post2/types_aiobotocore_transfer/literals.pyi` & `types-aiobotocore-transfer-2.5.4/types_aiobotocore_transfer/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-transfer-2.5.2.post2/types_aiobotocore_transfer/paginator.py` & `types-aiobotocore-transfer-2.5.4/types_aiobotocore_transfer/paginator.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-transfer-2.5.2.post2/types_aiobotocore_transfer/paginator.pyi` & `types-aiobotocore-transfer-2.5.4/types_aiobotocore_transfer/paginator.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-transfer-2.5.2.post2/types_aiobotocore_transfer/type_defs.py` & `types-aiobotocore-transfer-2.5.4/types_aiobotocore_transfer/type_defs.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-transfer-2.5.2.post2/types_aiobotocore_transfer/type_defs.pyi` & `types-aiobotocore-transfer-2.5.4/types_aiobotocore_transfer/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-transfer-2.5.2.post2/types_aiobotocore_transfer/waiter.py` & `types-aiobotocore-transfer-2.5.4/types_aiobotocore_transfer/waiter.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-transfer-2.5.2.post2/types_aiobotocore_transfer/waiter.pyi` & `types-aiobotocore-transfer-2.5.4/types_aiobotocore_transfer/waiter.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-transfer-2.5.2.post2/types_aiobotocore_transfer.egg-info/PKG-INFO` & `types-aiobotocore-transfer-2.5.4/types_aiobotocore_transfer.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-transfer
-Version: 2.5.2.post2
-Summary: Type annotations for aiobotocore.Transfer 2.5.2 service generated with mypy-boto3-builder 7.17.2
+Version: 2.5.4
+Summary: Type annotations for aiobotocore.Transfer 2.5.4 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_transfer/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-transfer.svg?color=blue)](https://pypi.org/project/types-aiobotocore-transfer)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_transfer/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-transfer)](https://pepy.tech/project/types-aiobotocore-transfer)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.Transfer 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transfer.html#Transfer)
+[aiobotocore.Transfer 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transfer.html#Transfer)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-transfer-2.5.2.post2/types_aiobotocore_transfer.egg-info/SOURCES.txt` & `types-aiobotocore-transfer-2.5.4/types_aiobotocore_transfer.egg-info/SOURCES.txt`

 * *Files identical despite different names*


# Comparing `tmp/types-aiobotocore-mq-2.5.2.post2.tar.gz` & `tmp/types-aiobotocore-mq-2.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-mq-2.5.2.post2.tar", last modified: Fri Aug  4 13:59:19 2023, max compression
+gzip compressed data, was "types-aiobotocore-mq-2.5.4.tar", last modified: Tue Aug  8 01:24:08 2023, max compression
```

## Comparing `types-aiobotocore-mq-2.5.2.post2.tar` & `types-aiobotocore-mq-2.5.4.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:19.156643 types-aiobotocore-mq-2.5.2.post2/
--rw-r--r--   0 vlad      (1000) vlad      (1000)     1070 2023-08-04 13:45:16.000000 types-aiobotocore-mq-2.5.2.post2/LICENSE
--rw-r--r--   0 vlad      (1000) vlad      (1000)    12606 2023-08-04 13:59:19.156643 types-aiobotocore-mq-2.5.2.post2/PKG-INFO
--rw-r--r--   0 vlad      (1000) vlad      (1000)    11108 2023-08-04 13:45:16.000000 types-aiobotocore-mq-2.5.2.post2/README.md
--rw-r--r--   0 vlad      (1000) vlad      (1000)       38 2023-08-04 13:59:19.156643 types-aiobotocore-mq-2.5.2.post2/setup.cfg
--rw-r--r--   0 vlad      (1000) vlad      (1000)     2002 2023-08-04 13:45:16.000000 types-aiobotocore-mq-2.5.2.post2/setup.py
-drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:19.156643 types-aiobotocore-mq-2.5.2.post2/types_aiobotocore_mq/
--rw-r--r--   0 vlad      (1000) vlad      (1000)      589 2023-08-04 13:45:16.000000 types-aiobotocore-mq-2.5.2.post2/types_aiobotocore_mq/__init__.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)      588 2023-08-04 13:45:16.000000 types-aiobotocore-mq-2.5.2.post2/types_aiobotocore_mq/__init__.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)      912 2023-08-04 13:45:16.000000 types-aiobotocore-mq-2.5.2.post2/types_aiobotocore_mq/__main__.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)    18730 2023-08-04 13:45:16.000000 types-aiobotocore-mq-2.5.2.post2/types_aiobotocore_mq/client.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)    18697 2023-08-04 13:45:16.000000 types-aiobotocore-mq-2.5.2.post2/types_aiobotocore_mq/client.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)     9414 2023-08-04 13:45:17.000000 types-aiobotocore-mq-2.5.2.post2/types_aiobotocore_mq/literals.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)     9412 2023-08-04 13:45:17.000000 types-aiobotocore-mq-2.5.2.post2/types_aiobotocore_mq/literals.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)     1878 2023-08-04 13:45:16.000000 types-aiobotocore-mq-2.5.2.post2/types_aiobotocore_mq/paginator.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)     1875 2023-08-04 13:45:16.000000 types-aiobotocore-mq-2.5.2.post2/types_aiobotocore_mq/paginator.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:45:16.000000 types-aiobotocore-mq-2.5.2.post2/types_aiobotocore_mq/py.typed
--rw-r--r--   0 vlad      (1000) vlad      (1000)    28037 2023-08-04 13:45:17.000000 types-aiobotocore-mq-2.5.2.post2/types_aiobotocore_mq/type_defs.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)    27990 2023-08-04 13:45:17.000000 types-aiobotocore-mq-2.5.2.post2/types_aiobotocore_mq/type_defs.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)       65 2023-08-04 13:45:16.000000 types-aiobotocore-mq-2.5.2.post2/types_aiobotocore_mq/version.py
-drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:19.156643 types-aiobotocore-mq-2.5.2.post2/types_aiobotocore_mq.egg-info/
--rw-r--r--   0 vlad      (1000) vlad      (1000)    12606 2023-08-04 13:59:19.000000 types-aiobotocore-mq-2.5.2.post2/types_aiobotocore_mq.egg-info/PKG-INFO
--rw-r--r--   0 vlad      (1000) vlad      (1000)      718 2023-08-04 13:59:19.000000 types-aiobotocore-mq-2.5.2.post2/types_aiobotocore_mq.egg-info/SOURCES.txt
--rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:19.000000 types-aiobotocore-mq-2.5.2.post2/types_aiobotocore_mq.egg-info/dependency_links.txt
--rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:19.000000 types-aiobotocore-mq-2.5.2.post2/types_aiobotocore_mq.egg-info/not-zip-safe
--rw-r--r--   0 vlad      (1000) vlad      (1000)       52 2023-08-04 13:59:19.000000 types-aiobotocore-mq-2.5.2.post2/types_aiobotocore_mq.egg-info/requires.txt
--rw-r--r--   0 vlad      (1000) vlad      (1000)       21 2023-08-04 13:59:19.000000 types-aiobotocore-mq-2.5.2.post2/types_aiobotocore_mq.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:24:08.746739 types-aiobotocore-mq-2.5.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-08 01:15:41.000000 types-aiobotocore-mq-2.5.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    12600 2023-08-08 01:24:08.746739 types-aiobotocore-mq-2.5.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    11108 2023-08-08 01:15:41.000000 types-aiobotocore-mq-2.5.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-08 01:24:08.746739 types-aiobotocore-mq-2.5.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1996 2023-08-08 01:15:41.000000 types-aiobotocore-mq-2.5.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:24:08.746739 types-aiobotocore-mq-2.5.4/types_aiobotocore_mq/
+-rw-r--r--   0 runner    (1001) docker     (123)      589 2023-08-08 01:15:41.000000 types-aiobotocore-mq-2.5.4/types_aiobotocore_mq/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      588 2023-08-08 01:15:41.000000 types-aiobotocore-mq-2.5.4/types_aiobotocore_mq/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      900 2023-08-08 01:15:41.000000 types-aiobotocore-mq-2.5.4/types_aiobotocore_mq/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18730 2023-08-08 01:15:41.000000 types-aiobotocore-mq-2.5.4/types_aiobotocore_mq/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18697 2023-08-08 01:15:41.000000 types-aiobotocore-mq-2.5.4/types_aiobotocore_mq/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9414 2023-08-08 01:15:41.000000 types-aiobotocore-mq-2.5.4/types_aiobotocore_mq/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9412 2023-08-08 01:15:41.000000 types-aiobotocore-mq-2.5.4/types_aiobotocore_mq/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1878 2023-08-08 01:15:41.000000 types-aiobotocore-mq-2.5.4/types_aiobotocore_mq/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1875 2023-08-08 01:15:41.000000 types-aiobotocore-mq-2.5.4/types_aiobotocore_mq/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 01:15:41.000000 types-aiobotocore-mq-2.5.4/types_aiobotocore_mq/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    28037 2023-08-08 01:15:42.000000 types-aiobotocore-mq-2.5.4/types_aiobotocore_mq/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27990 2023-08-08 01:15:42.000000 types-aiobotocore-mq-2.5.4/types_aiobotocore_mq/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-08-08 01:15:41.000000 types-aiobotocore-mq-2.5.4/types_aiobotocore_mq/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:24:08.746739 types-aiobotocore-mq-2.5.4/types_aiobotocore_mq.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    12600 2023-08-08 01:24:08.000000 types-aiobotocore-mq-2.5.4/types_aiobotocore_mq.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      718 2023-08-08 01:24:08.000000 types-aiobotocore-mq-2.5.4/types_aiobotocore_mq.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 01:24:08.000000 types-aiobotocore-mq-2.5.4/types_aiobotocore_mq.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 01:24:08.000000 types-aiobotocore-mq-2.5.4/types_aiobotocore_mq.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-08 01:24:08.000000 types-aiobotocore-mq-2.5.4/types_aiobotocore_mq.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-08-08 01:24:08.000000 types-aiobotocore-mq-2.5.4/types_aiobotocore_mq.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-mq-2.5.2.post2/LICENSE` & `types-aiobotocore-mq-2.5.4/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-mq-2.5.2.post2/PKG-INFO` & `types-aiobotocore-mq-2.5.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-mq
-Version: 2.5.2.post2
-Summary: Type annotations for aiobotocore.MQ 2.5.2 service generated with mypy-boto3-builder 7.17.2
+Version: 2.5.4
+Summary: Type annotations for aiobotocore.MQ 2.5.4 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mq/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-mq.svg?color=blue)](https://pypi.org/project/types-aiobotocore-mq)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mq/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-mq)](https://pepy.tech/project/types-aiobotocore-mq)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.MQ 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mq.html#MQ)
+[aiobotocore.MQ 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mq.html#MQ)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-mq-2.5.2.post2/README.md` & `types-aiobotocore-mq-2.5.4/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-mq.svg?color=blue)](https://pypi.org/project/types-aiobotocore-mq)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mq/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-mq)](https://pepy.tech/project/types-aiobotocore-mq)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.MQ 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mq.html#MQ)
+[aiobotocore.MQ 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mq.html#MQ)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-mq-2.5.2.post2/setup.py` & `types-aiobotocore-mq-2.5.4/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-mq",
-    version="2.5.2.post2",
+    version="2.5.4",
     packages=["types_aiobotocore_mq"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.MQ 2.5.2 service generated with mypy-boto3-builder 7.17.2"
+        "Type annotations for aiobotocore.MQ 2.5.4 service generated with mypy-boto3-builder 7.17.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

### Comparing `types-aiobotocore-mq-2.5.2.post2/types_aiobotocore_mq/__init__.py` & `types-aiobotocore-mq-2.5.4/types_aiobotocore_mq/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-mq-2.5.2.post2/types_aiobotocore_mq/__init__.pyi` & `types-aiobotocore-mq-2.5.4/types_aiobotocore_mq/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-mq-2.5.2.post2/types_aiobotocore_mq/__main__.py` & `types-aiobotocore-mq-2.5.4/types_aiobotocore_mq/__main__.py`

 * *Files 13% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.MQ 2.5.2\nVersion:         2.5.2.post2\nBuilder version:"
+        "Type annotations for aiobotocore.MQ 2.5.4\nVersion:         2.5.4\nBuilder version:"
         " 7.17.2\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mq//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mq.html#MQ\nOther"
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

### Comparing `types-aiobotocore-mq-2.5.2.post2/types_aiobotocore_mq/client.py` & `types-aiobotocore-mq-2.5.4/types_aiobotocore_mq/client.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-mq-2.5.2.post2/types_aiobotocore_mq/client.pyi` & `types-aiobotocore-mq-2.5.4/types_aiobotocore_mq/client.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-mq-2.5.2.post2/types_aiobotocore_mq/literals.py` & `types-aiobotocore-mq-2.5.4/types_aiobotocore_mq/literals.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-mq-2.5.2.post2/types_aiobotocore_mq/literals.pyi` & `types-aiobotocore-mq-2.5.4/types_aiobotocore_mq/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-mq-2.5.2.post2/types_aiobotocore_mq/paginator.py` & `types-aiobotocore-mq-2.5.4/types_aiobotocore_mq/paginator.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-mq-2.5.2.post2/types_aiobotocore_mq/paginator.pyi` & `types-aiobotocore-mq-2.5.4/types_aiobotocore_mq/paginator.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-mq-2.5.2.post2/types_aiobotocore_mq/type_defs.py` & `types-aiobotocore-mq-2.5.4/types_aiobotocore_mq/type_defs.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-mq-2.5.2.post2/types_aiobotocore_mq/type_defs.pyi` & `types-aiobotocore-mq-2.5.4/types_aiobotocore_mq/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-mq-2.5.2.post2/types_aiobotocore_mq.egg-info/PKG-INFO` & `types-aiobotocore-mq-2.5.4/types_aiobotocore_mq.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-mq
-Version: 2.5.2.post2
-Summary: Type annotations for aiobotocore.MQ 2.5.2 service generated with mypy-boto3-builder 7.17.2
+Version: 2.5.4
+Summary: Type annotations for aiobotocore.MQ 2.5.4 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mq/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-mq.svg?color=blue)](https://pypi.org/project/types-aiobotocore-mq)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mq/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-mq)](https://pepy.tech/project/types-aiobotocore-mq)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.MQ 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mq.html#MQ)
+[aiobotocore.MQ 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mq.html#MQ)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-mq-2.5.2.post2/types_aiobotocore_mq.egg-info/SOURCES.txt` & `types-aiobotocore-mq-2.5.4/types_aiobotocore_mq.egg-info/SOURCES.txt`

 * *Files identical despite different names*


# Comparing `tmp/types-aiobotocore-ses-2.5.2.post2.tar.gz` & `tmp/types-aiobotocore-ses-2.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-ses-2.5.2.post2.tar", last modified: Fri Aug  4 13:59:26 2023, max compression
+gzip compressed data, was "types-aiobotocore-ses-2.5.4.tar", last modified: Tue Aug  8 01:24:26 2023, max compression
```

## Comparing `types-aiobotocore-ses-2.5.2.post2.tar` & `types-aiobotocore-ses-2.5.4.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:26.626643 types-aiobotocore-ses-2.5.2.post2/
--rw-r--r--   0 vlad      (1000) vlad      (1000)     1070 2023-08-04 13:53:30.000000 types-aiobotocore-ses-2.5.2.post2/LICENSE
--rw-r--r--   0 vlad      (1000) vlad      (1000)    14033 2023-08-04 13:59:26.626643 types-aiobotocore-ses-2.5.2.post2/PKG-INFO
--rw-r--r--   0 vlad      (1000) vlad      (1000)    12531 2023-08-04 13:53:30.000000 types-aiobotocore-ses-2.5.2.post2/README.md
--rw-r--r--   0 vlad      (1000) vlad      (1000)       38 2023-08-04 13:59:26.626643 types-aiobotocore-ses-2.5.2.post2/setup.cfg
--rw-r--r--   0 vlad      (1000) vlad      (1000)     2020 2023-08-04 13:53:30.000000 types-aiobotocore-ses-2.5.2.post2/setup.py
-drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:26.626643 types-aiobotocore-ses-2.5.2.post2/types_aiobotocore_ses/
--rw-r--r--   0 vlad      (1000) vlad      (1000)     1797 2023-08-04 13:53:30.000000 types-aiobotocore-ses-2.5.2.post2/types_aiobotocore_ses/__init__.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)     1796 2023-08-04 13:53:30.000000 types-aiobotocore-ses-2.5.2.post2/types_aiobotocore_ses/__init__.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)      916 2023-08-04 13:53:30.000000 types-aiobotocore-ses-2.5.2.post2/types_aiobotocore_ses/__main__.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)    52059 2023-08-04 13:53:31.000000 types-aiobotocore-ses-2.5.2.post2/types_aiobotocore_ses/client.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)    51973 2023-08-04 13:53:31.000000 types-aiobotocore-ses-2.5.2.post2/types_aiobotocore_ses/client.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)    10983 2023-08-04 13:53:31.000000 types-aiobotocore-ses-2.5.2.post2/types_aiobotocore_ses/literals.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)    10981 2023-08-04 13:53:31.000000 types-aiobotocore-ses-2.5.2.post2/types_aiobotocore_ses/literals.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)     6591 2023-08-04 13:53:31.000000 types-aiobotocore-ses-2.5.2.post2/types_aiobotocore_ses/paginator.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)     6584 2023-08-04 13:53:31.000000 types-aiobotocore-ses-2.5.2.post2/types_aiobotocore_ses/paginator.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:53:30.000000 types-aiobotocore-ses-2.5.2.post2/types_aiobotocore_ses/py.typed
--rw-r--r--   0 vlad      (1000) vlad      (1000)    48024 2023-08-04 13:53:32.000000 types-aiobotocore-ses-2.5.2.post2/types_aiobotocore_ses/type_defs.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)    47961 2023-08-04 13:53:32.000000 types-aiobotocore-ses-2.5.2.post2/types_aiobotocore_ses/type_defs.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)       65 2023-08-04 13:53:30.000000 types-aiobotocore-ses-2.5.2.post2/types_aiobotocore_ses/version.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)     1521 2023-08-04 13:53:31.000000 types-aiobotocore-ses-2.5.2.post2/types_aiobotocore_ses/waiter.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)     1520 2023-08-04 13:53:31.000000 types-aiobotocore-ses-2.5.2.post2/types_aiobotocore_ses/waiter.pyi
-drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:26.626643 types-aiobotocore-ses-2.5.2.post2/types_aiobotocore_ses.egg-info/
--rw-r--r--   0 vlad      (1000) vlad      (1000)    14033 2023-08-04 13:59:26.000000 types-aiobotocore-ses-2.5.2.post2/types_aiobotocore_ses.egg-info/PKG-INFO
--rw-r--r--   0 vlad      (1000) vlad      (1000)      802 2023-08-04 13:59:26.000000 types-aiobotocore-ses-2.5.2.post2/types_aiobotocore_ses.egg-info/SOURCES.txt
--rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:26.000000 types-aiobotocore-ses-2.5.2.post2/types_aiobotocore_ses.egg-info/dependency_links.txt
--rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:26.000000 types-aiobotocore-ses-2.5.2.post2/types_aiobotocore_ses.egg-info/not-zip-safe
--rw-r--r--   0 vlad      (1000) vlad      (1000)       52 2023-08-04 13:59:26.000000 types-aiobotocore-ses-2.5.2.post2/types_aiobotocore_ses.egg-info/requires.txt
--rw-r--r--   0 vlad      (1000) vlad      (1000)       22 2023-08-04 13:59:26.000000 types-aiobotocore-ses-2.5.2.post2/types_aiobotocore_ses.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:24:26.922782 types-aiobotocore-ses-2.5.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-08 01:21:05.000000 types-aiobotocore-ses-2.5.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    14027 2023-08-08 01:24:26.922782 types-aiobotocore-ses-2.5.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    12531 2023-08-08 01:21:05.000000 types-aiobotocore-ses-2.5.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-08 01:24:26.922782 types-aiobotocore-ses-2.5.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2014 2023-08-08 01:21:05.000000 types-aiobotocore-ses-2.5.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:24:26.922782 types-aiobotocore-ses-2.5.4/types_aiobotocore_ses/
+-rw-r--r--   0 runner    (1001) docker     (123)     1797 2023-08-08 01:21:05.000000 types-aiobotocore-ses-2.5.4/types_aiobotocore_ses/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1796 2023-08-08 01:21:05.000000 types-aiobotocore-ses-2.5.4/types_aiobotocore_ses/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      904 2023-08-08 01:21:05.000000 types-aiobotocore-ses-2.5.4/types_aiobotocore_ses/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    52059 2023-08-08 01:21:06.000000 types-aiobotocore-ses-2.5.4/types_aiobotocore_ses/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    51973 2023-08-08 01:21:05.000000 types-aiobotocore-ses-2.5.4/types_aiobotocore_ses/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    10983 2023-08-08 01:21:06.000000 types-aiobotocore-ses-2.5.4/types_aiobotocore_ses/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10981 2023-08-08 01:21:06.000000 types-aiobotocore-ses-2.5.4/types_aiobotocore_ses/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     6591 2023-08-08 01:21:06.000000 types-aiobotocore-ses-2.5.4/types_aiobotocore_ses/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6584 2023-08-08 01:21:06.000000 types-aiobotocore-ses-2.5.4/types_aiobotocore_ses/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 01:21:05.000000 types-aiobotocore-ses-2.5.4/types_aiobotocore_ses/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    48024 2023-08-08 01:21:07.000000 types-aiobotocore-ses-2.5.4/types_aiobotocore_ses/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    47961 2023-08-08 01:21:06.000000 types-aiobotocore-ses-2.5.4/types_aiobotocore_ses/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-08-08 01:21:05.000000 types-aiobotocore-ses-2.5.4/types_aiobotocore_ses/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1521 2023-08-08 01:21:06.000000 types-aiobotocore-ses-2.5.4/types_aiobotocore_ses/waiter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1520 2023-08-08 01:21:06.000000 types-aiobotocore-ses-2.5.4/types_aiobotocore_ses/waiter.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:24:26.922782 types-aiobotocore-ses-2.5.4/types_aiobotocore_ses.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    14027 2023-08-08 01:24:26.000000 types-aiobotocore-ses-2.5.4/types_aiobotocore_ses.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      802 2023-08-08 01:24:26.000000 types-aiobotocore-ses-2.5.4/types_aiobotocore_ses.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 01:24:26.000000 types-aiobotocore-ses-2.5.4/types_aiobotocore_ses.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 01:24:26.000000 types-aiobotocore-ses-2.5.4/types_aiobotocore_ses.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-08 01:24:26.000000 types-aiobotocore-ses-2.5.4/types_aiobotocore_ses.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-08-08 01:24:26.000000 types-aiobotocore-ses-2.5.4/types_aiobotocore_ses.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-ses-2.5.2.post2/LICENSE` & `types-aiobotocore-ses-2.5.4/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-ses-2.5.2.post2/PKG-INFO` & `types-aiobotocore-ses-2.5.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-ses
-Version: 2.5.2.post2
-Summary: Type annotations for aiobotocore.SES 2.5.2 service generated with mypy-boto3-builder 7.17.2
+Version: 2.5.4
+Summary: Type annotations for aiobotocore.SES 2.5.4 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ses/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-ses.svg?color=blue)](https://pypi.org/project/types-aiobotocore-ses)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ses/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-ses)](https://pepy.tech/project/types-aiobotocore-ses)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.SES 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ses.html#SES)
+[aiobotocore.SES 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ses.html#SES)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-ses-2.5.2.post2/README.md` & `types-aiobotocore-ses-2.5.4/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-ses.svg?color=blue)](https://pypi.org/project/types-aiobotocore-ses)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ses/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-ses)](https://pepy.tech/project/types-aiobotocore-ses)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.SES 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ses.html#SES)
+[aiobotocore.SES 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ses.html#SES)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-ses-2.5.2.post2/setup.py` & `types-aiobotocore-ses-2.5.4/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-ses",
-    version="2.5.2.post2",
+    version="2.5.4",
     packages=["types_aiobotocore_ses"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.SES 2.5.2 service generated with mypy-boto3-builder"
+        "Type annotations for aiobotocore.SES 2.5.4 service generated with mypy-boto3-builder"
         " 7.17.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
```

### Comparing `types-aiobotocore-ses-2.5.2.post2/types_aiobotocore_ses/__init__.py` & `types-aiobotocore-ses-2.5.4/types_aiobotocore_ses/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-ses-2.5.2.post2/types_aiobotocore_ses/__init__.pyi` & `types-aiobotocore-ses-2.5.4/types_aiobotocore_ses/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-ses-2.5.2.post2/types_aiobotocore_ses/__main__.py` & `types-aiobotocore-ses-2.5.4/types_aiobotocore_ses/__main__.py`

 * *Files 21% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.SES 2.5.2\nVersion:         2.5.2.post2\nBuilder version:"
+        "Type annotations for aiobotocore.SES 2.5.4\nVersion:         2.5.4\nBuilder version:"
         " 7.17.2\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ses//\nBoto3 docs:    "
         "  https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ses.html#SES\nOther"
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

### Comparing `types-aiobotocore-ses-2.5.2.post2/types_aiobotocore_ses/client.py` & `types-aiobotocore-ses-2.5.4/types_aiobotocore_ses/client.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-ses-2.5.2.post2/types_aiobotocore_ses/client.pyi` & `types-aiobotocore-ses-2.5.4/types_aiobotocore_ses/client.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-ses-2.5.2.post2/types_aiobotocore_ses/literals.py` & `types-aiobotocore-ses-2.5.4/types_aiobotocore_ses/literals.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-ses-2.5.2.post2/types_aiobotocore_ses/literals.pyi` & `types-aiobotocore-ses-2.5.4/types_aiobotocore_ses/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-ses-2.5.2.post2/types_aiobotocore_ses/paginator.py` & `types-aiobotocore-ses-2.5.4/types_aiobotocore_ses/paginator.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-ses-2.5.2.post2/types_aiobotocore_ses/paginator.pyi` & `types-aiobotocore-ses-2.5.4/types_aiobotocore_ses/paginator.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-ses-2.5.2.post2/types_aiobotocore_ses/type_defs.py` & `types-aiobotocore-ses-2.5.4/types_aiobotocore_ses/type_defs.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-ses-2.5.2.post2/types_aiobotocore_ses/type_defs.pyi` & `types-aiobotocore-ses-2.5.4/types_aiobotocore_ses/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-ses-2.5.2.post2/types_aiobotocore_ses/waiter.py` & `types-aiobotocore-ses-2.5.4/types_aiobotocore_ses/waiter.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-ses-2.5.2.post2/types_aiobotocore_ses/waiter.pyi` & `types-aiobotocore-ses-2.5.4/types_aiobotocore_ses/waiter.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-ses-2.5.2.post2/types_aiobotocore_ses.egg-info/PKG-INFO` & `types-aiobotocore-ses-2.5.4/types_aiobotocore_ses.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-ses
-Version: 2.5.2.post2
-Summary: Type annotations for aiobotocore.SES 2.5.2 service generated with mypy-boto3-builder 7.17.2
+Version: 2.5.4
+Summary: Type annotations for aiobotocore.SES 2.5.4 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ses/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-ses.svg?color=blue)](https://pypi.org/project/types-aiobotocore-ses)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ses/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-ses)](https://pepy.tech/project/types-aiobotocore-ses)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.SES 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ses.html#SES)
+[aiobotocore.SES 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ses.html#SES)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-ses-2.5.2.post2/types_aiobotocore_ses.egg-info/SOURCES.txt` & `types-aiobotocore-ses-2.5.4/types_aiobotocore_ses.egg-info/SOURCES.txt`

 * *Files identical despite different names*


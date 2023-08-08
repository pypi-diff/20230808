# Comparing `tmp/types-aiobotocore-redshift-2.5.2.post2.tar.gz` & `tmp/types-aiobotocore-redshift-2.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-redshift-2.5.2.post2.tar", last modified: Fri Aug  4 13:59:22 2023, max compression
+gzip compressed data, was "types-aiobotocore-redshift-2.5.4.tar", last modified: Tue Aug  8 01:24:17 2023, max compression
```

## Comparing `types-aiobotocore-redshift-2.5.2.post2.tar` & `types-aiobotocore-redshift-2.5.4.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:22.766643 types-aiobotocore-redshift-2.5.2.post2/
--rw-r--r--   0 vlad      (1000) vlad      (1000)     1070 2023-08-04 13:50:19.000000 types-aiobotocore-redshift-2.5.2.post2/LICENSE
--rw-r--r--   0 vlad      (1000) vlad      (1000)    20300 2023-08-04 13:59:22.766643 types-aiobotocore-redshift-2.5.2.post2/PKG-INFO
--rw-r--r--   0 vlad      (1000) vlad      (1000)    18778 2023-08-04 13:50:19.000000 types-aiobotocore-redshift-2.5.2.post2/README.md
--rw-r--r--   0 vlad      (1000) vlad      (1000)       38 2023-08-04 13:59:22.766643 types-aiobotocore-redshift-2.5.2.post2/setup.cfg
--rw-r--r--   0 vlad      (1000) vlad      (1000)     2079 2023-08-04 13:50:19.000000 types-aiobotocore-redshift-2.5.2.post2/setup.py
-drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:22.766643 types-aiobotocore-redshift-2.5.2.post2/types_aiobotocore_redshift/
--rw-r--r--   0 vlad      (1000) vlad      (1000)    10002 2023-08-04 13:50:19.000000 types-aiobotocore-redshift-2.5.2.post2/types_aiobotocore_redshift/__init__.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)    10001 2023-08-04 13:50:19.000000 types-aiobotocore-redshift-2.5.2.post2/types_aiobotocore_redshift/__init__.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)      947 2023-08-04 13:50:19.000000 types-aiobotocore-redshift-2.5.2.post2/types_aiobotocore_redshift/__main__.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)   119965 2023-08-04 13:50:20.000000 types-aiobotocore-redshift-2.5.2.post2/types_aiobotocore_redshift/client.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)   119796 2023-08-04 13:50:20.000000 types-aiobotocore-redshift-2.5.2.post2/types_aiobotocore_redshift/client.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)    17391 2023-08-04 13:50:21.000000 types-aiobotocore-redshift-2.5.2.post2/types_aiobotocore_redshift/literals.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)    17389 2023-08-04 13:50:21.000000 types-aiobotocore-redshift-2.5.2.post2/types_aiobotocore_redshift/literals.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)    45116 2023-08-04 13:50:20.000000 types-aiobotocore-redshift-2.5.2.post2/types_aiobotocore_redshift/paginator.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)    45081 2023-08-04 13:50:20.000000 types-aiobotocore-redshift-2.5.2.post2/types_aiobotocore_redshift/paginator.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:50:19.000000 types-aiobotocore-redshift-2.5.2.post2/types_aiobotocore_redshift/py.typed
--rw-r--r--   0 vlad      (1000) vlad      (1000)   134049 2023-08-04 13:50:24.000000 types-aiobotocore-redshift-2.5.2.post2/types_aiobotocore_redshift/type_defs.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)   133930 2023-08-04 13:50:23.000000 types-aiobotocore-redshift-2.5.2.post2/types_aiobotocore_redshift/type_defs.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)       65 2023-08-04 13:50:19.000000 types-aiobotocore-redshift-2.5.2.post2/types_aiobotocore_redshift/version.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)     5583 2023-08-04 13:50:21.000000 types-aiobotocore-redshift-2.5.2.post2/types_aiobotocore_redshift/waiter.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)     5579 2023-08-04 13:50:21.000000 types-aiobotocore-redshift-2.5.2.post2/types_aiobotocore_redshift/waiter.pyi
-drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:22.766643 types-aiobotocore-redshift-2.5.2.post2/types_aiobotocore_redshift.egg-info/
--rw-r--r--   0 vlad      (1000) vlad      (1000)    20300 2023-08-04 13:59:22.000000 types-aiobotocore-redshift-2.5.2.post2/types_aiobotocore_redshift.egg-info/PKG-INFO
--rw-r--r--   0 vlad      (1000) vlad      (1000)      907 2023-08-04 13:59:22.000000 types-aiobotocore-redshift-2.5.2.post2/types_aiobotocore_redshift.egg-info/SOURCES.txt
--rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:22.000000 types-aiobotocore-redshift-2.5.2.post2/types_aiobotocore_redshift.egg-info/dependency_links.txt
--rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:22.000000 types-aiobotocore-redshift-2.5.2.post2/types_aiobotocore_redshift.egg-info/not-zip-safe
--rw-r--r--   0 vlad      (1000) vlad      (1000)       52 2023-08-04 13:59:22.000000 types-aiobotocore-redshift-2.5.2.post2/types_aiobotocore_redshift.egg-info/requires.txt
--rw-r--r--   0 vlad      (1000) vlad      (1000)       27 2023-08-04 13:59:22.000000 types-aiobotocore-redshift-2.5.2.post2/types_aiobotocore_redshift.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:24:17.906760 types-aiobotocore-redshift-2.5.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-08 01:19:07.000000 types-aiobotocore-redshift-2.5.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    20294 2023-08-08 01:24:17.898759 types-aiobotocore-redshift-2.5.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    18778 2023-08-08 01:19:07.000000 types-aiobotocore-redshift-2.5.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-08 01:24:17.906760 types-aiobotocore-redshift-2.5.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2073 2023-08-08 01:19:07.000000 types-aiobotocore-redshift-2.5.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:24:17.898759 types-aiobotocore-redshift-2.5.4/types_aiobotocore_redshift/
+-rw-r--r--   0 runner    (1001) docker     (123)    10002 2023-08-08 01:19:07.000000 types-aiobotocore-redshift-2.5.4/types_aiobotocore_redshift/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10001 2023-08-08 01:19:07.000000 types-aiobotocore-redshift-2.5.4/types_aiobotocore_redshift/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      935 2023-08-08 01:19:07.000000 types-aiobotocore-redshift-2.5.4/types_aiobotocore_redshift/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   119965 2023-08-08 01:19:08.000000 types-aiobotocore-redshift-2.5.4/types_aiobotocore_redshift/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)   119796 2023-08-08 01:19:08.000000 types-aiobotocore-redshift-2.5.4/types_aiobotocore_redshift/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    17391 2023-08-08 01:19:09.000000 types-aiobotocore-redshift-2.5.4/types_aiobotocore_redshift/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17389 2023-08-08 01:19:09.000000 types-aiobotocore-redshift-2.5.4/types_aiobotocore_redshift/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    45116 2023-08-08 01:19:08.000000 types-aiobotocore-redshift-2.5.4/types_aiobotocore_redshift/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    45081 2023-08-08 01:19:08.000000 types-aiobotocore-redshift-2.5.4/types_aiobotocore_redshift/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 01:19:07.000000 types-aiobotocore-redshift-2.5.4/types_aiobotocore_redshift/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)   134049 2023-08-08 01:19:11.000000 types-aiobotocore-redshift-2.5.4/types_aiobotocore_redshift/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)   133930 2023-08-08 01:19:10.000000 types-aiobotocore-redshift-2.5.4/types_aiobotocore_redshift/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-08-08 01:19:07.000000 types-aiobotocore-redshift-2.5.4/types_aiobotocore_redshift/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5583 2023-08-08 01:19:08.000000 types-aiobotocore-redshift-2.5.4/types_aiobotocore_redshift/waiter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5579 2023-08-08 01:19:08.000000 types-aiobotocore-redshift-2.5.4/types_aiobotocore_redshift/waiter.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:24:17.898759 types-aiobotocore-redshift-2.5.4/types_aiobotocore_redshift.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    20294 2023-08-08 01:24:17.000000 types-aiobotocore-redshift-2.5.4/types_aiobotocore_redshift.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      907 2023-08-08 01:24:17.000000 types-aiobotocore-redshift-2.5.4/types_aiobotocore_redshift.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 01:24:17.000000 types-aiobotocore-redshift-2.5.4/types_aiobotocore_redshift.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 01:24:17.000000 types-aiobotocore-redshift-2.5.4/types_aiobotocore_redshift.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-08 01:24:17.000000 types-aiobotocore-redshift-2.5.4/types_aiobotocore_redshift.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-08-08 01:24:17.000000 types-aiobotocore-redshift-2.5.4/types_aiobotocore_redshift.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-redshift-2.5.2.post2/LICENSE` & `types-aiobotocore-redshift-2.5.4/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-redshift-2.5.2.post2/PKG-INFO` & `types-aiobotocore-redshift-2.5.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-redshift
-Version: 2.5.2.post2
-Summary: Type annotations for aiobotocore.Redshift 2.5.2 service generated with mypy-boto3-builder 7.17.2
+Version: 2.5.4
+Summary: Type annotations for aiobotocore.Redshift 2.5.4 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-redshift.svg?color=blue)](https://pypi.org/project/types-aiobotocore-redshift)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-redshift)](https://pepy.tech/project/types-aiobotocore-redshift)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.Redshift 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift)
+[aiobotocore.Redshift 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-redshift-2.5.2.post2/README.md` & `types-aiobotocore-redshift-2.5.4/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-redshift.svg?color=blue)](https://pypi.org/project/types-aiobotocore-redshift)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-redshift)](https://pepy.tech/project/types-aiobotocore-redshift)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.Redshift 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift)
+[aiobotocore.Redshift 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-redshift-2.5.2.post2/setup.py` & `types-aiobotocore-redshift-2.5.4/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-redshift",
-    version="2.5.2.post2",
+    version="2.5.4",
     packages=["types_aiobotocore_redshift"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.Redshift 2.5.2 service generated with mypy-boto3-builder"
+        "Type annotations for aiobotocore.Redshift 2.5.4 service generated with mypy-boto3-builder"
         " 7.17.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
```

### Comparing `types-aiobotocore-redshift-2.5.2.post2/types_aiobotocore_redshift/__init__.py` & `types-aiobotocore-redshift-2.5.4/types_aiobotocore_redshift/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-redshift-2.5.2.post2/types_aiobotocore_redshift/__init__.pyi` & `types-aiobotocore-redshift-2.5.4/types_aiobotocore_redshift/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-redshift-2.5.2.post2/types_aiobotocore_redshift/__main__.py` & `types-aiobotocore-redshift-2.5.4/types_aiobotocore_redshift/__main__.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.Redshift 2.5.2\nVersion:         2.5.2.post2\nBuilder"
-        " version: 7.17.2\nDocs:           "
+        "Type annotations for aiobotocore.Redshift 2.5.4\nVersion:         2.5.4\nBuilder version:"
+        " 7.17.2\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift\nOther"
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

### Comparing `types-aiobotocore-redshift-2.5.2.post2/types_aiobotocore_redshift/client.py` & `types-aiobotocore-redshift-2.5.4/types_aiobotocore_redshift/client.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-redshift-2.5.2.post2/types_aiobotocore_redshift/client.pyi` & `types-aiobotocore-redshift-2.5.4/types_aiobotocore_redshift/client.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-redshift-2.5.2.post2/types_aiobotocore_redshift/literals.py` & `types-aiobotocore-redshift-2.5.4/types_aiobotocore_redshift/literals.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-redshift-2.5.2.post2/types_aiobotocore_redshift/literals.pyi` & `types-aiobotocore-redshift-2.5.4/types_aiobotocore_redshift/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-redshift-2.5.2.post2/types_aiobotocore_redshift/paginator.py` & `types-aiobotocore-redshift-2.5.4/types_aiobotocore_redshift/paginator.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-redshift-2.5.2.post2/types_aiobotocore_redshift/paginator.pyi` & `types-aiobotocore-redshift-2.5.4/types_aiobotocore_redshift/paginator.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-redshift-2.5.2.post2/types_aiobotocore_redshift/type_defs.py` & `types-aiobotocore-redshift-2.5.4/types_aiobotocore_redshift/type_defs.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-redshift-2.5.2.post2/types_aiobotocore_redshift/type_defs.pyi` & `types-aiobotocore-redshift-2.5.4/types_aiobotocore_redshift/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-redshift-2.5.2.post2/types_aiobotocore_redshift/waiter.py` & `types-aiobotocore-redshift-2.5.4/types_aiobotocore_redshift/waiter.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-redshift-2.5.2.post2/types_aiobotocore_redshift/waiter.pyi` & `types-aiobotocore-redshift-2.5.4/types_aiobotocore_redshift/waiter.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-redshift-2.5.2.post2/types_aiobotocore_redshift.egg-info/PKG-INFO` & `types-aiobotocore-redshift-2.5.4/types_aiobotocore_redshift.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-redshift
-Version: 2.5.2.post2
-Summary: Type annotations for aiobotocore.Redshift 2.5.2 service generated with mypy-boto3-builder 7.17.2
+Version: 2.5.4
+Summary: Type annotations for aiobotocore.Redshift 2.5.4 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-redshift.svg?color=blue)](https://pypi.org/project/types-aiobotocore-redshift)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-redshift)](https://pepy.tech/project/types-aiobotocore-redshift)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.Redshift 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift)
+[aiobotocore.Redshift 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-redshift-2.5.2.post2/types_aiobotocore_redshift.egg-info/SOURCES.txt` & `types-aiobotocore-redshift-2.5.4/types_aiobotocore_redshift.egg-info/SOURCES.txt`

 * *Files identical despite different names*


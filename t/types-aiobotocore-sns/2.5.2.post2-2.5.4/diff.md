# Comparing `tmp/types-aiobotocore-sns-2.5.2.post2.tar.gz` & `tmp/types-aiobotocore-sns-2.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-sns-2.5.2.post2.tar", last modified: Fri Aug  4 13:59:27 2023, max compression
+gzip compressed data, was "types-aiobotocore-sns-2.5.4.tar", last modified: Tue Aug  8 01:24:29 2023, max compression
```

## Comparing `types-aiobotocore-sns-2.5.2.post2.tar` & `types-aiobotocore-sns-2.5.4.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:27.356643 types-aiobotocore-sns-2.5.2.post2/
--rw-r--r--   0 vlad      (1000) vlad      (1000)     1070 2023-08-04 13:53:55.000000 types-aiobotocore-sns-2.5.2.post2/LICENSE
--rw-r--r--   0 vlad      (1000) vlad      (1000)    16539 2023-08-04 13:59:27.336643 types-aiobotocore-sns-2.5.2.post2/PKG-INFO
--rw-r--r--   0 vlad      (1000) vlad      (1000)    15037 2023-08-04 13:53:55.000000 types-aiobotocore-sns-2.5.2.post2/README.md
--rw-r--r--   0 vlad      (1000) vlad      (1000)       38 2023-08-04 13:59:27.356643 types-aiobotocore-sns-2.5.2.post2/setup.cfg
--rw-r--r--   0 vlad      (1000) vlad      (1000)     2020 2023-08-04 13:53:55.000000 types-aiobotocore-sns-2.5.2.post2/setup.py
-drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:27.336643 types-aiobotocore-sns-2.5.2.post2/types_aiobotocore_sns/
--rw-r--r--   0 vlad      (1000) vlad      (1000)     2599 2023-08-04 13:53:55.000000 types-aiobotocore-sns-2.5.2.post2/types_aiobotocore_sns/__init__.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)     2597 2023-08-04 13:53:55.000000 types-aiobotocore-sns-2.5.2.post2/types_aiobotocore_sns/__init__.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)      916 2023-08-04 13:53:55.000000 types-aiobotocore-sns-2.5.2.post2/types_aiobotocore_sns/__main__.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)    35353 2023-08-04 13:53:55.000000 types-aiobotocore-sns-2.5.2.post2/types_aiobotocore_sns/client.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)    35294 2023-08-04 13:53:55.000000 types-aiobotocore-sns-2.5.2.post2/types_aiobotocore_sns/client.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)     9976 2023-08-04 13:53:59.000000 types-aiobotocore-sns-2.5.2.post2/types_aiobotocore_sns/literals.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)     9974 2023-08-04 13:53:59.000000 types-aiobotocore-sns-2.5.2.post2/types_aiobotocore_sns/literals.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)    10074 2023-08-04 13:53:59.000000 types-aiobotocore-sns-2.5.2.post2/types_aiobotocore_sns/paginator.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)    10064 2023-08-04 13:53:59.000000 types-aiobotocore-sns-2.5.2.post2/types_aiobotocore_sns/paginator.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:53:55.000000 types-aiobotocore-sns-2.5.2.post2/types_aiobotocore_sns/py.typed
--rw-r--r--   0 vlad      (1000) vlad      (1000)    37388 2023-08-04 13:53:59.000000 types-aiobotocore-sns-2.5.2.post2/types_aiobotocore_sns/service_resource.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)    37313 2023-08-04 13:53:59.000000 types-aiobotocore-sns-2.5.2.post2/types_aiobotocore_sns/service_resource.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)    34610 2023-08-04 13:54:00.000000 types-aiobotocore-sns-2.5.2.post2/types_aiobotocore_sns/type_defs.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)    34563 2023-08-04 13:54:00.000000 types-aiobotocore-sns-2.5.2.post2/types_aiobotocore_sns/type_defs.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)       65 2023-08-04 13:53:55.000000 types-aiobotocore-sns-2.5.2.post2/types_aiobotocore_sns/version.py
-drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:27.336643 types-aiobotocore-sns-2.5.2.post2/types_aiobotocore_sns.egg-info/
--rw-r--r--   0 vlad      (1000) vlad      (1000)    16539 2023-08-04 13:59:27.000000 types-aiobotocore-sns-2.5.2.post2/types_aiobotocore_sns.egg-info/PKG-INFO
--rw-r--r--   0 vlad      (1000) vlad      (1000)      822 2023-08-04 13:59:27.000000 types-aiobotocore-sns-2.5.2.post2/types_aiobotocore_sns.egg-info/SOURCES.txt
--rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:27.000000 types-aiobotocore-sns-2.5.2.post2/types_aiobotocore_sns.egg-info/dependency_links.txt
--rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:27.000000 types-aiobotocore-sns-2.5.2.post2/types_aiobotocore_sns.egg-info/not-zip-safe
--rw-r--r--   0 vlad      (1000) vlad      (1000)       52 2023-08-04 13:59:27.000000 types-aiobotocore-sns-2.5.2.post2/types_aiobotocore_sns.egg-info/requires.txt
--rw-r--r--   0 vlad      (1000) vlad      (1000)       22 2023-08-04 13:59:27.000000 types-aiobotocore-sns-2.5.2.post2/types_aiobotocore_sns.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:24:29.190788 types-aiobotocore-sns-2.5.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-08 01:21:20.000000 types-aiobotocore-sns-2.5.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    16533 2023-08-08 01:24:29.186788 types-aiobotocore-sns-2.5.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    15037 2023-08-08 01:21:20.000000 types-aiobotocore-sns-2.5.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-08 01:24:29.190788 types-aiobotocore-sns-2.5.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2014 2023-08-08 01:21:20.000000 types-aiobotocore-sns-2.5.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:24:29.186788 types-aiobotocore-sns-2.5.4/types_aiobotocore_sns/
+-rw-r--r--   0 runner    (1001) docker     (123)     2599 2023-08-08 01:21:20.000000 types-aiobotocore-sns-2.5.4/types_aiobotocore_sns/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2597 2023-08-08 01:21:20.000000 types-aiobotocore-sns-2.5.4/types_aiobotocore_sns/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      904 2023-08-08 01:21:20.000000 types-aiobotocore-sns-2.5.4/types_aiobotocore_sns/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35353 2023-08-08 01:21:20.000000 types-aiobotocore-sns-2.5.4/types_aiobotocore_sns/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35294 2023-08-08 01:21:20.000000 types-aiobotocore-sns-2.5.4/types_aiobotocore_sns/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9976 2023-08-08 01:21:21.000000 types-aiobotocore-sns-2.5.4/types_aiobotocore_sns/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9974 2023-08-08 01:21:21.000000 types-aiobotocore-sns-2.5.4/types_aiobotocore_sns/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    10074 2023-08-08 01:21:21.000000 types-aiobotocore-sns-2.5.4/types_aiobotocore_sns/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10064 2023-08-08 01:21:21.000000 types-aiobotocore-sns-2.5.4/types_aiobotocore_sns/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 01:21:20.000000 types-aiobotocore-sns-2.5.4/types_aiobotocore_sns/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    37388 2023-08-08 01:21:21.000000 types-aiobotocore-sns-2.5.4/types_aiobotocore_sns/service_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37313 2023-08-08 01:21:21.000000 types-aiobotocore-sns-2.5.4/types_aiobotocore_sns/service_resource.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    34610 2023-08-08 01:21:21.000000 types-aiobotocore-sns-2.5.4/types_aiobotocore_sns/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34563 2023-08-08 01:21:21.000000 types-aiobotocore-sns-2.5.4/types_aiobotocore_sns/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-08-08 01:21:20.000000 types-aiobotocore-sns-2.5.4/types_aiobotocore_sns/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:24:29.186788 types-aiobotocore-sns-2.5.4/types_aiobotocore_sns.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    16533 2023-08-08 01:24:29.000000 types-aiobotocore-sns-2.5.4/types_aiobotocore_sns.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      822 2023-08-08 01:24:29.000000 types-aiobotocore-sns-2.5.4/types_aiobotocore_sns.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 01:24:29.000000 types-aiobotocore-sns-2.5.4/types_aiobotocore_sns.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 01:24:29.000000 types-aiobotocore-sns-2.5.4/types_aiobotocore_sns.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-08 01:24:29.000000 types-aiobotocore-sns-2.5.4/types_aiobotocore_sns.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-08-08 01:24:29.000000 types-aiobotocore-sns-2.5.4/types_aiobotocore_sns.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-sns-2.5.2.post2/LICENSE` & `types-aiobotocore-sns-2.5.4/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-sns-2.5.2.post2/PKG-INFO` & `types-aiobotocore-sns-2.5.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-sns
-Version: 2.5.2.post2
-Summary: Type annotations for aiobotocore.SNS 2.5.2 service generated with mypy-boto3-builder 7.17.2
+Version: 2.5.4
+Summary: Type annotations for aiobotocore.SNS 2.5.4 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sns/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-sns.svg?color=blue)](https://pypi.org/project/types-aiobotocore-sns)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sns/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-sns)](https://pepy.tech/project/types-aiobotocore-sns)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.SNS 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sns.html#SNS)
+[aiobotocore.SNS 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sns.html#SNS)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-sns-2.5.2.post2/README.md` & `types-aiobotocore-sns-2.5.4/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-sns.svg?color=blue)](https://pypi.org/project/types-aiobotocore-sns)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sns/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-sns)](https://pepy.tech/project/types-aiobotocore-sns)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.SNS 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sns.html#SNS)
+[aiobotocore.SNS 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sns.html#SNS)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-sns-2.5.2.post2/setup.py` & `types-aiobotocore-sns-2.5.4/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-sns",
-    version="2.5.2.post2",
+    version="2.5.4",
     packages=["types_aiobotocore_sns"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.SNS 2.5.2 service generated with mypy-boto3-builder"
+        "Type annotations for aiobotocore.SNS 2.5.4 service generated with mypy-boto3-builder"
         " 7.17.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
```

### Comparing `types-aiobotocore-sns-2.5.2.post2/types_aiobotocore_sns/__init__.py` & `types-aiobotocore-sns-2.5.4/types_aiobotocore_sns/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-sns-2.5.2.post2/types_aiobotocore_sns/__init__.pyi` & `types-aiobotocore-sns-2.5.4/types_aiobotocore_sns/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-sns-2.5.2.post2/types_aiobotocore_sns/__main__.py` & `types-aiobotocore-sns-2.5.4/types_aiobotocore_sns/__main__.py`

 * *Files 13% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.SNS 2.5.2\nVersion:         2.5.2.post2\nBuilder version:"
+        "Type annotations for aiobotocore.SNS 2.5.4\nVersion:         2.5.4\nBuilder version:"
         " 7.17.2\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sns//\nBoto3 docs:    "
         "  https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sns.html#SNS\nOther"
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

### Comparing `types-aiobotocore-sns-2.5.2.post2/types_aiobotocore_sns/client.py` & `types-aiobotocore-sns-2.5.4/types_aiobotocore_sns/client.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-sns-2.5.2.post2/types_aiobotocore_sns/client.pyi` & `types-aiobotocore-sns-2.5.4/types_aiobotocore_sns/client.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-sns-2.5.2.post2/types_aiobotocore_sns/literals.py` & `types-aiobotocore-sns-2.5.4/types_aiobotocore_sns/literals.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-sns-2.5.2.post2/types_aiobotocore_sns/literals.pyi` & `types-aiobotocore-sns-2.5.4/types_aiobotocore_sns/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-sns-2.5.2.post2/types_aiobotocore_sns/paginator.py` & `types-aiobotocore-sns-2.5.4/types_aiobotocore_sns/paginator.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-sns-2.5.2.post2/types_aiobotocore_sns/paginator.pyi` & `types-aiobotocore-sns-2.5.4/types_aiobotocore_sns/paginator.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-sns-2.5.2.post2/types_aiobotocore_sns/service_resource.py` & `types-aiobotocore-sns-2.5.4/types_aiobotocore_sns/service_resource.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-sns-2.5.2.post2/types_aiobotocore_sns/service_resource.pyi` & `types-aiobotocore-sns-2.5.4/types_aiobotocore_sns/service_resource.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-sns-2.5.2.post2/types_aiobotocore_sns/type_defs.py` & `types-aiobotocore-sns-2.5.4/types_aiobotocore_sns/type_defs.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-sns-2.5.2.post2/types_aiobotocore_sns/type_defs.pyi` & `types-aiobotocore-sns-2.5.4/types_aiobotocore_sns/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-sns-2.5.2.post2/types_aiobotocore_sns.egg-info/PKG-INFO` & `types-aiobotocore-sns-2.5.4/types_aiobotocore_sns.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-sns
-Version: 2.5.2.post2
-Summary: Type annotations for aiobotocore.SNS 2.5.2 service generated with mypy-boto3-builder 7.17.2
+Version: 2.5.4
+Summary: Type annotations for aiobotocore.SNS 2.5.4 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sns/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-sns.svg?color=blue)](https://pypi.org/project/types-aiobotocore-sns)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sns/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-sns)](https://pepy.tech/project/types-aiobotocore-sns)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.SNS 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sns.html#SNS)
+[aiobotocore.SNS 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sns.html#SNS)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-sns-2.5.2.post2/types_aiobotocore_sns.egg-info/SOURCES.txt` & `types-aiobotocore-sns-2.5.4/types_aiobotocore_sns.egg-info/SOURCES.txt`

 * *Files identical despite different names*


# Comparing `tmp/types-aiobotocore-translate-2.5.2.post2.tar.gz` & `tmp/types-aiobotocore-translate-2.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-translate-2.5.2.post2.tar", last modified: Fri Aug  4 13:59:29 2023, max compression
+gzip compressed data, was "types-aiobotocore-translate-2.5.4.tar", last modified: Tue Aug  8 01:24:34 2023, max compression
```

## Comparing `types-aiobotocore-translate-2.5.2.post2.tar` & `types-aiobotocore-translate-2.5.4.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:29.196643 types-aiobotocore-translate-2.5.2.post2/
--rw-r--r--   0 vlad      (1000) vlad      (1000)     1070 2023-08-04 13:55:21.000000 types-aiobotocore-translate-2.5.2.post2/LICENSE
--rw-r--r--   0 vlad      (1000) vlad      (1000)    13023 2023-08-04 13:59:29.196643 types-aiobotocore-translate-2.5.2.post2/PKG-INFO
--rw-r--r--   0 vlad      (1000) vlad      (1000)    11497 2023-08-04 13:55:21.000000 types-aiobotocore-translate-2.5.2.post2/README.md
--rw-r--r--   0 vlad      (1000) vlad      (1000)       38 2023-08-04 13:59:29.196643 types-aiobotocore-translate-2.5.2.post2/setup.cfg
--rw-r--r--   0 vlad      (1000) vlad      (1000)     2086 2023-08-04 13:55:21.000000 types-aiobotocore-translate-2.5.2.post2/setup.py
-drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:29.196643 types-aiobotocore-translate-2.5.2.post2/types_aiobotocore_translate/
--rw-r--r--   0 vlad      (1000) vlad      (1000)      681 2023-08-04 13:55:21.000000 types-aiobotocore-translate-2.5.2.post2/types_aiobotocore_translate/__init__.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)      680 2023-08-04 13:55:21.000000 types-aiobotocore-translate-2.5.2.post2/types_aiobotocore_translate/__init__.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)      951 2023-08-04 13:55:21.000000 types-aiobotocore-translate-2.5.2.post2/types_aiobotocore_translate/__main__.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)    18162 2023-08-04 13:55:21.000000 types-aiobotocore-translate-2.5.2.post2/types_aiobotocore_translate/client.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)    18133 2023-08-04 13:55:21.000000 types-aiobotocore-translate-2.5.2.post2/types_aiobotocore_translate/client.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)     9061 2023-08-04 13:55:21.000000 types-aiobotocore-translate-2.5.2.post2/types_aiobotocore_translate/literals.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)     9059 2023-08-04 13:55:21.000000 types-aiobotocore-translate-2.5.2.post2/types_aiobotocore_translate/literals.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)     2041 2023-08-04 13:55:21.000000 types-aiobotocore-translate-2.5.2.post2/types_aiobotocore_translate/paginator.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)     2038 2023-08-04 13:55:21.000000 types-aiobotocore-translate-2.5.2.post2/types_aiobotocore_translate/paginator.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:55:21.000000 types-aiobotocore-translate-2.5.2.post2/types_aiobotocore_translate/py.typed
--rw-r--r--   0 vlad      (1000) vlad      (1000)    20212 2023-08-04 13:55:22.000000 types-aiobotocore-translate-2.5.2.post2/types_aiobotocore_translate/type_defs.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)    20193 2023-08-04 13:55:21.000000 types-aiobotocore-translate-2.5.2.post2/types_aiobotocore_translate/type_defs.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)       65 2023-08-04 13:55:21.000000 types-aiobotocore-translate-2.5.2.post2/types_aiobotocore_translate/version.py
-drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:29.196643 types-aiobotocore-translate-2.5.2.post2/types_aiobotocore_translate.egg-info/
--rw-r--r--   0 vlad      (1000) vlad      (1000)    13023 2023-08-04 13:59:29.000000 types-aiobotocore-translate-2.5.2.post2/types_aiobotocore_translate.egg-info/PKG-INFO
--rw-r--r--   0 vlad      (1000) vlad      (1000)      851 2023-08-04 13:59:29.000000 types-aiobotocore-translate-2.5.2.post2/types_aiobotocore_translate.egg-info/SOURCES.txt
--rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:29.000000 types-aiobotocore-translate-2.5.2.post2/types_aiobotocore_translate.egg-info/dependency_links.txt
--rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:29.000000 types-aiobotocore-translate-2.5.2.post2/types_aiobotocore_translate.egg-info/not-zip-safe
--rw-r--r--   0 vlad      (1000) vlad      (1000)       52 2023-08-04 13:59:29.000000 types-aiobotocore-translate-2.5.2.post2/types_aiobotocore_translate.egg-info/requires.txt
--rw-r--r--   0 vlad      (1000) vlad      (1000)       28 2023-08-04 13:59:29.000000 types-aiobotocore-translate-2.5.2.post2/types_aiobotocore_translate.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:24:34.118799 types-aiobotocore-translate-2.5.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-08 01:22:10.000000 types-aiobotocore-translate-2.5.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    13017 2023-08-08 01:24:34.110799 types-aiobotocore-translate-2.5.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    11497 2023-08-08 01:22:10.000000 types-aiobotocore-translate-2.5.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-08 01:24:34.118799 types-aiobotocore-translate-2.5.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2080 2023-08-08 01:22:10.000000 types-aiobotocore-translate-2.5.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:24:34.110799 types-aiobotocore-translate-2.5.4/types_aiobotocore_translate/
+-rw-r--r--   0 runner    (1001) docker     (123)      681 2023-08-08 01:22:10.000000 types-aiobotocore-translate-2.5.4/types_aiobotocore_translate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      680 2023-08-08 01:22:10.000000 types-aiobotocore-translate-2.5.4/types_aiobotocore_translate/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      939 2023-08-08 01:22:10.000000 types-aiobotocore-translate-2.5.4/types_aiobotocore_translate/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18162 2023-08-08 01:22:10.000000 types-aiobotocore-translate-2.5.4/types_aiobotocore_translate/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18133 2023-08-08 01:22:10.000000 types-aiobotocore-translate-2.5.4/types_aiobotocore_translate/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9061 2023-08-08 01:22:10.000000 types-aiobotocore-translate-2.5.4/types_aiobotocore_translate/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9059 2023-08-08 01:22:10.000000 types-aiobotocore-translate-2.5.4/types_aiobotocore_translate/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2041 2023-08-08 01:22:10.000000 types-aiobotocore-translate-2.5.4/types_aiobotocore_translate/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2038 2023-08-08 01:22:10.000000 types-aiobotocore-translate-2.5.4/types_aiobotocore_translate/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 01:22:10.000000 types-aiobotocore-translate-2.5.4/types_aiobotocore_translate/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    20212 2023-08-08 01:22:11.000000 types-aiobotocore-translate-2.5.4/types_aiobotocore_translate/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20193 2023-08-08 01:22:11.000000 types-aiobotocore-translate-2.5.4/types_aiobotocore_translate/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-08-08 01:22:10.000000 types-aiobotocore-translate-2.5.4/types_aiobotocore_translate/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:24:34.110799 types-aiobotocore-translate-2.5.4/types_aiobotocore_translate.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    13017 2023-08-08 01:24:33.000000 types-aiobotocore-translate-2.5.4/types_aiobotocore_translate.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      851 2023-08-08 01:24:33.000000 types-aiobotocore-translate-2.5.4/types_aiobotocore_translate.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 01:24:33.000000 types-aiobotocore-translate-2.5.4/types_aiobotocore_translate.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 01:24:33.000000 types-aiobotocore-translate-2.5.4/types_aiobotocore_translate.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-08 01:24:33.000000 types-aiobotocore-translate-2.5.4/types_aiobotocore_translate.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-08-08 01:24:33.000000 types-aiobotocore-translate-2.5.4/types_aiobotocore_translate.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-translate-2.5.2.post2/LICENSE` & `types-aiobotocore-translate-2.5.4/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-translate-2.5.2.post2/PKG-INFO` & `types-aiobotocore-translate-2.5.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-translate
-Version: 2.5.2.post2
-Summary: Type annotations for aiobotocore.Translate 2.5.2 service generated with mypy-boto3-builder 7.17.2
+Version: 2.5.4
+Summary: Type annotations for aiobotocore.Translate 2.5.4 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_translate/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-translate.svg?color=blue)](https://pypi.org/project/types-aiobotocore-translate)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_translate/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-translate)](https://pepy.tech/project/types-aiobotocore-translate)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.Translate 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/translate.html#Translate)
+[aiobotocore.Translate 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/translate.html#Translate)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-translate-2.5.2.post2/README.md` & `types-aiobotocore-translate-2.5.4/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-translate.svg?color=blue)](https://pypi.org/project/types-aiobotocore-translate)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_translate/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-translate)](https://pepy.tech/project/types-aiobotocore-translate)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.Translate 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/translate.html#Translate)
+[aiobotocore.Translate 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/translate.html#Translate)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-translate-2.5.2.post2/setup.py` & `types-aiobotocore-translate-2.5.4/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-translate",
-    version="2.5.2.post2",
+    version="2.5.4",
     packages=["types_aiobotocore_translate"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.Translate 2.5.2 service generated with mypy-boto3-builder"
+        "Type annotations for aiobotocore.Translate 2.5.4 service generated with mypy-boto3-builder"
         " 7.17.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
```

### Comparing `types-aiobotocore-translate-2.5.2.post2/types_aiobotocore_translate/__init__.py` & `types-aiobotocore-translate-2.5.4/types_aiobotocore_translate/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-translate-2.5.2.post2/types_aiobotocore_translate/__init__.pyi` & `types-aiobotocore-translate-2.5.4/types_aiobotocore_translate/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-translate-2.5.2.post2/types_aiobotocore_translate/__main__.py` & `types-aiobotocore-translate-2.5.4/types_aiobotocore_translate/__main__.py`

 * *Files 10% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.Translate 2.5.2\nVersion:         2.5.2.post2\nBuilder"
-        " version: 7.17.2\nDocs:           "
+        "Type annotations for aiobotocore.Translate 2.5.4\nVersion:         2.5.4\nBuilder version:"
+        " 7.17.2\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_translate//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/translate.html#Translate\nOther"
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

### Comparing `types-aiobotocore-translate-2.5.2.post2/types_aiobotocore_translate/client.py` & `types-aiobotocore-translate-2.5.4/types_aiobotocore_translate/client.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-translate-2.5.2.post2/types_aiobotocore_translate/client.pyi` & `types-aiobotocore-translate-2.5.4/types_aiobotocore_translate/client.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-translate-2.5.2.post2/types_aiobotocore_translate/literals.py` & `types-aiobotocore-translate-2.5.4/types_aiobotocore_translate/literals.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-translate-2.5.2.post2/types_aiobotocore_translate/literals.pyi` & `types-aiobotocore-translate-2.5.4/types_aiobotocore_translate/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-translate-2.5.2.post2/types_aiobotocore_translate/paginator.py` & `types-aiobotocore-translate-2.5.4/types_aiobotocore_translate/paginator.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-translate-2.5.2.post2/types_aiobotocore_translate/paginator.pyi` & `types-aiobotocore-translate-2.5.4/types_aiobotocore_translate/paginator.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-translate-2.5.2.post2/types_aiobotocore_translate/type_defs.py` & `types-aiobotocore-translate-2.5.4/types_aiobotocore_translate/type_defs.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-translate-2.5.2.post2/types_aiobotocore_translate/type_defs.pyi` & `types-aiobotocore-translate-2.5.4/types_aiobotocore_translate/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-translate-2.5.2.post2/types_aiobotocore_translate.egg-info/PKG-INFO` & `types-aiobotocore-translate-2.5.4/types_aiobotocore_translate.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-translate
-Version: 2.5.2.post2
-Summary: Type annotations for aiobotocore.Translate 2.5.2 service generated with mypy-boto3-builder 7.17.2
+Version: 2.5.4
+Summary: Type annotations for aiobotocore.Translate 2.5.4 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_translate/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-translate.svg?color=blue)](https://pypi.org/project/types-aiobotocore-translate)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_translate/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-translate)](https://pepy.tech/project/types-aiobotocore-translate)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.Translate 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/translate.html#Translate)
+[aiobotocore.Translate 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/translate.html#Translate)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-translate-2.5.2.post2/types_aiobotocore_translate.egg-info/SOURCES.txt` & `types-aiobotocore-translate-2.5.4/types_aiobotocore_translate.egg-info/SOURCES.txt`

 * *Files identical despite different names*


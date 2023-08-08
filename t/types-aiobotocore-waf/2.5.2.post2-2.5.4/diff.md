# Comparing `tmp/types-aiobotocore-waf-2.5.2.post2.tar.gz` & `tmp/types-aiobotocore-waf-2.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-waf-2.5.2.post2.tar", last modified: Fri Aug  4 13:59:29 2023, max compression
+gzip compressed data, was "types-aiobotocore-waf-2.5.4.tar", last modified: Tue Aug  8 01:24:34 2023, max compression
```

## Comparing `types-aiobotocore-waf-2.5.2.post2.tar` & `types-aiobotocore-waf-2.5.4.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:29.566643 types-aiobotocore-waf-2.5.2.post2/
--rw-r--r--   0 vlad      (1000) vlad      (1000)     1070 2023-08-04 13:55:35.000000 types-aiobotocore-waf-2.5.2.post2/LICENSE
--rw-r--r--   0 vlad      (1000) vlad      (1000)    15098 2023-08-04 13:59:29.566643 types-aiobotocore-waf-2.5.2.post2/PKG-INFO
--rw-r--r--   0 vlad      (1000) vlad      (1000)    13596 2023-08-04 13:55:35.000000 types-aiobotocore-waf-2.5.2.post2/README.md
--rw-r--r--   0 vlad      (1000) vlad      (1000)       38 2023-08-04 13:59:29.576643 types-aiobotocore-waf-2.5.2.post2/setup.cfg
--rw-r--r--   0 vlad      (1000) vlad      (1000)     2020 2023-08-04 13:55:35.000000 types-aiobotocore-waf-2.5.2.post2/setup.py
-drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:29.566643 types-aiobotocore-waf-2.5.2.post2/types_aiobotocore_waf/
--rw-r--r--   0 vlad      (1000) vlad      (1000)     4013 2023-08-04 13:55:35.000000 types-aiobotocore-waf-2.5.2.post2/types_aiobotocore_waf/__init__.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)     4012 2023-08-04 13:55:35.000000 types-aiobotocore-waf-2.5.2.post2/types_aiobotocore_waf/__init__.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)      916 2023-08-04 13:55:35.000000 types-aiobotocore-waf-2.5.2.post2/types_aiobotocore_waf/__main__.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)    52660 2023-08-04 13:55:36.000000 types-aiobotocore-waf-2.5.2.post2/types_aiobotocore_waf/client.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)    52558 2023-08-04 13:55:35.000000 types-aiobotocore-waf-2.5.2.post2/types_aiobotocore_waf/client.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)    13774 2023-08-04 13:55:36.000000 types-aiobotocore-waf-2.5.2.post2/types_aiobotocore_waf/literals.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)    13772 2023-08-04 13:55:36.000000 types-aiobotocore-waf-2.5.2.post2/types_aiobotocore_waf/literals.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)    18479 2023-08-04 13:55:36.000000 types-aiobotocore-waf-2.5.2.post2/types_aiobotocore_waf/paginator.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)    18461 2023-08-04 13:55:36.000000 types-aiobotocore-waf-2.5.2.post2/types_aiobotocore_waf/paginator.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:55:35.000000 types-aiobotocore-waf-2.5.2.post2/types_aiobotocore_waf/py.typed
--rw-r--r--   0 vlad      (1000) vlad      (1000)    59140 2023-08-04 13:55:38.000000 types-aiobotocore-waf-2.5.2.post2/types_aiobotocore_waf/type_defs.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)    59093 2023-08-04 13:55:37.000000 types-aiobotocore-waf-2.5.2.post2/types_aiobotocore_waf/type_defs.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)       65 2023-08-04 13:55:35.000000 types-aiobotocore-waf-2.5.2.post2/types_aiobotocore_waf/version.py
-drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:29.566643 types-aiobotocore-waf-2.5.2.post2/types_aiobotocore_waf.egg-info/
--rw-r--r--   0 vlad      (1000) vlad      (1000)    15098 2023-08-04 13:59:29.000000 types-aiobotocore-waf-2.5.2.post2/types_aiobotocore_waf.egg-info/PKG-INFO
--rw-r--r--   0 vlad      (1000) vlad      (1000)      737 2023-08-04 13:59:29.000000 types-aiobotocore-waf-2.5.2.post2/types_aiobotocore_waf.egg-info/SOURCES.txt
--rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:29.000000 types-aiobotocore-waf-2.5.2.post2/types_aiobotocore_waf.egg-info/dependency_links.txt
--rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:29.000000 types-aiobotocore-waf-2.5.2.post2/types_aiobotocore_waf.egg-info/not-zip-safe
--rw-r--r--   0 vlad      (1000) vlad      (1000)       52 2023-08-04 13:59:29.000000 types-aiobotocore-waf-2.5.2.post2/types_aiobotocore_waf.egg-info/requires.txt
--rw-r--r--   0 vlad      (1000) vlad      (1000)       22 2023-08-04 13:59:29.000000 types-aiobotocore-waf-2.5.2.post2/types_aiobotocore_waf.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:24:34.726801 types-aiobotocore-waf-2.5.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-08 01:22:19.000000 types-aiobotocore-waf-2.5.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    15092 2023-08-08 01:24:34.726801 types-aiobotocore-waf-2.5.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    13596 2023-08-08 01:22:19.000000 types-aiobotocore-waf-2.5.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-08 01:24:34.726801 types-aiobotocore-waf-2.5.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2014 2023-08-08 01:22:19.000000 types-aiobotocore-waf-2.5.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:24:34.726801 types-aiobotocore-waf-2.5.4/types_aiobotocore_waf/
+-rw-r--r--   0 runner    (1001) docker     (123)     4013 2023-08-08 01:22:19.000000 types-aiobotocore-waf-2.5.4/types_aiobotocore_waf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4012 2023-08-08 01:22:19.000000 types-aiobotocore-waf-2.5.4/types_aiobotocore_waf/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      904 2023-08-08 01:22:19.000000 types-aiobotocore-waf-2.5.4/types_aiobotocore_waf/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    52660 2023-08-08 01:22:20.000000 types-aiobotocore-waf-2.5.4/types_aiobotocore_waf/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    52558 2023-08-08 01:22:20.000000 types-aiobotocore-waf-2.5.4/types_aiobotocore_waf/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    13774 2023-08-08 01:22:20.000000 types-aiobotocore-waf-2.5.4/types_aiobotocore_waf/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13772 2023-08-08 01:22:20.000000 types-aiobotocore-waf-2.5.4/types_aiobotocore_waf/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    18479 2023-08-08 01:22:20.000000 types-aiobotocore-waf-2.5.4/types_aiobotocore_waf/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18461 2023-08-08 01:22:20.000000 types-aiobotocore-waf-2.5.4/types_aiobotocore_waf/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 01:22:19.000000 types-aiobotocore-waf-2.5.4/types_aiobotocore_waf/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    59140 2023-08-08 01:22:21.000000 types-aiobotocore-waf-2.5.4/types_aiobotocore_waf/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    59093 2023-08-08 01:22:21.000000 types-aiobotocore-waf-2.5.4/types_aiobotocore_waf/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-08-08 01:22:19.000000 types-aiobotocore-waf-2.5.4/types_aiobotocore_waf/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:24:34.726801 types-aiobotocore-waf-2.5.4/types_aiobotocore_waf.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    15092 2023-08-08 01:24:34.000000 types-aiobotocore-waf-2.5.4/types_aiobotocore_waf.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      737 2023-08-08 01:24:34.000000 types-aiobotocore-waf-2.5.4/types_aiobotocore_waf.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 01:24:34.000000 types-aiobotocore-waf-2.5.4/types_aiobotocore_waf.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 01:24:34.000000 types-aiobotocore-waf-2.5.4/types_aiobotocore_waf.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-08 01:24:34.000000 types-aiobotocore-waf-2.5.4/types_aiobotocore_waf.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-08-08 01:24:34.000000 types-aiobotocore-waf-2.5.4/types_aiobotocore_waf.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-waf-2.5.2.post2/LICENSE` & `types-aiobotocore-waf-2.5.4/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-waf-2.5.2.post2/PKG-INFO` & `types-aiobotocore-waf-2.5.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-waf
-Version: 2.5.2.post2
-Summary: Type annotations for aiobotocore.WAF 2.5.2 service generated with mypy-boto3-builder 7.17.2
+Version: 2.5.4
+Summary: Type annotations for aiobotocore.WAF 2.5.4 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_waf/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-waf.svg?color=blue)](https://pypi.org/project/types-aiobotocore-waf)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_waf/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-waf)](https://pepy.tech/project/types-aiobotocore-waf)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.WAF 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/waf.html#WAF)
+[aiobotocore.WAF 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/waf.html#WAF)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-waf-2.5.2.post2/README.md` & `types-aiobotocore-waf-2.5.4/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-waf.svg?color=blue)](https://pypi.org/project/types-aiobotocore-waf)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_waf/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-waf)](https://pepy.tech/project/types-aiobotocore-waf)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.WAF 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/waf.html#WAF)
+[aiobotocore.WAF 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/waf.html#WAF)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-waf-2.5.2.post2/setup.py` & `types-aiobotocore-waf-2.5.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-waf",
-    version="2.5.2.post2",
+    version="2.5.4",
     packages=["types_aiobotocore_waf"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.WAF 2.5.2 service generated with mypy-boto3-builder"
+        "Type annotations for aiobotocore.WAF 2.5.4 service generated with mypy-boto3-builder"
         " 7.17.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
```

### Comparing `types-aiobotocore-waf-2.5.2.post2/types_aiobotocore_waf/__init__.py` & `types-aiobotocore-waf-2.5.4/types_aiobotocore_waf/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-waf-2.5.2.post2/types_aiobotocore_waf/__init__.pyi` & `types-aiobotocore-waf-2.5.4/types_aiobotocore_waf/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-waf-2.5.2.post2/types_aiobotocore_waf/__main__.py` & `types-aiobotocore-waf-2.5.4/types_aiobotocore_waf/__main__.py`

 * *Files 9% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.WAF 2.5.2\nVersion:         2.5.2.post2\nBuilder version:"
+        "Type annotations for aiobotocore.WAF 2.5.4\nVersion:         2.5.4\nBuilder version:"
         " 7.17.2\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_waf//\nBoto3 docs:    "
         "  https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/waf.html#WAF\nOther"
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

### Comparing `types-aiobotocore-waf-2.5.2.post2/types_aiobotocore_waf/client.py` & `types-aiobotocore-waf-2.5.4/types_aiobotocore_waf/client.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-waf-2.5.2.post2/types_aiobotocore_waf/client.pyi` & `types-aiobotocore-waf-2.5.4/types_aiobotocore_waf/client.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-waf-2.5.2.post2/types_aiobotocore_waf/literals.py` & `types-aiobotocore-waf-2.5.4/types_aiobotocore_waf/literals.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-waf-2.5.2.post2/types_aiobotocore_waf/literals.pyi` & `types-aiobotocore-waf-2.5.4/types_aiobotocore_waf/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-waf-2.5.2.post2/types_aiobotocore_waf/paginator.py` & `types-aiobotocore-waf-2.5.4/types_aiobotocore_waf/paginator.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-waf-2.5.2.post2/types_aiobotocore_waf/paginator.pyi` & `types-aiobotocore-waf-2.5.4/types_aiobotocore_waf/paginator.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-waf-2.5.2.post2/types_aiobotocore_waf/type_defs.py` & `types-aiobotocore-waf-2.5.4/types_aiobotocore_waf/type_defs.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-waf-2.5.2.post2/types_aiobotocore_waf/type_defs.pyi` & `types-aiobotocore-waf-2.5.4/types_aiobotocore_waf/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-waf-2.5.2.post2/types_aiobotocore_waf.egg-info/PKG-INFO` & `types-aiobotocore-waf-2.5.4/types_aiobotocore_waf.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-waf
-Version: 2.5.2.post2
-Summary: Type annotations for aiobotocore.WAF 2.5.2 service generated with mypy-boto3-builder 7.17.2
+Version: 2.5.4
+Summary: Type annotations for aiobotocore.WAF 2.5.4 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_waf/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-waf.svg?color=blue)](https://pypi.org/project/types-aiobotocore-waf)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_waf/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-waf)](https://pepy.tech/project/types-aiobotocore-waf)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.WAF 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/waf.html#WAF)
+[aiobotocore.WAF 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/waf.html#WAF)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-waf-2.5.2.post2/types_aiobotocore_waf.egg-info/SOURCES.txt` & `types-aiobotocore-waf-2.5.4/types_aiobotocore_waf.egg-info/SOURCES.txt`

 * *Files identical despite different names*


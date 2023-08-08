# Comparing `tmp/types-aiobotocore-sso-2.5.2.post2.tar.gz` & `tmp/types-aiobotocore-sso-2.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-sso-2.5.2.post2.tar", last modified: Fri Aug  4 13:59:27 2023, max compression
+gzip compressed data, was "types-aiobotocore-sso-2.5.4.tar", last modified: Tue Aug  8 01:24:30 2023, max compression
```

## Comparing `types-aiobotocore-sso-2.5.2.post2.tar` & `types-aiobotocore-sso-2.5.4.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:27.876643 types-aiobotocore-sso-2.5.2.post2/
--rw-r--r--   0 vlad      (1000) vlad      (1000)     1070 2023-08-04 13:54:30.000000 types-aiobotocore-sso-2.5.2.post2/LICENSE
--rw-r--r--   0 vlad      (1000) vlad      (1000)    12815 2023-08-04 13:59:27.876643 types-aiobotocore-sso-2.5.2.post2/PKG-INFO
--rw-r--r--   0 vlad      (1000) vlad      (1000)    11313 2023-08-04 13:54:30.000000 types-aiobotocore-sso-2.5.2.post2/README.md
--rw-r--r--   0 vlad      (1000) vlad      (1000)       38 2023-08-04 13:59:27.876643 types-aiobotocore-sso-2.5.2.post2/setup.cfg
--rw-r--r--   0 vlad      (1000) vlad      (1000)     2020 2023-08-04 13:54:29.000000 types-aiobotocore-sso-2.5.2.post2/setup.py
-drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:27.876643 types-aiobotocore-sso-2.5.2.post2/types_aiobotocore_sso/
--rw-r--r--   0 vlad      (1000) vlad      (1000)      799 2023-08-04 13:54:30.000000 types-aiobotocore-sso-2.5.2.post2/types_aiobotocore_sso/__init__.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)      798 2023-08-04 13:54:30.000000 types-aiobotocore-sso-2.5.2.post2/types_aiobotocore_sso/__init__.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)      916 2023-08-04 13:54:30.000000 types-aiobotocore-sso-2.5.2.post2/types_aiobotocore_sso/__main__.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)     7370 2023-08-04 13:54:30.000000 types-aiobotocore-sso-2.5.2.post2/types_aiobotocore_sso/client.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)     7355 2023-08-04 13:54:30.000000 types-aiobotocore-sso-2.5.2.post2/types_aiobotocore_sso/client.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)     8350 2023-08-04 13:54:30.000000 types-aiobotocore-sso-2.5.2.post2/types_aiobotocore_sso/literals.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)     8348 2023-08-04 13:54:30.000000 types-aiobotocore-sso-2.5.2.post2/types_aiobotocore_sso/literals.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)     3023 2023-08-04 13:54:30.000000 types-aiobotocore-sso-2.5.2.post2/types_aiobotocore_sso/paginator.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)     3019 2023-08-04 13:54:30.000000 types-aiobotocore-sso-2.5.2.post2/types_aiobotocore_sso/paginator.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:54:30.000000 types-aiobotocore-sso-2.5.2.post2/types_aiobotocore_sso/py.typed
--rw-r--r--   0 vlad      (1000) vlad      (1000)     5373 2023-08-04 13:54:30.000000 types-aiobotocore-sso-2.5.2.post2/types_aiobotocore_sso/type_defs.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)     5364 2023-08-04 13:54:30.000000 types-aiobotocore-sso-2.5.2.post2/types_aiobotocore_sso/type_defs.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)       65 2023-08-04 13:54:30.000000 types-aiobotocore-sso-2.5.2.post2/types_aiobotocore_sso/version.py
-drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:27.876643 types-aiobotocore-sso-2.5.2.post2/types_aiobotocore_sso.egg-info/
--rw-r--r--   0 vlad      (1000) vlad      (1000)    12815 2023-08-04 13:59:27.000000 types-aiobotocore-sso-2.5.2.post2/types_aiobotocore_sso.egg-info/PKG-INFO
--rw-r--r--   0 vlad      (1000) vlad      (1000)      737 2023-08-04 13:59:27.000000 types-aiobotocore-sso-2.5.2.post2/types_aiobotocore_sso.egg-info/SOURCES.txt
--rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:27.000000 types-aiobotocore-sso-2.5.2.post2/types_aiobotocore_sso.egg-info/dependency_links.txt
--rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:27.000000 types-aiobotocore-sso-2.5.2.post2/types_aiobotocore_sso.egg-info/not-zip-safe
--rw-r--r--   0 vlad      (1000) vlad      (1000)       52 2023-08-04 13:59:27.000000 types-aiobotocore-sso-2.5.2.post2/types_aiobotocore_sso.egg-info/requires.txt
--rw-r--r--   0 vlad      (1000) vlad      (1000)       22 2023-08-04 13:59:27.000000 types-aiobotocore-sso-2.5.2.post2/types_aiobotocore_sso.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:24:30.826792 types-aiobotocore-sso-2.5.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-08 01:21:41.000000 types-aiobotocore-sso-2.5.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    12809 2023-08-08 01:24:30.826792 types-aiobotocore-sso-2.5.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    11313 2023-08-08 01:21:41.000000 types-aiobotocore-sso-2.5.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-08 01:24:30.826792 types-aiobotocore-sso-2.5.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2014 2023-08-08 01:21:41.000000 types-aiobotocore-sso-2.5.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:24:30.826792 types-aiobotocore-sso-2.5.4/types_aiobotocore_sso/
+-rw-r--r--   0 runner    (1001) docker     (123)      799 2023-08-08 01:21:41.000000 types-aiobotocore-sso-2.5.4/types_aiobotocore_sso/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      798 2023-08-08 01:21:41.000000 types-aiobotocore-sso-2.5.4/types_aiobotocore_sso/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      904 2023-08-08 01:21:41.000000 types-aiobotocore-sso-2.5.4/types_aiobotocore_sso/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7370 2023-08-08 01:21:41.000000 types-aiobotocore-sso-2.5.4/types_aiobotocore_sso/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7355 2023-08-08 01:21:41.000000 types-aiobotocore-sso-2.5.4/types_aiobotocore_sso/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8350 2023-08-08 01:21:41.000000 types-aiobotocore-sso-2.5.4/types_aiobotocore_sso/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8348 2023-08-08 01:21:41.000000 types-aiobotocore-sso-2.5.4/types_aiobotocore_sso/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     3023 2023-08-08 01:21:41.000000 types-aiobotocore-sso-2.5.4/types_aiobotocore_sso/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3019 2023-08-08 01:21:41.000000 types-aiobotocore-sso-2.5.4/types_aiobotocore_sso/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 01:21:41.000000 types-aiobotocore-sso-2.5.4/types_aiobotocore_sso/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     5373 2023-08-08 01:21:42.000000 types-aiobotocore-sso-2.5.4/types_aiobotocore_sso/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5364 2023-08-08 01:21:41.000000 types-aiobotocore-sso-2.5.4/types_aiobotocore_sso/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-08-08 01:21:41.000000 types-aiobotocore-sso-2.5.4/types_aiobotocore_sso/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:24:30.826792 types-aiobotocore-sso-2.5.4/types_aiobotocore_sso.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    12809 2023-08-08 01:24:30.000000 types-aiobotocore-sso-2.5.4/types_aiobotocore_sso.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      737 2023-08-08 01:24:30.000000 types-aiobotocore-sso-2.5.4/types_aiobotocore_sso.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 01:24:30.000000 types-aiobotocore-sso-2.5.4/types_aiobotocore_sso.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 01:24:30.000000 types-aiobotocore-sso-2.5.4/types_aiobotocore_sso.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-08 01:24:30.000000 types-aiobotocore-sso-2.5.4/types_aiobotocore_sso.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-08-08 01:24:30.000000 types-aiobotocore-sso-2.5.4/types_aiobotocore_sso.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-sso-2.5.2.post2/LICENSE` & `types-aiobotocore-sso-2.5.4/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-sso-2.5.2.post2/PKG-INFO` & `types-aiobotocore-sso-2.5.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-sso
-Version: 2.5.2.post2
-Summary: Type annotations for aiobotocore.SSO 2.5.2 service generated with mypy-boto3-builder 7.17.2
+Version: 2.5.4
+Summary: Type annotations for aiobotocore.SSO 2.5.4 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sso/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-sso.svg?color=blue)](https://pypi.org/project/types-aiobotocore-sso)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sso/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-sso)](https://pepy.tech/project/types-aiobotocore-sso)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.SSO 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sso.html#SSO)
+[aiobotocore.SSO 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sso.html#SSO)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-sso-2.5.2.post2/README.md` & `types-aiobotocore-sso-2.5.4/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-sso.svg?color=blue)](https://pypi.org/project/types-aiobotocore-sso)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sso/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-sso)](https://pepy.tech/project/types-aiobotocore-sso)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.SSO 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sso.html#SSO)
+[aiobotocore.SSO 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sso.html#SSO)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-sso-2.5.2.post2/setup.py` & `types-aiobotocore-sso-2.5.4/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-sso",
-    version="2.5.2.post2",
+    version="2.5.4",
     packages=["types_aiobotocore_sso"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.SSO 2.5.2 service generated with mypy-boto3-builder"
+        "Type annotations for aiobotocore.SSO 2.5.4 service generated with mypy-boto3-builder"
         " 7.17.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
```

### Comparing `types-aiobotocore-sso-2.5.2.post2/types_aiobotocore_sso/__init__.py` & `types-aiobotocore-sso-2.5.4/types_aiobotocore_sso/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-sso-2.5.2.post2/types_aiobotocore_sso/__init__.pyi` & `types-aiobotocore-sso-2.5.4/types_aiobotocore_sso/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-sso-2.5.2.post2/types_aiobotocore_sso/__main__.py` & `types-aiobotocore-sso-2.5.4/types_aiobotocore_sso/__main__.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.SSO 2.5.2\nVersion:         2.5.2.post2\nBuilder version:"
+        "Type annotations for aiobotocore.SSO 2.5.4\nVersion:         2.5.4\nBuilder version:"
         " 7.17.2\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sso//\nBoto3 docs:    "
         "  https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sso.html#SSO\nOther"
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

### Comparing `types-aiobotocore-sso-2.5.2.post2/types_aiobotocore_sso/client.py` & `types-aiobotocore-sso-2.5.4/types_aiobotocore_sso/client.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-sso-2.5.2.post2/types_aiobotocore_sso/client.pyi` & `types-aiobotocore-sso-2.5.4/types_aiobotocore_sso/client.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-sso-2.5.2.post2/types_aiobotocore_sso/literals.py` & `types-aiobotocore-sso-2.5.4/types_aiobotocore_sso/literals.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-sso-2.5.2.post2/types_aiobotocore_sso/literals.pyi` & `types-aiobotocore-sso-2.5.4/types_aiobotocore_sso/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-sso-2.5.2.post2/types_aiobotocore_sso/paginator.py` & `types-aiobotocore-sso-2.5.4/types_aiobotocore_sso/paginator.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-sso-2.5.2.post2/types_aiobotocore_sso/paginator.pyi` & `types-aiobotocore-sso-2.5.4/types_aiobotocore_sso/paginator.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-sso-2.5.2.post2/types_aiobotocore_sso/type_defs.py` & `types-aiobotocore-sso-2.5.4/types_aiobotocore_sso/type_defs.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-sso-2.5.2.post2/types_aiobotocore_sso/type_defs.pyi` & `types-aiobotocore-sso-2.5.4/types_aiobotocore_sso/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-sso-2.5.2.post2/types_aiobotocore_sso.egg-info/PKG-INFO` & `types-aiobotocore-sso-2.5.4/types_aiobotocore_sso.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-sso
-Version: 2.5.2.post2
-Summary: Type annotations for aiobotocore.SSO 2.5.2 service generated with mypy-boto3-builder 7.17.2
+Version: 2.5.4
+Summary: Type annotations for aiobotocore.SSO 2.5.4 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sso/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-sso.svg?color=blue)](https://pypi.org/project/types-aiobotocore-sso)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sso/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-sso)](https://pepy.tech/project/types-aiobotocore-sso)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.SSO 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sso.html#SSO)
+[aiobotocore.SSO 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sso.html#SSO)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-sso-2.5.2.post2/types_aiobotocore_sso.egg-info/SOURCES.txt` & `types-aiobotocore-sso-2.5.4/types_aiobotocore_sso.egg-info/SOURCES.txt`

 * *Files identical despite different names*


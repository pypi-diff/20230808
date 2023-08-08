# Comparing `tmp/types-aiobotocore-wafv2-2.5.2.post2.tar.gz` & `tmp/types-aiobotocore-wafv2-2.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-wafv2-2.5.2.post2.tar", last modified: Fri Aug  4 13:59:29 2023, max compression
+gzip compressed data, was "types-aiobotocore-wafv2-2.5.4.tar", last modified: Tue Aug  8 01:24:35 2023, max compression
```

## Comparing `types-aiobotocore-wafv2-2.5.2.post2.tar` & `types-aiobotocore-wafv2-2.5.4.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:29.616643 types-aiobotocore-wafv2-2.5.2.post2/
--rw-r--r--   0 vlad      (1000) vlad      (1000)     1070 2023-08-04 13:55:51.000000 types-aiobotocore-wafv2-2.5.2.post2/LICENSE
--rw-r--r--   0 vlad      (1000) vlad      (1000)    12072 2023-08-04 13:59:29.616643 types-aiobotocore-wafv2-2.5.2.post2/PKG-INFO
--rw-r--r--   0 vlad      (1000) vlad      (1000)    10562 2023-08-04 13:55:51.000000 types-aiobotocore-wafv2-2.5.2.post2/README.md
--rw-r--r--   0 vlad      (1000) vlad      (1000)       38 2023-08-04 13:59:29.616643 types-aiobotocore-wafv2-2.5.2.post2/setup.cfg
--rw-r--r--   0 vlad      (1000) vlad      (1000)     2058 2023-08-04 13:55:51.000000 types-aiobotocore-wafv2-2.5.2.post2/setup.py
-drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:29.616643 types-aiobotocore-wafv2-2.5.2.post2/types_aiobotocore_wafv2/
--rw-r--r--   0 vlad      (1000) vlad      (1000)      426 2023-08-04 13:55:51.000000 types-aiobotocore-wafv2-2.5.2.post2/types_aiobotocore_wafv2/__init__.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)      425 2023-08-04 13:55:51.000000 types-aiobotocore-wafv2-2.5.2.post2/types_aiobotocore_wafv2/__init__.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)      924 2023-08-04 13:55:51.000000 types-aiobotocore-wafv2-2.5.2.post2/types_aiobotocore_wafv2/__main__.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)    39160 2023-08-04 13:55:51.000000 types-aiobotocore-wafv2-2.5.2.post2/types_aiobotocore_wafv2/client.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)    39099 2023-08-04 13:55:51.000000 types-aiobotocore-wafv2-2.5.2.post2/types_aiobotocore_wafv2/client.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)    13571 2023-08-04 13:55:51.000000 types-aiobotocore-wafv2-2.5.2.post2/types_aiobotocore_wafv2/literals.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)    13569 2023-08-04 13:55:51.000000 types-aiobotocore-wafv2-2.5.2.post2/types_aiobotocore_wafv2/literals.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:55:51.000000 types-aiobotocore-wafv2-2.5.2.post2/types_aiobotocore_wafv2/py.typed
--rw-r--r--   0 vlad      (1000) vlad      (1000)    68634 2023-08-04 13:55:57.000000 types-aiobotocore-wafv2-2.5.2.post2/types_aiobotocore_wafv2/type_defs.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)    68553 2023-08-04 13:55:56.000000 types-aiobotocore-wafv2-2.5.2.post2/types_aiobotocore_wafv2/type_defs.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)       65 2023-08-04 13:55:51.000000 types-aiobotocore-wafv2-2.5.2.post2/types_aiobotocore_wafv2/version.py
-drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:29.616643 types-aiobotocore-wafv2-2.5.2.post2/types_aiobotocore_wafv2.egg-info/
--rw-r--r--   0 vlad      (1000) vlad      (1000)    12072 2023-08-04 13:59:29.000000 types-aiobotocore-wafv2-2.5.2.post2/types_aiobotocore_wafv2.egg-info/PKG-INFO
--rw-r--r--   0 vlad      (1000) vlad      (1000)      700 2023-08-04 13:59:29.000000 types-aiobotocore-wafv2-2.5.2.post2/types_aiobotocore_wafv2.egg-info/SOURCES.txt
--rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:29.000000 types-aiobotocore-wafv2-2.5.2.post2/types_aiobotocore_wafv2.egg-info/dependency_links.txt
--rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:29.000000 types-aiobotocore-wafv2-2.5.2.post2/types_aiobotocore_wafv2.egg-info/not-zip-safe
--rw-r--r--   0 vlad      (1000) vlad      (1000)       52 2023-08-04 13:59:29.000000 types-aiobotocore-wafv2-2.5.2.post2/types_aiobotocore_wafv2.egg-info/requires.txt
--rw-r--r--   0 vlad      (1000) vlad      (1000)       24 2023-08-04 13:59:29.000000 types-aiobotocore-wafv2-2.5.2.post2/types_aiobotocore_wafv2.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:24:35.262802 types-aiobotocore-wafv2-2.5.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-08 01:22:30.000000 types-aiobotocore-wafv2-2.5.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    12066 2023-08-08 01:24:35.262802 types-aiobotocore-wafv2-2.5.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10562 2023-08-08 01:22:30.000000 types-aiobotocore-wafv2-2.5.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-08 01:24:35.262802 types-aiobotocore-wafv2-2.5.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2052 2023-08-08 01:22:30.000000 types-aiobotocore-wafv2-2.5.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:24:35.258802 types-aiobotocore-wafv2-2.5.4/types_aiobotocore_wafv2/
+-rw-r--r--   0 runner    (1001) docker     (123)      426 2023-08-08 01:22:30.000000 types-aiobotocore-wafv2-2.5.4/types_aiobotocore_wafv2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      425 2023-08-08 01:22:30.000000 types-aiobotocore-wafv2-2.5.4/types_aiobotocore_wafv2/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      912 2023-08-08 01:22:30.000000 types-aiobotocore-wafv2-2.5.4/types_aiobotocore_wafv2/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39160 2023-08-08 01:22:30.000000 types-aiobotocore-wafv2-2.5.4/types_aiobotocore_wafv2/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39099 2023-08-08 01:22:30.000000 types-aiobotocore-wafv2-2.5.4/types_aiobotocore_wafv2/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    13571 2023-08-08 01:22:31.000000 types-aiobotocore-wafv2-2.5.4/types_aiobotocore_wafv2/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13569 2023-08-08 01:22:31.000000 types-aiobotocore-wafv2-2.5.4/types_aiobotocore_wafv2/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 01:22:30.000000 types-aiobotocore-wafv2-2.5.4/types_aiobotocore_wafv2/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    68634 2023-08-08 01:22:32.000000 types-aiobotocore-wafv2-2.5.4/types_aiobotocore_wafv2/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    68553 2023-08-08 01:22:31.000000 types-aiobotocore-wafv2-2.5.4/types_aiobotocore_wafv2/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-08-08 01:22:30.000000 types-aiobotocore-wafv2-2.5.4/types_aiobotocore_wafv2/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:24:35.262802 types-aiobotocore-wafv2-2.5.4/types_aiobotocore_wafv2.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    12066 2023-08-08 01:24:35.000000 types-aiobotocore-wafv2-2.5.4/types_aiobotocore_wafv2.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      700 2023-08-08 01:24:35.000000 types-aiobotocore-wafv2-2.5.4/types_aiobotocore_wafv2.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 01:24:35.000000 types-aiobotocore-wafv2-2.5.4/types_aiobotocore_wafv2.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 01:24:35.000000 types-aiobotocore-wafv2-2.5.4/types_aiobotocore_wafv2.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-08 01:24:35.000000 types-aiobotocore-wafv2-2.5.4/types_aiobotocore_wafv2.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-08-08 01:24:35.000000 types-aiobotocore-wafv2-2.5.4/types_aiobotocore_wafv2.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-wafv2-2.5.2.post2/LICENSE` & `types-aiobotocore-wafv2-2.5.4/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-wafv2-2.5.2.post2/PKG-INFO` & `types-aiobotocore-wafv2-2.5.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-wafv2
-Version: 2.5.2.post2
-Summary: Type annotations for aiobotocore.WAFV2 2.5.2 service generated with mypy-boto3-builder 7.17.2
+Version: 2.5.4
+Summary: Type annotations for aiobotocore.WAFV2 2.5.4 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_wafv2/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-wafv2.svg?color=blue)](https://pypi.org/project/types-aiobotocore-wafv2)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_wafv2/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-wafv2)](https://pepy.tech/project/types-aiobotocore-wafv2)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.WAFV2 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wafv2.html#WAFV2)
+[aiobotocore.WAFV2 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wafv2.html#WAFV2)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-wafv2-2.5.2.post2/README.md` & `types-aiobotocore-wafv2-2.5.4/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-wafv2.svg?color=blue)](https://pypi.org/project/types-aiobotocore-wafv2)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_wafv2/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-wafv2)](https://pepy.tech/project/types-aiobotocore-wafv2)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.WAFV2 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wafv2.html#WAFV2)
+[aiobotocore.WAFV2 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wafv2.html#WAFV2)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-wafv2-2.5.2.post2/setup.py` & `types-aiobotocore-wafv2-2.5.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-wafv2",
-    version="2.5.2.post2",
+    version="2.5.4",
     packages=["types_aiobotocore_wafv2"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.WAFV2 2.5.2 service generated with mypy-boto3-builder"
+        "Type annotations for aiobotocore.WAFV2 2.5.4 service generated with mypy-boto3-builder"
         " 7.17.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
```

### Comparing `types-aiobotocore-wafv2-2.5.2.post2/types_aiobotocore_wafv2/__main__.py` & `types-aiobotocore-wafv2-2.5.4/types_aiobotocore_wafv2/__main__.py`

 * *Files 9% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.WAFV2 2.5.2\nVersion:         2.5.2.post2\nBuilder"
-        " version: 7.17.2\nDocs:           "
+        "Type annotations for aiobotocore.WAFV2 2.5.4\nVersion:         2.5.4\nBuilder version:"
+        " 7.17.2\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_wafv2//\nBoto3 docs:  "
         "    https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wafv2.html#WAFV2\nOther"
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

### Comparing `types-aiobotocore-wafv2-2.5.2.post2/types_aiobotocore_wafv2/client.py` & `types-aiobotocore-wafv2-2.5.4/types_aiobotocore_wafv2/client.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-wafv2-2.5.2.post2/types_aiobotocore_wafv2/client.pyi` & `types-aiobotocore-wafv2-2.5.4/types_aiobotocore_wafv2/client.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-wafv2-2.5.2.post2/types_aiobotocore_wafv2/literals.py` & `types-aiobotocore-wafv2-2.5.4/types_aiobotocore_wafv2/literals.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-wafv2-2.5.2.post2/types_aiobotocore_wafv2/literals.pyi` & `types-aiobotocore-wafv2-2.5.4/types_aiobotocore_wafv2/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-wafv2-2.5.2.post2/types_aiobotocore_wafv2/type_defs.py` & `types-aiobotocore-wafv2-2.5.4/types_aiobotocore_wafv2/type_defs.py`

 * *Files 0% similar despite different names*

```diff
@@ -1209,22 +1209,22 @@
     },
     total=False,
 )
 
 NotStatementTypeDef = TypedDict(
     "NotStatementTypeDef",
     {
-        "Statement": Dict[str, Any],
+        "Statement": "StatementTypeDef",
     },
 )
 
 OrStatementTypeDef = TypedDict(
     "OrStatementTypeDef",
     {
-        "Statements": Sequence["StatementTypeDef"],
+        "Statements": Sequence[Dict[str, Any]],
     },
 )
 
 PhoneNumberFieldTypeDef = TypedDict(
     "PhoneNumberFieldTypeDef",
     {
         "Identifier": str,
```

### Comparing `types-aiobotocore-wafv2-2.5.2.post2/types_aiobotocore_wafv2/type_defs.pyi` & `types-aiobotocore-wafv2-2.5.4/types_aiobotocore_wafv2/type_defs.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -1178,22 +1178,22 @@
     },
     total=False,
 )
 
 NotStatementTypeDef = TypedDict(
     "NotStatementTypeDef",
     {
-        "Statement": Dict[str, Any],
+        "Statement": "StatementTypeDef",
     },
 )
 
 OrStatementTypeDef = TypedDict(
     "OrStatementTypeDef",
     {
-        "Statements": Sequence["StatementTypeDef"],
+        "Statements": Sequence[Dict[str, Any]],
     },
 )
 
 PhoneNumberFieldTypeDef = TypedDict(
     "PhoneNumberFieldTypeDef",
     {
         "Identifier": str,
```

### Comparing `types-aiobotocore-wafv2-2.5.2.post2/types_aiobotocore_wafv2.egg-info/PKG-INFO` & `types-aiobotocore-wafv2-2.5.4/types_aiobotocore_wafv2.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-wafv2
-Version: 2.5.2.post2
-Summary: Type annotations for aiobotocore.WAFV2 2.5.2 service generated with mypy-boto3-builder 7.17.2
+Version: 2.5.4
+Summary: Type annotations for aiobotocore.WAFV2 2.5.4 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_wafv2/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-wafv2.svg?color=blue)](https://pypi.org/project/types-aiobotocore-wafv2)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_wafv2/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-wafv2)](https://pepy.tech/project/types-aiobotocore-wafv2)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.WAFV2 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wafv2.html#WAFV2)
+[aiobotocore.WAFV2 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wafv2.html#WAFV2)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-wafv2-2.5.2.post2/types_aiobotocore_wafv2.egg-info/SOURCES.txt` & `types-aiobotocore-wafv2-2.5.4/types_aiobotocore_wafv2.egg-info/SOURCES.txt`

 * *Files identical despite different names*


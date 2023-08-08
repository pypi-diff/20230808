# Comparing `tmp/types-aiobotocore-verifiedpermissions-2.5.2.post2.tar.gz` & `tmp/types-aiobotocore-verifiedpermissions-2.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-verifiedpermissions-2.5.2.post2.tar", last modified: Fri Aug  4 13:59:29 2023, max compression
+gzip compressed data, was "types-aiobotocore-verifiedpermissions-2.5.4.tar", last modified: Tue Aug  8 01:24:34 2023, max compression
```

## Comparing `types-aiobotocore-verifiedpermissions-2.5.2.post2.tar` & `types-aiobotocore-verifiedpermissions-2.5.4.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:29.266643 types-aiobotocore-verifiedpermissions-2.5.2.post2/
--rw-r--r--   0 vlad      (1000) vlad      (1000)     1070 2023-08-04 13:55:23.000000 types-aiobotocore-verifiedpermissions-2.5.2.post2/LICENSE
--rw-r--r--   0 vlad      (1000) vlad      (1000)    14074 2023-08-04 13:59:29.266643 types-aiobotocore-verifiedpermissions-2.5.2.post2/PKG-INFO
--rw-r--r--   0 vlad      (1000) vlad      (1000)    12508 2023-08-04 13:55:23.000000 types-aiobotocore-verifiedpermissions-2.5.2.post2/README.md
--rw-r--r--   0 vlad      (1000) vlad      (1000)       38 2023-08-04 13:59:29.266643 types-aiobotocore-verifiedpermissions-2.5.2.post2/setup.cfg
--rw-r--r--   0 vlad      (1000) vlad      (1000)     2132 2023-08-04 13:55:23.000000 types-aiobotocore-verifiedpermissions-2.5.2.post2/setup.py
-drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:29.266643 types-aiobotocore-verifiedpermissions-2.5.2.post2/types_aiobotocore_verifiedpermissions/
--rw-r--r--   0 vlad      (1000) vlad      (1000)     1403 2023-08-04 13:55:23.000000 types-aiobotocore-verifiedpermissions-2.5.2.post2/types_aiobotocore_verifiedpermissions/__init__.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)     1402 2023-08-04 13:55:23.000000 types-aiobotocore-verifiedpermissions-2.5.2.post2/types_aiobotocore_verifiedpermissions/__init__.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)      991 2023-08-04 13:55:23.000000 types-aiobotocore-verifiedpermissions-2.5.2.post2/types_aiobotocore_verifiedpermissions/__main__.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)    22783 2023-08-04 13:55:23.000000 types-aiobotocore-verifiedpermissions-2.5.2.post2/types_aiobotocore_verifiedpermissions/client.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)    22746 2023-08-04 13:55:23.000000 types-aiobotocore-verifiedpermissions-2.5.2.post2/types_aiobotocore_verifiedpermissions/client.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)     9039 2023-08-04 13:55:23.000000 types-aiobotocore-verifiedpermissions-2.5.2.post2/types_aiobotocore_verifiedpermissions/literals.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)     9037 2023-08-04 13:55:23.000000 types-aiobotocore-verifiedpermissions-2.5.2.post2/types_aiobotocore_verifiedpermissions/literals.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)     5935 2023-08-04 13:55:23.000000 types-aiobotocore-verifiedpermissions-2.5.2.post2/types_aiobotocore_verifiedpermissions/paginator.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)     5929 2023-08-04 13:55:23.000000 types-aiobotocore-verifiedpermissions-2.5.2.post2/types_aiobotocore_verifiedpermissions/paginator.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:55:23.000000 types-aiobotocore-verifiedpermissions-2.5.2.post2/types_aiobotocore_verifiedpermissions/py.typed
--rw-r--r--   0 vlad      (1000) vlad      (1000)    31216 2023-08-04 13:55:24.000000 types-aiobotocore-verifiedpermissions-2.5.2.post2/types_aiobotocore_verifiedpermissions/type_defs.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)    31165 2023-08-04 13:55:23.000000 types-aiobotocore-verifiedpermissions-2.5.2.post2/types_aiobotocore_verifiedpermissions/type_defs.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)       65 2023-08-04 13:55:23.000000 types-aiobotocore-verifiedpermissions-2.5.2.post2/types_aiobotocore_verifiedpermissions/version.py
-drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:29.266643 types-aiobotocore-verifiedpermissions-2.5.2.post2/types_aiobotocore_verifiedpermissions.egg-info/
--rw-r--r--   0 vlad      (1000) vlad      (1000)    14074 2023-08-04 13:59:29.000000 types-aiobotocore-verifiedpermissions-2.5.2.post2/types_aiobotocore_verifiedpermissions.egg-info/PKG-INFO
--rw-r--r--   0 vlad      (1000) vlad      (1000)     1041 2023-08-04 13:59:29.000000 types-aiobotocore-verifiedpermissions-2.5.2.post2/types_aiobotocore_verifiedpermissions.egg-info/SOURCES.txt
--rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:29.000000 types-aiobotocore-verifiedpermissions-2.5.2.post2/types_aiobotocore_verifiedpermissions.egg-info/dependency_links.txt
--rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:29.000000 types-aiobotocore-verifiedpermissions-2.5.2.post2/types_aiobotocore_verifiedpermissions.egg-info/not-zip-safe
--rw-r--r--   0 vlad      (1000) vlad      (1000)       52 2023-08-04 13:59:29.000000 types-aiobotocore-verifiedpermissions-2.5.2.post2/types_aiobotocore_verifiedpermissions.egg-info/requires.txt
--rw-r--r--   0 vlad      (1000) vlad      (1000)       38 2023-08-04 13:59:29.000000 types-aiobotocore-verifiedpermissions-2.5.2.post2/types_aiobotocore_verifiedpermissions.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:24:34.194800 types-aiobotocore-verifiedpermissions-2.5.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-08 01:22:11.000000 types-aiobotocore-verifiedpermissions-2.5.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    14068 2023-08-08 01:24:34.190800 types-aiobotocore-verifiedpermissions-2.5.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    12508 2023-08-08 01:22:11.000000 types-aiobotocore-verifiedpermissions-2.5.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-08 01:24:34.194800 types-aiobotocore-verifiedpermissions-2.5.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2126 2023-08-08 01:22:11.000000 types-aiobotocore-verifiedpermissions-2.5.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:24:34.186799 types-aiobotocore-verifiedpermissions-2.5.4/types_aiobotocore_verifiedpermissions/
+-rw-r--r--   0 runner    (1001) docker     (123)     1403 2023-08-08 01:22:11.000000 types-aiobotocore-verifiedpermissions-2.5.4/types_aiobotocore_verifiedpermissions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1402 2023-08-08 01:22:11.000000 types-aiobotocore-verifiedpermissions-2.5.4/types_aiobotocore_verifiedpermissions/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      979 2023-08-08 01:22:11.000000 types-aiobotocore-verifiedpermissions-2.5.4/types_aiobotocore_verifiedpermissions/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22783 2023-08-08 01:22:11.000000 types-aiobotocore-verifiedpermissions-2.5.4/types_aiobotocore_verifiedpermissions/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22746 2023-08-08 01:22:11.000000 types-aiobotocore-verifiedpermissions-2.5.4/types_aiobotocore_verifiedpermissions/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9039 2023-08-08 01:22:11.000000 types-aiobotocore-verifiedpermissions-2.5.4/types_aiobotocore_verifiedpermissions/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9037 2023-08-08 01:22:11.000000 types-aiobotocore-verifiedpermissions-2.5.4/types_aiobotocore_verifiedpermissions/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     5935 2023-08-08 01:22:11.000000 types-aiobotocore-verifiedpermissions-2.5.4/types_aiobotocore_verifiedpermissions/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5929 2023-08-08 01:22:11.000000 types-aiobotocore-verifiedpermissions-2.5.4/types_aiobotocore_verifiedpermissions/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 01:22:11.000000 types-aiobotocore-verifiedpermissions-2.5.4/types_aiobotocore_verifiedpermissions/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    31216 2023-08-08 01:22:12.000000 types-aiobotocore-verifiedpermissions-2.5.4/types_aiobotocore_verifiedpermissions/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31165 2023-08-08 01:22:12.000000 types-aiobotocore-verifiedpermissions-2.5.4/types_aiobotocore_verifiedpermissions/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-08-08 01:22:11.000000 types-aiobotocore-verifiedpermissions-2.5.4/types_aiobotocore_verifiedpermissions/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:24:34.190800 types-aiobotocore-verifiedpermissions-2.5.4/types_aiobotocore_verifiedpermissions.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    14068 2023-08-08 01:24:34.000000 types-aiobotocore-verifiedpermissions-2.5.4/types_aiobotocore_verifiedpermissions.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1041 2023-08-08 01:24:34.000000 types-aiobotocore-verifiedpermissions-2.5.4/types_aiobotocore_verifiedpermissions.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 01:24:34.000000 types-aiobotocore-verifiedpermissions-2.5.4/types_aiobotocore_verifiedpermissions.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 01:24:34.000000 types-aiobotocore-verifiedpermissions-2.5.4/types_aiobotocore_verifiedpermissions.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-08 01:24:34.000000 types-aiobotocore-verifiedpermissions-2.5.4/types_aiobotocore_verifiedpermissions.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-08 01:24:34.000000 types-aiobotocore-verifiedpermissions-2.5.4/types_aiobotocore_verifiedpermissions.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-verifiedpermissions-2.5.2.post2/LICENSE` & `types-aiobotocore-verifiedpermissions-2.5.4/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-verifiedpermissions-2.5.2.post2/PKG-INFO` & `types-aiobotocore-verifiedpermissions-2.5.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-verifiedpermissions
-Version: 2.5.2.post2
-Summary: Type annotations for aiobotocore.VerifiedPermissions 2.5.2 service generated with mypy-boto3-builder 7.17.2
+Version: 2.5.4
+Summary: Type annotations for aiobotocore.VerifiedPermissions 2.5.4 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_verifiedpermissions/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-verifiedpermissions.svg?color=blue)](https://pypi.org/project/types-aiobotocore-verifiedpermissions)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_verifiedpermissions/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-verifiedpermissions)](https://pepy.tech/project/types-aiobotocore-verifiedpermissions)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.VerifiedPermissions 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/verifiedpermissions.html#VerifiedPermissions)
+[aiobotocore.VerifiedPermissions 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/verifiedpermissions.html#VerifiedPermissions)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-verifiedpermissions-2.5.2.post2/README.md` & `types-aiobotocore-verifiedpermissions-2.5.4/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-verifiedpermissions.svg?color=blue)](https://pypi.org/project/types-aiobotocore-verifiedpermissions)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_verifiedpermissions/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-verifiedpermissions)](https://pepy.tech/project/types-aiobotocore-verifiedpermissions)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.VerifiedPermissions 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/verifiedpermissions.html#VerifiedPermissions)
+[aiobotocore.VerifiedPermissions 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/verifiedpermissions.html#VerifiedPermissions)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-verifiedpermissions-2.5.2.post2/setup.py` & `types-aiobotocore-verifiedpermissions-2.5.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-verifiedpermissions",
-    version="2.5.2.post2",
+    version="2.5.4",
     packages=["types_aiobotocore_verifiedpermissions"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.VerifiedPermissions 2.5.2 service generated with"
+        "Type annotations for aiobotocore.VerifiedPermissions 2.5.4 service generated with"
         " mypy-boto3-builder 7.17.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
```

### Comparing `types-aiobotocore-verifiedpermissions-2.5.2.post2/types_aiobotocore_verifiedpermissions/__init__.py` & `types-aiobotocore-verifiedpermissions-2.5.4/types_aiobotocore_verifiedpermissions/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-verifiedpermissions-2.5.2.post2/types_aiobotocore_verifiedpermissions/__init__.pyi` & `types-aiobotocore-verifiedpermissions-2.5.4/types_aiobotocore_verifiedpermissions/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-verifiedpermissions-2.5.2.post2/types_aiobotocore_verifiedpermissions/__main__.py` & `types-aiobotocore-verifiedpermissions-2.5.4/types_aiobotocore_verifiedpermissions/__main__.py`

 * *Files 10% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.VerifiedPermissions 2.5.2\nVersion:        "
-        " 2.5.2.post2\nBuilder version: 7.17.2\nDocs:           "
+        "Type annotations for aiobotocore.VerifiedPermissions 2.5.4\nVersion:        "
+        " 2.5.4\nBuilder version: 7.17.2\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_verifiedpermissions//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/verifiedpermissions.html#VerifiedPermissions\nOther"
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

### Comparing `types-aiobotocore-verifiedpermissions-2.5.2.post2/types_aiobotocore_verifiedpermissions/client.py` & `types-aiobotocore-verifiedpermissions-2.5.4/types_aiobotocore_verifiedpermissions/client.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-verifiedpermissions-2.5.2.post2/types_aiobotocore_verifiedpermissions/client.pyi` & `types-aiobotocore-verifiedpermissions-2.5.4/types_aiobotocore_verifiedpermissions/client.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-verifiedpermissions-2.5.2.post2/types_aiobotocore_verifiedpermissions/literals.py` & `types-aiobotocore-verifiedpermissions-2.5.4/types_aiobotocore_verifiedpermissions/literals.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-verifiedpermissions-2.5.2.post2/types_aiobotocore_verifiedpermissions/literals.pyi` & `types-aiobotocore-verifiedpermissions-2.5.4/types_aiobotocore_verifiedpermissions/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-verifiedpermissions-2.5.2.post2/types_aiobotocore_verifiedpermissions/paginator.py` & `types-aiobotocore-verifiedpermissions-2.5.4/types_aiobotocore_verifiedpermissions/paginator.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-verifiedpermissions-2.5.2.post2/types_aiobotocore_verifiedpermissions/paginator.pyi` & `types-aiobotocore-verifiedpermissions-2.5.4/types_aiobotocore_verifiedpermissions/paginator.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-verifiedpermissions-2.5.2.post2/types_aiobotocore_verifiedpermissions/type_defs.py` & `types-aiobotocore-verifiedpermissions-2.5.4/types_aiobotocore_verifiedpermissions/type_defs.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-verifiedpermissions-2.5.2.post2/types_aiobotocore_verifiedpermissions/type_defs.pyi` & `types-aiobotocore-verifiedpermissions-2.5.4/types_aiobotocore_verifiedpermissions/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-verifiedpermissions-2.5.2.post2/types_aiobotocore_verifiedpermissions.egg-info/PKG-INFO` & `types-aiobotocore-verifiedpermissions-2.5.4/types_aiobotocore_verifiedpermissions.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-verifiedpermissions
-Version: 2.5.2.post2
-Summary: Type annotations for aiobotocore.VerifiedPermissions 2.5.2 service generated with mypy-boto3-builder 7.17.2
+Version: 2.5.4
+Summary: Type annotations for aiobotocore.VerifiedPermissions 2.5.4 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_verifiedpermissions/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-verifiedpermissions.svg?color=blue)](https://pypi.org/project/types-aiobotocore-verifiedpermissions)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_verifiedpermissions/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-verifiedpermissions)](https://pepy.tech/project/types-aiobotocore-verifiedpermissions)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.VerifiedPermissions 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/verifiedpermissions.html#VerifiedPermissions)
+[aiobotocore.VerifiedPermissions 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/verifiedpermissions.html#VerifiedPermissions)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-verifiedpermissions-2.5.2.post2/types_aiobotocore_verifiedpermissions.egg-info/SOURCES.txt` & `types-aiobotocore-verifiedpermissions-2.5.4/types_aiobotocore_verifiedpermissions.egg-info/SOURCES.txt`

 * *Files identical despite different names*


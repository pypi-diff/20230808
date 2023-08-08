# Comparing `tmp/types-aiobotocore-iotsecuretunneling-2.5.2.post2.tar.gz` & `tmp/types-aiobotocore-iotsecuretunneling-2.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-iotsecuretunneling-2.5.2.post2.tar", last modified: Fri Aug  4 13:59:12 2023, max compression
+gzip compressed data, was "types-aiobotocore-iotsecuretunneling-2.5.4.tar", last modified: Tue Aug  8 01:23:53 2023, max compression
```

## Comparing `types-aiobotocore-iotsecuretunneling-2.5.2.post2.tar` & `types-aiobotocore-iotsecuretunneling-2.5.4.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:58:49.626642 types-aiobotocore-iotsecuretunneling-2.5.2.post2/
--rw-r--r--   0 vlad      (1000) vlad      (1000)     1070 2023-08-04 13:41:09.000000 types-aiobotocore-iotsecuretunneling-2.5.2.post2/LICENSE
--rw-r--r--   0 vlad      (1000) vlad      (1000)    12785 2023-08-04 13:59:12.456642 types-aiobotocore-iotsecuretunneling-2.5.2.post2/PKG-INFO
--rw-r--r--   0 vlad      (1000) vlad      (1000)    11223 2023-08-04 13:41:09.000000 types-aiobotocore-iotsecuretunneling-2.5.2.post2/README.md
--rw-r--r--   0 vlad      (1000) vlad      (1000)       38 2023-08-04 13:59:12.456642 types-aiobotocore-iotsecuretunneling-2.5.2.post2/setup.cfg
--rw-r--r--   0 vlad      (1000) vlad      (1000)     2149 2023-08-04 13:41:09.000000 types-aiobotocore-iotsecuretunneling-2.5.2.post2/setup.py
-drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:58:49.626642 types-aiobotocore-iotsecuretunneling-2.5.2.post2/types_aiobotocore_iotsecuretunneling/
--rw-r--r--   0 vlad      (1000) vlad      (1000)      530 2023-08-04 13:41:09.000000 types-aiobotocore-iotsecuretunneling-2.5.2.post2/types_aiobotocore_iotsecuretunneling/__init__.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)      529 2023-08-04 13:41:09.000000 types-aiobotocore-iotsecuretunneling-2.5.2.post2/types_aiobotocore_iotsecuretunneling/__init__.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)      987 2023-08-04 13:41:09.000000 types-aiobotocore-iotsecuretunneling-2.5.2.post2/types_aiobotocore_iotsecuretunneling/__main__.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)     9213 2023-08-04 13:41:09.000000 types-aiobotocore-iotsecuretunneling-2.5.2.post2/types_aiobotocore_iotsecuretunneling/client.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)     9197 2023-08-04 13:41:09.000000 types-aiobotocore-iotsecuretunneling-2.5.2.post2/types_aiobotocore_iotsecuretunneling/client.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)     8302 2023-08-04 13:41:10.000000 types-aiobotocore-iotsecuretunneling-2.5.2.post2/types_aiobotocore_iotsecuretunneling/literals.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)     8300 2023-08-04 13:41:09.000000 types-aiobotocore-iotsecuretunneling-2.5.2.post2/types_aiobotocore_iotsecuretunneling/literals.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:41:09.000000 types-aiobotocore-iotsecuretunneling-2.5.2.post2/types_aiobotocore_iotsecuretunneling/py.typed
--rw-r--r--   0 vlad      (1000) vlad      (1000)     6508 2023-08-04 13:41:10.000000 types-aiobotocore-iotsecuretunneling-2.5.2.post2/types_aiobotocore_iotsecuretunneling/type_defs.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)     6501 2023-08-04 13:41:10.000000 types-aiobotocore-iotsecuretunneling-2.5.2.post2/types_aiobotocore_iotsecuretunneling/type_defs.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)       65 2023-08-04 13:41:09.000000 types-aiobotocore-iotsecuretunneling-2.5.2.post2/types_aiobotocore_iotsecuretunneling/version.py
-drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:12.456642 types-aiobotocore-iotsecuretunneling-2.5.2.post2/types_aiobotocore_iotsecuretunneling.egg-info/
--rw-r--r--   0 vlad      (1000) vlad      (1000)    12785 2023-08-04 13:59:12.000000 types-aiobotocore-iotsecuretunneling-2.5.2.post2/types_aiobotocore_iotsecuretunneling.egg-info/PKG-INFO
--rw-r--r--   0 vlad      (1000) vlad      (1000)      921 2023-08-04 13:59:12.000000 types-aiobotocore-iotsecuretunneling-2.5.2.post2/types_aiobotocore_iotsecuretunneling.egg-info/SOURCES.txt
--rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:12.000000 types-aiobotocore-iotsecuretunneling-2.5.2.post2/types_aiobotocore_iotsecuretunneling.egg-info/dependency_links.txt
--rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:12.000000 types-aiobotocore-iotsecuretunneling-2.5.2.post2/types_aiobotocore_iotsecuretunneling.egg-info/not-zip-safe
--rw-r--r--   0 vlad      (1000) vlad      (1000)       52 2023-08-04 13:59:12.000000 types-aiobotocore-iotsecuretunneling-2.5.2.post2/types_aiobotocore_iotsecuretunneling.egg-info/requires.txt
--rw-r--r--   0 vlad      (1000) vlad      (1000)       37 2023-08-04 13:59:12.000000 types-aiobotocore-iotsecuretunneling-2.5.2.post2/types_aiobotocore_iotsecuretunneling.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:23:53.246707 types-aiobotocore-iotsecuretunneling-2.5.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-08 01:13:02.000000 types-aiobotocore-iotsecuretunneling-2.5.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    12779 2023-08-08 01:23:53.246707 types-aiobotocore-iotsecuretunneling-2.5.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    11223 2023-08-08 01:13:02.000000 types-aiobotocore-iotsecuretunneling-2.5.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-08 01:23:53.246707 types-aiobotocore-iotsecuretunneling-2.5.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2143 2023-08-08 01:13:02.000000 types-aiobotocore-iotsecuretunneling-2.5.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:23:53.246707 types-aiobotocore-iotsecuretunneling-2.5.4/types_aiobotocore_iotsecuretunneling/
+-rw-r--r--   0 runner    (1001) docker     (123)      530 2023-08-08 01:13:02.000000 types-aiobotocore-iotsecuretunneling-2.5.4/types_aiobotocore_iotsecuretunneling/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      529 2023-08-08 01:13:02.000000 types-aiobotocore-iotsecuretunneling-2.5.4/types_aiobotocore_iotsecuretunneling/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      975 2023-08-08 01:13:02.000000 types-aiobotocore-iotsecuretunneling-2.5.4/types_aiobotocore_iotsecuretunneling/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9213 2023-08-08 01:13:02.000000 types-aiobotocore-iotsecuretunneling-2.5.4/types_aiobotocore_iotsecuretunneling/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9197 2023-08-08 01:13:02.000000 types-aiobotocore-iotsecuretunneling-2.5.4/types_aiobotocore_iotsecuretunneling/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8302 2023-08-08 01:13:03.000000 types-aiobotocore-iotsecuretunneling-2.5.4/types_aiobotocore_iotsecuretunneling/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8300 2023-08-08 01:13:02.000000 types-aiobotocore-iotsecuretunneling-2.5.4/types_aiobotocore_iotsecuretunneling/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 01:13:02.000000 types-aiobotocore-iotsecuretunneling-2.5.4/types_aiobotocore_iotsecuretunneling/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     6508 2023-08-08 01:13:03.000000 types-aiobotocore-iotsecuretunneling-2.5.4/types_aiobotocore_iotsecuretunneling/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6501 2023-08-08 01:13:03.000000 types-aiobotocore-iotsecuretunneling-2.5.4/types_aiobotocore_iotsecuretunneling/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-08-08 01:13:02.000000 types-aiobotocore-iotsecuretunneling-2.5.4/types_aiobotocore_iotsecuretunneling/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:23:53.246707 types-aiobotocore-iotsecuretunneling-2.5.4/types_aiobotocore_iotsecuretunneling.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    12779 2023-08-08 01:23:53.000000 types-aiobotocore-iotsecuretunneling-2.5.4/types_aiobotocore_iotsecuretunneling.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      921 2023-08-08 01:23:53.000000 types-aiobotocore-iotsecuretunneling-2.5.4/types_aiobotocore_iotsecuretunneling.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 01:23:53.000000 types-aiobotocore-iotsecuretunneling-2.5.4/types_aiobotocore_iotsecuretunneling.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 01:23:53.000000 types-aiobotocore-iotsecuretunneling-2.5.4/types_aiobotocore_iotsecuretunneling.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-08 01:23:53.000000 types-aiobotocore-iotsecuretunneling-2.5.4/types_aiobotocore_iotsecuretunneling.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-08-08 01:23:53.000000 types-aiobotocore-iotsecuretunneling-2.5.4/types_aiobotocore_iotsecuretunneling.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-iotsecuretunneling-2.5.2.post2/LICENSE` & `types-aiobotocore-iotsecuretunneling-2.5.4/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-iotsecuretunneling-2.5.2.post2/PKG-INFO` & `types-aiobotocore-iotsecuretunneling-2.5.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-iotsecuretunneling
-Version: 2.5.2.post2
-Summary: Type annotations for aiobotocore.IoTSecureTunneling 2.5.2 service generated with mypy-boto3-builder 7.17.2
+Version: 2.5.4
+Summary: Type annotations for aiobotocore.IoTSecureTunneling 2.5.4 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotsecuretunneling/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-iotsecuretunneling.svg?color=blue)](https://pypi.org/project/types-aiobotocore-iotsecuretunneling)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotsecuretunneling/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-iotsecuretunneling)](https://pepy.tech/project/types-aiobotocore-iotsecuretunneling)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.IoTSecureTunneling 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotsecuretunneling.html#IoTSecureTunneling)
+[aiobotocore.IoTSecureTunneling 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotsecuretunneling.html#IoTSecureTunneling)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-iotsecuretunneling-2.5.2.post2/README.md` & `types-aiobotocore-iotsecuretunneling-2.5.4/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-iotsecuretunneling.svg?color=blue)](https://pypi.org/project/types-aiobotocore-iotsecuretunneling)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotsecuretunneling/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-iotsecuretunneling)](https://pepy.tech/project/types-aiobotocore-iotsecuretunneling)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.IoTSecureTunneling 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotsecuretunneling.html#IoTSecureTunneling)
+[aiobotocore.IoTSecureTunneling 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotsecuretunneling.html#IoTSecureTunneling)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-iotsecuretunneling-2.5.2.post2/setup.py` & `types-aiobotocore-iotsecuretunneling-2.5.4/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-iotsecuretunneling",
-    version="2.5.2.post2",
+    version="2.5.4",
     packages=["types_aiobotocore_iotsecuretunneling"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.IoTSecureTunneling 2.5.2 service generated with"
+        "Type annotations for aiobotocore.IoTSecureTunneling 2.5.4 service generated with"
         " mypy-boto3-builder 7.17.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
```

### Comparing `types-aiobotocore-iotsecuretunneling-2.5.2.post2/types_aiobotocore_iotsecuretunneling/__init__.py` & `types-aiobotocore-iotsecuretunneling-2.5.4/types_aiobotocore_iotsecuretunneling/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-iotsecuretunneling-2.5.2.post2/types_aiobotocore_iotsecuretunneling/__init__.pyi` & `types-aiobotocore-iotsecuretunneling-2.5.4/types_aiobotocore_iotsecuretunneling/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-iotsecuretunneling-2.5.2.post2/types_aiobotocore_iotsecuretunneling/__main__.py` & `types-aiobotocore-iotsecuretunneling-2.5.4/types_aiobotocore_iotsecuretunneling/__main__.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.IoTSecureTunneling 2.5.2\nVersion:        "
-        " 2.5.2.post2\nBuilder version: 7.17.2\nDocs:           "
+        "Type annotations for aiobotocore.IoTSecureTunneling 2.5.4\nVersion:         2.5.4\nBuilder"
+        " version: 7.17.2\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotsecuretunneling//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotsecuretunneling.html#IoTSecureTunneling\nOther"
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

### Comparing `types-aiobotocore-iotsecuretunneling-2.5.2.post2/types_aiobotocore_iotsecuretunneling/client.py` & `types-aiobotocore-iotsecuretunneling-2.5.4/types_aiobotocore_iotsecuretunneling/client.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-iotsecuretunneling-2.5.2.post2/types_aiobotocore_iotsecuretunneling/client.pyi` & `types-aiobotocore-iotsecuretunneling-2.5.4/types_aiobotocore_iotsecuretunneling/client.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-iotsecuretunneling-2.5.2.post2/types_aiobotocore_iotsecuretunneling/literals.py` & `types-aiobotocore-iotsecuretunneling-2.5.4/types_aiobotocore_iotsecuretunneling/literals.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-iotsecuretunneling-2.5.2.post2/types_aiobotocore_iotsecuretunneling/literals.pyi` & `types-aiobotocore-iotsecuretunneling-2.5.4/types_aiobotocore_iotsecuretunneling/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-iotsecuretunneling-2.5.2.post2/types_aiobotocore_iotsecuretunneling/type_defs.py` & `types-aiobotocore-iotsecuretunneling-2.5.4/types_aiobotocore_iotsecuretunneling/type_defs.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-iotsecuretunneling-2.5.2.post2/types_aiobotocore_iotsecuretunneling/type_defs.pyi` & `types-aiobotocore-iotsecuretunneling-2.5.4/types_aiobotocore_iotsecuretunneling/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-iotsecuretunneling-2.5.2.post2/types_aiobotocore_iotsecuretunneling.egg-info/PKG-INFO` & `types-aiobotocore-iotsecuretunneling-2.5.4/types_aiobotocore_iotsecuretunneling.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-iotsecuretunneling
-Version: 2.5.2.post2
-Summary: Type annotations for aiobotocore.IoTSecureTunneling 2.5.2 service generated with mypy-boto3-builder 7.17.2
+Version: 2.5.4
+Summary: Type annotations for aiobotocore.IoTSecureTunneling 2.5.4 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotsecuretunneling/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-iotsecuretunneling.svg?color=blue)](https://pypi.org/project/types-aiobotocore-iotsecuretunneling)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotsecuretunneling/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-iotsecuretunneling)](https://pepy.tech/project/types-aiobotocore-iotsecuretunneling)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.IoTSecureTunneling 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotsecuretunneling.html#IoTSecureTunneling)
+[aiobotocore.IoTSecureTunneling 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotsecuretunneling.html#IoTSecureTunneling)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-iotsecuretunneling-2.5.2.post2/types_aiobotocore_iotsecuretunneling.egg-info/SOURCES.txt` & `types-aiobotocore-iotsecuretunneling-2.5.4/types_aiobotocore_iotsecuretunneling.egg-info/SOURCES.txt`

 * *Files identical despite different names*


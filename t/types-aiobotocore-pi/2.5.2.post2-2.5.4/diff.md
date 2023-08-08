# Comparing `tmp/types-aiobotocore-pi-2.5.2.post2.tar.gz` & `tmp/types-aiobotocore-pi-2.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-pi-2.5.2.post2.tar", last modified: Fri Aug  4 13:59:21 2023, max compression
+gzip compressed data, was "types-aiobotocore-pi-2.5.4.tar", last modified: Tue Aug  8 01:24:13 2023, max compression
```

## Comparing `types-aiobotocore-pi-2.5.2.post2.tar` & `types-aiobotocore-pi-2.5.4.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:21.136643 types-aiobotocore-pi-2.5.2.post2/
--rw-r--r--   0 vlad      (1000) vlad      (1000)     1070 2023-08-04 13:46:38.000000 types-aiobotocore-pi-2.5.2.post2/LICENSE
--rw-r--r--   0 vlad      (1000) vlad      (1000)    11907 2023-08-04 13:59:21.136643 types-aiobotocore-pi-2.5.2.post2/PKG-INFO
--rw-r--r--   0 vlad      (1000) vlad      (1000)    10409 2023-08-04 13:46:38.000000 types-aiobotocore-pi-2.5.2.post2/README.md
--rw-r--r--   0 vlad      (1000) vlad      (1000)       38 2023-08-04 13:59:21.136643 types-aiobotocore-pi-2.5.2.post2/setup.cfg
--rw-r--r--   0 vlad      (1000) vlad      (1000)     2002 2023-08-04 13:46:37.000000 types-aiobotocore-pi-2.5.2.post2/setup.py
-drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:21.136643 types-aiobotocore-pi-2.5.2.post2/types_aiobotocore_pi/
--rw-r--r--   0 vlad      (1000) vlad      (1000)      402 2023-08-04 13:46:38.000000 types-aiobotocore-pi-2.5.2.post2/types_aiobotocore_pi/__init__.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)      401 2023-08-04 13:46:38.000000 types-aiobotocore-pi-2.5.2.post2/types_aiobotocore_pi/__init__.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)      912 2023-08-04 13:46:38.000000 types-aiobotocore-pi-2.5.2.post2/types_aiobotocore_pi/__main__.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)     8755 2023-08-04 13:46:38.000000 types-aiobotocore-pi-2.5.2.post2/types_aiobotocore_pi/client.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)     8741 2023-08-04 13:46:38.000000 types-aiobotocore-pi-2.5.2.post2/types_aiobotocore_pi/client.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)     8581 2023-08-04 13:46:38.000000 types-aiobotocore-pi-2.5.2.post2/types_aiobotocore_pi/literals.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)     8579 2023-08-04 13:46:38.000000 types-aiobotocore-pi-2.5.2.post2/types_aiobotocore_pi/literals.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:46:38.000000 types-aiobotocore-pi-2.5.2.post2/types_aiobotocore_pi/py.typed
--rw-r--r--   0 vlad      (1000) vlad      (1000)    10546 2023-08-04 13:46:38.000000 types-aiobotocore-pi-2.5.2.post2/types_aiobotocore_pi/type_defs.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)    10529 2023-08-04 13:46:38.000000 types-aiobotocore-pi-2.5.2.post2/types_aiobotocore_pi/type_defs.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)       65 2023-08-04 13:46:38.000000 types-aiobotocore-pi-2.5.2.post2/types_aiobotocore_pi/version.py
-drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:21.136643 types-aiobotocore-pi-2.5.2.post2/types_aiobotocore_pi.egg-info/
--rw-r--r--   0 vlad      (1000) vlad      (1000)    11907 2023-08-04 13:59:21.000000 types-aiobotocore-pi-2.5.2.post2/types_aiobotocore_pi.egg-info/PKG-INFO
--rw-r--r--   0 vlad      (1000) vlad      (1000)      649 2023-08-04 13:59:21.000000 types-aiobotocore-pi-2.5.2.post2/types_aiobotocore_pi.egg-info/SOURCES.txt
--rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:21.000000 types-aiobotocore-pi-2.5.2.post2/types_aiobotocore_pi.egg-info/dependency_links.txt
--rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:21.000000 types-aiobotocore-pi-2.5.2.post2/types_aiobotocore_pi.egg-info/not-zip-safe
--rw-r--r--   0 vlad      (1000) vlad      (1000)       52 2023-08-04 13:59:21.000000 types-aiobotocore-pi-2.5.2.post2/types_aiobotocore_pi.egg-info/requires.txt
--rw-r--r--   0 vlad      (1000) vlad      (1000)       21 2023-08-04 13:59:21.000000 types-aiobotocore-pi-2.5.2.post2/types_aiobotocore_pi.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:24:13.458749 types-aiobotocore-pi-2.5.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-08 01:16:32.000000 types-aiobotocore-pi-2.5.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    11901 2023-08-08 01:24:13.458749 types-aiobotocore-pi-2.5.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10409 2023-08-08 01:16:32.000000 types-aiobotocore-pi-2.5.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-08 01:24:13.458749 types-aiobotocore-pi-2.5.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1996 2023-08-08 01:16:32.000000 types-aiobotocore-pi-2.5.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:24:13.458749 types-aiobotocore-pi-2.5.4/types_aiobotocore_pi/
+-rw-r--r--   0 runner    (1001) docker     (123)      402 2023-08-08 01:16:32.000000 types-aiobotocore-pi-2.5.4/types_aiobotocore_pi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      401 2023-08-08 01:16:32.000000 types-aiobotocore-pi-2.5.4/types_aiobotocore_pi/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      900 2023-08-08 01:16:32.000000 types-aiobotocore-pi-2.5.4/types_aiobotocore_pi/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8755 2023-08-08 01:16:32.000000 types-aiobotocore-pi-2.5.4/types_aiobotocore_pi/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8741 2023-08-08 01:16:32.000000 types-aiobotocore-pi-2.5.4/types_aiobotocore_pi/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8581 2023-08-08 01:16:32.000000 types-aiobotocore-pi-2.5.4/types_aiobotocore_pi/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8579 2023-08-08 01:16:32.000000 types-aiobotocore-pi-2.5.4/types_aiobotocore_pi/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 01:16:32.000000 types-aiobotocore-pi-2.5.4/types_aiobotocore_pi/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    10546 2023-08-08 01:16:32.000000 types-aiobotocore-pi-2.5.4/types_aiobotocore_pi/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10529 2023-08-08 01:16:32.000000 types-aiobotocore-pi-2.5.4/types_aiobotocore_pi/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-08-08 01:16:32.000000 types-aiobotocore-pi-2.5.4/types_aiobotocore_pi/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:24:13.458749 types-aiobotocore-pi-2.5.4/types_aiobotocore_pi.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    11901 2023-08-08 01:24:13.000000 types-aiobotocore-pi-2.5.4/types_aiobotocore_pi.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      649 2023-08-08 01:24:13.000000 types-aiobotocore-pi-2.5.4/types_aiobotocore_pi.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 01:24:13.000000 types-aiobotocore-pi-2.5.4/types_aiobotocore_pi.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 01:24:13.000000 types-aiobotocore-pi-2.5.4/types_aiobotocore_pi.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-08 01:24:13.000000 types-aiobotocore-pi-2.5.4/types_aiobotocore_pi.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-08-08 01:24:13.000000 types-aiobotocore-pi-2.5.4/types_aiobotocore_pi.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-pi-2.5.2.post2/LICENSE` & `types-aiobotocore-pi-2.5.4/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-pi-2.5.2.post2/PKG-INFO` & `types-aiobotocore-pi-2.5.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-pi
-Version: 2.5.2.post2
-Summary: Type annotations for aiobotocore.PI 2.5.2 service generated with mypy-boto3-builder 7.17.2
+Version: 2.5.4
+Summary: Type annotations for aiobotocore.PI 2.5.4 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_pi/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-pi.svg?color=blue)](https://pypi.org/project/types-aiobotocore-pi)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_pi/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-pi)](https://pepy.tech/project/types-aiobotocore-pi)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.PI 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pi.html#PI)
+[aiobotocore.PI 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pi.html#PI)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-pi-2.5.2.post2/README.md` & `types-aiobotocore-pi-2.5.4/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-pi.svg?color=blue)](https://pypi.org/project/types-aiobotocore-pi)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_pi/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-pi)](https://pepy.tech/project/types-aiobotocore-pi)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.PI 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pi.html#PI)
+[aiobotocore.PI 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pi.html#PI)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-pi-2.5.2.post2/setup.py` & `types-aiobotocore-pi-2.5.4/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-pi",
-    version="2.5.2.post2",
+    version="2.5.4",
     packages=["types_aiobotocore_pi"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.PI 2.5.2 service generated with mypy-boto3-builder 7.17.2"
+        "Type annotations for aiobotocore.PI 2.5.4 service generated with mypy-boto3-builder 7.17.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

### Comparing `types-aiobotocore-pi-2.5.2.post2/types_aiobotocore_pi/__main__.py` & `types-aiobotocore-pi-2.5.4/types_aiobotocore_pi/__main__.py`

 * *Files 9% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.PI 2.5.2\nVersion:         2.5.2.post2\nBuilder version:"
+        "Type annotations for aiobotocore.PI 2.5.4\nVersion:         2.5.4\nBuilder version:"
         " 7.17.2\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_pi//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pi.html#PI\nOther"
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

### Comparing `types-aiobotocore-pi-2.5.2.post2/types_aiobotocore_pi/client.py` & `types-aiobotocore-pi-2.5.4/types_aiobotocore_pi/client.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-pi-2.5.2.post2/types_aiobotocore_pi/client.pyi` & `types-aiobotocore-pi-2.5.4/types_aiobotocore_pi/client.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-pi-2.5.2.post2/types_aiobotocore_pi/literals.py` & `types-aiobotocore-pi-2.5.4/types_aiobotocore_pi/literals.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-pi-2.5.2.post2/types_aiobotocore_pi/literals.pyi` & `types-aiobotocore-pi-2.5.4/types_aiobotocore_pi/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-pi-2.5.2.post2/types_aiobotocore_pi/type_defs.py` & `types-aiobotocore-pi-2.5.4/types_aiobotocore_pi/type_defs.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-pi-2.5.2.post2/types_aiobotocore_pi/type_defs.pyi` & `types-aiobotocore-pi-2.5.4/types_aiobotocore_pi/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-pi-2.5.2.post2/types_aiobotocore_pi.egg-info/PKG-INFO` & `types-aiobotocore-pi-2.5.4/types_aiobotocore_pi.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-pi
-Version: 2.5.2.post2
-Summary: Type annotations for aiobotocore.PI 2.5.2 service generated with mypy-boto3-builder 7.17.2
+Version: 2.5.4
+Summary: Type annotations for aiobotocore.PI 2.5.4 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_pi/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-pi.svg?color=blue)](https://pypi.org/project/types-aiobotocore-pi)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_pi/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-pi)](https://pepy.tech/project/types-aiobotocore-pi)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.PI 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pi.html#PI)
+[aiobotocore.PI 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pi.html#PI)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-pi-2.5.2.post2/types_aiobotocore_pi.egg-info/SOURCES.txt` & `types-aiobotocore-pi-2.5.4/types_aiobotocore_pi.egg-info/SOURCES.txt`

 * *Files identical despite different names*


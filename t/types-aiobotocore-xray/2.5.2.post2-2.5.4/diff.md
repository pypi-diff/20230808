# Comparing `tmp/types-aiobotocore-xray-2.5.2.post2.tar.gz` & `tmp/types-aiobotocore-xray-2.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-xray-2.5.2.post2.tar", last modified: Fri Aug  4 13:59:30 2023, max compression
+gzip compressed data, was "types-aiobotocore-xray-2.5.4.tar", last modified: Tue Aug  8 01:24:36 2023, max compression
```

## Comparing `types-aiobotocore-xray-2.5.2.post2.tar` & `types-aiobotocore-xray-2.5.4.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:30.476643 types-aiobotocore-xray-2.5.2.post2/
--rw-r--r--   0 vlad      (1000) vlad      (1000)     1070 2023-08-04 13:56:31.000000 types-aiobotocore-xray-2.5.2.post2/LICENSE
--rw-r--r--   0 vlad      (1000) vlad      (1000)    14159 2023-08-04 13:59:30.476643 types-aiobotocore-xray-2.5.2.post2/PKG-INFO
--rw-r--r--   0 vlad      (1000) vlad      (1000)    12653 2023-08-04 13:56:31.000000 types-aiobotocore-xray-2.5.2.post2/README.md
--rw-r--r--   0 vlad      (1000) vlad      (1000)       38 2023-08-04 13:59:30.476643 types-aiobotocore-xray-2.5.2.post2/setup.cfg
--rw-r--r--   0 vlad      (1000) vlad      (1000)     2027 2023-08-04 13:56:30.000000 types-aiobotocore-xray-2.5.2.post2/setup.py
-drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:30.476643 types-aiobotocore-xray-2.5.2.post2/types_aiobotocore_xray/
--rw-r--r--   0 vlad      (1000) vlad      (1000)     2635 2023-08-04 13:56:31.000000 types-aiobotocore-xray-2.5.2.post2/types_aiobotocore_xray/__init__.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)     2634 2023-08-04 13:56:31.000000 types-aiobotocore-xray-2.5.2.post2/types_aiobotocore_xray/__init__.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)      920 2023-08-04 13:56:31.000000 types-aiobotocore-xray-2.5.2.post2/types_aiobotocore_xray/__main__.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)    27722 2023-08-04 13:56:31.000000 types-aiobotocore-xray-2.5.2.post2/types_aiobotocore_xray/client.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)    27673 2023-08-04 13:56:31.000000 types-aiobotocore-xray-2.5.2.post2/types_aiobotocore_xray/client.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)    10047 2023-08-04 13:56:31.000000 types-aiobotocore-xray-2.5.2.post2/types_aiobotocore_xray/literals.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)    10045 2023-08-04 13:56:31.000000 types-aiobotocore-xray-2.5.2.post2/types_aiobotocore_xray/literals.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)    12648 2023-08-04 13:56:31.000000 types-aiobotocore-xray-2.5.2.post2/types_aiobotocore_xray/paginator.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)    12636 2023-08-04 13:56:31.000000 types-aiobotocore-xray-2.5.2.post2/types_aiobotocore_xray/paginator.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:56:31.000000 types-aiobotocore-xray-2.5.2.post2/types_aiobotocore_xray/py.typed
--rw-r--r--   0 vlad      (1000) vlad      (1000)    43285 2023-08-04 13:56:32.000000 types-aiobotocore-xray-2.5.2.post2/types_aiobotocore_xray/type_defs.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)    43236 2023-08-04 13:56:32.000000 types-aiobotocore-xray-2.5.2.post2/types_aiobotocore_xray/type_defs.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)       65 2023-08-04 13:56:31.000000 types-aiobotocore-xray-2.5.2.post2/types_aiobotocore_xray/version.py
-drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:30.476643 types-aiobotocore-xray-2.5.2.post2/types_aiobotocore_xray.egg-info/
--rw-r--r--   0 vlad      (1000) vlad      (1000)    14159 2023-08-04 13:59:30.000000 types-aiobotocore-xray-2.5.2.post2/types_aiobotocore_xray.egg-info/PKG-INFO
--rw-r--r--   0 vlad      (1000) vlad      (1000)      756 2023-08-04 13:59:30.000000 types-aiobotocore-xray-2.5.2.post2/types_aiobotocore_xray.egg-info/SOURCES.txt
--rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:30.000000 types-aiobotocore-xray-2.5.2.post2/types_aiobotocore_xray.egg-info/dependency_links.txt
--rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:30.000000 types-aiobotocore-xray-2.5.2.post2/types_aiobotocore_xray.egg-info/not-zip-safe
--rw-r--r--   0 vlad      (1000) vlad      (1000)       52 2023-08-04 13:59:30.000000 types-aiobotocore-xray-2.5.2.post2/types_aiobotocore_xray.egg-info/requires.txt
--rw-r--r--   0 vlad      (1000) vlad      (1000)       23 2023-08-04 13:59:30.000000 types-aiobotocore-xray-2.5.2.post2/types_aiobotocore_xray.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:24:36.914806 types-aiobotocore-xray-2.5.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-08 01:22:50.000000 types-aiobotocore-xray-2.5.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    14153 2023-08-08 01:24:36.914806 types-aiobotocore-xray-2.5.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    12653 2023-08-08 01:22:50.000000 types-aiobotocore-xray-2.5.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-08 01:24:36.914806 types-aiobotocore-xray-2.5.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2021 2023-08-08 01:22:50.000000 types-aiobotocore-xray-2.5.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:24:36.914806 types-aiobotocore-xray-2.5.4/types_aiobotocore_xray/
+-rw-r--r--   0 runner    (1001) docker     (123)     2635 2023-08-08 01:22:50.000000 types-aiobotocore-xray-2.5.4/types_aiobotocore_xray/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2634 2023-08-08 01:22:50.000000 types-aiobotocore-xray-2.5.4/types_aiobotocore_xray/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      908 2023-08-08 01:22:50.000000 types-aiobotocore-xray-2.5.4/types_aiobotocore_xray/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27722 2023-08-08 01:22:50.000000 types-aiobotocore-xray-2.5.4/types_aiobotocore_xray/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27673 2023-08-08 01:22:50.000000 types-aiobotocore-xray-2.5.4/types_aiobotocore_xray/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    10047 2023-08-08 01:22:50.000000 types-aiobotocore-xray-2.5.4/types_aiobotocore_xray/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10045 2023-08-08 01:22:50.000000 types-aiobotocore-xray-2.5.4/types_aiobotocore_xray/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    12648 2023-08-08 01:22:50.000000 types-aiobotocore-xray-2.5.4/types_aiobotocore_xray/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12636 2023-08-08 01:22:50.000000 types-aiobotocore-xray-2.5.4/types_aiobotocore_xray/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 01:22:50.000000 types-aiobotocore-xray-2.5.4/types_aiobotocore_xray/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    43285 2023-08-08 01:22:54.000000 types-aiobotocore-xray-2.5.4/types_aiobotocore_xray/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    43236 2023-08-08 01:22:51.000000 types-aiobotocore-xray-2.5.4/types_aiobotocore_xray/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-08-08 01:22:50.000000 types-aiobotocore-xray-2.5.4/types_aiobotocore_xray/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:24:36.914806 types-aiobotocore-xray-2.5.4/types_aiobotocore_xray.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    14153 2023-08-08 01:24:36.000000 types-aiobotocore-xray-2.5.4/types_aiobotocore_xray.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      756 2023-08-08 01:24:36.000000 types-aiobotocore-xray-2.5.4/types_aiobotocore_xray.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 01:24:36.000000 types-aiobotocore-xray-2.5.4/types_aiobotocore_xray.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 01:24:36.000000 types-aiobotocore-xray-2.5.4/types_aiobotocore_xray.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-08 01:24:36.000000 types-aiobotocore-xray-2.5.4/types_aiobotocore_xray.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-08-08 01:24:36.000000 types-aiobotocore-xray-2.5.4/types_aiobotocore_xray.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-xray-2.5.2.post2/LICENSE` & `types-aiobotocore-xray-2.5.4/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-xray-2.5.2.post2/PKG-INFO` & `types-aiobotocore-xray-2.5.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-xray
-Version: 2.5.2.post2
-Summary: Type annotations for aiobotocore.XRay 2.5.2 service generated with mypy-boto3-builder 7.17.2
+Version: 2.5.4
+Summary: Type annotations for aiobotocore.XRay 2.5.4 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_xray/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-xray.svg?color=blue)](https://pypi.org/project/types-aiobotocore-xray)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_xray/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-xray)](https://pepy.tech/project/types-aiobotocore-xray)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.XRay 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/xray.html#XRay)
+[aiobotocore.XRay 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/xray.html#XRay)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-xray-2.5.2.post2/README.md` & `types-aiobotocore-xray-2.5.4/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-xray.svg?color=blue)](https://pypi.org/project/types-aiobotocore-xray)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_xray/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-xray)](https://pepy.tech/project/types-aiobotocore-xray)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.XRay 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/xray.html#XRay)
+[aiobotocore.XRay 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/xray.html#XRay)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-xray-2.5.2.post2/setup.py` & `types-aiobotocore-xray-2.5.4/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-xray",
-    version="2.5.2.post2",
+    version="2.5.4",
     packages=["types_aiobotocore_xray"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.XRay 2.5.2 service generated with mypy-boto3-builder"
+        "Type annotations for aiobotocore.XRay 2.5.4 service generated with mypy-boto3-builder"
         " 7.17.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
```

### Comparing `types-aiobotocore-xray-2.5.2.post2/types_aiobotocore_xray/__init__.py` & `types-aiobotocore-xray-2.5.4/types_aiobotocore_xray/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-xray-2.5.2.post2/types_aiobotocore_xray/__init__.pyi` & `types-aiobotocore-xray-2.5.4/types_aiobotocore_xray/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-xray-2.5.2.post2/types_aiobotocore_xray/__main__.py` & `types-aiobotocore-xray-2.5.4/types_aiobotocore_xray/__main__.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.XRay 2.5.2\nVersion:         2.5.2.post2\nBuilder"
-        " version: 7.17.2\nDocs:           "
+        "Type annotations for aiobotocore.XRay 2.5.4\nVersion:         2.5.4\nBuilder version:"
+        " 7.17.2\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_xray//\nBoto3 docs:   "
         "   https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/xray.html#XRay\nOther"
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

### Comparing `types-aiobotocore-xray-2.5.2.post2/types_aiobotocore_xray/client.py` & `types-aiobotocore-xray-2.5.4/types_aiobotocore_xray/client.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-xray-2.5.2.post2/types_aiobotocore_xray/client.pyi` & `types-aiobotocore-xray-2.5.4/types_aiobotocore_xray/client.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-xray-2.5.2.post2/types_aiobotocore_xray/literals.py` & `types-aiobotocore-xray-2.5.4/types_aiobotocore_xray/literals.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-xray-2.5.2.post2/types_aiobotocore_xray/literals.pyi` & `types-aiobotocore-xray-2.5.4/types_aiobotocore_xray/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-xray-2.5.2.post2/types_aiobotocore_xray/paginator.py` & `types-aiobotocore-xray-2.5.4/types_aiobotocore_xray/paginator.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-xray-2.5.2.post2/types_aiobotocore_xray/paginator.pyi` & `types-aiobotocore-xray-2.5.4/types_aiobotocore_xray/paginator.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-xray-2.5.2.post2/types_aiobotocore_xray/type_defs.py` & `types-aiobotocore-xray-2.5.4/types_aiobotocore_xray/type_defs.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-xray-2.5.2.post2/types_aiobotocore_xray/type_defs.pyi` & `types-aiobotocore-xray-2.5.4/types_aiobotocore_xray/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-xray-2.5.2.post2/types_aiobotocore_xray.egg-info/PKG-INFO` & `types-aiobotocore-xray-2.5.4/types_aiobotocore_xray.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-xray
-Version: 2.5.2.post2
-Summary: Type annotations for aiobotocore.XRay 2.5.2 service generated with mypy-boto3-builder 7.17.2
+Version: 2.5.4
+Summary: Type annotations for aiobotocore.XRay 2.5.4 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_xray/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-xray.svg?color=blue)](https://pypi.org/project/types-aiobotocore-xray)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_xray/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-xray)](https://pepy.tech/project/types-aiobotocore-xray)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.XRay 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/xray.html#XRay)
+[aiobotocore.XRay 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/xray.html#XRay)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-xray-2.5.2.post2/types_aiobotocore_xray.egg-info/SOURCES.txt` & `types-aiobotocore-xray-2.5.4/types_aiobotocore_xray.egg-info/SOURCES.txt`

 * *Files identical despite different names*


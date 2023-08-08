# Comparing `tmp/types-aiobotocore-mgn-2.5.2.post2.tar.gz` & `tmp/types-aiobotocore-mgn-2.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-mgn-2.5.2.post2.tar", last modified: Fri Aug  4 13:59:18 2023, max compression
+gzip compressed data, was "types-aiobotocore-mgn-2.5.4.tar", last modified: Tue Aug  8 01:24:07 2023, max compression
```

## Comparing `types-aiobotocore-mgn-2.5.2.post2.tar` & `types-aiobotocore-mgn-2.5.4.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:18.526643 types-aiobotocore-mgn-2.5.2.post2/
--rw-r--r--   0 vlad      (1000) vlad      (1000)     1070 2023-08-04 13:44:58.000000 types-aiobotocore-mgn-2.5.2.post2/LICENSE
--rw-r--r--   0 vlad      (1000) vlad      (1000)    14966 2023-08-04 13:59:18.526643 types-aiobotocore-mgn-2.5.2.post2/PKG-INFO
--rw-r--r--   0 vlad      (1000) vlad      (1000)    13464 2023-08-04 13:44:58.000000 types-aiobotocore-mgn-2.5.2.post2/README.md
--rw-r--r--   0 vlad      (1000) vlad      (1000)       38 2023-08-04 13:59:18.526643 types-aiobotocore-mgn-2.5.2.post2/setup.cfg
--rw-r--r--   0 vlad      (1000) vlad      (1000)     2020 2023-08-04 13:44:58.000000 types-aiobotocore-mgn-2.5.2.post2/setup.py
-drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:18.526643 types-aiobotocore-mgn-2.5.2.post2/types_aiobotocore_mgn/
--rw-r--r--   0 vlad      (1000) vlad      (1000)     3813 2023-08-04 13:44:58.000000 types-aiobotocore-mgn-2.5.2.post2/types_aiobotocore_mgn/__init__.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)     3812 2023-08-04 13:44:58.000000 types-aiobotocore-mgn-2.5.2.post2/types_aiobotocore_mgn/__init__.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)      916 2023-08-04 13:44:58.000000 types-aiobotocore-mgn-2.5.2.post2/types_aiobotocore_mgn/__main__.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)    54555 2023-08-04 13:44:58.000000 types-aiobotocore-mgn-2.5.2.post2/types_aiobotocore_mgn/client.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)    54466 2023-08-04 13:44:58.000000 types-aiobotocore-mgn-2.5.2.post2/types_aiobotocore_mgn/client.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)    15622 2023-08-04 13:44:59.000000 types-aiobotocore-mgn-2.5.2.post2/types_aiobotocore_mgn/literals.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)    15620 2023-08-04 13:44:59.000000 types-aiobotocore-mgn-2.5.2.post2/types_aiobotocore_mgn/literals.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)    18818 2023-08-04 13:44:59.000000 types-aiobotocore-mgn-2.5.2.post2/types_aiobotocore_mgn/paginator.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)    18801 2023-08-04 13:44:59.000000 types-aiobotocore-mgn-2.5.2.post2/types_aiobotocore_mgn/paginator.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:44:58.000000 types-aiobotocore-mgn-2.5.2.post2/types_aiobotocore_mgn/py.typed
--rw-r--r--   0 vlad      (1000) vlad      (1000)    79861 2023-08-04 13:45:02.000000 types-aiobotocore-mgn-2.5.2.post2/types_aiobotocore_mgn/type_defs.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)    79746 2023-08-04 13:45:01.000000 types-aiobotocore-mgn-2.5.2.post2/types_aiobotocore_mgn/type_defs.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)       65 2023-08-04 13:44:58.000000 types-aiobotocore-mgn-2.5.2.post2/types_aiobotocore_mgn/version.py
-drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:18.526643 types-aiobotocore-mgn-2.5.2.post2/types_aiobotocore_mgn.egg-info/
--rw-r--r--   0 vlad      (1000) vlad      (1000)    14966 2023-08-04 13:59:18.000000 types-aiobotocore-mgn-2.5.2.post2/types_aiobotocore_mgn.egg-info/PKG-INFO
--rw-r--r--   0 vlad      (1000) vlad      (1000)      737 2023-08-04 13:59:18.000000 types-aiobotocore-mgn-2.5.2.post2/types_aiobotocore_mgn.egg-info/SOURCES.txt
--rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:18.000000 types-aiobotocore-mgn-2.5.2.post2/types_aiobotocore_mgn.egg-info/dependency_links.txt
--rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:18.000000 types-aiobotocore-mgn-2.5.2.post2/types_aiobotocore_mgn.egg-info/not-zip-safe
--rw-r--r--   0 vlad      (1000) vlad      (1000)       52 2023-08-04 13:59:18.000000 types-aiobotocore-mgn-2.5.2.post2/types_aiobotocore_mgn.egg-info/requires.txt
--rw-r--r--   0 vlad      (1000) vlad      (1000)       22 2023-08-04 13:59:18.000000 types-aiobotocore-mgn-2.5.2.post2/types_aiobotocore_mgn.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:24:07.082736 types-aiobotocore-mgn-2.5.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-08 01:15:29.000000 types-aiobotocore-mgn-2.5.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    14960 2023-08-08 01:24:07.082736 types-aiobotocore-mgn-2.5.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    13464 2023-08-08 01:15:29.000000 types-aiobotocore-mgn-2.5.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-08 01:24:07.082736 types-aiobotocore-mgn-2.5.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2014 2023-08-08 01:15:29.000000 types-aiobotocore-mgn-2.5.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:24:07.082736 types-aiobotocore-mgn-2.5.4/types_aiobotocore_mgn/
+-rw-r--r--   0 runner    (1001) docker     (123)     3813 2023-08-08 01:15:29.000000 types-aiobotocore-mgn-2.5.4/types_aiobotocore_mgn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3812 2023-08-08 01:15:29.000000 types-aiobotocore-mgn-2.5.4/types_aiobotocore_mgn/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      904 2023-08-08 01:15:29.000000 types-aiobotocore-mgn-2.5.4/types_aiobotocore_mgn/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    54555 2023-08-08 01:15:30.000000 types-aiobotocore-mgn-2.5.4/types_aiobotocore_mgn/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    54466 2023-08-08 01:15:30.000000 types-aiobotocore-mgn-2.5.4/types_aiobotocore_mgn/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    15622 2023-08-08 01:15:30.000000 types-aiobotocore-mgn-2.5.4/types_aiobotocore_mgn/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15620 2023-08-08 01:15:30.000000 types-aiobotocore-mgn-2.5.4/types_aiobotocore_mgn/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    18818 2023-08-08 01:15:30.000000 types-aiobotocore-mgn-2.5.4/types_aiobotocore_mgn/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18801 2023-08-08 01:15:30.000000 types-aiobotocore-mgn-2.5.4/types_aiobotocore_mgn/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 01:15:29.000000 types-aiobotocore-mgn-2.5.4/types_aiobotocore_mgn/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    79861 2023-08-08 01:15:33.000000 types-aiobotocore-mgn-2.5.4/types_aiobotocore_mgn/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    79746 2023-08-08 01:15:31.000000 types-aiobotocore-mgn-2.5.4/types_aiobotocore_mgn/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-08-08 01:15:29.000000 types-aiobotocore-mgn-2.5.4/types_aiobotocore_mgn/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:24:07.082736 types-aiobotocore-mgn-2.5.4/types_aiobotocore_mgn.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    14960 2023-08-08 01:24:06.000000 types-aiobotocore-mgn-2.5.4/types_aiobotocore_mgn.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      737 2023-08-08 01:24:06.000000 types-aiobotocore-mgn-2.5.4/types_aiobotocore_mgn.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 01:24:06.000000 types-aiobotocore-mgn-2.5.4/types_aiobotocore_mgn.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 01:24:06.000000 types-aiobotocore-mgn-2.5.4/types_aiobotocore_mgn.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-08 01:24:06.000000 types-aiobotocore-mgn-2.5.4/types_aiobotocore_mgn.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-08-08 01:24:06.000000 types-aiobotocore-mgn-2.5.4/types_aiobotocore_mgn.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-mgn-2.5.2.post2/LICENSE` & `types-aiobotocore-mgn-2.5.4/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-mgn-2.5.2.post2/PKG-INFO` & `types-aiobotocore-mgn-2.5.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-mgn
-Version: 2.5.2.post2
-Summary: Type annotations for aiobotocore.mgn 2.5.2 service generated with mypy-boto3-builder 7.17.2
+Version: 2.5.4
+Summary: Type annotations for aiobotocore.mgn 2.5.4 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mgn/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-mgn.svg?color=blue)](https://pypi.org/project/types-aiobotocore-mgn)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mgn/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-mgn)](https://pepy.tech/project/types-aiobotocore-mgn)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.mgn 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn)
+[aiobotocore.mgn 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-mgn-2.5.2.post2/README.md` & `types-aiobotocore-mgn-2.5.4/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-mgn.svg?color=blue)](https://pypi.org/project/types-aiobotocore-mgn)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mgn/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-mgn)](https://pepy.tech/project/types-aiobotocore-mgn)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.mgn 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn)
+[aiobotocore.mgn 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-mgn-2.5.2.post2/setup.py` & `types-aiobotocore-mgn-2.5.4/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-mgn",
-    version="2.5.2.post2",
+    version="2.5.4",
     packages=["types_aiobotocore_mgn"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.mgn 2.5.2 service generated with mypy-boto3-builder"
+        "Type annotations for aiobotocore.mgn 2.5.4 service generated with mypy-boto3-builder"
         " 7.17.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
```

### Comparing `types-aiobotocore-mgn-2.5.2.post2/types_aiobotocore_mgn/__init__.py` & `types-aiobotocore-mgn-2.5.4/types_aiobotocore_mgn/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-mgn-2.5.2.post2/types_aiobotocore_mgn/__init__.pyi` & `types-aiobotocore-mgn-2.5.4/types_aiobotocore_mgn/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-mgn-2.5.2.post2/types_aiobotocore_mgn/__main__.py` & `types-aiobotocore-mgn-2.5.4/types_aiobotocore_mgn/__main__.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.mgn 2.5.2\nVersion:         2.5.2.post2\nBuilder version:"
+        "Type annotations for aiobotocore.mgn 2.5.4\nVersion:         2.5.4\nBuilder version:"
         " 7.17.2\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mgn//\nBoto3 docs:    "
         "  https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn\nOther"
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

### Comparing `types-aiobotocore-mgn-2.5.2.post2/types_aiobotocore_mgn/client.py` & `types-aiobotocore-mgn-2.5.4/types_aiobotocore_mgn/client.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-mgn-2.5.2.post2/types_aiobotocore_mgn/client.pyi` & `types-aiobotocore-mgn-2.5.4/types_aiobotocore_mgn/client.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-mgn-2.5.2.post2/types_aiobotocore_mgn/literals.py` & `types-aiobotocore-mgn-2.5.4/types_aiobotocore_mgn/literals.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-mgn-2.5.2.post2/types_aiobotocore_mgn/literals.pyi` & `types-aiobotocore-mgn-2.5.4/types_aiobotocore_mgn/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-mgn-2.5.2.post2/types_aiobotocore_mgn/paginator.py` & `types-aiobotocore-mgn-2.5.4/types_aiobotocore_mgn/paginator.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-mgn-2.5.2.post2/types_aiobotocore_mgn/paginator.pyi` & `types-aiobotocore-mgn-2.5.4/types_aiobotocore_mgn/paginator.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-mgn-2.5.2.post2/types_aiobotocore_mgn/type_defs.py` & `types-aiobotocore-mgn-2.5.4/types_aiobotocore_mgn/type_defs.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-mgn-2.5.2.post2/types_aiobotocore_mgn/type_defs.pyi` & `types-aiobotocore-mgn-2.5.4/types_aiobotocore_mgn/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-mgn-2.5.2.post2/types_aiobotocore_mgn.egg-info/PKG-INFO` & `types-aiobotocore-mgn-2.5.4/types_aiobotocore_mgn.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-mgn
-Version: 2.5.2.post2
-Summary: Type annotations for aiobotocore.mgn 2.5.2 service generated with mypy-boto3-builder 7.17.2
+Version: 2.5.4
+Summary: Type annotations for aiobotocore.mgn 2.5.4 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mgn/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-mgn.svg?color=blue)](https://pypi.org/project/types-aiobotocore-mgn)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mgn/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-mgn)](https://pepy.tech/project/types-aiobotocore-mgn)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.mgn 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn)
+[aiobotocore.mgn 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-mgn-2.5.2.post2/types_aiobotocore_mgn.egg-info/SOURCES.txt` & `types-aiobotocore-mgn-2.5.4/types_aiobotocore_mgn.egg-info/SOURCES.txt`

 * *Files identical despite different names*


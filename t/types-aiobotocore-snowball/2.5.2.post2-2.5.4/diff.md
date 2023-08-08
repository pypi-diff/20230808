# Comparing `tmp/types-aiobotocore-snowball-2.5.2.post2.tar.gz` & `tmp/types-aiobotocore-snowball-2.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-snowball-2.5.2.post2.tar", last modified: Fri Aug  4 13:59:27 2023, max compression
+gzip compressed data, was "types-aiobotocore-snowball-2.5.4.tar", last modified: Tue Aug  8 01:24:28 2023, max compression
```

## Comparing `types-aiobotocore-snowball-2.5.2.post2.tar` & `types-aiobotocore-snowball-2.5.4.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:27.356643 types-aiobotocore-snowball-2.5.2.post2/
--rw-r--r--   0 vlad      (1000) vlad      (1000)     1070 2023-08-04 13:53:52.000000 types-aiobotocore-snowball-2.5.2.post2/LICENSE
--rw-r--r--   0 vlad      (1000) vlad      (1000)    13669 2023-08-04 13:59:27.356643 types-aiobotocore-snowball-2.5.2.post2/PKG-INFO
--rw-r--r--   0 vlad      (1000) vlad      (1000)    12147 2023-08-04 13:53:52.000000 types-aiobotocore-snowball-2.5.2.post2/README.md
--rw-r--r--   0 vlad      (1000) vlad      (1000)       38 2023-08-04 13:59:27.356643 types-aiobotocore-snowball-2.5.2.post2/setup.cfg
--rw-r--r--   0 vlad      (1000) vlad      (1000)     2079 2023-08-04 13:53:52.000000 types-aiobotocore-snowball-2.5.2.post2/setup.py
-drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:27.356643 types-aiobotocore-snowball-2.5.2.post2/types_aiobotocore_snowball/
--rw-r--r--   0 vlad      (1000) vlad      (1000)     1679 2023-08-04 13:53:52.000000 types-aiobotocore-snowball-2.5.2.post2/types_aiobotocore_snowball/__init__.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)     1678 2023-08-04 13:53:52.000000 types-aiobotocore-snowball-2.5.2.post2/types_aiobotocore_snowball/__init__.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)      947 2023-08-04 13:53:52.000000 types-aiobotocore-snowball-2.5.2.post2/types_aiobotocore_snowball/__main__.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)    26027 2023-08-04 13:53:53.000000 types-aiobotocore-snowball-2.5.2.post2/types_aiobotocore_snowball/client.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)    25985 2023-08-04 13:53:53.000000 types-aiobotocore-snowball-2.5.2.post2/types_aiobotocore_snowball/client.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)    10698 2023-08-04 13:53:53.000000 types-aiobotocore-snowball-2.5.2.post2/types_aiobotocore_snowball/literals.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)    10696 2023-08-04 13:53:53.000000 types-aiobotocore-snowball-2.5.2.post2/types_aiobotocore_snowball/literals.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)     7415 2023-08-04 13:53:53.000000 types-aiobotocore-snowball-2.5.2.post2/types_aiobotocore_snowball/paginator.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)     7407 2023-08-04 13:53:53.000000 types-aiobotocore-snowball-2.5.2.post2/types_aiobotocore_snowball/paginator.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:53:52.000000 types-aiobotocore-snowball-2.5.2.post2/types_aiobotocore_snowball/py.typed
--rw-r--r--   0 vlad      (1000) vlad      (1000)    28869 2023-08-04 13:53:54.000000 types-aiobotocore-snowball-2.5.2.post2/types_aiobotocore_snowball/type_defs.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)    28848 2023-08-04 13:53:53.000000 types-aiobotocore-snowball-2.5.2.post2/types_aiobotocore_snowball/type_defs.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)       65 2023-08-04 13:53:52.000000 types-aiobotocore-snowball-2.5.2.post2/types_aiobotocore_snowball/version.py
-drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:27.356643 types-aiobotocore-snowball-2.5.2.post2/types_aiobotocore_snowball.egg-info/
--rw-r--r--   0 vlad      (1000) vlad      (1000)    13669 2023-08-04 13:59:27.000000 types-aiobotocore-snowball-2.5.2.post2/types_aiobotocore_snowball.egg-info/PKG-INFO
--rw-r--r--   0 vlad      (1000) vlad      (1000)      832 2023-08-04 13:59:27.000000 types-aiobotocore-snowball-2.5.2.post2/types_aiobotocore_snowball.egg-info/SOURCES.txt
--rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:27.000000 types-aiobotocore-snowball-2.5.2.post2/types_aiobotocore_snowball.egg-info/dependency_links.txt
--rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:27.000000 types-aiobotocore-snowball-2.5.2.post2/types_aiobotocore_snowball.egg-info/not-zip-safe
--rw-r--r--   0 vlad      (1000) vlad      (1000)       52 2023-08-04 13:59:27.000000 types-aiobotocore-snowball-2.5.2.post2/types_aiobotocore_snowball.egg-info/requires.txt
--rw-r--r--   0 vlad      (1000) vlad      (1000)       27 2023-08-04 13:59:27.000000 types-aiobotocore-snowball-2.5.2.post2/types_aiobotocore_snowball.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:24:28.838787 types-aiobotocore-snowball-2.5.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-08 01:21:19.000000 types-aiobotocore-snowball-2.5.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    13663 2023-08-08 01:24:28.834787 types-aiobotocore-snowball-2.5.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    12147 2023-08-08 01:21:19.000000 types-aiobotocore-snowball-2.5.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-08 01:24:28.838787 types-aiobotocore-snowball-2.5.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2073 2023-08-08 01:21:19.000000 types-aiobotocore-snowball-2.5.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:24:28.834787 types-aiobotocore-snowball-2.5.4/types_aiobotocore_snowball/
+-rw-r--r--   0 runner    (1001) docker     (123)     1679 2023-08-08 01:21:19.000000 types-aiobotocore-snowball-2.5.4/types_aiobotocore_snowball/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1678 2023-08-08 01:21:19.000000 types-aiobotocore-snowball-2.5.4/types_aiobotocore_snowball/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      935 2023-08-08 01:21:19.000000 types-aiobotocore-snowball-2.5.4/types_aiobotocore_snowball/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26027 2023-08-08 01:21:19.000000 types-aiobotocore-snowball-2.5.4/types_aiobotocore_snowball/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25985 2023-08-08 01:21:19.000000 types-aiobotocore-snowball-2.5.4/types_aiobotocore_snowball/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    10698 2023-08-08 01:21:19.000000 types-aiobotocore-snowball-2.5.4/types_aiobotocore_snowball/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10696 2023-08-08 01:21:19.000000 types-aiobotocore-snowball-2.5.4/types_aiobotocore_snowball/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     7415 2023-08-08 01:21:19.000000 types-aiobotocore-snowball-2.5.4/types_aiobotocore_snowball/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7407 2023-08-08 01:21:19.000000 types-aiobotocore-snowball-2.5.4/types_aiobotocore_snowball/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 01:21:19.000000 types-aiobotocore-snowball-2.5.4/types_aiobotocore_snowball/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    28869 2023-08-08 01:21:20.000000 types-aiobotocore-snowball-2.5.4/types_aiobotocore_snowball/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28848 2023-08-08 01:21:19.000000 types-aiobotocore-snowball-2.5.4/types_aiobotocore_snowball/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-08-08 01:21:19.000000 types-aiobotocore-snowball-2.5.4/types_aiobotocore_snowball/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:24:28.834787 types-aiobotocore-snowball-2.5.4/types_aiobotocore_snowball.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    13663 2023-08-08 01:24:28.000000 types-aiobotocore-snowball-2.5.4/types_aiobotocore_snowball.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      832 2023-08-08 01:24:28.000000 types-aiobotocore-snowball-2.5.4/types_aiobotocore_snowball.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 01:24:28.000000 types-aiobotocore-snowball-2.5.4/types_aiobotocore_snowball.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 01:24:28.000000 types-aiobotocore-snowball-2.5.4/types_aiobotocore_snowball.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-08 01:24:28.000000 types-aiobotocore-snowball-2.5.4/types_aiobotocore_snowball.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-08-08 01:24:28.000000 types-aiobotocore-snowball-2.5.4/types_aiobotocore_snowball.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-snowball-2.5.2.post2/LICENSE` & `types-aiobotocore-snowball-2.5.4/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-snowball-2.5.2.post2/PKG-INFO` & `types-aiobotocore-snowball-2.5.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-snowball
-Version: 2.5.2.post2
-Summary: Type annotations for aiobotocore.Snowball 2.5.2 service generated with mypy-boto3-builder 7.17.2
+Version: 2.5.4
+Summary: Type annotations for aiobotocore.Snowball 2.5.4 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_snowball/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-snowball.svg?color=blue)](https://pypi.org/project/types-aiobotocore-snowball)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_snowball/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-snowball)](https://pepy.tech/project/types-aiobotocore-snowball)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.Snowball 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/snowball.html#Snowball)
+[aiobotocore.Snowball 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/snowball.html#Snowball)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-snowball-2.5.2.post2/README.md` & `types-aiobotocore-snowball-2.5.4/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-snowball.svg?color=blue)](https://pypi.org/project/types-aiobotocore-snowball)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_snowball/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-snowball)](https://pepy.tech/project/types-aiobotocore-snowball)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.Snowball 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/snowball.html#Snowball)
+[aiobotocore.Snowball 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/snowball.html#Snowball)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-snowball-2.5.2.post2/setup.py` & `types-aiobotocore-snowball-2.5.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-snowball",
-    version="2.5.2.post2",
+    version="2.5.4",
     packages=["types_aiobotocore_snowball"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.Snowball 2.5.2 service generated with mypy-boto3-builder"
+        "Type annotations for aiobotocore.Snowball 2.5.4 service generated with mypy-boto3-builder"
         " 7.17.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
```

### Comparing `types-aiobotocore-snowball-2.5.2.post2/types_aiobotocore_snowball/__init__.py` & `types-aiobotocore-snowball-2.5.4/types_aiobotocore_snowball/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-snowball-2.5.2.post2/types_aiobotocore_snowball/__init__.pyi` & `types-aiobotocore-snowball-2.5.4/types_aiobotocore_snowball/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-snowball-2.5.2.post2/types_aiobotocore_snowball/__main__.py` & `types-aiobotocore-snowball-2.5.4/types_aiobotocore_snowball/__main__.py`

 * *Files 11% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.Snowball 2.5.2\nVersion:         2.5.2.post2\nBuilder"
-        " version: 7.17.2\nDocs:           "
+        "Type annotations for aiobotocore.Snowball 2.5.4\nVersion:         2.5.4\nBuilder version:"
+        " 7.17.2\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_snowball//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/snowball.html#Snowball\nOther"
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

### Comparing `types-aiobotocore-snowball-2.5.2.post2/types_aiobotocore_snowball/client.py` & `types-aiobotocore-snowball-2.5.4/types_aiobotocore_snowball/client.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-snowball-2.5.2.post2/types_aiobotocore_snowball/client.pyi` & `types-aiobotocore-snowball-2.5.4/types_aiobotocore_snowball/client.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-snowball-2.5.2.post2/types_aiobotocore_snowball/literals.py` & `types-aiobotocore-snowball-2.5.4/types_aiobotocore_snowball/literals.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-snowball-2.5.2.post2/types_aiobotocore_snowball/literals.pyi` & `types-aiobotocore-snowball-2.5.4/types_aiobotocore_snowball/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-snowball-2.5.2.post2/types_aiobotocore_snowball/paginator.py` & `types-aiobotocore-snowball-2.5.4/types_aiobotocore_snowball/paginator.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-snowball-2.5.2.post2/types_aiobotocore_snowball/paginator.pyi` & `types-aiobotocore-snowball-2.5.4/types_aiobotocore_snowball/paginator.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-snowball-2.5.2.post2/types_aiobotocore_snowball/type_defs.py` & `types-aiobotocore-snowball-2.5.4/types_aiobotocore_snowball/type_defs.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-snowball-2.5.2.post2/types_aiobotocore_snowball/type_defs.pyi` & `types-aiobotocore-snowball-2.5.4/types_aiobotocore_snowball/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-snowball-2.5.2.post2/types_aiobotocore_snowball.egg-info/PKG-INFO` & `types-aiobotocore-snowball-2.5.4/types_aiobotocore_snowball.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-snowball
-Version: 2.5.2.post2
-Summary: Type annotations for aiobotocore.Snowball 2.5.2 service generated with mypy-boto3-builder 7.17.2
+Version: 2.5.4
+Summary: Type annotations for aiobotocore.Snowball 2.5.4 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_snowball/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-snowball.svg?color=blue)](https://pypi.org/project/types-aiobotocore-snowball)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_snowball/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-snowball)](https://pepy.tech/project/types-aiobotocore-snowball)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.Snowball 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/snowball.html#Snowball)
+[aiobotocore.Snowball 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/snowball.html#Snowball)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-snowball-2.5.2.post2/types_aiobotocore_snowball.egg-info/SOURCES.txt` & `types-aiobotocore-snowball-2.5.4/types_aiobotocore_snowball.egg-info/SOURCES.txt`

 * *Files identical despite different names*


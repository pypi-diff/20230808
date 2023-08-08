# Comparing `tmp/types-aiobotocore-simspaceweaver-2.5.2.post2.tar.gz` & `tmp/types-aiobotocore-simspaceweaver-2.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-simspaceweaver-2.5.2.post2.tar", last modified: Fri Aug  4 13:59:26 2023, max compression
+gzip compressed data, was "types-aiobotocore-simspaceweaver-2.5.4.tar", last modified: Tue Aug  8 01:24:27 2023, max compression
```

## Comparing `types-aiobotocore-simspaceweaver-2.5.2.post2.tar` & `types-aiobotocore-simspaceweaver-2.5.4.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:26.836643 types-aiobotocore-simspaceweaver-2.5.2.post2/
--rw-r--r--   0 vlad      (1000) vlad      (1000)     1070 2023-08-04 13:53:45.000000 types-aiobotocore-simspaceweaver-2.5.2.post2/LICENSE
--rw-r--r--   0 vlad      (1000) vlad      (1000)    12569 2023-08-04 13:59:26.836643 types-aiobotocore-simspaceweaver-2.5.2.post2/PKG-INFO
--rw-r--r--   0 vlad      (1000) vlad      (1000)    11023 2023-08-04 13:53:45.000000 types-aiobotocore-simspaceweaver-2.5.2.post2/README.md
--rw-r--r--   0 vlad      (1000) vlad      (1000)       38 2023-08-04 13:59:26.836643 types-aiobotocore-simspaceweaver-2.5.2.post2/setup.cfg
--rw-r--r--   0 vlad      (1000) vlad      (1000)     2121 2023-08-04 13:53:45.000000 types-aiobotocore-simspaceweaver-2.5.2.post2/setup.py
-drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:26.826643 types-aiobotocore-simspaceweaver-2.5.2.post2/types_aiobotocore_simspaceweaver/
--rw-r--r--   0 vlad      (1000) vlad      (1000)      498 2023-08-04 13:53:45.000000 types-aiobotocore-simspaceweaver-2.5.2.post2/types_aiobotocore_simspaceweaver/__init__.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)      497 2023-08-04 13:53:45.000000 types-aiobotocore-simspaceweaver-2.5.2.post2/types_aiobotocore_simspaceweaver/__init__.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)      971 2023-08-04 13:53:45.000000 types-aiobotocore-simspaceweaver-2.5.2.post2/types_aiobotocore_simspaceweaver/__main__.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)    13279 2023-08-04 13:53:45.000000 types-aiobotocore-simspaceweaver-2.5.2.post2/types_aiobotocore_simspaceweaver/client.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)    13255 2023-08-04 13:53:45.000000 types-aiobotocore-simspaceweaver-2.5.2.post2/types_aiobotocore_simspaceweaver/client.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)     8759 2023-08-04 13:53:45.000000 types-aiobotocore-simspaceweaver-2.5.2.post2/types_aiobotocore_simspaceweaver/literals.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)     8757 2023-08-04 13:53:45.000000 types-aiobotocore-simspaceweaver-2.5.2.post2/types_aiobotocore_simspaceweaver/literals.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:53:45.000000 types-aiobotocore-simspaceweaver-2.5.2.post2/types_aiobotocore_simspaceweaver/py.typed
--rw-r--r--   0 vlad      (1000) vlad      (1000)    10576 2023-08-04 13:53:45.000000 types-aiobotocore-simspaceweaver-2.5.2.post2/types_aiobotocore_simspaceweaver/type_defs.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)    10569 2023-08-04 13:53:45.000000 types-aiobotocore-simspaceweaver-2.5.2.post2/types_aiobotocore_simspaceweaver/type_defs.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)       65 2023-08-04 13:53:45.000000 types-aiobotocore-simspaceweaver-2.5.2.post2/types_aiobotocore_simspaceweaver/version.py
-drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:26.826643 types-aiobotocore-simspaceweaver-2.5.2.post2/types_aiobotocore_simspaceweaver.egg-info/
--rw-r--r--   0 vlad      (1000) vlad      (1000)    12569 2023-08-04 13:59:26.000000 types-aiobotocore-simspaceweaver-2.5.2.post2/types_aiobotocore_simspaceweaver.egg-info/PKG-INFO
--rw-r--r--   0 vlad      (1000) vlad      (1000)      853 2023-08-04 13:59:26.000000 types-aiobotocore-simspaceweaver-2.5.2.post2/types_aiobotocore_simspaceweaver.egg-info/SOURCES.txt
--rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:26.000000 types-aiobotocore-simspaceweaver-2.5.2.post2/types_aiobotocore_simspaceweaver.egg-info/dependency_links.txt
--rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:26.000000 types-aiobotocore-simspaceweaver-2.5.2.post2/types_aiobotocore_simspaceweaver.egg-info/not-zip-safe
--rw-r--r--   0 vlad      (1000) vlad      (1000)       52 2023-08-04 13:59:26.000000 types-aiobotocore-simspaceweaver-2.5.2.post2/types_aiobotocore_simspaceweaver.egg-info/requires.txt
--rw-r--r--   0 vlad      (1000) vlad      (1000)       33 2023-08-04 13:59:26.000000 types-aiobotocore-simspaceweaver-2.5.2.post2/types_aiobotocore_simspaceweaver.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:24:27.602784 types-aiobotocore-simspaceweaver-2.5.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-08 01:21:12.000000 types-aiobotocore-simspaceweaver-2.5.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    12563 2023-08-08 01:24:27.602784 types-aiobotocore-simspaceweaver-2.5.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    11023 2023-08-08 01:21:12.000000 types-aiobotocore-simspaceweaver-2.5.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-08 01:24:27.602784 types-aiobotocore-simspaceweaver-2.5.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2115 2023-08-08 01:21:12.000000 types-aiobotocore-simspaceweaver-2.5.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:24:27.602784 types-aiobotocore-simspaceweaver-2.5.4/types_aiobotocore_simspaceweaver/
+-rw-r--r--   0 runner    (1001) docker     (123)      498 2023-08-08 01:21:12.000000 types-aiobotocore-simspaceweaver-2.5.4/types_aiobotocore_simspaceweaver/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-08-08 01:21:12.000000 types-aiobotocore-simspaceweaver-2.5.4/types_aiobotocore_simspaceweaver/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      959 2023-08-08 01:21:12.000000 types-aiobotocore-simspaceweaver-2.5.4/types_aiobotocore_simspaceweaver/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13279 2023-08-08 01:21:12.000000 types-aiobotocore-simspaceweaver-2.5.4/types_aiobotocore_simspaceweaver/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13255 2023-08-08 01:21:12.000000 types-aiobotocore-simspaceweaver-2.5.4/types_aiobotocore_simspaceweaver/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8759 2023-08-08 01:21:12.000000 types-aiobotocore-simspaceweaver-2.5.4/types_aiobotocore_simspaceweaver/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8757 2023-08-08 01:21:12.000000 types-aiobotocore-simspaceweaver-2.5.4/types_aiobotocore_simspaceweaver/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 01:21:12.000000 types-aiobotocore-simspaceweaver-2.5.4/types_aiobotocore_simspaceweaver/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    10576 2023-08-08 01:21:12.000000 types-aiobotocore-simspaceweaver-2.5.4/types_aiobotocore_simspaceweaver/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10569 2023-08-08 01:21:12.000000 types-aiobotocore-simspaceweaver-2.5.4/types_aiobotocore_simspaceweaver/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-08-08 01:21:12.000000 types-aiobotocore-simspaceweaver-2.5.4/types_aiobotocore_simspaceweaver/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:24:27.602784 types-aiobotocore-simspaceweaver-2.5.4/types_aiobotocore_simspaceweaver.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    12563 2023-08-08 01:24:27.000000 types-aiobotocore-simspaceweaver-2.5.4/types_aiobotocore_simspaceweaver.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      853 2023-08-08 01:24:27.000000 types-aiobotocore-simspaceweaver-2.5.4/types_aiobotocore_simspaceweaver.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 01:24:27.000000 types-aiobotocore-simspaceweaver-2.5.4/types_aiobotocore_simspaceweaver.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 01:24:27.000000 types-aiobotocore-simspaceweaver-2.5.4/types_aiobotocore_simspaceweaver.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-08 01:24:27.000000 types-aiobotocore-simspaceweaver-2.5.4/types_aiobotocore_simspaceweaver.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-08-08 01:24:27.000000 types-aiobotocore-simspaceweaver-2.5.4/types_aiobotocore_simspaceweaver.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-simspaceweaver-2.5.2.post2/LICENSE` & `types-aiobotocore-simspaceweaver-2.5.4/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-simspaceweaver-2.5.2.post2/PKG-INFO` & `types-aiobotocore-simspaceweaver-2.5.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-simspaceweaver
-Version: 2.5.2.post2
-Summary: Type annotations for aiobotocore.SimSpaceWeaver 2.5.2 service generated with mypy-boto3-builder 7.17.2
+Version: 2.5.4
+Summary: Type annotations for aiobotocore.SimSpaceWeaver 2.5.4 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_simspaceweaver/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-simspaceweaver.svg?color=blue)](https://pypi.org/project/types-aiobotocore-simspaceweaver)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_simspaceweaver/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-simspaceweaver)](https://pepy.tech/project/types-aiobotocore-simspaceweaver)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.SimSpaceWeaver 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/simspaceweaver.html#SimSpaceWeaver)
+[aiobotocore.SimSpaceWeaver 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/simspaceweaver.html#SimSpaceWeaver)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-simspaceweaver-2.5.2.post2/README.md` & `types-aiobotocore-simspaceweaver-2.5.4/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-simspaceweaver.svg?color=blue)](https://pypi.org/project/types-aiobotocore-simspaceweaver)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_simspaceweaver/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-simspaceweaver)](https://pepy.tech/project/types-aiobotocore-simspaceweaver)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.SimSpaceWeaver 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/simspaceweaver.html#SimSpaceWeaver)
+[aiobotocore.SimSpaceWeaver 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/simspaceweaver.html#SimSpaceWeaver)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-simspaceweaver-2.5.2.post2/setup.py` & `types-aiobotocore-simspaceweaver-2.5.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-simspaceweaver",
-    version="2.5.2.post2",
+    version="2.5.4",
     packages=["types_aiobotocore_simspaceweaver"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.SimSpaceWeaver 2.5.2 service generated with"
+        "Type annotations for aiobotocore.SimSpaceWeaver 2.5.4 service generated with"
         " mypy-boto3-builder 7.17.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
```

### Comparing `types-aiobotocore-simspaceweaver-2.5.2.post2/types_aiobotocore_simspaceweaver/__main__.py` & `types-aiobotocore-simspaceweaver-2.5.4/types_aiobotocore_simspaceweaver/__main__.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.SimSpaceWeaver 2.5.2\nVersion:        "
-        " 2.5.2.post2\nBuilder version: 7.17.2\nDocs:           "
+        "Type annotations for aiobotocore.SimSpaceWeaver 2.5.4\nVersion:         2.5.4\nBuilder"
+        " version: 7.17.2\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_simspaceweaver//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/simspaceweaver.html#SimSpaceWeaver\nOther"
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

### Comparing `types-aiobotocore-simspaceweaver-2.5.2.post2/types_aiobotocore_simspaceweaver/client.py` & `types-aiobotocore-simspaceweaver-2.5.4/types_aiobotocore_simspaceweaver/client.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-simspaceweaver-2.5.2.post2/types_aiobotocore_simspaceweaver/client.pyi` & `types-aiobotocore-simspaceweaver-2.5.4/types_aiobotocore_simspaceweaver/client.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-simspaceweaver-2.5.2.post2/types_aiobotocore_simspaceweaver/literals.py` & `types-aiobotocore-simspaceweaver-2.5.4/types_aiobotocore_simspaceweaver/literals.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-simspaceweaver-2.5.2.post2/types_aiobotocore_simspaceweaver/literals.pyi` & `types-aiobotocore-simspaceweaver-2.5.4/types_aiobotocore_simspaceweaver/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-simspaceweaver-2.5.2.post2/types_aiobotocore_simspaceweaver/type_defs.py` & `types-aiobotocore-simspaceweaver-2.5.4/types_aiobotocore_simspaceweaver/type_defs.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-simspaceweaver-2.5.2.post2/types_aiobotocore_simspaceweaver/type_defs.pyi` & `types-aiobotocore-simspaceweaver-2.5.4/types_aiobotocore_simspaceweaver/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-simspaceweaver-2.5.2.post2/types_aiobotocore_simspaceweaver.egg-info/PKG-INFO` & `types-aiobotocore-simspaceweaver-2.5.4/types_aiobotocore_simspaceweaver.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-simspaceweaver
-Version: 2.5.2.post2
-Summary: Type annotations for aiobotocore.SimSpaceWeaver 2.5.2 service generated with mypy-boto3-builder 7.17.2
+Version: 2.5.4
+Summary: Type annotations for aiobotocore.SimSpaceWeaver 2.5.4 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_simspaceweaver/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-simspaceweaver.svg?color=blue)](https://pypi.org/project/types-aiobotocore-simspaceweaver)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_simspaceweaver/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-simspaceweaver)](https://pepy.tech/project/types-aiobotocore-simspaceweaver)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.SimSpaceWeaver 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/simspaceweaver.html#SimSpaceWeaver)
+[aiobotocore.SimSpaceWeaver 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/simspaceweaver.html#SimSpaceWeaver)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-simspaceweaver-2.5.2.post2/types_aiobotocore_simspaceweaver.egg-info/SOURCES.txt` & `types-aiobotocore-simspaceweaver-2.5.4/types_aiobotocore_simspaceweaver.egg-info/SOURCES.txt`

 * *Files identical despite different names*


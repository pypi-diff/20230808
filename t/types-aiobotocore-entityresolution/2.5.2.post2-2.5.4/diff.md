# Comparing `tmp/types-aiobotocore-entityresolution-2.5.2.post2.tar.gz` & `tmp/types-aiobotocore-entityresolution-2.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-entityresolution-2.5.2.post2.tar", last modified: Fri Aug  4 13:59:11 2023, max compression
+gzip compressed data, was "types-aiobotocore-entityresolution-2.5.4.tar", last modified: Tue Aug  8 01:23:43 2023, max compression
```

## Comparing `types-aiobotocore-entityresolution-2.5.2.post2.tar` & `types-aiobotocore-entityresolution-2.5.4.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:11.216642 types-aiobotocore-entityresolution-2.5.2.post2/
--rw-r--r--   0 vlad      (1000) vlad      (1000)     1070 2023-08-04 13:40:00.000000 types-aiobotocore-entityresolution-2.5.2.post2/LICENSE
--rw-r--r--   0 vlad      (1000) vlad      (1000)    13819 2023-08-04 13:59:11.216642 types-aiobotocore-entityresolution-2.5.2.post2/PKG-INFO
--rw-r--r--   0 vlad      (1000) vlad      (1000)    12265 2023-08-04 13:40:00.000000 types-aiobotocore-entityresolution-2.5.2.post2/README.md
--rw-r--r--   0 vlad      (1000) vlad      (1000)       38 2023-08-04 13:59:11.216642 types-aiobotocore-entityresolution-2.5.2.post2/setup.cfg
--rw-r--r--   0 vlad      (1000) vlad      (1000)     2135 2023-08-04 13:39:59.000000 types-aiobotocore-entityresolution-2.5.2.post2/setup.py
-drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:11.206642 types-aiobotocore-entityresolution-2.5.2.post2/types_aiobotocore_entityresolution/
--rw-r--r--   0 vlad      (1000) vlad      (1000)     1207 2023-08-04 13:40:00.000000 types-aiobotocore-entityresolution-2.5.2.post2/types_aiobotocore_entityresolution/__init__.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)     1206 2023-08-04 13:40:00.000000 types-aiobotocore-entityresolution-2.5.2.post2/types_aiobotocore_entityresolution/__init__.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)      979 2023-08-04 13:40:00.000000 types-aiobotocore-entityresolution-2.5.2.post2/types_aiobotocore_entityresolution/__main__.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)    16604 2023-08-04 13:40:00.000000 types-aiobotocore-entityresolution-2.5.2.post2/types_aiobotocore_entityresolution/client.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)    16576 2023-08-04 13:40:00.000000 types-aiobotocore-entityresolution-2.5.2.post2/types_aiobotocore_entityresolution/client.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)     8909 2023-08-04 13:40:00.000000 types-aiobotocore-entityresolution-2.5.2.post2/types_aiobotocore_entityresolution/literals.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)     8907 2023-08-04 13:40:00.000000 types-aiobotocore-entityresolution-2.5.2.post2/types_aiobotocore_entityresolution/literals.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)     4508 2023-08-04 13:40:00.000000 types-aiobotocore-entityresolution-2.5.2.post2/types_aiobotocore_entityresolution/paginator.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)     4503 2023-08-04 13:40:00.000000 types-aiobotocore-entityresolution-2.5.2.post2/types_aiobotocore_entityresolution/paginator.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:40:00.000000 types-aiobotocore-entityresolution-2.5.2.post2/types_aiobotocore_entityresolution/py.typed
--rw-r--r--   0 vlad      (1000) vlad      (1000)    16520 2023-08-04 13:40:01.000000 types-aiobotocore-entityresolution-2.5.2.post2/types_aiobotocore_entityresolution/type_defs.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)    16499 2023-08-04 13:40:00.000000 types-aiobotocore-entityresolution-2.5.2.post2/types_aiobotocore_entityresolution/type_defs.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)       65 2023-08-04 13:40:00.000000 types-aiobotocore-entityresolution-2.5.2.post2/types_aiobotocore_entityresolution/version.py
-drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:11.216642 types-aiobotocore-entityresolution-2.5.2.post2/types_aiobotocore_entityresolution.egg-info/
--rw-r--r--   0 vlad      (1000) vlad      (1000)    13819 2023-08-04 13:59:11.000000 types-aiobotocore-entityresolution-2.5.2.post2/types_aiobotocore_entityresolution.egg-info/PKG-INFO
--rw-r--r--   0 vlad      (1000) vlad      (1000)      984 2023-08-04 13:59:11.000000 types-aiobotocore-entityresolution-2.5.2.post2/types_aiobotocore_entityresolution.egg-info/SOURCES.txt
--rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:11.000000 types-aiobotocore-entityresolution-2.5.2.post2/types_aiobotocore_entityresolution.egg-info/dependency_links.txt
--rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:11.000000 types-aiobotocore-entityresolution-2.5.2.post2/types_aiobotocore_entityresolution.egg-info/not-zip-safe
--rw-r--r--   0 vlad      (1000) vlad      (1000)       52 2023-08-04 13:59:11.000000 types-aiobotocore-entityresolution-2.5.2.post2/types_aiobotocore_entityresolution.egg-info/requires.txt
--rw-r--r--   0 vlad      (1000) vlad      (1000)       35 2023-08-04 13:59:11.000000 types-aiobotocore-entityresolution-2.5.2.post2/types_aiobotocore_entityresolution.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:23:43.202714 types-aiobotocore-entityresolution-2.5.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-08 01:10:58.000000 types-aiobotocore-entityresolution-2.5.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    13813 2023-08-08 01:23:43.202714 types-aiobotocore-entityresolution-2.5.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    12265 2023-08-08 01:10:58.000000 types-aiobotocore-entityresolution-2.5.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-08 01:23:43.202714 types-aiobotocore-entityresolution-2.5.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2129 2023-08-08 01:10:58.000000 types-aiobotocore-entityresolution-2.5.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:23:43.198714 types-aiobotocore-entityresolution-2.5.4/types_aiobotocore_entityresolution/
+-rw-r--r--   0 runner    (1001) docker     (123)     1207 2023-08-08 01:10:58.000000 types-aiobotocore-entityresolution-2.5.4/types_aiobotocore_entityresolution/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1206 2023-08-08 01:10:58.000000 types-aiobotocore-entityresolution-2.5.4/types_aiobotocore_entityresolution/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      967 2023-08-08 01:10:58.000000 types-aiobotocore-entityresolution-2.5.4/types_aiobotocore_entityresolution/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16604 2023-08-08 01:10:58.000000 types-aiobotocore-entityresolution-2.5.4/types_aiobotocore_entityresolution/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16576 2023-08-08 01:10:58.000000 types-aiobotocore-entityresolution-2.5.4/types_aiobotocore_entityresolution/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8909 2023-08-08 01:10:58.000000 types-aiobotocore-entityresolution-2.5.4/types_aiobotocore_entityresolution/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8907 2023-08-08 01:10:58.000000 types-aiobotocore-entityresolution-2.5.4/types_aiobotocore_entityresolution/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     4508 2023-08-08 01:10:58.000000 types-aiobotocore-entityresolution-2.5.4/types_aiobotocore_entityresolution/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4503 2023-08-08 01:10:58.000000 types-aiobotocore-entityresolution-2.5.4/types_aiobotocore_entityresolution/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 01:10:58.000000 types-aiobotocore-entityresolution-2.5.4/types_aiobotocore_entityresolution/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    16520 2023-08-08 01:10:58.000000 types-aiobotocore-entityresolution-2.5.4/types_aiobotocore_entityresolution/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16499 2023-08-08 01:10:58.000000 types-aiobotocore-entityresolution-2.5.4/types_aiobotocore_entityresolution/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-08-08 01:10:58.000000 types-aiobotocore-entityresolution-2.5.4/types_aiobotocore_entityresolution/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:23:43.202714 types-aiobotocore-entityresolution-2.5.4/types_aiobotocore_entityresolution.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    13813 2023-08-08 01:23:43.000000 types-aiobotocore-entityresolution-2.5.4/types_aiobotocore_entityresolution.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      984 2023-08-08 01:23:43.000000 types-aiobotocore-entityresolution-2.5.4/types_aiobotocore_entityresolution.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 01:23:43.000000 types-aiobotocore-entityresolution-2.5.4/types_aiobotocore_entityresolution.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 01:23:43.000000 types-aiobotocore-entityresolution-2.5.4/types_aiobotocore_entityresolution.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-08 01:23:43.000000 types-aiobotocore-entityresolution-2.5.4/types_aiobotocore_entityresolution.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-08-08 01:23:43.000000 types-aiobotocore-entityresolution-2.5.4/types_aiobotocore_entityresolution.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-entityresolution-2.5.2.post2/LICENSE` & `types-aiobotocore-entityresolution-2.5.4/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-entityresolution-2.5.2.post2/PKG-INFO` & `types-aiobotocore-entityresolution-2.5.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-entityresolution
-Version: 2.5.2.post2
-Summary: Type annotations for aiobotocore.EntityResolution 2.5.2 service generated with mypy-boto3-builder 7.17.2
+Version: 2.5.4
+Summary: Type annotations for aiobotocore.EntityResolution 2.5.4 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_entityresolution/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-entityresolution.svg?color=blue)](https://pypi.org/project/types-aiobotocore-entityresolution)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_entityresolution/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-entityresolution)](https://pepy.tech/project/types-aiobotocore-entityresolution)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.EntityResolution 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/entityresolution.html#EntityResolution)
+[aiobotocore.EntityResolution 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/entityresolution.html#EntityResolution)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-entityresolution-2.5.2.post2/README.md` & `types-aiobotocore-entityresolution-2.5.4/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-entityresolution.svg?color=blue)](https://pypi.org/project/types-aiobotocore-entityresolution)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_entityresolution/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-entityresolution)](https://pepy.tech/project/types-aiobotocore-entityresolution)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.EntityResolution 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/entityresolution.html#EntityResolution)
+[aiobotocore.EntityResolution 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/entityresolution.html#EntityResolution)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-entityresolution-2.5.2.post2/setup.py` & `types-aiobotocore-entityresolution-2.5.4/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-entityresolution",
-    version="2.5.2.post2",
+    version="2.5.4",
     packages=["types_aiobotocore_entityresolution"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.EntityResolution 2.5.2 service generated with"
+        "Type annotations for aiobotocore.EntityResolution 2.5.4 service generated with"
         " mypy-boto3-builder 7.17.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
```

### Comparing `types-aiobotocore-entityresolution-2.5.2.post2/types_aiobotocore_entityresolution/__init__.py` & `types-aiobotocore-entityresolution-2.5.4/types_aiobotocore_entityresolution/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-entityresolution-2.5.2.post2/types_aiobotocore_entityresolution/__init__.pyi` & `types-aiobotocore-entityresolution-2.5.4/types_aiobotocore_entityresolution/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-entityresolution-2.5.2.post2/types_aiobotocore_entityresolution/__main__.py` & `types-aiobotocore-entityresolution-2.5.4/types_aiobotocore_entityresolution/__main__.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.EntityResolution 2.5.2\nVersion:        "
-        " 2.5.2.post2\nBuilder version: 7.17.2\nDocs:           "
+        "Type annotations for aiobotocore.EntityResolution 2.5.4\nVersion:         2.5.4\nBuilder"
+        " version: 7.17.2\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_entityresolution//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/entityresolution.html#EntityResolution\nOther"
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

### Comparing `types-aiobotocore-entityresolution-2.5.2.post2/types_aiobotocore_entityresolution/client.py` & `types-aiobotocore-entityresolution-2.5.4/types_aiobotocore_entityresolution/client.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-entityresolution-2.5.2.post2/types_aiobotocore_entityresolution/client.pyi` & `types-aiobotocore-entityresolution-2.5.4/types_aiobotocore_entityresolution/client.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-entityresolution-2.5.2.post2/types_aiobotocore_entityresolution/literals.py` & `types-aiobotocore-entityresolution-2.5.4/types_aiobotocore_entityresolution/literals.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-entityresolution-2.5.2.post2/types_aiobotocore_entityresolution/literals.pyi` & `types-aiobotocore-entityresolution-2.5.4/types_aiobotocore_entityresolution/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-entityresolution-2.5.2.post2/types_aiobotocore_entityresolution/paginator.py` & `types-aiobotocore-entityresolution-2.5.4/types_aiobotocore_entityresolution/paginator.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-entityresolution-2.5.2.post2/types_aiobotocore_entityresolution/paginator.pyi` & `types-aiobotocore-entityresolution-2.5.4/types_aiobotocore_entityresolution/paginator.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-entityresolution-2.5.2.post2/types_aiobotocore_entityresolution/type_defs.py` & `types-aiobotocore-entityresolution-2.5.4/types_aiobotocore_entityresolution/type_defs.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-entityresolution-2.5.2.post2/types_aiobotocore_entityresolution/type_defs.pyi` & `types-aiobotocore-entityresolution-2.5.4/types_aiobotocore_entityresolution/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-entityresolution-2.5.2.post2/types_aiobotocore_entityresolution.egg-info/PKG-INFO` & `types-aiobotocore-entityresolution-2.5.4/types_aiobotocore_entityresolution.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-entityresolution
-Version: 2.5.2.post2
-Summary: Type annotations for aiobotocore.EntityResolution 2.5.2 service generated with mypy-boto3-builder 7.17.2
+Version: 2.5.4
+Summary: Type annotations for aiobotocore.EntityResolution 2.5.4 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_entityresolution/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-entityresolution.svg?color=blue)](https://pypi.org/project/types-aiobotocore-entityresolution)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_entityresolution/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-entityresolution)](https://pepy.tech/project/types-aiobotocore-entityresolution)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.EntityResolution 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/entityresolution.html#EntityResolution)
+[aiobotocore.EntityResolution 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/entityresolution.html#EntityResolution)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-entityresolution-2.5.2.post2/types_aiobotocore_entityresolution.egg-info/SOURCES.txt` & `types-aiobotocore-entityresolution-2.5.4/types_aiobotocore_entityresolution.egg-info/SOURCES.txt`

 * *Files identical despite different names*


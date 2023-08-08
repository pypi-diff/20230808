# Comparing `tmp/types-aiobotocore-location-2.5.2.post2.tar.gz` & `tmp/types-aiobotocore-location-2.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-location-2.5.2.post2.tar", last modified: Fri Aug  4 13:59:15 2023, max compression
+gzip compressed data, was "types-aiobotocore-location-2.5.4.tar", last modified: Tue Aug  8 01:24:01 2023, max compression
```

## Comparing `types-aiobotocore-location-2.5.2.post2.tar` & `types-aiobotocore-location-2.5.4.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:15.956643 types-aiobotocore-location-2.5.2.post2/
--rw-r--r--   0 vlad      (1000) vlad      (1000)     1070 2023-08-04 13:43:16.000000 types-aiobotocore-location-2.5.2.post2/LICENSE
--rw-r--r--   0 vlad      (1000) vlad      (1000)    14372 2023-08-04 13:59:15.956643 types-aiobotocore-location-2.5.2.post2/PKG-INFO
--rw-r--r--   0 vlad      (1000) vlad      (1000)    12843 2023-08-04 13:43:16.000000 types-aiobotocore-location-2.5.2.post2/README.md
--rw-r--r--   0 vlad      (1000) vlad      (1000)       38 2023-08-04 13:59:15.956643 types-aiobotocore-location-2.5.2.post2/setup.cfg
--rw-r--r--   0 vlad      (1000) vlad      (1000)     2086 2023-08-04 13:43:15.000000 types-aiobotocore-location-2.5.2.post2/setup.py
-drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:15.946643 types-aiobotocore-location-2.5.2.post2/types_aiobotocore_location/
--rw-r--r--   0 vlad      (1000) vlad      (1000)     2576 2023-08-04 13:43:16.000000 types-aiobotocore-location-2.5.2.post2/types_aiobotocore_location/__init__.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)     2575 2023-08-04 13:43:16.000000 types-aiobotocore-location-2.5.2.post2/types_aiobotocore_location/__init__.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)      961 2023-08-04 13:43:16.000000 types-aiobotocore-location-2.5.2.post2/types_aiobotocore_location/__main__.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)    48161 2023-08-04 13:43:16.000000 types-aiobotocore-location-2.5.2.post2/types_aiobotocore_location/client.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)    48084 2023-08-04 13:43:16.000000 types-aiobotocore-location-2.5.2.post2/types_aiobotocore_location/client.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)    10376 2023-08-04 13:43:17.000000 types-aiobotocore-location-2.5.2.post2/types_aiobotocore_location/literals.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)    10374 2023-08-04 13:43:16.000000 types-aiobotocore-location-2.5.2.post2/types_aiobotocore_location/literals.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)    12337 2023-08-04 13:43:16.000000 types-aiobotocore-location-2.5.2.post2/types_aiobotocore_location/paginator.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)    12325 2023-08-04 13:43:16.000000 types-aiobotocore-location-2.5.2.post2/types_aiobotocore_location/paginator.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:43:16.000000 types-aiobotocore-location-2.5.2.post2/types_aiobotocore_location/py.typed
--rw-r--r--   0 vlad      (1000) vlad      (1000)    65015 2023-08-04 13:43:18.000000 types-aiobotocore-location-2.5.2.post2/types_aiobotocore_location/type_defs.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)    64904 2023-08-04 13:43:17.000000 types-aiobotocore-location-2.5.2.post2/types_aiobotocore_location/type_defs.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)       65 2023-08-04 13:43:16.000000 types-aiobotocore-location-2.5.2.post2/types_aiobotocore_location/version.py
-drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:15.946643 types-aiobotocore-location-2.5.2.post2/types_aiobotocore_location.egg-info/
--rw-r--r--   0 vlad      (1000) vlad      (1000)    14372 2023-08-04 13:59:15.000000 types-aiobotocore-location-2.5.2.post2/types_aiobotocore_location.egg-info/PKG-INFO
--rw-r--r--   0 vlad      (1000) vlad      (1000)      832 2023-08-04 13:59:15.000000 types-aiobotocore-location-2.5.2.post2/types_aiobotocore_location.egg-info/SOURCES.txt
--rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:15.000000 types-aiobotocore-location-2.5.2.post2/types_aiobotocore_location.egg-info/dependency_links.txt
--rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:15.000000 types-aiobotocore-location-2.5.2.post2/types_aiobotocore_location.egg-info/not-zip-safe
--rw-r--r--   0 vlad      (1000) vlad      (1000)       52 2023-08-04 13:59:15.000000 types-aiobotocore-location-2.5.2.post2/types_aiobotocore_location.egg-info/requires.txt
--rw-r--r--   0 vlad      (1000) vlad      (1000)       27 2023-08-04 13:59:15.000000 types-aiobotocore-location-2.5.2.post2/types_aiobotocore_location.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:24:01.786724 types-aiobotocore-location-2.5.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-08 01:14:25.000000 types-aiobotocore-location-2.5.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    14366 2023-08-08 01:24:01.786724 types-aiobotocore-location-2.5.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    12843 2023-08-08 01:14:25.000000 types-aiobotocore-location-2.5.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-08 01:24:01.786724 types-aiobotocore-location-2.5.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2080 2023-08-08 01:14:25.000000 types-aiobotocore-location-2.5.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:24:01.782724 types-aiobotocore-location-2.5.4/types_aiobotocore_location/
+-rw-r--r--   0 runner    (1001) docker     (123)     2576 2023-08-08 01:14:25.000000 types-aiobotocore-location-2.5.4/types_aiobotocore_location/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2575 2023-08-08 01:14:25.000000 types-aiobotocore-location-2.5.4/types_aiobotocore_location/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      949 2023-08-08 01:14:25.000000 types-aiobotocore-location-2.5.4/types_aiobotocore_location/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    48161 2023-08-08 01:14:25.000000 types-aiobotocore-location-2.5.4/types_aiobotocore_location/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    48084 2023-08-08 01:14:25.000000 types-aiobotocore-location-2.5.4/types_aiobotocore_location/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    10376 2023-08-08 01:14:26.000000 types-aiobotocore-location-2.5.4/types_aiobotocore_location/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10374 2023-08-08 01:14:26.000000 types-aiobotocore-location-2.5.4/types_aiobotocore_location/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    12337 2023-08-08 01:14:26.000000 types-aiobotocore-location-2.5.4/types_aiobotocore_location/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12325 2023-08-08 01:14:26.000000 types-aiobotocore-location-2.5.4/types_aiobotocore_location/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 01:14:25.000000 types-aiobotocore-location-2.5.4/types_aiobotocore_location/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    65015 2023-08-08 01:14:27.000000 types-aiobotocore-location-2.5.4/types_aiobotocore_location/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    64904 2023-08-08 01:14:26.000000 types-aiobotocore-location-2.5.4/types_aiobotocore_location/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-08-08 01:14:25.000000 types-aiobotocore-location-2.5.4/types_aiobotocore_location/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:24:01.786724 types-aiobotocore-location-2.5.4/types_aiobotocore_location.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    14366 2023-08-08 01:24:01.000000 types-aiobotocore-location-2.5.4/types_aiobotocore_location.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      832 2023-08-08 01:24:01.000000 types-aiobotocore-location-2.5.4/types_aiobotocore_location.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 01:24:01.000000 types-aiobotocore-location-2.5.4/types_aiobotocore_location.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 01:24:01.000000 types-aiobotocore-location-2.5.4/types_aiobotocore_location.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-08 01:24:01.000000 types-aiobotocore-location-2.5.4/types_aiobotocore_location.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-08-08 01:24:01.000000 types-aiobotocore-location-2.5.4/types_aiobotocore_location.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-location-2.5.2.post2/LICENSE` & `types-aiobotocore-location-2.5.4/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-location-2.5.2.post2/PKG-INFO` & `types-aiobotocore-location-2.5.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-location
-Version: 2.5.2.post2
-Summary: Type annotations for aiobotocore.LocationService 2.5.2 service generated with mypy-boto3-builder 7.17.2
+Version: 2.5.4
+Summary: Type annotations for aiobotocore.LocationService 2.5.4 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_location/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-location.svg?color=blue)](https://pypi.org/project/types-aiobotocore-location)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_location/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-location)](https://pepy.tech/project/types-aiobotocore-location)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.LocationService 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/location.html#LocationService)
+[aiobotocore.LocationService 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/location.html#LocationService)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-location-2.5.2.post2/README.md` & `types-aiobotocore-location-2.5.4/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-location.svg?color=blue)](https://pypi.org/project/types-aiobotocore-location)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_location/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-location)](https://pepy.tech/project/types-aiobotocore-location)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.LocationService 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/location.html#LocationService)
+[aiobotocore.LocationService 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/location.html#LocationService)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-location-2.5.2.post2/setup.py` & `types-aiobotocore-location-2.5.4/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-location",
-    version="2.5.2.post2",
+    version="2.5.4",
     packages=["types_aiobotocore_location"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.LocationService 2.5.2 service generated with"
+        "Type annotations for aiobotocore.LocationService 2.5.4 service generated with"
         " mypy-boto3-builder 7.17.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
```

### Comparing `types-aiobotocore-location-2.5.2.post2/types_aiobotocore_location/__init__.py` & `types-aiobotocore-location-2.5.4/types_aiobotocore_location/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-location-2.5.2.post2/types_aiobotocore_location/__init__.pyi` & `types-aiobotocore-location-2.5.4/types_aiobotocore_location/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-location-2.5.2.post2/types_aiobotocore_location/__main__.py` & `types-aiobotocore-location-2.5.4/types_aiobotocore_location/__main__.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.LocationService 2.5.2\nVersion:        "
-        " 2.5.2.post2\nBuilder version: 7.17.2\nDocs:           "
+        "Type annotations for aiobotocore.LocationService 2.5.4\nVersion:         2.5.4\nBuilder"
+        " version: 7.17.2\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_location//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/location.html#LocationService\nOther"
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

### Comparing `types-aiobotocore-location-2.5.2.post2/types_aiobotocore_location/client.py` & `types-aiobotocore-location-2.5.4/types_aiobotocore_location/client.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-location-2.5.2.post2/types_aiobotocore_location/client.pyi` & `types-aiobotocore-location-2.5.4/types_aiobotocore_location/client.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-location-2.5.2.post2/types_aiobotocore_location/literals.py` & `types-aiobotocore-location-2.5.4/types_aiobotocore_location/literals.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-location-2.5.2.post2/types_aiobotocore_location/literals.pyi` & `types-aiobotocore-location-2.5.4/types_aiobotocore_location/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-location-2.5.2.post2/types_aiobotocore_location/paginator.py` & `types-aiobotocore-location-2.5.4/types_aiobotocore_location/paginator.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-location-2.5.2.post2/types_aiobotocore_location/paginator.pyi` & `types-aiobotocore-location-2.5.4/types_aiobotocore_location/paginator.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-location-2.5.2.post2/types_aiobotocore_location/type_defs.py` & `types-aiobotocore-location-2.5.4/types_aiobotocore_location/type_defs.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-location-2.5.2.post2/types_aiobotocore_location/type_defs.pyi` & `types-aiobotocore-location-2.5.4/types_aiobotocore_location/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-location-2.5.2.post2/types_aiobotocore_location.egg-info/PKG-INFO` & `types-aiobotocore-location-2.5.4/types_aiobotocore_location.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-location
-Version: 2.5.2.post2
-Summary: Type annotations for aiobotocore.LocationService 2.5.2 service generated with mypy-boto3-builder 7.17.2
+Version: 2.5.4
+Summary: Type annotations for aiobotocore.LocationService 2.5.4 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_location/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-location.svg?color=blue)](https://pypi.org/project/types-aiobotocore-location)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_location/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-location)](https://pepy.tech/project/types-aiobotocore-location)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.LocationService 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/location.html#LocationService)
+[aiobotocore.LocationService 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/location.html#LocationService)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-location-2.5.2.post2/types_aiobotocore_location.egg-info/SOURCES.txt` & `types-aiobotocore-location-2.5.4/types_aiobotocore_location.egg-info/SOURCES.txt`

 * *Files identical despite different names*


# Comparing `tmp/types-aiobotocore-mediastore-data-2.5.2.post2.tar.gz` & `tmp/types-aiobotocore-mediastore-data-2.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-mediastore-data-2.5.2.post2.tar", last modified: Fri Aug  4 13:59:18 2023, max compression
+gzip compressed data, was "types-aiobotocore-mediastore-data-2.5.4.tar", last modified: Tue Aug  8 01:24:06 2023, max compression
```

## Comparing `types-aiobotocore-mediastore-data-2.5.2.post2.tar` & `types-aiobotocore-mediastore-data-2.5.4.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:18.326643 types-aiobotocore-mediastore-data-2.5.2.post2/
--rw-r--r--   0 vlad      (1000) vlad      (1000)     1070 2023-08-04 13:44:40.000000 types-aiobotocore-mediastore-data-2.5.2.post2/LICENSE
--rw-r--r--   0 vlad      (1000) vlad      (1000)    13308 2023-08-04 13:59:18.326643 types-aiobotocore-mediastore-data-2.5.2.post2/PKG-INFO
--rw-r--r--   0 vlad      (1000) vlad      (1000)    11759 2023-08-04 13:44:40.000000 types-aiobotocore-mediastore-data-2.5.2.post2/README.md
--rw-r--r--   0 vlad      (1000) vlad      (1000)       38 2023-08-04 13:59:18.326643 types-aiobotocore-mediastore-data-2.5.2.post2/setup.cfg
--rw-r--r--   0 vlad      (1000) vlad      (1000)     2127 2023-08-04 13:44:40.000000 types-aiobotocore-mediastore-data-2.5.2.post2/setup.py
-drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:18.326643 types-aiobotocore-mediastore-data-2.5.2.post2/types_aiobotocore_mediastore_data/
--rw-r--r--   0 vlad      (1000) vlad      (1000)      676 2023-08-04 13:44:40.000000 types-aiobotocore-mediastore-data-2.5.2.post2/types_aiobotocore_mediastore_data/__init__.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)      675 2023-08-04 13:44:40.000000 types-aiobotocore-mediastore-data-2.5.2.post2/types_aiobotocore_mediastore_data/__init__.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)      973 2023-08-04 13:44:40.000000 types-aiobotocore-mediastore-data-2.5.2.post2/types_aiobotocore_mediastore_data/__main__.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)     7770 2023-08-04 13:44:40.000000 types-aiobotocore-mediastore-data-2.5.2.post2/types_aiobotocore_mediastore_data/client.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)     7755 2023-08-04 13:44:40.000000 types-aiobotocore-mediastore-data-2.5.2.post2/types_aiobotocore_mediastore_data/client.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)     8212 2023-08-04 13:44:41.000000 types-aiobotocore-mediastore-data-2.5.2.post2/types_aiobotocore_mediastore_data/literals.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)     8210 2023-08-04 13:44:40.000000 types-aiobotocore-mediastore-data-2.5.2.post2/types_aiobotocore_mediastore_data/literals.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)     2036 2023-08-04 13:44:40.000000 types-aiobotocore-mediastore-data-2.5.2.post2/types_aiobotocore_mediastore_data/paginator.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)     2033 2023-08-04 13:44:40.000000 types-aiobotocore-mediastore-data-2.5.2.post2/types_aiobotocore_mediastore_data/paginator.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:44:40.000000 types-aiobotocore-mediastore-data-2.5.2.post2/types_aiobotocore_mediastore_data/py.typed
--rw-r--r--   0 vlad      (1000) vlad      (1000)     4711 2023-08-04 13:44:41.000000 types-aiobotocore-mediastore-data-2.5.2.post2/types_aiobotocore_mediastore_data/type_defs.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)     4706 2023-08-04 13:44:41.000000 types-aiobotocore-mediastore-data-2.5.2.post2/types_aiobotocore_mediastore_data/type_defs.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)       65 2023-08-04 13:44:40.000000 types-aiobotocore-mediastore-data-2.5.2.post2/types_aiobotocore_mediastore_data/version.py
-drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:18.326643 types-aiobotocore-mediastore-data-2.5.2.post2/types_aiobotocore_mediastore_data.egg-info/
--rw-r--r--   0 vlad      (1000) vlad      (1000)    13308 2023-08-04 13:59:18.000000 types-aiobotocore-mediastore-data-2.5.2.post2/types_aiobotocore_mediastore_data.egg-info/PKG-INFO
--rw-r--r--   0 vlad      (1000) vlad      (1000)      965 2023-08-04 13:59:18.000000 types-aiobotocore-mediastore-data-2.5.2.post2/types_aiobotocore_mediastore_data.egg-info/SOURCES.txt
--rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:18.000000 types-aiobotocore-mediastore-data-2.5.2.post2/types_aiobotocore_mediastore_data.egg-info/dependency_links.txt
--rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:18.000000 types-aiobotocore-mediastore-data-2.5.2.post2/types_aiobotocore_mediastore_data.egg-info/not-zip-safe
--rw-r--r--   0 vlad      (1000) vlad      (1000)       52 2023-08-04 13:59:18.000000 types-aiobotocore-mediastore-data-2.5.2.post2/types_aiobotocore_mediastore_data.egg-info/requires.txt
--rw-r--r--   0 vlad      (1000) vlad      (1000)       34 2023-08-04 13:59:18.000000 types-aiobotocore-mediastore-data-2.5.2.post2/types_aiobotocore_mediastore_data.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:24:06.386735 types-aiobotocore-mediastore-data-2.5.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-08 01:15:20.000000 types-aiobotocore-mediastore-data-2.5.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    13302 2023-08-08 01:24:06.386735 types-aiobotocore-mediastore-data-2.5.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    11759 2023-08-08 01:15:20.000000 types-aiobotocore-mediastore-data-2.5.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-08 01:24:06.386735 types-aiobotocore-mediastore-data-2.5.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2121 2023-08-08 01:15:20.000000 types-aiobotocore-mediastore-data-2.5.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:24:06.386735 types-aiobotocore-mediastore-data-2.5.4/types_aiobotocore_mediastore_data/
+-rw-r--r--   0 runner    (1001) docker     (123)      676 2023-08-08 01:15:20.000000 types-aiobotocore-mediastore-data-2.5.4/types_aiobotocore_mediastore_data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      675 2023-08-08 01:15:20.000000 types-aiobotocore-mediastore-data-2.5.4/types_aiobotocore_mediastore_data/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      961 2023-08-08 01:15:20.000000 types-aiobotocore-mediastore-data-2.5.4/types_aiobotocore_mediastore_data/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7770 2023-08-08 01:15:20.000000 types-aiobotocore-mediastore-data-2.5.4/types_aiobotocore_mediastore_data/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7755 2023-08-08 01:15:20.000000 types-aiobotocore-mediastore-data-2.5.4/types_aiobotocore_mediastore_data/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8212 2023-08-08 01:15:20.000000 types-aiobotocore-mediastore-data-2.5.4/types_aiobotocore_mediastore_data/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8210 2023-08-08 01:15:20.000000 types-aiobotocore-mediastore-data-2.5.4/types_aiobotocore_mediastore_data/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2036 2023-08-08 01:15:20.000000 types-aiobotocore-mediastore-data-2.5.4/types_aiobotocore_mediastore_data/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2033 2023-08-08 01:15:20.000000 types-aiobotocore-mediastore-data-2.5.4/types_aiobotocore_mediastore_data/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 01:15:20.000000 types-aiobotocore-mediastore-data-2.5.4/types_aiobotocore_mediastore_data/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     4711 2023-08-08 01:15:20.000000 types-aiobotocore-mediastore-data-2.5.4/types_aiobotocore_mediastore_data/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4706 2023-08-08 01:15:20.000000 types-aiobotocore-mediastore-data-2.5.4/types_aiobotocore_mediastore_data/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-08-08 01:15:20.000000 types-aiobotocore-mediastore-data-2.5.4/types_aiobotocore_mediastore_data/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:24:06.386735 types-aiobotocore-mediastore-data-2.5.4/types_aiobotocore_mediastore_data.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    13302 2023-08-08 01:24:06.000000 types-aiobotocore-mediastore-data-2.5.4/types_aiobotocore_mediastore_data.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      965 2023-08-08 01:24:06.000000 types-aiobotocore-mediastore-data-2.5.4/types_aiobotocore_mediastore_data.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 01:24:06.000000 types-aiobotocore-mediastore-data-2.5.4/types_aiobotocore_mediastore_data.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 01:24:06.000000 types-aiobotocore-mediastore-data-2.5.4/types_aiobotocore_mediastore_data.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-08 01:24:06.000000 types-aiobotocore-mediastore-data-2.5.4/types_aiobotocore_mediastore_data.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-08-08 01:24:06.000000 types-aiobotocore-mediastore-data-2.5.4/types_aiobotocore_mediastore_data.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-mediastore-data-2.5.2.post2/LICENSE` & `types-aiobotocore-mediastore-data-2.5.4/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-mediastore-data-2.5.2.post2/PKG-INFO` & `types-aiobotocore-mediastore-data-2.5.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-mediastore-data
-Version: 2.5.2.post2
-Summary: Type annotations for aiobotocore.MediaStoreData 2.5.2 service generated with mypy-boto3-builder 7.17.2
+Version: 2.5.4
+Summary: Type annotations for aiobotocore.MediaStoreData 2.5.4 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mediastore_data/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-mediastore-data.svg?color=blue)](https://pypi.org/project/types-aiobotocore-mediastore-data)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mediastore_data/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-mediastore-data)](https://pepy.tech/project/types-aiobotocore-mediastore-data)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.MediaStoreData 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediastore-data.html#MediaStoreData)
+[aiobotocore.MediaStoreData 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediastore-data.html#MediaStoreData)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-mediastore-data-2.5.2.post2/README.md` & `types-aiobotocore-mediastore-data-2.5.4/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-mediastore-data.svg?color=blue)](https://pypi.org/project/types-aiobotocore-mediastore-data)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mediastore_data/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-mediastore-data)](https://pepy.tech/project/types-aiobotocore-mediastore-data)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.MediaStoreData 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediastore-data.html#MediaStoreData)
+[aiobotocore.MediaStoreData 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediastore-data.html#MediaStoreData)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-mediastore-data-2.5.2.post2/setup.py` & `types-aiobotocore-mediastore-data-2.5.4/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-mediastore-data",
-    version="2.5.2.post2",
+    version="2.5.4",
     packages=["types_aiobotocore_mediastore_data"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.MediaStoreData 2.5.2 service generated with"
+        "Type annotations for aiobotocore.MediaStoreData 2.5.4 service generated with"
         " mypy-boto3-builder 7.17.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
```

### Comparing `types-aiobotocore-mediastore-data-2.5.2.post2/types_aiobotocore_mediastore_data/__init__.py` & `types-aiobotocore-mediastore-data-2.5.4/types_aiobotocore_mediastore_data/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-mediastore-data-2.5.2.post2/types_aiobotocore_mediastore_data/__init__.pyi` & `types-aiobotocore-mediastore-data-2.5.4/types_aiobotocore_mediastore_data/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-mediastore-data-2.5.2.post2/types_aiobotocore_mediastore_data/__main__.py` & `types-aiobotocore-mediastore-data-2.5.4/types_aiobotocore_mediastore_data/__main__.py`

 * *Files 13% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.MediaStoreData 2.5.2\nVersion:        "
-        " 2.5.2.post2\nBuilder version: 7.17.2\nDocs:           "
+        "Type annotations for aiobotocore.MediaStoreData 2.5.4\nVersion:         2.5.4\nBuilder"
+        " version: 7.17.2\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mediastore_data//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediastore-data.html#MediaStoreData\nOther"
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

### Comparing `types-aiobotocore-mediastore-data-2.5.2.post2/types_aiobotocore_mediastore_data/client.py` & `types-aiobotocore-mediastore-data-2.5.4/types_aiobotocore_mediastore_data/client.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-mediastore-data-2.5.2.post2/types_aiobotocore_mediastore_data/client.pyi` & `types-aiobotocore-mediastore-data-2.5.4/types_aiobotocore_mediastore_data/client.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-mediastore-data-2.5.2.post2/types_aiobotocore_mediastore_data/literals.py` & `types-aiobotocore-mediastore-data-2.5.4/types_aiobotocore_mediastore_data/literals.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-mediastore-data-2.5.2.post2/types_aiobotocore_mediastore_data/literals.pyi` & `types-aiobotocore-mediastore-data-2.5.4/types_aiobotocore_mediastore_data/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-mediastore-data-2.5.2.post2/types_aiobotocore_mediastore_data/paginator.py` & `types-aiobotocore-mediastore-data-2.5.4/types_aiobotocore_mediastore_data/paginator.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-mediastore-data-2.5.2.post2/types_aiobotocore_mediastore_data/paginator.pyi` & `types-aiobotocore-mediastore-data-2.5.4/types_aiobotocore_mediastore_data/paginator.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-mediastore-data-2.5.2.post2/types_aiobotocore_mediastore_data/type_defs.py` & `types-aiobotocore-mediastore-data-2.5.4/types_aiobotocore_mediastore_data/type_defs.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-mediastore-data-2.5.2.post2/types_aiobotocore_mediastore_data/type_defs.pyi` & `types-aiobotocore-mediastore-data-2.5.4/types_aiobotocore_mediastore_data/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-mediastore-data-2.5.2.post2/types_aiobotocore_mediastore_data.egg-info/PKG-INFO` & `types-aiobotocore-mediastore-data-2.5.4/types_aiobotocore_mediastore_data.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-mediastore-data
-Version: 2.5.2.post2
-Summary: Type annotations for aiobotocore.MediaStoreData 2.5.2 service generated with mypy-boto3-builder 7.17.2
+Version: 2.5.4
+Summary: Type annotations for aiobotocore.MediaStoreData 2.5.4 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mediastore_data/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-mediastore-data.svg?color=blue)](https://pypi.org/project/types-aiobotocore-mediastore-data)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mediastore_data/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-mediastore-data)](https://pepy.tech/project/types-aiobotocore-mediastore-data)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.MediaStoreData 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediastore-data.html#MediaStoreData)
+[aiobotocore.MediaStoreData 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediastore-data.html#MediaStoreData)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-mediastore-data-2.5.2.post2/types_aiobotocore_mediastore_data.egg-info/SOURCES.txt` & `types-aiobotocore-mediastore-data-2.5.4/types_aiobotocore_mediastore_data.egg-info/SOURCES.txt`

 * *Files identical despite different names*


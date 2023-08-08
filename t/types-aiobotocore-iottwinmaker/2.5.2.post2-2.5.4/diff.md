# Comparing `tmp/types-aiobotocore-iottwinmaker-2.5.2.post2.tar.gz` & `tmp/types-aiobotocore-iottwinmaker-2.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-iottwinmaker-2.5.2.post2.tar", last modified: Fri Aug  4 13:59:13 2023, max compression
+gzip compressed data, was "types-aiobotocore-iottwinmaker-2.5.4.tar", last modified: Tue Aug  8 01:23:54 2023, max compression
```

## Comparing `types-aiobotocore-iottwinmaker-2.5.2.post2.tar` & `types-aiobotocore-iottwinmaker-2.5.4.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:13.106643 types-aiobotocore-iottwinmaker-2.5.2.post2/
--rw-r--r--   0 vlad      (1000) vlad      (1000)     1070 2023-08-04 13:41:22.000000 types-aiobotocore-iottwinmaker-2.5.2.post2/LICENSE
--rw-r--r--   0 vlad      (1000) vlad      (1000)    12449 2023-08-04 13:59:13.106643 types-aiobotocore-iottwinmaker-2.5.2.post2/PKG-INFO
--rw-r--r--   0 vlad      (1000) vlad      (1000)    10911 2023-08-04 13:41:22.000000 types-aiobotocore-iottwinmaker-2.5.2.post2/README.md
--rw-r--r--   0 vlad      (1000) vlad      (1000)       38 2023-08-04 13:59:13.106643 types-aiobotocore-iottwinmaker-2.5.2.post2/setup.cfg
--rw-r--r--   0 vlad      (1000) vlad      (1000)     2107 2023-08-04 13:41:22.000000 types-aiobotocore-iottwinmaker-2.5.2.post2/setup.py
-drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:13.106643 types-aiobotocore-iottwinmaker-2.5.2.post2/types_aiobotocore_iottwinmaker/
--rw-r--r--   0 vlad      (1000) vlad      (1000)      482 2023-08-04 13:41:22.000000 types-aiobotocore-iottwinmaker-2.5.2.post2/types_aiobotocore_iottwinmaker/__init__.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)      481 2023-08-04 13:41:22.000000 types-aiobotocore-iottwinmaker-2.5.2.post2/types_aiobotocore_iottwinmaker/__init__.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)      963 2023-08-04 13:41:22.000000 types-aiobotocore-iottwinmaker-2.5.2.post2/types_aiobotocore_iottwinmaker/__main__.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)    26590 2023-08-04 13:41:22.000000 types-aiobotocore-iottwinmaker-2.5.2.post2/types_aiobotocore_iottwinmaker/client.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)    26548 2023-08-04 13:41:22.000000 types-aiobotocore-iottwinmaker-2.5.2.post2/types_aiobotocore_iottwinmaker/client.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)     9664 2023-08-04 13:41:22.000000 types-aiobotocore-iottwinmaker-2.5.2.post2/types_aiobotocore_iottwinmaker/literals.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)     9662 2023-08-04 13:41:22.000000 types-aiobotocore-iottwinmaker-2.5.2.post2/types_aiobotocore_iottwinmaker/literals.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:41:22.000000 types-aiobotocore-iottwinmaker-2.5.2.post2/types_aiobotocore_iottwinmaker/py.typed
--rw-r--r--   0 vlad      (1000) vlad      (1000)    43547 2023-08-04 13:41:23.000000 types-aiobotocore-iottwinmaker-2.5.2.post2/types_aiobotocore_iottwinmaker/type_defs.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)    43474 2023-08-04 13:41:23.000000 types-aiobotocore-iottwinmaker-2.5.2.post2/types_aiobotocore_iottwinmaker/type_defs.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)       65 2023-08-04 13:41:22.000000 types-aiobotocore-iottwinmaker-2.5.2.post2/types_aiobotocore_iottwinmaker/version.py
-drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:13.106643 types-aiobotocore-iottwinmaker-2.5.2.post2/types_aiobotocore_iottwinmaker.egg-info/
--rw-r--r--   0 vlad      (1000) vlad      (1000)    12449 2023-08-04 13:59:13.000000 types-aiobotocore-iottwinmaker-2.5.2.post2/types_aiobotocore_iottwinmaker.egg-info/PKG-INFO
--rw-r--r--   0 vlad      (1000) vlad      (1000)      819 2023-08-04 13:59:13.000000 types-aiobotocore-iottwinmaker-2.5.2.post2/types_aiobotocore_iottwinmaker.egg-info/SOURCES.txt
--rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:13.000000 types-aiobotocore-iottwinmaker-2.5.2.post2/types_aiobotocore_iottwinmaker.egg-info/dependency_links.txt
--rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:13.000000 types-aiobotocore-iottwinmaker-2.5.2.post2/types_aiobotocore_iottwinmaker.egg-info/not-zip-safe
--rw-r--r--   0 vlad      (1000) vlad      (1000)       52 2023-08-04 13:59:13.000000 types-aiobotocore-iottwinmaker-2.5.2.post2/types_aiobotocore_iottwinmaker.egg-info/requires.txt
--rw-r--r--   0 vlad      (1000) vlad      (1000)       31 2023-08-04 13:59:13.000000 types-aiobotocore-iottwinmaker-2.5.2.post2/types_aiobotocore_iottwinmaker.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:23:54.810711 types-aiobotocore-iottwinmaker-2.5.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-08 01:13:11.000000 types-aiobotocore-iottwinmaker-2.5.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    12443 2023-08-08 01:23:54.806711 types-aiobotocore-iottwinmaker-2.5.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10911 2023-08-08 01:13:11.000000 types-aiobotocore-iottwinmaker-2.5.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-08 01:23:54.810711 types-aiobotocore-iottwinmaker-2.5.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2101 2023-08-08 01:13:10.000000 types-aiobotocore-iottwinmaker-2.5.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:23:54.802711 types-aiobotocore-iottwinmaker-2.5.4/types_aiobotocore_iottwinmaker/
+-rw-r--r--   0 runner    (1001) docker     (123)      482 2023-08-08 01:13:11.000000 types-aiobotocore-iottwinmaker-2.5.4/types_aiobotocore_iottwinmaker/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      481 2023-08-08 01:13:11.000000 types-aiobotocore-iottwinmaker-2.5.4/types_aiobotocore_iottwinmaker/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      951 2023-08-08 01:13:11.000000 types-aiobotocore-iottwinmaker-2.5.4/types_aiobotocore_iottwinmaker/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26590 2023-08-08 01:13:11.000000 types-aiobotocore-iottwinmaker-2.5.4/types_aiobotocore_iottwinmaker/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26548 2023-08-08 01:13:11.000000 types-aiobotocore-iottwinmaker-2.5.4/types_aiobotocore_iottwinmaker/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9664 2023-08-08 01:13:11.000000 types-aiobotocore-iottwinmaker-2.5.4/types_aiobotocore_iottwinmaker/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9662 2023-08-08 01:13:11.000000 types-aiobotocore-iottwinmaker-2.5.4/types_aiobotocore_iottwinmaker/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 01:13:11.000000 types-aiobotocore-iottwinmaker-2.5.4/types_aiobotocore_iottwinmaker/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    43547 2023-08-08 01:13:12.000000 types-aiobotocore-iottwinmaker-2.5.4/types_aiobotocore_iottwinmaker/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    43474 2023-08-08 01:13:11.000000 types-aiobotocore-iottwinmaker-2.5.4/types_aiobotocore_iottwinmaker/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-08-08 01:13:11.000000 types-aiobotocore-iottwinmaker-2.5.4/types_aiobotocore_iottwinmaker/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:23:54.806711 types-aiobotocore-iottwinmaker-2.5.4/types_aiobotocore_iottwinmaker.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    12443 2023-08-08 01:23:54.000000 types-aiobotocore-iottwinmaker-2.5.4/types_aiobotocore_iottwinmaker.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      819 2023-08-08 01:23:54.000000 types-aiobotocore-iottwinmaker-2.5.4/types_aiobotocore_iottwinmaker.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 01:23:54.000000 types-aiobotocore-iottwinmaker-2.5.4/types_aiobotocore_iottwinmaker.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 01:23:54.000000 types-aiobotocore-iottwinmaker-2.5.4/types_aiobotocore_iottwinmaker.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-08 01:23:54.000000 types-aiobotocore-iottwinmaker-2.5.4/types_aiobotocore_iottwinmaker.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-08-08 01:23:54.000000 types-aiobotocore-iottwinmaker-2.5.4/types_aiobotocore_iottwinmaker.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-iottwinmaker-2.5.2.post2/LICENSE` & `types-aiobotocore-iottwinmaker-2.5.4/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-iottwinmaker-2.5.2.post2/PKG-INFO` & `types-aiobotocore-iottwinmaker-2.5.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-iottwinmaker
-Version: 2.5.2.post2
-Summary: Type annotations for aiobotocore.IoTTwinMaker 2.5.2 service generated with mypy-boto3-builder 7.17.2
+Version: 2.5.4
+Summary: Type annotations for aiobotocore.IoTTwinMaker 2.5.4 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iottwinmaker/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-iottwinmaker.svg?color=blue)](https://pypi.org/project/types-aiobotocore-iottwinmaker)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iottwinmaker/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-iottwinmaker)](https://pepy.tech/project/types-aiobotocore-iottwinmaker)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.IoTTwinMaker 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iottwinmaker.html#IoTTwinMaker)
+[aiobotocore.IoTTwinMaker 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iottwinmaker.html#IoTTwinMaker)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-iottwinmaker-2.5.2.post2/README.md` & `types-aiobotocore-iottwinmaker-2.5.4/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-iottwinmaker.svg?color=blue)](https://pypi.org/project/types-aiobotocore-iottwinmaker)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iottwinmaker/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-iottwinmaker)](https://pepy.tech/project/types-aiobotocore-iottwinmaker)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.IoTTwinMaker 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iottwinmaker.html#IoTTwinMaker)
+[aiobotocore.IoTTwinMaker 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iottwinmaker.html#IoTTwinMaker)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-iottwinmaker-2.5.2.post2/setup.py` & `types-aiobotocore-iottwinmaker-2.5.4/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-iottwinmaker",
-    version="2.5.2.post2",
+    version="2.5.4",
     packages=["types_aiobotocore_iottwinmaker"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.IoTTwinMaker 2.5.2 service generated with"
+        "Type annotations for aiobotocore.IoTTwinMaker 2.5.4 service generated with"
         " mypy-boto3-builder 7.17.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
```

### Comparing `types-aiobotocore-iottwinmaker-2.5.2.post2/types_aiobotocore_iottwinmaker/__main__.py` & `types-aiobotocore-iottwinmaker-2.5.4/types_aiobotocore_iottwinmaker/__main__.py`

 * *Files 13% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.IoTTwinMaker 2.5.2\nVersion:         2.5.2.post2\nBuilder"
+        "Type annotations for aiobotocore.IoTTwinMaker 2.5.4\nVersion:         2.5.4\nBuilder"
         " version: 7.17.2\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iottwinmaker//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iottwinmaker.html#IoTTwinMaker\nOther"
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

### Comparing `types-aiobotocore-iottwinmaker-2.5.2.post2/types_aiobotocore_iottwinmaker/client.py` & `types-aiobotocore-iottwinmaker-2.5.4/types_aiobotocore_iottwinmaker/client.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-iottwinmaker-2.5.2.post2/types_aiobotocore_iottwinmaker/client.pyi` & `types-aiobotocore-iottwinmaker-2.5.4/types_aiobotocore_iottwinmaker/client.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-iottwinmaker-2.5.2.post2/types_aiobotocore_iottwinmaker/literals.py` & `types-aiobotocore-iottwinmaker-2.5.4/types_aiobotocore_iottwinmaker/literals.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-iottwinmaker-2.5.2.post2/types_aiobotocore_iottwinmaker/literals.pyi` & `types-aiobotocore-iottwinmaker-2.5.4/types_aiobotocore_iottwinmaker/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-iottwinmaker-2.5.2.post2/types_aiobotocore_iottwinmaker/type_defs.py` & `types-aiobotocore-iottwinmaker-2.5.4/types_aiobotocore_iottwinmaker/type_defs.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-iottwinmaker-2.5.2.post2/types_aiobotocore_iottwinmaker/type_defs.pyi` & `types-aiobotocore-iottwinmaker-2.5.4/types_aiobotocore_iottwinmaker/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-iottwinmaker-2.5.2.post2/types_aiobotocore_iottwinmaker.egg-info/PKG-INFO` & `types-aiobotocore-iottwinmaker-2.5.4/types_aiobotocore_iottwinmaker.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-iottwinmaker
-Version: 2.5.2.post2
-Summary: Type annotations for aiobotocore.IoTTwinMaker 2.5.2 service generated with mypy-boto3-builder 7.17.2
+Version: 2.5.4
+Summary: Type annotations for aiobotocore.IoTTwinMaker 2.5.4 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iottwinmaker/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-iottwinmaker.svg?color=blue)](https://pypi.org/project/types-aiobotocore-iottwinmaker)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iottwinmaker/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-iottwinmaker)](https://pepy.tech/project/types-aiobotocore-iottwinmaker)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.IoTTwinMaker 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iottwinmaker.html#IoTTwinMaker)
+[aiobotocore.IoTTwinMaker 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iottwinmaker.html#IoTTwinMaker)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-iottwinmaker-2.5.2.post2/types_aiobotocore_iottwinmaker.egg-info/SOURCES.txt` & `types-aiobotocore-iottwinmaker-2.5.4/types_aiobotocore_iottwinmaker.egg-info/SOURCES.txt`

 * *Files identical despite different names*


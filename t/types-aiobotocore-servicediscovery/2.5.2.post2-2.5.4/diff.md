# Comparing `tmp/types-aiobotocore-servicediscovery-2.5.2.post2.tar.gz` & `tmp/types-aiobotocore-servicediscovery-2.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-servicediscovery-2.5.2.post2.tar", last modified: Fri Aug  4 13:59:26 2023, max compression
+gzip compressed data, was "types-aiobotocore-servicediscovery-2.5.4.tar", last modified: Tue Aug  8 01:24:26 2023, max compression
```

## Comparing `types-aiobotocore-servicediscovery-2.5.2.post2.tar` & `types-aiobotocore-servicediscovery-2.5.4.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:26.506643 types-aiobotocore-servicediscovery-2.5.2.post2/
--rw-r--r--   0 vlad      (1000) vlad      (1000)     1070 2023-08-04 13:53:24.000000 types-aiobotocore-servicediscovery-2.5.2.post2/LICENSE
--rw-r--r--   0 vlad      (1000) vlad      (1000)    13791 2023-08-04 13:59:26.506643 types-aiobotocore-servicediscovery-2.5.2.post2/PKG-INFO
--rw-r--r--   0 vlad      (1000) vlad      (1000)    12237 2023-08-04 13:53:24.000000 types-aiobotocore-servicediscovery-2.5.2.post2/README.md
--rw-r--r--   0 vlad      (1000) vlad      (1000)       38 2023-08-04 13:59:26.506643 types-aiobotocore-servicediscovery-2.5.2.post2/setup.cfg
--rw-r--r--   0 vlad      (1000) vlad      (1000)     2135 2023-08-04 13:53:24.000000 types-aiobotocore-servicediscovery-2.5.2.post2/setup.py
-drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:26.506643 types-aiobotocore-servicediscovery-2.5.2.post2/types_aiobotocore_servicediscovery/
--rw-r--r--   0 vlad      (1000) vlad      (1000)     1295 2023-08-04 13:53:24.000000 types-aiobotocore-servicediscovery-2.5.2.post2/types_aiobotocore_servicediscovery/__init__.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)     1294 2023-08-04 13:53:24.000000 types-aiobotocore-servicediscovery-2.5.2.post2/types_aiobotocore_servicediscovery/__init__.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)      979 2023-08-04 13:53:24.000000 types-aiobotocore-servicediscovery-2.5.2.post2/types_aiobotocore_servicediscovery/__main__.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)    24549 2023-08-04 13:53:25.000000 types-aiobotocore-servicediscovery-2.5.2.post2/types_aiobotocore_servicediscovery/client.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)    24510 2023-08-04 13:53:24.000000 types-aiobotocore-servicediscovery-2.5.2.post2/types_aiobotocore_servicediscovery/client.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)    10287 2023-08-04 13:53:28.000000 types-aiobotocore-servicediscovery-2.5.2.post2/types_aiobotocore_servicediscovery/literals.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)    10285 2023-08-04 13:53:28.000000 types-aiobotocore-servicediscovery-2.5.2.post2/types_aiobotocore_servicediscovery/literals.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)     5740 2023-08-04 13:53:28.000000 types-aiobotocore-servicediscovery-2.5.2.post2/types_aiobotocore_servicediscovery/paginator.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)     5734 2023-08-04 13:53:28.000000 types-aiobotocore-servicediscovery-2.5.2.post2/types_aiobotocore_servicediscovery/paginator.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:53:24.000000 types-aiobotocore-servicediscovery-2.5.2.post2/types_aiobotocore_servicediscovery/py.typed
--rw-r--r--   0 vlad      (1000) vlad      (1000)    28436 2023-08-04 13:53:29.000000 types-aiobotocore-servicediscovery-2.5.2.post2/types_aiobotocore_servicediscovery/type_defs.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)    28400 2023-08-04 13:53:29.000000 types-aiobotocore-servicediscovery-2.5.2.post2/types_aiobotocore_servicediscovery/type_defs.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)       65 2023-08-04 13:53:24.000000 types-aiobotocore-servicediscovery-2.5.2.post2/types_aiobotocore_servicediscovery/version.py
-drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:26.506643 types-aiobotocore-servicediscovery-2.5.2.post2/types_aiobotocore_servicediscovery.egg-info/
--rw-r--r--   0 vlad      (1000) vlad      (1000)    13791 2023-08-04 13:59:26.000000 types-aiobotocore-servicediscovery-2.5.2.post2/types_aiobotocore_servicediscovery.egg-info/PKG-INFO
--rw-r--r--   0 vlad      (1000) vlad      (1000)      984 2023-08-04 13:59:26.000000 types-aiobotocore-servicediscovery-2.5.2.post2/types_aiobotocore_servicediscovery.egg-info/SOURCES.txt
--rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:26.000000 types-aiobotocore-servicediscovery-2.5.2.post2/types_aiobotocore_servicediscovery.egg-info/dependency_links.txt
--rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:26.000000 types-aiobotocore-servicediscovery-2.5.2.post2/types_aiobotocore_servicediscovery.egg-info/not-zip-safe
--rw-r--r--   0 vlad      (1000) vlad      (1000)       52 2023-08-04 13:59:26.000000 types-aiobotocore-servicediscovery-2.5.2.post2/types_aiobotocore_servicediscovery.egg-info/requires.txt
--rw-r--r--   0 vlad      (1000) vlad      (1000)       35 2023-08-04 13:59:26.000000 types-aiobotocore-servicediscovery-2.5.2.post2/types_aiobotocore_servicediscovery.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:24:26.842782 types-aiobotocore-servicediscovery-2.5.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-08 01:21:04.000000 types-aiobotocore-servicediscovery-2.5.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    13785 2023-08-08 01:24:26.842782 types-aiobotocore-servicediscovery-2.5.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    12237 2023-08-08 01:21:04.000000 types-aiobotocore-servicediscovery-2.5.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-08 01:24:26.842782 types-aiobotocore-servicediscovery-2.5.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2129 2023-08-08 01:21:04.000000 types-aiobotocore-servicediscovery-2.5.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:24:26.842782 types-aiobotocore-servicediscovery-2.5.4/types_aiobotocore_servicediscovery/
+-rw-r--r--   0 runner    (1001) docker     (123)     1295 2023-08-08 01:21:04.000000 types-aiobotocore-servicediscovery-2.5.4/types_aiobotocore_servicediscovery/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1294 2023-08-08 01:21:04.000000 types-aiobotocore-servicediscovery-2.5.4/types_aiobotocore_servicediscovery/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      967 2023-08-08 01:21:04.000000 types-aiobotocore-servicediscovery-2.5.4/types_aiobotocore_servicediscovery/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24549 2023-08-08 01:21:04.000000 types-aiobotocore-servicediscovery-2.5.4/types_aiobotocore_servicediscovery/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24510 2023-08-08 01:21:04.000000 types-aiobotocore-servicediscovery-2.5.4/types_aiobotocore_servicediscovery/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    10287 2023-08-08 01:21:04.000000 types-aiobotocore-servicediscovery-2.5.4/types_aiobotocore_servicediscovery/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10285 2023-08-08 01:21:04.000000 types-aiobotocore-servicediscovery-2.5.4/types_aiobotocore_servicediscovery/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     5740 2023-08-08 01:21:04.000000 types-aiobotocore-servicediscovery-2.5.4/types_aiobotocore_servicediscovery/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5734 2023-08-08 01:21:04.000000 types-aiobotocore-servicediscovery-2.5.4/types_aiobotocore_servicediscovery/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 01:21:04.000000 types-aiobotocore-servicediscovery-2.5.4/types_aiobotocore_servicediscovery/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    28436 2023-08-08 01:21:05.000000 types-aiobotocore-servicediscovery-2.5.4/types_aiobotocore_servicediscovery/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28400 2023-08-08 01:21:04.000000 types-aiobotocore-servicediscovery-2.5.4/types_aiobotocore_servicediscovery/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-08-08 01:21:04.000000 types-aiobotocore-servicediscovery-2.5.4/types_aiobotocore_servicediscovery/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:24:26.842782 types-aiobotocore-servicediscovery-2.5.4/types_aiobotocore_servicediscovery.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    13785 2023-08-08 01:24:26.000000 types-aiobotocore-servicediscovery-2.5.4/types_aiobotocore_servicediscovery.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      984 2023-08-08 01:24:26.000000 types-aiobotocore-servicediscovery-2.5.4/types_aiobotocore_servicediscovery.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 01:24:26.000000 types-aiobotocore-servicediscovery-2.5.4/types_aiobotocore_servicediscovery.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 01:24:26.000000 types-aiobotocore-servicediscovery-2.5.4/types_aiobotocore_servicediscovery.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-08 01:24:26.000000 types-aiobotocore-servicediscovery-2.5.4/types_aiobotocore_servicediscovery.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-08-08 01:24:26.000000 types-aiobotocore-servicediscovery-2.5.4/types_aiobotocore_servicediscovery.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-servicediscovery-2.5.2.post2/LICENSE` & `types-aiobotocore-servicediscovery-2.5.4/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-servicediscovery-2.5.2.post2/PKG-INFO` & `types-aiobotocore-servicediscovery-2.5.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-servicediscovery
-Version: 2.5.2.post2
-Summary: Type annotations for aiobotocore.ServiceDiscovery 2.5.2 service generated with mypy-boto3-builder 7.17.2
+Version: 2.5.4
+Summary: Type annotations for aiobotocore.ServiceDiscovery 2.5.4 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_servicediscovery/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-servicediscovery.svg?color=blue)](https://pypi.org/project/types-aiobotocore-servicediscovery)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_servicediscovery/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-servicediscovery)](https://pepy.tech/project/types-aiobotocore-servicediscovery)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.ServiceDiscovery 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/servicediscovery.html#ServiceDiscovery)
+[aiobotocore.ServiceDiscovery 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/servicediscovery.html#ServiceDiscovery)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-servicediscovery-2.5.2.post2/README.md` & `types-aiobotocore-servicediscovery-2.5.4/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-servicediscovery.svg?color=blue)](https://pypi.org/project/types-aiobotocore-servicediscovery)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_servicediscovery/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-servicediscovery)](https://pepy.tech/project/types-aiobotocore-servicediscovery)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.ServiceDiscovery 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/servicediscovery.html#ServiceDiscovery)
+[aiobotocore.ServiceDiscovery 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/servicediscovery.html#ServiceDiscovery)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-servicediscovery-2.5.2.post2/setup.py` & `types-aiobotocore-servicediscovery-2.5.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-servicediscovery",
-    version="2.5.2.post2",
+    version="2.5.4",
     packages=["types_aiobotocore_servicediscovery"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.ServiceDiscovery 2.5.2 service generated with"
+        "Type annotations for aiobotocore.ServiceDiscovery 2.5.4 service generated with"
         " mypy-boto3-builder 7.17.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
```

### Comparing `types-aiobotocore-servicediscovery-2.5.2.post2/types_aiobotocore_servicediscovery/__init__.py` & `types-aiobotocore-servicediscovery-2.5.4/types_aiobotocore_servicediscovery/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-servicediscovery-2.5.2.post2/types_aiobotocore_servicediscovery/__init__.pyi` & `types-aiobotocore-servicediscovery-2.5.4/types_aiobotocore_servicediscovery/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-servicediscovery-2.5.2.post2/types_aiobotocore_servicediscovery/__main__.py` & `types-aiobotocore-servicediscovery-2.5.4/types_aiobotocore_servicediscovery/__main__.py`

 * *Files 20% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.ServiceDiscovery 2.5.2\nVersion:        "
-        " 2.5.2.post2\nBuilder version: 7.17.2\nDocs:           "
+        "Type annotations for aiobotocore.ServiceDiscovery 2.5.4\nVersion:         2.5.4\nBuilder"
+        " version: 7.17.2\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_servicediscovery//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/servicediscovery.html#ServiceDiscovery\nOther"
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

### Comparing `types-aiobotocore-servicediscovery-2.5.2.post2/types_aiobotocore_servicediscovery/client.py` & `types-aiobotocore-servicediscovery-2.5.4/types_aiobotocore_servicediscovery/client.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-servicediscovery-2.5.2.post2/types_aiobotocore_servicediscovery/client.pyi` & `types-aiobotocore-servicediscovery-2.5.4/types_aiobotocore_servicediscovery/client.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-servicediscovery-2.5.2.post2/types_aiobotocore_servicediscovery/literals.py` & `types-aiobotocore-servicediscovery-2.5.4/types_aiobotocore_servicediscovery/literals.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-servicediscovery-2.5.2.post2/types_aiobotocore_servicediscovery/literals.pyi` & `types-aiobotocore-servicediscovery-2.5.4/types_aiobotocore_servicediscovery/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-servicediscovery-2.5.2.post2/types_aiobotocore_servicediscovery/paginator.py` & `types-aiobotocore-servicediscovery-2.5.4/types_aiobotocore_servicediscovery/paginator.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-servicediscovery-2.5.2.post2/types_aiobotocore_servicediscovery/paginator.pyi` & `types-aiobotocore-servicediscovery-2.5.4/types_aiobotocore_servicediscovery/paginator.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-servicediscovery-2.5.2.post2/types_aiobotocore_servicediscovery/type_defs.py` & `types-aiobotocore-servicediscovery-2.5.4/types_aiobotocore_servicediscovery/type_defs.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-servicediscovery-2.5.2.post2/types_aiobotocore_servicediscovery/type_defs.pyi` & `types-aiobotocore-servicediscovery-2.5.4/types_aiobotocore_servicediscovery/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-servicediscovery-2.5.2.post2/types_aiobotocore_servicediscovery.egg-info/PKG-INFO` & `types-aiobotocore-servicediscovery-2.5.4/types_aiobotocore_servicediscovery.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-servicediscovery
-Version: 2.5.2.post2
-Summary: Type annotations for aiobotocore.ServiceDiscovery 2.5.2 service generated with mypy-boto3-builder 7.17.2
+Version: 2.5.4
+Summary: Type annotations for aiobotocore.ServiceDiscovery 2.5.4 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_servicediscovery/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-servicediscovery.svg?color=blue)](https://pypi.org/project/types-aiobotocore-servicediscovery)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_servicediscovery/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-servicediscovery)](https://pepy.tech/project/types-aiobotocore-servicediscovery)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.ServiceDiscovery 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/servicediscovery.html#ServiceDiscovery)
+[aiobotocore.ServiceDiscovery 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/servicediscovery.html#ServiceDiscovery)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-servicediscovery-2.5.2.post2/types_aiobotocore_servicediscovery.egg-info/SOURCES.txt` & `types-aiobotocore-servicediscovery-2.5.4/types_aiobotocore_servicediscovery.egg-info/SOURCES.txt`

 * *Files identical despite different names*


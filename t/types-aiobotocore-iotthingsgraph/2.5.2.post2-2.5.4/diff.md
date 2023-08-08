# Comparing `tmp/types-aiobotocore-iotthingsgraph-2.5.2.post2.tar.gz` & `tmp/types-aiobotocore-iotthingsgraph-2.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-iotthingsgraph-2.5.2.post2.tar", last modified: Fri Aug  4 13:59:13 2023, max compression
+gzip compressed data, was "types-aiobotocore-iotthingsgraph-2.5.4.tar", last modified: Tue Aug  8 01:23:54 2023, max compression
```

## Comparing `types-aiobotocore-iotthingsgraph-2.5.2.post2.tar` & `types-aiobotocore-iotthingsgraph-2.5.4.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:13.116643 types-aiobotocore-iotthingsgraph-2.5.2.post2/
--rw-r--r--   0 vlad      (1000) vlad      (1000)     1070 2023-08-04 13:41:18.000000 types-aiobotocore-iotthingsgraph-2.5.2.post2/LICENSE
--rw-r--r--   0 vlad      (1000) vlad      (1000)    14891 2023-08-04 13:59:13.116643 types-aiobotocore-iotthingsgraph-2.5.2.post2/PKG-INFO
--rw-r--r--   0 vlad      (1000) vlad      (1000)    13345 2023-08-04 13:41:18.000000 types-aiobotocore-iotthingsgraph-2.5.2.post2/README.md
--rw-r--r--   0 vlad      (1000) vlad      (1000)       38 2023-08-04 13:59:13.116643 types-aiobotocore-iotthingsgraph-2.5.2.post2/setup.cfg
--rw-r--r--   0 vlad      (1000) vlad      (1000)     2121 2023-08-04 13:41:18.000000 types-aiobotocore-iotthingsgraph-2.5.2.post2/setup.py
-drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:13.116643 types-aiobotocore-iotthingsgraph-2.5.2.post2/types_aiobotocore_iotthingsgraph/
--rw-r--r--   0 vlad      (1000) vlad      (1000)     2827 2023-08-04 13:41:18.000000 types-aiobotocore-iotthingsgraph-2.5.2.post2/types_aiobotocore_iotthingsgraph/__init__.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)     2826 2023-08-04 13:41:18.000000 types-aiobotocore-iotthingsgraph-2.5.2.post2/types_aiobotocore_iotthingsgraph/__init__.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)      971 2023-08-04 13:41:18.000000 types-aiobotocore-iotthingsgraph-2.5.2.post2/types_aiobotocore_iotthingsgraph/__main__.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)    31302 2023-08-04 13:41:19.000000 types-aiobotocore-iotthingsgraph-2.5.2.post2/types_aiobotocore_iotthingsgraph/client.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)    31248 2023-08-04 13:41:18.000000 types-aiobotocore-iotthingsgraph-2.5.2.post2/types_aiobotocore_iotthingsgraph/client.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)    11290 2023-08-04 13:41:19.000000 types-aiobotocore-iotthingsgraph-2.5.2.post2/types_aiobotocore_iotthingsgraph/literals.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)    11288 2023-08-04 13:41:19.000000 types-aiobotocore-iotthingsgraph-2.5.2.post2/types_aiobotocore_iotthingsgraph/literals.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)    13623 2023-08-04 13:41:19.000000 types-aiobotocore-iotthingsgraph-2.5.2.post2/types_aiobotocore_iotthingsgraph/paginator.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)    13611 2023-08-04 13:41:19.000000 types-aiobotocore-iotthingsgraph-2.5.2.post2/types_aiobotocore_iotthingsgraph/paginator.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:41:18.000000 types-aiobotocore-iotthingsgraph-2.5.2.post2/types_aiobotocore_iotthingsgraph/py.typed
--rw-r--r--   0 vlad      (1000) vlad      (1000)    33751 2023-08-04 13:41:20.000000 types-aiobotocore-iotthingsgraph-2.5.2.post2/types_aiobotocore_iotthingsgraph/type_defs.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)    33704 2023-08-04 13:41:19.000000 types-aiobotocore-iotthingsgraph-2.5.2.post2/types_aiobotocore_iotthingsgraph/type_defs.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)       65 2023-08-04 13:41:18.000000 types-aiobotocore-iotthingsgraph-2.5.2.post2/types_aiobotocore_iotthingsgraph/version.py
-drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:13.116643 types-aiobotocore-iotthingsgraph-2.5.2.post2/types_aiobotocore_iotthingsgraph.egg-info/
--rw-r--r--   0 vlad      (1000) vlad      (1000)    14891 2023-08-04 13:59:13.000000 types-aiobotocore-iotthingsgraph-2.5.2.post2/types_aiobotocore_iotthingsgraph.egg-info/PKG-INFO
--rw-r--r--   0 vlad      (1000) vlad      (1000)      946 2023-08-04 13:59:13.000000 types-aiobotocore-iotthingsgraph-2.5.2.post2/types_aiobotocore_iotthingsgraph.egg-info/SOURCES.txt
--rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:13.000000 types-aiobotocore-iotthingsgraph-2.5.2.post2/types_aiobotocore_iotthingsgraph.egg-info/dependency_links.txt
--rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:13.000000 types-aiobotocore-iotthingsgraph-2.5.2.post2/types_aiobotocore_iotthingsgraph.egg-info/not-zip-safe
--rw-r--r--   0 vlad      (1000) vlad      (1000)       52 2023-08-04 13:59:13.000000 types-aiobotocore-iotthingsgraph-2.5.2.post2/types_aiobotocore_iotthingsgraph.egg-info/requires.txt
--rw-r--r--   0 vlad      (1000) vlad      (1000)       33 2023-08-04 13:59:13.000000 types-aiobotocore-iotthingsgraph-2.5.2.post2/types_aiobotocore_iotthingsgraph.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:23:54.714711 types-aiobotocore-iotthingsgraph-2.5.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-08 01:13:07.000000 types-aiobotocore-iotthingsgraph-2.5.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    14885 2023-08-08 01:23:54.702711 types-aiobotocore-iotthingsgraph-2.5.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    13345 2023-08-08 01:13:07.000000 types-aiobotocore-iotthingsgraph-2.5.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-08 01:23:54.714711 types-aiobotocore-iotthingsgraph-2.5.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2115 2023-08-08 01:13:07.000000 types-aiobotocore-iotthingsgraph-2.5.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:23:54.702711 types-aiobotocore-iotthingsgraph-2.5.4/types_aiobotocore_iotthingsgraph/
+-rw-r--r--   0 runner    (1001) docker     (123)     2827 2023-08-08 01:13:08.000000 types-aiobotocore-iotthingsgraph-2.5.4/types_aiobotocore_iotthingsgraph/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2826 2023-08-08 01:13:08.000000 types-aiobotocore-iotthingsgraph-2.5.4/types_aiobotocore_iotthingsgraph/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      959 2023-08-08 01:13:08.000000 types-aiobotocore-iotthingsgraph-2.5.4/types_aiobotocore_iotthingsgraph/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31302 2023-08-08 01:13:08.000000 types-aiobotocore-iotthingsgraph-2.5.4/types_aiobotocore_iotthingsgraph/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31248 2023-08-08 01:13:08.000000 types-aiobotocore-iotthingsgraph-2.5.4/types_aiobotocore_iotthingsgraph/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    11290 2023-08-08 01:13:09.000000 types-aiobotocore-iotthingsgraph-2.5.4/types_aiobotocore_iotthingsgraph/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11288 2023-08-08 01:13:09.000000 types-aiobotocore-iotthingsgraph-2.5.4/types_aiobotocore_iotthingsgraph/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    13623 2023-08-08 01:13:08.000000 types-aiobotocore-iotthingsgraph-2.5.4/types_aiobotocore_iotthingsgraph/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13611 2023-08-08 01:13:08.000000 types-aiobotocore-iotthingsgraph-2.5.4/types_aiobotocore_iotthingsgraph/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 01:13:08.000000 types-aiobotocore-iotthingsgraph-2.5.4/types_aiobotocore_iotthingsgraph/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    33751 2023-08-08 01:13:10.000000 types-aiobotocore-iotthingsgraph-2.5.4/types_aiobotocore_iotthingsgraph/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33704 2023-08-08 01:13:10.000000 types-aiobotocore-iotthingsgraph-2.5.4/types_aiobotocore_iotthingsgraph/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-08-08 01:13:07.000000 types-aiobotocore-iotthingsgraph-2.5.4/types_aiobotocore_iotthingsgraph/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:23:54.702711 types-aiobotocore-iotthingsgraph-2.5.4/types_aiobotocore_iotthingsgraph.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    14885 2023-08-08 01:23:54.000000 types-aiobotocore-iotthingsgraph-2.5.4/types_aiobotocore_iotthingsgraph.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      946 2023-08-08 01:23:54.000000 types-aiobotocore-iotthingsgraph-2.5.4/types_aiobotocore_iotthingsgraph.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 01:23:54.000000 types-aiobotocore-iotthingsgraph-2.5.4/types_aiobotocore_iotthingsgraph.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 01:23:54.000000 types-aiobotocore-iotthingsgraph-2.5.4/types_aiobotocore_iotthingsgraph.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-08 01:23:54.000000 types-aiobotocore-iotthingsgraph-2.5.4/types_aiobotocore_iotthingsgraph.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-08-08 01:23:54.000000 types-aiobotocore-iotthingsgraph-2.5.4/types_aiobotocore_iotthingsgraph.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-iotthingsgraph-2.5.2.post2/LICENSE` & `types-aiobotocore-iotthingsgraph-2.5.4/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-iotthingsgraph-2.5.2.post2/PKG-INFO` & `types-aiobotocore-iotthingsgraph-2.5.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-iotthingsgraph
-Version: 2.5.2.post2
-Summary: Type annotations for aiobotocore.IoTThingsGraph 2.5.2 service generated with mypy-boto3-builder 7.17.2
+Version: 2.5.4
+Summary: Type annotations for aiobotocore.IoTThingsGraph 2.5.4 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotthingsgraph/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-iotthingsgraph.svg?color=blue)](https://pypi.org/project/types-aiobotocore-iotthingsgraph)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotthingsgraph/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-iotthingsgraph)](https://pepy.tech/project/types-aiobotocore-iotthingsgraph)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.IoTThingsGraph 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotthingsgraph.html#IoTThingsGraph)
+[aiobotocore.IoTThingsGraph 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotthingsgraph.html#IoTThingsGraph)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-iotthingsgraph-2.5.2.post2/README.md` & `types-aiobotocore-iotthingsgraph-2.5.4/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-iotthingsgraph.svg?color=blue)](https://pypi.org/project/types-aiobotocore-iotthingsgraph)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotthingsgraph/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-iotthingsgraph)](https://pepy.tech/project/types-aiobotocore-iotthingsgraph)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.IoTThingsGraph 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotthingsgraph.html#IoTThingsGraph)
+[aiobotocore.IoTThingsGraph 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotthingsgraph.html#IoTThingsGraph)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-iotthingsgraph-2.5.2.post2/setup.py` & `types-aiobotocore-iotthingsgraph-2.5.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-iotthingsgraph",
-    version="2.5.2.post2",
+    version="2.5.4",
     packages=["types_aiobotocore_iotthingsgraph"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.IoTThingsGraph 2.5.2 service generated with"
+        "Type annotations for aiobotocore.IoTThingsGraph 2.5.4 service generated with"
         " mypy-boto3-builder 7.17.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
```

### Comparing `types-aiobotocore-iotthingsgraph-2.5.2.post2/types_aiobotocore_iotthingsgraph/__init__.py` & `types-aiobotocore-iotthingsgraph-2.5.4/types_aiobotocore_iotthingsgraph/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-iotthingsgraph-2.5.2.post2/types_aiobotocore_iotthingsgraph/__init__.pyi` & `types-aiobotocore-iotthingsgraph-2.5.4/types_aiobotocore_iotthingsgraph/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-iotthingsgraph-2.5.2.post2/types_aiobotocore_iotthingsgraph/client.py` & `types-aiobotocore-iotthingsgraph-2.5.4/types_aiobotocore_iotthingsgraph/client.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-iotthingsgraph-2.5.2.post2/types_aiobotocore_iotthingsgraph/client.pyi` & `types-aiobotocore-iotthingsgraph-2.5.4/types_aiobotocore_iotthingsgraph/client.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-iotthingsgraph-2.5.2.post2/types_aiobotocore_iotthingsgraph/literals.py` & `types-aiobotocore-iotthingsgraph-2.5.4/types_aiobotocore_iotthingsgraph/literals.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-iotthingsgraph-2.5.2.post2/types_aiobotocore_iotthingsgraph/literals.pyi` & `types-aiobotocore-iotthingsgraph-2.5.4/types_aiobotocore_iotthingsgraph/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-iotthingsgraph-2.5.2.post2/types_aiobotocore_iotthingsgraph/paginator.py` & `types-aiobotocore-iotthingsgraph-2.5.4/types_aiobotocore_iotthingsgraph/paginator.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-iotthingsgraph-2.5.2.post2/types_aiobotocore_iotthingsgraph/paginator.pyi` & `types-aiobotocore-iotthingsgraph-2.5.4/types_aiobotocore_iotthingsgraph/paginator.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-iotthingsgraph-2.5.2.post2/types_aiobotocore_iotthingsgraph/type_defs.py` & `types-aiobotocore-iotthingsgraph-2.5.4/types_aiobotocore_iotthingsgraph/type_defs.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-iotthingsgraph-2.5.2.post2/types_aiobotocore_iotthingsgraph/type_defs.pyi` & `types-aiobotocore-iotthingsgraph-2.5.4/types_aiobotocore_iotthingsgraph/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-iotthingsgraph-2.5.2.post2/types_aiobotocore_iotthingsgraph.egg-info/PKG-INFO` & `types-aiobotocore-iotthingsgraph-2.5.4/types_aiobotocore_iotthingsgraph.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-iotthingsgraph
-Version: 2.5.2.post2
-Summary: Type annotations for aiobotocore.IoTThingsGraph 2.5.2 service generated with mypy-boto3-builder 7.17.2
+Version: 2.5.4
+Summary: Type annotations for aiobotocore.IoTThingsGraph 2.5.4 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotthingsgraph/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-iotthingsgraph.svg?color=blue)](https://pypi.org/project/types-aiobotocore-iotthingsgraph)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotthingsgraph/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-iotthingsgraph)](https://pepy.tech/project/types-aiobotocore-iotthingsgraph)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.IoTThingsGraph 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotthingsgraph.html#IoTThingsGraph)
+[aiobotocore.IoTThingsGraph 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotthingsgraph.html#IoTThingsGraph)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-iotthingsgraph-2.5.2.post2/types_aiobotocore_iotthingsgraph.egg-info/SOURCES.txt` & `types-aiobotocore-iotthingsgraph-2.5.4/types_aiobotocore_iotthingsgraph.egg-info/SOURCES.txt`

 * *Files identical despite different names*


# Comparing `tmp/types-aiobotocore-iotdeviceadvisor-2.5.2.post2.tar.gz` & `tmp/types-aiobotocore-iotdeviceadvisor-2.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-iotdeviceadvisor-2.5.2.post2.tar", last modified: Fri Aug  4 13:59:12 2023, max compression
+gzip compressed data, was "types-aiobotocore-iotdeviceadvisor-2.5.4.tar", last modified: Tue Aug  8 01:23:52 2023, max compression
```

## Comparing `types-aiobotocore-iotdeviceadvisor-2.5.2.post2.tar` & `types-aiobotocore-iotdeviceadvisor-2.5.4.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:12.256642 types-aiobotocore-iotdeviceadvisor-2.5.2.post2/
--rw-r--r--   0 vlad      (1000) vlad      (1000)     1070 2023-08-04 13:40:56.000000 types-aiobotocore-iotdeviceadvisor-2.5.2.post2/LICENSE
--rw-r--r--   0 vlad      (1000) vlad      (1000)    12681 2023-08-04 13:59:12.256642 types-aiobotocore-iotdeviceadvisor-2.5.2.post2/PKG-INFO
--rw-r--r--   0 vlad      (1000) vlad      (1000)    11127 2023-08-04 13:40:56.000000 types-aiobotocore-iotdeviceadvisor-2.5.2.post2/README.md
--rw-r--r--   0 vlad      (1000) vlad      (1000)       38 2023-08-04 13:59:12.256642 types-aiobotocore-iotdeviceadvisor-2.5.2.post2/setup.cfg
--rw-r--r--   0 vlad      (1000) vlad      (1000)     2135 2023-08-04 13:40:56.000000 types-aiobotocore-iotdeviceadvisor-2.5.2.post2/setup.py
-drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:12.256642 types-aiobotocore-iotdeviceadvisor-2.5.2.post2/types_aiobotocore_iotdeviceadvisor/
--rw-r--r--   0 vlad      (1000) vlad      (1000)      514 2023-08-04 13:40:56.000000 types-aiobotocore-iotdeviceadvisor-2.5.2.post2/types_aiobotocore_iotdeviceadvisor/__init__.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)      513 2023-08-04 13:40:56.000000 types-aiobotocore-iotdeviceadvisor-2.5.2.post2/types_aiobotocore_iotdeviceadvisor/__init__.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)      979 2023-08-04 13:40:56.000000 types-aiobotocore-iotdeviceadvisor-2.5.2.post2/types_aiobotocore_iotdeviceadvisor/__main__.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)    12963 2023-08-04 13:40:56.000000 types-aiobotocore-iotdeviceadvisor-2.5.2.post2/types_aiobotocore_iotdeviceadvisor/client.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)    12941 2023-08-04 13:40:56.000000 types-aiobotocore-iotdeviceadvisor-2.5.2.post2/types_aiobotocore_iotdeviceadvisor/client.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)     8701 2023-08-04 13:40:57.000000 types-aiobotocore-iotdeviceadvisor-2.5.2.post2/types_aiobotocore_iotdeviceadvisor/literals.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)     8699 2023-08-04 13:40:57.000000 types-aiobotocore-iotdeviceadvisor-2.5.2.post2/types_aiobotocore_iotdeviceadvisor/literals.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:40:56.000000 types-aiobotocore-iotdeviceadvisor-2.5.2.post2/types_aiobotocore_iotdeviceadvisor/py.typed
--rw-r--r--   0 vlad      (1000) vlad      (1000)    12286 2023-08-04 13:40:57.000000 types-aiobotocore-iotdeviceadvisor-2.5.2.post2/types_aiobotocore_iotdeviceadvisor/type_defs.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)    12275 2023-08-04 13:40:57.000000 types-aiobotocore-iotdeviceadvisor-2.5.2.post2/types_aiobotocore_iotdeviceadvisor/type_defs.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)       65 2023-08-04 13:40:56.000000 types-aiobotocore-iotdeviceadvisor-2.5.2.post2/types_aiobotocore_iotdeviceadvisor/version.py
-drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:12.256642 types-aiobotocore-iotdeviceadvisor-2.5.2.post2/types_aiobotocore_iotdeviceadvisor.egg-info/
--rw-r--r--   0 vlad      (1000) vlad      (1000)    12681 2023-08-04 13:59:12.000000 types-aiobotocore-iotdeviceadvisor-2.5.2.post2/types_aiobotocore_iotdeviceadvisor.egg-info/PKG-INFO
--rw-r--r--   0 vlad      (1000) vlad      (1000)      887 2023-08-04 13:59:12.000000 types-aiobotocore-iotdeviceadvisor-2.5.2.post2/types_aiobotocore_iotdeviceadvisor.egg-info/SOURCES.txt
--rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:12.000000 types-aiobotocore-iotdeviceadvisor-2.5.2.post2/types_aiobotocore_iotdeviceadvisor.egg-info/dependency_links.txt
--rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:12.000000 types-aiobotocore-iotdeviceadvisor-2.5.2.post2/types_aiobotocore_iotdeviceadvisor.egg-info/not-zip-safe
--rw-r--r--   0 vlad      (1000) vlad      (1000)       52 2023-08-04 13:59:12.000000 types-aiobotocore-iotdeviceadvisor-2.5.2.post2/types_aiobotocore_iotdeviceadvisor.egg-info/requires.txt
--rw-r--r--   0 vlad      (1000) vlad      (1000)       35 2023-08-04 13:59:12.000000 types-aiobotocore-iotdeviceadvisor-2.5.2.post2/types_aiobotocore_iotdeviceadvisor.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:23:52.570705 types-aiobotocore-iotdeviceadvisor-2.5.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-08 01:12:54.000000 types-aiobotocore-iotdeviceadvisor-2.5.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    12675 2023-08-08 01:23:52.570705 types-aiobotocore-iotdeviceadvisor-2.5.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    11127 2023-08-08 01:12:54.000000 types-aiobotocore-iotdeviceadvisor-2.5.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-08 01:23:52.570705 types-aiobotocore-iotdeviceadvisor-2.5.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2129 2023-08-08 01:12:54.000000 types-aiobotocore-iotdeviceadvisor-2.5.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:23:52.570705 types-aiobotocore-iotdeviceadvisor-2.5.4/types_aiobotocore_iotdeviceadvisor/
+-rw-r--r--   0 runner    (1001) docker     (123)      514 2023-08-08 01:12:54.000000 types-aiobotocore-iotdeviceadvisor-2.5.4/types_aiobotocore_iotdeviceadvisor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      513 2023-08-08 01:12:54.000000 types-aiobotocore-iotdeviceadvisor-2.5.4/types_aiobotocore_iotdeviceadvisor/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      967 2023-08-08 01:12:54.000000 types-aiobotocore-iotdeviceadvisor-2.5.4/types_aiobotocore_iotdeviceadvisor/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12963 2023-08-08 01:12:54.000000 types-aiobotocore-iotdeviceadvisor-2.5.4/types_aiobotocore_iotdeviceadvisor/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12941 2023-08-08 01:12:54.000000 types-aiobotocore-iotdeviceadvisor-2.5.4/types_aiobotocore_iotdeviceadvisor/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8701 2023-08-08 01:12:54.000000 types-aiobotocore-iotdeviceadvisor-2.5.4/types_aiobotocore_iotdeviceadvisor/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8699 2023-08-08 01:12:54.000000 types-aiobotocore-iotdeviceadvisor-2.5.4/types_aiobotocore_iotdeviceadvisor/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 01:12:54.000000 types-aiobotocore-iotdeviceadvisor-2.5.4/types_aiobotocore_iotdeviceadvisor/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    12286 2023-08-08 01:12:55.000000 types-aiobotocore-iotdeviceadvisor-2.5.4/types_aiobotocore_iotdeviceadvisor/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12275 2023-08-08 01:12:54.000000 types-aiobotocore-iotdeviceadvisor-2.5.4/types_aiobotocore_iotdeviceadvisor/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-08-08 01:12:54.000000 types-aiobotocore-iotdeviceadvisor-2.5.4/types_aiobotocore_iotdeviceadvisor/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:23:52.570705 types-aiobotocore-iotdeviceadvisor-2.5.4/types_aiobotocore_iotdeviceadvisor.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    12675 2023-08-08 01:23:52.000000 types-aiobotocore-iotdeviceadvisor-2.5.4/types_aiobotocore_iotdeviceadvisor.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      887 2023-08-08 01:23:52.000000 types-aiobotocore-iotdeviceadvisor-2.5.4/types_aiobotocore_iotdeviceadvisor.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 01:23:52.000000 types-aiobotocore-iotdeviceadvisor-2.5.4/types_aiobotocore_iotdeviceadvisor.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 01:23:52.000000 types-aiobotocore-iotdeviceadvisor-2.5.4/types_aiobotocore_iotdeviceadvisor.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-08 01:23:52.000000 types-aiobotocore-iotdeviceadvisor-2.5.4/types_aiobotocore_iotdeviceadvisor.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-08-08 01:23:52.000000 types-aiobotocore-iotdeviceadvisor-2.5.4/types_aiobotocore_iotdeviceadvisor.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-iotdeviceadvisor-2.5.2.post2/LICENSE` & `types-aiobotocore-iotdeviceadvisor-2.5.4/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-iotdeviceadvisor-2.5.2.post2/PKG-INFO` & `types-aiobotocore-iotdeviceadvisor-2.5.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-iotdeviceadvisor
-Version: 2.5.2.post2
-Summary: Type annotations for aiobotocore.IoTDeviceAdvisor 2.5.2 service generated with mypy-boto3-builder 7.17.2
+Version: 2.5.4
+Summary: Type annotations for aiobotocore.IoTDeviceAdvisor 2.5.4 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotdeviceadvisor/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-iotdeviceadvisor.svg?color=blue)](https://pypi.org/project/types-aiobotocore-iotdeviceadvisor)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotdeviceadvisor/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-iotdeviceadvisor)](https://pepy.tech/project/types-aiobotocore-iotdeviceadvisor)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.IoTDeviceAdvisor 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotdeviceadvisor.html#IoTDeviceAdvisor)
+[aiobotocore.IoTDeviceAdvisor 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotdeviceadvisor.html#IoTDeviceAdvisor)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-iotdeviceadvisor-2.5.2.post2/README.md` & `types-aiobotocore-iotdeviceadvisor-2.5.4/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-iotdeviceadvisor.svg?color=blue)](https://pypi.org/project/types-aiobotocore-iotdeviceadvisor)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotdeviceadvisor/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-iotdeviceadvisor)](https://pepy.tech/project/types-aiobotocore-iotdeviceadvisor)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.IoTDeviceAdvisor 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotdeviceadvisor.html#IoTDeviceAdvisor)
+[aiobotocore.IoTDeviceAdvisor 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotdeviceadvisor.html#IoTDeviceAdvisor)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-iotdeviceadvisor-2.5.2.post2/setup.py` & `types-aiobotocore-iotdeviceadvisor-2.5.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-iotdeviceadvisor",
-    version="2.5.2.post2",
+    version="2.5.4",
     packages=["types_aiobotocore_iotdeviceadvisor"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.IoTDeviceAdvisor 2.5.2 service generated with"
+        "Type annotations for aiobotocore.IoTDeviceAdvisor 2.5.4 service generated with"
         " mypy-boto3-builder 7.17.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
```

### Comparing `types-aiobotocore-iotdeviceadvisor-2.5.2.post2/types_aiobotocore_iotdeviceadvisor/__init__.py` & `types-aiobotocore-iotdeviceadvisor-2.5.4/types_aiobotocore_iotdeviceadvisor/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-iotdeviceadvisor-2.5.2.post2/types_aiobotocore_iotdeviceadvisor/__init__.pyi` & `types-aiobotocore-iotdeviceadvisor-2.5.4/types_aiobotocore_iotdeviceadvisor/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-iotdeviceadvisor-2.5.2.post2/types_aiobotocore_iotdeviceadvisor/client.py` & `types-aiobotocore-iotdeviceadvisor-2.5.4/types_aiobotocore_iotdeviceadvisor/client.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-iotdeviceadvisor-2.5.2.post2/types_aiobotocore_iotdeviceadvisor/client.pyi` & `types-aiobotocore-iotdeviceadvisor-2.5.4/types_aiobotocore_iotdeviceadvisor/client.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-iotdeviceadvisor-2.5.2.post2/types_aiobotocore_iotdeviceadvisor/literals.py` & `types-aiobotocore-iotdeviceadvisor-2.5.4/types_aiobotocore_iotdeviceadvisor/literals.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-iotdeviceadvisor-2.5.2.post2/types_aiobotocore_iotdeviceadvisor/literals.pyi` & `types-aiobotocore-iotdeviceadvisor-2.5.4/types_aiobotocore_iotdeviceadvisor/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-iotdeviceadvisor-2.5.2.post2/types_aiobotocore_iotdeviceadvisor/type_defs.py` & `types-aiobotocore-iotdeviceadvisor-2.5.4/types_aiobotocore_iotdeviceadvisor/type_defs.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-iotdeviceadvisor-2.5.2.post2/types_aiobotocore_iotdeviceadvisor/type_defs.pyi` & `types-aiobotocore-iotdeviceadvisor-2.5.4/types_aiobotocore_iotdeviceadvisor/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-iotdeviceadvisor-2.5.2.post2/types_aiobotocore_iotdeviceadvisor.egg-info/PKG-INFO` & `types-aiobotocore-iotdeviceadvisor-2.5.4/types_aiobotocore_iotdeviceadvisor.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-iotdeviceadvisor
-Version: 2.5.2.post2
-Summary: Type annotations for aiobotocore.IoTDeviceAdvisor 2.5.2 service generated with mypy-boto3-builder 7.17.2
+Version: 2.5.4
+Summary: Type annotations for aiobotocore.IoTDeviceAdvisor 2.5.4 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotdeviceadvisor/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-iotdeviceadvisor.svg?color=blue)](https://pypi.org/project/types-aiobotocore-iotdeviceadvisor)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotdeviceadvisor/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-iotdeviceadvisor)](https://pepy.tech/project/types-aiobotocore-iotdeviceadvisor)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.IoTDeviceAdvisor 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotdeviceadvisor.html#IoTDeviceAdvisor)
+[aiobotocore.IoTDeviceAdvisor 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotdeviceadvisor.html#IoTDeviceAdvisor)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-iotdeviceadvisor-2.5.2.post2/types_aiobotocore_iotdeviceadvisor.egg-info/SOURCES.txt` & `types-aiobotocore-iotdeviceadvisor-2.5.4/types_aiobotocore_iotdeviceadvisor.egg-info/SOURCES.txt`

 * *Files identical despite different names*


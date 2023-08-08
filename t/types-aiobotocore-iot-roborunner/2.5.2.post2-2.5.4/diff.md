# Comparing `tmp/types-aiobotocore-iot-roborunner-2.5.2.post2.tar.gz` & `tmp/types-aiobotocore-iot-roborunner-2.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-iot-roborunner-2.5.2.post2.tar", last modified: Fri Aug  4 13:59:12 2023, max compression
+gzip compressed data, was "types-aiobotocore-iot-roborunner-2.5.4.tar", last modified: Tue Aug  8 01:23:52 2023, max compression
```

## Comparing `types-aiobotocore-iot-roborunner-2.5.2.post2.tar` & `types-aiobotocore-iot-roborunner-2.5.4.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:12.156643 types-aiobotocore-iot-roborunner-2.5.2.post2/
--rw-r--r--   0 vlad      (1000) vlad      (1000)     1070 2023-08-04 13:40:47.000000 types-aiobotocore-iot-roborunner-2.5.2.post2/LICENSE
--rw-r--r--   0 vlad      (1000) vlad      (1000)    13718 2023-08-04 13:59:12.156643 types-aiobotocore-iot-roborunner-2.5.2.post2/PKG-INFO
--rw-r--r--   0 vlad      (1000) vlad      (1000)    12173 2023-08-04 13:40:47.000000 types-aiobotocore-iot-roborunner-2.5.2.post2/README.md
--rw-r--r--   0 vlad      (1000) vlad      (1000)       38 2023-08-04 13:59:12.156643 types-aiobotocore-iot-roborunner-2.5.2.post2/setup.cfg
--rw-r--r--   0 vlad      (1000) vlad      (1000)     2120 2023-08-04 13:40:47.000000 types-aiobotocore-iot-roborunner-2.5.2.post2/setup.py
-drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:12.146643 types-aiobotocore-iot-roborunner-2.5.2.post2/types_aiobotocore_iot_roborunner/
--rw-r--r--   0 vlad      (1000) vlad      (1000)     1270 2023-08-04 13:40:47.000000 types-aiobotocore-iot-roborunner-2.5.2.post2/types_aiobotocore_iot_roborunner/__init__.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)     1269 2023-08-04 13:40:47.000000 types-aiobotocore-iot-roborunner-2.5.2.post2/types_aiobotocore_iot_roborunner/__init__.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)      969 2023-08-04 13:40:47.000000 types-aiobotocore-iot-roborunner-2.5.2.post2/types_aiobotocore_iot_roborunner/__main__.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)    20847 2023-08-04 13:40:47.000000 types-aiobotocore-iot-roborunner-2.5.2.post2/types_aiobotocore_iot_roborunner/client.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)    20814 2023-08-04 13:40:47.000000 types-aiobotocore-iot-roborunner-2.5.2.post2/types_aiobotocore_iot_roborunner/client.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)     8309 2023-08-04 13:40:47.000000 types-aiobotocore-iot-roborunner-2.5.2.post2/types_aiobotocore_iot_roborunner/literals.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)     8307 2023-08-04 13:40:47.000000 types-aiobotocore-iot-roborunner-2.5.2.post2/types_aiobotocore_iot_roborunner/literals.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)     5494 2023-08-04 13:40:47.000000 types-aiobotocore-iot-roborunner-2.5.2.post2/types_aiobotocore_iot_roborunner/paginator.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)     5488 2023-08-04 13:40:47.000000 types-aiobotocore-iot-roborunner-2.5.2.post2/types_aiobotocore_iot_roborunner/paginator.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:40:47.000000 types-aiobotocore-iot-roborunner-2.5.2.post2/types_aiobotocore_iot_roborunner/py.typed
--rw-r--r--   0 vlad      (1000) vlad      (1000)    20234 2023-08-04 13:40:48.000000 types-aiobotocore-iot-roborunner-2.5.2.post2/types_aiobotocore_iot_roborunner/type_defs.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)    20195 2023-08-04 13:40:47.000000 types-aiobotocore-iot-roborunner-2.5.2.post2/types_aiobotocore_iot_roborunner/type_defs.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)       65 2023-08-04 13:40:47.000000 types-aiobotocore-iot-roborunner-2.5.2.post2/types_aiobotocore_iot_roborunner/version.py
-drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:12.156643 types-aiobotocore-iot-roborunner-2.5.2.post2/types_aiobotocore_iot_roborunner.egg-info/
--rw-r--r--   0 vlad      (1000) vlad      (1000)    13718 2023-08-04 13:59:12.000000 types-aiobotocore-iot-roborunner-2.5.2.post2/types_aiobotocore_iot_roborunner.egg-info/PKG-INFO
--rw-r--r--   0 vlad      (1000) vlad      (1000)      946 2023-08-04 13:59:12.000000 types-aiobotocore-iot-roborunner-2.5.2.post2/types_aiobotocore_iot_roborunner.egg-info/SOURCES.txt
--rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:12.000000 types-aiobotocore-iot-roborunner-2.5.2.post2/types_aiobotocore_iot_roborunner.egg-info/dependency_links.txt
--rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:12.000000 types-aiobotocore-iot-roborunner-2.5.2.post2/types_aiobotocore_iot_roborunner.egg-info/not-zip-safe
--rw-r--r--   0 vlad      (1000) vlad      (1000)       52 2023-08-04 13:59:12.000000 types-aiobotocore-iot-roborunner-2.5.2.post2/types_aiobotocore_iot_roborunner.egg-info/requires.txt
--rw-r--r--   0 vlad      (1000) vlad      (1000)       33 2023-08-04 13:59:12.000000 types-aiobotocore-iot-roborunner-2.5.2.post2/types_aiobotocore_iot_roborunner.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:23:52.358708 types-aiobotocore-iot-roborunner-2.5.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-08 01:12:48.000000 types-aiobotocore-iot-roborunner-2.5.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    13712 2023-08-08 01:23:52.358708 types-aiobotocore-iot-roborunner-2.5.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    12173 2023-08-08 01:12:48.000000 types-aiobotocore-iot-roborunner-2.5.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-08 01:23:52.358708 types-aiobotocore-iot-roborunner-2.5.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2114 2023-08-08 01:12:48.000000 types-aiobotocore-iot-roborunner-2.5.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:23:52.354708 types-aiobotocore-iot-roborunner-2.5.4/types_aiobotocore_iot_roborunner/
+-rw-r--r--   0 runner    (1001) docker     (123)     1270 2023-08-08 01:12:48.000000 types-aiobotocore-iot-roborunner-2.5.4/types_aiobotocore_iot_roborunner/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1269 2023-08-08 01:12:48.000000 types-aiobotocore-iot-roborunner-2.5.4/types_aiobotocore_iot_roborunner/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      957 2023-08-08 01:12:48.000000 types-aiobotocore-iot-roborunner-2.5.4/types_aiobotocore_iot_roborunner/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20847 2023-08-08 01:12:49.000000 types-aiobotocore-iot-roborunner-2.5.4/types_aiobotocore_iot_roborunner/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20814 2023-08-08 01:12:48.000000 types-aiobotocore-iot-roborunner-2.5.4/types_aiobotocore_iot_roborunner/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8309 2023-08-08 01:12:49.000000 types-aiobotocore-iot-roborunner-2.5.4/types_aiobotocore_iot_roborunner/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8307 2023-08-08 01:12:49.000000 types-aiobotocore-iot-roborunner-2.5.4/types_aiobotocore_iot_roborunner/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     5494 2023-08-08 01:12:49.000000 types-aiobotocore-iot-roborunner-2.5.4/types_aiobotocore_iot_roborunner/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5488 2023-08-08 01:12:49.000000 types-aiobotocore-iot-roborunner-2.5.4/types_aiobotocore_iot_roborunner/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 01:12:48.000000 types-aiobotocore-iot-roborunner-2.5.4/types_aiobotocore_iot_roborunner/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    20234 2023-08-08 01:12:49.000000 types-aiobotocore-iot-roborunner-2.5.4/types_aiobotocore_iot_roborunner/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20195 2023-08-08 01:12:49.000000 types-aiobotocore-iot-roborunner-2.5.4/types_aiobotocore_iot_roborunner/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-08-08 01:12:48.000000 types-aiobotocore-iot-roborunner-2.5.4/types_aiobotocore_iot_roborunner/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:23:52.358708 types-aiobotocore-iot-roborunner-2.5.4/types_aiobotocore_iot_roborunner.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    13712 2023-08-08 01:23:52.000000 types-aiobotocore-iot-roborunner-2.5.4/types_aiobotocore_iot_roborunner.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      946 2023-08-08 01:23:52.000000 types-aiobotocore-iot-roborunner-2.5.4/types_aiobotocore_iot_roborunner.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 01:23:52.000000 types-aiobotocore-iot-roborunner-2.5.4/types_aiobotocore_iot_roborunner.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 01:23:52.000000 types-aiobotocore-iot-roborunner-2.5.4/types_aiobotocore_iot_roborunner.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-08 01:23:52.000000 types-aiobotocore-iot-roborunner-2.5.4/types_aiobotocore_iot_roborunner.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-08-08 01:23:52.000000 types-aiobotocore-iot-roborunner-2.5.4/types_aiobotocore_iot_roborunner.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-iot-roborunner-2.5.2.post2/LICENSE` & `types-aiobotocore-iot-roborunner-2.5.4/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-iot-roborunner-2.5.2.post2/PKG-INFO` & `types-aiobotocore-iot-roborunner-2.5.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-iot-roborunner
-Version: 2.5.2.post2
-Summary: Type annotations for aiobotocore.IoTRoboRunner 2.5.2 service generated with mypy-boto3-builder 7.17.2
+Version: 2.5.4
+Summary: Type annotations for aiobotocore.IoTRoboRunner 2.5.4 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot_roborunner/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-iot-roborunner.svg?color=blue)](https://pypi.org/project/types-aiobotocore-iot-roborunner)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot_roborunner/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-iot-roborunner)](https://pepy.tech/project/types-aiobotocore-iot-roborunner)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.IoTRoboRunner 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot-roborunner.html#IoTRoboRunner)
+[aiobotocore.IoTRoboRunner 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot-roborunner.html#IoTRoboRunner)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-iot-roborunner-2.5.2.post2/README.md` & `types-aiobotocore-iot-roborunner-2.5.4/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-iot-roborunner.svg?color=blue)](https://pypi.org/project/types-aiobotocore-iot-roborunner)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot_roborunner/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-iot-roborunner)](https://pepy.tech/project/types-aiobotocore-iot-roborunner)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.IoTRoboRunner 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot-roborunner.html#IoTRoboRunner)
+[aiobotocore.IoTRoboRunner 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot-roborunner.html#IoTRoboRunner)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-iot-roborunner-2.5.2.post2/setup.py` & `types-aiobotocore-iot-roborunner-2.5.4/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-iot-roborunner",
-    version="2.5.2.post2",
+    version="2.5.4",
     packages=["types_aiobotocore_iot_roborunner"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.IoTRoboRunner 2.5.2 service generated with"
+        "Type annotations for aiobotocore.IoTRoboRunner 2.5.4 service generated with"
         " mypy-boto3-builder 7.17.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
```

### Comparing `types-aiobotocore-iot-roborunner-2.5.2.post2/types_aiobotocore_iot_roborunner/__init__.py` & `types-aiobotocore-iot-roborunner-2.5.4/types_aiobotocore_iot_roborunner/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-iot-roborunner-2.5.2.post2/types_aiobotocore_iot_roborunner/__init__.pyi` & `types-aiobotocore-iot-roborunner-2.5.4/types_aiobotocore_iot_roborunner/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-iot-roborunner-2.5.2.post2/types_aiobotocore_iot_roborunner/__main__.py` & `types-aiobotocore-iot-roborunner-2.5.4/types_aiobotocore_iot_roborunner/__main__.py`

 * *Files 16% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.IoTRoboRunner 2.5.2\nVersion:        "
-        " 2.5.2.post2\nBuilder version: 7.17.2\nDocs:           "
+        "Type annotations for aiobotocore.IoTRoboRunner 2.5.4\nVersion:         2.5.4\nBuilder"
+        " version: 7.17.2\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot_roborunner//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot-roborunner.html#IoTRoboRunner\nOther"
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

### Comparing `types-aiobotocore-iot-roborunner-2.5.2.post2/types_aiobotocore_iot_roborunner/client.py` & `types-aiobotocore-iot-roborunner-2.5.4/types_aiobotocore_iot_roborunner/client.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-iot-roborunner-2.5.2.post2/types_aiobotocore_iot_roborunner/client.pyi` & `types-aiobotocore-iot-roborunner-2.5.4/types_aiobotocore_iot_roborunner/client.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-iot-roborunner-2.5.2.post2/types_aiobotocore_iot_roborunner/literals.py` & `types-aiobotocore-iot-roborunner-2.5.4/types_aiobotocore_iot_roborunner/literals.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-iot-roborunner-2.5.2.post2/types_aiobotocore_iot_roborunner/literals.pyi` & `types-aiobotocore-iot-roborunner-2.5.4/types_aiobotocore_iot_roborunner/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-iot-roborunner-2.5.2.post2/types_aiobotocore_iot_roborunner/paginator.py` & `types-aiobotocore-iot-roborunner-2.5.4/types_aiobotocore_iot_roborunner/paginator.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-iot-roborunner-2.5.2.post2/types_aiobotocore_iot_roborunner/paginator.pyi` & `types-aiobotocore-iot-roborunner-2.5.4/types_aiobotocore_iot_roborunner/paginator.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-iot-roborunner-2.5.2.post2/types_aiobotocore_iot_roborunner/type_defs.py` & `types-aiobotocore-iot-roborunner-2.5.4/types_aiobotocore_iot_roborunner/type_defs.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-iot-roborunner-2.5.2.post2/types_aiobotocore_iot_roborunner/type_defs.pyi` & `types-aiobotocore-iot-roborunner-2.5.4/types_aiobotocore_iot_roborunner/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-iot-roborunner-2.5.2.post2/types_aiobotocore_iot_roborunner.egg-info/PKG-INFO` & `types-aiobotocore-iot-roborunner-2.5.4/types_aiobotocore_iot_roborunner.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-iot-roborunner
-Version: 2.5.2.post2
-Summary: Type annotations for aiobotocore.IoTRoboRunner 2.5.2 service generated with mypy-boto3-builder 7.17.2
+Version: 2.5.4
+Summary: Type annotations for aiobotocore.IoTRoboRunner 2.5.4 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot_roborunner/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-iot-roborunner.svg?color=blue)](https://pypi.org/project/types-aiobotocore-iot-roborunner)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot_roborunner/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-iot-roborunner)](https://pepy.tech/project/types-aiobotocore-iot-roborunner)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.IoTRoboRunner 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot-roborunner.html#IoTRoboRunner)
+[aiobotocore.IoTRoboRunner 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot-roborunner.html#IoTRoboRunner)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-iot-roborunner-2.5.2.post2/types_aiobotocore_iot_roborunner.egg-info/SOURCES.txt` & `types-aiobotocore-iot-roborunner-2.5.4/types_aiobotocore_iot_roborunner.egg-info/SOURCES.txt`

 * *Files identical despite different names*


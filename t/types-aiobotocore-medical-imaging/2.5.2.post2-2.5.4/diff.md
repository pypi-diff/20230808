# Comparing `tmp/types-aiobotocore-medical-imaging-2.5.2.post2.tar.gz` & `tmp/types-aiobotocore-medical-imaging-2.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-medical-imaging-2.5.2.post2.tar", last modified: Fri Aug  4 13:59:18 2023, max compression
+gzip compressed data, was "types-aiobotocore-medical-imaging-2.5.4.tar", last modified: Tue Aug  8 01:24:06 2023, max compression
```

## Comparing `types-aiobotocore-medical-imaging-2.5.2.post2.tar` & `types-aiobotocore-medical-imaging-2.5.4.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:18.326643 types-aiobotocore-medical-imaging-2.5.2.post2/
--rw-r--r--   0 vlad      (1000) vlad      (1000)     1070 2023-08-04 13:44:46.000000 types-aiobotocore-medical-imaging-2.5.2.post2/LICENSE
--rw-r--r--   0 vlad      (1000) vlad      (1000)    13818 2023-08-04 13:59:18.326643 types-aiobotocore-medical-imaging-2.5.2.post2/PKG-INFO
--rw-r--r--   0 vlad      (1000) vlad      (1000)    12270 2023-08-04 13:44:46.000000 types-aiobotocore-medical-imaging-2.5.2.post2/README.md
--rw-r--r--   0 vlad      (1000) vlad      (1000)       38 2023-08-04 13:59:18.326643 types-aiobotocore-medical-imaging-2.5.2.post2/setup.cfg
--rw-r--r--   0 vlad      (1000) vlad      (1000)     2126 2023-08-04 13:44:46.000000 types-aiobotocore-medical-imaging-2.5.2.post2/setup.py
-drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:18.326643 types-aiobotocore-medical-imaging-2.5.2.post2/types_aiobotocore_medical_imaging/
--rw-r--r--   0 vlad      (1000) vlad      (1000)     1377 2023-08-04 13:44:46.000000 types-aiobotocore-medical-imaging-2.5.2.post2/types_aiobotocore_medical_imaging/__init__.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)     1376 2023-08-04 13:44:46.000000 types-aiobotocore-medical-imaging-2.5.2.post2/types_aiobotocore_medical_imaging/__init__.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)      971 2023-08-04 13:44:46.000000 types-aiobotocore-medical-imaging-2.5.2.post2/types_aiobotocore_medical_imaging/__main__.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)    17746 2023-08-04 13:44:46.000000 types-aiobotocore-medical-imaging-2.5.2.post2/types_aiobotocore_medical_imaging/client.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)    17715 2023-08-04 13:44:46.000000 types-aiobotocore-medical-imaging-2.5.2.post2/types_aiobotocore_medical_imaging/client.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)     8832 2023-08-04 13:44:47.000000 types-aiobotocore-medical-imaging-2.5.2.post2/types_aiobotocore_medical_imaging/literals.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)     8830 2023-08-04 13:44:46.000000 types-aiobotocore-medical-imaging-2.5.2.post2/types_aiobotocore_medical_imaging/literals.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)     5918 2023-08-04 13:44:46.000000 types-aiobotocore-medical-imaging-2.5.2.post2/types_aiobotocore_medical_imaging/paginator.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)     5912 2023-08-04 13:44:46.000000 types-aiobotocore-medical-imaging-2.5.2.post2/types_aiobotocore_medical_imaging/paginator.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:44:46.000000 types-aiobotocore-medical-imaging-2.5.2.post2/types_aiobotocore_medical_imaging/py.typed
--rw-r--r--   0 vlad      (1000) vlad      (1000)    24232 2023-08-04 13:44:48.000000 types-aiobotocore-medical-imaging-2.5.2.post2/types_aiobotocore_medical_imaging/type_defs.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)    24192 2023-08-04 13:44:47.000000 types-aiobotocore-medical-imaging-2.5.2.post2/types_aiobotocore_medical_imaging/type_defs.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)       65 2023-08-04 13:44:46.000000 types-aiobotocore-medical-imaging-2.5.2.post2/types_aiobotocore_medical_imaging/version.py
-drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:18.326643 types-aiobotocore-medical-imaging-2.5.2.post2/types_aiobotocore_medical_imaging.egg-info/
--rw-r--r--   0 vlad      (1000) vlad      (1000)    13818 2023-08-04 13:59:18.000000 types-aiobotocore-medical-imaging-2.5.2.post2/types_aiobotocore_medical_imaging.egg-info/PKG-INFO
--rw-r--r--   0 vlad      (1000) vlad      (1000)      965 2023-08-04 13:59:18.000000 types-aiobotocore-medical-imaging-2.5.2.post2/types_aiobotocore_medical_imaging.egg-info/SOURCES.txt
--rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:18.000000 types-aiobotocore-medical-imaging-2.5.2.post2/types_aiobotocore_medical_imaging.egg-info/dependency_links.txt
--rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:18.000000 types-aiobotocore-medical-imaging-2.5.2.post2/types_aiobotocore_medical_imaging.egg-info/not-zip-safe
--rw-r--r--   0 vlad      (1000) vlad      (1000)       52 2023-08-04 13:59:18.000000 types-aiobotocore-medical-imaging-2.5.2.post2/types_aiobotocore_medical_imaging.egg-info/requires.txt
--rw-r--r--   0 vlad      (1000) vlad      (1000)       34 2023-08-04 13:59:18.000000 types-aiobotocore-medical-imaging-2.5.2.post2/types_aiobotocore_medical_imaging.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:24:06.486735 types-aiobotocore-medical-imaging-2.5.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-08 01:15:23.000000 types-aiobotocore-medical-imaging-2.5.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    13812 2023-08-08 01:24:06.486735 types-aiobotocore-medical-imaging-2.5.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    12270 2023-08-08 01:15:23.000000 types-aiobotocore-medical-imaging-2.5.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-08 01:24:06.486735 types-aiobotocore-medical-imaging-2.5.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2120 2023-08-08 01:15:22.000000 types-aiobotocore-medical-imaging-2.5.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:24:06.470735 types-aiobotocore-medical-imaging-2.5.4/types_aiobotocore_medical_imaging/
+-rw-r--r--   0 runner    (1001) docker     (123)     1377 2023-08-08 01:15:23.000000 types-aiobotocore-medical-imaging-2.5.4/types_aiobotocore_medical_imaging/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1376 2023-08-08 01:15:23.000000 types-aiobotocore-medical-imaging-2.5.4/types_aiobotocore_medical_imaging/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      959 2023-08-08 01:15:23.000000 types-aiobotocore-medical-imaging-2.5.4/types_aiobotocore_medical_imaging/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17746 2023-08-08 01:15:23.000000 types-aiobotocore-medical-imaging-2.5.4/types_aiobotocore_medical_imaging/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17715 2023-08-08 01:15:23.000000 types-aiobotocore-medical-imaging-2.5.4/types_aiobotocore_medical_imaging/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8832 2023-08-08 01:15:23.000000 types-aiobotocore-medical-imaging-2.5.4/types_aiobotocore_medical_imaging/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8830 2023-08-08 01:15:23.000000 types-aiobotocore-medical-imaging-2.5.4/types_aiobotocore_medical_imaging/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     5918 2023-08-08 01:15:23.000000 types-aiobotocore-medical-imaging-2.5.4/types_aiobotocore_medical_imaging/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5912 2023-08-08 01:15:23.000000 types-aiobotocore-medical-imaging-2.5.4/types_aiobotocore_medical_imaging/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 01:15:23.000000 types-aiobotocore-medical-imaging-2.5.4/types_aiobotocore_medical_imaging/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    24232 2023-08-08 01:15:23.000000 types-aiobotocore-medical-imaging-2.5.4/types_aiobotocore_medical_imaging/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24192 2023-08-08 01:15:23.000000 types-aiobotocore-medical-imaging-2.5.4/types_aiobotocore_medical_imaging/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-08-08 01:15:23.000000 types-aiobotocore-medical-imaging-2.5.4/types_aiobotocore_medical_imaging/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:24:06.486735 types-aiobotocore-medical-imaging-2.5.4/types_aiobotocore_medical_imaging.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    13812 2023-08-08 01:24:06.000000 types-aiobotocore-medical-imaging-2.5.4/types_aiobotocore_medical_imaging.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      965 2023-08-08 01:24:06.000000 types-aiobotocore-medical-imaging-2.5.4/types_aiobotocore_medical_imaging.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 01:24:06.000000 types-aiobotocore-medical-imaging-2.5.4/types_aiobotocore_medical_imaging.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 01:24:06.000000 types-aiobotocore-medical-imaging-2.5.4/types_aiobotocore_medical_imaging.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-08 01:24:06.000000 types-aiobotocore-medical-imaging-2.5.4/types_aiobotocore_medical_imaging.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-08-08 01:24:06.000000 types-aiobotocore-medical-imaging-2.5.4/types_aiobotocore_medical_imaging.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-medical-imaging-2.5.2.post2/LICENSE` & `types-aiobotocore-medical-imaging-2.5.4/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-medical-imaging-2.5.2.post2/PKG-INFO` & `types-aiobotocore-medical-imaging-2.5.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-medical-imaging
-Version: 2.5.2.post2
-Summary: Type annotations for aiobotocore.HealthImaging 2.5.2 service generated with mypy-boto3-builder 7.17.2
+Version: 2.5.4
+Summary: Type annotations for aiobotocore.HealthImaging 2.5.4 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_medical_imaging/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-medical-imaging.svg?color=blue)](https://pypi.org/project/types-aiobotocore-medical-imaging)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_medical_imaging/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-medical-imaging)](https://pepy.tech/project/types-aiobotocore-medical-imaging)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.HealthImaging 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medical-imaging.html#HealthImaging)
+[aiobotocore.HealthImaging 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medical-imaging.html#HealthImaging)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-medical-imaging-2.5.2.post2/README.md` & `types-aiobotocore-medical-imaging-2.5.4/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-medical-imaging.svg?color=blue)](https://pypi.org/project/types-aiobotocore-medical-imaging)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_medical_imaging/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-medical-imaging)](https://pepy.tech/project/types-aiobotocore-medical-imaging)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.HealthImaging 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medical-imaging.html#HealthImaging)
+[aiobotocore.HealthImaging 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medical-imaging.html#HealthImaging)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-medical-imaging-2.5.2.post2/setup.py` & `types-aiobotocore-medical-imaging-2.5.4/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-medical-imaging",
-    version="2.5.2.post2",
+    version="2.5.4",
     packages=["types_aiobotocore_medical_imaging"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.HealthImaging 2.5.2 service generated with"
+        "Type annotations for aiobotocore.HealthImaging 2.5.4 service generated with"
         " mypy-boto3-builder 7.17.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
```

### Comparing `types-aiobotocore-medical-imaging-2.5.2.post2/types_aiobotocore_medical_imaging/__init__.py` & `types-aiobotocore-medical-imaging-2.5.4/types_aiobotocore_medical_imaging/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-medical-imaging-2.5.2.post2/types_aiobotocore_medical_imaging/__init__.pyi` & `types-aiobotocore-medical-imaging-2.5.4/types_aiobotocore_medical_imaging/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-medical-imaging-2.5.2.post2/types_aiobotocore_medical_imaging/__main__.py` & `types-aiobotocore-medical-imaging-2.5.4/types_aiobotocore_medical_imaging/__main__.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.HealthImaging 2.5.2\nVersion:        "
-        " 2.5.2.post2\nBuilder version: 7.17.2\nDocs:           "
+        "Type annotations for aiobotocore.HealthImaging 2.5.4\nVersion:         2.5.4\nBuilder"
+        " version: 7.17.2\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_medical_imaging//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medical-imaging.html#HealthImaging\nOther"
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

### Comparing `types-aiobotocore-medical-imaging-2.5.2.post2/types_aiobotocore_medical_imaging/client.py` & `types-aiobotocore-medical-imaging-2.5.4/types_aiobotocore_medical_imaging/client.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-medical-imaging-2.5.2.post2/types_aiobotocore_medical_imaging/client.pyi` & `types-aiobotocore-medical-imaging-2.5.4/types_aiobotocore_medical_imaging/client.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-medical-imaging-2.5.2.post2/types_aiobotocore_medical_imaging/literals.py` & `types-aiobotocore-medical-imaging-2.5.4/types_aiobotocore_medical_imaging/literals.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-medical-imaging-2.5.2.post2/types_aiobotocore_medical_imaging/literals.pyi` & `types-aiobotocore-medical-imaging-2.5.4/types_aiobotocore_medical_imaging/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-medical-imaging-2.5.2.post2/types_aiobotocore_medical_imaging/paginator.py` & `types-aiobotocore-medical-imaging-2.5.4/types_aiobotocore_medical_imaging/paginator.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-medical-imaging-2.5.2.post2/types_aiobotocore_medical_imaging/paginator.pyi` & `types-aiobotocore-medical-imaging-2.5.4/types_aiobotocore_medical_imaging/paginator.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-medical-imaging-2.5.2.post2/types_aiobotocore_medical_imaging/type_defs.py` & `types-aiobotocore-medical-imaging-2.5.4/types_aiobotocore_medical_imaging/type_defs.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-medical-imaging-2.5.2.post2/types_aiobotocore_medical_imaging/type_defs.pyi` & `types-aiobotocore-medical-imaging-2.5.4/types_aiobotocore_medical_imaging/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-medical-imaging-2.5.2.post2/types_aiobotocore_medical_imaging.egg-info/PKG-INFO` & `types-aiobotocore-medical-imaging-2.5.4/types_aiobotocore_medical_imaging.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-medical-imaging
-Version: 2.5.2.post2
-Summary: Type annotations for aiobotocore.HealthImaging 2.5.2 service generated with mypy-boto3-builder 7.17.2
+Version: 2.5.4
+Summary: Type annotations for aiobotocore.HealthImaging 2.5.4 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_medical_imaging/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-medical-imaging.svg?color=blue)](https://pypi.org/project/types-aiobotocore-medical-imaging)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_medical_imaging/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-medical-imaging)](https://pepy.tech/project/types-aiobotocore-medical-imaging)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.HealthImaging 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medical-imaging.html#HealthImaging)
+[aiobotocore.HealthImaging 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medical-imaging.html#HealthImaging)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-medical-imaging-2.5.2.post2/types_aiobotocore_medical_imaging.egg-info/SOURCES.txt` & `types-aiobotocore-medical-imaging-2.5.4/types_aiobotocore_medical_imaging.egg-info/SOURCES.txt`

 * *Files identical despite different names*


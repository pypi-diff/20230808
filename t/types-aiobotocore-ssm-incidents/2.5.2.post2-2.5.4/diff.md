# Comparing `tmp/types-aiobotocore-ssm-incidents-2.5.2.post2.tar.gz` & `tmp/types-aiobotocore-ssm-incidents-2.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-ssm-incidents-2.5.2.post2.tar", last modified: Fri Aug  4 13:59:27 2023, max compression
+gzip compressed data, was "types-aiobotocore-ssm-incidents-2.5.4.tar", last modified: Tue Aug  8 01:24:29 2023, max compression
```

## Comparing `types-aiobotocore-ssm-incidents-2.5.2.post2.tar` & `types-aiobotocore-ssm-incidents-2.5.4.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:27.556643 types-aiobotocore-ssm-incidents-2.5.2.post2/
--rw-r--r--   0 vlad      (1000) vlad      (1000)     1070 2023-08-04 13:54:25.000000 types-aiobotocore-ssm-incidents-2.5.2.post2/LICENSE
--rw-r--r--   0 vlad      (1000) vlad      (1000)    15093 2023-08-04 13:59:27.556643 types-aiobotocore-ssm-incidents-2.5.2.post2/PKG-INFO
--rw-r--r--   0 vlad      (1000) vlad      (1000)    13552 2023-08-04 13:54:25.000000 types-aiobotocore-ssm-incidents-2.5.2.post2/README.md
--rw-r--r--   0 vlad      (1000) vlad      (1000)       38 2023-08-04 13:59:27.556643 types-aiobotocore-ssm-incidents-2.5.2.post2/setup.cfg
--rw-r--r--   0 vlad      (1000) vlad      (1000)     2113 2023-08-04 13:54:21.000000 types-aiobotocore-ssm-incidents-2.5.2.post2/setup.py
-drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:27.556643 types-aiobotocore-ssm-incidents-2.5.2.post2/types_aiobotocore_ssm_incidents/
--rw-r--r--   0 vlad      (1000) vlad      (1000)     2350 2023-08-04 13:54:25.000000 types-aiobotocore-ssm-incidents-2.5.2.post2/types_aiobotocore_ssm_incidents/__init__.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)     2349 2023-08-04 13:54:25.000000 types-aiobotocore-ssm-incidents-2.5.2.post2/types_aiobotocore_ssm_incidents/__init__.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)      965 2023-08-04 13:54:25.000000 types-aiobotocore-ssm-incidents-2.5.2.post2/types_aiobotocore_ssm_incidents/__main__.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)    27541 2023-08-04 13:54:25.000000 types-aiobotocore-ssm-incidents-2.5.2.post2/types_aiobotocore_ssm_incidents/client.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)    27495 2023-08-04 13:54:25.000000 types-aiobotocore-ssm-incidents-2.5.2.post2/types_aiobotocore_ssm_incidents/client.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)    10098 2023-08-04 13:54:25.000000 types-aiobotocore-ssm-incidents-2.5.2.post2/types_aiobotocore_ssm_incidents/literals.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)    10096 2023-08-04 13:54:25.000000 types-aiobotocore-ssm-incidents-2.5.2.post2/types_aiobotocore_ssm_incidents/literals.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)     8283 2023-08-04 13:54:25.000000 types-aiobotocore-ssm-incidents-2.5.2.post2/types_aiobotocore_ssm_incidents/paginator.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)     8274 2023-08-04 13:54:25.000000 types-aiobotocore-ssm-incidents-2.5.2.post2/types_aiobotocore_ssm_incidents/paginator.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:54:25.000000 types-aiobotocore-ssm-incidents-2.5.2.post2/types_aiobotocore_ssm_incidents/py.typed
--rw-r--r--   0 vlad      (1000) vlad      (1000)    33953 2023-08-04 13:54:26.000000 types-aiobotocore-ssm-incidents-2.5.2.post2/types_aiobotocore_ssm_incidents/type_defs.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)    33889 2023-08-04 13:54:26.000000 types-aiobotocore-ssm-incidents-2.5.2.post2/types_aiobotocore_ssm_incidents/type_defs.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)       65 2023-08-04 13:54:25.000000 types-aiobotocore-ssm-incidents-2.5.2.post2/types_aiobotocore_ssm_incidents/version.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)     2829 2023-08-04 13:54:25.000000 types-aiobotocore-ssm-incidents-2.5.2.post2/types_aiobotocore_ssm_incidents/waiter.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)     2827 2023-08-04 13:54:25.000000 types-aiobotocore-ssm-incidents-2.5.2.post2/types_aiobotocore_ssm_incidents/waiter.pyi
-drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:27.556643 types-aiobotocore-ssm-incidents-2.5.2.post2/types_aiobotocore_ssm_incidents.egg-info/
--rw-r--r--   0 vlad      (1000) vlad      (1000)    15093 2023-08-04 13:59:27.000000 types-aiobotocore-ssm-incidents-2.5.2.post2/types_aiobotocore_ssm_incidents.egg-info/PKG-INFO
--rw-r--r--   0 vlad      (1000) vlad      (1000)     1012 2023-08-04 13:59:27.000000 types-aiobotocore-ssm-incidents-2.5.2.post2/types_aiobotocore_ssm_incidents.egg-info/SOURCES.txt
--rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:27.000000 types-aiobotocore-ssm-incidents-2.5.2.post2/types_aiobotocore_ssm_incidents.egg-info/dependency_links.txt
--rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:27.000000 types-aiobotocore-ssm-incidents-2.5.2.post2/types_aiobotocore_ssm_incidents.egg-info/not-zip-safe
--rw-r--r--   0 vlad      (1000) vlad      (1000)       52 2023-08-04 13:59:27.000000 types-aiobotocore-ssm-incidents-2.5.2.post2/types_aiobotocore_ssm_incidents.egg-info/requires.txt
--rw-r--r--   0 vlad      (1000) vlad      (1000)       32 2023-08-04 13:59:27.000000 types-aiobotocore-ssm-incidents-2.5.2.post2/types_aiobotocore_ssm_incidents.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:24:29.606789 types-aiobotocore-ssm-incidents-2.5.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-08 01:21:36.000000 types-aiobotocore-ssm-incidents-2.5.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    15087 2023-08-08 01:24:29.606789 types-aiobotocore-ssm-incidents-2.5.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    13552 2023-08-08 01:21:36.000000 types-aiobotocore-ssm-incidents-2.5.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-08 01:24:29.606789 types-aiobotocore-ssm-incidents-2.5.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2107 2023-08-08 01:21:36.000000 types-aiobotocore-ssm-incidents-2.5.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:24:29.602789 types-aiobotocore-ssm-incidents-2.5.4/types_aiobotocore_ssm_incidents/
+-rw-r--r--   0 runner    (1001) docker     (123)     2350 2023-08-08 01:21:36.000000 types-aiobotocore-ssm-incidents-2.5.4/types_aiobotocore_ssm_incidents/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2349 2023-08-08 01:21:36.000000 types-aiobotocore-ssm-incidents-2.5.4/types_aiobotocore_ssm_incidents/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      953 2023-08-08 01:21:36.000000 types-aiobotocore-ssm-incidents-2.5.4/types_aiobotocore_ssm_incidents/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27541 2023-08-08 01:21:36.000000 types-aiobotocore-ssm-incidents-2.5.4/types_aiobotocore_ssm_incidents/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27495 2023-08-08 01:21:36.000000 types-aiobotocore-ssm-incidents-2.5.4/types_aiobotocore_ssm_incidents/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    10098 2023-08-08 01:21:36.000000 types-aiobotocore-ssm-incidents-2.5.4/types_aiobotocore_ssm_incidents/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10096 2023-08-08 01:21:36.000000 types-aiobotocore-ssm-incidents-2.5.4/types_aiobotocore_ssm_incidents/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8283 2023-08-08 01:21:36.000000 types-aiobotocore-ssm-incidents-2.5.4/types_aiobotocore_ssm_incidents/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8274 2023-08-08 01:21:36.000000 types-aiobotocore-ssm-incidents-2.5.4/types_aiobotocore_ssm_incidents/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 01:21:36.000000 types-aiobotocore-ssm-incidents-2.5.4/types_aiobotocore_ssm_incidents/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    33953 2023-08-08 01:21:40.000000 types-aiobotocore-ssm-incidents-2.5.4/types_aiobotocore_ssm_incidents/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33889 2023-08-08 01:21:40.000000 types-aiobotocore-ssm-incidents-2.5.4/types_aiobotocore_ssm_incidents/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-08-08 01:21:36.000000 types-aiobotocore-ssm-incidents-2.5.4/types_aiobotocore_ssm_incidents/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2829 2023-08-08 01:21:36.000000 types-aiobotocore-ssm-incidents-2.5.4/types_aiobotocore_ssm_incidents/waiter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2827 2023-08-08 01:21:36.000000 types-aiobotocore-ssm-incidents-2.5.4/types_aiobotocore_ssm_incidents/waiter.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:24:29.602789 types-aiobotocore-ssm-incidents-2.5.4/types_aiobotocore_ssm_incidents.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    15087 2023-08-08 01:24:29.000000 types-aiobotocore-ssm-incidents-2.5.4/types_aiobotocore_ssm_incidents.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1012 2023-08-08 01:24:29.000000 types-aiobotocore-ssm-incidents-2.5.4/types_aiobotocore_ssm_incidents.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 01:24:29.000000 types-aiobotocore-ssm-incidents-2.5.4/types_aiobotocore_ssm_incidents.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 01:24:29.000000 types-aiobotocore-ssm-incidents-2.5.4/types_aiobotocore_ssm_incidents.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-08 01:24:29.000000 types-aiobotocore-ssm-incidents-2.5.4/types_aiobotocore_ssm_incidents.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-08-08 01:24:29.000000 types-aiobotocore-ssm-incidents-2.5.4/types_aiobotocore_ssm_incidents.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-ssm-incidents-2.5.2.post2/LICENSE` & `types-aiobotocore-ssm-incidents-2.5.4/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-ssm-incidents-2.5.2.post2/PKG-INFO` & `types-aiobotocore-ssm-incidents-2.5.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-ssm-incidents
-Version: 2.5.2.post2
-Summary: Type annotations for aiobotocore.SSMIncidents 2.5.2 service generated with mypy-boto3-builder 7.17.2
+Version: 2.5.4
+Summary: Type annotations for aiobotocore.SSMIncidents 2.5.4 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm_incidents/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-ssm-incidents.svg?color=blue)](https://pypi.org/project/types-aiobotocore-ssm-incidents)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm_incidents/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-ssm-incidents)](https://pepy.tech/project/types-aiobotocore-ssm-incidents)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.SSMIncidents 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-incidents.html#SSMIncidents)
+[aiobotocore.SSMIncidents 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-incidents.html#SSMIncidents)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-ssm-incidents-2.5.2.post2/README.md` & `types-aiobotocore-ssm-incidents-2.5.4/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-ssm-incidents.svg?color=blue)](https://pypi.org/project/types-aiobotocore-ssm-incidents)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm_incidents/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-ssm-incidents)](https://pepy.tech/project/types-aiobotocore-ssm-incidents)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.SSMIncidents 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-incidents.html#SSMIncidents)
+[aiobotocore.SSMIncidents 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-incidents.html#SSMIncidents)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-ssm-incidents-2.5.2.post2/setup.py` & `types-aiobotocore-ssm-incidents-2.5.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-ssm-incidents",
-    version="2.5.2.post2",
+    version="2.5.4",
     packages=["types_aiobotocore_ssm_incidents"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.SSMIncidents 2.5.2 service generated with"
+        "Type annotations for aiobotocore.SSMIncidents 2.5.4 service generated with"
         " mypy-boto3-builder 7.17.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
```

### Comparing `types-aiobotocore-ssm-incidents-2.5.2.post2/types_aiobotocore_ssm_incidents/__init__.py` & `types-aiobotocore-ssm-incidents-2.5.4/types_aiobotocore_ssm_incidents/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-ssm-incidents-2.5.2.post2/types_aiobotocore_ssm_incidents/__init__.pyi` & `types-aiobotocore-ssm-incidents-2.5.4/types_aiobotocore_ssm_incidents/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-ssm-incidents-2.5.2.post2/types_aiobotocore_ssm_incidents/__main__.py` & `types-aiobotocore-ssm-incidents-2.5.4/types_aiobotocore_ssm_incidents/__main__.py`

 * *Files 15% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.SSMIncidents 2.5.2\nVersion:         2.5.2.post2\nBuilder"
+        "Type annotations for aiobotocore.SSMIncidents 2.5.4\nVersion:         2.5.4\nBuilder"
         " version: 7.17.2\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm_incidents//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-incidents.html#SSMIncidents\nOther"
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

### Comparing `types-aiobotocore-ssm-incidents-2.5.2.post2/types_aiobotocore_ssm_incidents/client.py` & `types-aiobotocore-ssm-incidents-2.5.4/types_aiobotocore_ssm_incidents/client.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-ssm-incidents-2.5.2.post2/types_aiobotocore_ssm_incidents/client.pyi` & `types-aiobotocore-ssm-incidents-2.5.4/types_aiobotocore_ssm_incidents/client.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-ssm-incidents-2.5.2.post2/types_aiobotocore_ssm_incidents/literals.py` & `types-aiobotocore-ssm-incidents-2.5.4/types_aiobotocore_ssm_incidents/literals.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-ssm-incidents-2.5.2.post2/types_aiobotocore_ssm_incidents/literals.pyi` & `types-aiobotocore-ssm-incidents-2.5.4/types_aiobotocore_ssm_incidents/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-ssm-incidents-2.5.2.post2/types_aiobotocore_ssm_incidents/paginator.py` & `types-aiobotocore-ssm-incidents-2.5.4/types_aiobotocore_ssm_incidents/paginator.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-ssm-incidents-2.5.2.post2/types_aiobotocore_ssm_incidents/paginator.pyi` & `types-aiobotocore-ssm-incidents-2.5.4/types_aiobotocore_ssm_incidents/paginator.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-ssm-incidents-2.5.2.post2/types_aiobotocore_ssm_incidents/type_defs.py` & `types-aiobotocore-ssm-incidents-2.5.4/types_aiobotocore_ssm_incidents/type_defs.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-ssm-incidents-2.5.2.post2/types_aiobotocore_ssm_incidents/type_defs.pyi` & `types-aiobotocore-ssm-incidents-2.5.4/types_aiobotocore_ssm_incidents/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-ssm-incidents-2.5.2.post2/types_aiobotocore_ssm_incidents/waiter.py` & `types-aiobotocore-ssm-incidents-2.5.4/types_aiobotocore_ssm_incidents/waiter.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-ssm-incidents-2.5.2.post2/types_aiobotocore_ssm_incidents/waiter.pyi` & `types-aiobotocore-ssm-incidents-2.5.4/types_aiobotocore_ssm_incidents/waiter.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-ssm-incidents-2.5.2.post2/types_aiobotocore_ssm_incidents.egg-info/PKG-INFO` & `types-aiobotocore-ssm-incidents-2.5.4/types_aiobotocore_ssm_incidents.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-ssm-incidents
-Version: 2.5.2.post2
-Summary: Type annotations for aiobotocore.SSMIncidents 2.5.2 service generated with mypy-boto3-builder 7.17.2
+Version: 2.5.4
+Summary: Type annotations for aiobotocore.SSMIncidents 2.5.4 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm_incidents/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-ssm-incidents.svg?color=blue)](https://pypi.org/project/types-aiobotocore-ssm-incidents)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm_incidents/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-ssm-incidents)](https://pepy.tech/project/types-aiobotocore-ssm-incidents)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.SSMIncidents 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-incidents.html#SSMIncidents)
+[aiobotocore.SSMIncidents 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-incidents.html#SSMIncidents)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-ssm-incidents-2.5.2.post2/types_aiobotocore_ssm_incidents.egg-info/SOURCES.txt` & `types-aiobotocore-ssm-incidents-2.5.4/types_aiobotocore_ssm_incidents.egg-info/SOURCES.txt`

 * *Files identical despite different names*


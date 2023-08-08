# Comparing `tmp/types-aiobotocore-license-manager-2.5.2.post2.tar.gz` & `tmp/types-aiobotocore-license-manager-2.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-license-manager-2.5.2.post2.tar", last modified: Fri Aug  4 13:59:15 2023, max compression
+gzip compressed data, was "types-aiobotocore-license-manager-2.5.4.tar", last modified: Tue Aug  8 01:24:00 2023, max compression
```

## Comparing `types-aiobotocore-license-manager-2.5.2.post2.tar` & `types-aiobotocore-license-manager-2.5.4.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:15.256643 types-aiobotocore-license-manager-2.5.2.post2/
--rw-r--r--   0 vlad      (1000) vlad      (1000)     1070 2023-08-04 13:42:57.000000 types-aiobotocore-license-manager-2.5.2.post2/LICENSE
--rw-r--r--   0 vlad      (1000) vlad      (1000)    14347 2023-08-04 13:59:15.256643 types-aiobotocore-license-manager-2.5.2.post2/PKG-INFO
--rw-r--r--   0 vlad      (1000) vlad      (1000)    12798 2023-08-04 13:42:57.000000 types-aiobotocore-license-manager-2.5.2.post2/README.md
--rw-r--r--   0 vlad      (1000) vlad      (1000)       38 2023-08-04 13:59:15.256643 types-aiobotocore-license-manager-2.5.2.post2/setup.cfg
--rw-r--r--   0 vlad      (1000) vlad      (1000)     2127 2023-08-04 13:42:57.000000 types-aiobotocore-license-manager-2.5.2.post2/setup.py
-drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:15.256643 types-aiobotocore-license-manager-2.5.2.post2/types_aiobotocore_license_manager/
--rw-r--r--   0 vlad      (1000) vlad      (1000)     2010 2023-08-04 13:42:57.000000 types-aiobotocore-license-manager-2.5.2.post2/types_aiobotocore_license_manager/__init__.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)     2009 2023-08-04 13:42:57.000000 types-aiobotocore-license-manager-2.5.2.post2/types_aiobotocore_license_manager/__init__.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)      973 2023-08-04 13:42:57.000000 types-aiobotocore-license-manager-2.5.2.post2/types_aiobotocore_license_manager/__main__.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)    43066 2023-08-04 13:42:58.000000 types-aiobotocore-license-manager-2.5.2.post2/types_aiobotocore_license_manager/client.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)    43002 2023-08-04 13:42:58.000000 types-aiobotocore-license-manager-2.5.2.post2/types_aiobotocore_license_manager/client.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)    12487 2023-08-04 13:42:58.000000 types-aiobotocore-license-manager-2.5.2.post2/types_aiobotocore_license_manager/literals.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)    12485 2023-08-04 13:42:58.000000 types-aiobotocore-license-manager-2.5.2.post2/types_aiobotocore_license_manager/literals.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)     7931 2023-08-04 13:42:58.000000 types-aiobotocore-license-manager-2.5.2.post2/types_aiobotocore_license_manager/paginator.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)     7924 2023-08-04 13:42:58.000000 types-aiobotocore-license-manager-2.5.2.post2/types_aiobotocore_license_manager/paginator.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:42:57.000000 types-aiobotocore-license-manager-2.5.2.post2/types_aiobotocore_license_manager/py.typed
--rw-r--r--   0 vlad      (1000) vlad      (1000)    55079 2023-08-04 13:42:59.000000 types-aiobotocore-license-manager-2.5.2.post2/types_aiobotocore_license_manager/type_defs.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)    55008 2023-08-04 13:42:59.000000 types-aiobotocore-license-manager-2.5.2.post2/types_aiobotocore_license_manager/type_defs.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)       65 2023-08-04 13:42:57.000000 types-aiobotocore-license-manager-2.5.2.post2/types_aiobotocore_license_manager/version.py
-drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:15.256643 types-aiobotocore-license-manager-2.5.2.post2/types_aiobotocore_license_manager.egg-info/
--rw-r--r--   0 vlad      (1000) vlad      (1000)    14347 2023-08-04 13:59:15.000000 types-aiobotocore-license-manager-2.5.2.post2/types_aiobotocore_license_manager.egg-info/PKG-INFO
--rw-r--r--   0 vlad      (1000) vlad      (1000)      965 2023-08-04 13:59:15.000000 types-aiobotocore-license-manager-2.5.2.post2/types_aiobotocore_license_manager.egg-info/SOURCES.txt
--rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:15.000000 types-aiobotocore-license-manager-2.5.2.post2/types_aiobotocore_license_manager.egg-info/dependency_links.txt
--rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:15.000000 types-aiobotocore-license-manager-2.5.2.post2/types_aiobotocore_license_manager.egg-info/not-zip-safe
--rw-r--r--   0 vlad      (1000) vlad      (1000)       52 2023-08-04 13:59:15.000000 types-aiobotocore-license-manager-2.5.2.post2/types_aiobotocore_license_manager.egg-info/requires.txt
--rw-r--r--   0 vlad      (1000) vlad      (1000)       34 2023-08-04 13:59:15.000000 types-aiobotocore-license-manager-2.5.2.post2/types_aiobotocore_license_manager.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:23:59.986722 types-aiobotocore-license-manager-2.5.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-08 01:14:12.000000 types-aiobotocore-license-manager-2.5.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    14341 2023-08-08 01:23:59.986722 types-aiobotocore-license-manager-2.5.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    12798 2023-08-08 01:14:12.000000 types-aiobotocore-license-manager-2.5.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-08 01:23:59.986722 types-aiobotocore-license-manager-2.5.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2121 2023-08-08 01:14:12.000000 types-aiobotocore-license-manager-2.5.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:23:59.986722 types-aiobotocore-license-manager-2.5.4/types_aiobotocore_license_manager/
+-rw-r--r--   0 runner    (1001) docker     (123)     2010 2023-08-08 01:14:12.000000 types-aiobotocore-license-manager-2.5.4/types_aiobotocore_license_manager/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2009 2023-08-08 01:14:12.000000 types-aiobotocore-license-manager-2.5.4/types_aiobotocore_license_manager/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      961 2023-08-08 01:14:12.000000 types-aiobotocore-license-manager-2.5.4/types_aiobotocore_license_manager/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    43066 2023-08-08 01:14:13.000000 types-aiobotocore-license-manager-2.5.4/types_aiobotocore_license_manager/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    43002 2023-08-08 01:14:13.000000 types-aiobotocore-license-manager-2.5.4/types_aiobotocore_license_manager/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    12487 2023-08-08 01:14:13.000000 types-aiobotocore-license-manager-2.5.4/types_aiobotocore_license_manager/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12485 2023-08-08 01:14:13.000000 types-aiobotocore-license-manager-2.5.4/types_aiobotocore_license_manager/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     7931 2023-08-08 01:14:13.000000 types-aiobotocore-license-manager-2.5.4/types_aiobotocore_license_manager/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7924 2023-08-08 01:14:13.000000 types-aiobotocore-license-manager-2.5.4/types_aiobotocore_license_manager/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 01:14:12.000000 types-aiobotocore-license-manager-2.5.4/types_aiobotocore_license_manager/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    55079 2023-08-08 01:14:14.000000 types-aiobotocore-license-manager-2.5.4/types_aiobotocore_license_manager/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    55008 2023-08-08 01:14:13.000000 types-aiobotocore-license-manager-2.5.4/types_aiobotocore_license_manager/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-08-08 01:14:12.000000 types-aiobotocore-license-manager-2.5.4/types_aiobotocore_license_manager/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:23:59.986722 types-aiobotocore-license-manager-2.5.4/types_aiobotocore_license_manager.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    14341 2023-08-08 01:23:59.000000 types-aiobotocore-license-manager-2.5.4/types_aiobotocore_license_manager.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      965 2023-08-08 01:23:59.000000 types-aiobotocore-license-manager-2.5.4/types_aiobotocore_license_manager.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 01:23:59.000000 types-aiobotocore-license-manager-2.5.4/types_aiobotocore_license_manager.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 01:23:59.000000 types-aiobotocore-license-manager-2.5.4/types_aiobotocore_license_manager.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-08 01:23:59.000000 types-aiobotocore-license-manager-2.5.4/types_aiobotocore_license_manager.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-08-08 01:23:59.000000 types-aiobotocore-license-manager-2.5.4/types_aiobotocore_license_manager.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-license-manager-2.5.2.post2/LICENSE` & `types-aiobotocore-license-manager-2.5.4/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-license-manager-2.5.2.post2/PKG-INFO` & `types-aiobotocore-license-manager-2.5.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-license-manager
-Version: 2.5.2.post2
-Summary: Type annotations for aiobotocore.LicenseManager 2.5.2 service generated with mypy-boto3-builder 7.17.2
+Version: 2.5.4
+Summary: Type annotations for aiobotocore.LicenseManager 2.5.4 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_license_manager/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-license-manager.svg?color=blue)](https://pypi.org/project/types-aiobotocore-license-manager)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_license_manager/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-license-manager)](https://pepy.tech/project/types-aiobotocore-license-manager)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.LicenseManager 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/license-manager.html#LicenseManager)
+[aiobotocore.LicenseManager 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/license-manager.html#LicenseManager)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-license-manager-2.5.2.post2/README.md` & `types-aiobotocore-license-manager-2.5.4/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-license-manager.svg?color=blue)](https://pypi.org/project/types-aiobotocore-license-manager)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_license_manager/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-license-manager)](https://pepy.tech/project/types-aiobotocore-license-manager)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.LicenseManager 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/license-manager.html#LicenseManager)
+[aiobotocore.LicenseManager 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/license-manager.html#LicenseManager)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-license-manager-2.5.2.post2/setup.py` & `types-aiobotocore-license-manager-2.5.4/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-license-manager",
-    version="2.5.2.post2",
+    version="2.5.4",
     packages=["types_aiobotocore_license_manager"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.LicenseManager 2.5.2 service generated with"
+        "Type annotations for aiobotocore.LicenseManager 2.5.4 service generated with"
         " mypy-boto3-builder 7.17.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
```

### Comparing `types-aiobotocore-license-manager-2.5.2.post2/types_aiobotocore_license_manager/__init__.py` & `types-aiobotocore-license-manager-2.5.4/types_aiobotocore_license_manager/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-license-manager-2.5.2.post2/types_aiobotocore_license_manager/__init__.pyi` & `types-aiobotocore-license-manager-2.5.4/types_aiobotocore_license_manager/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-license-manager-2.5.2.post2/types_aiobotocore_license_manager/__main__.py` & `types-aiobotocore-license-manager-2.5.4/types_aiobotocore_license_manager/__main__.py`

 * *Files 21% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.LicenseManager 2.5.2\nVersion:        "
-        " 2.5.2.post2\nBuilder version: 7.17.2\nDocs:           "
+        "Type annotations for aiobotocore.LicenseManager 2.5.4\nVersion:         2.5.4\nBuilder"
+        " version: 7.17.2\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_license_manager//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/license-manager.html#LicenseManager\nOther"
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

### Comparing `types-aiobotocore-license-manager-2.5.2.post2/types_aiobotocore_license_manager/client.py` & `types-aiobotocore-license-manager-2.5.4/types_aiobotocore_license_manager/client.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-license-manager-2.5.2.post2/types_aiobotocore_license_manager/client.pyi` & `types-aiobotocore-license-manager-2.5.4/types_aiobotocore_license_manager/client.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-license-manager-2.5.2.post2/types_aiobotocore_license_manager/literals.py` & `types-aiobotocore-license-manager-2.5.4/types_aiobotocore_license_manager/literals.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-license-manager-2.5.2.post2/types_aiobotocore_license_manager/literals.pyi` & `types-aiobotocore-license-manager-2.5.4/types_aiobotocore_license_manager/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-license-manager-2.5.2.post2/types_aiobotocore_license_manager/paginator.py` & `types-aiobotocore-license-manager-2.5.4/types_aiobotocore_license_manager/paginator.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-license-manager-2.5.2.post2/types_aiobotocore_license_manager/paginator.pyi` & `types-aiobotocore-license-manager-2.5.4/types_aiobotocore_license_manager/paginator.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-license-manager-2.5.2.post2/types_aiobotocore_license_manager/type_defs.py` & `types-aiobotocore-license-manager-2.5.4/types_aiobotocore_license_manager/type_defs.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-license-manager-2.5.2.post2/types_aiobotocore_license_manager/type_defs.pyi` & `types-aiobotocore-license-manager-2.5.4/types_aiobotocore_license_manager/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-license-manager-2.5.2.post2/types_aiobotocore_license_manager.egg-info/PKG-INFO` & `types-aiobotocore-license-manager-2.5.4/types_aiobotocore_license_manager.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-license-manager
-Version: 2.5.2.post2
-Summary: Type annotations for aiobotocore.LicenseManager 2.5.2 service generated with mypy-boto3-builder 7.17.2
+Version: 2.5.4
+Summary: Type annotations for aiobotocore.LicenseManager 2.5.4 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_license_manager/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-license-manager.svg?color=blue)](https://pypi.org/project/types-aiobotocore-license-manager)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_license_manager/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-license-manager)](https://pepy.tech/project/types-aiobotocore-license-manager)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.LicenseManager 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/license-manager.html#LicenseManager)
+[aiobotocore.LicenseManager 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/license-manager.html#LicenseManager)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-license-manager-2.5.2.post2/types_aiobotocore_license_manager.egg-info/SOURCES.txt` & `types-aiobotocore-license-manager-2.5.4/types_aiobotocore_license_manager.egg-info/SOURCES.txt`

 * *Files identical despite different names*


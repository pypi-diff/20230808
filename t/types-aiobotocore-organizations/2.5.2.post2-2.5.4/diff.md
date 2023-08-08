# Comparing `tmp/types-aiobotocore-organizations-2.5.2.post2.tar.gz` & `tmp/types-aiobotocore-organizations-2.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-organizations-2.5.2.post2.tar", last modified: Fri Aug  4 13:59:20 2023, max compression
+gzip compressed data, was "types-aiobotocore-organizations-2.5.4.tar", last modified: Tue Aug  8 01:24:11 2023, max compression
```

## Comparing `types-aiobotocore-organizations-2.5.2.post2.tar` & `types-aiobotocore-organizations-2.5.4.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:20.276643 types-aiobotocore-organizations-2.5.2.post2/
--rw-r--r--   0 vlad      (1000) vlad      (1000)     1070 2023-08-04 13:46:13.000000 types-aiobotocore-organizations-2.5.2.post2/LICENSE
--rw-r--r--   0 vlad      (1000) vlad      (1000)    15860 2023-08-04 13:59:20.276643 types-aiobotocore-organizations-2.5.2.post2/PKG-INFO
--rw-r--r--   0 vlad      (1000) vlad      (1000)    14318 2023-08-04 13:46:13.000000 types-aiobotocore-organizations-2.5.2.post2/README.md
--rw-r--r--   0 vlad      (1000) vlad      (1000)       38 2023-08-04 13:59:20.276643 types-aiobotocore-organizations-2.5.2.post2/setup.cfg
--rw-r--r--   0 vlad      (1000) vlad      (1000)     2114 2023-08-04 13:46:13.000000 types-aiobotocore-organizations-2.5.2.post2/setup.py
-drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:20.276643 types-aiobotocore-organizations-2.5.2.post2/types_aiobotocore_organizations/
--rw-r--r--   0 vlad      (1000) vlad      (1000)     4303 2023-08-04 13:46:13.000000 types-aiobotocore-organizations-2.5.2.post2/types_aiobotocore_organizations/__init__.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)     4302 2023-08-04 13:46:13.000000 types-aiobotocore-organizations-2.5.2.post2/types_aiobotocore_organizations/__init__.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)      967 2023-08-04 13:46:13.000000 types-aiobotocore-organizations-2.5.2.post2/types_aiobotocore_organizations/__main__.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)    49679 2023-08-04 13:46:14.000000 types-aiobotocore-organizations-2.5.2.post2/types_aiobotocore_organizations/client.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)    49599 2023-08-04 13:46:13.000000 types-aiobotocore-organizations-2.5.2.post2/types_aiobotocore_organizations/client.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)    12356 2023-08-04 13:46:14.000000 types-aiobotocore-organizations-2.5.2.post2/types_aiobotocore_organizations/literals.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)    12354 2023-08-04 13:46:14.000000 types-aiobotocore-organizations-2.5.2.post2/types_aiobotocore_organizations/literals.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)    20503 2023-08-04 13:46:14.000000 types-aiobotocore-organizations-2.5.2.post2/types_aiobotocore_organizations/paginator.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)    20485 2023-08-04 13:46:14.000000 types-aiobotocore-organizations-2.5.2.post2/types_aiobotocore_organizations/paginator.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:46:13.000000 types-aiobotocore-organizations-2.5.2.post2/types_aiobotocore_organizations/py.typed
--rw-r--r--   0 vlad      (1000) vlad      (1000)    44300 2023-08-04 13:46:17.000000 types-aiobotocore-organizations-2.5.2.post2/types_aiobotocore_organizations/type_defs.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)    44245 2023-08-04 13:46:16.000000 types-aiobotocore-organizations-2.5.2.post2/types_aiobotocore_organizations/type_defs.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)       65 2023-08-04 13:46:13.000000 types-aiobotocore-organizations-2.5.2.post2/types_aiobotocore_organizations/version.py
-drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:20.276643 types-aiobotocore-organizations-2.5.2.post2/types_aiobotocore_organizations.egg-info/
--rw-r--r--   0 vlad      (1000) vlad      (1000)    15860 2023-08-04 13:59:20.000000 types-aiobotocore-organizations-2.5.2.post2/types_aiobotocore_organizations.egg-info/PKG-INFO
--rw-r--r--   0 vlad      (1000) vlad      (1000)      927 2023-08-04 13:59:20.000000 types-aiobotocore-organizations-2.5.2.post2/types_aiobotocore_organizations.egg-info/SOURCES.txt
--rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:20.000000 types-aiobotocore-organizations-2.5.2.post2/types_aiobotocore_organizations.egg-info/dependency_links.txt
--rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:20.000000 types-aiobotocore-organizations-2.5.2.post2/types_aiobotocore_organizations.egg-info/not-zip-safe
--rw-r--r--   0 vlad      (1000) vlad      (1000)       52 2023-08-04 13:59:20.000000 types-aiobotocore-organizations-2.5.2.post2/types_aiobotocore_organizations.egg-info/requires.txt
--rw-r--r--   0 vlad      (1000) vlad      (1000)       32 2023-08-04 13:59:20.000000 types-aiobotocore-organizations-2.5.2.post2/types_aiobotocore_organizations.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:24:11.466745 types-aiobotocore-organizations-2.5.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-08 01:16:19.000000 types-aiobotocore-organizations-2.5.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    15854 2023-08-08 01:24:11.466745 types-aiobotocore-organizations-2.5.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    14318 2023-08-08 01:16:19.000000 types-aiobotocore-organizations-2.5.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-08 01:24:11.466745 types-aiobotocore-organizations-2.5.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2108 2023-08-08 01:16:19.000000 types-aiobotocore-organizations-2.5.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:24:11.466745 types-aiobotocore-organizations-2.5.4/types_aiobotocore_organizations/
+-rw-r--r--   0 runner    (1001) docker     (123)     4303 2023-08-08 01:16:19.000000 types-aiobotocore-organizations-2.5.4/types_aiobotocore_organizations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4302 2023-08-08 01:16:19.000000 types-aiobotocore-organizations-2.5.4/types_aiobotocore_organizations/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      955 2023-08-08 01:16:19.000000 types-aiobotocore-organizations-2.5.4/types_aiobotocore_organizations/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    49679 2023-08-08 01:16:19.000000 types-aiobotocore-organizations-2.5.4/types_aiobotocore_organizations/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    49599 2023-08-08 01:16:19.000000 types-aiobotocore-organizations-2.5.4/types_aiobotocore_organizations/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    12356 2023-08-08 01:16:19.000000 types-aiobotocore-organizations-2.5.4/types_aiobotocore_organizations/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12354 2023-08-08 01:16:19.000000 types-aiobotocore-organizations-2.5.4/types_aiobotocore_organizations/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    20503 2023-08-08 01:16:19.000000 types-aiobotocore-organizations-2.5.4/types_aiobotocore_organizations/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20485 2023-08-08 01:16:19.000000 types-aiobotocore-organizations-2.5.4/types_aiobotocore_organizations/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 01:16:19.000000 types-aiobotocore-organizations-2.5.4/types_aiobotocore_organizations/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    44300 2023-08-08 01:16:20.000000 types-aiobotocore-organizations-2.5.4/types_aiobotocore_organizations/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    44245 2023-08-08 01:16:20.000000 types-aiobotocore-organizations-2.5.4/types_aiobotocore_organizations/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-08-08 01:16:19.000000 types-aiobotocore-organizations-2.5.4/types_aiobotocore_organizations/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:24:11.466745 types-aiobotocore-organizations-2.5.4/types_aiobotocore_organizations.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    15854 2023-08-08 01:24:11.000000 types-aiobotocore-organizations-2.5.4/types_aiobotocore_organizations.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      927 2023-08-08 01:24:11.000000 types-aiobotocore-organizations-2.5.4/types_aiobotocore_organizations.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 01:24:11.000000 types-aiobotocore-organizations-2.5.4/types_aiobotocore_organizations.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 01:24:11.000000 types-aiobotocore-organizations-2.5.4/types_aiobotocore_organizations.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-08 01:24:11.000000 types-aiobotocore-organizations-2.5.4/types_aiobotocore_organizations.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-08-08 01:24:11.000000 types-aiobotocore-organizations-2.5.4/types_aiobotocore_organizations.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-organizations-2.5.2.post2/LICENSE` & `types-aiobotocore-organizations-2.5.4/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-organizations-2.5.2.post2/PKG-INFO` & `types-aiobotocore-organizations-2.5.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-organizations
-Version: 2.5.2.post2
-Summary: Type annotations for aiobotocore.Organizations 2.5.2 service generated with mypy-boto3-builder 7.17.2
+Version: 2.5.4
+Summary: Type annotations for aiobotocore.Organizations 2.5.4 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_organizations/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-organizations.svg?color=blue)](https://pypi.org/project/types-aiobotocore-organizations)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_organizations/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-organizations)](https://pepy.tech/project/types-aiobotocore-organizations)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.Organizations 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/organizations.html#Organizations)
+[aiobotocore.Organizations 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/organizations.html#Organizations)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-organizations-2.5.2.post2/README.md` & `types-aiobotocore-organizations-2.5.4/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-organizations.svg?color=blue)](https://pypi.org/project/types-aiobotocore-organizations)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_organizations/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-organizations)](https://pepy.tech/project/types-aiobotocore-organizations)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.Organizations 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/organizations.html#Organizations)
+[aiobotocore.Organizations 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/organizations.html#Organizations)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-organizations-2.5.2.post2/setup.py` & `types-aiobotocore-organizations-2.5.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-organizations",
-    version="2.5.2.post2",
+    version="2.5.4",
     packages=["types_aiobotocore_organizations"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.Organizations 2.5.2 service generated with"
+        "Type annotations for aiobotocore.Organizations 2.5.4 service generated with"
         " mypy-boto3-builder 7.17.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
```

### Comparing `types-aiobotocore-organizations-2.5.2.post2/types_aiobotocore_organizations/__init__.py` & `types-aiobotocore-organizations-2.5.4/types_aiobotocore_organizations/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-organizations-2.5.2.post2/types_aiobotocore_organizations/__init__.pyi` & `types-aiobotocore-organizations-2.5.4/types_aiobotocore_organizations/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-organizations-2.5.2.post2/types_aiobotocore_organizations/client.py` & `types-aiobotocore-organizations-2.5.4/types_aiobotocore_organizations/client.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-organizations-2.5.2.post2/types_aiobotocore_organizations/client.pyi` & `types-aiobotocore-organizations-2.5.4/types_aiobotocore_organizations/client.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-organizations-2.5.2.post2/types_aiobotocore_organizations/literals.py` & `types-aiobotocore-organizations-2.5.4/types_aiobotocore_organizations/literals.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-organizations-2.5.2.post2/types_aiobotocore_organizations/literals.pyi` & `types-aiobotocore-organizations-2.5.4/types_aiobotocore_organizations/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-organizations-2.5.2.post2/types_aiobotocore_organizations/paginator.py` & `types-aiobotocore-organizations-2.5.4/types_aiobotocore_organizations/paginator.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-organizations-2.5.2.post2/types_aiobotocore_organizations/paginator.pyi` & `types-aiobotocore-organizations-2.5.4/types_aiobotocore_organizations/paginator.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-organizations-2.5.2.post2/types_aiobotocore_organizations/type_defs.py` & `types-aiobotocore-organizations-2.5.4/types_aiobotocore_organizations/type_defs.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-organizations-2.5.2.post2/types_aiobotocore_organizations/type_defs.pyi` & `types-aiobotocore-organizations-2.5.4/types_aiobotocore_organizations/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-organizations-2.5.2.post2/types_aiobotocore_organizations.egg-info/PKG-INFO` & `types-aiobotocore-organizations-2.5.4/types_aiobotocore_organizations.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-organizations
-Version: 2.5.2.post2
-Summary: Type annotations for aiobotocore.Organizations 2.5.2 service generated with mypy-boto3-builder 7.17.2
+Version: 2.5.4
+Summary: Type annotations for aiobotocore.Organizations 2.5.4 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_organizations/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-organizations.svg?color=blue)](https://pypi.org/project/types-aiobotocore-organizations)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_organizations/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-organizations)](https://pepy.tech/project/types-aiobotocore-organizations)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.Organizations 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/organizations.html#Organizations)
+[aiobotocore.Organizations 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/organizations.html#Organizations)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-organizations-2.5.2.post2/types_aiobotocore_organizations.egg-info/SOURCES.txt` & `types-aiobotocore-organizations-2.5.4/types_aiobotocore_organizations.egg-info/SOURCES.txt`

 * *Files identical despite different names*


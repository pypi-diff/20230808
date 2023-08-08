# Comparing `tmp/types-aiobotocore-waf-regional-2.5.2.post2.tar.gz` & `tmp/types-aiobotocore-waf-regional-2.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-waf-regional-2.5.2.post2.tar", last modified: Fri Aug  4 13:59:29 2023, max compression
+gzip compressed data, was "types-aiobotocore-waf-regional-2.5.4.tar", last modified: Tue Aug  8 01:24:34 2023, max compression
```

## Comparing `types-aiobotocore-waf-regional-2.5.2.post2.tar` & `types-aiobotocore-waf-regional-2.5.4.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:29.576643 types-aiobotocore-waf-regional-2.5.2.post2/
--rw-r--r--   0 vlad      (1000) vlad      (1000)     1070 2023-08-04 13:55:40.000000 types-aiobotocore-waf-regional-2.5.2.post2/LICENSE
--rw-r--r--   0 vlad      (1000) vlad      (1000)    12436 2023-08-04 13:59:29.576643 types-aiobotocore-waf-regional-2.5.2.post2/PKG-INFO
--rw-r--r--   0 vlad      (1000) vlad      (1000)    10899 2023-08-04 13:55:40.000000 types-aiobotocore-waf-regional-2.5.2.post2/README.md
--rw-r--r--   0 vlad      (1000) vlad      (1000)       38 2023-08-04 13:59:29.576643 types-aiobotocore-waf-regional-2.5.2.post2/setup.cfg
--rw-r--r--   0 vlad      (1000) vlad      (1000)     2106 2023-08-04 13:55:39.000000 types-aiobotocore-waf-regional-2.5.2.post2/setup.py
-drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:29.576643 types-aiobotocore-waf-regional-2.5.2.post2/types_aiobotocore_waf_regional/
--rw-r--r--   0 vlad      (1000) vlad      (1000)      477 2023-08-04 13:55:40.000000 types-aiobotocore-waf-regional-2.5.2.post2/types_aiobotocore_waf_regional/__init__.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)      476 2023-08-04 13:55:40.000000 types-aiobotocore-waf-regional-2.5.2.post2/types_aiobotocore_waf_regional/__init__.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)      961 2023-08-04 13:55:40.000000 types-aiobotocore-waf-regional-2.5.2.post2/types_aiobotocore_waf_regional/__main__.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)    49296 2023-08-04 13:55:40.000000 types-aiobotocore-waf-regional-2.5.2.post2/types_aiobotocore_waf_regional/client.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)    49206 2023-08-04 13:55:40.000000 types-aiobotocore-waf-regional-2.5.2.post2/types_aiobotocore_waf_regional/client.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)    12238 2023-08-04 13:55:40.000000 types-aiobotocore-waf-regional-2.5.2.post2/types_aiobotocore_waf_regional/literals.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)    12236 2023-08-04 13:55:40.000000 types-aiobotocore-waf-regional-2.5.2.post2/types_aiobotocore_waf_regional/literals.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:55:40.000000 types-aiobotocore-waf-regional-2.5.2.post2/types_aiobotocore_waf_regional/py.typed
--rw-r--r--   0 vlad      (1000) vlad      (1000)    55412 2023-08-04 13:55:42.000000 types-aiobotocore-waf-regional-2.5.2.post2/types_aiobotocore_waf_regional/type_defs.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)    55365 2023-08-04 13:55:41.000000 types-aiobotocore-waf-regional-2.5.2.post2/types_aiobotocore_waf_regional/type_defs.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)       65 2023-08-04 13:55:40.000000 types-aiobotocore-waf-regional-2.5.2.post2/types_aiobotocore_waf_regional/version.py
-drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:29.576643 types-aiobotocore-waf-regional-2.5.2.post2/types_aiobotocore_waf_regional.egg-info/
--rw-r--r--   0 vlad      (1000) vlad      (1000)    12436 2023-08-04 13:59:29.000000 types-aiobotocore-waf-regional-2.5.2.post2/types_aiobotocore_waf_regional.egg-info/PKG-INFO
--rw-r--r--   0 vlad      (1000) vlad      (1000)      819 2023-08-04 13:59:29.000000 types-aiobotocore-waf-regional-2.5.2.post2/types_aiobotocore_waf_regional.egg-info/SOURCES.txt
--rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:29.000000 types-aiobotocore-waf-regional-2.5.2.post2/types_aiobotocore_waf_regional.egg-info/dependency_links.txt
--rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:29.000000 types-aiobotocore-waf-regional-2.5.2.post2/types_aiobotocore_waf_regional.egg-info/not-zip-safe
--rw-r--r--   0 vlad      (1000) vlad      (1000)       52 2023-08-04 13:59:29.000000 types-aiobotocore-waf-regional-2.5.2.post2/types_aiobotocore_waf_regional.egg-info/requires.txt
--rw-r--r--   0 vlad      (1000) vlad      (1000)       31 2023-08-04 13:59:29.000000 types-aiobotocore-waf-regional-2.5.2.post2/types_aiobotocore_waf_regional.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:24:34.798801 types-aiobotocore-waf-regional-2.5.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-08 01:22:22.000000 types-aiobotocore-waf-regional-2.5.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    12430 2023-08-08 01:24:34.798801 types-aiobotocore-waf-regional-2.5.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10899 2023-08-08 01:22:22.000000 types-aiobotocore-waf-regional-2.5.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-08 01:24:34.798801 types-aiobotocore-waf-regional-2.5.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2100 2023-08-08 01:22:22.000000 types-aiobotocore-waf-regional-2.5.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:24:34.798801 types-aiobotocore-waf-regional-2.5.4/types_aiobotocore_waf_regional/
+-rw-r--r--   0 runner    (1001) docker     (123)      477 2023-08-08 01:22:22.000000 types-aiobotocore-waf-regional-2.5.4/types_aiobotocore_waf_regional/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      476 2023-08-08 01:22:22.000000 types-aiobotocore-waf-regional-2.5.4/types_aiobotocore_waf_regional/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      949 2023-08-08 01:22:22.000000 types-aiobotocore-waf-regional-2.5.4/types_aiobotocore_waf_regional/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    49296 2023-08-08 01:22:22.000000 types-aiobotocore-waf-regional-2.5.4/types_aiobotocore_waf_regional/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    49206 2023-08-08 01:22:22.000000 types-aiobotocore-waf-regional-2.5.4/types_aiobotocore_waf_regional/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    12238 2023-08-08 01:22:23.000000 types-aiobotocore-waf-regional-2.5.4/types_aiobotocore_waf_regional/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12236 2023-08-08 01:22:22.000000 types-aiobotocore-waf-regional-2.5.4/types_aiobotocore_waf_regional/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 01:22:22.000000 types-aiobotocore-waf-regional-2.5.4/types_aiobotocore_waf_regional/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    55412 2023-08-08 01:22:24.000000 types-aiobotocore-waf-regional-2.5.4/types_aiobotocore_waf_regional/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    55365 2023-08-08 01:22:23.000000 types-aiobotocore-waf-regional-2.5.4/types_aiobotocore_waf_regional/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-08-08 01:22:22.000000 types-aiobotocore-waf-regional-2.5.4/types_aiobotocore_waf_regional/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:24:34.798801 types-aiobotocore-waf-regional-2.5.4/types_aiobotocore_waf_regional.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    12430 2023-08-08 01:24:34.000000 types-aiobotocore-waf-regional-2.5.4/types_aiobotocore_waf_regional.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      819 2023-08-08 01:24:34.000000 types-aiobotocore-waf-regional-2.5.4/types_aiobotocore_waf_regional.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 01:24:34.000000 types-aiobotocore-waf-regional-2.5.4/types_aiobotocore_waf_regional.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 01:24:34.000000 types-aiobotocore-waf-regional-2.5.4/types_aiobotocore_waf_regional.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-08 01:24:34.000000 types-aiobotocore-waf-regional-2.5.4/types_aiobotocore_waf_regional.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-08-08 01:24:34.000000 types-aiobotocore-waf-regional-2.5.4/types_aiobotocore_waf_regional.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-waf-regional-2.5.2.post2/LICENSE` & `types-aiobotocore-waf-regional-2.5.4/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-waf-regional-2.5.2.post2/PKG-INFO` & `types-aiobotocore-waf-regional-2.5.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-waf-regional
-Version: 2.5.2.post2
-Summary: Type annotations for aiobotocore.WAFRegional 2.5.2 service generated with mypy-boto3-builder 7.17.2
+Version: 2.5.4
+Summary: Type annotations for aiobotocore.WAFRegional 2.5.4 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_waf_regional/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-waf-regional.svg?color=blue)](https://pypi.org/project/types-aiobotocore-waf-regional)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_waf_regional/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-waf-regional)](https://pepy.tech/project/types-aiobotocore-waf-regional)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.WAFRegional 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/waf-regional.html#WAFRegional)
+[aiobotocore.WAFRegional 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/waf-regional.html#WAFRegional)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-waf-regional-2.5.2.post2/README.md` & `types-aiobotocore-waf-regional-2.5.4/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-waf-regional.svg?color=blue)](https://pypi.org/project/types-aiobotocore-waf-regional)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_waf_regional/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-waf-regional)](https://pepy.tech/project/types-aiobotocore-waf-regional)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.WAFRegional 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/waf-regional.html#WAFRegional)
+[aiobotocore.WAFRegional 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/waf-regional.html#WAFRegional)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-waf-regional-2.5.2.post2/setup.py` & `types-aiobotocore-waf-regional-2.5.4/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-waf-regional",
-    version="2.5.2.post2",
+    version="2.5.4",
     packages=["types_aiobotocore_waf_regional"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.WAFRegional 2.5.2 service generated with"
+        "Type annotations for aiobotocore.WAFRegional 2.5.4 service generated with"
         " mypy-boto3-builder 7.17.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
```

### Comparing `types-aiobotocore-waf-regional-2.5.2.post2/types_aiobotocore_waf_regional/client.py` & `types-aiobotocore-waf-regional-2.5.4/types_aiobotocore_waf_regional/client.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-waf-regional-2.5.2.post2/types_aiobotocore_waf_regional/client.pyi` & `types-aiobotocore-waf-regional-2.5.4/types_aiobotocore_waf_regional/client.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-waf-regional-2.5.2.post2/types_aiobotocore_waf_regional/literals.py` & `types-aiobotocore-waf-regional-2.5.4/types_aiobotocore_waf_regional/literals.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-waf-regional-2.5.2.post2/types_aiobotocore_waf_regional/literals.pyi` & `types-aiobotocore-waf-regional-2.5.4/types_aiobotocore_waf_regional/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-waf-regional-2.5.2.post2/types_aiobotocore_waf_regional/type_defs.py` & `types-aiobotocore-waf-regional-2.5.4/types_aiobotocore_waf_regional/type_defs.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-waf-regional-2.5.2.post2/types_aiobotocore_waf_regional/type_defs.pyi` & `types-aiobotocore-waf-regional-2.5.4/types_aiobotocore_waf_regional/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-waf-regional-2.5.2.post2/types_aiobotocore_waf_regional.egg-info/PKG-INFO` & `types-aiobotocore-waf-regional-2.5.4/types_aiobotocore_waf_regional.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-waf-regional
-Version: 2.5.2.post2
-Summary: Type annotations for aiobotocore.WAFRegional 2.5.2 service generated with mypy-boto3-builder 7.17.2
+Version: 2.5.4
+Summary: Type annotations for aiobotocore.WAFRegional 2.5.4 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_waf_regional/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-waf-regional.svg?color=blue)](https://pypi.org/project/types-aiobotocore-waf-regional)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_waf_regional/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-waf-regional)](https://pepy.tech/project/types-aiobotocore-waf-regional)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.WAFRegional 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/waf-regional.html#WAFRegional)
+[aiobotocore.WAFRegional 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/waf-regional.html#WAFRegional)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-waf-regional-2.5.2.post2/types_aiobotocore_waf_regional.egg-info/SOURCES.txt` & `types-aiobotocore-waf-regional-2.5.4/types_aiobotocore_waf_regional.egg-info/SOURCES.txt`

 * *Files identical despite different names*


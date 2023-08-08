# Comparing `tmp/types-aiobotocore-service-quotas-2.5.2.post2.tar.gz` & `tmp/types-aiobotocore-service-quotas-2.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-service-quotas-2.5.2.post2.tar", last modified: Fri Aug  4 13:59:25 2023, max compression
+gzip compressed data, was "types-aiobotocore-service-quotas-2.5.4.tar", last modified: Tue Aug  8 01:24:25 2023, max compression
```

## Comparing `types-aiobotocore-service-quotas-2.5.2.post2.tar` & `types-aiobotocore-service-quotas-2.5.4.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:25.936643 types-aiobotocore-service-quotas-2.5.2.post2/
--rw-r--r--   0 vlad      (1000) vlad      (1000)     1070 2023-08-04 13:53:15.000000 types-aiobotocore-service-quotas-2.5.2.post2/LICENSE
--rw-r--r--   0 vlad      (1000) vlad      (1000)    14527 2023-08-04 13:59:25.936643 types-aiobotocore-service-quotas-2.5.2.post2/PKG-INFO
--rw-r--r--   0 vlad      (1000) vlad      (1000)    12982 2023-08-04 13:53:15.000000 types-aiobotocore-service-quotas-2.5.2.post2/README.md
--rw-r--r--   0 vlad      (1000) vlad      (1000)       38 2023-08-04 13:59:25.936643 types-aiobotocore-service-quotas-2.5.2.post2/setup.cfg
--rw-r--r--   0 vlad      (1000) vlad      (1000)     2120 2023-08-04 13:53:15.000000 types-aiobotocore-service-quotas-2.5.2.post2/setup.py
-drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:25.936643 types-aiobotocore-service-quotas-2.5.2.post2/types_aiobotocore_service_quotas/
--rw-r--r--   0 vlad      (1000) vlad      (1000)     2292 2023-08-04 13:53:15.000000 types-aiobotocore-service-quotas-2.5.2.post2/types_aiobotocore_service_quotas/__init__.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)     2291 2023-08-04 13:53:15.000000 types-aiobotocore-service-quotas-2.5.2.post2/types_aiobotocore_service_quotas/__init__.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)      969 2023-08-04 13:53:15.000000 types-aiobotocore-service-quotas-2.5.2.post2/types_aiobotocore_service_quotas/__main__.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)    21026 2023-08-04 13:53:15.000000 types-aiobotocore-service-quotas-2.5.2.post2/types_aiobotocore_service_quotas/client.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)    20992 2023-08-04 13:53:15.000000 types-aiobotocore-service-quotas-2.5.2.post2/types_aiobotocore_service_quotas/client.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)     9967 2023-08-04 13:53:15.000000 types-aiobotocore-service-quotas-2.5.2.post2/types_aiobotocore_service_quotas/literals.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)     9965 2023-08-04 13:53:15.000000 types-aiobotocore-service-quotas-2.5.2.post2/types_aiobotocore_service_quotas/literals.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)     9127 2023-08-04 13:53:15.000000 types-aiobotocore-service-quotas-2.5.2.post2/types_aiobotocore_service_quotas/paginator.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)     9119 2023-08-04 13:53:15.000000 types-aiobotocore-service-quotas-2.5.2.post2/types_aiobotocore_service_quotas/paginator.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:53:15.000000 types-aiobotocore-service-quotas-2.5.2.post2/types_aiobotocore_service_quotas/py.typed
--rw-r--r--   0 vlad      (1000) vlad      (1000)    17540 2023-08-04 13:53:16.000000 types-aiobotocore-service-quotas-2.5.2.post2/types_aiobotocore_service_quotas/type_defs.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)    17527 2023-08-04 13:53:16.000000 types-aiobotocore-service-quotas-2.5.2.post2/types_aiobotocore_service_quotas/type_defs.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)       65 2023-08-04 13:53:15.000000 types-aiobotocore-service-quotas-2.5.2.post2/types_aiobotocore_service_quotas/version.py
-drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:25.936643 types-aiobotocore-service-quotas-2.5.2.post2/types_aiobotocore_service_quotas.egg-info/
--rw-r--r--   0 vlad      (1000) vlad      (1000)    14527 2023-08-04 13:59:25.000000 types-aiobotocore-service-quotas-2.5.2.post2/types_aiobotocore_service_quotas.egg-info/PKG-INFO
--rw-r--r--   0 vlad      (1000) vlad      (1000)      946 2023-08-04 13:59:25.000000 types-aiobotocore-service-quotas-2.5.2.post2/types_aiobotocore_service_quotas.egg-info/SOURCES.txt
--rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:25.000000 types-aiobotocore-service-quotas-2.5.2.post2/types_aiobotocore_service_quotas.egg-info/dependency_links.txt
--rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:25.000000 types-aiobotocore-service-quotas-2.5.2.post2/types_aiobotocore_service_quotas.egg-info/not-zip-safe
--rw-r--r--   0 vlad      (1000) vlad      (1000)       52 2023-08-04 13:59:25.000000 types-aiobotocore-service-quotas-2.5.2.post2/types_aiobotocore_service_quotas.egg-info/requires.txt
--rw-r--r--   0 vlad      (1000) vlad      (1000)       33 2023-08-04 13:59:25.000000 types-aiobotocore-service-quotas-2.5.2.post2/types_aiobotocore_service_quotas.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:24:25.870779 types-aiobotocore-service-quotas-2.5.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-08 01:20:55.000000 types-aiobotocore-service-quotas-2.5.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    14521 2023-08-08 01:24:25.870779 types-aiobotocore-service-quotas-2.5.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    12982 2023-08-08 01:20:55.000000 types-aiobotocore-service-quotas-2.5.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-08 01:24:25.870779 types-aiobotocore-service-quotas-2.5.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2114 2023-08-08 01:20:55.000000 types-aiobotocore-service-quotas-2.5.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:24:25.870779 types-aiobotocore-service-quotas-2.5.4/types_aiobotocore_service_quotas/
+-rw-r--r--   0 runner    (1001) docker     (123)     2292 2023-08-08 01:20:55.000000 types-aiobotocore-service-quotas-2.5.4/types_aiobotocore_service_quotas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2291 2023-08-08 01:20:55.000000 types-aiobotocore-service-quotas-2.5.4/types_aiobotocore_service_quotas/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      957 2023-08-08 01:20:55.000000 types-aiobotocore-service-quotas-2.5.4/types_aiobotocore_service_quotas/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21026 2023-08-08 01:20:55.000000 types-aiobotocore-service-quotas-2.5.4/types_aiobotocore_service_quotas/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20992 2023-08-08 01:20:55.000000 types-aiobotocore-service-quotas-2.5.4/types_aiobotocore_service_quotas/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9967 2023-08-08 01:20:55.000000 types-aiobotocore-service-quotas-2.5.4/types_aiobotocore_service_quotas/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9965 2023-08-08 01:20:55.000000 types-aiobotocore-service-quotas-2.5.4/types_aiobotocore_service_quotas/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9127 2023-08-08 01:20:55.000000 types-aiobotocore-service-quotas-2.5.4/types_aiobotocore_service_quotas/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9119 2023-08-08 01:20:55.000000 types-aiobotocore-service-quotas-2.5.4/types_aiobotocore_service_quotas/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 01:20:55.000000 types-aiobotocore-service-quotas-2.5.4/types_aiobotocore_service_quotas/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    17540 2023-08-08 01:20:56.000000 types-aiobotocore-service-quotas-2.5.4/types_aiobotocore_service_quotas/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17527 2023-08-08 01:20:56.000000 types-aiobotocore-service-quotas-2.5.4/types_aiobotocore_service_quotas/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-08-08 01:20:55.000000 types-aiobotocore-service-quotas-2.5.4/types_aiobotocore_service_quotas/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:24:25.870779 types-aiobotocore-service-quotas-2.5.4/types_aiobotocore_service_quotas.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    14521 2023-08-08 01:24:25.000000 types-aiobotocore-service-quotas-2.5.4/types_aiobotocore_service_quotas.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      946 2023-08-08 01:24:25.000000 types-aiobotocore-service-quotas-2.5.4/types_aiobotocore_service_quotas.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 01:24:25.000000 types-aiobotocore-service-quotas-2.5.4/types_aiobotocore_service_quotas.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 01:24:25.000000 types-aiobotocore-service-quotas-2.5.4/types_aiobotocore_service_quotas.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-08 01:24:25.000000 types-aiobotocore-service-quotas-2.5.4/types_aiobotocore_service_quotas.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-08-08 01:24:25.000000 types-aiobotocore-service-quotas-2.5.4/types_aiobotocore_service_quotas.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-service-quotas-2.5.2.post2/LICENSE` & `types-aiobotocore-service-quotas-2.5.4/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-service-quotas-2.5.2.post2/PKG-INFO` & `types-aiobotocore-service-quotas-2.5.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-service-quotas
-Version: 2.5.2.post2
-Summary: Type annotations for aiobotocore.ServiceQuotas 2.5.2 service generated with mypy-boto3-builder 7.17.2
+Version: 2.5.4
+Summary: Type annotations for aiobotocore.ServiceQuotas 2.5.4 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_service_quotas/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-service-quotas.svg?color=blue)](https://pypi.org/project/types-aiobotocore-service-quotas)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_service_quotas/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-service-quotas)](https://pepy.tech/project/types-aiobotocore-service-quotas)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.ServiceQuotas 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/service-quotas.html#ServiceQuotas)
+[aiobotocore.ServiceQuotas 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/service-quotas.html#ServiceQuotas)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-service-quotas-2.5.2.post2/README.md` & `types-aiobotocore-service-quotas-2.5.4/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-service-quotas.svg?color=blue)](https://pypi.org/project/types-aiobotocore-service-quotas)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_service_quotas/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-service-quotas)](https://pepy.tech/project/types-aiobotocore-service-quotas)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.ServiceQuotas 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/service-quotas.html#ServiceQuotas)
+[aiobotocore.ServiceQuotas 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/service-quotas.html#ServiceQuotas)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-service-quotas-2.5.2.post2/setup.py` & `types-aiobotocore-service-quotas-2.5.4/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-service-quotas",
-    version="2.5.2.post2",
+    version="2.5.4",
     packages=["types_aiobotocore_service_quotas"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.ServiceQuotas 2.5.2 service generated with"
+        "Type annotations for aiobotocore.ServiceQuotas 2.5.4 service generated with"
         " mypy-boto3-builder 7.17.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
```

### Comparing `types-aiobotocore-service-quotas-2.5.2.post2/types_aiobotocore_service_quotas/__init__.py` & `types-aiobotocore-service-quotas-2.5.4/types_aiobotocore_service_quotas/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-service-quotas-2.5.2.post2/types_aiobotocore_service_quotas/__init__.pyi` & `types-aiobotocore-service-quotas-2.5.4/types_aiobotocore_service_quotas/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-service-quotas-2.5.2.post2/types_aiobotocore_service_quotas/__main__.py` & `types-aiobotocore-service-quotas-2.5.4/types_aiobotocore_service_quotas/__main__.py`

 * *Files 9% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.ServiceQuotas 2.5.2\nVersion:        "
-        " 2.5.2.post2\nBuilder version: 7.17.2\nDocs:           "
+        "Type annotations for aiobotocore.ServiceQuotas 2.5.4\nVersion:         2.5.4\nBuilder"
+        " version: 7.17.2\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_service_quotas//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/service-quotas.html#ServiceQuotas\nOther"
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

### Comparing `types-aiobotocore-service-quotas-2.5.2.post2/types_aiobotocore_service_quotas/client.py` & `types-aiobotocore-service-quotas-2.5.4/types_aiobotocore_service_quotas/client.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-service-quotas-2.5.2.post2/types_aiobotocore_service_quotas/client.pyi` & `types-aiobotocore-service-quotas-2.5.4/types_aiobotocore_service_quotas/client.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-service-quotas-2.5.2.post2/types_aiobotocore_service_quotas/literals.py` & `types-aiobotocore-service-quotas-2.5.4/types_aiobotocore_service_quotas/literals.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-service-quotas-2.5.2.post2/types_aiobotocore_service_quotas/literals.pyi` & `types-aiobotocore-service-quotas-2.5.4/types_aiobotocore_service_quotas/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-service-quotas-2.5.2.post2/types_aiobotocore_service_quotas/paginator.py` & `types-aiobotocore-service-quotas-2.5.4/types_aiobotocore_service_quotas/paginator.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-service-quotas-2.5.2.post2/types_aiobotocore_service_quotas/paginator.pyi` & `types-aiobotocore-service-quotas-2.5.4/types_aiobotocore_service_quotas/paginator.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-service-quotas-2.5.2.post2/types_aiobotocore_service_quotas/type_defs.py` & `types-aiobotocore-service-quotas-2.5.4/types_aiobotocore_service_quotas/type_defs.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-service-quotas-2.5.2.post2/types_aiobotocore_service_quotas/type_defs.pyi` & `types-aiobotocore-service-quotas-2.5.4/types_aiobotocore_service_quotas/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-service-quotas-2.5.2.post2/types_aiobotocore_service_quotas.egg-info/PKG-INFO` & `types-aiobotocore-service-quotas-2.5.4/types_aiobotocore_service_quotas.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-service-quotas
-Version: 2.5.2.post2
-Summary: Type annotations for aiobotocore.ServiceQuotas 2.5.2 service generated with mypy-boto3-builder 7.17.2
+Version: 2.5.4
+Summary: Type annotations for aiobotocore.ServiceQuotas 2.5.4 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_service_quotas/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-service-quotas.svg?color=blue)](https://pypi.org/project/types-aiobotocore-service-quotas)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_service_quotas/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-service-quotas)](https://pepy.tech/project/types-aiobotocore-service-quotas)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.ServiceQuotas 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/service-quotas.html#ServiceQuotas)
+[aiobotocore.ServiceQuotas 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/service-quotas.html#ServiceQuotas)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-service-quotas-2.5.2.post2/types_aiobotocore_service_quotas.egg-info/SOURCES.txt` & `types-aiobotocore-service-quotas-2.5.4/types_aiobotocore_service_quotas.egg-info/SOURCES.txt`

 * *Files identical despite different names*


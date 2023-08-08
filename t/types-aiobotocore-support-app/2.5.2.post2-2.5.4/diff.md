# Comparing `tmp/types-aiobotocore-support-app-2.5.2.post2.tar.gz` & `tmp/types-aiobotocore-support-app-2.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-support-app-2.5.2.post2.tar", last modified: Fri Aug  4 13:59:28 2023, max compression
+gzip compressed data, was "types-aiobotocore-support-app-2.5.4.tar", last modified: Tue Aug  8 01:24:31 2023, max compression
```

## Comparing `types-aiobotocore-support-app-2.5.2.post2.tar` & `types-aiobotocore-support-app-2.5.4.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:28.386643 types-aiobotocore-support-app-2.5.2.post2/
--rw-r--r--   0 vlad      (1000) vlad      (1000)     1070 2023-08-04 13:54:50.000000 types-aiobotocore-support-app-2.5.2.post2/LICENSE
--rw-r--r--   0 vlad      (1000) vlad      (1000)    12456 2023-08-04 13:59:28.386643 types-aiobotocore-support-app-2.5.2.post2/PKG-INFO
--rw-r--r--   0 vlad      (1000) vlad      (1000)    10923 2023-08-04 13:54:50.000000 types-aiobotocore-support-app-2.5.2.post2/README.md
--rw-r--r--   0 vlad      (1000) vlad      (1000)       38 2023-08-04 13:59:28.386643 types-aiobotocore-support-app-2.5.2.post2/setup.cfg
--rw-r--r--   0 vlad      (1000) vlad      (1000)     2099 2023-08-04 13:54:49.000000 types-aiobotocore-support-app-2.5.2.post2/setup.py
-drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:28.376643 types-aiobotocore-support-app-2.5.2.post2/types_aiobotocore_support_app/
--rw-r--r--   0 vlad      (1000) vlad      (1000)      469 2023-08-04 13:54:50.000000 types-aiobotocore-support-app-2.5.2.post2/types_aiobotocore_support_app/__init__.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)      468 2023-08-04 13:54:50.000000 types-aiobotocore-support-app-2.5.2.post2/types_aiobotocore_support_app/__init__.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)      957 2023-08-04 13:54:50.000000 types-aiobotocore-support-app-2.5.2.post2/types_aiobotocore_support_app/__main__.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)    10743 2023-08-04 13:54:50.000000 types-aiobotocore-support-app-2.5.2.post2/types_aiobotocore_support_app/client.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)    10725 2023-08-04 13:54:50.000000 types-aiobotocore-support-app-2.5.2.post2/types_aiobotocore_support_app/client.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)     7885 2023-08-04 13:54:50.000000 types-aiobotocore-support-app-2.5.2.post2/types_aiobotocore_support_app/literals.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)     7883 2023-08-04 13:54:50.000000 types-aiobotocore-support-app-2.5.2.post2/types_aiobotocore_support_app/literals.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:54:50.000000 types-aiobotocore-support-app-2.5.2.post2/types_aiobotocore_support_app/py.typed
--rw-r--r--   0 vlad      (1000) vlad      (1000)     7155 2023-08-04 13:54:50.000000 types-aiobotocore-support-app-2.5.2.post2/types_aiobotocore_support_app/type_defs.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)     7146 2023-08-04 13:54:50.000000 types-aiobotocore-support-app-2.5.2.post2/types_aiobotocore_support_app/type_defs.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)       65 2023-08-04 13:54:50.000000 types-aiobotocore-support-app-2.5.2.post2/types_aiobotocore_support_app/version.py
-drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:28.386643 types-aiobotocore-support-app-2.5.2.post2/types_aiobotocore_support_app.egg-info/
--rw-r--r--   0 vlad      (1000) vlad      (1000)    12456 2023-08-04 13:59:28.000000 types-aiobotocore-support-app-2.5.2.post2/types_aiobotocore_support_app.egg-info/PKG-INFO
--rw-r--r--   0 vlad      (1000) vlad      (1000)      802 2023-08-04 13:59:28.000000 types-aiobotocore-support-app-2.5.2.post2/types_aiobotocore_support_app.egg-info/SOURCES.txt
--rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:28.000000 types-aiobotocore-support-app-2.5.2.post2/types_aiobotocore_support_app.egg-info/dependency_links.txt
--rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:28.000000 types-aiobotocore-support-app-2.5.2.post2/types_aiobotocore_support_app.egg-info/not-zip-safe
--rw-r--r--   0 vlad      (1000) vlad      (1000)       52 2023-08-04 13:59:28.000000 types-aiobotocore-support-app-2.5.2.post2/types_aiobotocore_support_app.egg-info/requires.txt
--rw-r--r--   0 vlad      (1000) vlad      (1000)       30 2023-08-04 13:59:28.000000 types-aiobotocore-support-app-2.5.2.post2/types_aiobotocore_support_app.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:24:31.882794 types-aiobotocore-support-app-2.5.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-08 01:21:53.000000 types-aiobotocore-support-app-2.5.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    12450 2023-08-08 01:24:31.882794 types-aiobotocore-support-app-2.5.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10923 2023-08-08 01:21:53.000000 types-aiobotocore-support-app-2.5.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-08 01:24:31.882794 types-aiobotocore-support-app-2.5.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2093 2023-08-08 01:21:53.000000 types-aiobotocore-support-app-2.5.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:24:31.874794 types-aiobotocore-support-app-2.5.4/types_aiobotocore_support_app/
+-rw-r--r--   0 runner    (1001) docker     (123)      469 2023-08-08 01:21:53.000000 types-aiobotocore-support-app-2.5.4/types_aiobotocore_support_app/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      468 2023-08-08 01:21:53.000000 types-aiobotocore-support-app-2.5.4/types_aiobotocore_support_app/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      945 2023-08-08 01:21:53.000000 types-aiobotocore-support-app-2.5.4/types_aiobotocore_support_app/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10743 2023-08-08 01:21:53.000000 types-aiobotocore-support-app-2.5.4/types_aiobotocore_support_app/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10725 2023-08-08 01:21:53.000000 types-aiobotocore-support-app-2.5.4/types_aiobotocore_support_app/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     7885 2023-08-08 01:21:54.000000 types-aiobotocore-support-app-2.5.4/types_aiobotocore_support_app/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7883 2023-08-08 01:21:54.000000 types-aiobotocore-support-app-2.5.4/types_aiobotocore_support_app/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 01:21:53.000000 types-aiobotocore-support-app-2.5.4/types_aiobotocore_support_app/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     7155 2023-08-08 01:21:54.000000 types-aiobotocore-support-app-2.5.4/types_aiobotocore_support_app/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7146 2023-08-08 01:21:54.000000 types-aiobotocore-support-app-2.5.4/types_aiobotocore_support_app/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-08-08 01:21:53.000000 types-aiobotocore-support-app-2.5.4/types_aiobotocore_support_app/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:24:31.874794 types-aiobotocore-support-app-2.5.4/types_aiobotocore_support_app.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    12450 2023-08-08 01:24:31.000000 types-aiobotocore-support-app-2.5.4/types_aiobotocore_support_app.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      802 2023-08-08 01:24:31.000000 types-aiobotocore-support-app-2.5.4/types_aiobotocore_support_app.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 01:24:31.000000 types-aiobotocore-support-app-2.5.4/types_aiobotocore_support_app.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 01:24:31.000000 types-aiobotocore-support-app-2.5.4/types_aiobotocore_support_app.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-08 01:24:31.000000 types-aiobotocore-support-app-2.5.4/types_aiobotocore_support_app.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-08-08 01:24:31.000000 types-aiobotocore-support-app-2.5.4/types_aiobotocore_support_app.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-support-app-2.5.2.post2/LICENSE` & `types-aiobotocore-support-app-2.5.4/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-support-app-2.5.2.post2/PKG-INFO` & `types-aiobotocore-support-app-2.5.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-support-app
-Version: 2.5.2.post2
-Summary: Type annotations for aiobotocore.SupportApp 2.5.2 service generated with mypy-boto3-builder 7.17.2
+Version: 2.5.4
+Summary: Type annotations for aiobotocore.SupportApp 2.5.4 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_support_app/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-support-app.svg?color=blue)](https://pypi.org/project/types-aiobotocore-support-app)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_support_app/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-support-app)](https://pepy.tech/project/types-aiobotocore-support-app)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.SupportApp 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/support-app.html#SupportApp)
+[aiobotocore.SupportApp 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/support-app.html#SupportApp)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-support-app-2.5.2.post2/README.md` & `types-aiobotocore-support-app-2.5.4/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-support-app.svg?color=blue)](https://pypi.org/project/types-aiobotocore-support-app)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_support_app/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-support-app)](https://pepy.tech/project/types-aiobotocore-support-app)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.SupportApp 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/support-app.html#SupportApp)
+[aiobotocore.SupportApp 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/support-app.html#SupportApp)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-support-app-2.5.2.post2/setup.py` & `types-aiobotocore-support-app-2.5.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-support-app",
-    version="2.5.2.post2",
+    version="2.5.4",
     packages=["types_aiobotocore_support_app"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.SupportApp 2.5.2 service generated with"
+        "Type annotations for aiobotocore.SupportApp 2.5.4 service generated with"
         " mypy-boto3-builder 7.17.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
```

### Comparing `types-aiobotocore-support-app-2.5.2.post2/types_aiobotocore_support_app/__main__.py` & `types-aiobotocore-support-app-2.5.4/types_aiobotocore_support_app/__main__.py`

 * *Files 15% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.SupportApp 2.5.2\nVersion:         2.5.2.post2\nBuilder"
+        "Type annotations for aiobotocore.SupportApp 2.5.4\nVersion:         2.5.4\nBuilder"
         " version: 7.17.2\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_support_app//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/support-app.html#SupportApp\nOther"
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

### Comparing `types-aiobotocore-support-app-2.5.2.post2/types_aiobotocore_support_app/client.py` & `types-aiobotocore-support-app-2.5.4/types_aiobotocore_support_app/client.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-support-app-2.5.2.post2/types_aiobotocore_support_app/client.pyi` & `types-aiobotocore-support-app-2.5.4/types_aiobotocore_support_app/client.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-support-app-2.5.2.post2/types_aiobotocore_support_app/literals.py` & `types-aiobotocore-support-app-2.5.4/types_aiobotocore_support_app/literals.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-support-app-2.5.2.post2/types_aiobotocore_support_app/literals.pyi` & `types-aiobotocore-support-app-2.5.4/types_aiobotocore_support_app/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-support-app-2.5.2.post2/types_aiobotocore_support_app/type_defs.py` & `types-aiobotocore-support-app-2.5.4/types_aiobotocore_support_app/type_defs.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-support-app-2.5.2.post2/types_aiobotocore_support_app/type_defs.pyi` & `types-aiobotocore-support-app-2.5.4/types_aiobotocore_support_app/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-support-app-2.5.2.post2/types_aiobotocore_support_app.egg-info/PKG-INFO` & `types-aiobotocore-support-app-2.5.4/types_aiobotocore_support_app.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-support-app
-Version: 2.5.2.post2
-Summary: Type annotations for aiobotocore.SupportApp 2.5.2 service generated with mypy-boto3-builder 7.17.2
+Version: 2.5.4
+Summary: Type annotations for aiobotocore.SupportApp 2.5.4 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_support_app/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-support-app.svg?color=blue)](https://pypi.org/project/types-aiobotocore-support-app)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_support_app/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-support-app)](https://pepy.tech/project/types-aiobotocore-support-app)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.SupportApp 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/support-app.html#SupportApp)
+[aiobotocore.SupportApp 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/support-app.html#SupportApp)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-support-app-2.5.2.post2/types_aiobotocore_support_app.egg-info/SOURCES.txt` & `types-aiobotocore-support-app-2.5.4/types_aiobotocore_support_app.egg-info/SOURCES.txt`

 * *Files identical despite different names*


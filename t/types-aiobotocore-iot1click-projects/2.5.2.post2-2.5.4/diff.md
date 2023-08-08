# Comparing `tmp/types-aiobotocore-iot1click-projects-2.5.2.post2.tar.gz` & `tmp/types-aiobotocore-iot1click-projects-2.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-iot1click-projects-2.5.2.post2.tar", last modified: Fri Aug  4 13:59:11 2023, max compression
+gzip compressed data, was "types-aiobotocore-iot1click-projects-2.5.4.tar", last modified: Tue Aug  8 01:23:50 2023, max compression
```

## Comparing `types-aiobotocore-iot1click-projects-2.5.2.post2.tar` & `types-aiobotocore-iot1click-projects-2.5.4.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:11.236642 types-aiobotocore-iot1click-projects-2.5.2.post2/
--rw-r--r--   0 vlad      (1000) vlad      (1000)     1070 2023-08-04 13:40:51.000000 types-aiobotocore-iot1click-projects-2.5.2.post2/LICENSE
--rw-r--r--   0 vlad      (1000) vlad      (1000)    13747 2023-08-04 13:59:11.236642 types-aiobotocore-iot1click-projects-2.5.2.post2/PKG-INFO
--rw-r--r--   0 vlad      (1000) vlad      (1000)    12186 2023-08-04 13:40:51.000000 types-aiobotocore-iot1click-projects-2.5.2.post2/README.md
--rw-r--r--   0 vlad      (1000) vlad      (1000)       38 2023-08-04 13:59:11.236642 types-aiobotocore-iot1click-projects-2.5.2.post2/setup.cfg
--rw-r--r--   0 vlad      (1000) vlad      (1000)     2148 2023-08-04 13:40:51.000000 types-aiobotocore-iot1click-projects-2.5.2.post2/setup.py
-drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:11.236642 types-aiobotocore-iot1click-projects-2.5.2.post2/types_aiobotocore_iot1click_projects/
--rw-r--r--   0 vlad      (1000) vlad      (1000)      900 2023-08-04 13:40:51.000000 types-aiobotocore-iot1click-projects-2.5.2.post2/types_aiobotocore_iot1click_projects/__init__.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)      899 2023-08-04 13:40:51.000000 types-aiobotocore-iot1click-projects-2.5.2.post2/types_aiobotocore_iot1click_projects/__init__.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)      985 2023-08-04 13:40:51.000000 types-aiobotocore-iot1click-projects-2.5.2.post2/types_aiobotocore_iot1click_projects/__main__.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)    14748 2023-08-04 13:40:51.000000 types-aiobotocore-iot1click-projects-2.5.2.post2/types_aiobotocore_iot1click_projects/client.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)    14721 2023-08-04 13:40:51.000000 types-aiobotocore-iot1click-projects-2.5.2.post2/types_aiobotocore_iot1click_projects/client.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)     8133 2023-08-04 13:40:51.000000 types-aiobotocore-iot1click-projects-2.5.2.post2/types_aiobotocore_iot1click_projects/literals.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)     8131 2023-08-04 13:40:51.000000 types-aiobotocore-iot1click-projects-2.5.2.post2/types_aiobotocore_iot1click_projects/literals.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)     3242 2023-08-04 13:40:51.000000 types-aiobotocore-iot1click-projects-2.5.2.post2/types_aiobotocore_iot1click_projects/paginator.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)     3238 2023-08-04 13:40:51.000000 types-aiobotocore-iot1click-projects-2.5.2.post2/types_aiobotocore_iot1click_projects/paginator.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:40:51.000000 types-aiobotocore-iot1click-projects-2.5.2.post2/types_aiobotocore_iot1click_projects/py.typed
--rw-r--r--   0 vlad      (1000) vlad      (1000)    10882 2023-08-04 13:40:51.000000 types-aiobotocore-iot1click-projects-2.5.2.post2/types_aiobotocore_iot1click_projects/type_defs.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)    10865 2023-08-04 13:40:51.000000 types-aiobotocore-iot1click-projects-2.5.2.post2/types_aiobotocore_iot1click_projects/type_defs.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)       65 2023-08-04 13:40:51.000000 types-aiobotocore-iot1click-projects-2.5.2.post2/types_aiobotocore_iot1click_projects/version.py
-drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:11.236642 types-aiobotocore-iot1click-projects-2.5.2.post2/types_aiobotocore_iot1click_projects.egg-info/
--rw-r--r--   0 vlad      (1000) vlad      (1000)    13747 2023-08-04 13:59:11.000000 types-aiobotocore-iot1click-projects-2.5.2.post2/types_aiobotocore_iot1click_projects.egg-info/PKG-INFO
--rw-r--r--   0 vlad      (1000) vlad      (1000)     1022 2023-08-04 13:59:11.000000 types-aiobotocore-iot1click-projects-2.5.2.post2/types_aiobotocore_iot1click_projects.egg-info/SOURCES.txt
--rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:11.000000 types-aiobotocore-iot1click-projects-2.5.2.post2/types_aiobotocore_iot1click_projects.egg-info/dependency_links.txt
--rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:11.000000 types-aiobotocore-iot1click-projects-2.5.2.post2/types_aiobotocore_iot1click_projects.egg-info/not-zip-safe
--rw-r--r--   0 vlad      (1000) vlad      (1000)       52 2023-08-04 13:59:11.000000 types-aiobotocore-iot1click-projects-2.5.2.post2/types_aiobotocore_iot1click_projects.egg-info/requires.txt
--rw-r--r--   0 vlad      (1000) vlad      (1000)       37 2023-08-04 13:59:11.000000 types-aiobotocore-iot1click-projects-2.5.2.post2/types_aiobotocore_iot1click_projects.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:23:50.582734 types-aiobotocore-iot1click-projects-2.5.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-08 01:12:50.000000 types-aiobotocore-iot1click-projects-2.5.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    13741 2023-08-08 01:23:50.582734 types-aiobotocore-iot1click-projects-2.5.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    12186 2023-08-08 01:12:50.000000 types-aiobotocore-iot1click-projects-2.5.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-08 01:23:50.582734 types-aiobotocore-iot1click-projects-2.5.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2142 2023-08-08 01:12:50.000000 types-aiobotocore-iot1click-projects-2.5.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:23:50.582734 types-aiobotocore-iot1click-projects-2.5.4/types_aiobotocore_iot1click_projects/
+-rw-r--r--   0 runner    (1001) docker     (123)      900 2023-08-08 01:12:50.000000 types-aiobotocore-iot1click-projects-2.5.4/types_aiobotocore_iot1click_projects/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      899 2023-08-08 01:12:50.000000 types-aiobotocore-iot1click-projects-2.5.4/types_aiobotocore_iot1click_projects/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      973 2023-08-08 01:12:50.000000 types-aiobotocore-iot1click-projects-2.5.4/types_aiobotocore_iot1click_projects/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14748 2023-08-08 01:12:50.000000 types-aiobotocore-iot1click-projects-2.5.4/types_aiobotocore_iot1click_projects/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14721 2023-08-08 01:12:50.000000 types-aiobotocore-iot1click-projects-2.5.4/types_aiobotocore_iot1click_projects/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8133 2023-08-08 01:12:52.000000 types-aiobotocore-iot1click-projects-2.5.4/types_aiobotocore_iot1click_projects/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8131 2023-08-08 01:12:52.000000 types-aiobotocore-iot1click-projects-2.5.4/types_aiobotocore_iot1click_projects/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     3242 2023-08-08 01:12:52.000000 types-aiobotocore-iot1click-projects-2.5.4/types_aiobotocore_iot1click_projects/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3238 2023-08-08 01:12:50.000000 types-aiobotocore-iot1click-projects-2.5.4/types_aiobotocore_iot1click_projects/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 01:12:50.000000 types-aiobotocore-iot1click-projects-2.5.4/types_aiobotocore_iot1click_projects/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    10882 2023-08-08 01:12:52.000000 types-aiobotocore-iot1click-projects-2.5.4/types_aiobotocore_iot1click_projects/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10865 2023-08-08 01:12:52.000000 types-aiobotocore-iot1click-projects-2.5.4/types_aiobotocore_iot1click_projects/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-08-08 01:12:50.000000 types-aiobotocore-iot1click-projects-2.5.4/types_aiobotocore_iot1click_projects/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:23:50.582734 types-aiobotocore-iot1click-projects-2.5.4/types_aiobotocore_iot1click_projects.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    13741 2023-08-08 01:23:50.000000 types-aiobotocore-iot1click-projects-2.5.4/types_aiobotocore_iot1click_projects.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1022 2023-08-08 01:23:50.000000 types-aiobotocore-iot1click-projects-2.5.4/types_aiobotocore_iot1click_projects.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 01:23:50.000000 types-aiobotocore-iot1click-projects-2.5.4/types_aiobotocore_iot1click_projects.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 01:23:50.000000 types-aiobotocore-iot1click-projects-2.5.4/types_aiobotocore_iot1click_projects.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-08 01:23:50.000000 types-aiobotocore-iot1click-projects-2.5.4/types_aiobotocore_iot1click_projects.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-08-08 01:23:50.000000 types-aiobotocore-iot1click-projects-2.5.4/types_aiobotocore_iot1click_projects.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-iot1click-projects-2.5.2.post2/LICENSE` & `types-aiobotocore-iot1click-projects-2.5.4/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-iot1click-projects-2.5.2.post2/PKG-INFO` & `types-aiobotocore-iot1click-projects-2.5.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-iot1click-projects
-Version: 2.5.2.post2
-Summary: Type annotations for aiobotocore.IoT1ClickProjects 2.5.2 service generated with mypy-boto3-builder 7.17.2
+Version: 2.5.4
+Summary: Type annotations for aiobotocore.IoT1ClickProjects 2.5.4 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot1click_projects/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-iot1click-projects.svg?color=blue)](https://pypi.org/project/types-aiobotocore-iot1click-projects)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot1click_projects/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-iot1click-projects)](https://pepy.tech/project/types-aiobotocore-iot1click-projects)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.IoT1ClickProjects 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot1click-projects.html#IoT1ClickProjects)
+[aiobotocore.IoT1ClickProjects 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot1click-projects.html#IoT1ClickProjects)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-iot1click-projects-2.5.2.post2/README.md` & `types-aiobotocore-iot1click-projects-2.5.4/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-iot1click-projects.svg?color=blue)](https://pypi.org/project/types-aiobotocore-iot1click-projects)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot1click_projects/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-iot1click-projects)](https://pepy.tech/project/types-aiobotocore-iot1click-projects)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.IoT1ClickProjects 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot1click-projects.html#IoT1ClickProjects)
+[aiobotocore.IoT1ClickProjects 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot1click-projects.html#IoT1ClickProjects)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-iot1click-projects-2.5.2.post2/setup.py` & `types-aiobotocore-iot1click-projects-2.5.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-iot1click-projects",
-    version="2.5.2.post2",
+    version="2.5.4",
     packages=["types_aiobotocore_iot1click_projects"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.IoT1ClickProjects 2.5.2 service generated with"
+        "Type annotations for aiobotocore.IoT1ClickProjects 2.5.4 service generated with"
         " mypy-boto3-builder 7.17.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
```

### Comparing `types-aiobotocore-iot1click-projects-2.5.2.post2/types_aiobotocore_iot1click_projects/__init__.py` & `types-aiobotocore-iot1click-projects-2.5.4/types_aiobotocore_iot1click_projects/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-iot1click-projects-2.5.2.post2/types_aiobotocore_iot1click_projects/__init__.pyi` & `types-aiobotocore-iot1click-projects-2.5.4/types_aiobotocore_iot1click_projects/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-iot1click-projects-2.5.2.post2/types_aiobotocore_iot1click_projects/__main__.py` & `types-aiobotocore-iot1click-projects-2.5.4/types_aiobotocore_iot1click_projects/__main__.py`

 * *Files 17% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.IoT1ClickProjects 2.5.2\nVersion:        "
-        " 2.5.2.post2\nBuilder version: 7.17.2\nDocs:           "
+        "Type annotations for aiobotocore.IoT1ClickProjects 2.5.4\nVersion:         2.5.4\nBuilder"
+        " version: 7.17.2\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot1click_projects//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot1click-projects.html#IoT1ClickProjects\nOther"
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

### Comparing `types-aiobotocore-iot1click-projects-2.5.2.post2/types_aiobotocore_iot1click_projects/client.py` & `types-aiobotocore-iot1click-projects-2.5.4/types_aiobotocore_iot1click_projects/client.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-iot1click-projects-2.5.2.post2/types_aiobotocore_iot1click_projects/client.pyi` & `types-aiobotocore-iot1click-projects-2.5.4/types_aiobotocore_iot1click_projects/client.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-iot1click-projects-2.5.2.post2/types_aiobotocore_iot1click_projects/literals.py` & `types-aiobotocore-iot1click-projects-2.5.4/types_aiobotocore_iot1click_projects/literals.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-iot1click-projects-2.5.2.post2/types_aiobotocore_iot1click_projects/literals.pyi` & `types-aiobotocore-iot1click-projects-2.5.4/types_aiobotocore_iot1click_projects/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-iot1click-projects-2.5.2.post2/types_aiobotocore_iot1click_projects/paginator.py` & `types-aiobotocore-iot1click-projects-2.5.4/types_aiobotocore_iot1click_projects/paginator.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-iot1click-projects-2.5.2.post2/types_aiobotocore_iot1click_projects/paginator.pyi` & `types-aiobotocore-iot1click-projects-2.5.4/types_aiobotocore_iot1click_projects/paginator.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-iot1click-projects-2.5.2.post2/types_aiobotocore_iot1click_projects/type_defs.py` & `types-aiobotocore-iot1click-projects-2.5.4/types_aiobotocore_iot1click_projects/type_defs.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-iot1click-projects-2.5.2.post2/types_aiobotocore_iot1click_projects/type_defs.pyi` & `types-aiobotocore-iot1click-projects-2.5.4/types_aiobotocore_iot1click_projects/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-iot1click-projects-2.5.2.post2/types_aiobotocore_iot1click_projects.egg-info/PKG-INFO` & `types-aiobotocore-iot1click-projects-2.5.4/types_aiobotocore_iot1click_projects.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-iot1click-projects
-Version: 2.5.2.post2
-Summary: Type annotations for aiobotocore.IoT1ClickProjects 2.5.2 service generated with mypy-boto3-builder 7.17.2
+Version: 2.5.4
+Summary: Type annotations for aiobotocore.IoT1ClickProjects 2.5.4 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot1click_projects/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-iot1click-projects.svg?color=blue)](https://pypi.org/project/types-aiobotocore-iot1click-projects)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot1click_projects/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-iot1click-projects)](https://pepy.tech/project/types-aiobotocore-iot1click-projects)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.IoT1ClickProjects 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot1click-projects.html#IoT1ClickProjects)
+[aiobotocore.IoT1ClickProjects 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot1click-projects.html#IoT1ClickProjects)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-iot1click-projects-2.5.2.post2/types_aiobotocore_iot1click_projects.egg-info/SOURCES.txt` & `types-aiobotocore-iot1click-projects-2.5.4/types_aiobotocore_iot1click_projects.egg-info/SOURCES.txt`

 * *Files identical despite different names*


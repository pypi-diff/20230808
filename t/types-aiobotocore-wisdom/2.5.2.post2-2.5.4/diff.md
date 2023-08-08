# Comparing `tmp/types-aiobotocore-wisdom-2.5.2.post2.tar.gz` & `tmp/types-aiobotocore-wisdom-2.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-wisdom-2.5.2.post2.tar", last modified: Fri Aug  4 13:59:30 2023, max compression
+gzip compressed data, was "types-aiobotocore-wisdom-2.5.4.tar", last modified: Tue Aug  8 01:24:36 2023, max compression
```

## Comparing `types-aiobotocore-wisdom-2.5.2.post2.tar` & `types-aiobotocore-wisdom-2.5.4.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:30.076643 types-aiobotocore-wisdom-2.5.2.post2/
--rw-r--r--   0 vlad      (1000) vlad      (1000)     1070 2023-08-04 13:56:02.000000 types-aiobotocore-wisdom-2.5.2.post2/LICENSE
--rw-r--r--   0 vlad      (1000) vlad      (1000)    13871 2023-08-04 13:59:30.066643 types-aiobotocore-wisdom-2.5.2.post2/PKG-INFO
--rw-r--r--   0 vlad      (1000) vlad      (1000)    12343 2023-08-04 13:56:02.000000 types-aiobotocore-wisdom-2.5.2.post2/README.md
--rw-r--r--   0 vlad      (1000) vlad      (1000)       38 2023-08-04 13:59:30.076643 types-aiobotocore-wisdom-2.5.2.post2/setup.cfg
--rw-r--r--   0 vlad      (1000) vlad      (1000)     2079 2023-08-04 13:56:02.000000 types-aiobotocore-wisdom-2.5.2.post2/setup.py
-drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:30.066643 types-aiobotocore-wisdom-2.5.2.post2/types_aiobotocore_wisdom/
--rw-r--r--   0 vlad      (1000) vlad      (1000)     1949 2023-08-04 13:56:02.000000 types-aiobotocore-wisdom-2.5.2.post2/types_aiobotocore_wisdom/__init__.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)     1948 2023-08-04 13:56:02.000000 types-aiobotocore-wisdom-2.5.2.post2/types_aiobotocore_wisdom/__init__.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)      956 2023-08-04 13:56:02.000000 types-aiobotocore-wisdom-2.5.2.post2/types_aiobotocore_wisdom/__main__.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)    26939 2023-08-04 13:56:02.000000 types-aiobotocore-wisdom-2.5.2.post2/types_aiobotocore_wisdom/client.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)    26892 2023-08-04 13:56:02.000000 types-aiobotocore-wisdom-2.5.2.post2/types_aiobotocore_wisdom/client.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)     9967 2023-08-04 13:56:02.000000 types-aiobotocore-wisdom-2.5.2.post2/types_aiobotocore_wisdom/literals.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)     9965 2023-08-04 13:56:02.000000 types-aiobotocore-wisdom-2.5.2.post2/types_aiobotocore_wisdom/literals.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)     8962 2023-08-04 13:56:02.000000 types-aiobotocore-wisdom-2.5.2.post2/types_aiobotocore_wisdom/paginator.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)     8953 2023-08-04 13:56:02.000000 types-aiobotocore-wisdom-2.5.2.post2/types_aiobotocore_wisdom/paginator.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:56:02.000000 types-aiobotocore-wisdom-2.5.2.post2/types_aiobotocore_wisdom/py.typed
--rw-r--r--   0 vlad      (1000) vlad      (1000)    36192 2023-08-04 13:56:03.000000 types-aiobotocore-wisdom-2.5.2.post2/types_aiobotocore_wisdom/type_defs.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)    36131 2023-08-04 13:56:03.000000 types-aiobotocore-wisdom-2.5.2.post2/types_aiobotocore_wisdom/type_defs.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)       65 2023-08-04 13:56:02.000000 types-aiobotocore-wisdom-2.5.2.post2/types_aiobotocore_wisdom/version.py
-drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:30.066643 types-aiobotocore-wisdom-2.5.2.post2/types_aiobotocore_wisdom.egg-info/
--rw-r--r--   0 vlad      (1000) vlad      (1000)    13871 2023-08-04 13:59:29.000000 types-aiobotocore-wisdom-2.5.2.post2/types_aiobotocore_wisdom.egg-info/PKG-INFO
--rw-r--r--   0 vlad      (1000) vlad      (1000)      794 2023-08-04 13:59:30.000000 types-aiobotocore-wisdom-2.5.2.post2/types_aiobotocore_wisdom.egg-info/SOURCES.txt
--rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:29.000000 types-aiobotocore-wisdom-2.5.2.post2/types_aiobotocore_wisdom.egg-info/dependency_links.txt
--rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:29.000000 types-aiobotocore-wisdom-2.5.2.post2/types_aiobotocore_wisdom.egg-info/not-zip-safe
--rw-r--r--   0 vlad      (1000) vlad      (1000)       52 2023-08-04 13:59:29.000000 types-aiobotocore-wisdom-2.5.2.post2/types_aiobotocore_wisdom.egg-info/requires.txt
--rw-r--r--   0 vlad      (1000) vlad      (1000)       25 2023-08-04 13:59:29.000000 types-aiobotocore-wisdom-2.5.2.post2/types_aiobotocore_wisdom.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:24:36.050804 types-aiobotocore-wisdom-2.5.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-08 01:22:35.000000 types-aiobotocore-wisdom-2.5.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    13865 2023-08-08 01:24:36.050804 types-aiobotocore-wisdom-2.5.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    12343 2023-08-08 01:22:35.000000 types-aiobotocore-wisdom-2.5.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-08 01:24:36.050804 types-aiobotocore-wisdom-2.5.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2073 2023-08-08 01:22:35.000000 types-aiobotocore-wisdom-2.5.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:24:36.046804 types-aiobotocore-wisdom-2.5.4/types_aiobotocore_wisdom/
+-rw-r--r--   0 runner    (1001) docker     (123)     1949 2023-08-08 01:22:35.000000 types-aiobotocore-wisdom-2.5.4/types_aiobotocore_wisdom/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1948 2023-08-08 01:22:35.000000 types-aiobotocore-wisdom-2.5.4/types_aiobotocore_wisdom/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      944 2023-08-08 01:22:35.000000 types-aiobotocore-wisdom-2.5.4/types_aiobotocore_wisdom/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26939 2023-08-08 01:22:35.000000 types-aiobotocore-wisdom-2.5.4/types_aiobotocore_wisdom/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26892 2023-08-08 01:22:35.000000 types-aiobotocore-wisdom-2.5.4/types_aiobotocore_wisdom/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9967 2023-08-08 01:22:35.000000 types-aiobotocore-wisdom-2.5.4/types_aiobotocore_wisdom/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9965 2023-08-08 01:22:35.000000 types-aiobotocore-wisdom-2.5.4/types_aiobotocore_wisdom/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8962 2023-08-08 01:22:35.000000 types-aiobotocore-wisdom-2.5.4/types_aiobotocore_wisdom/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8953 2023-08-08 01:22:35.000000 types-aiobotocore-wisdom-2.5.4/types_aiobotocore_wisdom/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 01:22:35.000000 types-aiobotocore-wisdom-2.5.4/types_aiobotocore_wisdom/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    36192 2023-08-08 01:22:36.000000 types-aiobotocore-wisdom-2.5.4/types_aiobotocore_wisdom/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36131 2023-08-08 01:22:35.000000 types-aiobotocore-wisdom-2.5.4/types_aiobotocore_wisdom/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-08-08 01:22:35.000000 types-aiobotocore-wisdom-2.5.4/types_aiobotocore_wisdom/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:24:36.050804 types-aiobotocore-wisdom-2.5.4/types_aiobotocore_wisdom.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    13865 2023-08-08 01:24:35.000000 types-aiobotocore-wisdom-2.5.4/types_aiobotocore_wisdom.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      794 2023-08-08 01:24:35.000000 types-aiobotocore-wisdom-2.5.4/types_aiobotocore_wisdom.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 01:24:35.000000 types-aiobotocore-wisdom-2.5.4/types_aiobotocore_wisdom.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 01:24:35.000000 types-aiobotocore-wisdom-2.5.4/types_aiobotocore_wisdom.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-08 01:24:35.000000 types-aiobotocore-wisdom-2.5.4/types_aiobotocore_wisdom.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-08-08 01:24:35.000000 types-aiobotocore-wisdom-2.5.4/types_aiobotocore_wisdom.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-wisdom-2.5.2.post2/LICENSE` & `types-aiobotocore-wisdom-2.5.4/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-wisdom-2.5.2.post2/PKG-INFO` & `types-aiobotocore-wisdom-2.5.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-wisdom
-Version: 2.5.2.post2
-Summary: Type annotations for aiobotocore.ConnectWisdomService 2.5.2 service generated with mypy-boto3-builder 7.17.2
+Version: 2.5.4
+Summary: Type annotations for aiobotocore.ConnectWisdomService 2.5.4 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_wisdom/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-wisdom.svg?color=blue)](https://pypi.org/project/types-aiobotocore-wisdom)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_wisdom/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-wisdom)](https://pepy.tech/project/types-aiobotocore-wisdom)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.ConnectWisdomService 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wisdom.html#ConnectWisdomService)
+[aiobotocore.ConnectWisdomService 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wisdom.html#ConnectWisdomService)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-wisdom-2.5.2.post2/README.md` & `types-aiobotocore-wisdom-2.5.4/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-wisdom.svg?color=blue)](https://pypi.org/project/types-aiobotocore-wisdom)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_wisdom/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-wisdom)](https://pepy.tech/project/types-aiobotocore-wisdom)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.ConnectWisdomService 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wisdom.html#ConnectWisdomService)
+[aiobotocore.ConnectWisdomService 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wisdom.html#ConnectWisdomService)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-wisdom-2.5.2.post2/setup.py` & `types-aiobotocore-wisdom-2.5.4/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-wisdom",
-    version="2.5.2.post2",
+    version="2.5.4",
     packages=["types_aiobotocore_wisdom"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.ConnectWisdomService 2.5.2 service generated with"
+        "Type annotations for aiobotocore.ConnectWisdomService 2.5.4 service generated with"
         " mypy-boto3-builder 7.17.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
```

### Comparing `types-aiobotocore-wisdom-2.5.2.post2/types_aiobotocore_wisdom/__init__.py` & `types-aiobotocore-wisdom-2.5.4/types_aiobotocore_wisdom/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-wisdom-2.5.2.post2/types_aiobotocore_wisdom/__init__.pyi` & `types-aiobotocore-wisdom-2.5.4/types_aiobotocore_wisdom/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-wisdom-2.5.2.post2/types_aiobotocore_wisdom/__main__.py` & `types-aiobotocore-wisdom-2.5.4/types_aiobotocore_wisdom/__main__.py`

 * *Files 20% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.ConnectWisdomService 2.5.2\nVersion:        "
-        " 2.5.2.post2\nBuilder version: 7.17.2\nDocs:           "
+        "Type annotations for aiobotocore.ConnectWisdomService 2.5.4\nVersion:        "
+        " 2.5.4\nBuilder version: 7.17.2\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_wisdom//\nBoto3 docs: "
         "     https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wisdom.html#ConnectWisdomService\nOther"
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

### Comparing `types-aiobotocore-wisdom-2.5.2.post2/types_aiobotocore_wisdom/client.py` & `types-aiobotocore-wisdom-2.5.4/types_aiobotocore_wisdom/client.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-wisdom-2.5.2.post2/types_aiobotocore_wisdom/client.pyi` & `types-aiobotocore-wisdom-2.5.4/types_aiobotocore_wisdom/client.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-wisdom-2.5.2.post2/types_aiobotocore_wisdom/literals.py` & `types-aiobotocore-wisdom-2.5.4/types_aiobotocore_wisdom/literals.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-wisdom-2.5.2.post2/types_aiobotocore_wisdom/literals.pyi` & `types-aiobotocore-wisdom-2.5.4/types_aiobotocore_wisdom/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-wisdom-2.5.2.post2/types_aiobotocore_wisdom/paginator.py` & `types-aiobotocore-wisdom-2.5.4/types_aiobotocore_wisdom/paginator.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-wisdom-2.5.2.post2/types_aiobotocore_wisdom/paginator.pyi` & `types-aiobotocore-wisdom-2.5.4/types_aiobotocore_wisdom/paginator.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-wisdom-2.5.2.post2/types_aiobotocore_wisdom/type_defs.py` & `types-aiobotocore-wisdom-2.5.4/types_aiobotocore_wisdom/type_defs.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-wisdom-2.5.2.post2/types_aiobotocore_wisdom/type_defs.pyi` & `types-aiobotocore-wisdom-2.5.4/types_aiobotocore_wisdom/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-wisdom-2.5.2.post2/types_aiobotocore_wisdom.egg-info/PKG-INFO` & `types-aiobotocore-wisdom-2.5.4/types_aiobotocore_wisdom.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-wisdom
-Version: 2.5.2.post2
-Summary: Type annotations for aiobotocore.ConnectWisdomService 2.5.2 service generated with mypy-boto3-builder 7.17.2
+Version: 2.5.4
+Summary: Type annotations for aiobotocore.ConnectWisdomService 2.5.4 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_wisdom/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-wisdom.svg?color=blue)](https://pypi.org/project/types-aiobotocore-wisdom)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_wisdom/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-wisdom)](https://pepy.tech/project/types-aiobotocore-wisdom)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.ConnectWisdomService 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wisdom.html#ConnectWisdomService)
+[aiobotocore.ConnectWisdomService 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wisdom.html#ConnectWisdomService)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-wisdom-2.5.2.post2/types_aiobotocore_wisdom.egg-info/SOURCES.txt` & `types-aiobotocore-wisdom-2.5.4/types_aiobotocore_wisdom.egg-info/SOURCES.txt`

 * *Files identical despite different names*


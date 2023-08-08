# Comparing `tmp/types-aiobotocore-transcribe-2.5.2.post2.tar.gz` & `tmp/types-aiobotocore-transcribe-2.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-transcribe-2.5.2.post2.tar", last modified: Fri Aug  4 13:59:29 2023, max compression
+gzip compressed data, was "types-aiobotocore-transcribe-2.5.4.tar", last modified: Tue Aug  8 01:24:33 2023, max compression
```

## Comparing `types-aiobotocore-transcribe-2.5.2.post2.tar` & `types-aiobotocore-transcribe-2.5.4.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:29.176643 types-aiobotocore-transcribe-2.5.2.post2/
--rw-r--r--   0 vlad      (1000) vlad      (1000)     1070 2023-08-04 13:55:10.000000 types-aiobotocore-transcribe-2.5.2.post2/LICENSE
--rw-r--r--   0 vlad      (1000) vlad      (1000)    12414 2023-08-04 13:59:29.176643 types-aiobotocore-transcribe-2.5.2.post2/PKG-INFO
--rw-r--r--   0 vlad      (1000) vlad      (1000)    10877 2023-08-04 13:55:10.000000 types-aiobotocore-transcribe-2.5.2.post2/README.md
--rw-r--r--   0 vlad      (1000) vlad      (1000)       38 2023-08-04 13:59:29.176643 types-aiobotocore-transcribe-2.5.2.post2/setup.cfg
--rw-r--r--   0 vlad      (1000) vlad      (1000)     2100 2023-08-04 13:55:10.000000 types-aiobotocore-transcribe-2.5.2.post2/setup.py
-drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:29.176643 types-aiobotocore-transcribe-2.5.2.post2/types_aiobotocore_transcribe/
--rw-r--r--   0 vlad      (1000) vlad      (1000)      501 2023-08-04 13:55:10.000000 types-aiobotocore-transcribe-2.5.2.post2/types_aiobotocore_transcribe/__init__.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)      500 2023-08-04 13:55:10.000000 types-aiobotocore-transcribe-2.5.2.post2/types_aiobotocore_transcribe/__init__.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)      969 2023-08-04 13:55:10.000000 types-aiobotocore-transcribe-2.5.2.post2/types_aiobotocore_transcribe/__main__.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)    31836 2023-08-04 13:55:10.000000 types-aiobotocore-transcribe-2.5.2.post2/types_aiobotocore_transcribe/client.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)    31788 2023-08-04 13:55:10.000000 types-aiobotocore-transcribe-2.5.2.post2/types_aiobotocore_transcribe/client.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)    10615 2023-08-04 13:55:11.000000 types-aiobotocore-transcribe-2.5.2.post2/types_aiobotocore_transcribe/literals.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)    10613 2023-08-04 13:55:11.000000 types-aiobotocore-transcribe-2.5.2.post2/types_aiobotocore_transcribe/literals.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:55:10.000000 types-aiobotocore-transcribe-2.5.2.post2/types_aiobotocore_transcribe/py.typed
--rw-r--r--   0 vlad      (1000) vlad      (1000)    39556 2023-08-04 13:55:15.000000 types-aiobotocore-transcribe-2.5.2.post2/types_aiobotocore_transcribe/type_defs.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)    39525 2023-08-04 13:55:15.000000 types-aiobotocore-transcribe-2.5.2.post2/types_aiobotocore_transcribe/type_defs.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)       65 2023-08-04 13:55:10.000000 types-aiobotocore-transcribe-2.5.2.post2/types_aiobotocore_transcribe/version.py
-drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:29.176643 types-aiobotocore-transcribe-2.5.2.post2/types_aiobotocore_transcribe.egg-info/
--rw-r--r--   0 vlad      (1000) vlad      (1000)    12414 2023-08-04 13:59:29.000000 types-aiobotocore-transcribe-2.5.2.post2/types_aiobotocore_transcribe.egg-info/PKG-INFO
--rw-r--r--   0 vlad      (1000) vlad      (1000)      785 2023-08-04 13:59:29.000000 types-aiobotocore-transcribe-2.5.2.post2/types_aiobotocore_transcribe.egg-info/SOURCES.txt
--rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:29.000000 types-aiobotocore-transcribe-2.5.2.post2/types_aiobotocore_transcribe.egg-info/dependency_links.txt
--rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:29.000000 types-aiobotocore-transcribe-2.5.2.post2/types_aiobotocore_transcribe.egg-info/not-zip-safe
--rw-r--r--   0 vlad      (1000) vlad      (1000)       52 2023-08-04 13:59:29.000000 types-aiobotocore-transcribe-2.5.2.post2/types_aiobotocore_transcribe.egg-info/requires.txt
--rw-r--r--   0 vlad      (1000) vlad      (1000)       29 2023-08-04 13:59:29.000000 types-aiobotocore-transcribe-2.5.2.post2/types_aiobotocore_transcribe.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:24:33.758798 types-aiobotocore-transcribe-2.5.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-08 01:22:06.000000 types-aiobotocore-transcribe-2.5.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    12408 2023-08-08 01:24:33.758798 types-aiobotocore-transcribe-2.5.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10877 2023-08-08 01:22:06.000000 types-aiobotocore-transcribe-2.5.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-08 01:24:33.758798 types-aiobotocore-transcribe-2.5.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2094 2023-08-08 01:22:06.000000 types-aiobotocore-transcribe-2.5.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:24:33.754799 types-aiobotocore-transcribe-2.5.4/types_aiobotocore_transcribe/
+-rw-r--r--   0 runner    (1001) docker     (123)      501 2023-08-08 01:22:06.000000 types-aiobotocore-transcribe-2.5.4/types_aiobotocore_transcribe/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      500 2023-08-08 01:22:06.000000 types-aiobotocore-transcribe-2.5.4/types_aiobotocore_transcribe/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      957 2023-08-08 01:22:06.000000 types-aiobotocore-transcribe-2.5.4/types_aiobotocore_transcribe/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31836 2023-08-08 01:22:06.000000 types-aiobotocore-transcribe-2.5.4/types_aiobotocore_transcribe/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31788 2023-08-08 01:22:06.000000 types-aiobotocore-transcribe-2.5.4/types_aiobotocore_transcribe/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    10615 2023-08-08 01:22:06.000000 types-aiobotocore-transcribe-2.5.4/types_aiobotocore_transcribe/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10613 2023-08-08 01:22:06.000000 types-aiobotocore-transcribe-2.5.4/types_aiobotocore_transcribe/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 01:22:06.000000 types-aiobotocore-transcribe-2.5.4/types_aiobotocore_transcribe/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    39556 2023-08-08 01:22:07.000000 types-aiobotocore-transcribe-2.5.4/types_aiobotocore_transcribe/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39525 2023-08-08 01:22:07.000000 types-aiobotocore-transcribe-2.5.4/types_aiobotocore_transcribe/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-08-08 01:22:06.000000 types-aiobotocore-transcribe-2.5.4/types_aiobotocore_transcribe/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:24:33.758798 types-aiobotocore-transcribe-2.5.4/types_aiobotocore_transcribe.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    12408 2023-08-08 01:24:33.000000 types-aiobotocore-transcribe-2.5.4/types_aiobotocore_transcribe.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      785 2023-08-08 01:24:33.000000 types-aiobotocore-transcribe-2.5.4/types_aiobotocore_transcribe.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 01:24:33.000000 types-aiobotocore-transcribe-2.5.4/types_aiobotocore_transcribe.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 01:24:33.000000 types-aiobotocore-transcribe-2.5.4/types_aiobotocore_transcribe.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-08 01:24:33.000000 types-aiobotocore-transcribe-2.5.4/types_aiobotocore_transcribe.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-08-08 01:24:33.000000 types-aiobotocore-transcribe-2.5.4/types_aiobotocore_transcribe.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-transcribe-2.5.2.post2/LICENSE` & `types-aiobotocore-transcribe-2.5.4/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-transcribe-2.5.2.post2/PKG-INFO` & `types-aiobotocore-transcribe-2.5.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-transcribe
-Version: 2.5.2.post2
-Summary: Type annotations for aiobotocore.TranscribeService 2.5.2 service generated with mypy-boto3-builder 7.17.2
+Version: 2.5.4
+Summary: Type annotations for aiobotocore.TranscribeService 2.5.4 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_transcribe/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-transcribe.svg?color=blue)](https://pypi.org/project/types-aiobotocore-transcribe)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_transcribe/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-transcribe)](https://pepy.tech/project/types-aiobotocore-transcribe)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.TranscribeService 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transcribe.html#TranscribeService)
+[aiobotocore.TranscribeService 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transcribe.html#TranscribeService)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-transcribe-2.5.2.post2/README.md` & `types-aiobotocore-transcribe-2.5.4/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-transcribe.svg?color=blue)](https://pypi.org/project/types-aiobotocore-transcribe)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_transcribe/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-transcribe)](https://pepy.tech/project/types-aiobotocore-transcribe)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.TranscribeService 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transcribe.html#TranscribeService)
+[aiobotocore.TranscribeService 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transcribe.html#TranscribeService)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-transcribe-2.5.2.post2/setup.py` & `types-aiobotocore-transcribe-2.5.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-transcribe",
-    version="2.5.2.post2",
+    version="2.5.4",
     packages=["types_aiobotocore_transcribe"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.TranscribeService 2.5.2 service generated with"
+        "Type annotations for aiobotocore.TranscribeService 2.5.4 service generated with"
         " mypy-boto3-builder 7.17.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
```

### Comparing `types-aiobotocore-transcribe-2.5.2.post2/types_aiobotocore_transcribe/__main__.py` & `types-aiobotocore-transcribe-2.5.4/types_aiobotocore_transcribe/__main__.py`

 * *Files 16% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.TranscribeService 2.5.2\nVersion:        "
-        " 2.5.2.post2\nBuilder version: 7.17.2\nDocs:           "
+        "Type annotations for aiobotocore.TranscribeService 2.5.4\nVersion:         2.5.4\nBuilder"
+        " version: 7.17.2\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_transcribe//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transcribe.html#TranscribeService\nOther"
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

### Comparing `types-aiobotocore-transcribe-2.5.2.post2/types_aiobotocore_transcribe/client.py` & `types-aiobotocore-transcribe-2.5.4/types_aiobotocore_transcribe/client.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-transcribe-2.5.2.post2/types_aiobotocore_transcribe/client.pyi` & `types-aiobotocore-transcribe-2.5.4/types_aiobotocore_transcribe/client.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-transcribe-2.5.2.post2/types_aiobotocore_transcribe/literals.py` & `types-aiobotocore-transcribe-2.5.4/types_aiobotocore_transcribe/literals.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-transcribe-2.5.2.post2/types_aiobotocore_transcribe/literals.pyi` & `types-aiobotocore-transcribe-2.5.4/types_aiobotocore_transcribe/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-transcribe-2.5.2.post2/types_aiobotocore_transcribe/type_defs.py` & `types-aiobotocore-transcribe-2.5.4/types_aiobotocore_transcribe/type_defs.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-transcribe-2.5.2.post2/types_aiobotocore_transcribe/type_defs.pyi` & `types-aiobotocore-transcribe-2.5.4/types_aiobotocore_transcribe/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-transcribe-2.5.2.post2/types_aiobotocore_transcribe.egg-info/PKG-INFO` & `types-aiobotocore-transcribe-2.5.4/types_aiobotocore_transcribe.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-transcribe
-Version: 2.5.2.post2
-Summary: Type annotations for aiobotocore.TranscribeService 2.5.2 service generated with mypy-boto3-builder 7.17.2
+Version: 2.5.4
+Summary: Type annotations for aiobotocore.TranscribeService 2.5.4 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_transcribe/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-transcribe.svg?color=blue)](https://pypi.org/project/types-aiobotocore-transcribe)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_transcribe/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-transcribe)](https://pepy.tech/project/types-aiobotocore-transcribe)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.TranscribeService 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transcribe.html#TranscribeService)
+[aiobotocore.TranscribeService 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transcribe.html#TranscribeService)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-transcribe-2.5.2.post2/types_aiobotocore_transcribe.egg-info/SOURCES.txt` & `types-aiobotocore-transcribe-2.5.4/types_aiobotocore_transcribe.egg-info/SOURCES.txt`

 * *Files identical despite different names*


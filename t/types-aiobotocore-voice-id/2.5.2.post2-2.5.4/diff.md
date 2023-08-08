# Comparing `tmp/types-aiobotocore-voice-id-2.5.2.post2.tar.gz` & `tmp/types-aiobotocore-voice-id-2.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-voice-id-2.5.2.post2.tar", last modified: Fri Aug  4 13:59:29 2023, max compression
+gzip compressed data, was "types-aiobotocore-voice-id-2.5.4.tar", last modified: Tue Aug  8 01:24:34 2023, max compression
```

## Comparing `types-aiobotocore-voice-id-2.5.2.post2.tar` & `types-aiobotocore-voice-id-2.5.4.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:29.316643 types-aiobotocore-voice-id-2.5.2.post2/
--rw-r--r--   0 vlad      (1000) vlad      (1000)     1070 2023-08-04 13:55:25.000000 types-aiobotocore-voice-id-2.5.2.post2/LICENSE
--rw-r--r--   0 vlad      (1000) vlad      (1000)    13762 2023-08-04 13:59:29.316643 types-aiobotocore-voice-id-2.5.2.post2/PKG-INFO
--rw-r--r--   0 vlad      (1000) vlad      (1000)    12241 2023-08-04 13:55:25.000000 types-aiobotocore-voice-id-2.5.2.post2/README.md
--rw-r--r--   0 vlad      (1000) vlad      (1000)       38 2023-08-04 13:59:29.316643 types-aiobotocore-voice-id-2.5.2.post2/setup.cfg
--rw-r--r--   0 vlad      (1000) vlad      (1000)     2078 2023-08-04 13:55:25.000000 types-aiobotocore-voice-id-2.5.2.post2/setup.py
-drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:29.316643 types-aiobotocore-voice-id-2.5.2.post2/types_aiobotocore_voice_id/
--rw-r--r--   0 vlad      (1000) vlad      (1000)     1758 2023-08-04 13:55:25.000000 types-aiobotocore-voice-id-2.5.2.post2/types_aiobotocore_voice_id/__init__.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)     1757 2023-08-04 13:55:25.000000 types-aiobotocore-voice-id-2.5.2.post2/types_aiobotocore_voice_id/__init__.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)      945 2023-08-04 13:55:25.000000 types-aiobotocore-voice-id-2.5.2.post2/types_aiobotocore_voice_id/__main__.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)    25008 2023-08-04 13:55:25.000000 types-aiobotocore-voice-id-2.5.2.post2/types_aiobotocore_voice_id/client.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)    24964 2023-08-04 13:55:25.000000 types-aiobotocore-voice-id-2.5.2.post2/types_aiobotocore_voice_id/client.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)    10153 2023-08-04 13:55:26.000000 types-aiobotocore-voice-id-2.5.2.post2/types_aiobotocore_voice_id/literals.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)    10151 2023-08-04 13:55:25.000000 types-aiobotocore-voice-id-2.5.2.post2/types_aiobotocore_voice_id/literals.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)     7963 2023-08-04 13:55:25.000000 types-aiobotocore-voice-id-2.5.2.post2/types_aiobotocore_voice_id/paginator.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)     7955 2023-08-04 13:55:25.000000 types-aiobotocore-voice-id-2.5.2.post2/types_aiobotocore_voice_id/paginator.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:55:25.000000 types-aiobotocore-voice-id-2.5.2.post2/types_aiobotocore_voice_id/py.typed
--rw-r--r--   0 vlad      (1000) vlad      (1000)    32445 2023-08-04 13:55:26.000000 types-aiobotocore-voice-id-2.5.2.post2/types_aiobotocore_voice_id/type_defs.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)    32408 2023-08-04 13:55:26.000000 types-aiobotocore-voice-id-2.5.2.post2/types_aiobotocore_voice_id/type_defs.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)       65 2023-08-04 13:55:25.000000 types-aiobotocore-voice-id-2.5.2.post2/types_aiobotocore_voice_id/version.py
-drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:29.316643 types-aiobotocore-voice-id-2.5.2.post2/types_aiobotocore_voice_id.egg-info/
--rw-r--r--   0 vlad      (1000) vlad      (1000)    13762 2023-08-04 13:59:29.000000 types-aiobotocore-voice-id-2.5.2.post2/types_aiobotocore_voice_id.egg-info/PKG-INFO
--rw-r--r--   0 vlad      (1000) vlad      (1000)      832 2023-08-04 13:59:29.000000 types-aiobotocore-voice-id-2.5.2.post2/types_aiobotocore_voice_id.egg-info/SOURCES.txt
--rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:29.000000 types-aiobotocore-voice-id-2.5.2.post2/types_aiobotocore_voice_id.egg-info/dependency_links.txt
--rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:29.000000 types-aiobotocore-voice-id-2.5.2.post2/types_aiobotocore_voice_id.egg-info/not-zip-safe
--rw-r--r--   0 vlad      (1000) vlad      (1000)       52 2023-08-04 13:59:29.000000 types-aiobotocore-voice-id-2.5.2.post2/types_aiobotocore_voice_id.egg-info/requires.txt
--rw-r--r--   0 vlad      (1000) vlad      (1000)       27 2023-08-04 13:59:29.000000 types-aiobotocore-voice-id-2.5.2.post2/types_aiobotocore_voice_id.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:24:34.514800 types-aiobotocore-voice-id-2.5.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-08 01:22:12.000000 types-aiobotocore-voice-id-2.5.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    13756 2023-08-08 01:24:34.510800 types-aiobotocore-voice-id-2.5.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    12241 2023-08-08 01:22:12.000000 types-aiobotocore-voice-id-2.5.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-08 01:24:34.514800 types-aiobotocore-voice-id-2.5.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2072 2023-08-08 01:22:12.000000 types-aiobotocore-voice-id-2.5.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:24:34.510800 types-aiobotocore-voice-id-2.5.4/types_aiobotocore_voice_id/
+-rw-r--r--   0 runner    (1001) docker     (123)     1758 2023-08-08 01:22:12.000000 types-aiobotocore-voice-id-2.5.4/types_aiobotocore_voice_id/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1757 2023-08-08 01:22:12.000000 types-aiobotocore-voice-id-2.5.4/types_aiobotocore_voice_id/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      933 2023-08-08 01:22:13.000000 types-aiobotocore-voice-id-2.5.4/types_aiobotocore_voice_id/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25008 2023-08-08 01:22:13.000000 types-aiobotocore-voice-id-2.5.4/types_aiobotocore_voice_id/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24964 2023-08-08 01:22:13.000000 types-aiobotocore-voice-id-2.5.4/types_aiobotocore_voice_id/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    10153 2023-08-08 01:22:13.000000 types-aiobotocore-voice-id-2.5.4/types_aiobotocore_voice_id/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10151 2023-08-08 01:22:13.000000 types-aiobotocore-voice-id-2.5.4/types_aiobotocore_voice_id/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     7963 2023-08-08 01:22:13.000000 types-aiobotocore-voice-id-2.5.4/types_aiobotocore_voice_id/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7955 2023-08-08 01:22:13.000000 types-aiobotocore-voice-id-2.5.4/types_aiobotocore_voice_id/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 01:22:13.000000 types-aiobotocore-voice-id-2.5.4/types_aiobotocore_voice_id/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    32445 2023-08-08 01:22:13.000000 types-aiobotocore-voice-id-2.5.4/types_aiobotocore_voice_id/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32408 2023-08-08 01:22:13.000000 types-aiobotocore-voice-id-2.5.4/types_aiobotocore_voice_id/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-08-08 01:22:12.000000 types-aiobotocore-voice-id-2.5.4/types_aiobotocore_voice_id/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:24:34.510800 types-aiobotocore-voice-id-2.5.4/types_aiobotocore_voice_id.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    13756 2023-08-08 01:24:34.000000 types-aiobotocore-voice-id-2.5.4/types_aiobotocore_voice_id.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      832 2023-08-08 01:24:34.000000 types-aiobotocore-voice-id-2.5.4/types_aiobotocore_voice_id.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 01:24:34.000000 types-aiobotocore-voice-id-2.5.4/types_aiobotocore_voice_id.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 01:24:34.000000 types-aiobotocore-voice-id-2.5.4/types_aiobotocore_voice_id.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-08 01:24:34.000000 types-aiobotocore-voice-id-2.5.4/types_aiobotocore_voice_id.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-08-08 01:24:34.000000 types-aiobotocore-voice-id-2.5.4/types_aiobotocore_voice_id.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-voice-id-2.5.2.post2/LICENSE` & `types-aiobotocore-voice-id-2.5.4/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-voice-id-2.5.2.post2/PKG-INFO` & `types-aiobotocore-voice-id-2.5.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-voice-id
-Version: 2.5.2.post2
-Summary: Type annotations for aiobotocore.VoiceID 2.5.2 service generated with mypy-boto3-builder 7.17.2
+Version: 2.5.4
+Summary: Type annotations for aiobotocore.VoiceID 2.5.4 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_voice_id/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-voice-id.svg?color=blue)](https://pypi.org/project/types-aiobotocore-voice-id)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_voice_id/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-voice-id)](https://pepy.tech/project/types-aiobotocore-voice-id)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.VoiceID 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/voice-id.html#VoiceID)
+[aiobotocore.VoiceID 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/voice-id.html#VoiceID)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-voice-id-2.5.2.post2/README.md` & `types-aiobotocore-voice-id-2.5.4/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-voice-id.svg?color=blue)](https://pypi.org/project/types-aiobotocore-voice-id)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_voice_id/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-voice-id)](https://pepy.tech/project/types-aiobotocore-voice-id)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.VoiceID 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/voice-id.html#VoiceID)
+[aiobotocore.VoiceID 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/voice-id.html#VoiceID)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-voice-id-2.5.2.post2/setup.py` & `types-aiobotocore-voice-id-2.5.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-voice-id",
-    version="2.5.2.post2",
+    version="2.5.4",
     packages=["types_aiobotocore_voice_id"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.VoiceID 2.5.2 service generated with mypy-boto3-builder"
+        "Type annotations for aiobotocore.VoiceID 2.5.4 service generated with mypy-boto3-builder"
         " 7.17.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
```

### Comparing `types-aiobotocore-voice-id-2.5.2.post2/types_aiobotocore_voice_id/__init__.py` & `types-aiobotocore-voice-id-2.5.4/types_aiobotocore_voice_id/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-voice-id-2.5.2.post2/types_aiobotocore_voice_id/__init__.pyi` & `types-aiobotocore-voice-id-2.5.4/types_aiobotocore_voice_id/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-voice-id-2.5.2.post2/types_aiobotocore_voice_id/__main__.py` & `types-aiobotocore-voice-id-2.5.4/types_aiobotocore_voice_id/__main__.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.VoiceID 2.5.2\nVersion:         2.5.2.post2\nBuilder"
-        " version: 7.17.2\nDocs:           "
+        "Type annotations for aiobotocore.VoiceID 2.5.4\nVersion:         2.5.4\nBuilder version:"
+        " 7.17.2\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_voice_id//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/voice-id.html#VoiceID\nOther"
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

### Comparing `types-aiobotocore-voice-id-2.5.2.post2/types_aiobotocore_voice_id/client.py` & `types-aiobotocore-voice-id-2.5.4/types_aiobotocore_voice_id/client.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-voice-id-2.5.2.post2/types_aiobotocore_voice_id/client.pyi` & `types-aiobotocore-voice-id-2.5.4/types_aiobotocore_voice_id/client.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-voice-id-2.5.2.post2/types_aiobotocore_voice_id/literals.py` & `types-aiobotocore-voice-id-2.5.4/types_aiobotocore_voice_id/literals.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-voice-id-2.5.2.post2/types_aiobotocore_voice_id/literals.pyi` & `types-aiobotocore-voice-id-2.5.4/types_aiobotocore_voice_id/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-voice-id-2.5.2.post2/types_aiobotocore_voice_id/paginator.py` & `types-aiobotocore-voice-id-2.5.4/types_aiobotocore_voice_id/paginator.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-voice-id-2.5.2.post2/types_aiobotocore_voice_id/paginator.pyi` & `types-aiobotocore-voice-id-2.5.4/types_aiobotocore_voice_id/paginator.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-voice-id-2.5.2.post2/types_aiobotocore_voice_id/type_defs.py` & `types-aiobotocore-voice-id-2.5.4/types_aiobotocore_voice_id/type_defs.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-voice-id-2.5.2.post2/types_aiobotocore_voice_id/type_defs.pyi` & `types-aiobotocore-voice-id-2.5.4/types_aiobotocore_voice_id/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-voice-id-2.5.2.post2/types_aiobotocore_voice_id.egg-info/PKG-INFO` & `types-aiobotocore-voice-id-2.5.4/types_aiobotocore_voice_id.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-voice-id
-Version: 2.5.2.post2
-Summary: Type annotations for aiobotocore.VoiceID 2.5.2 service generated with mypy-boto3-builder 7.17.2
+Version: 2.5.4
+Summary: Type annotations for aiobotocore.VoiceID 2.5.4 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_voice_id/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-voice-id.svg?color=blue)](https://pypi.org/project/types-aiobotocore-voice-id)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_voice_id/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-voice-id)](https://pepy.tech/project/types-aiobotocore-voice-id)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.VoiceID 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/voice-id.html#VoiceID)
+[aiobotocore.VoiceID 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/voice-id.html#VoiceID)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-voice-id-2.5.2.post2/types_aiobotocore_voice_id.egg-info/SOURCES.txt` & `types-aiobotocore-voice-id-2.5.4/types_aiobotocore_voice_id.egg-info/SOURCES.txt`

 * *Files identical despite different names*


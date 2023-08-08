# Comparing `tmp/types-aiobotocore-kinesis-video-webrtc-storage-2.5.2.post2.tar.gz` & `tmp/types-aiobotocore-kinesis-video-webrtc-storage-2.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-kinesis-video-webrtc-storage-2.5.2.post2.tar", last modified: Fri Aug  4 13:59:14 2023, max compression
+gzip compressed data, was "types-aiobotocore-kinesis-video-webrtc-storage-2.5.4.tar", last modified: Tue Aug  8 01:23:57 2023, max compression
```

## Comparing `types-aiobotocore-kinesis-video-webrtc-storage-2.5.2.post2.tar` & `types-aiobotocore-kinesis-video-webrtc-storage-2.5.4.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:14.326643 types-aiobotocore-kinesis-video-webrtc-storage-2.5.2.post2/
--rw-r--r--   0 vlad      (1000) vlad      (1000)     1070 2023-08-04 13:42:04.000000 types-aiobotocore-kinesis-video-webrtc-storage-2.5.2.post2/LICENSE
--rw-r--r--   0 vlad      (1000) vlad      (1000)    13329 2023-08-04 13:59:14.326643 types-aiobotocore-kinesis-video-webrtc-storage-2.5.2.post2/PKG-INFO
--rw-r--r--   0 vlad      (1000) vlad      (1000)    11730 2023-08-04 13:42:04.000000 types-aiobotocore-kinesis-video-webrtc-storage-2.5.2.post2/README.md
--rw-r--r--   0 vlad      (1000) vlad      (1000)       38 2023-08-04 13:59:14.326643 types-aiobotocore-kinesis-video-webrtc-storage-2.5.2.post2/setup.cfg
--rw-r--r--   0 vlad      (1000) vlad      (1000)     2219 2023-08-04 13:42:04.000000 types-aiobotocore-kinesis-video-webrtc-storage-2.5.2.post2/setup.py
-drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:14.326643 types-aiobotocore-kinesis-video-webrtc-storage-2.5.2.post2/types_aiobotocore_kinesis_video_webrtc_storage/
--rw-r--r--   0 vlad      (1000) vlad      (1000)      595 2023-08-04 13:42:04.000000 types-aiobotocore-kinesis-video-webrtc-storage-2.5.2.post2/types_aiobotocore_kinesis_video_webrtc_storage/__init__.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)      594 2023-08-04 13:42:04.000000 types-aiobotocore-kinesis-video-webrtc-storage-2.5.2.post2/types_aiobotocore_kinesis_video_webrtc_storage/__init__.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)     1021 2023-08-04 13:42:04.000000 types-aiobotocore-kinesis-video-webrtc-storage-2.5.2.post2/types_aiobotocore_kinesis_video_webrtc_storage/__main__.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)     5283 2023-08-04 13:42:04.000000 types-aiobotocore-kinesis-video-webrtc-storage-2.5.2.post2/types_aiobotocore_kinesis_video_webrtc_storage/client.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)     5274 2023-08-04 13:42:04.000000 types-aiobotocore-kinesis-video-webrtc-storage-2.5.2.post2/types_aiobotocore_kinesis_video_webrtc_storage/client.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)     8134 2023-08-04 13:42:04.000000 types-aiobotocore-kinesis-video-webrtc-storage-2.5.2.post2/types_aiobotocore_kinesis_video_webrtc_storage/literals.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)     8132 2023-08-04 13:42:04.000000 types-aiobotocore-kinesis-video-webrtc-storage-2.5.2.post2/types_aiobotocore_kinesis_video_webrtc_storage/literals.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:42:04.000000 types-aiobotocore-kinesis-video-webrtc-storage-2.5.2.post2/types_aiobotocore_kinesis_video_webrtc_storage/py.typed
--rw-r--r--   0 vlad      (1000) vlad      (1000)     1181 2023-08-04 13:42:04.000000 types-aiobotocore-kinesis-video-webrtc-storage-2.5.2.post2/types_aiobotocore_kinesis_video_webrtc_storage/type_defs.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)     1180 2023-08-04 13:42:04.000000 types-aiobotocore-kinesis-video-webrtc-storage-2.5.2.post2/types_aiobotocore_kinesis_video_webrtc_storage/type_defs.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)       65 2023-08-04 13:42:04.000000 types-aiobotocore-kinesis-video-webrtc-storage-2.5.2.post2/types_aiobotocore_kinesis_video_webrtc_storage/version.py
-drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:14.326643 types-aiobotocore-kinesis-video-webrtc-storage-2.5.2.post2/types_aiobotocore_kinesis_video_webrtc_storage.egg-info/
--rw-r--r--   0 vlad      (1000) vlad      (1000)    13329 2023-08-04 13:59:14.000000 types-aiobotocore-kinesis-video-webrtc-storage-2.5.2.post2/types_aiobotocore_kinesis_video_webrtc_storage.egg-info/PKG-INFO
--rw-r--r--   0 vlad      (1000) vlad      (1000)     1091 2023-08-04 13:59:14.000000 types-aiobotocore-kinesis-video-webrtc-storage-2.5.2.post2/types_aiobotocore_kinesis_video_webrtc_storage.egg-info/SOURCES.txt
--rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:14.000000 types-aiobotocore-kinesis-video-webrtc-storage-2.5.2.post2/types_aiobotocore_kinesis_video_webrtc_storage.egg-info/dependency_links.txt
--rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:14.000000 types-aiobotocore-kinesis-video-webrtc-storage-2.5.2.post2/types_aiobotocore_kinesis_video_webrtc_storage.egg-info/not-zip-safe
--rw-r--r--   0 vlad      (1000) vlad      (1000)       52 2023-08-04 13:59:14.000000 types-aiobotocore-kinesis-video-webrtc-storage-2.5.2.post2/types_aiobotocore_kinesis_video_webrtc_storage.egg-info/requires.txt
--rw-r--r--   0 vlad      (1000) vlad      (1000)       47 2023-08-04 13:59:14.000000 types-aiobotocore-kinesis-video-webrtc-storage-2.5.2.post2/types_aiobotocore_kinesis_video_webrtc_storage.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:23:57.394718 types-aiobotocore-kinesis-video-webrtc-storage-2.5.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-08 01:13:36.000000 types-aiobotocore-kinesis-video-webrtc-storage-2.5.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    13323 2023-08-08 01:23:57.394718 types-aiobotocore-kinesis-video-webrtc-storage-2.5.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    11730 2023-08-08 01:13:36.000000 types-aiobotocore-kinesis-video-webrtc-storage-2.5.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-08 01:23:57.394718 types-aiobotocore-kinesis-video-webrtc-storage-2.5.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2213 2023-08-08 01:13:36.000000 types-aiobotocore-kinesis-video-webrtc-storage-2.5.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:23:57.394718 types-aiobotocore-kinesis-video-webrtc-storage-2.5.4/types_aiobotocore_kinesis_video_webrtc_storage/
+-rw-r--r--   0 runner    (1001) docker     (123)      595 2023-08-08 01:13:36.000000 types-aiobotocore-kinesis-video-webrtc-storage-2.5.4/types_aiobotocore_kinesis_video_webrtc_storage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      594 2023-08-08 01:13:36.000000 types-aiobotocore-kinesis-video-webrtc-storage-2.5.4/types_aiobotocore_kinesis_video_webrtc_storage/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1009 2023-08-08 01:13:36.000000 types-aiobotocore-kinesis-video-webrtc-storage-2.5.4/types_aiobotocore_kinesis_video_webrtc_storage/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5283 2023-08-08 01:13:36.000000 types-aiobotocore-kinesis-video-webrtc-storage-2.5.4/types_aiobotocore_kinesis_video_webrtc_storage/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5274 2023-08-08 01:13:36.000000 types-aiobotocore-kinesis-video-webrtc-storage-2.5.4/types_aiobotocore_kinesis_video_webrtc_storage/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8134 2023-08-08 01:13:37.000000 types-aiobotocore-kinesis-video-webrtc-storage-2.5.4/types_aiobotocore_kinesis_video_webrtc_storage/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8132 2023-08-08 01:13:37.000000 types-aiobotocore-kinesis-video-webrtc-storage-2.5.4/types_aiobotocore_kinesis_video_webrtc_storage/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 01:13:36.000000 types-aiobotocore-kinesis-video-webrtc-storage-2.5.4/types_aiobotocore_kinesis_video_webrtc_storage/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     1181 2023-08-08 01:13:37.000000 types-aiobotocore-kinesis-video-webrtc-storage-2.5.4/types_aiobotocore_kinesis_video_webrtc_storage/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1180 2023-08-08 01:13:37.000000 types-aiobotocore-kinesis-video-webrtc-storage-2.5.4/types_aiobotocore_kinesis_video_webrtc_storage/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-08-08 01:13:36.000000 types-aiobotocore-kinesis-video-webrtc-storage-2.5.4/types_aiobotocore_kinesis_video_webrtc_storage/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:23:57.394718 types-aiobotocore-kinesis-video-webrtc-storage-2.5.4/types_aiobotocore_kinesis_video_webrtc_storage.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    13323 2023-08-08 01:23:57.000000 types-aiobotocore-kinesis-video-webrtc-storage-2.5.4/types_aiobotocore_kinesis_video_webrtc_storage.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1091 2023-08-08 01:23:57.000000 types-aiobotocore-kinesis-video-webrtc-storage-2.5.4/types_aiobotocore_kinesis_video_webrtc_storage.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 01:23:57.000000 types-aiobotocore-kinesis-video-webrtc-storage-2.5.4/types_aiobotocore_kinesis_video_webrtc_storage.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 01:23:57.000000 types-aiobotocore-kinesis-video-webrtc-storage-2.5.4/types_aiobotocore_kinesis_video_webrtc_storage.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-08 01:23:57.000000 types-aiobotocore-kinesis-video-webrtc-storage-2.5.4/types_aiobotocore_kinesis_video_webrtc_storage.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-08-08 01:23:57.000000 types-aiobotocore-kinesis-video-webrtc-storage-2.5.4/types_aiobotocore_kinesis_video_webrtc_storage.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-kinesis-video-webrtc-storage-2.5.2.post2/LICENSE` & `types-aiobotocore-kinesis-video-webrtc-storage-2.5.4/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-kinesis-video-webrtc-storage-2.5.2.post2/PKG-INFO` & `types-aiobotocore-kinesis-video-webrtc-storage-2.5.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-kinesis-video-webrtc-storage
-Version: 2.5.2.post2
-Summary: Type annotations for aiobotocore.KinesisVideoWebRTCStorage 2.5.2 service generated with mypy-boto3-builder 7.17.2
+Version: 2.5.4
+Summary: Type annotations for aiobotocore.KinesisVideoWebRTCStorage 2.5.4 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kinesis_video_webrtc_storage/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-kinesis-video-webrtc-storage.svg?color=blue)](https://pypi.org/project/types-aiobotocore-kinesis-video-webrtc-storage)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kinesis_video_webrtc_storage/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-kinesis-video-webrtc-storage)](https://pepy.tech/project/types-aiobotocore-kinesis-video-webrtc-storage)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.KinesisVideoWebRTCStorage 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesis-video-webrtc-storage.html#KinesisVideoWebRTCStorage)
+[aiobotocore.KinesisVideoWebRTCStorage 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesis-video-webrtc-storage.html#KinesisVideoWebRTCStorage)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-kinesis-video-webrtc-storage-2.5.2.post2/README.md` & `types-aiobotocore-kinesis-video-webrtc-storage-2.5.4/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-kinesis-video-webrtc-storage.svg?color=blue)](https://pypi.org/project/types-aiobotocore-kinesis-video-webrtc-storage)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kinesis_video_webrtc_storage/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-kinesis-video-webrtc-storage)](https://pepy.tech/project/types-aiobotocore-kinesis-video-webrtc-storage)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.KinesisVideoWebRTCStorage 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesis-video-webrtc-storage.html#KinesisVideoWebRTCStorage)
+[aiobotocore.KinesisVideoWebRTCStorage 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesis-video-webrtc-storage.html#KinesisVideoWebRTCStorage)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-kinesis-video-webrtc-storage-2.5.2.post2/setup.py` & `types-aiobotocore-kinesis-video-webrtc-storage-2.5.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-kinesis-video-webrtc-storage",
-    version="2.5.2.post2",
+    version="2.5.4",
     packages=["types_aiobotocore_kinesis_video_webrtc_storage"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.KinesisVideoWebRTCStorage 2.5.2 service generated with"
+        "Type annotations for aiobotocore.KinesisVideoWebRTCStorage 2.5.4 service generated with"
         " mypy-boto3-builder 7.17.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
```

### Comparing `types-aiobotocore-kinesis-video-webrtc-storage-2.5.2.post2/types_aiobotocore_kinesis_video_webrtc_storage/__init__.py` & `types-aiobotocore-kinesis-video-webrtc-storage-2.5.4/types_aiobotocore_kinesis_video_webrtc_storage/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-kinesis-video-webrtc-storage-2.5.2.post2/types_aiobotocore_kinesis_video_webrtc_storage/__init__.pyi` & `types-aiobotocore-kinesis-video-webrtc-storage-2.5.4/types_aiobotocore_kinesis_video_webrtc_storage/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-kinesis-video-webrtc-storage-2.5.2.post2/types_aiobotocore_kinesis_video_webrtc_storage/__main__.py` & `types-aiobotocore-kinesis-video-webrtc-storage-2.5.4/types_aiobotocore_kinesis_video_webrtc_storage/__main__.py`

 * *Files 7% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.KinesisVideoWebRTCStorage 2.5.2\nVersion:        "
-        " 2.5.2.post2\nBuilder version: 7.17.2\nDocs:           "
+        "Type annotations for aiobotocore.KinesisVideoWebRTCStorage 2.5.4\nVersion:        "
+        " 2.5.4\nBuilder version: 7.17.2\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kinesis_video_webrtc_storage//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesis-video-webrtc-storage.html#KinesisVideoWebRTCStorage\nOther"
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

### Comparing `types-aiobotocore-kinesis-video-webrtc-storage-2.5.2.post2/types_aiobotocore_kinesis_video_webrtc_storage/client.py` & `types-aiobotocore-kinesis-video-webrtc-storage-2.5.4/types_aiobotocore_kinesis_video_webrtc_storage/client.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-kinesis-video-webrtc-storage-2.5.2.post2/types_aiobotocore_kinesis_video_webrtc_storage/client.pyi` & `types-aiobotocore-kinesis-video-webrtc-storage-2.5.4/types_aiobotocore_kinesis_video_webrtc_storage/client.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-kinesis-video-webrtc-storage-2.5.2.post2/types_aiobotocore_kinesis_video_webrtc_storage/literals.py` & `types-aiobotocore-kinesis-video-webrtc-storage-2.5.4/types_aiobotocore_kinesis_video_webrtc_storage/literals.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-kinesis-video-webrtc-storage-2.5.2.post2/types_aiobotocore_kinesis_video_webrtc_storage/literals.pyi` & `types-aiobotocore-kinesis-video-webrtc-storage-2.5.4/types_aiobotocore_kinesis_video_webrtc_storage/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-kinesis-video-webrtc-storage-2.5.2.post2/types_aiobotocore_kinesis_video_webrtc_storage/type_defs.py` & `types-aiobotocore-kinesis-video-webrtc-storage-2.5.4/types_aiobotocore_kinesis_video_webrtc_storage/type_defs.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-kinesis-video-webrtc-storage-2.5.2.post2/types_aiobotocore_kinesis_video_webrtc_storage/type_defs.pyi` & `types-aiobotocore-kinesis-video-webrtc-storage-2.5.4/types_aiobotocore_kinesis_video_webrtc_storage/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-kinesis-video-webrtc-storage-2.5.2.post2/types_aiobotocore_kinesis_video_webrtc_storage.egg-info/PKG-INFO` & `types-aiobotocore-kinesis-video-webrtc-storage-2.5.4/types_aiobotocore_kinesis_video_webrtc_storage.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-kinesis-video-webrtc-storage
-Version: 2.5.2.post2
-Summary: Type annotations for aiobotocore.KinesisVideoWebRTCStorage 2.5.2 service generated with mypy-boto3-builder 7.17.2
+Version: 2.5.4
+Summary: Type annotations for aiobotocore.KinesisVideoWebRTCStorage 2.5.4 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kinesis_video_webrtc_storage/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-kinesis-video-webrtc-storage.svg?color=blue)](https://pypi.org/project/types-aiobotocore-kinesis-video-webrtc-storage)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kinesis_video_webrtc_storage/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-kinesis-video-webrtc-storage)](https://pepy.tech/project/types-aiobotocore-kinesis-video-webrtc-storage)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.KinesisVideoWebRTCStorage 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesis-video-webrtc-storage.html#KinesisVideoWebRTCStorage)
+[aiobotocore.KinesisVideoWebRTCStorage 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesis-video-webrtc-storage.html#KinesisVideoWebRTCStorage)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-kinesis-video-webrtc-storage-2.5.2.post2/types_aiobotocore_kinesis_video_webrtc_storage.egg-info/SOURCES.txt` & `types-aiobotocore-kinesis-video-webrtc-storage-2.5.4/types_aiobotocore_kinesis_video_webrtc_storage.egg-info/SOURCES.txt`

 * *Files identical despite different names*


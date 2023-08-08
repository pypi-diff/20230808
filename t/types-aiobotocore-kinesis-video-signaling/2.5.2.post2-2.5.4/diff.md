# Comparing `tmp/types-aiobotocore-kinesis-video-signaling-2.5.2.post2.tar.gz` & `tmp/types-aiobotocore-kinesis-video-signaling-2.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-kinesis-video-signaling-2.5.2.post2.tar", last modified: Fri Aug  4 13:59:14 2023, max compression
+gzip compressed data, was "types-aiobotocore-kinesis-video-signaling-2.5.4.tar", last modified: Tue Aug  8 01:23:57 2023, max compression
```

## Comparing `types-aiobotocore-kinesis-video-signaling-2.5.2.post2.tar` & `types-aiobotocore-kinesis-video-signaling-2.5.4.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:14.166643 types-aiobotocore-kinesis-video-signaling-2.5.2.post2/
--rw-r--r--   0 vlad      (1000) vlad      (1000)     1070 2023-08-04 13:42:03.000000 types-aiobotocore-kinesis-video-signaling-2.5.2.post2/LICENSE
--rw-r--r--   0 vlad      (1000) vlad      (1000)    13121 2023-08-04 13:59:14.166643 types-aiobotocore-kinesis-video-signaling-2.5.2.post2/PKG-INFO
--rw-r--r--   0 vlad      (1000) vlad      (1000)    11533 2023-08-04 13:42:03.000000 types-aiobotocore-kinesis-video-signaling-2.5.2.post2/README.md
--rw-r--r--   0 vlad      (1000) vlad      (1000)       38 2023-08-04 13:59:14.166643 types-aiobotocore-kinesis-video-signaling-2.5.2.post2/setup.cfg
--rw-r--r--   0 vlad      (1000) vlad      (1000)     2182 2023-08-04 13:42:03.000000 types-aiobotocore-kinesis-video-signaling-2.5.2.post2/setup.py
-drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:14.166643 types-aiobotocore-kinesis-video-signaling-2.5.2.post2/types_aiobotocore_kinesis_video_signaling/
--rw-r--r--   0 vlad      (1000) vlad      (1000)      600 2023-08-04 13:42:03.000000 types-aiobotocore-kinesis-video-signaling-2.5.2.post2/types_aiobotocore_kinesis_video_signaling/__init__.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)      599 2023-08-04 13:42:03.000000 types-aiobotocore-kinesis-video-signaling-2.5.2.post2/types_aiobotocore_kinesis_video_signaling/__init__.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)     1019 2023-08-04 13:42:03.000000 types-aiobotocore-kinesis-video-signaling-2.5.2.post2/types_aiobotocore_kinesis_video_signaling/__main__.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)     6389 2023-08-04 13:42:03.000000 types-aiobotocore-kinesis-video-signaling-2.5.2.post2/types_aiobotocore_kinesis_video_signaling/client.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)     6378 2023-08-04 13:42:03.000000 types-aiobotocore-kinesis-video-signaling-2.5.2.post2/types_aiobotocore_kinesis_video_signaling/client.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)     8097 2023-08-04 13:42:03.000000 types-aiobotocore-kinesis-video-signaling-2.5.2.post2/types_aiobotocore_kinesis_video_signaling/literals.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)     8095 2023-08-04 13:42:03.000000 types-aiobotocore-kinesis-video-signaling-2.5.2.post2/types_aiobotocore_kinesis_video_signaling/literals.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:42:03.000000 types-aiobotocore-kinesis-video-signaling-2.5.2.post2/types_aiobotocore_kinesis_video_signaling/py.typed
--rw-r--r--   0 vlad      (1000) vlad      (1000)     2513 2023-08-04 13:42:03.000000 types-aiobotocore-kinesis-video-signaling-2.5.2.post2/types_aiobotocore_kinesis_video_signaling/type_defs.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)     2510 2023-08-04 13:42:03.000000 types-aiobotocore-kinesis-video-signaling-2.5.2.post2/types_aiobotocore_kinesis_video_signaling/type_defs.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)       65 2023-08-04 13:42:03.000000 types-aiobotocore-kinesis-video-signaling-2.5.2.post2/types_aiobotocore_kinesis_video_signaling/version.py
-drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:14.166643 types-aiobotocore-kinesis-video-signaling-2.5.2.post2/types_aiobotocore_kinesis_video_signaling.egg-info/
--rw-r--r--   0 vlad      (1000) vlad      (1000)    13121 2023-08-04 13:59:14.000000 types-aiobotocore-kinesis-video-signaling-2.5.2.post2/types_aiobotocore_kinesis_video_signaling.egg-info/PKG-INFO
--rw-r--r--   0 vlad      (1000) vlad      (1000)     1006 2023-08-04 13:59:14.000000 types-aiobotocore-kinesis-video-signaling-2.5.2.post2/types_aiobotocore_kinesis_video_signaling.egg-info/SOURCES.txt
--rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:14.000000 types-aiobotocore-kinesis-video-signaling-2.5.2.post2/types_aiobotocore_kinesis_video_signaling.egg-info/dependency_links.txt
--rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:14.000000 types-aiobotocore-kinesis-video-signaling-2.5.2.post2/types_aiobotocore_kinesis_video_signaling.egg-info/not-zip-safe
--rw-r--r--   0 vlad      (1000) vlad      (1000)       52 2023-08-04 13:59:14.000000 types-aiobotocore-kinesis-video-signaling-2.5.2.post2/types_aiobotocore_kinesis_video_signaling.egg-info/requires.txt
--rw-r--r--   0 vlad      (1000) vlad      (1000)       42 2023-08-04 13:59:14.000000 types-aiobotocore-kinesis-video-signaling-2.5.2.post2/types_aiobotocore_kinesis_video_signaling.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:23:57.374718 types-aiobotocore-kinesis-video-signaling-2.5.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-08 01:13:36.000000 types-aiobotocore-kinesis-video-signaling-2.5.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    13115 2023-08-08 01:23:57.370718 types-aiobotocore-kinesis-video-signaling-2.5.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    11533 2023-08-08 01:13:36.000000 types-aiobotocore-kinesis-video-signaling-2.5.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-08 01:23:57.374718 types-aiobotocore-kinesis-video-signaling-2.5.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2176 2023-08-08 01:13:36.000000 types-aiobotocore-kinesis-video-signaling-2.5.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:23:57.370718 types-aiobotocore-kinesis-video-signaling-2.5.4/types_aiobotocore_kinesis_video_signaling/
+-rw-r--r--   0 runner    (1001) docker     (123)      600 2023-08-08 01:13:36.000000 types-aiobotocore-kinesis-video-signaling-2.5.4/types_aiobotocore_kinesis_video_signaling/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      599 2023-08-08 01:13:36.000000 types-aiobotocore-kinesis-video-signaling-2.5.4/types_aiobotocore_kinesis_video_signaling/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1007 2023-08-08 01:13:36.000000 types-aiobotocore-kinesis-video-signaling-2.5.4/types_aiobotocore_kinesis_video_signaling/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6389 2023-08-08 01:13:36.000000 types-aiobotocore-kinesis-video-signaling-2.5.4/types_aiobotocore_kinesis_video_signaling/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6378 2023-08-08 01:13:36.000000 types-aiobotocore-kinesis-video-signaling-2.5.4/types_aiobotocore_kinesis_video_signaling/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8097 2023-08-08 01:13:36.000000 types-aiobotocore-kinesis-video-signaling-2.5.4/types_aiobotocore_kinesis_video_signaling/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8095 2023-08-08 01:13:36.000000 types-aiobotocore-kinesis-video-signaling-2.5.4/types_aiobotocore_kinesis_video_signaling/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 01:13:36.000000 types-aiobotocore-kinesis-video-signaling-2.5.4/types_aiobotocore_kinesis_video_signaling/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     2513 2023-08-08 01:13:36.000000 types-aiobotocore-kinesis-video-signaling-2.5.4/types_aiobotocore_kinesis_video_signaling/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2510 2023-08-08 01:13:36.000000 types-aiobotocore-kinesis-video-signaling-2.5.4/types_aiobotocore_kinesis_video_signaling/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-08-08 01:13:36.000000 types-aiobotocore-kinesis-video-signaling-2.5.4/types_aiobotocore_kinesis_video_signaling/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:23:57.370718 types-aiobotocore-kinesis-video-signaling-2.5.4/types_aiobotocore_kinesis_video_signaling.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    13115 2023-08-08 01:23:57.000000 types-aiobotocore-kinesis-video-signaling-2.5.4/types_aiobotocore_kinesis_video_signaling.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-08-08 01:23:57.000000 types-aiobotocore-kinesis-video-signaling-2.5.4/types_aiobotocore_kinesis_video_signaling.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 01:23:57.000000 types-aiobotocore-kinesis-video-signaling-2.5.4/types_aiobotocore_kinesis_video_signaling.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 01:23:57.000000 types-aiobotocore-kinesis-video-signaling-2.5.4/types_aiobotocore_kinesis_video_signaling.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-08 01:23:57.000000 types-aiobotocore-kinesis-video-signaling-2.5.4/types_aiobotocore_kinesis_video_signaling.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-08-08 01:23:57.000000 types-aiobotocore-kinesis-video-signaling-2.5.4/types_aiobotocore_kinesis_video_signaling.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-kinesis-video-signaling-2.5.2.post2/LICENSE` & `types-aiobotocore-kinesis-video-signaling-2.5.4/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-kinesis-video-signaling-2.5.2.post2/PKG-INFO` & `types-aiobotocore-kinesis-video-signaling-2.5.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-kinesis-video-signaling
-Version: 2.5.2.post2
-Summary: Type annotations for aiobotocore.KinesisVideoSignalingChannels 2.5.2 service generated with mypy-boto3-builder 7.17.2
+Version: 2.5.4
+Summary: Type annotations for aiobotocore.KinesisVideoSignalingChannels 2.5.4 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kinesis_video_signaling/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-kinesis-video-signaling.svg?color=blue)](https://pypi.org/project/types-aiobotocore-kinesis-video-signaling)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kinesis_video_signaling/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-kinesis-video-signaling)](https://pepy.tech/project/types-aiobotocore-kinesis-video-signaling)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.KinesisVideoSignalingChannels 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesis-video-signaling.html#KinesisVideoSignalingChannels)
+[aiobotocore.KinesisVideoSignalingChannels 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesis-video-signaling.html#KinesisVideoSignalingChannels)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-kinesis-video-signaling-2.5.2.post2/README.md` & `types-aiobotocore-kinesis-video-signaling-2.5.4/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-kinesis-video-signaling.svg?color=blue)](https://pypi.org/project/types-aiobotocore-kinesis-video-signaling)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kinesis_video_signaling/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-kinesis-video-signaling)](https://pepy.tech/project/types-aiobotocore-kinesis-video-signaling)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.KinesisVideoSignalingChannels 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesis-video-signaling.html#KinesisVideoSignalingChannels)
+[aiobotocore.KinesisVideoSignalingChannels 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesis-video-signaling.html#KinesisVideoSignalingChannels)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-kinesis-video-signaling-2.5.2.post2/setup.py` & `types-aiobotocore-kinesis-video-signaling-2.5.4/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-kinesis-video-signaling",
-    version="2.5.2.post2",
+    version="2.5.4",
     packages=["types_aiobotocore_kinesis_video_signaling"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.KinesisVideoSignalingChannels 2.5.2 service generated"
+        "Type annotations for aiobotocore.KinesisVideoSignalingChannels 2.5.4 service generated"
         " with mypy-boto3-builder 7.17.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
```

### Comparing `types-aiobotocore-kinesis-video-signaling-2.5.2.post2/types_aiobotocore_kinesis_video_signaling/__init__.py` & `types-aiobotocore-kinesis-video-signaling-2.5.4/types_aiobotocore_kinesis_video_signaling/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-kinesis-video-signaling-2.5.2.post2/types_aiobotocore_kinesis_video_signaling/__init__.pyi` & `types-aiobotocore-kinesis-video-signaling-2.5.4/types_aiobotocore_kinesis_video_signaling/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-kinesis-video-signaling-2.5.2.post2/types_aiobotocore_kinesis_video_signaling/client.py` & `types-aiobotocore-kinesis-video-signaling-2.5.4/types_aiobotocore_kinesis_video_signaling/client.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-kinesis-video-signaling-2.5.2.post2/types_aiobotocore_kinesis_video_signaling/client.pyi` & `types-aiobotocore-kinesis-video-signaling-2.5.4/types_aiobotocore_kinesis_video_signaling/client.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-kinesis-video-signaling-2.5.2.post2/types_aiobotocore_kinesis_video_signaling/literals.py` & `types-aiobotocore-kinesis-video-signaling-2.5.4/types_aiobotocore_kinesis_video_signaling/literals.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-kinesis-video-signaling-2.5.2.post2/types_aiobotocore_kinesis_video_signaling/literals.pyi` & `types-aiobotocore-kinesis-video-signaling-2.5.4/types_aiobotocore_kinesis_video_signaling/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-kinesis-video-signaling-2.5.2.post2/types_aiobotocore_kinesis_video_signaling/type_defs.py` & `types-aiobotocore-kinesis-video-signaling-2.5.4/types_aiobotocore_kinesis_video_signaling/type_defs.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-kinesis-video-signaling-2.5.2.post2/types_aiobotocore_kinesis_video_signaling/type_defs.pyi` & `types-aiobotocore-kinesis-video-signaling-2.5.4/types_aiobotocore_kinesis_video_signaling/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-kinesis-video-signaling-2.5.2.post2/types_aiobotocore_kinesis_video_signaling.egg-info/PKG-INFO` & `types-aiobotocore-kinesis-video-signaling-2.5.4/types_aiobotocore_kinesis_video_signaling.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-kinesis-video-signaling
-Version: 2.5.2.post2
-Summary: Type annotations for aiobotocore.KinesisVideoSignalingChannels 2.5.2 service generated with mypy-boto3-builder 7.17.2
+Version: 2.5.4
+Summary: Type annotations for aiobotocore.KinesisVideoSignalingChannels 2.5.4 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kinesis_video_signaling/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-kinesis-video-signaling.svg?color=blue)](https://pypi.org/project/types-aiobotocore-kinesis-video-signaling)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kinesis_video_signaling/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-kinesis-video-signaling)](https://pepy.tech/project/types-aiobotocore-kinesis-video-signaling)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.KinesisVideoSignalingChannels 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesis-video-signaling.html#KinesisVideoSignalingChannels)
+[aiobotocore.KinesisVideoSignalingChannels 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesis-video-signaling.html#KinesisVideoSignalingChannels)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-kinesis-video-signaling-2.5.2.post2/types_aiobotocore_kinesis_video_signaling.egg-info/SOURCES.txt` & `types-aiobotocore-kinesis-video-signaling-2.5.4/types_aiobotocore_kinesis_video_signaling.egg-info/SOURCES.txt`

 * *Files identical despite different names*


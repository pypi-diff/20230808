# Comparing `tmp/types-aiobotocore-chime-sdk-media-pipelines-2.5.2.post3.tar.gz` & `tmp/types-aiobotocore-chime-sdk-media-pipelines-2.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-chime-sdk-media-pipelines-2.5.2.post3.tar", last modified: Fri Aug  4 12:37:22 2023, max compression
+gzip compressed data, was "types-aiobotocore-chime-sdk-media-pipelines-2.5.4.tar", last modified: Tue Aug  8 01:23:23 2023, max compression
```

## Comparing `types-aiobotocore-chime-sdk-media-pipelines-2.5.2.post3.tar` & `types-aiobotocore-chime-sdk-media-pipelines-2.5.4.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:37:22.435299 types-aiobotocore-chime-sdk-media-pipelines-2.5.2.post3/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-04 12:19:17.000000 types-aiobotocore-chime-sdk-media-pipelines-2.5.2.post3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    13163 2023-08-04 12:37:22.411298 types-aiobotocore-chime-sdk-media-pipelines-2.5.2.post3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    11576 2023-08-04 12:19:17.000000 types-aiobotocore-chime-sdk-media-pipelines-2.5.2.post3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-04 12:37:22.435299 types-aiobotocore-chime-sdk-media-pipelines-2.5.2.post3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2187 2023-08-04 12:19:17.000000 types-aiobotocore-chime-sdk-media-pipelines-2.5.2.post3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:37:22.411298 types-aiobotocore-chime-sdk-media-pipelines-2.5.2.post3/types_aiobotocore_chime_sdk_media_pipelines/
--rw-r--r--   0 runner    (1001) docker     (123)      571 2023-08-04 12:19:17.000000 types-aiobotocore-chime-sdk-media-pipelines-2.5.2.post3/types_aiobotocore_chime_sdk_media_pipelines/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      570 2023-08-04 12:19:17.000000 types-aiobotocore-chime-sdk-media-pipelines-2.5.2.post3/types_aiobotocore_chime_sdk_media_pipelines/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1009 2023-08-04 12:19:17.000000 types-aiobotocore-chime-sdk-media-pipelines-2.5.2.post3/types_aiobotocore_chime_sdk_media_pipelines/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19230 2023-08-04 12:19:17.000000 types-aiobotocore-chime-sdk-media-pipelines-2.5.2.post3/types_aiobotocore_chime_sdk_media_pipelines/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    19202 2023-08-04 12:19:17.000000 types-aiobotocore-chime-sdk-media-pipelines-2.5.2.post3/types_aiobotocore_chime_sdk_media_pipelines/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    11118 2023-08-04 12:19:18.000000 types-aiobotocore-chime-sdk-media-pipelines-2.5.2.post3/types_aiobotocore_chime_sdk_media_pipelines/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    11116 2023-08-04 12:19:17.000000 types-aiobotocore-chime-sdk-media-pipelines-2.5.2.post3/types_aiobotocore_chime_sdk_media_pipelines/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 12:19:17.000000 types-aiobotocore-chime-sdk-media-pipelines-2.5.2.post3/types_aiobotocore_chime_sdk_media_pipelines/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    38685 2023-08-04 12:19:18.000000 types-aiobotocore-chime-sdk-media-pipelines-2.5.2.post3/types_aiobotocore_chime_sdk_media_pipelines/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    38640 2023-08-04 12:19:18.000000 types-aiobotocore-chime-sdk-media-pipelines-2.5.2.post3/types_aiobotocore_chime_sdk_media_pipelines/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-04 12:19:17.000000 types-aiobotocore-chime-sdk-media-pipelines-2.5.2.post3/types_aiobotocore_chime_sdk_media_pipelines/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:37:22.411298 types-aiobotocore-chime-sdk-media-pipelines-2.5.2.post3/types_aiobotocore_chime_sdk_media_pipelines.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    13163 2023-08-04 12:37:22.000000 types-aiobotocore-chime-sdk-media-pipelines-2.5.2.post3/types_aiobotocore_chime_sdk_media_pipelines.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-08-04 12:37:22.000000 types-aiobotocore-chime-sdk-media-pipelines-2.5.2.post3/types_aiobotocore_chime_sdk_media_pipelines.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 12:37:22.000000 types-aiobotocore-chime-sdk-media-pipelines-2.5.2.post3/types_aiobotocore_chime_sdk_media_pipelines.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 12:37:22.000000 types-aiobotocore-chime-sdk-media-pipelines-2.5.2.post3/types_aiobotocore_chime_sdk_media_pipelines.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-04 12:37:22.000000 types-aiobotocore-chime-sdk-media-pipelines-2.5.2.post3/types_aiobotocore_chime_sdk_media_pipelines.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-08-04 12:37:22.000000 types-aiobotocore-chime-sdk-media-pipelines-2.5.2.post3/types_aiobotocore_chime_sdk_media_pipelines.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:23:23.974623 types-aiobotocore-chime-sdk-media-pipelines-2.5.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-08 01:07:01.000000 types-aiobotocore-chime-sdk-media-pipelines-2.5.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    13164 2023-08-08 01:23:23.974623 types-aiobotocore-chime-sdk-media-pipelines-2.5.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    11583 2023-08-08 01:07:01.000000 types-aiobotocore-chime-sdk-media-pipelines-2.5.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-08 01:23:23.974623 types-aiobotocore-chime-sdk-media-pipelines-2.5.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2181 2023-08-08 01:07:01.000000 types-aiobotocore-chime-sdk-media-pipelines-2.5.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:23:23.974623 types-aiobotocore-chime-sdk-media-pipelines-2.5.4/types_aiobotocore_chime_sdk_media_pipelines/
+-rw-r--r--   0 runner    (1001) docker     (123)      571 2023-08-08 01:07:01.000000 types-aiobotocore-chime-sdk-media-pipelines-2.5.4/types_aiobotocore_chime_sdk_media_pipelines/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      570 2023-08-08 01:07:01.000000 types-aiobotocore-chime-sdk-media-pipelines-2.5.4/types_aiobotocore_chime_sdk_media_pipelines/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      997 2023-08-08 01:07:01.000000 types-aiobotocore-chime-sdk-media-pipelines-2.5.4/types_aiobotocore_chime_sdk_media_pipelines/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19230 2023-08-08 01:07:01.000000 types-aiobotocore-chime-sdk-media-pipelines-2.5.4/types_aiobotocore_chime_sdk_media_pipelines/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19202 2023-08-08 01:07:01.000000 types-aiobotocore-chime-sdk-media-pipelines-2.5.4/types_aiobotocore_chime_sdk_media_pipelines/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    11897 2023-08-08 01:07:02.000000 types-aiobotocore-chime-sdk-media-pipelines-2.5.4/types_aiobotocore_chime_sdk_media_pipelines/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11895 2023-08-08 01:07:02.000000 types-aiobotocore-chime-sdk-media-pipelines-2.5.4/types_aiobotocore_chime_sdk_media_pipelines/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 01:07:01.000000 types-aiobotocore-chime-sdk-media-pipelines-2.5.4/types_aiobotocore_chime_sdk_media_pipelines/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    40193 2023-08-08 01:07:03.000000 types-aiobotocore-chime-sdk-media-pipelines-2.5.4/types_aiobotocore_chime_sdk_media_pipelines/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40150 2023-08-08 01:07:02.000000 types-aiobotocore-chime-sdk-media-pipelines-2.5.4/types_aiobotocore_chime_sdk_media_pipelines/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-08-08 01:07:01.000000 types-aiobotocore-chime-sdk-media-pipelines-2.5.4/types_aiobotocore_chime_sdk_media_pipelines/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:23:23.974623 types-aiobotocore-chime-sdk-media-pipelines-2.5.4/types_aiobotocore_chime_sdk_media_pipelines.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    13164 2023-08-08 01:23:23.000000 types-aiobotocore-chime-sdk-media-pipelines-2.5.4/types_aiobotocore_chime_sdk_media_pipelines.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-08-08 01:23:23.000000 types-aiobotocore-chime-sdk-media-pipelines-2.5.4/types_aiobotocore_chime_sdk_media_pipelines.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 01:23:23.000000 types-aiobotocore-chime-sdk-media-pipelines-2.5.4/types_aiobotocore_chime_sdk_media_pipelines.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 01:23:23.000000 types-aiobotocore-chime-sdk-media-pipelines-2.5.4/types_aiobotocore_chime_sdk_media_pipelines.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-08 01:23:23.000000 types-aiobotocore-chime-sdk-media-pipelines-2.5.4/types_aiobotocore_chime_sdk_media_pipelines.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-08-08 01:23:23.000000 types-aiobotocore-chime-sdk-media-pipelines-2.5.4/types_aiobotocore_chime_sdk_media_pipelines.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-chime-sdk-media-pipelines-2.5.2.post3/LICENSE` & `types-aiobotocore-chime-sdk-media-pipelines-2.5.4/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-chime-sdk-media-pipelines-2.5.2.post3/PKG-INFO` & `types-aiobotocore-chime-sdk-media-pipelines-2.5.4/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-chime-sdk-media-pipelines
-Version: 2.5.2.post3
-Summary: Type annotations for aiobotocore.ChimeSDKMediaPipelines 2.5.2 service generated with mypy-boto3-builder 7.17.2
+Version: 2.5.4
+Summary: Type annotations for aiobotocore.ChimeSDKMediaPipelines 2.5.4 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_chime_sdk_media_pipelines/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-chime-sdk-media-pipelines.svg?color=blue)](https://pypi.org/project/types-aiobotocore-chime-sdk-media-pipelines)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_chime_sdk_media_pipelines/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-chime-sdk-media-pipelines)](https://pepy.tech/project/types-aiobotocore-chime-sdk-media-pipelines)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.ChimeSDKMediaPipelines 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-media-pipelines.html#ChimeSDKMediaPipelines)
+[aiobotocore.ChimeSDKMediaPipelines 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-media-pipelines.html#ChimeSDKMediaPipelines)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
@@ -271,18 +271,18 @@
 `types_aiobotocore_chime_sdk_media_pipelines.literals` module contains literals
 extracted from shapes that can be used in user code for type checking.
 
 Full list of `ChimeSDKMediaPipelines` Literals can be found in
 [docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_chime_sdk_media_pipelines/literals/).
 
 ```python
-from types_aiobotocore_chime_sdk_media_pipelines.literals import ArtifactsConcatenationStateType
+from types_aiobotocore_chime_sdk_media_pipelines.literals import ActiveSpeakerPositionType
 
 
-def check_value(value: ArtifactsConcatenationStateType) -> bool:
+def check_value(value: ActiveSpeakerPositionType) -> bool:
     ...
 ```
 
 <a id="type-definitions"></a>
 
 ### Type definitions
 
@@ -290,18 +290,20 @@
 structures and shapes assembled to typed dictionaries and unions for additional
 type checking.
 
 Full list of `ChimeSDKMediaPipelines` TypeDefs can be found in
 [docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_chime_sdk_media_pipelines/type_defs/).
 
 ```python
-from types_aiobotocore_chime_sdk_media_pipelines.type_defs import PostCallAnalyticsSettingsTypeDef
+from types_aiobotocore_chime_sdk_media_pipelines.type_defs import (
+    ActiveSpeakerOnlyConfigurationTypeDef,
+)
 
 
-def get_value() -> PostCallAnalyticsSettingsTypeDef:
+def get_value() -> ActiveSpeakerOnlyConfigurationTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-chime-sdk-media-pipelines-2.5.2.post3/README.md` & `types-aiobotocore-chime-sdk-media-pipelines-2.5.4/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-chime-sdk-media-pipelines.svg?color=blue)](https://pypi.org/project/types-aiobotocore-chime-sdk-media-pipelines)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_chime_sdk_media_pipelines/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-chime-sdk-media-pipelines)](https://pepy.tech/project/types-aiobotocore-chime-sdk-media-pipelines)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.ChimeSDKMediaPipelines 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-media-pipelines.html#ChimeSDKMediaPipelines)
+[aiobotocore.ChimeSDKMediaPipelines 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-media-pipelines.html#ChimeSDKMediaPipelines)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
@@ -239,18 +239,18 @@
 `types_aiobotocore_chime_sdk_media_pipelines.literals` module contains literals
 extracted from shapes that can be used in user code for type checking.
 
 Full list of `ChimeSDKMediaPipelines` Literals can be found in
 [docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_chime_sdk_media_pipelines/literals/).
 
 ```python
-from types_aiobotocore_chime_sdk_media_pipelines.literals import ArtifactsConcatenationStateType
+from types_aiobotocore_chime_sdk_media_pipelines.literals import ActiveSpeakerPositionType
 
 
-def check_value(value: ArtifactsConcatenationStateType) -> bool:
+def check_value(value: ActiveSpeakerPositionType) -> bool:
     ...
 ```
 
 <a id="type-definitions"></a>
 
 ### Type definitions
 
@@ -258,18 +258,20 @@
 structures and shapes assembled to typed dictionaries and unions for additional
 type checking.
 
 Full list of `ChimeSDKMediaPipelines` TypeDefs can be found in
 [docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_chime_sdk_media_pipelines/type_defs/).
 
 ```python
-from types_aiobotocore_chime_sdk_media_pipelines.type_defs import PostCallAnalyticsSettingsTypeDef
+from types_aiobotocore_chime_sdk_media_pipelines.type_defs import (
+    ActiveSpeakerOnlyConfigurationTypeDef,
+)
 
 
-def get_value() -> PostCallAnalyticsSettingsTypeDef:
+def get_value() -> ActiveSpeakerOnlyConfigurationTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-chime-sdk-media-pipelines-2.5.2.post3/setup.py` & `types-aiobotocore-chime-sdk-media-pipelines-2.5.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-chime-sdk-media-pipelines",
-    version="2.5.2.post3",
+    version="2.5.4",
     packages=["types_aiobotocore_chime_sdk_media_pipelines"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.ChimeSDKMediaPipelines 2.5.2 service generated with"
+        "Type annotations for aiobotocore.ChimeSDKMediaPipelines 2.5.4 service generated with"
         " mypy-boto3-builder 7.17.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
```

### Comparing `types-aiobotocore-chime-sdk-media-pipelines-2.5.2.post3/types_aiobotocore_chime_sdk_media_pipelines/__init__.py` & `types-aiobotocore-chime-sdk-media-pipelines-2.5.4/types_aiobotocore_chime_sdk_media_pipelines/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-chime-sdk-media-pipelines-2.5.2.post3/types_aiobotocore_chime_sdk_media_pipelines/__init__.pyi` & `types-aiobotocore-chime-sdk-media-pipelines-2.5.4/types_aiobotocore_chime_sdk_media_pipelines/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-chime-sdk-media-pipelines-2.5.2.post3/types_aiobotocore_chime_sdk_media_pipelines/__main__.py` & `types-aiobotocore-chime-sdk-media-pipelines-2.5.4/types_aiobotocore_chime_sdk_media_pipelines/__main__.py`

 * *Files 13% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.ChimeSDKMediaPipelines 2.5.2\nVersion:        "
-        " 2.5.2.post3\nBuilder version: 7.17.2\nDocs:           "
+        "Type annotations for aiobotocore.ChimeSDKMediaPipelines 2.5.4\nVersion:        "
+        " 2.5.4\nBuilder version: 7.17.2\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_chime_sdk_media_pipelines//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-media-pipelines.html#ChimeSDKMediaPipelines\nOther"
         " services:  https://pypi.org/project/boto3-stubs/\nChangelog:      "
         " https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("2.5.2.post3")
+    print("2.5.4")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `types-aiobotocore-chime-sdk-media-pipelines-2.5.2.post3/types_aiobotocore_chime_sdk_media_pipelines/client.py` & `types-aiobotocore-chime-sdk-media-pipelines-2.5.4/types_aiobotocore_chime_sdk_media_pipelines/client.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-chime-sdk-media-pipelines-2.5.2.post3/types_aiobotocore_chime_sdk_media_pipelines/client.pyi` & `types-aiobotocore-chime-sdk-media-pipelines-2.5.4/types_aiobotocore_chime_sdk_media_pipelines/client.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-chime-sdk-media-pipelines-2.5.2.post3/types_aiobotocore_chime_sdk_media_pipelines/literals.py` & `types-aiobotocore-chime-sdk-media-pipelines-2.5.4/types_aiobotocore_chime_sdk_media_pipelines/literals.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,41 +2,46 @@
 Type annotations for chime-sdk-media-pipelines service literal definitions.
 
 [Open documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_chime_sdk_media_pipelines/literals/)
 
 Usage::
 
     ```python
-    from types_aiobotocore_chime_sdk_media_pipelines.literals import ArtifactsConcatenationStateType
+    from types_aiobotocore_chime_sdk_media_pipelines.literals import ActiveSpeakerPositionType
 
-    data: ArtifactsConcatenationStateType = "Disabled"
+    data: ActiveSpeakerPositionType = "BottomLeft"
     ```
 """
 import sys
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
 
 __all__ = (
+    "ActiveSpeakerPositionType",
     "ArtifactsConcatenationStateType",
     "ArtifactsStateType",
     "AudioArtifactsConcatenationStateType",
     "AudioChannelsOptionType",
     "AudioMuxTypeType",
+    "BorderColorType",
     "CallAnalyticsLanguageCodeType",
+    "CanvasOrientationType",
     "ConcatenationSinkTypeType",
     "ConcatenationSourceTypeType",
     "ContentMuxTypeType",
     "ContentRedactionOutputType",
     "ContentShareLayoutOptionType",
     "ContentTypeType",
     "FragmentSelectorTypeType",
+    "HighlightColorType",
+    "HorizontalTilePositionType",
     "LayoutOptionType",
     "LiveConnectorMuxTypeType",
     "LiveConnectorSinkTypeType",
     "LiveConnectorSourceTypeType",
     "MediaEncodingType",
     "MediaInsightsPipelineConfigurationElementTypeType",
     "MediaPipelineSinkTypeType",
@@ -46,39 +51,48 @@
     "PartialResultsStabilityType",
     "ParticipantRoleType",
     "PresenterPositionType",
     "RealTimeAlertRuleTypeType",
     "RecordingFileFormatType",
     "ResolutionOptionType",
     "SentimentTypeType",
+    "TileOrderType",
+    "VerticalTilePositionType",
     "VideoMuxTypeType",
     "VocabularyFilterMethodType",
     "VoiceAnalyticsConfigurationStatusType",
     "ChimeSDKMediaPipelinesServiceName",
     "ServiceName",
     "ResourceServiceName",
     "RegionName",
 )
 
 
+ActiveSpeakerPositionType = Literal["BottomLeft", "BottomRight", "TopLeft", "TopRight"]
 ArtifactsConcatenationStateType = Literal["Disabled", "Enabled"]
 ArtifactsStateType = Literal["Disabled", "Enabled"]
 AudioArtifactsConcatenationStateType = Literal["Enabled"]
 AudioChannelsOptionType = Literal["Mono", "Stereo"]
 AudioMuxTypeType = Literal["AudioOnly", "AudioWithActiveSpeakerVideo", "AudioWithCompositedVideo"]
+BorderColorType = Literal["Black", "Blue", "Green", "Red", "White", "Yellow"]
 CallAnalyticsLanguageCodeType = Literal[
     "de-DE", "en-AU", "en-GB", "en-US", "es-US", "fr-CA", "fr-FR", "it-IT", "pt-BR"
 ]
+CanvasOrientationType = Literal["Landscape", "Portrait"]
 ConcatenationSinkTypeType = Literal["S3Bucket"]
 ConcatenationSourceTypeType = Literal["MediaCapturePipeline"]
 ContentMuxTypeType = Literal["ContentOnly"]
 ContentRedactionOutputType = Literal["redacted", "redacted_and_unredacted"]
-ContentShareLayoutOptionType = Literal["Horizontal", "PresenterOnly", "Vertical"]
+ContentShareLayoutOptionType = Literal[
+    "ActiveSpeakerOnly", "Horizontal", "PresenterOnly", "Vertical"
+]
 ContentTypeType = Literal["PII"]
 FragmentSelectorTypeType = Literal["ProducerTimestamp", "ServerTimestamp"]
+HighlightColorType = Literal["Black", "Blue", "Green", "Red", "White", "Yellow"]
+HorizontalTilePositionType = Literal["Bottom", "Top"]
 LayoutOptionType = Literal["GridView"]
 LiveConnectorMuxTypeType = Literal["AudioWithActiveSpeakerVideo", "AudioWithCompositedVideo"]
 LiveConnectorSinkTypeType = Literal["RTMP"]
 LiveConnectorSourceTypeType = Literal["ChimeSdkMeeting"]
 MediaEncodingType = Literal["pcm"]
 MediaInsightsPipelineConfigurationElementTypeType = Literal[
     "AmazonTranscribeCallAnalyticsProcessor",
@@ -99,14 +113,16 @@
 PartialResultsStabilityType = Literal["high", "low", "medium"]
 ParticipantRoleType = Literal["AGENT", "CUSTOMER"]
 PresenterPositionType = Literal["BottomLeft", "BottomRight", "TopLeft", "TopRight"]
 RealTimeAlertRuleTypeType = Literal["IssueDetection", "KeywordMatch", "Sentiment"]
 RecordingFileFormatType = Literal["Opus", "Wav"]
 ResolutionOptionType = Literal["FHD", "HD"]
 SentimentTypeType = Literal["NEGATIVE"]
+TileOrderType = Literal["JoinSequence", "SpeakerSequence"]
+VerticalTilePositionType = Literal["Left", "Right"]
 VideoMuxTypeType = Literal["VideoOnly"]
 VocabularyFilterMethodType = Literal["mask", "remove", "tag"]
 VoiceAnalyticsConfigurationStatusType = Literal["Disabled", "Enabled"]
 ChimeSDKMediaPipelinesServiceName = Literal["chime-sdk-media-pipelines"]
 ServiceName = Literal[
     "accessanalyzer",
     "account",
@@ -118,14 +134,15 @@
     "amplifybackend",
     "amplifyuibuilder",
     "apigateway",
     "apigatewaymanagementapi",
     "apigatewayv2",
     "appconfig",
     "appconfigdata",
+    "appfabric",
     "appflow",
     "appintegrations",
     "application-autoscaling",
     "application-insights",
     "applicationcostprofiler",
     "appmesh",
     "apprunner",
@@ -221,14 +238,15 @@
     "elasticbeanstalk",
     "elastictranscoder",
     "elb",
     "elbv2",
     "emr",
     "emr-containers",
     "emr-serverless",
+    "entityresolution",
     "es",
     "events",
     "evidently",
     "finspace",
     "finspace-data",
     "firehose",
     "fis",
@@ -307,26 +325,28 @@
     "lookoutmetrics",
     "lookoutvision",
     "m2",
     "machinelearning",
     "macie",
     "macie2",
     "managedblockchain",
+    "managedblockchain-query",
     "marketplace-catalog",
     "marketplace-entitlement",
     "marketplacecommerceanalytics",
     "mediaconnect",
     "mediaconvert",
     "medialive",
     "mediapackage",
     "mediapackage-vod",
     "mediapackagev2",
     "mediastore",
     "mediastore-data",
     "mediatailor",
+    "medical-imaging",
     "memorydb",
     "meteringmarketplace",
     "mgh",
     "mgn",
     "migration-hub-refactor-spaces",
     "migrationhub-config",
     "migrationhuborchestrator",
```

### Comparing `types-aiobotocore-chime-sdk-media-pipelines-2.5.2.post3/types_aiobotocore_chime_sdk_media_pipelines/literals.pyi` & `types-aiobotocore-chime-sdk-media-pipelines-2.5.4/types_aiobotocore_chime_sdk_media_pipelines/literals.pyi`

 * *Files 3% similar despite different names*

```diff
@@ -2,40 +2,45 @@
 Type annotations for chime-sdk-media-pipelines service literal definitions.
 
 [Open documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_chime_sdk_media_pipelines/literals/)
 
 Usage::
 
     ```python
-    from types_aiobotocore_chime_sdk_media_pipelines.literals import ArtifactsConcatenationStateType
+    from types_aiobotocore_chime_sdk_media_pipelines.literals import ActiveSpeakerPositionType
 
-    data: ArtifactsConcatenationStateType = "Disabled"
+    data: ActiveSpeakerPositionType = "BottomLeft"
     ```
 """
 import sys
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
 __all__ = (
+    "ActiveSpeakerPositionType",
     "ArtifactsConcatenationStateType",
     "ArtifactsStateType",
     "AudioArtifactsConcatenationStateType",
     "AudioChannelsOptionType",
     "AudioMuxTypeType",
+    "BorderColorType",
     "CallAnalyticsLanguageCodeType",
+    "CanvasOrientationType",
     "ConcatenationSinkTypeType",
     "ConcatenationSourceTypeType",
     "ContentMuxTypeType",
     "ContentRedactionOutputType",
     "ContentShareLayoutOptionType",
     "ContentTypeType",
     "FragmentSelectorTypeType",
+    "HighlightColorType",
+    "HorizontalTilePositionType",
     "LayoutOptionType",
     "LiveConnectorMuxTypeType",
     "LiveConnectorSinkTypeType",
     "LiveConnectorSourceTypeType",
     "MediaEncodingType",
     "MediaInsightsPipelineConfigurationElementTypeType",
     "MediaPipelineSinkTypeType",
@@ -45,38 +50,47 @@
     "PartialResultsStabilityType",
     "ParticipantRoleType",
     "PresenterPositionType",
     "RealTimeAlertRuleTypeType",
     "RecordingFileFormatType",
     "ResolutionOptionType",
     "SentimentTypeType",
+    "TileOrderType",
+    "VerticalTilePositionType",
     "VideoMuxTypeType",
     "VocabularyFilterMethodType",
     "VoiceAnalyticsConfigurationStatusType",
     "ChimeSDKMediaPipelinesServiceName",
     "ServiceName",
     "ResourceServiceName",
     "RegionName",
 )
 
+ActiveSpeakerPositionType = Literal["BottomLeft", "BottomRight", "TopLeft", "TopRight"]
 ArtifactsConcatenationStateType = Literal["Disabled", "Enabled"]
 ArtifactsStateType = Literal["Disabled", "Enabled"]
 AudioArtifactsConcatenationStateType = Literal["Enabled"]
 AudioChannelsOptionType = Literal["Mono", "Stereo"]
 AudioMuxTypeType = Literal["AudioOnly", "AudioWithActiveSpeakerVideo", "AudioWithCompositedVideo"]
+BorderColorType = Literal["Black", "Blue", "Green", "Red", "White", "Yellow"]
 CallAnalyticsLanguageCodeType = Literal[
     "de-DE", "en-AU", "en-GB", "en-US", "es-US", "fr-CA", "fr-FR", "it-IT", "pt-BR"
 ]
+CanvasOrientationType = Literal["Landscape", "Portrait"]
 ConcatenationSinkTypeType = Literal["S3Bucket"]
 ConcatenationSourceTypeType = Literal["MediaCapturePipeline"]
 ContentMuxTypeType = Literal["ContentOnly"]
 ContentRedactionOutputType = Literal["redacted", "redacted_and_unredacted"]
-ContentShareLayoutOptionType = Literal["Horizontal", "PresenterOnly", "Vertical"]
+ContentShareLayoutOptionType = Literal[
+    "ActiveSpeakerOnly", "Horizontal", "PresenterOnly", "Vertical"
+]
 ContentTypeType = Literal["PII"]
 FragmentSelectorTypeType = Literal["ProducerTimestamp", "ServerTimestamp"]
+HighlightColorType = Literal["Black", "Blue", "Green", "Red", "White", "Yellow"]
+HorizontalTilePositionType = Literal["Bottom", "Top"]
 LayoutOptionType = Literal["GridView"]
 LiveConnectorMuxTypeType = Literal["AudioWithActiveSpeakerVideo", "AudioWithCompositedVideo"]
 LiveConnectorSinkTypeType = Literal["RTMP"]
 LiveConnectorSourceTypeType = Literal["ChimeSdkMeeting"]
 MediaEncodingType = Literal["pcm"]
 MediaInsightsPipelineConfigurationElementTypeType = Literal[
     "AmazonTranscribeCallAnalyticsProcessor",
@@ -97,14 +111,16 @@
 PartialResultsStabilityType = Literal["high", "low", "medium"]
 ParticipantRoleType = Literal["AGENT", "CUSTOMER"]
 PresenterPositionType = Literal["BottomLeft", "BottomRight", "TopLeft", "TopRight"]
 RealTimeAlertRuleTypeType = Literal["IssueDetection", "KeywordMatch", "Sentiment"]
 RecordingFileFormatType = Literal["Opus", "Wav"]
 ResolutionOptionType = Literal["FHD", "HD"]
 SentimentTypeType = Literal["NEGATIVE"]
+TileOrderType = Literal["JoinSequence", "SpeakerSequence"]
+VerticalTilePositionType = Literal["Left", "Right"]
 VideoMuxTypeType = Literal["VideoOnly"]
 VocabularyFilterMethodType = Literal["mask", "remove", "tag"]
 VoiceAnalyticsConfigurationStatusType = Literal["Disabled", "Enabled"]
 ChimeSDKMediaPipelinesServiceName = Literal["chime-sdk-media-pipelines"]
 ServiceName = Literal[
     "accessanalyzer",
     "account",
@@ -116,14 +132,15 @@
     "amplifybackend",
     "amplifyuibuilder",
     "apigateway",
     "apigatewaymanagementapi",
     "apigatewayv2",
     "appconfig",
     "appconfigdata",
+    "appfabric",
     "appflow",
     "appintegrations",
     "application-autoscaling",
     "application-insights",
     "applicationcostprofiler",
     "appmesh",
     "apprunner",
@@ -219,14 +236,15 @@
     "elasticbeanstalk",
     "elastictranscoder",
     "elb",
     "elbv2",
     "emr",
     "emr-containers",
     "emr-serverless",
+    "entityresolution",
     "es",
     "events",
     "evidently",
     "finspace",
     "finspace-data",
     "firehose",
     "fis",
@@ -305,26 +323,28 @@
     "lookoutmetrics",
     "lookoutvision",
     "m2",
     "machinelearning",
     "macie",
     "macie2",
     "managedblockchain",
+    "managedblockchain-query",
     "marketplace-catalog",
     "marketplace-entitlement",
     "marketplacecommerceanalytics",
     "mediaconnect",
     "mediaconvert",
     "medialive",
     "mediapackage",
     "mediapackage-vod",
     "mediapackagev2",
     "mediastore",
     "mediastore-data",
     "mediatailor",
+    "medical-imaging",
     "memorydb",
     "meteringmarketplace",
     "mgh",
     "mgn",
     "migration-hub-refactor-spaces",
     "migrationhub-config",
     "migrationhuborchestrator",
```

### Comparing `types-aiobotocore-chime-sdk-media-pipelines-2.5.2.post3/types_aiobotocore_chime_sdk_media_pipelines/type_defs.py` & `types-aiobotocore-chime-sdk-media-pipelines-2.5.4/types_aiobotocore_chime_sdk_media_pipelines/type_defs.pyi`

 * *Files 3% similar despite different names*

```diff
@@ -2,57 +2,64 @@
 Type annotations for chime-sdk-media-pipelines service type definitions.
 
 [Open documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_chime_sdk_media_pipelines/type_defs/)
 
 Usage::
 
     ```python
-    from types_aiobotocore_chime_sdk_media_pipelines.type_defs import PostCallAnalyticsSettingsTypeDef
+    from types_aiobotocore_chime_sdk_media_pipelines.type_defs import ActiveSpeakerOnlyConfigurationTypeDef
 
-    data: PostCallAnalyticsSettingsTypeDef = ...
+    data: ActiveSpeakerOnlyConfigurationTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, List, Mapping, Sequence, Union
 
 from .literals import (
+    ActiveSpeakerPositionType,
     ArtifactsConcatenationStateType,
     ArtifactsStateType,
     AudioChannelsOptionType,
     AudioMuxTypeType,
+    BorderColorType,
     CallAnalyticsLanguageCodeType,
+    CanvasOrientationType,
     ContentRedactionOutputType,
     ContentShareLayoutOptionType,
     FragmentSelectorTypeType,
+    HighlightColorType,
+    HorizontalTilePositionType,
     LiveConnectorMuxTypeType,
     MediaInsightsPipelineConfigurationElementTypeType,
     MediaPipelineStatusType,
     MediaPipelineStatusUpdateType,
     PartialResultsStabilityType,
     ParticipantRoleType,
     PresenterPositionType,
     RealTimeAlertRuleTypeType,
     RecordingFileFormatType,
     ResolutionOptionType,
+    TileOrderType,
+    VerticalTilePositionType,
     VocabularyFilterMethodType,
     VoiceAnalyticsConfigurationStatusType,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
+    "ActiveSpeakerOnlyConfigurationTypeDef",
     "PostCallAnalyticsSettingsTypeDef",
     "AmazonTranscribeProcessorConfigurationTypeDef",
     "AudioConcatenationConfigurationTypeDef",
     "CompositedVideoConcatenationConfigurationTypeDef",
     "ContentConcatenationConfigurationTypeDef",
     "DataChannelConcatenationConfigurationTypeDef",
     "MeetingEventsConcatenationConfigurationTypeDef",
@@ -68,15 +75,18 @@
     "S3RecordingSinkRuntimeConfigurationTypeDef",
     "DeleteMediaCapturePipelineRequestRequestTypeDef",
     "DeleteMediaInsightsPipelineConfigurationRequestRequestTypeDef",
     "DeleteMediaPipelineRequestRequestTypeDef",
     "GetMediaCapturePipelineRequestRequestTypeDef",
     "GetMediaInsightsPipelineConfigurationRequestRequestTypeDef",
     "GetMediaPipelineRequestRequestTypeDef",
+    "HorizontalLayoutConfigurationTypeDef",
     "PresenterOnlyConfigurationTypeDef",
+    "VerticalLayoutConfigurationTypeDef",
+    "VideoAttributeTypeDef",
     "IssueDetectionConfigurationTypeDef",
     "KeywordMatchConfigurationTypeDef",
     "KinesisDataStreamSinkConfigurationTypeDef",
     "RecordingStreamConfigurationTypeDef",
     "LambdaFunctionSinkConfigurationTypeDef",
     "ListMediaCapturePipelinesRequestRequestTypeDef",
     "MediaCapturePipelineSummaryTypeDef",
@@ -143,14 +153,22 @@
     "CreateMediaCapturePipelineResponseTypeDef",
     "GetMediaCapturePipelineResponseTypeDef",
     "CreateMediaLiveConnectorPipelineResponseTypeDef",
     "MediaPipelineTypeDef",
     "GetMediaPipelineResponseTypeDef",
 )
 
+ActiveSpeakerOnlyConfigurationTypeDef = TypedDict(
+    "ActiveSpeakerOnlyConfigurationTypeDef",
+    {
+        "ActiveSpeakerPosition": ActiveSpeakerPositionType,
+    },
+    total=False,
+)
+
 _RequiredPostCallAnalyticsSettingsTypeDef = TypedDict(
     "_RequiredPostCallAnalyticsSettingsTypeDef",
     {
         "OutputLocation": str,
         "DataAccessRoleArn": str,
     },
 )
@@ -159,53 +177,43 @@
     {
         "ContentRedactionOutput": ContentRedactionOutputType,
         "OutputEncryptionKMSKeyId": str,
     },
     total=False,
 )
 
-
 class PostCallAnalyticsSettingsTypeDef(
     _RequiredPostCallAnalyticsSettingsTypeDef, _OptionalPostCallAnalyticsSettingsTypeDef
 ):
     pass
 
-
-_RequiredAmazonTranscribeProcessorConfigurationTypeDef = TypedDict(
-    "_RequiredAmazonTranscribeProcessorConfigurationTypeDef",
+AmazonTranscribeProcessorConfigurationTypeDef = TypedDict(
+    "AmazonTranscribeProcessorConfigurationTypeDef",
     {
         "LanguageCode": CallAnalyticsLanguageCodeType,
-    },
-)
-_OptionalAmazonTranscribeProcessorConfigurationTypeDef = TypedDict(
-    "_OptionalAmazonTranscribeProcessorConfigurationTypeDef",
-    {
         "VocabularyName": str,
         "VocabularyFilterName": str,
         "VocabularyFilterMethod": VocabularyFilterMethodType,
         "ShowSpeakerLabel": bool,
         "EnablePartialResultsStabilization": bool,
         "PartialResultsStability": PartialResultsStabilityType,
         "ContentIdentificationType": Literal["PII"],
         "ContentRedactionType": Literal["PII"],
         "PiiEntityTypes": str,
         "LanguageModelName": str,
         "FilterPartialResults": bool,
+        "IdentifyLanguage": bool,
+        "LanguageOptions": str,
+        "PreferredLanguage": CallAnalyticsLanguageCodeType,
+        "VocabularyNames": str,
+        "VocabularyFilterNames": str,
     },
     total=False,
 )
 
-
-class AmazonTranscribeProcessorConfigurationTypeDef(
-    _RequiredAmazonTranscribeProcessorConfigurationTypeDef,
-    _OptionalAmazonTranscribeProcessorConfigurationTypeDef,
-):
-    pass
-
-
 AudioConcatenationConfigurationTypeDef = TypedDict(
     "AudioConcatenationConfigurationTypeDef",
     {
         "State": Literal["Enabled"],
     },
 )
 
@@ -268,63 +276,57 @@
     "_OptionalContentArtifactsConfigurationTypeDef",
     {
         "MuxType": Literal["ContentOnly"],
     },
     total=False,
 )
 
-
 class ContentArtifactsConfigurationTypeDef(
     _RequiredContentArtifactsConfigurationTypeDef, _OptionalContentArtifactsConfigurationTypeDef
 ):
     pass
 
-
 _RequiredVideoArtifactsConfigurationTypeDef = TypedDict(
     "_RequiredVideoArtifactsConfigurationTypeDef",
     {
         "State": ArtifactsStateType,
     },
 )
 _OptionalVideoArtifactsConfigurationTypeDef = TypedDict(
     "_OptionalVideoArtifactsConfigurationTypeDef",
     {
         "MuxType": Literal["VideoOnly"],
     },
     total=False,
 )
 
-
 class VideoArtifactsConfigurationTypeDef(
     _RequiredVideoArtifactsConfigurationTypeDef, _OptionalVideoArtifactsConfigurationTypeDef
 ):
     pass
 
-
 _RequiredChannelDefinitionTypeDef = TypedDict(
     "_RequiredChannelDefinitionTypeDef",
     {
         "ChannelId": int,
     },
 )
 _OptionalChannelDefinitionTypeDef = TypedDict(
     "_OptionalChannelDefinitionTypeDef",
     {
         "ParticipantRole": ParticipantRoleType,
     },
     total=False,
 )
 
-
 class ChannelDefinitionTypeDef(
     _RequiredChannelDefinitionTypeDef, _OptionalChannelDefinitionTypeDef
 ):
     pass
 
-
 S3BucketSinkConfigurationTypeDef = TypedDict(
     "S3BucketSinkConfigurationTypeDef",
     {
         "Destination": str,
     },
 )
 
@@ -393,22 +395,55 @@
 GetMediaPipelineRequestRequestTypeDef = TypedDict(
     "GetMediaPipelineRequestRequestTypeDef",
     {
         "MediaPipelineId": str,
     },
 )
 
+HorizontalLayoutConfigurationTypeDef = TypedDict(
+    "HorizontalLayoutConfigurationTypeDef",
+    {
+        "TileOrder": TileOrderType,
+        "TilePosition": HorizontalTilePositionType,
+        "TileCount": int,
+        "TileAspectRatio": str,
+    },
+    total=False,
+)
+
 PresenterOnlyConfigurationTypeDef = TypedDict(
     "PresenterOnlyConfigurationTypeDef",
     {
         "PresenterPosition": PresenterPositionType,
     },
     total=False,
 )
 
+VerticalLayoutConfigurationTypeDef = TypedDict(
+    "VerticalLayoutConfigurationTypeDef",
+    {
+        "TileOrder": TileOrderType,
+        "TilePosition": VerticalTilePositionType,
+        "TileCount": int,
+        "TileAspectRatio": str,
+    },
+    total=False,
+)
+
+VideoAttributeTypeDef = TypedDict(
+    "VideoAttributeTypeDef",
+    {
+        "CornerRadius": int,
+        "BorderColor": BorderColorType,
+        "HighlightColor": HighlightColorType,
+        "BorderThickness": int,
+    },
+    total=False,
+)
+
 IssueDetectionConfigurationTypeDef = TypedDict(
     "IssueDetectionConfigurationTypeDef",
     {
         "RuleName": str,
     },
 )
 
@@ -423,21 +458,19 @@
     "_OptionalKeywordMatchConfigurationTypeDef",
     {
         "Negate": bool,
     },
     total=False,
 )
 
-
 class KeywordMatchConfigurationTypeDef(
     _RequiredKeywordMatchConfigurationTypeDef, _OptionalKeywordMatchConfigurationTypeDef
 ):
     pass
 
-
 KinesisDataStreamSinkConfigurationTypeDef = TypedDict(
     "KinesisDataStreamSinkConfigurationTypeDef",
     {
         "InsightsTarget": str,
     },
     total=False,
 )
@@ -531,21 +564,19 @@
     {
         "AudioChannels": AudioChannelsOptionType,
         "AudioSampleRate": str,
     },
     total=False,
 )
 
-
 class LiveConnectorRTMPConfigurationTypeDef(
     _RequiredLiveConnectorRTMPConfigurationTypeDef, _OptionalLiveConnectorRTMPConfigurationTypeDef
 ):
     pass
 
-
 S3RecordingSinkConfigurationTypeDef = TypedDict(
     "S3RecordingSinkConfigurationTypeDef",
     {
         "Destination": str,
         "RecordingFileFormat": RecordingFileFormatType,
     },
     total=False,
@@ -632,22 +663,20 @@
         "FilterPartialResults": bool,
         "PostCallAnalyticsSettings": PostCallAnalyticsSettingsTypeDef,
         "CallAnalyticsStreamCategories": Sequence[str],
     },
     total=False,
 )
 
-
 class AmazonTranscribeCallAnalyticsProcessorConfigurationTypeDef(
     _RequiredAmazonTranscribeCallAnalyticsProcessorConfigurationTypeDef,
     _OptionalAmazonTranscribeCallAnalyticsProcessorConfigurationTypeDef,
 ):
     pass
 
-
 ArtifactsConcatenationConfigurationTypeDef = TypedDict(
     "ArtifactsConcatenationConfigurationTypeDef",
     {
         "Audio": AudioConcatenationConfigurationTypeDef,
         "Video": VideoConcatenationConfigurationTypeDef,
         "Content": ContentConcatenationConfigurationTypeDef,
         "DataChannel": DataChannelConcatenationConfigurationTypeDef,
@@ -667,21 +696,19 @@
     "_OptionalStreamChannelDefinitionTypeDef",
     {
         "ChannelDefinitions": Sequence[ChannelDefinitionTypeDef],
     },
     total=False,
 )
 
-
 class StreamChannelDefinitionTypeDef(
     _RequiredStreamChannelDefinitionTypeDef, _OptionalStreamChannelDefinitionTypeDef
 ):
     pass
 
-
 ConcatenationSinkTypeDef = TypedDict(
     "ConcatenationSinkTypeDef",
     {
         "Type": Literal["S3Bucket"],
         "S3BucketSinkConfiguration": S3BucketSinkConfigurationTypeDef,
     },
 )
@@ -715,25 +742,28 @@
         "ContentShareLayout": ContentShareLayoutOptionType,
     },
 )
 _OptionalGridViewConfigurationTypeDef = TypedDict(
     "_OptionalGridViewConfigurationTypeDef",
     {
         "PresenterOnlyConfiguration": PresenterOnlyConfigurationTypeDef,
+        "ActiveSpeakerOnlyConfiguration": ActiveSpeakerOnlyConfigurationTypeDef,
+        "HorizontalLayoutConfiguration": HorizontalLayoutConfigurationTypeDef,
+        "VerticalLayoutConfiguration": VerticalLayoutConfigurationTypeDef,
+        "VideoAttribute": VideoAttributeTypeDef,
+        "CanvasOrientation": CanvasOrientationType,
     },
     total=False,
 )
 
-
 class GridViewConfigurationTypeDef(
     _RequiredGridViewConfigurationTypeDef, _OptionalGridViewConfigurationTypeDef
 ):
     pass
 
-
 ListMediaCapturePipelinesResponseTypeDef = TypedDict(
     "ListMediaCapturePipelinesResponseTypeDef",
     {
         "MediaCapturePipelines": List[MediaCapturePipelineSummaryTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -779,21 +809,19 @@
         "KeywordMatchConfiguration": KeywordMatchConfigurationTypeDef,
         "SentimentConfiguration": SentimentConfigurationTypeDef,
         "IssueDetectionConfiguration": IssueDetectionConfigurationTypeDef,
     },
     total=False,
 )
 
-
 class RealTimeAlertRuleTypeDef(
     _RequiredRealTimeAlertRuleTypeDef, _OptionalRealTimeAlertRuleTypeDef
 ):
     pass
 
-
 SourceConfigurationTypeDef = TypedDict(
     "SourceConfigurationTypeDef",
     {
         "SelectedVideoStreams": SelectedVideoStreamsTypeDef,
     },
     total=False,
 )
@@ -825,22 +853,20 @@
         "LambdaFunctionSinkConfiguration": LambdaFunctionSinkConfigurationTypeDef,
         "SqsQueueSinkConfiguration": SqsQueueSinkConfigurationTypeDef,
         "SnsTopicSinkConfiguration": SnsTopicSinkConfigurationTypeDef,
     },
     total=False,
 )
 
-
 class MediaInsightsPipelineConfigurationElementTypeDef(
     _RequiredMediaInsightsPipelineConfigurationElementTypeDef,
     _OptionalMediaInsightsPipelineConfigurationElementTypeDef,
 ):
     pass
 
-
 ChimeSdkMeetingConcatenationConfigurationTypeDef = TypedDict(
     "ChimeSdkMeetingConcatenationConfigurationTypeDef",
     {
         "ArtifactsConfiguration": ArtifactsConcatenationConfigurationTypeDef,
     },
 )
 
@@ -855,21 +881,19 @@
     "_OptionalStreamConfigurationTypeDef",
     {
         "FragmentNumber": str,
     },
     total=False,
 )
 
-
 class StreamConfigurationTypeDef(
     _RequiredStreamConfigurationTypeDef, _OptionalStreamConfigurationTypeDef
 ):
     pass
 
-
 _RequiredCompositedVideoArtifactsConfigurationTypeDef = TypedDict(
     "_RequiredCompositedVideoArtifactsConfigurationTypeDef",
     {
         "GridViewConfiguration": GridViewConfigurationTypeDef,
     },
 )
 _OptionalCompositedVideoArtifactsConfigurationTypeDef = TypedDict(
@@ -877,22 +901,20 @@
     {
         "Layout": Literal["GridView"],
         "Resolution": ResolutionOptionType,
     },
     total=False,
 )
 
-
 class CompositedVideoArtifactsConfigurationTypeDef(
     _RequiredCompositedVideoArtifactsConfigurationTypeDef,
     _OptionalCompositedVideoArtifactsConfigurationTypeDef,
 ):
     pass
 
-
 RealTimeAlertConfigurationTypeDef = TypedDict(
     "RealTimeAlertConfigurationTypeDef",
     {
         "Disabled": bool,
         "Rules": Sequence[RealTimeAlertRuleTypeDef],
     },
     total=False,
@@ -935,21 +957,19 @@
     "_OptionalArtifactsConfigurationTypeDef",
     {
         "CompositedVideo": CompositedVideoArtifactsConfigurationTypeDef,
     },
     total=False,
 )
 
-
 class ArtifactsConfigurationTypeDef(
     _RequiredArtifactsConfigurationTypeDef, _OptionalArtifactsConfigurationTypeDef
 ):
     pass
 
-
 _RequiredChimeSdkMeetingLiveConnectorConfigurationTypeDef = TypedDict(
     "_RequiredChimeSdkMeetingLiveConnectorConfigurationTypeDef",
     {
         "Arn": str,
         "MuxType": LiveConnectorMuxTypeType,
     },
 )
@@ -958,22 +978,20 @@
     {
         "CompositedVideo": CompositedVideoArtifactsConfigurationTypeDef,
         "SourceConfiguration": SourceConfigurationTypeDef,
     },
     total=False,
 )
 
-
 class ChimeSdkMeetingLiveConnectorConfigurationTypeDef(
     _RequiredChimeSdkMeetingLiveConnectorConfigurationTypeDef,
     _OptionalChimeSdkMeetingLiveConnectorConfigurationTypeDef,
 ):
     pass
 
-
 _RequiredCreateMediaInsightsPipelineConfigurationRequestRequestTypeDef = TypedDict(
     "_RequiredCreateMediaInsightsPipelineConfigurationRequestRequestTypeDef",
     {
         "MediaInsightsPipelineConfigurationName": str,
         "ResourceAccessRoleArn": str,
         "Elements": Sequence[MediaInsightsPipelineConfigurationElementTypeDef],
     },
@@ -984,22 +1002,20 @@
         "RealTimeAlertConfiguration": RealTimeAlertConfigurationTypeDef,
         "Tags": Sequence[TagTypeDef],
         "ClientRequestToken": str,
     },
     total=False,
 )
 
-
 class CreateMediaInsightsPipelineConfigurationRequestRequestTypeDef(
     _RequiredCreateMediaInsightsPipelineConfigurationRequestRequestTypeDef,
     _OptionalCreateMediaInsightsPipelineConfigurationRequestRequestTypeDef,
 ):
     pass
 
-
 MediaInsightsPipelineConfigurationTypeDef = TypedDict(
     "MediaInsightsPipelineConfigurationTypeDef",
     {
         "MediaInsightsPipelineConfigurationName": str,
         "MediaInsightsPipelineConfigurationArn": str,
         "ResourceAccessRoleArn": str,
         "RealTimeAlertConfiguration": RealTimeAlertConfigurationTypeDef,
@@ -1023,22 +1039,20 @@
     "_OptionalUpdateMediaInsightsPipelineConfigurationRequestRequestTypeDef",
     {
         "RealTimeAlertConfiguration": RealTimeAlertConfigurationTypeDef,
     },
     total=False,
 )
 
-
 class UpdateMediaInsightsPipelineConfigurationRequestRequestTypeDef(
     _RequiredUpdateMediaInsightsPipelineConfigurationRequestRequestTypeDef,
     _OptionalUpdateMediaInsightsPipelineConfigurationRequestRequestTypeDef,
 ):
     pass
 
-
 KinesisVideoStreamRecordingSourceRuntimeConfigurationTypeDef = TypedDict(
     "KinesisVideoStreamRecordingSourceRuntimeConfigurationTypeDef",
     {
         "Streams": Sequence[RecordingStreamConfigurationTypeDef],
         "FragmentSelector": FragmentSelectorTypeDef,
     },
 )
@@ -1113,22 +1127,20 @@
         "S3RecordingSinkRuntimeConfiguration": S3RecordingSinkRuntimeConfigurationTypeDef,
         "Tags": Sequence[TagTypeDef],
         "ClientRequestToken": str,
     },
     total=False,
 )
 
-
 class CreateMediaInsightsPipelineRequestRequestTypeDef(
     _RequiredCreateMediaInsightsPipelineRequestRequestTypeDef,
     _OptionalCreateMediaInsightsPipelineRequestRequestTypeDef,
 ):
     pass
 
-
 MediaInsightsPipelineTypeDef = TypedDict(
     "MediaInsightsPipelineTypeDef",
     {
         "MediaPipelineId": str,
         "MediaPipelineArn": str,
         "MediaInsightsPipelineConfigurationArn": str,
         "Status": MediaPipelineStatusType,
@@ -1157,22 +1169,20 @@
     {
         "ClientRequestToken": str,
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
-
 class CreateMediaConcatenationPipelineRequestRequestTypeDef(
     _RequiredCreateMediaConcatenationPipelineRequestRequestTypeDef,
     _OptionalCreateMediaConcatenationPipelineRequestRequestTypeDef,
 ):
     pass
 
-
 MediaConcatenationPipelineTypeDef = TypedDict(
     "MediaConcatenationPipelineTypeDef",
     {
         "MediaPipelineId": str,
         "MediaPipelineArn": str,
         "Sources": List[ConcatenationSourceTypeDef],
         "Sinks": List[ConcatenationSinkTypeDef],
@@ -1198,22 +1208,20 @@
         "ClientRequestToken": str,
         "ChimeSdkMeetingConfiguration": ChimeSdkMeetingConfigurationTypeDef,
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
-
 class CreateMediaCapturePipelineRequestRequestTypeDef(
     _RequiredCreateMediaCapturePipelineRequestRequestTypeDef,
     _OptionalCreateMediaCapturePipelineRequestRequestTypeDef,
 ):
     pass
 
-
 MediaCapturePipelineTypeDef = TypedDict(
     "MediaCapturePipelineTypeDef",
     {
         "MediaPipelineId": str,
         "MediaPipelineArn": str,
         "SourceType": Literal["ChimeSdkMeeting"],
         "SourceArn": str,
@@ -1239,22 +1247,20 @@
     {
         "ClientRequestToken": str,
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
-
 class CreateMediaLiveConnectorPipelineRequestRequestTypeDef(
     _RequiredCreateMediaLiveConnectorPipelineRequestRequestTypeDef,
     _OptionalCreateMediaLiveConnectorPipelineRequestRequestTypeDef,
 ):
     pass
 
-
 MediaLiveConnectorPipelineTypeDef = TypedDict(
     "MediaLiveConnectorPipelineTypeDef",
     {
         "Sources": List[LiveConnectorSourceConfigurationTypeDef],
         "Sinks": List[LiveConnectorSinkConfigurationTypeDef],
         "MediaPipelineId": str,
         "MediaPipelineArn": str,
```

### Comparing `types-aiobotocore-chime-sdk-media-pipelines-2.5.2.post3/types_aiobotocore_chime_sdk_media_pipelines/type_defs.pyi` & `types-aiobotocore-chime-sdk-media-pipelines-2.5.4/types_aiobotocore_chime_sdk_media_pipelines/type_defs.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,56 +2,65 @@
 Type annotations for chime-sdk-media-pipelines service type definitions.
 
 [Open documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_chime_sdk_media_pipelines/type_defs/)
 
 Usage::
 
     ```python
-    from types_aiobotocore_chime_sdk_media_pipelines.type_defs import PostCallAnalyticsSettingsTypeDef
+    from types_aiobotocore_chime_sdk_media_pipelines.type_defs import ActiveSpeakerOnlyConfigurationTypeDef
 
-    data: PostCallAnalyticsSettingsTypeDef = ...
+    data: ActiveSpeakerOnlyConfigurationTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, List, Mapping, Sequence, Union
 
 from .literals import (
+    ActiveSpeakerPositionType,
     ArtifactsConcatenationStateType,
     ArtifactsStateType,
     AudioChannelsOptionType,
     AudioMuxTypeType,
+    BorderColorType,
     CallAnalyticsLanguageCodeType,
+    CanvasOrientationType,
     ContentRedactionOutputType,
     ContentShareLayoutOptionType,
     FragmentSelectorTypeType,
+    HighlightColorType,
+    HorizontalTilePositionType,
     LiveConnectorMuxTypeType,
     MediaInsightsPipelineConfigurationElementTypeType,
     MediaPipelineStatusType,
     MediaPipelineStatusUpdateType,
     PartialResultsStabilityType,
     ParticipantRoleType,
     PresenterPositionType,
     RealTimeAlertRuleTypeType,
     RecordingFileFormatType,
     ResolutionOptionType,
+    TileOrderType,
+    VerticalTilePositionType,
     VocabularyFilterMethodType,
     VoiceAnalyticsConfigurationStatusType,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
+
 __all__ = (
+    "ActiveSpeakerOnlyConfigurationTypeDef",
     "PostCallAnalyticsSettingsTypeDef",
     "AmazonTranscribeProcessorConfigurationTypeDef",
     "AudioConcatenationConfigurationTypeDef",
     "CompositedVideoConcatenationConfigurationTypeDef",
     "ContentConcatenationConfigurationTypeDef",
     "DataChannelConcatenationConfigurationTypeDef",
     "MeetingEventsConcatenationConfigurationTypeDef",
@@ -67,15 +76,18 @@
     "S3RecordingSinkRuntimeConfigurationTypeDef",
     "DeleteMediaCapturePipelineRequestRequestTypeDef",
     "DeleteMediaInsightsPipelineConfigurationRequestRequestTypeDef",
     "DeleteMediaPipelineRequestRequestTypeDef",
     "GetMediaCapturePipelineRequestRequestTypeDef",
     "GetMediaInsightsPipelineConfigurationRequestRequestTypeDef",
     "GetMediaPipelineRequestRequestTypeDef",
+    "HorizontalLayoutConfigurationTypeDef",
     "PresenterOnlyConfigurationTypeDef",
+    "VerticalLayoutConfigurationTypeDef",
+    "VideoAttributeTypeDef",
     "IssueDetectionConfigurationTypeDef",
     "KeywordMatchConfigurationTypeDef",
     "KinesisDataStreamSinkConfigurationTypeDef",
     "RecordingStreamConfigurationTypeDef",
     "LambdaFunctionSinkConfigurationTypeDef",
     "ListMediaCapturePipelinesRequestRequestTypeDef",
     "MediaCapturePipelineSummaryTypeDef",
@@ -142,14 +154,22 @@
     "CreateMediaCapturePipelineResponseTypeDef",
     "GetMediaCapturePipelineResponseTypeDef",
     "CreateMediaLiveConnectorPipelineResponseTypeDef",
     "MediaPipelineTypeDef",
     "GetMediaPipelineResponseTypeDef",
 )
 
+ActiveSpeakerOnlyConfigurationTypeDef = TypedDict(
+    "ActiveSpeakerOnlyConfigurationTypeDef",
+    {
+        "ActiveSpeakerPosition": ActiveSpeakerPositionType,
+    },
+    total=False,
+)
+
 _RequiredPostCallAnalyticsSettingsTypeDef = TypedDict(
     "_RequiredPostCallAnalyticsSettingsTypeDef",
     {
         "OutputLocation": str,
         "DataAccessRoleArn": str,
     },
 )
@@ -158,49 +178,45 @@
     {
         "ContentRedactionOutput": ContentRedactionOutputType,
         "OutputEncryptionKMSKeyId": str,
     },
     total=False,
 )
 
+
 class PostCallAnalyticsSettingsTypeDef(
     _RequiredPostCallAnalyticsSettingsTypeDef, _OptionalPostCallAnalyticsSettingsTypeDef
 ):
     pass
 
-_RequiredAmazonTranscribeProcessorConfigurationTypeDef = TypedDict(
-    "_RequiredAmazonTranscribeProcessorConfigurationTypeDef",
+
+AmazonTranscribeProcessorConfigurationTypeDef = TypedDict(
+    "AmazonTranscribeProcessorConfigurationTypeDef",
     {
         "LanguageCode": CallAnalyticsLanguageCodeType,
-    },
-)
-_OptionalAmazonTranscribeProcessorConfigurationTypeDef = TypedDict(
-    "_OptionalAmazonTranscribeProcessorConfigurationTypeDef",
-    {
         "VocabularyName": str,
         "VocabularyFilterName": str,
         "VocabularyFilterMethod": VocabularyFilterMethodType,
         "ShowSpeakerLabel": bool,
         "EnablePartialResultsStabilization": bool,
         "PartialResultsStability": PartialResultsStabilityType,
         "ContentIdentificationType": Literal["PII"],
         "ContentRedactionType": Literal["PII"],
         "PiiEntityTypes": str,
         "LanguageModelName": str,
         "FilterPartialResults": bool,
+        "IdentifyLanguage": bool,
+        "LanguageOptions": str,
+        "PreferredLanguage": CallAnalyticsLanguageCodeType,
+        "VocabularyNames": str,
+        "VocabularyFilterNames": str,
     },
     total=False,
 )
 
-class AmazonTranscribeProcessorConfigurationTypeDef(
-    _RequiredAmazonTranscribeProcessorConfigurationTypeDef,
-    _OptionalAmazonTranscribeProcessorConfigurationTypeDef,
-):
-    pass
-
 AudioConcatenationConfigurationTypeDef = TypedDict(
     "AudioConcatenationConfigurationTypeDef",
     {
         "State": Literal["Enabled"],
     },
 )
 
@@ -263,57 +279,63 @@
     "_OptionalContentArtifactsConfigurationTypeDef",
     {
         "MuxType": Literal["ContentOnly"],
     },
     total=False,
 )
 
+
 class ContentArtifactsConfigurationTypeDef(
     _RequiredContentArtifactsConfigurationTypeDef, _OptionalContentArtifactsConfigurationTypeDef
 ):
     pass
 
+
 _RequiredVideoArtifactsConfigurationTypeDef = TypedDict(
     "_RequiredVideoArtifactsConfigurationTypeDef",
     {
         "State": ArtifactsStateType,
     },
 )
 _OptionalVideoArtifactsConfigurationTypeDef = TypedDict(
     "_OptionalVideoArtifactsConfigurationTypeDef",
     {
         "MuxType": Literal["VideoOnly"],
     },
     total=False,
 )
 
+
 class VideoArtifactsConfigurationTypeDef(
     _RequiredVideoArtifactsConfigurationTypeDef, _OptionalVideoArtifactsConfigurationTypeDef
 ):
     pass
 
+
 _RequiredChannelDefinitionTypeDef = TypedDict(
     "_RequiredChannelDefinitionTypeDef",
     {
         "ChannelId": int,
     },
 )
 _OptionalChannelDefinitionTypeDef = TypedDict(
     "_OptionalChannelDefinitionTypeDef",
     {
         "ParticipantRole": ParticipantRoleType,
     },
     total=False,
 )
 
+
 class ChannelDefinitionTypeDef(
     _RequiredChannelDefinitionTypeDef, _OptionalChannelDefinitionTypeDef
 ):
     pass
 
+
 S3BucketSinkConfigurationTypeDef = TypedDict(
     "S3BucketSinkConfigurationTypeDef",
     {
         "Destination": str,
     },
 )
 
@@ -382,22 +404,55 @@
 GetMediaPipelineRequestRequestTypeDef = TypedDict(
     "GetMediaPipelineRequestRequestTypeDef",
     {
         "MediaPipelineId": str,
     },
 )
 
+HorizontalLayoutConfigurationTypeDef = TypedDict(
+    "HorizontalLayoutConfigurationTypeDef",
+    {
+        "TileOrder": TileOrderType,
+        "TilePosition": HorizontalTilePositionType,
+        "TileCount": int,
+        "TileAspectRatio": str,
+    },
+    total=False,
+)
+
 PresenterOnlyConfigurationTypeDef = TypedDict(
     "PresenterOnlyConfigurationTypeDef",
     {
         "PresenterPosition": PresenterPositionType,
     },
     total=False,
 )
 
+VerticalLayoutConfigurationTypeDef = TypedDict(
+    "VerticalLayoutConfigurationTypeDef",
+    {
+        "TileOrder": TileOrderType,
+        "TilePosition": VerticalTilePositionType,
+        "TileCount": int,
+        "TileAspectRatio": str,
+    },
+    total=False,
+)
+
+VideoAttributeTypeDef = TypedDict(
+    "VideoAttributeTypeDef",
+    {
+        "CornerRadius": int,
+        "BorderColor": BorderColorType,
+        "HighlightColor": HighlightColorType,
+        "BorderThickness": int,
+    },
+    total=False,
+)
+
 IssueDetectionConfigurationTypeDef = TypedDict(
     "IssueDetectionConfigurationTypeDef",
     {
         "RuleName": str,
     },
 )
 
@@ -412,19 +467,21 @@
     "_OptionalKeywordMatchConfigurationTypeDef",
     {
         "Negate": bool,
     },
     total=False,
 )
 
+
 class KeywordMatchConfigurationTypeDef(
     _RequiredKeywordMatchConfigurationTypeDef, _OptionalKeywordMatchConfigurationTypeDef
 ):
     pass
 
+
 KinesisDataStreamSinkConfigurationTypeDef = TypedDict(
     "KinesisDataStreamSinkConfigurationTypeDef",
     {
         "InsightsTarget": str,
     },
     total=False,
 )
@@ -518,19 +575,21 @@
     {
         "AudioChannels": AudioChannelsOptionType,
         "AudioSampleRate": str,
     },
     total=False,
 )
 
+
 class LiveConnectorRTMPConfigurationTypeDef(
     _RequiredLiveConnectorRTMPConfigurationTypeDef, _OptionalLiveConnectorRTMPConfigurationTypeDef
 ):
     pass
 
+
 S3RecordingSinkConfigurationTypeDef = TypedDict(
     "S3RecordingSinkConfigurationTypeDef",
     {
         "Destination": str,
         "RecordingFileFormat": RecordingFileFormatType,
     },
     total=False,
@@ -617,20 +676,22 @@
         "FilterPartialResults": bool,
         "PostCallAnalyticsSettings": PostCallAnalyticsSettingsTypeDef,
         "CallAnalyticsStreamCategories": Sequence[str],
     },
     total=False,
 )
 
+
 class AmazonTranscribeCallAnalyticsProcessorConfigurationTypeDef(
     _RequiredAmazonTranscribeCallAnalyticsProcessorConfigurationTypeDef,
     _OptionalAmazonTranscribeCallAnalyticsProcessorConfigurationTypeDef,
 ):
     pass
 
+
 ArtifactsConcatenationConfigurationTypeDef = TypedDict(
     "ArtifactsConcatenationConfigurationTypeDef",
     {
         "Audio": AudioConcatenationConfigurationTypeDef,
         "Video": VideoConcatenationConfigurationTypeDef,
         "Content": ContentConcatenationConfigurationTypeDef,
         "DataChannel": DataChannelConcatenationConfigurationTypeDef,
@@ -650,19 +711,21 @@
     "_OptionalStreamChannelDefinitionTypeDef",
     {
         "ChannelDefinitions": Sequence[ChannelDefinitionTypeDef],
     },
     total=False,
 )
 
+
 class StreamChannelDefinitionTypeDef(
     _RequiredStreamChannelDefinitionTypeDef, _OptionalStreamChannelDefinitionTypeDef
 ):
     pass
 
+
 ConcatenationSinkTypeDef = TypedDict(
     "ConcatenationSinkTypeDef",
     {
         "Type": Literal["S3Bucket"],
         "S3BucketSinkConfiguration": S3BucketSinkConfigurationTypeDef,
     },
 )
@@ -696,23 +759,30 @@
         "ContentShareLayout": ContentShareLayoutOptionType,
     },
 )
 _OptionalGridViewConfigurationTypeDef = TypedDict(
     "_OptionalGridViewConfigurationTypeDef",
     {
         "PresenterOnlyConfiguration": PresenterOnlyConfigurationTypeDef,
+        "ActiveSpeakerOnlyConfiguration": ActiveSpeakerOnlyConfigurationTypeDef,
+        "HorizontalLayoutConfiguration": HorizontalLayoutConfigurationTypeDef,
+        "VerticalLayoutConfiguration": VerticalLayoutConfigurationTypeDef,
+        "VideoAttribute": VideoAttributeTypeDef,
+        "CanvasOrientation": CanvasOrientationType,
     },
     total=False,
 )
 
+
 class GridViewConfigurationTypeDef(
     _RequiredGridViewConfigurationTypeDef, _OptionalGridViewConfigurationTypeDef
 ):
     pass
 
+
 ListMediaCapturePipelinesResponseTypeDef = TypedDict(
     "ListMediaCapturePipelinesResponseTypeDef",
     {
         "MediaCapturePipelines": List[MediaCapturePipelineSummaryTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -758,19 +828,21 @@
         "KeywordMatchConfiguration": KeywordMatchConfigurationTypeDef,
         "SentimentConfiguration": SentimentConfigurationTypeDef,
         "IssueDetectionConfiguration": IssueDetectionConfigurationTypeDef,
     },
     total=False,
 )
 
+
 class RealTimeAlertRuleTypeDef(
     _RequiredRealTimeAlertRuleTypeDef, _OptionalRealTimeAlertRuleTypeDef
 ):
     pass
 
+
 SourceConfigurationTypeDef = TypedDict(
     "SourceConfigurationTypeDef",
     {
         "SelectedVideoStreams": SelectedVideoStreamsTypeDef,
     },
     total=False,
 )
@@ -802,20 +874,22 @@
         "LambdaFunctionSinkConfiguration": LambdaFunctionSinkConfigurationTypeDef,
         "SqsQueueSinkConfiguration": SqsQueueSinkConfigurationTypeDef,
         "SnsTopicSinkConfiguration": SnsTopicSinkConfigurationTypeDef,
     },
     total=False,
 )
 
+
 class MediaInsightsPipelineConfigurationElementTypeDef(
     _RequiredMediaInsightsPipelineConfigurationElementTypeDef,
     _OptionalMediaInsightsPipelineConfigurationElementTypeDef,
 ):
     pass
 
+
 ChimeSdkMeetingConcatenationConfigurationTypeDef = TypedDict(
     "ChimeSdkMeetingConcatenationConfigurationTypeDef",
     {
         "ArtifactsConfiguration": ArtifactsConcatenationConfigurationTypeDef,
     },
 )
 
@@ -830,19 +904,21 @@
     "_OptionalStreamConfigurationTypeDef",
     {
         "FragmentNumber": str,
     },
     total=False,
 )
 
+
 class StreamConfigurationTypeDef(
     _RequiredStreamConfigurationTypeDef, _OptionalStreamConfigurationTypeDef
 ):
     pass
 
+
 _RequiredCompositedVideoArtifactsConfigurationTypeDef = TypedDict(
     "_RequiredCompositedVideoArtifactsConfigurationTypeDef",
     {
         "GridViewConfiguration": GridViewConfigurationTypeDef,
     },
 )
 _OptionalCompositedVideoArtifactsConfigurationTypeDef = TypedDict(
@@ -850,20 +926,22 @@
     {
         "Layout": Literal["GridView"],
         "Resolution": ResolutionOptionType,
     },
     total=False,
 )
 
+
 class CompositedVideoArtifactsConfigurationTypeDef(
     _RequiredCompositedVideoArtifactsConfigurationTypeDef,
     _OptionalCompositedVideoArtifactsConfigurationTypeDef,
 ):
     pass
 
+
 RealTimeAlertConfigurationTypeDef = TypedDict(
     "RealTimeAlertConfigurationTypeDef",
     {
         "Disabled": bool,
         "Rules": Sequence[RealTimeAlertRuleTypeDef],
     },
     total=False,
@@ -906,19 +984,21 @@
     "_OptionalArtifactsConfigurationTypeDef",
     {
         "CompositedVideo": CompositedVideoArtifactsConfigurationTypeDef,
     },
     total=False,
 )
 
+
 class ArtifactsConfigurationTypeDef(
     _RequiredArtifactsConfigurationTypeDef, _OptionalArtifactsConfigurationTypeDef
 ):
     pass
 
+
 _RequiredChimeSdkMeetingLiveConnectorConfigurationTypeDef = TypedDict(
     "_RequiredChimeSdkMeetingLiveConnectorConfigurationTypeDef",
     {
         "Arn": str,
         "MuxType": LiveConnectorMuxTypeType,
     },
 )
@@ -927,20 +1007,22 @@
     {
         "CompositedVideo": CompositedVideoArtifactsConfigurationTypeDef,
         "SourceConfiguration": SourceConfigurationTypeDef,
     },
     total=False,
 )
 
+
 class ChimeSdkMeetingLiveConnectorConfigurationTypeDef(
     _RequiredChimeSdkMeetingLiveConnectorConfigurationTypeDef,
     _OptionalChimeSdkMeetingLiveConnectorConfigurationTypeDef,
 ):
     pass
 
+
 _RequiredCreateMediaInsightsPipelineConfigurationRequestRequestTypeDef = TypedDict(
     "_RequiredCreateMediaInsightsPipelineConfigurationRequestRequestTypeDef",
     {
         "MediaInsightsPipelineConfigurationName": str,
         "ResourceAccessRoleArn": str,
         "Elements": Sequence[MediaInsightsPipelineConfigurationElementTypeDef],
     },
@@ -951,20 +1033,22 @@
         "RealTimeAlertConfiguration": RealTimeAlertConfigurationTypeDef,
         "Tags": Sequence[TagTypeDef],
         "ClientRequestToken": str,
     },
     total=False,
 )
 
+
 class CreateMediaInsightsPipelineConfigurationRequestRequestTypeDef(
     _RequiredCreateMediaInsightsPipelineConfigurationRequestRequestTypeDef,
     _OptionalCreateMediaInsightsPipelineConfigurationRequestRequestTypeDef,
 ):
     pass
 
+
 MediaInsightsPipelineConfigurationTypeDef = TypedDict(
     "MediaInsightsPipelineConfigurationTypeDef",
     {
         "MediaInsightsPipelineConfigurationName": str,
         "MediaInsightsPipelineConfigurationArn": str,
         "ResourceAccessRoleArn": str,
         "RealTimeAlertConfiguration": RealTimeAlertConfigurationTypeDef,
@@ -988,20 +1072,22 @@
     "_OptionalUpdateMediaInsightsPipelineConfigurationRequestRequestTypeDef",
     {
         "RealTimeAlertConfiguration": RealTimeAlertConfigurationTypeDef,
     },
     total=False,
 )
 
+
 class UpdateMediaInsightsPipelineConfigurationRequestRequestTypeDef(
     _RequiredUpdateMediaInsightsPipelineConfigurationRequestRequestTypeDef,
     _OptionalUpdateMediaInsightsPipelineConfigurationRequestRequestTypeDef,
 ):
     pass
 
+
 KinesisVideoStreamRecordingSourceRuntimeConfigurationTypeDef = TypedDict(
     "KinesisVideoStreamRecordingSourceRuntimeConfigurationTypeDef",
     {
         "Streams": Sequence[RecordingStreamConfigurationTypeDef],
         "FragmentSelector": FragmentSelectorTypeDef,
     },
 )
@@ -1076,20 +1162,22 @@
         "S3RecordingSinkRuntimeConfiguration": S3RecordingSinkRuntimeConfigurationTypeDef,
         "Tags": Sequence[TagTypeDef],
         "ClientRequestToken": str,
     },
     total=False,
 )
 
+
 class CreateMediaInsightsPipelineRequestRequestTypeDef(
     _RequiredCreateMediaInsightsPipelineRequestRequestTypeDef,
     _OptionalCreateMediaInsightsPipelineRequestRequestTypeDef,
 ):
     pass
 
+
 MediaInsightsPipelineTypeDef = TypedDict(
     "MediaInsightsPipelineTypeDef",
     {
         "MediaPipelineId": str,
         "MediaPipelineArn": str,
         "MediaInsightsPipelineConfigurationArn": str,
         "Status": MediaPipelineStatusType,
@@ -1118,20 +1206,22 @@
     {
         "ClientRequestToken": str,
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
+
 class CreateMediaConcatenationPipelineRequestRequestTypeDef(
     _RequiredCreateMediaConcatenationPipelineRequestRequestTypeDef,
     _OptionalCreateMediaConcatenationPipelineRequestRequestTypeDef,
 ):
     pass
 
+
 MediaConcatenationPipelineTypeDef = TypedDict(
     "MediaConcatenationPipelineTypeDef",
     {
         "MediaPipelineId": str,
         "MediaPipelineArn": str,
         "Sources": List[ConcatenationSourceTypeDef],
         "Sinks": List[ConcatenationSinkTypeDef],
@@ -1157,20 +1247,22 @@
         "ClientRequestToken": str,
         "ChimeSdkMeetingConfiguration": ChimeSdkMeetingConfigurationTypeDef,
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
+
 class CreateMediaCapturePipelineRequestRequestTypeDef(
     _RequiredCreateMediaCapturePipelineRequestRequestTypeDef,
     _OptionalCreateMediaCapturePipelineRequestRequestTypeDef,
 ):
     pass
 
+
 MediaCapturePipelineTypeDef = TypedDict(
     "MediaCapturePipelineTypeDef",
     {
         "MediaPipelineId": str,
         "MediaPipelineArn": str,
         "SourceType": Literal["ChimeSdkMeeting"],
         "SourceArn": str,
@@ -1196,20 +1288,22 @@
     {
         "ClientRequestToken": str,
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
+
 class CreateMediaLiveConnectorPipelineRequestRequestTypeDef(
     _RequiredCreateMediaLiveConnectorPipelineRequestRequestTypeDef,
     _OptionalCreateMediaLiveConnectorPipelineRequestRequestTypeDef,
 ):
     pass
 
+
 MediaLiveConnectorPipelineTypeDef = TypedDict(
     "MediaLiveConnectorPipelineTypeDef",
     {
         "Sources": List[LiveConnectorSourceConfigurationTypeDef],
         "Sinks": List[LiveConnectorSinkConfigurationTypeDef],
         "MediaPipelineId": str,
         "MediaPipelineArn": str,
```

### Comparing `types-aiobotocore-chime-sdk-media-pipelines-2.5.2.post3/types_aiobotocore_chime_sdk_media_pipelines.egg-info/PKG-INFO` & `types-aiobotocore-chime-sdk-media-pipelines-2.5.4/types_aiobotocore_chime_sdk_media_pipelines.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-chime-sdk-media-pipelines
-Version: 2.5.2.post3
-Summary: Type annotations for aiobotocore.ChimeSDKMediaPipelines 2.5.2 service generated with mypy-boto3-builder 7.17.2
+Version: 2.5.4
+Summary: Type annotations for aiobotocore.ChimeSDKMediaPipelines 2.5.4 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_chime_sdk_media_pipelines/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-chime-sdk-media-pipelines.svg?color=blue)](https://pypi.org/project/types-aiobotocore-chime-sdk-media-pipelines)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_chime_sdk_media_pipelines/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-chime-sdk-media-pipelines)](https://pepy.tech/project/types-aiobotocore-chime-sdk-media-pipelines)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.ChimeSDKMediaPipelines 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-media-pipelines.html#ChimeSDKMediaPipelines)
+[aiobotocore.ChimeSDKMediaPipelines 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-media-pipelines.html#ChimeSDKMediaPipelines)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
@@ -271,18 +271,18 @@
 `types_aiobotocore_chime_sdk_media_pipelines.literals` module contains literals
 extracted from shapes that can be used in user code for type checking.
 
 Full list of `ChimeSDKMediaPipelines` Literals can be found in
 [docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_chime_sdk_media_pipelines/literals/).
 
 ```python
-from types_aiobotocore_chime_sdk_media_pipelines.literals import ArtifactsConcatenationStateType
+from types_aiobotocore_chime_sdk_media_pipelines.literals import ActiveSpeakerPositionType
 
 
-def check_value(value: ArtifactsConcatenationStateType) -> bool:
+def check_value(value: ActiveSpeakerPositionType) -> bool:
     ...
 ```
 
 <a id="type-definitions"></a>
 
 ### Type definitions
 
@@ -290,18 +290,20 @@
 structures and shapes assembled to typed dictionaries and unions for additional
 type checking.
 
 Full list of `ChimeSDKMediaPipelines` TypeDefs can be found in
 [docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_chime_sdk_media_pipelines/type_defs/).
 
 ```python
-from types_aiobotocore_chime_sdk_media_pipelines.type_defs import PostCallAnalyticsSettingsTypeDef
+from types_aiobotocore_chime_sdk_media_pipelines.type_defs import (
+    ActiveSpeakerOnlyConfigurationTypeDef,
+)
 
 
-def get_value() -> PostCallAnalyticsSettingsTypeDef:
+def get_value() -> ActiveSpeakerOnlyConfigurationTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-chime-sdk-media-pipelines-2.5.2.post3/types_aiobotocore_chime_sdk_media_pipelines.egg-info/SOURCES.txt` & `types-aiobotocore-chime-sdk-media-pipelines-2.5.4/types_aiobotocore_chime_sdk_media_pipelines.egg-info/SOURCES.txt`

 * *Files identical despite different names*


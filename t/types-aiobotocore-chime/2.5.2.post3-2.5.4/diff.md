# Comparing `tmp/types-aiobotocore-chime-2.5.2.post3.tar.gz` & `tmp/types-aiobotocore-chime-2.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-chime-2.5.2.post3.tar", last modified: Fri Aug  4 12:37:21 2023, max compression
+gzip compressed data, was "types-aiobotocore-chime-2.5.4.tar", last modified: Tue Aug  8 01:23:23 2023, max compression
```

## Comparing `types-aiobotocore-chime-2.5.2.post3.tar` & `types-aiobotocore-chime-2.5.4.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:37:21.699283 types-aiobotocore-chime-2.5.2.post3/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-04 12:19:09.000000 types-aiobotocore-chime-2.5.2.post3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    12873 2023-08-04 12:37:21.695283 types-aiobotocore-chime-2.5.2.post3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    11363 2023-08-04 12:19:09.000000 types-aiobotocore-chime-2.5.2.post3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-04 12:37:21.699283 types-aiobotocore-chime-2.5.2.post3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2058 2023-08-04 12:19:09.000000 types-aiobotocore-chime-2.5.2.post3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:37:21.687283 types-aiobotocore-chime-2.5.2.post3/types_aiobotocore_chime/
--rw-r--r--   0 runner    (1001) docker     (123)      771 2023-08-04 12:19:09.000000 types-aiobotocore-chime-2.5.2.post3/types_aiobotocore_chime/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      770 2023-08-04 12:19:09.000000 types-aiobotocore-chime-2.5.2.post3/types_aiobotocore_chime/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      924 2023-08-04 12:19:09.000000 types-aiobotocore-chime-2.5.2.post3/types_aiobotocore_chime/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)   127505 2023-08-04 12:19:11.000000 types-aiobotocore-chime-2.5.2.post3/types_aiobotocore_chime/client.py
--rw-r--r--   0 runner    (1001) docker     (123)   127303 2023-08-04 12:19:10.000000 types-aiobotocore-chime-2.5.2.post3/types_aiobotocore_chime/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    13503 2023-08-04 12:19:11.000000 types-aiobotocore-chime-2.5.2.post3/types_aiobotocore_chime/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    13501 2023-08-04 12:19:11.000000 types-aiobotocore-chime-2.5.2.post3/types_aiobotocore_chime/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     3120 2023-08-04 12:19:11.000000 types-aiobotocore-chime-2.5.2.post3/types_aiobotocore_chime/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     3116 2023-08-04 12:19:11.000000 types-aiobotocore-chime-2.5.2.post3/types_aiobotocore_chime/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 12:19:09.000000 types-aiobotocore-chime-2.5.2.post3/types_aiobotocore_chime/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)   144510 2023-08-04 12:19:15.000000 types-aiobotocore-chime-2.5.2.post3/types_aiobotocore_chime/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)   144351 2023-08-04 12:19:13.000000 types-aiobotocore-chime-2.5.2.post3/types_aiobotocore_chime/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-04 12:19:09.000000 types-aiobotocore-chime-2.5.2.post3/types_aiobotocore_chime/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:37:21.695283 types-aiobotocore-chime-2.5.2.post3/types_aiobotocore_chime.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    12873 2023-08-04 12:37:21.000000 types-aiobotocore-chime-2.5.2.post3/types_aiobotocore_chime.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      775 2023-08-04 12:37:21.000000 types-aiobotocore-chime-2.5.2.post3/types_aiobotocore_chime.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 12:37:21.000000 types-aiobotocore-chime-2.5.2.post3/types_aiobotocore_chime.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 12:37:21.000000 types-aiobotocore-chime-2.5.2.post3/types_aiobotocore_chime.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-04 12:37:21.000000 types-aiobotocore-chime-2.5.2.post3/types_aiobotocore_chime.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-08-04 12:37:21.000000 types-aiobotocore-chime-2.5.2.post3/types_aiobotocore_chime.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:23:23.886623 types-aiobotocore-chime-2.5.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-08 01:06:55.000000 types-aiobotocore-chime-2.5.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    12867 2023-08-08 01:23:23.886623 types-aiobotocore-chime-2.5.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    11363 2023-08-08 01:06:55.000000 types-aiobotocore-chime-2.5.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-08 01:23:23.886623 types-aiobotocore-chime-2.5.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2052 2023-08-08 01:06:54.000000 types-aiobotocore-chime-2.5.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:23:23.882623 types-aiobotocore-chime-2.5.4/types_aiobotocore_chime/
+-rw-r--r--   0 runner    (1001) docker     (123)      771 2023-08-08 01:06:55.000000 types-aiobotocore-chime-2.5.4/types_aiobotocore_chime/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      770 2023-08-08 01:06:55.000000 types-aiobotocore-chime-2.5.4/types_aiobotocore_chime/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      912 2023-08-08 01:06:55.000000 types-aiobotocore-chime-2.5.4/types_aiobotocore_chime/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   127287 2023-08-08 01:06:56.000000 types-aiobotocore-chime-2.5.4/types_aiobotocore_chime/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)   127085 2023-08-08 01:06:55.000000 types-aiobotocore-chime-2.5.4/types_aiobotocore_chime/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    13598 2023-08-08 01:06:56.000000 types-aiobotocore-chime-2.5.4/types_aiobotocore_chime/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13596 2023-08-08 01:06:56.000000 types-aiobotocore-chime-2.5.4/types_aiobotocore_chime/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     3120 2023-08-08 01:06:56.000000 types-aiobotocore-chime-2.5.4/types_aiobotocore_chime/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3116 2023-08-08 01:06:56.000000 types-aiobotocore-chime-2.5.4/types_aiobotocore_chime/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 01:06:55.000000 types-aiobotocore-chime-2.5.4/types_aiobotocore_chime/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)   144510 2023-08-08 01:06:59.000000 types-aiobotocore-chime-2.5.4/types_aiobotocore_chime/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)   144351 2023-08-08 01:06:57.000000 types-aiobotocore-chime-2.5.4/types_aiobotocore_chime/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-08-08 01:06:55.000000 types-aiobotocore-chime-2.5.4/types_aiobotocore_chime/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:23:23.886623 types-aiobotocore-chime-2.5.4/types_aiobotocore_chime.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    12867 2023-08-08 01:23:23.000000 types-aiobotocore-chime-2.5.4/types_aiobotocore_chime.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      775 2023-08-08 01:23:23.000000 types-aiobotocore-chime-2.5.4/types_aiobotocore_chime.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 01:23:23.000000 types-aiobotocore-chime-2.5.4/types_aiobotocore_chime.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 01:23:23.000000 types-aiobotocore-chime-2.5.4/types_aiobotocore_chime.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-08 01:23:23.000000 types-aiobotocore-chime-2.5.4/types_aiobotocore_chime.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-08-08 01:23:23.000000 types-aiobotocore-chime-2.5.4/types_aiobotocore_chime.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-chime-2.5.2.post3/LICENSE` & `types-aiobotocore-chime-2.5.4/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-chime-2.5.2.post3/PKG-INFO` & `types-aiobotocore-chime-2.5.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-chime
-Version: 2.5.2.post3
-Summary: Type annotations for aiobotocore.Chime 2.5.2 service generated with mypy-boto3-builder 7.17.2
+Version: 2.5.4
+Summary: Type annotations for aiobotocore.Chime 2.5.4 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_chime/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-chime.svg?color=blue)](https://pypi.org/project/types-aiobotocore-chime)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_chime/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-chime)](https://pepy.tech/project/types-aiobotocore-chime)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.Chime 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime.html#Chime)
+[aiobotocore.Chime 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime.html#Chime)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-chime-2.5.2.post3/README.md` & `types-aiobotocore-chime-2.5.4/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-chime.svg?color=blue)](https://pypi.org/project/types-aiobotocore-chime)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_chime/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-chime)](https://pepy.tech/project/types-aiobotocore-chime)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.Chime 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime.html#Chime)
+[aiobotocore.Chime 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime.html#Chime)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-chime-2.5.2.post3/setup.py` & `types-aiobotocore-chime-2.5.4/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-chime",
-    version="2.5.2.post3",
+    version="2.5.4",
     packages=["types_aiobotocore_chime"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.Chime 2.5.2 service generated with mypy-boto3-builder"
+        "Type annotations for aiobotocore.Chime 2.5.4 service generated with mypy-boto3-builder"
         " 7.17.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
```

### Comparing `types-aiobotocore-chime-2.5.2.post3/types_aiobotocore_chime/__init__.py` & `types-aiobotocore-chime-2.5.4/types_aiobotocore_chime/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-chime-2.5.2.post3/types_aiobotocore_chime/__init__.pyi` & `types-aiobotocore-chime-2.5.4/types_aiobotocore_chime/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-chime-2.5.2.post3/types_aiobotocore_chime/__main__.py` & `types-aiobotocore-chime-2.5.4/types_aiobotocore_chime/__main__.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.Chime 2.5.2\nVersion:         2.5.2.post3\nBuilder"
-        " version: 7.17.2\nDocs:           "
+        "Type annotations for aiobotocore.Chime 2.5.4\nVersion:         2.5.4\nBuilder version:"
+        " 7.17.2\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_chime//\nBoto3 docs:  "
         "    https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime.html#Chime\nOther"
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

### Comparing `types-aiobotocore-chime-2.5.2.post3/types_aiobotocore_chime/client.py` & `types-aiobotocore-chime-2.5.4/types_aiobotocore_chime/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1248,15 +1248,15 @@
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime.html#Chime.Client.get_media_capture_pipeline)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_chime/client/#get_media_capture_pipeline)
         """
 
     async def get_meeting(self, *, MeetingId: str) -> GetMeetingResponseTypeDef:
         """
-        Gets the Amazon Chime SDK meeting details for the specified meeting ID.
+        .
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime.html#Chime.Client.get_meeting)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_chime/client/#get_meeting)
         """
 
     async def get_messaging_session_endpoint(self) -> GetMessagingSessionEndpointResponseTypeDef:
         """
@@ -1464,16 +1464,15 @@
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_chime/client/#get_voice_connector_termination)
         """
 
     async def get_voice_connector_termination_health(
         self, *, VoiceConnectorId: str
     ) -> GetVoiceConnectorTerminationHealthResponseTypeDef:
         """
-        Retrieves information about the last time a SIP `OPTIONS` ping was received from
-        your SIP infrastructure for the specified Amazon Chime Voice Connector.
+        .
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime.html#Chime.Client.get_voice_connector_termination_health)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_chime/client/#get_voice_connector_termination_health)
         """
 
     async def invite_users(
         self, *, AccountId: str, UserEmailList: Sequence[str], UserType: UserTypeType = ...
@@ -1789,15 +1788,15 @@
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_chime/client/#list_supported_phone_number_countries)
         """
 
     async def list_tags_for_resource(
         self, *, ResourceARN: str
     ) -> ListTagsForResourceResponseTypeDef:
         """
-        Lists the tags applied to an Amazon Chime SDK meeting resource.
+        Lists the tags applied to an Amazon Chime SDK meeting and messaging resources.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime.html#Chime.Client.list_tags_for_resource)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_chime/client/#list_tags_for_resource)
         """
 
     async def list_users(
         self,
@@ -2118,15 +2117,15 @@
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_chime/client/#stop_meeting_transcription)
         """
 
     async def tag_attendee(
         self, *, MeetingId: str, AttendeeId: str, Tags: Sequence[TagTypeDef]
     ) -> EmptyResponseMetadataTypeDef:
         """
-        Applies the specified tags to the specified Amazon Chime SDK attendee.
+        Applies the specified tags to the specified Amazon Chime attendee.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime.html#Chime.Client.tag_attendee)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_chime/client/#tag_attendee)
         """
 
     async def tag_meeting(
         self, *, MeetingId: str, Tags: Sequence[TagTypeDef]
```

### Comparing `types-aiobotocore-chime-2.5.2.post3/types_aiobotocore_chime/client.pyi` & `types-aiobotocore-chime-2.5.4/types_aiobotocore_chime/client.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -1153,15 +1153,15 @@
         Gets an existing media capture pipeline.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime.html#Chime.Client.get_media_capture_pipeline)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_chime/client/#get_media_capture_pipeline)
         """
     async def get_meeting(self, *, MeetingId: str) -> GetMeetingResponseTypeDef:
         """
-        Gets the Amazon Chime SDK meeting details for the specified meeting ID.
+        .
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime.html#Chime.Client.get_meeting)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_chime/client/#get_meeting)
         """
     async def get_messaging_session_endpoint(self) -> GetMessagingSessionEndpointResponseTypeDef:
         """
         The details of the endpoint for the messaging session.
@@ -1348,16 +1348,15 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime.html#Chime.Client.get_voice_connector_termination)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_chime/client/#get_voice_connector_termination)
         """
     async def get_voice_connector_termination_health(
         self, *, VoiceConnectorId: str
     ) -> GetVoiceConnectorTerminationHealthResponseTypeDef:
         """
-        Retrieves information about the last time a SIP `OPTIONS` ping was received from
-        your SIP infrastructure for the specified Amazon Chime Voice Connector.
+        .
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime.html#Chime.Client.get_voice_connector_termination_health)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_chime/client/#get_voice_connector_termination_health)
         """
     async def invite_users(
         self, *, AccountId: str, UserEmailList: Sequence[str], UserType: UserTypeType = ...
     ) -> InviteUsersResponseTypeDef:
@@ -1646,15 +1645,15 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime.html#Chime.Client.list_supported_phone_number_countries)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_chime/client/#list_supported_phone_number_countries)
         """
     async def list_tags_for_resource(
         self, *, ResourceARN: str
     ) -> ListTagsForResourceResponseTypeDef:
         """
-        Lists the tags applied to an Amazon Chime SDK meeting resource.
+        Lists the tags applied to an Amazon Chime SDK meeting and messaging resources.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime.html#Chime.Client.list_tags_for_resource)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_chime/client/#list_tags_for_resource)
         """
     async def list_users(
         self,
         *,
@@ -1947,15 +1946,15 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime.html#Chime.Client.stop_meeting_transcription)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_chime/client/#stop_meeting_transcription)
         """
     async def tag_attendee(
         self, *, MeetingId: str, AttendeeId: str, Tags: Sequence[TagTypeDef]
     ) -> EmptyResponseMetadataTypeDef:
         """
-        Applies the specified tags to the specified Amazon Chime SDK attendee.
+        Applies the specified tags to the specified Amazon Chime attendee.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime.html#Chime.Client.tag_attendee)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_chime/client/#tag_attendee)
         """
     async def tag_meeting(
         self, *, MeetingId: str, Tags: Sequence[TagTypeDef]
     ) -> EmptyResponseMetadataTypeDef:
```

### Comparing `types-aiobotocore-chime-2.5.2.post3/types_aiobotocore_chime/literals.py` & `types-aiobotocore-chime-2.5.4/types_aiobotocore_chime/literals.py`

 * *Files 1% similar despite different names*

```diff
@@ -206,14 +206,15 @@
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
@@ -309,14 +310,15 @@
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
@@ -395,26 +397,28 @@
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

### Comparing `types-aiobotocore-chime-2.5.2.post3/types_aiobotocore_chime/literals.pyi` & `types-aiobotocore-chime-2.5.4/types_aiobotocore_chime/literals.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -204,14 +204,15 @@
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
@@ -307,14 +308,15 @@
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
@@ -393,26 +395,28 @@
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

### Comparing `types-aiobotocore-chime-2.5.2.post3/types_aiobotocore_chime/paginator.py` & `types-aiobotocore-chime-2.5.4/types_aiobotocore_chime/paginator.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-chime-2.5.2.post3/types_aiobotocore_chime/paginator.pyi` & `types-aiobotocore-chime-2.5.4/types_aiobotocore_chime/paginator.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-chime-2.5.2.post3/types_aiobotocore_chime/type_defs.py` & `types-aiobotocore-chime-2.5.4/types_aiobotocore_chime/type_defs.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-chime-2.5.2.post3/types_aiobotocore_chime/type_defs.pyi` & `types-aiobotocore-chime-2.5.4/types_aiobotocore_chime/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-chime-2.5.2.post3/types_aiobotocore_chime.egg-info/PKG-INFO` & `types-aiobotocore-chime-2.5.4/types_aiobotocore_chime.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-chime
-Version: 2.5.2.post3
-Summary: Type annotations for aiobotocore.Chime 2.5.2 service generated with mypy-boto3-builder 7.17.2
+Version: 2.5.4
+Summary: Type annotations for aiobotocore.Chime 2.5.4 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_chime/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-chime.svg?color=blue)](https://pypi.org/project/types-aiobotocore-chime)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_chime/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-chime)](https://pepy.tech/project/types-aiobotocore-chime)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.Chime 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime.html#Chime)
+[aiobotocore.Chime 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime.html#Chime)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-chime-2.5.2.post3/types_aiobotocore_chime.egg-info/SOURCES.txt` & `types-aiobotocore-chime-2.5.4/types_aiobotocore_chime.egg-info/SOURCES.txt`

 * *Files identical despite different names*


# Comparing `tmp/types-aiobotocore-sqs-2.5.2.post1.tar.gz` & `tmp/types-aiobotocore-sqs-2.5.2.post2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-sqs-2.5.2.post1.tar", last modified: Wed Aug  2 14:53:03 2023, max compression
+gzip compressed data, was "types-aiobotocore-sqs-2.5.2.post2.tar", last modified: Fri Aug  4 13:59:27 2023, max compression
```

## Comparing `types-aiobotocore-sqs-2.5.2.post1.tar` & `types-aiobotocore-sqs-2.5.2.post2.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:53:03.461450 types-aiobotocore-sqs-2.5.2.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-02 14:49:57.000000 types-aiobotocore-sqs-2.5.2.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    17742 2023-08-02 14:53:03.461450 types-aiobotocore-sqs-2.5.2.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    16240 2023-08-02 14:49:57.000000 types-aiobotocore-sqs-2.5.2.post1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 14:53:03.461450 types-aiobotocore-sqs-2.5.2.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2020 2023-08-02 14:49:57.000000 types-aiobotocore-sqs-2.5.2.post1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:53:03.461450 types-aiobotocore-sqs-2.5.2.post1/types_aiobotocore_sqs/
--rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-08-02 14:49:57.000000 types-aiobotocore-sqs-2.5.2.post1/types_aiobotocore_sqs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1058 2023-08-02 14:49:57.000000 types-aiobotocore-sqs-2.5.2.post1/types_aiobotocore_sqs/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      916 2023-08-02 14:49:57.000000 types-aiobotocore-sqs-2.5.2.post1/types_aiobotocore_sqs/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19623 2023-08-02 14:49:57.000000 types-aiobotocore-sqs-2.5.2.post1/types_aiobotocore_sqs/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    19589 2023-08-02 14:49:57.000000 types-aiobotocore-sqs-2.5.2.post1/types_aiobotocore_sqs/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    10372 2023-08-02 14:49:57.000000 types-aiobotocore-sqs-2.5.2.post1/types_aiobotocore_sqs/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    10370 2023-08-02 14:49:57.000000 types-aiobotocore-sqs-2.5.2.post1/types_aiobotocore_sqs/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     3106 2023-08-02 14:49:57.000000 types-aiobotocore-sqs-2.5.2.post1/types_aiobotocore_sqs/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     3102 2023-08-02 14:49:57.000000 types-aiobotocore-sqs-2.5.2.post1/types_aiobotocore_sqs/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:49:57.000000 types-aiobotocore-sqs-2.5.2.post1/types_aiobotocore_sqs/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    20888 2023-08-02 14:49:57.000000 types-aiobotocore-sqs-2.5.2.post1/types_aiobotocore_sqs/service_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)    20847 2023-08-02 14:49:57.000000 types-aiobotocore-sqs-2.5.2.post1/types_aiobotocore_sqs/service_resource.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    25343 2023-08-02 14:49:58.000000 types-aiobotocore-sqs-2.5.2.post1/types_aiobotocore_sqs/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    25304 2023-08-02 14:49:58.000000 types-aiobotocore-sqs-2.5.2.post1/types_aiobotocore_sqs/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-02 14:49:57.000000 types-aiobotocore-sqs-2.5.2.post1/types_aiobotocore_sqs/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:53:03.461450 types-aiobotocore-sqs-2.5.2.post1/types_aiobotocore_sqs.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    17742 2023-08-02 14:53:03.000000 types-aiobotocore-sqs-2.5.2.post1/types_aiobotocore_sqs.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      822 2023-08-02 14:53:03.000000 types-aiobotocore-sqs-2.5.2.post1/types_aiobotocore_sqs.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:53:03.000000 types-aiobotocore-sqs-2.5.2.post1/types_aiobotocore_sqs.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:53:03.000000 types-aiobotocore-sqs-2.5.2.post1/types_aiobotocore_sqs.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-02 14:53:03.000000 types-aiobotocore-sqs-2.5.2.post1/types_aiobotocore_sqs.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-08-02 14:53:03.000000 types-aiobotocore-sqs-2.5.2.post1/types_aiobotocore_sqs.egg-info/top_level.txt
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:27.546643 types-aiobotocore-sqs-2.5.2.post2/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     1070 2023-08-04 13:54:01.000000 types-aiobotocore-sqs-2.5.2.post2/LICENSE
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    14902 2023-08-04 13:59:27.546643 types-aiobotocore-sqs-2.5.2.post2/PKG-INFO
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    13400 2023-08-04 13:54:01.000000 types-aiobotocore-sqs-2.5.2.post2/README.md
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       38 2023-08-04 13:59:27.546643 types-aiobotocore-sqs-2.5.2.post2/setup.cfg
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     2020 2023-08-04 13:54:01.000000 types-aiobotocore-sqs-2.5.2.post2/setup.py
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:27.546643 types-aiobotocore-sqs-2.5.2.post2/types_aiobotocore_sqs/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     1060 2023-08-04 13:54:01.000000 types-aiobotocore-sqs-2.5.2.post2/types_aiobotocore_sqs/__init__.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     1058 2023-08-04 13:54:01.000000 types-aiobotocore-sqs-2.5.2.post2/types_aiobotocore_sqs/__init__.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)      916 2023-08-04 13:54:01.000000 types-aiobotocore-sqs-2.5.2.post2/types_aiobotocore_sqs/__main__.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    19658 2023-08-04 13:54:02.000000 types-aiobotocore-sqs-2.5.2.post2/types_aiobotocore_sqs/client.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    19624 2023-08-04 13:54:02.000000 types-aiobotocore-sqs-2.5.2.post2/types_aiobotocore_sqs/client.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    10487 2023-08-04 13:54:02.000000 types-aiobotocore-sqs-2.5.2.post2/types_aiobotocore_sqs/literals.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    10485 2023-08-04 13:54:02.000000 types-aiobotocore-sqs-2.5.2.post2/types_aiobotocore_sqs/literals.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     3106 2023-08-04 13:54:02.000000 types-aiobotocore-sqs-2.5.2.post2/types_aiobotocore_sqs/paginator.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     3102 2023-08-04 13:54:02.000000 types-aiobotocore-sqs-2.5.2.post2/types_aiobotocore_sqs/paginator.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:54:01.000000 types-aiobotocore-sqs-2.5.2.post2/types_aiobotocore_sqs/py.typed
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    20941 2023-08-04 13:54:02.000000 types-aiobotocore-sqs-2.5.2.post2/types_aiobotocore_sqs/service_resource.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    20900 2023-08-04 13:54:02.000000 types-aiobotocore-sqs-2.5.2.post2/types_aiobotocore_sqs/service_resource.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    26041 2023-08-04 13:54:03.000000 types-aiobotocore-sqs-2.5.2.post2/types_aiobotocore_sqs/type_defs.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    26000 2023-08-04 13:54:03.000000 types-aiobotocore-sqs-2.5.2.post2/types_aiobotocore_sqs/type_defs.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       65 2023-08-04 13:54:01.000000 types-aiobotocore-sqs-2.5.2.post2/types_aiobotocore_sqs/version.py
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:27.546643 types-aiobotocore-sqs-2.5.2.post2/types_aiobotocore_sqs.egg-info/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    14902 2023-08-04 13:59:27.000000 types-aiobotocore-sqs-2.5.2.post2/types_aiobotocore_sqs.egg-info/PKG-INFO
+-rw-r--r--   0 vlad      (1000) vlad      (1000)      822 2023-08-04 13:59:27.000000 types-aiobotocore-sqs-2.5.2.post2/types_aiobotocore_sqs.egg-info/SOURCES.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:27.000000 types-aiobotocore-sqs-2.5.2.post2/types_aiobotocore_sqs.egg-info/dependency_links.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:27.000000 types-aiobotocore-sqs-2.5.2.post2/types_aiobotocore_sqs.egg-info/not-zip-safe
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       52 2023-08-04 13:59:27.000000 types-aiobotocore-sqs-2.5.2.post2/types_aiobotocore_sqs.egg-info/requires.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       22 2023-08-04 13:59:27.000000 types-aiobotocore-sqs-2.5.2.post2/types_aiobotocore_sqs.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-sqs-2.5.2.post1/LICENSE` & `types-aiobotocore-sqs-2.5.2.post2/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-sqs-2.5.2.post1/PKG-INFO` & `types-aiobotocore-sqs-2.5.2.post2/README.md`

 * *Files 25% similar despite different names*

```diff
@@ -1,39 +1,7 @@
-Metadata-Version: 2.1
-Name: types-aiobotocore-sqs
-Version: 2.5.2.post1
-Summary: Type annotations for aiobotocore.SQS 2.5.2 service generated with mypy-boto3-builder 7.17.1
-Home-page: https://github.com/youtype/mypy_boto3_builder
-Author: Vlad Emelianov
-Author-email: vlad.emelianov.nz@gmail.com
-License: MIT License
-Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sqs/
-Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
-Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: aiobotocore sqs type-annotations botocore mypy typeshed autocomplete
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Intended Audience :: Developers
-Classifier: Environment :: Console
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Natural Language :: English
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.12
-Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: Implementation :: CPython
-Classifier: Typing :: Typed
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 <a id="types-aiobotocore-sqs"></a>
 
 # types-aiobotocore-sqs
 
 [![PyPI - types-aiobotocore-sqs](https://img.shields.io/pypi/v/types-aiobotocore-sqs.svg?color=blue)](https://pypi.org/project/types-aiobotocore-sqs)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-sqs.svg?color=blue)](https://pypi.org/project/types-aiobotocore-sqs)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sqs/)
@@ -47,15 +15,15 @@
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.17.1](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.17.2](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [types-aiobotocore](https://pypi.org/project/types-aiobotocore/) page and in
 [types-aiobotocore-sqs docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sqs/).
 
 See how it helps to find and fix potential bugs:
 
@@ -355,111 +323,37 @@
 <a id="literals"></a>
 
 ### Literals
 
 `types_aiobotocore_sqs.literals` module contains literals extracted from shapes
 that can be used in user code for type checking.
 
+Full list of `SQS` Literals can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sqs/literals/).
+
 ```python
-from types_aiobotocore_sqs.literals import (
-    ListDeadLetterSourceQueuesPaginatorName,
-    ListQueuesPaginatorName,
-    MessageSystemAttributeNameForSendsType,
-    MessageSystemAttributeNameType,
-    QueueAttributeFilterType,
-    QueueAttributeNameType,
-    SQSServiceName,
-    ServiceName,
-    ResourceServiceName,
-    PaginatorName,
-    RegionName,
-)
+from types_aiobotocore_sqs.literals import ListDeadLetterSourceQueuesPaginatorName
 
 
 def check_value(value: ListDeadLetterSourceQueuesPaginatorName) -> bool:
     ...
 ```
 
 <a id="type-definitions"></a>
 
 ### Type definitions
 
 `types_aiobotocore_sqs.type_defs` module contains structures and shapes
 assembled to typed dictionaries and unions for additional type checking.
 
+Full list of `SQS` TypeDefs can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sqs/type_defs/).
+
 ```python
-from types_aiobotocore_sqs.type_defs import (
-    AddPermissionRequestQueueAddPermissionTypeDef,
-    AddPermissionRequestRequestTypeDef,
-    BatchResultErrorEntryTypeDef,
-    BlobTypeDef,
-    CancelMessageMoveTaskRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
-    ChangeMessageVisibilityBatchRequestEntryTypeDef,
-    ChangeMessageVisibilityBatchResultEntryTypeDef,
-    ChangeMessageVisibilityRequestMessageChangeVisibilityTypeDef,
-    ChangeMessageVisibilityRequestRequestTypeDef,
-    CreateQueueRequestRequestTypeDef,
-    CreateQueueRequestServiceResourceCreateQueueTypeDef,
-    DeleteMessageBatchRequestEntryTypeDef,
-    DeleteMessageBatchResultEntryTypeDef,
-    DeleteMessageRequestRequestTypeDef,
-    DeleteQueueRequestRequestTypeDef,
-    GetQueueAttributesRequestRequestTypeDef,
-    GetQueueUrlRequestRequestTypeDef,
-    GetQueueUrlRequestServiceResourceGetQueueByNameTypeDef,
-    PaginatorConfigTypeDef,
-    ListDeadLetterSourceQueuesRequestRequestTypeDef,
-    ListMessageMoveTasksRequestRequestTypeDef,
-    ListMessageMoveTasksResultEntryTypeDef,
-    ListQueueTagsRequestRequestTypeDef,
-    ListQueuesRequestRequestTypeDef,
-    MessageAttributeValueOutputTypeDef,
-    PurgeQueueRequestRequestTypeDef,
-    ReceiveMessageRequestQueueReceiveMessagesTypeDef,
-    ReceiveMessageRequestRequestTypeDef,
-    RemovePermissionRequestQueueRemovePermissionTypeDef,
-    RemovePermissionRequestRequestTypeDef,
-    SendMessageBatchResultEntryTypeDef,
-    SetQueueAttributesRequestQueueSetAttributesTypeDef,
-    SetQueueAttributesRequestRequestTypeDef,
-    StartMessageMoveTaskRequestRequestTypeDef,
-    TagQueueRequestRequestTypeDef,
-    UntagQueueRequestRequestTypeDef,
-    MessageAttributeValueTypeDef,
-    MessageSystemAttributeValueTypeDef,
-    CancelMessageMoveTaskResultTypeDef,
-    CreateQueueResultTypeDef,
-    EmptyResponseMetadataTypeDef,
-    GetQueueAttributesResultTypeDef,
-    GetQueueUrlResultTypeDef,
-    ListDeadLetterSourceQueuesResultTypeDef,
-    ListQueueTagsResultTypeDef,
-    ListQueuesResultTypeDef,
-    SendMessageResultTypeDef,
-    StartMessageMoveTaskResultTypeDef,
-    ChangeMessageVisibilityBatchRequestQueueChangeMessageVisibilityBatchTypeDef,
-    ChangeMessageVisibilityBatchRequestRequestTypeDef,
-    ChangeMessageVisibilityBatchResultTypeDef,
-    DeleteMessageBatchRequestQueueDeleteMessagesTypeDef,
-    DeleteMessageBatchRequestRequestTypeDef,
-    DeleteMessageBatchResultTypeDef,
-    ListDeadLetterSourceQueuesRequestListDeadLetterSourceQueuesPaginateTypeDef,
-    ListQueuesRequestListQueuesPaginateTypeDef,
-    ListMessageMoveTasksResultTypeDef,
-    MessageTypeDef,
-    SendMessageBatchResultTypeDef,
-    MessageAttributeValueUnionTypeDef,
-    SendMessageBatchRequestEntryTypeDef,
-    SendMessageRequestQueueSendMessageTypeDef,
-    ReceiveMessageResultTypeDef,
-    SendMessageRequestRequestTypeDef,
-    SendMessageBatchRequestQueueSendMessagesTypeDef,
-    SendMessageBatchRequestRequestTypeDef,
-)
+from types_aiobotocore_sqs.type_defs import AddPermissionRequestQueueAddPermissionTypeDef
 
 
 def get_value() -> AddPermissionRequestQueueAddPermissionTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
```

### Comparing `types-aiobotocore-sqs-2.5.2.post1/README.md` & `types-aiobotocore-sqs-2.5.2.post2/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,7 +1,39 @@
+Metadata-Version: 2.1
+Name: types-aiobotocore-sqs
+Version: 2.5.2.post2
+Summary: Type annotations for aiobotocore.SQS 2.5.2 service generated with mypy-boto3-builder 7.17.2
+Home-page: https://github.com/youtype/mypy_boto3_builder
+Author: Vlad Emelianov
+Author-email: vlad.emelianov.nz@gmail.com
+License: MIT License
+Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sqs/
+Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
+Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
+Keywords: aiobotocore sqs type-annotations botocore mypy typeshed autocomplete
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Intended Audience :: Developers
+Classifier: Environment :: Console
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Natural Language :: English
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Programming Language :: Python :: Implementation :: CPython
+Classifier: Typing :: Typed
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 <a id="types-aiobotocore-sqs"></a>
 
 # types-aiobotocore-sqs
 
 [![PyPI - types-aiobotocore-sqs](https://img.shields.io/pypi/v/types-aiobotocore-sqs.svg?color=blue)](https://pypi.org/project/types-aiobotocore-sqs)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-sqs.svg?color=blue)](https://pypi.org/project/types-aiobotocore-sqs)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sqs/)
@@ -15,15 +47,15 @@
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.17.1](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.17.2](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [types-aiobotocore](https://pypi.org/project/types-aiobotocore/) page and in
 [types-aiobotocore-sqs docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sqs/).
 
 See how it helps to find and fix potential bugs:
 
@@ -323,111 +355,37 @@
 <a id="literals"></a>
 
 ### Literals
 
 `types_aiobotocore_sqs.literals` module contains literals extracted from shapes
 that can be used in user code for type checking.
 
+Full list of `SQS` Literals can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sqs/literals/).
+
 ```python
-from types_aiobotocore_sqs.literals import (
-    ListDeadLetterSourceQueuesPaginatorName,
-    ListQueuesPaginatorName,
-    MessageSystemAttributeNameForSendsType,
-    MessageSystemAttributeNameType,
-    QueueAttributeFilterType,
-    QueueAttributeNameType,
-    SQSServiceName,
-    ServiceName,
-    ResourceServiceName,
-    PaginatorName,
-    RegionName,
-)
+from types_aiobotocore_sqs.literals import ListDeadLetterSourceQueuesPaginatorName
 
 
 def check_value(value: ListDeadLetterSourceQueuesPaginatorName) -> bool:
     ...
 ```
 
 <a id="type-definitions"></a>
 
 ### Type definitions
 
 `types_aiobotocore_sqs.type_defs` module contains structures and shapes
 assembled to typed dictionaries and unions for additional type checking.
 
+Full list of `SQS` TypeDefs can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sqs/type_defs/).
+
 ```python
-from types_aiobotocore_sqs.type_defs import (
-    AddPermissionRequestQueueAddPermissionTypeDef,
-    AddPermissionRequestRequestTypeDef,
-    BatchResultErrorEntryTypeDef,
-    BlobTypeDef,
-    CancelMessageMoveTaskRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
-    ChangeMessageVisibilityBatchRequestEntryTypeDef,
-    ChangeMessageVisibilityBatchResultEntryTypeDef,
-    ChangeMessageVisibilityRequestMessageChangeVisibilityTypeDef,
-    ChangeMessageVisibilityRequestRequestTypeDef,
-    CreateQueueRequestRequestTypeDef,
-    CreateQueueRequestServiceResourceCreateQueueTypeDef,
-    DeleteMessageBatchRequestEntryTypeDef,
-    DeleteMessageBatchResultEntryTypeDef,
-    DeleteMessageRequestRequestTypeDef,
-    DeleteQueueRequestRequestTypeDef,
-    GetQueueAttributesRequestRequestTypeDef,
-    GetQueueUrlRequestRequestTypeDef,
-    GetQueueUrlRequestServiceResourceGetQueueByNameTypeDef,
-    PaginatorConfigTypeDef,
-    ListDeadLetterSourceQueuesRequestRequestTypeDef,
-    ListMessageMoveTasksRequestRequestTypeDef,
-    ListMessageMoveTasksResultEntryTypeDef,
-    ListQueueTagsRequestRequestTypeDef,
-    ListQueuesRequestRequestTypeDef,
-    MessageAttributeValueOutputTypeDef,
-    PurgeQueueRequestRequestTypeDef,
-    ReceiveMessageRequestQueueReceiveMessagesTypeDef,
-    ReceiveMessageRequestRequestTypeDef,
-    RemovePermissionRequestQueueRemovePermissionTypeDef,
-    RemovePermissionRequestRequestTypeDef,
-    SendMessageBatchResultEntryTypeDef,
-    SetQueueAttributesRequestQueueSetAttributesTypeDef,
-    SetQueueAttributesRequestRequestTypeDef,
-    StartMessageMoveTaskRequestRequestTypeDef,
-    TagQueueRequestRequestTypeDef,
-    UntagQueueRequestRequestTypeDef,
-    MessageAttributeValueTypeDef,
-    MessageSystemAttributeValueTypeDef,
-    CancelMessageMoveTaskResultTypeDef,
-    CreateQueueResultTypeDef,
-    EmptyResponseMetadataTypeDef,
-    GetQueueAttributesResultTypeDef,
-    GetQueueUrlResultTypeDef,
-    ListDeadLetterSourceQueuesResultTypeDef,
-    ListQueueTagsResultTypeDef,
-    ListQueuesResultTypeDef,
-    SendMessageResultTypeDef,
-    StartMessageMoveTaskResultTypeDef,
-    ChangeMessageVisibilityBatchRequestQueueChangeMessageVisibilityBatchTypeDef,
-    ChangeMessageVisibilityBatchRequestRequestTypeDef,
-    ChangeMessageVisibilityBatchResultTypeDef,
-    DeleteMessageBatchRequestQueueDeleteMessagesTypeDef,
-    DeleteMessageBatchRequestRequestTypeDef,
-    DeleteMessageBatchResultTypeDef,
-    ListDeadLetterSourceQueuesRequestListDeadLetterSourceQueuesPaginateTypeDef,
-    ListQueuesRequestListQueuesPaginateTypeDef,
-    ListMessageMoveTasksResultTypeDef,
-    MessageTypeDef,
-    SendMessageBatchResultTypeDef,
-    MessageAttributeValueUnionTypeDef,
-    SendMessageBatchRequestEntryTypeDef,
-    SendMessageRequestQueueSendMessageTypeDef,
-    ReceiveMessageResultTypeDef,
-    SendMessageRequestRequestTypeDef,
-    SendMessageBatchRequestQueueSendMessagesTypeDef,
-    SendMessageBatchRequestRequestTypeDef,
-)
+from types_aiobotocore_sqs.type_defs import AddPermissionRequestQueueAddPermissionTypeDef
 
 
 def get_value() -> AddPermissionRequestQueueAddPermissionTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
```

### Comparing `types-aiobotocore-sqs-2.5.2.post1/setup.py` & `types-aiobotocore-sqs-2.5.2.post2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-sqs",
-    version="2.5.2.post1",
+    version="2.5.2.post2",
     packages=["types_aiobotocore_sqs"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for aiobotocore.SQS 2.5.2 service generated with mypy-boto3-builder"
-        " 7.17.1"
+        " 7.17.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

### Comparing `types-aiobotocore-sqs-2.5.2.post1/types_aiobotocore_sqs/__init__.py` & `types-aiobotocore-sqs-2.5.2.post2/types_aiobotocore_sqs/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-sqs-2.5.2.post1/types_aiobotocore_sqs/__init__.pyi` & `types-aiobotocore-sqs-2.5.2.post2/types_aiobotocore_sqs/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-sqs-2.5.2.post1/types_aiobotocore_sqs/__main__.py` & `types-aiobotocore-sqs-2.5.2.post2/types_aiobotocore_sqs/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.SQS 2.5.2\nVersion:         2.5.2.post1\nBuilder version:"
-        " 7.17.1\nDocs:           "
+        "Type annotations for aiobotocore.SQS 2.5.2\nVersion:         2.5.2.post2\nBuilder version:"
+        " 7.17.2\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sqs//\nBoto3 docs:    "
         "  https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sqs.html#SQS\nOther"
         " services:  https://pypi.org/project/boto3-stubs/\nChangelog:      "
         " https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("2.5.2.post1")
+    print("2.5.2.post2")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `types-aiobotocore-sqs-2.5.2.post1/types_aiobotocore_sqs/client.py` & `types-aiobotocore-sqs-2.5.2.post2/types_aiobotocore_sqs/client.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -32,40 +32,37 @@
     EmptyResponseMetadataTypeDef,
     GetQueueAttributesResultTypeDef,
     GetQueueUrlResultTypeDef,
     ListDeadLetterSourceQueuesResultTypeDef,
     ListMessageMoveTasksResultTypeDef,
     ListQueuesResultTypeDef,
     ListQueueTagsResultTypeDef,
-    MessageAttributeValueUnionTypeDef,
+    MessageAttributeValueTypeDef,
     MessageSystemAttributeValueTypeDef,
     ReceiveMessageResultTypeDef,
     SendMessageBatchRequestEntryTypeDef,
     SendMessageBatchResultTypeDef,
     SendMessageResultTypeDef,
     StartMessageMoveTaskResultTypeDef,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = ("SQSClient",)
 
-
 class BotocoreClientError(BaseException):
     MSG_TEMPLATE: str
 
     def __init__(self, error_response: Mapping[str, Any], operation_name: str) -> None:
         self.response: Dict[str, Any]
         self.operation_name: str
 
-
 class Exceptions:
     BatchEntryIdsNotDistinct: Type[BotocoreClientError]
     BatchRequestTooLong: Type[BotocoreClientError]
     ClientError: Type[BotocoreClientError]
     EmptyBatchRequest: Type[BotocoreClientError]
     InvalidAttributeName: Type[BotocoreClientError]
     InvalidBatchEntryId: Type[BotocoreClientError]
@@ -78,15 +75,14 @@
     QueueDoesNotExist: Type[BotocoreClientError]
     QueueNameExists: Type[BotocoreClientError]
     ReceiptHandleIsInvalid: Type[BotocoreClientError]
     ResourceNotFoundException: Type[BotocoreClientError]
     TooManyEntriesInBatchRequest: Type[BotocoreClientError]
     UnsupportedOperation: Type[BotocoreClientError]
 
-
 class SQSClient(AioBaseClient):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sqs.html#SQS.Client)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sqs/client/)
     """
 
     meta: ClientMeta
@@ -95,197 +91,179 @@
     def exceptions(self) -> Exceptions:
         """
         SQSClient exceptions.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sqs.html#SQS.Client.exceptions)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sqs/client/#exceptions)
         """
-
     async def add_permission(
         self, *, QueueUrl: str, Label: str, AWSAccountIds: Sequence[str], Actions: Sequence[str]
     ) -> EmptyResponseMetadataTypeDef:
         """
         Adds a permission to a queue for a specific
         [principal](https://docs.aws.amazon.com/general/latest/gr/glos-chap.html#P)_.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sqs.html#SQS.Client.add_permission)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sqs/client/#add_permission)
         """
-
     def can_paginate(self, operation_name: str) -> bool:
         """
         Check if an operation can be paginated.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sqs.html#SQS.Client.can_paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sqs/client/#can_paginate)
         """
-
     async def cancel_message_move_task(
         self, *, TaskHandle: str
     ) -> CancelMessageMoveTaskResultTypeDef:
         """
         Cancels a specified message movement task.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sqs.html#SQS.Client.cancel_message_move_task)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sqs/client/#cancel_message_move_task)
         """
-
     async def change_message_visibility(
         self, *, QueueUrl: str, ReceiptHandle: str, VisibilityTimeout: int
     ) -> EmptyResponseMetadataTypeDef:
         """
         Changes the visibility timeout of a specified message in a queue to a new value.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sqs.html#SQS.Client.change_message_visibility)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sqs/client/#change_message_visibility)
         """
-
     async def change_message_visibility_batch(
         self, *, QueueUrl: str, Entries: Sequence[ChangeMessageVisibilityBatchRequestEntryTypeDef]
     ) -> ChangeMessageVisibilityBatchResultTypeDef:
         """
         Changes the visibility timeout of multiple messages.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sqs.html#SQS.Client.change_message_visibility_batch)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sqs/client/#change_message_visibility_batch)
         """
-
     async def close(self) -> None:
         """
         Closes underlying endpoint connections.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sqs.html#SQS.Client.close)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sqs/client/#close)
         """
-
     async def create_queue(
         self,
         *,
         QueueName: str,
         Attributes: Mapping[QueueAttributeNameType, str] = ...,
         tags: Mapping[str, str] = ...
     ) -> CreateQueueResultTypeDef:
         """
         Creates a new standard or FIFO queue.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sqs.html#SQS.Client.create_queue)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sqs/client/#create_queue)
         """
-
     async def delete_message(
         self, *, QueueUrl: str, ReceiptHandle: str
     ) -> EmptyResponseMetadataTypeDef:
         """
         Deletes the specified message from the specified queue.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sqs.html#SQS.Client.delete_message)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sqs/client/#delete_message)
         """
-
     async def delete_message_batch(
         self, *, QueueUrl: str, Entries: Sequence[DeleteMessageBatchRequestEntryTypeDef]
     ) -> DeleteMessageBatchResultTypeDef:
         """
         Deletes up to ten messages from the specified queue.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sqs.html#SQS.Client.delete_message_batch)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sqs/client/#delete_message_batch)
         """
-
     async def delete_queue(self, *, QueueUrl: str) -> EmptyResponseMetadataTypeDef:
         """
         Deletes the queue specified by the `QueueUrl`, regardless of the queue's
         contents.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sqs.html#SQS.Client.delete_queue)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sqs/client/#delete_queue)
         """
-
     async def generate_presigned_url(
         self,
         ClientMethod: str,
         Params: Mapping[str, Any] = ...,
         ExpiresIn: int = 3600,
         HttpMethod: str = ...,
     ) -> str:
         """
         Generate a presigned url given a client, its method, and arguments.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sqs.html#SQS.Client.generate_presigned_url)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sqs/client/#generate_presigned_url)
         """
-
     async def get_queue_attributes(
         self, *, QueueUrl: str, AttributeNames: Sequence[QueueAttributeFilterType] = ...
     ) -> GetQueueAttributesResultTypeDef:
         """
         Gets attributes for the specified queue.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sqs.html#SQS.Client.get_queue_attributes)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sqs/client/#get_queue_attributes)
         """
-
     async def get_queue_url(
         self, *, QueueName: str, QueueOwnerAWSAccountId: str = ...
     ) -> GetQueueUrlResultTypeDef:
         """
         Returns the URL of an existing Amazon SQS queue.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sqs.html#SQS.Client.get_queue_url)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sqs/client/#get_queue_url)
         """
-
     async def list_dead_letter_source_queues(
         self, *, QueueUrl: str, NextToken: str = ..., MaxResults: int = ...
     ) -> ListDeadLetterSourceQueuesResultTypeDef:
         """
         Returns a list of your queues that have the `RedrivePolicy` queue attribute
         configured with a dead-letter queue.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sqs.html#SQS.Client.list_dead_letter_source_queues)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sqs/client/#list_dead_letter_source_queues)
         """
-
     async def list_message_move_tasks(
         self, *, SourceArn: str, MaxResults: int = ...
     ) -> ListMessageMoveTasksResultTypeDef:
         """
         Gets the most recent message movement tasks (up to 10) under a specific source
         queue.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sqs.html#SQS.Client.list_message_move_tasks)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sqs/client/#list_message_move_tasks)
         """
-
     async def list_queue_tags(self, *, QueueUrl: str) -> ListQueueTagsResultTypeDef:
         """
         List all cost allocation tags added to the specified Amazon SQS queue.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sqs.html#SQS.Client.list_queue_tags)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sqs/client/#list_queue_tags)
         """
-
     async def list_queues(
         self, *, QueueNamePrefix: str = ..., NextToken: str = ..., MaxResults: int = ...
     ) -> ListQueuesResultTypeDef:
         """
         Returns a list of your queues in the current region.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sqs.html#SQS.Client.list_queues)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sqs/client/#list_queues)
         """
-
     async def purge_queue(self, *, QueueUrl: str) -> EmptyResponseMetadataTypeDef:
         """
-        Deletes the messages in a queue specified by the `QueueURL` parameter.
+        Deletes available messages in a queue (including in-flight messages) specified
+        by the `QueueURL` parameter.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sqs.html#SQS.Client.purge_queue)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sqs/client/#purge_queue)
         """
-
     async def receive_message(
         self,
         *,
         QueueUrl: str,
         AttributeNames: Sequence[QueueAttributeFilterType] = ...,
         MessageAttributeNames: Sequence[str] = ...,
         MaxNumberOfMessages: int = ...,
@@ -295,117 +273,106 @@
     ) -> ReceiveMessageResultTypeDef:
         """
         Retrieves one or more messages (up to 10), from the specified queue.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sqs.html#SQS.Client.receive_message)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sqs/client/#receive_message)
         """
-
     async def remove_permission(self, *, QueueUrl: str, Label: str) -> EmptyResponseMetadataTypeDef:
         """
         Revokes any permissions in the queue policy that matches the specified `Label`
         parameter.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sqs.html#SQS.Client.remove_permission)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sqs/client/#remove_permission)
         """
-
     async def send_message(
         self,
         *,
         QueueUrl: str,
         MessageBody: str,
         DelaySeconds: int = ...,
-        MessageAttributes: Mapping[str, MessageAttributeValueUnionTypeDef] = ...,
+        MessageAttributes: Mapping[str, MessageAttributeValueTypeDef] = ...,
         MessageSystemAttributes: Mapping[
             Literal["AWSTraceHeader"], MessageSystemAttributeValueTypeDef
         ] = ...,
         MessageDeduplicationId: str = ...,
         MessageGroupId: str = ...
     ) -> SendMessageResultTypeDef:
         """
         Delivers a message to the specified queue.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sqs.html#SQS.Client.send_message)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sqs/client/#send_message)
         """
-
     async def send_message_batch(
         self, *, QueueUrl: str, Entries: Sequence[SendMessageBatchRequestEntryTypeDef]
     ) -> SendMessageBatchResultTypeDef:
         """
         You can use `SendMessageBatch` to send up to 10 messages to the specified queue
         by assigning either identical or different values to each message (or by not
         assigning values at all).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sqs.html#SQS.Client.send_message_batch)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sqs/client/#send_message_batch)
         """
-
     async def set_queue_attributes(
         self, *, QueueUrl: str, Attributes: Mapping[QueueAttributeNameType, str]
     ) -> EmptyResponseMetadataTypeDef:
         """
         Sets the value of one or more queue attributes.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sqs.html#SQS.Client.set_queue_attributes)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sqs/client/#set_queue_attributes)
         """
-
     async def start_message_move_task(
         self, *, SourceArn: str, DestinationArn: str = ..., MaxNumberOfMessagesPerSecond: int = ...
     ) -> StartMessageMoveTaskResultTypeDef:
         """
         Starts an asynchronous task to move messages from a specified source queue to a
         specified destination queue.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sqs.html#SQS.Client.start_message_move_task)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sqs/client/#start_message_move_task)
         """
-
     async def tag_queue(
         self, *, QueueUrl: str, Tags: Mapping[str, str]
     ) -> EmptyResponseMetadataTypeDef:
         """
         Add cost allocation tags to the specified Amazon SQS queue.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sqs.html#SQS.Client.tag_queue)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sqs/client/#tag_queue)
         """
-
     async def untag_queue(
         self, *, QueueUrl: str, TagKeys: Sequence[str]
     ) -> EmptyResponseMetadataTypeDef:
         """
         Remove cost allocation tags from the specified Amazon SQS queue.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sqs.html#SQS.Client.untag_queue)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sqs/client/#untag_queue)
         """
-
     @overload
     def get_paginator(
         self, operation_name: Literal["list_dead_letter_source_queues"]
     ) -> ListDeadLetterSourceQueuesPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sqs.html#SQS.Client.get_paginator)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sqs/client/#get_paginator)
         """
-
     @overload
     def get_paginator(self, operation_name: Literal["list_queues"]) -> ListQueuesPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sqs.html#SQS.Client.get_paginator)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sqs/client/#get_paginator)
         """
-
     async def __aenter__(self) -> "SQSClient":
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sqs.html#SQS.Client)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sqs/client/)
         """
-
     async def __aexit__(self, exc_type: Any, exc_val: Any, exc_tb: Any) -> Any:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sqs.html#SQS.Client)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sqs/client/)
         """
```

### Comparing `types-aiobotocore-sqs-2.5.2.post1/types_aiobotocore_sqs/client.pyi` & `types-aiobotocore-sqs-2.5.2.post2/types_aiobotocore_sqs/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -32,37 +32,40 @@
     EmptyResponseMetadataTypeDef,
     GetQueueAttributesResultTypeDef,
     GetQueueUrlResultTypeDef,
     ListDeadLetterSourceQueuesResultTypeDef,
     ListMessageMoveTasksResultTypeDef,
     ListQueuesResultTypeDef,
     ListQueueTagsResultTypeDef,
-    MessageAttributeValueUnionTypeDef,
+    MessageAttributeValueTypeDef,
     MessageSystemAttributeValueTypeDef,
     ReceiveMessageResultTypeDef,
     SendMessageBatchRequestEntryTypeDef,
     SendMessageBatchResultTypeDef,
     SendMessageResultTypeDef,
     StartMessageMoveTaskResultTypeDef,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
+
 __all__ = ("SQSClient",)
 
+
 class BotocoreClientError(BaseException):
     MSG_TEMPLATE: str
 
     def __init__(self, error_response: Mapping[str, Any], operation_name: str) -> None:
         self.response: Dict[str, Any]
         self.operation_name: str
 
+
 class Exceptions:
     BatchEntryIdsNotDistinct: Type[BotocoreClientError]
     BatchRequestTooLong: Type[BotocoreClientError]
     ClientError: Type[BotocoreClientError]
     EmptyBatchRequest: Type[BotocoreClientError]
     InvalidAttributeName: Type[BotocoreClientError]
     InvalidBatchEntryId: Type[BotocoreClientError]
@@ -75,14 +78,15 @@
     QueueDoesNotExist: Type[BotocoreClientError]
     QueueNameExists: Type[BotocoreClientError]
     ReceiptHandleIsInvalid: Type[BotocoreClientError]
     ResourceNotFoundException: Type[BotocoreClientError]
     TooManyEntriesInBatchRequest: Type[BotocoreClientError]
     UnsupportedOperation: Type[BotocoreClientError]
 
+
 class SQSClient(AioBaseClient):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sqs.html#SQS.Client)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sqs/client/)
     """
 
     meta: ClientMeta
@@ -91,178 +95,198 @@
     def exceptions(self) -> Exceptions:
         """
         SQSClient exceptions.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sqs.html#SQS.Client.exceptions)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sqs/client/#exceptions)
         """
+
     async def add_permission(
         self, *, QueueUrl: str, Label: str, AWSAccountIds: Sequence[str], Actions: Sequence[str]
     ) -> EmptyResponseMetadataTypeDef:
         """
         Adds a permission to a queue for a specific
         [principal](https://docs.aws.amazon.com/general/latest/gr/glos-chap.html#P)_.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sqs.html#SQS.Client.add_permission)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sqs/client/#add_permission)
         """
+
     def can_paginate(self, operation_name: str) -> bool:
         """
         Check if an operation can be paginated.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sqs.html#SQS.Client.can_paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sqs/client/#can_paginate)
         """
+
     async def cancel_message_move_task(
         self, *, TaskHandle: str
     ) -> CancelMessageMoveTaskResultTypeDef:
         """
         Cancels a specified message movement task.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sqs.html#SQS.Client.cancel_message_move_task)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sqs/client/#cancel_message_move_task)
         """
+
     async def change_message_visibility(
         self, *, QueueUrl: str, ReceiptHandle: str, VisibilityTimeout: int
     ) -> EmptyResponseMetadataTypeDef:
         """
         Changes the visibility timeout of a specified message in a queue to a new value.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sqs.html#SQS.Client.change_message_visibility)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sqs/client/#change_message_visibility)
         """
+
     async def change_message_visibility_batch(
         self, *, QueueUrl: str, Entries: Sequence[ChangeMessageVisibilityBatchRequestEntryTypeDef]
     ) -> ChangeMessageVisibilityBatchResultTypeDef:
         """
         Changes the visibility timeout of multiple messages.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sqs.html#SQS.Client.change_message_visibility_batch)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sqs/client/#change_message_visibility_batch)
         """
+
     async def close(self) -> None:
         """
         Closes underlying endpoint connections.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sqs.html#SQS.Client.close)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sqs/client/#close)
         """
+
     async def create_queue(
         self,
         *,
         QueueName: str,
         Attributes: Mapping[QueueAttributeNameType, str] = ...,
         tags: Mapping[str, str] = ...
     ) -> CreateQueueResultTypeDef:
         """
         Creates a new standard or FIFO queue.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sqs.html#SQS.Client.create_queue)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sqs/client/#create_queue)
         """
+
     async def delete_message(
         self, *, QueueUrl: str, ReceiptHandle: str
     ) -> EmptyResponseMetadataTypeDef:
         """
         Deletes the specified message from the specified queue.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sqs.html#SQS.Client.delete_message)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sqs/client/#delete_message)
         """
+
     async def delete_message_batch(
         self, *, QueueUrl: str, Entries: Sequence[DeleteMessageBatchRequestEntryTypeDef]
     ) -> DeleteMessageBatchResultTypeDef:
         """
         Deletes up to ten messages from the specified queue.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sqs.html#SQS.Client.delete_message_batch)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sqs/client/#delete_message_batch)
         """
+
     async def delete_queue(self, *, QueueUrl: str) -> EmptyResponseMetadataTypeDef:
         """
         Deletes the queue specified by the `QueueUrl`, regardless of the queue's
         contents.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sqs.html#SQS.Client.delete_queue)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sqs/client/#delete_queue)
         """
+
     async def generate_presigned_url(
         self,
         ClientMethod: str,
         Params: Mapping[str, Any] = ...,
         ExpiresIn: int = 3600,
         HttpMethod: str = ...,
     ) -> str:
         """
         Generate a presigned url given a client, its method, and arguments.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sqs.html#SQS.Client.generate_presigned_url)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sqs/client/#generate_presigned_url)
         """
+
     async def get_queue_attributes(
         self, *, QueueUrl: str, AttributeNames: Sequence[QueueAttributeFilterType] = ...
     ) -> GetQueueAttributesResultTypeDef:
         """
         Gets attributes for the specified queue.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sqs.html#SQS.Client.get_queue_attributes)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sqs/client/#get_queue_attributes)
         """
+
     async def get_queue_url(
         self, *, QueueName: str, QueueOwnerAWSAccountId: str = ...
     ) -> GetQueueUrlResultTypeDef:
         """
         Returns the URL of an existing Amazon SQS queue.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sqs.html#SQS.Client.get_queue_url)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sqs/client/#get_queue_url)
         """
+
     async def list_dead_letter_source_queues(
         self, *, QueueUrl: str, NextToken: str = ..., MaxResults: int = ...
     ) -> ListDeadLetterSourceQueuesResultTypeDef:
         """
         Returns a list of your queues that have the `RedrivePolicy` queue attribute
         configured with a dead-letter queue.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sqs.html#SQS.Client.list_dead_letter_source_queues)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sqs/client/#list_dead_letter_source_queues)
         """
+
     async def list_message_move_tasks(
         self, *, SourceArn: str, MaxResults: int = ...
     ) -> ListMessageMoveTasksResultTypeDef:
         """
         Gets the most recent message movement tasks (up to 10) under a specific source
         queue.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sqs.html#SQS.Client.list_message_move_tasks)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sqs/client/#list_message_move_tasks)
         """
+
     async def list_queue_tags(self, *, QueueUrl: str) -> ListQueueTagsResultTypeDef:
         """
         List all cost allocation tags added to the specified Amazon SQS queue.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sqs.html#SQS.Client.list_queue_tags)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sqs/client/#list_queue_tags)
         """
+
     async def list_queues(
         self, *, QueueNamePrefix: str = ..., NextToken: str = ..., MaxResults: int = ...
     ) -> ListQueuesResultTypeDef:
         """
         Returns a list of your queues in the current region.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sqs.html#SQS.Client.list_queues)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sqs/client/#list_queues)
         """
+
     async def purge_queue(self, *, QueueUrl: str) -> EmptyResponseMetadataTypeDef:
         """
-        Deletes the messages in a queue specified by the `QueueURL` parameter.
+        Deletes available messages in a queue (including in-flight messages) specified
+        by the `QueueURL` parameter.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sqs.html#SQS.Client.purge_queue)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sqs/client/#purge_queue)
         """
+
     async def receive_message(
         self,
         *,
         QueueUrl: str,
         AttributeNames: Sequence[QueueAttributeFilterType] = ...,
         MessageAttributeNames: Sequence[str] = ...,
         MaxNumberOfMessages: int = ...,
@@ -272,106 +296,117 @@
     ) -> ReceiveMessageResultTypeDef:
         """
         Retrieves one or more messages (up to 10), from the specified queue.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sqs.html#SQS.Client.receive_message)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sqs/client/#receive_message)
         """
+
     async def remove_permission(self, *, QueueUrl: str, Label: str) -> EmptyResponseMetadataTypeDef:
         """
         Revokes any permissions in the queue policy that matches the specified `Label`
         parameter.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sqs.html#SQS.Client.remove_permission)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sqs/client/#remove_permission)
         """
+
     async def send_message(
         self,
         *,
         QueueUrl: str,
         MessageBody: str,
         DelaySeconds: int = ...,
-        MessageAttributes: Mapping[str, MessageAttributeValueUnionTypeDef] = ...,
+        MessageAttributes: Mapping[str, MessageAttributeValueTypeDef] = ...,
         MessageSystemAttributes: Mapping[
             Literal["AWSTraceHeader"], MessageSystemAttributeValueTypeDef
         ] = ...,
         MessageDeduplicationId: str = ...,
         MessageGroupId: str = ...
     ) -> SendMessageResultTypeDef:
         """
         Delivers a message to the specified queue.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sqs.html#SQS.Client.send_message)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sqs/client/#send_message)
         """
+
     async def send_message_batch(
         self, *, QueueUrl: str, Entries: Sequence[SendMessageBatchRequestEntryTypeDef]
     ) -> SendMessageBatchResultTypeDef:
         """
         You can use `SendMessageBatch` to send up to 10 messages to the specified queue
         by assigning either identical or different values to each message (or by not
         assigning values at all).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sqs.html#SQS.Client.send_message_batch)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sqs/client/#send_message_batch)
         """
+
     async def set_queue_attributes(
         self, *, QueueUrl: str, Attributes: Mapping[QueueAttributeNameType, str]
     ) -> EmptyResponseMetadataTypeDef:
         """
         Sets the value of one or more queue attributes.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sqs.html#SQS.Client.set_queue_attributes)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sqs/client/#set_queue_attributes)
         """
+
     async def start_message_move_task(
         self, *, SourceArn: str, DestinationArn: str = ..., MaxNumberOfMessagesPerSecond: int = ...
     ) -> StartMessageMoveTaskResultTypeDef:
         """
         Starts an asynchronous task to move messages from a specified source queue to a
         specified destination queue.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sqs.html#SQS.Client.start_message_move_task)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sqs/client/#start_message_move_task)
         """
+
     async def tag_queue(
         self, *, QueueUrl: str, Tags: Mapping[str, str]
     ) -> EmptyResponseMetadataTypeDef:
         """
         Add cost allocation tags to the specified Amazon SQS queue.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sqs.html#SQS.Client.tag_queue)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sqs/client/#tag_queue)
         """
+
     async def untag_queue(
         self, *, QueueUrl: str, TagKeys: Sequence[str]
     ) -> EmptyResponseMetadataTypeDef:
         """
         Remove cost allocation tags from the specified Amazon SQS queue.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sqs.html#SQS.Client.untag_queue)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sqs/client/#untag_queue)
         """
+
     @overload
     def get_paginator(
         self, operation_name: Literal["list_dead_letter_source_queues"]
     ) -> ListDeadLetterSourceQueuesPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sqs.html#SQS.Client.get_paginator)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sqs/client/#get_paginator)
         """
+
     @overload
     def get_paginator(self, operation_name: Literal["list_queues"]) -> ListQueuesPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sqs.html#SQS.Client.get_paginator)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sqs/client/#get_paginator)
         """
+
     async def __aenter__(self) -> "SQSClient":
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sqs.html#SQS.Client)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sqs/client/)
         """
+
     async def __aexit__(self, exc_type: Any, exc_val: Any, exc_tb: Any) -> Any:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sqs.html#SQS.Client)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sqs/client/)
         """
```

### Comparing `types-aiobotocore-sqs-2.5.2.post1/types_aiobotocore_sqs/literals.py` & `types-aiobotocore-sqs-2.5.2.post2/types_aiobotocore_sqs/literals.py`

 * *Files 1% similar despite different names*

```diff
@@ -116,14 +116,15 @@
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
@@ -219,14 +220,15 @@
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
@@ -305,26 +307,28 @@
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
@@ -486,14 +490,15 @@
     "eu-central-2",
     "eu-north-1",
     "eu-south-1",
     "eu-south-2",
     "eu-west-1",
     "eu-west-2",
     "eu-west-3",
+    "il-central-1",
     "me-central-1",
     "me-south-1",
     "sa-east-1",
     "us-east-1",
     "us-east-2",
     "us-west-1",
     "us-west-2",
```

### Comparing `types-aiobotocore-sqs-2.5.2.post1/types_aiobotocore_sqs/literals.pyi` & `types-aiobotocore-sqs-2.5.2.post2/types_aiobotocore_sqs/literals.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -114,14 +114,15 @@
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
@@ -217,14 +218,15 @@
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
@@ -303,26 +305,28 @@
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
@@ -484,14 +488,15 @@
     "eu-central-2",
     "eu-north-1",
     "eu-south-1",
     "eu-south-2",
     "eu-west-1",
     "eu-west-2",
     "eu-west-3",
+    "il-central-1",
     "me-central-1",
     "me-south-1",
     "sa-east-1",
     "us-east-1",
     "us-east-2",
     "us-west-1",
     "us-west-2",
```

### Comparing `types-aiobotocore-sqs-2.5.2.post1/types_aiobotocore_sqs/paginator.py` & `types-aiobotocore-sqs-2.5.2.post2/types_aiobotocore_sqs/paginator.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-sqs-2.5.2.post1/types_aiobotocore_sqs/paginator.pyi` & `types-aiobotocore-sqs-2.5.2.post2/types_aiobotocore_sqs/paginator.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-sqs-2.5.2.post1/types_aiobotocore_sqs/service_resource.py` & `types-aiobotocore-sqs-2.5.2.post2/types_aiobotocore_sqs/service_resource.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,18 +29,18 @@
     QueueAttributeNameType,
 )
 from .type_defs import (
     ChangeMessageVisibilityBatchRequestEntryTypeDef,
     ChangeMessageVisibilityBatchResultTypeDef,
     DeleteMessageBatchRequestEntryTypeDef,
     DeleteMessageBatchResultTypeDef,
-    MessageAttributeValueOutputTypeDef,
+    MessageAttributeValueQueueTypeDef,
     MessageAttributeValueTypeDef,
     MessageSystemAttributeValueTypeDef,
-    SendMessageBatchRequestEntryTypeDef,
+    SendMessageBatchRequestEntryQueueTypeDef,
     SendMessageBatchResultTypeDef,
     SendMessageResultTypeDef,
 )
 
 try:
     from aioboto3.resources.base import AIOBoto3ServiceResource
 except (ModuleNotFoundError, ImportError):
@@ -179,15 +179,15 @@
     """
 
     message_id: Awaitable[str]
     md5_of_body: Awaitable[str]
     body: Awaitable[str]
     attributes: Awaitable[Dict[MessageSystemAttributeNameType, str]]
     md5_of_message_attributes: Awaitable[str]
-    message_attributes: Awaitable[Dict[str, MessageAttributeValueOutputTypeDef]]
+    message_attributes: Awaitable[Dict[str, MessageAttributeValueTypeDef]]
     queue_url: str
     receipt_handle: str
 
     async def Queue(self) -> "_Queue":
         """
         Creates a Queue resource.
 
@@ -296,15 +296,16 @@
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sqs.html#SQS.Queue.load)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sqs/service_resource/#queueload-method)
         """
 
     async def purge(self) -> None:
         """
-        Deletes the messages in a queue specified by the `QueueURL` parameter.
+        Deletes available messages in a queue (including in-flight messages) specified
+        by the `QueueURL` parameter.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sqs.html#SQS.Queue.purge)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sqs/service_resource/#queuepurge-method)
         """
 
     async def receive_messages(
         self,
@@ -342,30 +343,30 @@
         """
 
     async def send_message(
         self,
         *,
         MessageBody: str,
         DelaySeconds: int = ...,
-        MessageAttributes: Mapping[str, MessageAttributeValueTypeDef] = ...,
+        MessageAttributes: Mapping[str, MessageAttributeValueQueueTypeDef] = ...,
         MessageSystemAttributes: Mapping[
             Literal["AWSTraceHeader"], MessageSystemAttributeValueTypeDef
         ] = ...,
         MessageDeduplicationId: str = ...,
         MessageGroupId: str = ...
     ) -> SendMessageResultTypeDef:
         """
         Delivers a message to the specified queue.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sqs.html#SQS.Queue.send_message)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sqs/service_resource/#queuesend_message-method)
         """
 
     async def send_messages(
-        self, *, Entries: Sequence[SendMessageBatchRequestEntryTypeDef]
+        self, *, Entries: Sequence[SendMessageBatchRequestEntryQueueTypeDef]
     ) -> SendMessageBatchResultTypeDef:
         """
         You can use `SendMessageBatch` to send up to 10 messages to the specified queue
         by assigning either identical or different values to each message (or by not
         assigning values at all).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sqs.html#SQS.Queue.send_messages)
```

### Comparing `types-aiobotocore-sqs-2.5.2.post1/types_aiobotocore_sqs/service_resource.pyi` & `types-aiobotocore-sqs-2.5.2.post2/types_aiobotocore_sqs/service_resource.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -29,18 +29,18 @@
     QueueAttributeNameType,
 )
 from .type_defs import (
     ChangeMessageVisibilityBatchRequestEntryTypeDef,
     ChangeMessageVisibilityBatchResultTypeDef,
     DeleteMessageBatchRequestEntryTypeDef,
     DeleteMessageBatchResultTypeDef,
-    MessageAttributeValueOutputTypeDef,
+    MessageAttributeValueQueueTypeDef,
     MessageAttributeValueTypeDef,
     MessageSystemAttributeValueTypeDef,
-    SendMessageBatchRequestEntryTypeDef,
+    SendMessageBatchRequestEntryQueueTypeDef,
     SendMessageBatchResultTypeDef,
     SendMessageResultTypeDef,
 )
 
 try:
     from aioboto3.resources.base import AIOBoto3ServiceResource
 except (ModuleNotFoundError, ImportError):
@@ -163,15 +163,15 @@
     """
 
     message_id: Awaitable[str]
     md5_of_body: Awaitable[str]
     body: Awaitable[str]
     attributes: Awaitable[Dict[MessageSystemAttributeNameType, str]]
     md5_of_message_attributes: Awaitable[str]
-    message_attributes: Awaitable[Dict[str, MessageAttributeValueOutputTypeDef]]
+    message_attributes: Awaitable[Dict[str, MessageAttributeValueTypeDef]]
     queue_url: str
     receipt_handle: str
 
     async def Queue(self) -> "_Queue":
         """
         Creates a Queue resource.
 
@@ -268,15 +268,16 @@
         Queue resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sqs.html#SQS.Queue.load)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sqs/service_resource/#queueload-method)
         """
     async def purge(self) -> None:
         """
-        Deletes the messages in a queue specified by the `QueueURL` parameter.
+        Deletes available messages in a queue (including in-flight messages) specified
+        by the `QueueURL` parameter.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sqs.html#SQS.Queue.purge)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sqs/service_resource/#queuepurge-method)
         """
     async def receive_messages(
         self,
         *,
@@ -310,29 +311,29 @@
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sqs/service_resource/#queueremove_permission-method)
         """
     async def send_message(
         self,
         *,
         MessageBody: str,
         DelaySeconds: int = ...,
-        MessageAttributes: Mapping[str, MessageAttributeValueTypeDef] = ...,
+        MessageAttributes: Mapping[str, MessageAttributeValueQueueTypeDef] = ...,
         MessageSystemAttributes: Mapping[
             Literal["AWSTraceHeader"], MessageSystemAttributeValueTypeDef
         ] = ...,
         MessageDeduplicationId: str = ...,
         MessageGroupId: str = ...
     ) -> SendMessageResultTypeDef:
         """
         Delivers a message to the specified queue.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sqs.html#SQS.Queue.send_message)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sqs/service_resource/#queuesend_message-method)
         """
     async def send_messages(
-        self, *, Entries: Sequence[SendMessageBatchRequestEntryTypeDef]
+        self, *, Entries: Sequence[SendMessageBatchRequestEntryQueueTypeDef]
     ) -> SendMessageBatchResultTypeDef:
         """
         You can use `SendMessageBatch` to send up to 10 messages to the specified queue
         by assigning either identical or different values to each message (or by not
         assigning values at all).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sqs.html#SQS.Queue.send_messages)
```

### Comparing `types-aiobotocore-sqs-2.5.2.post1/types_aiobotocore_sqs/type_defs.py` & `types-aiobotocore-sqs-2.5.2.post2/types_aiobotocore_sqs/type_defs.py`

 * *Files 1% similar despite different names*

```diff
@@ -54,27 +54,27 @@
     "GetQueueUrlRequestServiceResourceGetQueueByNameTypeDef",
     "PaginatorConfigTypeDef",
     "ListDeadLetterSourceQueuesRequestRequestTypeDef",
     "ListMessageMoveTasksRequestRequestTypeDef",
     "ListMessageMoveTasksResultEntryTypeDef",
     "ListQueueTagsRequestRequestTypeDef",
     "ListQueuesRequestRequestTypeDef",
-    "MessageAttributeValueOutputTypeDef",
+    "MessageAttributeValueTypeDef",
     "PurgeQueueRequestRequestTypeDef",
     "ReceiveMessageRequestQueueReceiveMessagesTypeDef",
     "ReceiveMessageRequestRequestTypeDef",
     "RemovePermissionRequestQueueRemovePermissionTypeDef",
     "RemovePermissionRequestRequestTypeDef",
     "SendMessageBatchResultEntryTypeDef",
     "SetQueueAttributesRequestQueueSetAttributesTypeDef",
     "SetQueueAttributesRequestRequestTypeDef",
     "StartMessageMoveTaskRequestRequestTypeDef",
     "TagQueueRequestRequestTypeDef",
     "UntagQueueRequestRequestTypeDef",
-    "MessageAttributeValueTypeDef",
+    "MessageAttributeValueQueueTypeDef",
     "MessageSystemAttributeValueTypeDef",
     "CancelMessageMoveTaskResultTypeDef",
     "CreateQueueResultTypeDef",
     "EmptyResponseMetadataTypeDef",
     "GetQueueAttributesResultTypeDef",
     "GetQueueUrlResultTypeDef",
     "ListDeadLetterSourceQueuesResultTypeDef",
@@ -89,19 +89,19 @@
     "DeleteMessageBatchRequestRequestTypeDef",
     "DeleteMessageBatchResultTypeDef",
     "ListDeadLetterSourceQueuesRequestListDeadLetterSourceQueuesPaginateTypeDef",
     "ListQueuesRequestListQueuesPaginateTypeDef",
     "ListMessageMoveTasksResultTypeDef",
     "MessageTypeDef",
     "SendMessageBatchResultTypeDef",
-    "MessageAttributeValueUnionTypeDef",
+    "SendMessageBatchRequestEntryQueueTypeDef",
     "SendMessageBatchRequestEntryTypeDef",
     "SendMessageRequestQueueSendMessageTypeDef",
-    "ReceiveMessageResultTypeDef",
     "SendMessageRequestRequestTypeDef",
+    "ReceiveMessageResultTypeDef",
     "SendMessageBatchRequestQueueSendMessagesTypeDef",
     "SendMessageBatchRequestRequestTypeDef",
 )
 
 AddPermissionRequestQueueAddPermissionTypeDef = TypedDict(
     "AddPermissionRequestQueueAddPermissionTypeDef",
     {
@@ -433,34 +433,34 @@
         "QueueNamePrefix": str,
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
-_RequiredMessageAttributeValueOutputTypeDef = TypedDict(
-    "_RequiredMessageAttributeValueOutputTypeDef",
+_RequiredMessageAttributeValueTypeDef = TypedDict(
+    "_RequiredMessageAttributeValueTypeDef",
     {
         "DataType": str,
     },
 )
-_OptionalMessageAttributeValueOutputTypeDef = TypedDict(
-    "_OptionalMessageAttributeValueOutputTypeDef",
+_OptionalMessageAttributeValueTypeDef = TypedDict(
+    "_OptionalMessageAttributeValueTypeDef",
     {
         "StringValue": str,
         "BinaryValue": bytes,
         "StringListValues": List[str],
         "BinaryListValues": List[bytes],
     },
     total=False,
 )
 
 
-class MessageAttributeValueOutputTypeDef(
-    _RequiredMessageAttributeValueOutputTypeDef, _OptionalMessageAttributeValueOutputTypeDef
+class MessageAttributeValueTypeDef(
+    _RequiredMessageAttributeValueTypeDef, _OptionalMessageAttributeValueTypeDef
 ):
     pass
 
 
 PurgeQueueRequestRequestTypeDef = TypedDict(
     "PurgeQueueRequestRequestTypeDef",
     {
@@ -597,34 +597,34 @@
     "UntagQueueRequestRequestTypeDef",
     {
         "QueueUrl": str,
         "TagKeys": Sequence[str],
     },
 )
 
-_RequiredMessageAttributeValueTypeDef = TypedDict(
-    "_RequiredMessageAttributeValueTypeDef",
+_RequiredMessageAttributeValueQueueTypeDef = TypedDict(
+    "_RequiredMessageAttributeValueQueueTypeDef",
     {
         "DataType": str,
     },
 )
-_OptionalMessageAttributeValueTypeDef = TypedDict(
-    "_OptionalMessageAttributeValueTypeDef",
+_OptionalMessageAttributeValueQueueTypeDef = TypedDict(
+    "_OptionalMessageAttributeValueQueueTypeDef",
     {
         "StringValue": str,
         "BinaryValue": BlobTypeDef,
         "StringListValues": Sequence[str],
         "BinaryListValues": Sequence[BlobTypeDef],
     },
     total=False,
 )
 
 
-class MessageAttributeValueTypeDef(
-    _RequiredMessageAttributeValueTypeDef, _OptionalMessageAttributeValueTypeDef
+class MessageAttributeValueQueueTypeDef(
+    _RequiredMessageAttributeValueQueueTypeDef, _OptionalMessageAttributeValueQueueTypeDef
 ):
     pass
 
 
 _RequiredMessageSystemAttributeValueTypeDef = TypedDict(
     "_RequiredMessageSystemAttributeValueTypeDef",
     {
@@ -826,31 +826,57 @@
     {
         "MessageId": str,
         "ReceiptHandle": str,
         "MD5OfBody": str,
         "Body": str,
         "Attributes": Dict[MessageSystemAttributeNameType, str],
         "MD5OfMessageAttributes": str,
-        "MessageAttributes": Dict[str, MessageAttributeValueOutputTypeDef],
+        "MessageAttributes": Dict[str, MessageAttributeValueTypeDef],
     },
     total=False,
 )
 
 SendMessageBatchResultTypeDef = TypedDict(
     "SendMessageBatchResultTypeDef",
     {
         "Successful": List[SendMessageBatchResultEntryTypeDef],
         "Failed": List[BatchResultErrorEntryTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-MessageAttributeValueUnionTypeDef = Union[
-    MessageAttributeValueTypeDef, MessageAttributeValueOutputTypeDef
-]
+_RequiredSendMessageBatchRequestEntryQueueTypeDef = TypedDict(
+    "_RequiredSendMessageBatchRequestEntryQueueTypeDef",
+    {
+        "Id": str,
+        "MessageBody": str,
+    },
+)
+_OptionalSendMessageBatchRequestEntryQueueTypeDef = TypedDict(
+    "_OptionalSendMessageBatchRequestEntryQueueTypeDef",
+    {
+        "DelaySeconds": int,
+        "MessageAttributes": Mapping[str, MessageAttributeValueQueueTypeDef],
+        "MessageSystemAttributes": Mapping[
+            Literal["AWSTraceHeader"], MessageSystemAttributeValueTypeDef
+        ],
+        "MessageDeduplicationId": str,
+        "MessageGroupId": str,
+    },
+    total=False,
+)
+
+
+class SendMessageBatchRequestEntryQueueTypeDef(
+    _RequiredSendMessageBatchRequestEntryQueueTypeDef,
+    _OptionalSendMessageBatchRequestEntryQueueTypeDef,
+):
+    pass
+
+
 _RequiredSendMessageBatchRequestEntryTypeDef = TypedDict(
     "_RequiredSendMessageBatchRequestEntryTypeDef",
     {
         "Id": str,
         "MessageBody": str,
     },
 )
@@ -881,15 +907,15 @@
         "MessageBody": str,
     },
 )
 _OptionalSendMessageRequestQueueSendMessageTypeDef = TypedDict(
     "_OptionalSendMessageRequestQueueSendMessageTypeDef",
     {
         "DelaySeconds": int,
-        "MessageAttributes": Mapping[str, MessageAttributeValueTypeDef],
+        "MessageAttributes": Mapping[str, MessageAttributeValueQueueTypeDef],
         "MessageSystemAttributes": Mapping[
             Literal["AWSTraceHeader"], MessageSystemAttributeValueTypeDef
         ],
         "MessageDeduplicationId": str,
         "MessageGroupId": str,
     },
     total=False,
@@ -899,34 +925,26 @@
 class SendMessageRequestQueueSendMessageTypeDef(
     _RequiredSendMessageRequestQueueSendMessageTypeDef,
     _OptionalSendMessageRequestQueueSendMessageTypeDef,
 ):
     pass
 
 
-ReceiveMessageResultTypeDef = TypedDict(
-    "ReceiveMessageResultTypeDef",
-    {
-        "Messages": List[MessageTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 _RequiredSendMessageRequestRequestTypeDef = TypedDict(
     "_RequiredSendMessageRequestRequestTypeDef",
     {
         "QueueUrl": str,
         "MessageBody": str,
     },
 )
 _OptionalSendMessageRequestRequestTypeDef = TypedDict(
     "_OptionalSendMessageRequestRequestTypeDef",
     {
         "DelaySeconds": int,
-        "MessageAttributes": Mapping[str, MessageAttributeValueUnionTypeDef],
+        "MessageAttributes": Mapping[str, MessageAttributeValueTypeDef],
         "MessageSystemAttributes": Mapping[
             Literal["AWSTraceHeader"], MessageSystemAttributeValueTypeDef
         ],
         "MessageDeduplicationId": str,
         "MessageGroupId": str,
     },
     total=False,
@@ -935,18 +953,26 @@
 
 class SendMessageRequestRequestTypeDef(
     _RequiredSendMessageRequestRequestTypeDef, _OptionalSendMessageRequestRequestTypeDef
 ):
     pass
 
 
+ReceiveMessageResultTypeDef = TypedDict(
+    "ReceiveMessageResultTypeDef",
+    {
+        "Messages": List[MessageTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 SendMessageBatchRequestQueueSendMessagesTypeDef = TypedDict(
     "SendMessageBatchRequestQueueSendMessagesTypeDef",
     {
-        "Entries": Sequence[SendMessageBatchRequestEntryTypeDef],
+        "Entries": Sequence[SendMessageBatchRequestEntryQueueTypeDef],
     },
 )
 
 SendMessageBatchRequestRequestTypeDef = TypedDict(
     "SendMessageBatchRequestRequestTypeDef",
     {
         "QueueUrl": str,
```

### Comparing `types-aiobotocore-sqs-2.5.2.post1/types_aiobotocore_sqs/type_defs.pyi` & `types-aiobotocore-sqs-2.5.2.post2/types_aiobotocore_sqs/type_defs.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -53,27 +53,27 @@
     "GetQueueUrlRequestServiceResourceGetQueueByNameTypeDef",
     "PaginatorConfigTypeDef",
     "ListDeadLetterSourceQueuesRequestRequestTypeDef",
     "ListMessageMoveTasksRequestRequestTypeDef",
     "ListMessageMoveTasksResultEntryTypeDef",
     "ListQueueTagsRequestRequestTypeDef",
     "ListQueuesRequestRequestTypeDef",
-    "MessageAttributeValueOutputTypeDef",
+    "MessageAttributeValueTypeDef",
     "PurgeQueueRequestRequestTypeDef",
     "ReceiveMessageRequestQueueReceiveMessagesTypeDef",
     "ReceiveMessageRequestRequestTypeDef",
     "RemovePermissionRequestQueueRemovePermissionTypeDef",
     "RemovePermissionRequestRequestTypeDef",
     "SendMessageBatchResultEntryTypeDef",
     "SetQueueAttributesRequestQueueSetAttributesTypeDef",
     "SetQueueAttributesRequestRequestTypeDef",
     "StartMessageMoveTaskRequestRequestTypeDef",
     "TagQueueRequestRequestTypeDef",
     "UntagQueueRequestRequestTypeDef",
-    "MessageAttributeValueTypeDef",
+    "MessageAttributeValueQueueTypeDef",
     "MessageSystemAttributeValueTypeDef",
     "CancelMessageMoveTaskResultTypeDef",
     "CreateQueueResultTypeDef",
     "EmptyResponseMetadataTypeDef",
     "GetQueueAttributesResultTypeDef",
     "GetQueueUrlResultTypeDef",
     "ListDeadLetterSourceQueuesResultTypeDef",
@@ -88,19 +88,19 @@
     "DeleteMessageBatchRequestRequestTypeDef",
     "DeleteMessageBatchResultTypeDef",
     "ListDeadLetterSourceQueuesRequestListDeadLetterSourceQueuesPaginateTypeDef",
     "ListQueuesRequestListQueuesPaginateTypeDef",
     "ListMessageMoveTasksResultTypeDef",
     "MessageTypeDef",
     "SendMessageBatchResultTypeDef",
-    "MessageAttributeValueUnionTypeDef",
+    "SendMessageBatchRequestEntryQueueTypeDef",
     "SendMessageBatchRequestEntryTypeDef",
     "SendMessageRequestQueueSendMessageTypeDef",
-    "ReceiveMessageResultTypeDef",
     "SendMessageRequestRequestTypeDef",
+    "ReceiveMessageResultTypeDef",
     "SendMessageBatchRequestQueueSendMessagesTypeDef",
     "SendMessageBatchRequestRequestTypeDef",
 )
 
 AddPermissionRequestQueueAddPermissionTypeDef = TypedDict(
     "AddPermissionRequestQueueAddPermissionTypeDef",
     {
@@ -414,33 +414,33 @@
         "QueueNamePrefix": str,
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
-_RequiredMessageAttributeValueOutputTypeDef = TypedDict(
-    "_RequiredMessageAttributeValueOutputTypeDef",
+_RequiredMessageAttributeValueTypeDef = TypedDict(
+    "_RequiredMessageAttributeValueTypeDef",
     {
         "DataType": str,
     },
 )
-_OptionalMessageAttributeValueOutputTypeDef = TypedDict(
-    "_OptionalMessageAttributeValueOutputTypeDef",
+_OptionalMessageAttributeValueTypeDef = TypedDict(
+    "_OptionalMessageAttributeValueTypeDef",
     {
         "StringValue": str,
         "BinaryValue": bytes,
         "StringListValues": List[str],
         "BinaryListValues": List[bytes],
     },
     total=False,
 )
 
-class MessageAttributeValueOutputTypeDef(
-    _RequiredMessageAttributeValueOutputTypeDef, _OptionalMessageAttributeValueOutputTypeDef
+class MessageAttributeValueTypeDef(
+    _RequiredMessageAttributeValueTypeDef, _OptionalMessageAttributeValueTypeDef
 ):
     pass
 
 PurgeQueueRequestRequestTypeDef = TypedDict(
     "PurgeQueueRequestRequestTypeDef",
     {
         "QueueUrl": str,
@@ -570,33 +570,33 @@
     "UntagQueueRequestRequestTypeDef",
     {
         "QueueUrl": str,
         "TagKeys": Sequence[str],
     },
 )
 
-_RequiredMessageAttributeValueTypeDef = TypedDict(
-    "_RequiredMessageAttributeValueTypeDef",
+_RequiredMessageAttributeValueQueueTypeDef = TypedDict(
+    "_RequiredMessageAttributeValueQueueTypeDef",
     {
         "DataType": str,
     },
 )
-_OptionalMessageAttributeValueTypeDef = TypedDict(
-    "_OptionalMessageAttributeValueTypeDef",
+_OptionalMessageAttributeValueQueueTypeDef = TypedDict(
+    "_OptionalMessageAttributeValueQueueTypeDef",
     {
         "StringValue": str,
         "BinaryValue": BlobTypeDef,
         "StringListValues": Sequence[str],
         "BinaryListValues": Sequence[BlobTypeDef],
     },
     total=False,
 )
 
-class MessageAttributeValueTypeDef(
-    _RequiredMessageAttributeValueTypeDef, _OptionalMessageAttributeValueTypeDef
+class MessageAttributeValueQueueTypeDef(
+    _RequiredMessageAttributeValueQueueTypeDef, _OptionalMessageAttributeValueQueueTypeDef
 ):
     pass
 
 _RequiredMessageSystemAttributeValueTypeDef = TypedDict(
     "_RequiredMessageSystemAttributeValueTypeDef",
     {
         "DataType": str,
@@ -793,31 +793,55 @@
     {
         "MessageId": str,
         "ReceiptHandle": str,
         "MD5OfBody": str,
         "Body": str,
         "Attributes": Dict[MessageSystemAttributeNameType, str],
         "MD5OfMessageAttributes": str,
-        "MessageAttributes": Dict[str, MessageAttributeValueOutputTypeDef],
+        "MessageAttributes": Dict[str, MessageAttributeValueTypeDef],
     },
     total=False,
 )
 
 SendMessageBatchResultTypeDef = TypedDict(
     "SendMessageBatchResultTypeDef",
     {
         "Successful": List[SendMessageBatchResultEntryTypeDef],
         "Failed": List[BatchResultErrorEntryTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-MessageAttributeValueUnionTypeDef = Union[
-    MessageAttributeValueTypeDef, MessageAttributeValueOutputTypeDef
-]
+_RequiredSendMessageBatchRequestEntryQueueTypeDef = TypedDict(
+    "_RequiredSendMessageBatchRequestEntryQueueTypeDef",
+    {
+        "Id": str,
+        "MessageBody": str,
+    },
+)
+_OptionalSendMessageBatchRequestEntryQueueTypeDef = TypedDict(
+    "_OptionalSendMessageBatchRequestEntryQueueTypeDef",
+    {
+        "DelaySeconds": int,
+        "MessageAttributes": Mapping[str, MessageAttributeValueQueueTypeDef],
+        "MessageSystemAttributes": Mapping[
+            Literal["AWSTraceHeader"], MessageSystemAttributeValueTypeDef
+        ],
+        "MessageDeduplicationId": str,
+        "MessageGroupId": str,
+    },
+    total=False,
+)
+
+class SendMessageBatchRequestEntryQueueTypeDef(
+    _RequiredSendMessageBatchRequestEntryQueueTypeDef,
+    _OptionalSendMessageBatchRequestEntryQueueTypeDef,
+):
+    pass
+
 _RequiredSendMessageBatchRequestEntryTypeDef = TypedDict(
     "_RequiredSendMessageBatchRequestEntryTypeDef",
     {
         "Id": str,
         "MessageBody": str,
     },
 )
@@ -846,15 +870,15 @@
         "MessageBody": str,
     },
 )
 _OptionalSendMessageRequestQueueSendMessageTypeDef = TypedDict(
     "_OptionalSendMessageRequestQueueSendMessageTypeDef",
     {
         "DelaySeconds": int,
-        "MessageAttributes": Mapping[str, MessageAttributeValueTypeDef],
+        "MessageAttributes": Mapping[str, MessageAttributeValueQueueTypeDef],
         "MessageSystemAttributes": Mapping[
             Literal["AWSTraceHeader"], MessageSystemAttributeValueTypeDef
         ],
         "MessageDeduplicationId": str,
         "MessageGroupId": str,
     },
     total=False,
@@ -862,52 +886,52 @@
 
 class SendMessageRequestQueueSendMessageTypeDef(
     _RequiredSendMessageRequestQueueSendMessageTypeDef,
     _OptionalSendMessageRequestQueueSendMessageTypeDef,
 ):
     pass
 
-ReceiveMessageResultTypeDef = TypedDict(
-    "ReceiveMessageResultTypeDef",
-    {
-        "Messages": List[MessageTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 _RequiredSendMessageRequestRequestTypeDef = TypedDict(
     "_RequiredSendMessageRequestRequestTypeDef",
     {
         "QueueUrl": str,
         "MessageBody": str,
     },
 )
 _OptionalSendMessageRequestRequestTypeDef = TypedDict(
     "_OptionalSendMessageRequestRequestTypeDef",
     {
         "DelaySeconds": int,
-        "MessageAttributes": Mapping[str, MessageAttributeValueUnionTypeDef],
+        "MessageAttributes": Mapping[str, MessageAttributeValueTypeDef],
         "MessageSystemAttributes": Mapping[
             Literal["AWSTraceHeader"], MessageSystemAttributeValueTypeDef
         ],
         "MessageDeduplicationId": str,
         "MessageGroupId": str,
     },
     total=False,
 )
 
 class SendMessageRequestRequestTypeDef(
     _RequiredSendMessageRequestRequestTypeDef, _OptionalSendMessageRequestRequestTypeDef
 ):
     pass
 
+ReceiveMessageResultTypeDef = TypedDict(
+    "ReceiveMessageResultTypeDef",
+    {
+        "Messages": List[MessageTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 SendMessageBatchRequestQueueSendMessagesTypeDef = TypedDict(
     "SendMessageBatchRequestQueueSendMessagesTypeDef",
     {
-        "Entries": Sequence[SendMessageBatchRequestEntryTypeDef],
+        "Entries": Sequence[SendMessageBatchRequestEntryQueueTypeDef],
     },
 )
 
 SendMessageBatchRequestRequestTypeDef = TypedDict(
     "SendMessageBatchRequestRequestTypeDef",
     {
         "QueueUrl": str,
```

### Comparing `types-aiobotocore-sqs-2.5.2.post1/types_aiobotocore_sqs.egg-info/SOURCES.txt` & `types-aiobotocore-sqs-2.5.2.post2/types_aiobotocore_sqs.egg-info/SOURCES.txt`

 * *Files identical despite different names*


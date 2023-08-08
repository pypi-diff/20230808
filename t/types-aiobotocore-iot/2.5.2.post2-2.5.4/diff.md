# Comparing `tmp/types-aiobotocore-iot-2.5.2.post2.tar.gz` & `tmp/types-aiobotocore-iot-2.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-iot-2.5.2.post2.tar", last modified: Fri Aug  4 13:59:12 2023, max compression
+gzip compressed data, was "types-aiobotocore-iot-2.5.4.tar", last modified: Tue Aug  8 01:23:52 2023, max compression
```

## Comparing `types-aiobotocore-iot-2.5.2.post2.tar` & `types-aiobotocore-iot-2.5.4.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:12.206642 types-aiobotocore-iot-2.5.2.post2/
--rw-r--r--   0 vlad      (1000) vlad      (1000)     1070 2023-08-04 13:40:31.000000 types-aiobotocore-iot-2.5.2.post2/LICENSE
--rw-r--r--   0 vlad      (1000) vlad      (1000)    22394 2023-08-04 13:59:12.206642 types-aiobotocore-iot-2.5.2.post2/PKG-INFO
--rw-r--r--   0 vlad      (1000) vlad      (1000)    20892 2023-08-04 13:40:31.000000 types-aiobotocore-iot-2.5.2.post2/README.md
--rw-r--r--   0 vlad      (1000) vlad      (1000)       38 2023-08-04 13:59:12.206642 types-aiobotocore-iot-2.5.2.post2/setup.cfg
--rw-r--r--   0 vlad      (1000) vlad      (1000)     2020 2023-08-04 13:40:31.000000 types-aiobotocore-iot-2.5.2.post2/setup.py
-drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:12.206642 types-aiobotocore-iot-2.5.2.post2/types_aiobotocore_iot/
--rw-r--r--   0 vlad      (1000) vlad      (1000)    14185 2023-08-04 13:40:31.000000 types-aiobotocore-iot-2.5.2.post2/types_aiobotocore_iot/__init__.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)    14184 2023-08-04 13:40:31.000000 types-aiobotocore-iot-2.5.2.post2/types_aiobotocore_iot/__init__.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)      916 2023-08-04 13:40:31.000000 types-aiobotocore-iot-2.5.2.post2/types_aiobotocore_iot/__main__.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)   190004 2023-08-04 13:40:34.000000 types-aiobotocore-iot-2.5.2.post2/types_aiobotocore_iot/client.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)   189686 2023-08-04 13:40:32.000000 types-aiobotocore-iot-2.5.2.post2/types_aiobotocore_iot/client.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)    25057 2023-08-04 13:40:35.000000 types-aiobotocore-iot-2.5.2.post2/types_aiobotocore_iot/literals.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)    25055 2023-08-04 13:40:35.000000 types-aiobotocore-iot-2.5.2.post2/types_aiobotocore_iot/literals.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)    71670 2023-08-04 13:40:34.000000 types-aiobotocore-iot-2.5.2.post2/types_aiobotocore_iot/paginator.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)    71609 2023-08-04 13:40:34.000000 types-aiobotocore-iot-2.5.2.post2/types_aiobotocore_iot/paginator.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:40:31.000000 types-aiobotocore-iot-2.5.2.post2/types_aiobotocore_iot/py.typed
--rw-r--r--   0 vlad      (1000) vlad      (1000)   256609 2023-08-04 13:40:43.000000 types-aiobotocore-iot-2.5.2.post2/types_aiobotocore_iot/type_defs.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)   256282 2023-08-04 13:40:39.000000 types-aiobotocore-iot-2.5.2.post2/types_aiobotocore_iot/type_defs.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)       65 2023-08-04 13:40:31.000000 types-aiobotocore-iot-2.5.2.post2/types_aiobotocore_iot/version.py
-drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:12.206642 types-aiobotocore-iot-2.5.2.post2/types_aiobotocore_iot.egg-info/
--rw-r--r--   0 vlad      (1000) vlad      (1000)    22394 2023-08-04 13:59:12.000000 types-aiobotocore-iot-2.5.2.post2/types_aiobotocore_iot.egg-info/PKG-INFO
--rw-r--r--   0 vlad      (1000) vlad      (1000)      737 2023-08-04 13:59:12.000000 types-aiobotocore-iot-2.5.2.post2/types_aiobotocore_iot.egg-info/SOURCES.txt
--rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:12.000000 types-aiobotocore-iot-2.5.2.post2/types_aiobotocore_iot.egg-info/dependency_links.txt
--rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:12.000000 types-aiobotocore-iot-2.5.2.post2/types_aiobotocore_iot.egg-info/not-zip-safe
--rw-r--r--   0 vlad      (1000) vlad      (1000)       52 2023-08-04 13:59:12.000000 types-aiobotocore-iot-2.5.2.post2/types_aiobotocore_iot.egg-info/requires.txt
--rw-r--r--   0 vlad      (1000) vlad      (1000)       22 2023-08-04 13:59:12.000000 types-aiobotocore-iot-2.5.2.post2/types_aiobotocore_iot.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:23:52.114713 types-aiobotocore-iot-2.5.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-08 01:12:38.000000 types-aiobotocore-iot-2.5.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    22388 2023-08-08 01:23:52.106713 types-aiobotocore-iot-2.5.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    20892 2023-08-08 01:12:38.000000 types-aiobotocore-iot-2.5.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-08 01:23:52.114713 types-aiobotocore-iot-2.5.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2014 2023-08-08 01:12:38.000000 types-aiobotocore-iot-2.5.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:23:52.106713 types-aiobotocore-iot-2.5.4/types_aiobotocore_iot/
+-rw-r--r--   0 runner    (1001) docker     (123)    14185 2023-08-08 01:12:38.000000 types-aiobotocore-iot-2.5.4/types_aiobotocore_iot/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14184 2023-08-08 01:12:38.000000 types-aiobotocore-iot-2.5.4/types_aiobotocore_iot/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      904 2023-08-08 01:12:38.000000 types-aiobotocore-iot-2.5.4/types_aiobotocore_iot/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   190004 2023-08-08 01:12:40.000000 types-aiobotocore-iot-2.5.4/types_aiobotocore_iot/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)   189686 2023-08-08 01:12:38.000000 types-aiobotocore-iot-2.5.4/types_aiobotocore_iot/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    25057 2023-08-08 01:12:41.000000 types-aiobotocore-iot-2.5.4/types_aiobotocore_iot/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25055 2023-08-08 01:12:41.000000 types-aiobotocore-iot-2.5.4/types_aiobotocore_iot/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    71670 2023-08-08 01:12:41.000000 types-aiobotocore-iot-2.5.4/types_aiobotocore_iot/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    71609 2023-08-08 01:12:40.000000 types-aiobotocore-iot-2.5.4/types_aiobotocore_iot/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 01:12:38.000000 types-aiobotocore-iot-2.5.4/types_aiobotocore_iot/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)   256612 2023-08-08 01:12:47.000000 types-aiobotocore-iot-2.5.4/types_aiobotocore_iot/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)   256285 2023-08-08 01:12:43.000000 types-aiobotocore-iot-2.5.4/types_aiobotocore_iot/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-08-08 01:12:38.000000 types-aiobotocore-iot-2.5.4/types_aiobotocore_iot/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:23:52.106713 types-aiobotocore-iot-2.5.4/types_aiobotocore_iot.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    22388 2023-08-08 01:23:51.000000 types-aiobotocore-iot-2.5.4/types_aiobotocore_iot.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      737 2023-08-08 01:23:51.000000 types-aiobotocore-iot-2.5.4/types_aiobotocore_iot.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 01:23:51.000000 types-aiobotocore-iot-2.5.4/types_aiobotocore_iot.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 01:23:51.000000 types-aiobotocore-iot-2.5.4/types_aiobotocore_iot.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-08 01:23:51.000000 types-aiobotocore-iot-2.5.4/types_aiobotocore_iot.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-08-08 01:23:51.000000 types-aiobotocore-iot-2.5.4/types_aiobotocore_iot.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-iot-2.5.2.post2/LICENSE` & `types-aiobotocore-iot-2.5.4/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-iot-2.5.2.post2/PKG-INFO` & `types-aiobotocore-iot-2.5.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-iot
-Version: 2.5.2.post2
-Summary: Type annotations for aiobotocore.IoT 2.5.2 service generated with mypy-boto3-builder 7.17.2
+Version: 2.5.4
+Summary: Type annotations for aiobotocore.IoT 2.5.4 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-iot.svg?color=blue)](https://pypi.org/project/types-aiobotocore-iot)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-iot)](https://pepy.tech/project/types-aiobotocore-iot)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.IoT 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT)
+[aiobotocore.IoT 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-iot-2.5.2.post2/README.md` & `types-aiobotocore-iot-2.5.4/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-iot.svg?color=blue)](https://pypi.org/project/types-aiobotocore-iot)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-iot)](https://pepy.tech/project/types-aiobotocore-iot)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.IoT 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT)
+[aiobotocore.IoT 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-iot-2.5.2.post2/setup.py` & `types-aiobotocore-iot-2.5.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-iot",
-    version="2.5.2.post2",
+    version="2.5.4",
     packages=["types_aiobotocore_iot"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.IoT 2.5.2 service generated with mypy-boto3-builder"
+        "Type annotations for aiobotocore.IoT 2.5.4 service generated with mypy-boto3-builder"
         " 7.17.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
```

### Comparing `types-aiobotocore-iot-2.5.2.post2/types_aiobotocore_iot/__init__.py` & `types-aiobotocore-iot-2.5.4/types_aiobotocore_iot/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-iot-2.5.2.post2/types_aiobotocore_iot/__init__.pyi` & `types-aiobotocore-iot-2.5.4/types_aiobotocore_iot/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-iot-2.5.2.post2/types_aiobotocore_iot/__main__.py` & `types-aiobotocore-iot-2.5.4/types_aiobotocore_iot/__main__.py`

 * *Files 13% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.IoT 2.5.2\nVersion:         2.5.2.post2\nBuilder version:"
+        "Type annotations for aiobotocore.IoT 2.5.4\nVersion:         2.5.4\nBuilder version:"
         " 7.17.2\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot//\nBoto3 docs:    "
         "  https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT\nOther"
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

### Comparing `types-aiobotocore-iot-2.5.2.post2/types_aiobotocore_iot/client.py` & `types-aiobotocore-iot-2.5.4/types_aiobotocore_iot/client.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-iot-2.5.2.post2/types_aiobotocore_iot/client.pyi` & `types-aiobotocore-iot-2.5.4/types_aiobotocore_iot/client.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-iot-2.5.2.post2/types_aiobotocore_iot/literals.py` & `types-aiobotocore-iot-2.5.4/types_aiobotocore_iot/literals.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-iot-2.5.2.post2/types_aiobotocore_iot/literals.pyi` & `types-aiobotocore-iot-2.5.4/types_aiobotocore_iot/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-iot-2.5.2.post2/types_aiobotocore_iot/paginator.py` & `types-aiobotocore-iot-2.5.4/types_aiobotocore_iot/paginator.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-iot-2.5.2.post2/types_aiobotocore_iot/paginator.pyi` & `types-aiobotocore-iot-2.5.4/types_aiobotocore_iot/paginator.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-iot-2.5.2.post2/types_aiobotocore_iot/type_defs.py` & `types-aiobotocore-iot-2.5.4/types_aiobotocore_iot/type_defs.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     data: AbortCriteriaTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import IO, Any, Dict, List, Mapping, Sequence, Union
 
-from botocore.response import StreamingBody
+from aiobotocore.response import StreamingBody
 
 from .literals import (
     ActionTypeType,
     AggregationTypeNameType,
     AuditCheckRunStatusType,
     AuditFindingSeverityType,
     AuditFrequencyType,
```

### Comparing `types-aiobotocore-iot-2.5.2.post2/types_aiobotocore_iot/type_defs.pyi` & `types-aiobotocore-iot-2.5.4/types_aiobotocore_iot/type_defs.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     data: AbortCriteriaTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import IO, Any, Dict, List, Mapping, Sequence, Union
 
-from botocore.response import StreamingBody
+from aiobotocore.response import StreamingBody
 
 from .literals import (
     ActionTypeType,
     AggregationTypeNameType,
     AuditCheckRunStatusType,
     AuditFindingSeverityType,
     AuditFrequencyType,
```

### Comparing `types-aiobotocore-iot-2.5.2.post2/types_aiobotocore_iot.egg-info/PKG-INFO` & `types-aiobotocore-iot-2.5.4/types_aiobotocore_iot.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-iot
-Version: 2.5.2.post2
-Summary: Type annotations for aiobotocore.IoT 2.5.2 service generated with mypy-boto3-builder 7.17.2
+Version: 2.5.4
+Summary: Type annotations for aiobotocore.IoT 2.5.4 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-iot.svg?color=blue)](https://pypi.org/project/types-aiobotocore-iot)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-iot)](https://pepy.tech/project/types-aiobotocore-iot)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.IoT 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT)
+[aiobotocore.IoT 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-iot-2.5.2.post2/types_aiobotocore_iot.egg-info/SOURCES.txt` & `types-aiobotocore-iot-2.5.4/types_aiobotocore_iot.egg-info/SOURCES.txt`

 * *Files identical despite different names*


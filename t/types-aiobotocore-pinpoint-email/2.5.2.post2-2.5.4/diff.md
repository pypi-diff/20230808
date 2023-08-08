# Comparing `tmp/types-aiobotocore-pinpoint-email-2.5.2.post2.tar.gz` & `tmp/types-aiobotocore-pinpoint-email-2.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-pinpoint-email-2.5.2.post2.tar", last modified: Fri Aug  4 13:59:21 2023, max compression
+gzip compressed data, was "types-aiobotocore-pinpoint-email-2.5.4.tar", last modified: Tue Aug  8 01:24:13 2023, max compression
```

## Comparing `types-aiobotocore-pinpoint-email-2.5.2.post2.tar` & `types-aiobotocore-pinpoint-email-2.5.4.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:21.136643 types-aiobotocore-pinpoint-email-2.5.2.post2/
--rw-r--r--   0 vlad      (1000) vlad      (1000)     1070 2023-08-04 13:46:54.000000 types-aiobotocore-pinpoint-email-2.5.2.post2/LICENSE
--rw-r--r--   0 vlad      (1000) vlad      (1000)    14046 2023-08-04 13:59:21.136643 types-aiobotocore-pinpoint-email-2.5.2.post2/PKG-INFO
--rw-r--r--   0 vlad      (1000) vlad      (1000)    12501 2023-08-04 13:46:54.000000 types-aiobotocore-pinpoint-email-2.5.2.post2/README.md
--rw-r--r--   0 vlad      (1000) vlad      (1000)       38 2023-08-04 13:59:21.136643 types-aiobotocore-pinpoint-email-2.5.2.post2/setup.cfg
--rw-r--r--   0 vlad      (1000) vlad      (1000)     2120 2023-08-04 13:46:54.000000 types-aiobotocore-pinpoint-email-2.5.2.post2/setup.py
-drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:21.126643 types-aiobotocore-pinpoint-email-2.5.2.post2/types_aiobotocore_pinpoint_email/
--rw-r--r--   0 vlad      (1000) vlad      (1000)     1700 2023-08-04 13:46:54.000000 types-aiobotocore-pinpoint-email-2.5.2.post2/types_aiobotocore_pinpoint_email/__init__.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)     1699 2023-08-04 13:46:54.000000 types-aiobotocore-pinpoint-email-2.5.2.post2/types_aiobotocore_pinpoint_email/__init__.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)      969 2023-08-04 13:46:54.000000 types-aiobotocore-pinpoint-email-2.5.2.post2/types_aiobotocore_pinpoint_email/__main__.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)    35092 2023-08-04 13:46:55.000000 types-aiobotocore-pinpoint-email-2.5.2.post2/types_aiobotocore_pinpoint_email/client.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)    35036 2023-08-04 13:46:54.000000 types-aiobotocore-pinpoint-email-2.5.2.post2/types_aiobotocore_pinpoint_email/client.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)     9960 2023-08-04 13:46:55.000000 types-aiobotocore-pinpoint-email-2.5.2.post2/types_aiobotocore_pinpoint_email/literals.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)     9958 2023-08-04 13:46:55.000000 types-aiobotocore-pinpoint-email-2.5.2.post2/types_aiobotocore_pinpoint_email/literals.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)     6920 2023-08-04 13:46:55.000000 types-aiobotocore-pinpoint-email-2.5.2.post2/types_aiobotocore_pinpoint_email/paginator.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)     6913 2023-08-04 13:46:55.000000 types-aiobotocore-pinpoint-email-2.5.2.post2/types_aiobotocore_pinpoint_email/paginator.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:46:54.000000 types-aiobotocore-pinpoint-email-2.5.2.post2/types_aiobotocore_pinpoint_email/py.typed
--rw-r--r--   0 vlad      (1000) vlad      (1000)    35045 2023-08-04 13:46:56.000000 types-aiobotocore-pinpoint-email-2.5.2.post2/types_aiobotocore_pinpoint_email/type_defs.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)    35011 2023-08-04 13:46:55.000000 types-aiobotocore-pinpoint-email-2.5.2.post2/types_aiobotocore_pinpoint_email/type_defs.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)       65 2023-08-04 13:46:54.000000 types-aiobotocore-pinpoint-email-2.5.2.post2/types_aiobotocore_pinpoint_email/version.py
-drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:21.136643 types-aiobotocore-pinpoint-email-2.5.2.post2/types_aiobotocore_pinpoint_email.egg-info/
--rw-r--r--   0 vlad      (1000) vlad      (1000)    14046 2023-08-04 13:59:21.000000 types-aiobotocore-pinpoint-email-2.5.2.post2/types_aiobotocore_pinpoint_email.egg-info/PKG-INFO
--rw-r--r--   0 vlad      (1000) vlad      (1000)      946 2023-08-04 13:59:21.000000 types-aiobotocore-pinpoint-email-2.5.2.post2/types_aiobotocore_pinpoint_email.egg-info/SOURCES.txt
--rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:21.000000 types-aiobotocore-pinpoint-email-2.5.2.post2/types_aiobotocore_pinpoint_email.egg-info/dependency_links.txt
--rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:21.000000 types-aiobotocore-pinpoint-email-2.5.2.post2/types_aiobotocore_pinpoint_email.egg-info/not-zip-safe
--rw-r--r--   0 vlad      (1000) vlad      (1000)       52 2023-08-04 13:59:21.000000 types-aiobotocore-pinpoint-email-2.5.2.post2/types_aiobotocore_pinpoint_email.egg-info/requires.txt
--rw-r--r--   0 vlad      (1000) vlad      (1000)       33 2023-08-04 13:59:21.000000 types-aiobotocore-pinpoint-email-2.5.2.post2/types_aiobotocore_pinpoint_email.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:24:13.746749 types-aiobotocore-pinpoint-email-2.5.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-08 01:16:43.000000 types-aiobotocore-pinpoint-email-2.5.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    14040 2023-08-08 01:24:13.746749 types-aiobotocore-pinpoint-email-2.5.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    12501 2023-08-08 01:16:43.000000 types-aiobotocore-pinpoint-email-2.5.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-08 01:24:13.746749 types-aiobotocore-pinpoint-email-2.5.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2114 2023-08-08 01:16:43.000000 types-aiobotocore-pinpoint-email-2.5.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:24:13.746749 types-aiobotocore-pinpoint-email-2.5.4/types_aiobotocore_pinpoint_email/
+-rw-r--r--   0 runner    (1001) docker     (123)     1700 2023-08-08 01:16:43.000000 types-aiobotocore-pinpoint-email-2.5.4/types_aiobotocore_pinpoint_email/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1699 2023-08-08 01:16:43.000000 types-aiobotocore-pinpoint-email-2.5.4/types_aiobotocore_pinpoint_email/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      957 2023-08-08 01:16:43.000000 types-aiobotocore-pinpoint-email-2.5.4/types_aiobotocore_pinpoint_email/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35092 2023-08-08 01:16:43.000000 types-aiobotocore-pinpoint-email-2.5.4/types_aiobotocore_pinpoint_email/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35036 2023-08-08 01:16:43.000000 types-aiobotocore-pinpoint-email-2.5.4/types_aiobotocore_pinpoint_email/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9960 2023-08-08 01:16:44.000000 types-aiobotocore-pinpoint-email-2.5.4/types_aiobotocore_pinpoint_email/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9958 2023-08-08 01:16:44.000000 types-aiobotocore-pinpoint-email-2.5.4/types_aiobotocore_pinpoint_email/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     6920 2023-08-08 01:16:43.000000 types-aiobotocore-pinpoint-email-2.5.4/types_aiobotocore_pinpoint_email/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6913 2023-08-08 01:16:43.000000 types-aiobotocore-pinpoint-email-2.5.4/types_aiobotocore_pinpoint_email/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 01:16:43.000000 types-aiobotocore-pinpoint-email-2.5.4/types_aiobotocore_pinpoint_email/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    35045 2023-08-08 01:16:44.000000 types-aiobotocore-pinpoint-email-2.5.4/types_aiobotocore_pinpoint_email/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35011 2023-08-08 01:16:44.000000 types-aiobotocore-pinpoint-email-2.5.4/types_aiobotocore_pinpoint_email/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-08-08 01:16:43.000000 types-aiobotocore-pinpoint-email-2.5.4/types_aiobotocore_pinpoint_email/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:24:13.746749 types-aiobotocore-pinpoint-email-2.5.4/types_aiobotocore_pinpoint_email.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    14040 2023-08-08 01:24:13.000000 types-aiobotocore-pinpoint-email-2.5.4/types_aiobotocore_pinpoint_email.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      946 2023-08-08 01:24:13.000000 types-aiobotocore-pinpoint-email-2.5.4/types_aiobotocore_pinpoint_email.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 01:24:13.000000 types-aiobotocore-pinpoint-email-2.5.4/types_aiobotocore_pinpoint_email.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 01:24:13.000000 types-aiobotocore-pinpoint-email-2.5.4/types_aiobotocore_pinpoint_email.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-08 01:24:13.000000 types-aiobotocore-pinpoint-email-2.5.4/types_aiobotocore_pinpoint_email.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-08-08 01:24:13.000000 types-aiobotocore-pinpoint-email-2.5.4/types_aiobotocore_pinpoint_email.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-pinpoint-email-2.5.2.post2/LICENSE` & `types-aiobotocore-pinpoint-email-2.5.4/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-pinpoint-email-2.5.2.post2/PKG-INFO` & `types-aiobotocore-pinpoint-email-2.5.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-pinpoint-email
-Version: 2.5.2.post2
-Summary: Type annotations for aiobotocore.PinpointEmail 2.5.2 service generated with mypy-boto3-builder 7.17.2
+Version: 2.5.4
+Summary: Type annotations for aiobotocore.PinpointEmail 2.5.4 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_pinpoint_email/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-pinpoint-email.svg?color=blue)](https://pypi.org/project/types-aiobotocore-pinpoint-email)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_pinpoint_email/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-pinpoint-email)](https://pepy.tech/project/types-aiobotocore-pinpoint-email)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.PinpointEmail 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-email.html#PinpointEmail)
+[aiobotocore.PinpointEmail 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-email.html#PinpointEmail)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-pinpoint-email-2.5.2.post2/README.md` & `types-aiobotocore-pinpoint-email-2.5.4/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-pinpoint-email.svg?color=blue)](https://pypi.org/project/types-aiobotocore-pinpoint-email)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_pinpoint_email/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-pinpoint-email)](https://pepy.tech/project/types-aiobotocore-pinpoint-email)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.PinpointEmail 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-email.html#PinpointEmail)
+[aiobotocore.PinpointEmail 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-email.html#PinpointEmail)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-pinpoint-email-2.5.2.post2/setup.py` & `types-aiobotocore-pinpoint-email-2.5.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-pinpoint-email",
-    version="2.5.2.post2",
+    version="2.5.4",
     packages=["types_aiobotocore_pinpoint_email"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.PinpointEmail 2.5.2 service generated with"
+        "Type annotations for aiobotocore.PinpointEmail 2.5.4 service generated with"
         " mypy-boto3-builder 7.17.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
```

### Comparing `types-aiobotocore-pinpoint-email-2.5.2.post2/types_aiobotocore_pinpoint_email/__init__.py` & `types-aiobotocore-pinpoint-email-2.5.4/types_aiobotocore_pinpoint_email/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-pinpoint-email-2.5.2.post2/types_aiobotocore_pinpoint_email/__init__.pyi` & `types-aiobotocore-pinpoint-email-2.5.4/types_aiobotocore_pinpoint_email/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-pinpoint-email-2.5.2.post2/types_aiobotocore_pinpoint_email/client.py` & `types-aiobotocore-pinpoint-email-2.5.4/types_aiobotocore_pinpoint_email/client.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-pinpoint-email-2.5.2.post2/types_aiobotocore_pinpoint_email/client.pyi` & `types-aiobotocore-pinpoint-email-2.5.4/types_aiobotocore_pinpoint_email/client.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-pinpoint-email-2.5.2.post2/types_aiobotocore_pinpoint_email/literals.py` & `types-aiobotocore-pinpoint-email-2.5.4/types_aiobotocore_pinpoint_email/literals.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-pinpoint-email-2.5.2.post2/types_aiobotocore_pinpoint_email/literals.pyi` & `types-aiobotocore-pinpoint-email-2.5.4/types_aiobotocore_pinpoint_email/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-pinpoint-email-2.5.2.post2/types_aiobotocore_pinpoint_email/paginator.py` & `types-aiobotocore-pinpoint-email-2.5.4/types_aiobotocore_pinpoint_email/paginator.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-pinpoint-email-2.5.2.post2/types_aiobotocore_pinpoint_email/paginator.pyi` & `types-aiobotocore-pinpoint-email-2.5.4/types_aiobotocore_pinpoint_email/paginator.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-pinpoint-email-2.5.2.post2/types_aiobotocore_pinpoint_email/type_defs.py` & `types-aiobotocore-pinpoint-email-2.5.4/types_aiobotocore_pinpoint_email/type_defs.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-pinpoint-email-2.5.2.post2/types_aiobotocore_pinpoint_email/type_defs.pyi` & `types-aiobotocore-pinpoint-email-2.5.4/types_aiobotocore_pinpoint_email/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-pinpoint-email-2.5.2.post2/types_aiobotocore_pinpoint_email.egg-info/PKG-INFO` & `types-aiobotocore-pinpoint-email-2.5.4/types_aiobotocore_pinpoint_email.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-pinpoint-email
-Version: 2.5.2.post2
-Summary: Type annotations for aiobotocore.PinpointEmail 2.5.2 service generated with mypy-boto3-builder 7.17.2
+Version: 2.5.4
+Summary: Type annotations for aiobotocore.PinpointEmail 2.5.4 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_pinpoint_email/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-pinpoint-email.svg?color=blue)](https://pypi.org/project/types-aiobotocore-pinpoint-email)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_pinpoint_email/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-pinpoint-email)](https://pepy.tech/project/types-aiobotocore-pinpoint-email)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.PinpointEmail 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-email.html#PinpointEmail)
+[aiobotocore.PinpointEmail 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-email.html#PinpointEmail)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-pinpoint-email-2.5.2.post2/types_aiobotocore_pinpoint_email.egg-info/SOURCES.txt` & `types-aiobotocore-pinpoint-email-2.5.4/types_aiobotocore_pinpoint_email.egg-info/SOURCES.txt`

 * *Files identical despite different names*


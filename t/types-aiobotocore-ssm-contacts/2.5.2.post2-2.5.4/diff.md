# Comparing `tmp/types-aiobotocore-ssm-contacts-2.5.2.post2.tar.gz` & `tmp/types-aiobotocore-ssm-contacts-2.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-ssm-contacts-2.5.2.post2.tar", last modified: Fri Aug  4 13:59:27 2023, max compression
+gzip compressed data, was "types-aiobotocore-ssm-contacts-2.5.4.tar", last modified: Tue Aug  8 01:24:29 2023, max compression
```

## Comparing `types-aiobotocore-ssm-contacts-2.5.2.post2.tar` & `types-aiobotocore-ssm-contacts-2.5.4.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:27.476643 types-aiobotocore-ssm-contacts-2.5.2.post2/
--rw-r--r--   0 vlad      (1000) vlad      (1000)     1070 2023-08-04 13:54:18.000000 types-aiobotocore-ssm-contacts-2.5.2.post2/LICENSE
--rw-r--r--   0 vlad      (1000) vlad      (1000)    14792 2023-08-04 13:59:27.476643 types-aiobotocore-ssm-contacts-2.5.2.post2/PKG-INFO
--rw-r--r--   0 vlad      (1000) vlad      (1000)    13255 2023-08-04 13:54:18.000000 types-aiobotocore-ssm-contacts-2.5.2.post2/README.md
--rw-r--r--   0 vlad      (1000) vlad      (1000)       38 2023-08-04 13:59:27.476643 types-aiobotocore-ssm-contacts-2.5.2.post2/setup.cfg
--rw-r--r--   0 vlad      (1000) vlad      (1000)     2106 2023-08-04 13:54:18.000000 types-aiobotocore-ssm-contacts-2.5.2.post2/setup.py
-drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:27.466643 types-aiobotocore-ssm-contacts-2.5.2.post2/types_aiobotocore_ssm_contacts/
--rw-r--r--   0 vlad      (1000) vlad      (1000)     2886 2023-08-04 13:54:18.000000 types-aiobotocore-ssm-contacts-2.5.2.post2/types_aiobotocore_ssm_contacts/__init__.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)     2885 2023-08-04 13:54:18.000000 types-aiobotocore-ssm-contacts-2.5.2.post2/types_aiobotocore_ssm_contacts/__init__.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)      961 2023-08-04 13:54:18.000000 types-aiobotocore-ssm-contacts-2.5.2.post2/types_aiobotocore_ssm_contacts/__main__.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)    34323 2023-08-04 13:54:19.000000 types-aiobotocore-ssm-contacts-2.5.2.post2/types_aiobotocore_ssm_contacts/client.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)    34264 2023-08-04 13:54:19.000000 types-aiobotocore-ssm-contacts-2.5.2.post2/types_aiobotocore_ssm_contacts/client.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)    10176 2023-08-04 13:54:19.000000 types-aiobotocore-ssm-contacts-2.5.2.post2/types_aiobotocore_ssm_contacts/literals.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)    10174 2023-08-04 13:54:19.000000 types-aiobotocore-ssm-contacts-2.5.2.post2/types_aiobotocore_ssm_contacts/literals.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)    14392 2023-08-04 13:54:19.000000 types-aiobotocore-ssm-contacts-2.5.2.post2/types_aiobotocore_ssm_contacts/paginator.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)    14379 2023-08-04 13:54:19.000000 types-aiobotocore-ssm-contacts-2.5.2.post2/types_aiobotocore_ssm_contacts/paginator.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:54:18.000000 types-aiobotocore-ssm-contacts-2.5.2.post2/types_aiobotocore_ssm_contacts/py.typed
--rw-r--r--   0 vlad      (1000) vlad      (1000)    39429 2023-08-04 13:54:20.000000 types-aiobotocore-ssm-contacts-2.5.2.post2/types_aiobotocore_ssm_contacts/type_defs.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)    39354 2023-08-04 13:54:20.000000 types-aiobotocore-ssm-contacts-2.5.2.post2/types_aiobotocore_ssm_contacts/type_defs.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)       65 2023-08-04 13:54:18.000000 types-aiobotocore-ssm-contacts-2.5.2.post2/types_aiobotocore_ssm_contacts/version.py
-drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:27.466643 types-aiobotocore-ssm-contacts-2.5.2.post2/types_aiobotocore_ssm_contacts.egg-info/
--rw-r--r--   0 vlad      (1000) vlad      (1000)    14792 2023-08-04 13:59:27.000000 types-aiobotocore-ssm-contacts-2.5.2.post2/types_aiobotocore_ssm_contacts.egg-info/PKG-INFO
--rw-r--r--   0 vlad      (1000) vlad      (1000)      908 2023-08-04 13:59:27.000000 types-aiobotocore-ssm-contacts-2.5.2.post2/types_aiobotocore_ssm_contacts.egg-info/SOURCES.txt
--rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:27.000000 types-aiobotocore-ssm-contacts-2.5.2.post2/types_aiobotocore_ssm_contacts.egg-info/dependency_links.txt
--rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:27.000000 types-aiobotocore-ssm-contacts-2.5.2.post2/types_aiobotocore_ssm_contacts.egg-info/not-zip-safe
--rw-r--r--   0 vlad      (1000) vlad      (1000)       52 2023-08-04 13:59:27.000000 types-aiobotocore-ssm-contacts-2.5.2.post2/types_aiobotocore_ssm_contacts.egg-info/requires.txt
--rw-r--r--   0 vlad      (1000) vlad      (1000)       31 2023-08-04 13:59:27.000000 types-aiobotocore-ssm-contacts-2.5.2.post2/types_aiobotocore_ssm_contacts.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:24:29.574789 types-aiobotocore-ssm-contacts-2.5.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-08 01:21:34.000000 types-aiobotocore-ssm-contacts-2.5.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    14786 2023-08-08 01:24:29.566789 types-aiobotocore-ssm-contacts-2.5.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    13255 2023-08-08 01:21:34.000000 types-aiobotocore-ssm-contacts-2.5.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-08 01:24:29.574789 types-aiobotocore-ssm-contacts-2.5.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2100 2023-08-08 01:21:34.000000 types-aiobotocore-ssm-contacts-2.5.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:24:29.566789 types-aiobotocore-ssm-contacts-2.5.4/types_aiobotocore_ssm_contacts/
+-rw-r--r--   0 runner    (1001) docker     (123)     2886 2023-08-08 01:21:34.000000 types-aiobotocore-ssm-contacts-2.5.4/types_aiobotocore_ssm_contacts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2885 2023-08-08 01:21:34.000000 types-aiobotocore-ssm-contacts-2.5.4/types_aiobotocore_ssm_contacts/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      949 2023-08-08 01:21:34.000000 types-aiobotocore-ssm-contacts-2.5.4/types_aiobotocore_ssm_contacts/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34323 2023-08-08 01:21:34.000000 types-aiobotocore-ssm-contacts-2.5.4/types_aiobotocore_ssm_contacts/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34264 2023-08-08 01:21:34.000000 types-aiobotocore-ssm-contacts-2.5.4/types_aiobotocore_ssm_contacts/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    10176 2023-08-08 01:21:35.000000 types-aiobotocore-ssm-contacts-2.5.4/types_aiobotocore_ssm_contacts/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10174 2023-08-08 01:21:34.000000 types-aiobotocore-ssm-contacts-2.5.4/types_aiobotocore_ssm_contacts/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    14392 2023-08-08 01:21:34.000000 types-aiobotocore-ssm-contacts-2.5.4/types_aiobotocore_ssm_contacts/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14379 2023-08-08 01:21:34.000000 types-aiobotocore-ssm-contacts-2.5.4/types_aiobotocore_ssm_contacts/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 01:21:34.000000 types-aiobotocore-ssm-contacts-2.5.4/types_aiobotocore_ssm_contacts/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    39429 2023-08-08 01:21:35.000000 types-aiobotocore-ssm-contacts-2.5.4/types_aiobotocore_ssm_contacts/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39354 2023-08-08 01:21:35.000000 types-aiobotocore-ssm-contacts-2.5.4/types_aiobotocore_ssm_contacts/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-08-08 01:21:34.000000 types-aiobotocore-ssm-contacts-2.5.4/types_aiobotocore_ssm_contacts/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:24:29.566789 types-aiobotocore-ssm-contacts-2.5.4/types_aiobotocore_ssm_contacts.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    14786 2023-08-08 01:24:29.000000 types-aiobotocore-ssm-contacts-2.5.4/types_aiobotocore_ssm_contacts.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      908 2023-08-08 01:24:29.000000 types-aiobotocore-ssm-contacts-2.5.4/types_aiobotocore_ssm_contacts.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 01:24:29.000000 types-aiobotocore-ssm-contacts-2.5.4/types_aiobotocore_ssm_contacts.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 01:24:29.000000 types-aiobotocore-ssm-contacts-2.5.4/types_aiobotocore_ssm_contacts.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-08 01:24:29.000000 types-aiobotocore-ssm-contacts-2.5.4/types_aiobotocore_ssm_contacts.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-08-08 01:24:29.000000 types-aiobotocore-ssm-contacts-2.5.4/types_aiobotocore_ssm_contacts.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-ssm-contacts-2.5.2.post2/LICENSE` & `types-aiobotocore-ssm-contacts-2.5.4/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-ssm-contacts-2.5.2.post2/PKG-INFO` & `types-aiobotocore-ssm-contacts-2.5.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-ssm-contacts
-Version: 2.5.2.post2
-Summary: Type annotations for aiobotocore.SSMContacts 2.5.2 service generated with mypy-boto3-builder 7.17.2
+Version: 2.5.4
+Summary: Type annotations for aiobotocore.SSMContacts 2.5.4 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm_contacts/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-ssm-contacts.svg?color=blue)](https://pypi.org/project/types-aiobotocore-ssm-contacts)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm_contacts/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-ssm-contacts)](https://pepy.tech/project/types-aiobotocore-ssm-contacts)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.SSMContacts 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-contacts.html#SSMContacts)
+[aiobotocore.SSMContacts 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-contacts.html#SSMContacts)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-ssm-contacts-2.5.2.post2/README.md` & `types-aiobotocore-ssm-contacts-2.5.4/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-ssm-contacts.svg?color=blue)](https://pypi.org/project/types-aiobotocore-ssm-contacts)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm_contacts/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-ssm-contacts)](https://pepy.tech/project/types-aiobotocore-ssm-contacts)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.SSMContacts 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-contacts.html#SSMContacts)
+[aiobotocore.SSMContacts 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-contacts.html#SSMContacts)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-ssm-contacts-2.5.2.post2/setup.py` & `types-aiobotocore-ssm-contacts-2.5.4/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-ssm-contacts",
-    version="2.5.2.post2",
+    version="2.5.4",
     packages=["types_aiobotocore_ssm_contacts"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.SSMContacts 2.5.2 service generated with"
+        "Type annotations for aiobotocore.SSMContacts 2.5.4 service generated with"
         " mypy-boto3-builder 7.17.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
```

### Comparing `types-aiobotocore-ssm-contacts-2.5.2.post2/types_aiobotocore_ssm_contacts/__init__.py` & `types-aiobotocore-ssm-contacts-2.5.4/types_aiobotocore_ssm_contacts/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-ssm-contacts-2.5.2.post2/types_aiobotocore_ssm_contacts/__init__.pyi` & `types-aiobotocore-ssm-contacts-2.5.4/types_aiobotocore_ssm_contacts/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-ssm-contacts-2.5.2.post2/types_aiobotocore_ssm_contacts/__main__.py` & `types-aiobotocore-ssm-contacts-2.5.4/types_aiobotocore_ssm_contacts/__main__.py`

 * *Files 13% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.SSMContacts 2.5.2\nVersion:         2.5.2.post2\nBuilder"
+        "Type annotations for aiobotocore.SSMContacts 2.5.4\nVersion:         2.5.4\nBuilder"
         " version: 7.17.2\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm_contacts//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-contacts.html#SSMContacts\nOther"
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

### Comparing `types-aiobotocore-ssm-contacts-2.5.2.post2/types_aiobotocore_ssm_contacts/client.py` & `types-aiobotocore-ssm-contacts-2.5.4/types_aiobotocore_ssm_contacts/client.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-ssm-contacts-2.5.2.post2/types_aiobotocore_ssm_contacts/client.pyi` & `types-aiobotocore-ssm-contacts-2.5.4/types_aiobotocore_ssm_contacts/client.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-ssm-contacts-2.5.2.post2/types_aiobotocore_ssm_contacts/literals.py` & `types-aiobotocore-ssm-contacts-2.5.4/types_aiobotocore_ssm_contacts/literals.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-ssm-contacts-2.5.2.post2/types_aiobotocore_ssm_contacts/literals.pyi` & `types-aiobotocore-ssm-contacts-2.5.4/types_aiobotocore_ssm_contacts/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-ssm-contacts-2.5.2.post2/types_aiobotocore_ssm_contacts/paginator.py` & `types-aiobotocore-ssm-contacts-2.5.4/types_aiobotocore_ssm_contacts/paginator.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-ssm-contacts-2.5.2.post2/types_aiobotocore_ssm_contacts/paginator.pyi` & `types-aiobotocore-ssm-contacts-2.5.4/types_aiobotocore_ssm_contacts/paginator.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-ssm-contacts-2.5.2.post2/types_aiobotocore_ssm_contacts/type_defs.py` & `types-aiobotocore-ssm-contacts-2.5.4/types_aiobotocore_ssm_contacts/type_defs.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-ssm-contacts-2.5.2.post2/types_aiobotocore_ssm_contacts/type_defs.pyi` & `types-aiobotocore-ssm-contacts-2.5.4/types_aiobotocore_ssm_contacts/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-ssm-contacts-2.5.2.post2/types_aiobotocore_ssm_contacts.egg-info/PKG-INFO` & `types-aiobotocore-ssm-contacts-2.5.4/types_aiobotocore_ssm_contacts.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-ssm-contacts
-Version: 2.5.2.post2
-Summary: Type annotations for aiobotocore.SSMContacts 2.5.2 service generated with mypy-boto3-builder 7.17.2
+Version: 2.5.4
+Summary: Type annotations for aiobotocore.SSMContacts 2.5.4 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm_contacts/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-ssm-contacts.svg?color=blue)](https://pypi.org/project/types-aiobotocore-ssm-contacts)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm_contacts/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-ssm-contacts)](https://pepy.tech/project/types-aiobotocore-ssm-contacts)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.SSMContacts 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-contacts.html#SSMContacts)
+[aiobotocore.SSMContacts 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-contacts.html#SSMContacts)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-ssm-contacts-2.5.2.post2/types_aiobotocore_ssm_contacts.egg-info/SOURCES.txt` & `types-aiobotocore-ssm-contacts-2.5.4/types_aiobotocore_ssm_contacts.egg-info/SOURCES.txt`

 * *Files identical despite different names*


# Comparing `tmp/types-aiobotocore-payment-cryptography-2.5.2.post2.tar.gz` & `tmp/types-aiobotocore-payment-cryptography-2.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-payment-cryptography-2.5.2.post2.tar", last modified: Fri Aug  4 13:59:20 2023, max compression
+gzip compressed data, was "types-aiobotocore-payment-cryptography-2.5.4.tar", last modified: Tue Aug  8 01:24:13 2023, max compression
```

## Comparing `types-aiobotocore-payment-cryptography-2.5.2.post2.tar` & `types-aiobotocore-payment-cryptography-2.5.4.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:20.906643 types-aiobotocore-payment-cryptography-2.5.2.post2/
--rw-r--r--   0 vlad      (1000) vlad      (1000)     1070 2023-08-04 13:46:25.000000 types-aiobotocore-payment-cryptography-2.5.2.post2/LICENSE
--rw-r--r--   0 vlad      (1000) vlad      (1000)    14028 2023-08-04 13:59:20.906643 types-aiobotocore-payment-cryptography-2.5.2.post2/PKG-INFO
--rw-r--r--   0 vlad      (1000) vlad      (1000)    12447 2023-08-04 13:46:25.000000 types-aiobotocore-payment-cryptography-2.5.2.post2/README.md
--rw-r--r--   0 vlad      (1000) vlad      (1000)       38 2023-08-04 13:59:20.906643 types-aiobotocore-payment-cryptography-2.5.2.post2/setup.cfg
--rw-r--r--   0 vlad      (1000) vlad      (1000)     2166 2023-08-04 13:46:25.000000 types-aiobotocore-payment-cryptography-2.5.2.post2/setup.py
-drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:20.896643 types-aiobotocore-payment-cryptography-2.5.2.post2/types_aiobotocore_payment_cryptography/
--rw-r--r--   0 vlad      (1000) vlad      (1000)     1173 2023-08-04 13:46:25.000000 types-aiobotocore-payment-cryptography-2.5.2.post2/types_aiobotocore_payment_cryptography/__init__.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)     1172 2023-08-04 13:46:25.000000 types-aiobotocore-payment-cryptography-2.5.2.post2/types_aiobotocore_payment_cryptography/__init__.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)     1017 2023-08-04 13:46:26.000000 types-aiobotocore-payment-cryptography-2.5.2.post2/types_aiobotocore_payment_cryptography/__main__.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)    19845 2023-08-04 13:46:26.000000 types-aiobotocore-payment-cryptography-2.5.2.post2/types_aiobotocore_payment_cryptography/client.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)    19813 2023-08-04 13:46:26.000000 types-aiobotocore-payment-cryptography-2.5.2.post2/types_aiobotocore_payment_cryptography/client.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)     9922 2023-08-04 13:46:26.000000 types-aiobotocore-payment-cryptography-2.5.2.post2/types_aiobotocore_payment_cryptography/literals.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)     9920 2023-08-04 13:46:26.000000 types-aiobotocore-payment-cryptography-2.5.2.post2/types_aiobotocore_payment_cryptography/literals.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)     4539 2023-08-04 13:46:26.000000 types-aiobotocore-payment-cryptography-2.5.2.post2/types_aiobotocore_payment_cryptography/paginator.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)     4534 2023-08-04 13:46:26.000000 types-aiobotocore-payment-cryptography-2.5.2.post2/types_aiobotocore_payment_cryptography/paginator.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:46:26.000000 types-aiobotocore-payment-cryptography-2.5.2.post2/types_aiobotocore_payment_cryptography/py.typed
--rw-r--r--   0 vlad      (1000) vlad      (1000)    17665 2023-08-04 13:46:26.000000 types-aiobotocore-payment-cryptography-2.5.2.post2/types_aiobotocore_payment_cryptography/type_defs.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)    17641 2023-08-04 13:46:26.000000 types-aiobotocore-payment-cryptography-2.5.2.post2/types_aiobotocore_payment_cryptography/type_defs.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)       65 2023-08-04 13:46:25.000000 types-aiobotocore-payment-cryptography-2.5.2.post2/types_aiobotocore_payment_cryptography/version.py
-drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:20.906643 types-aiobotocore-payment-cryptography-2.5.2.post2/types_aiobotocore_payment_cryptography.egg-info/
--rw-r--r--   0 vlad      (1000) vlad      (1000)    14028 2023-08-04 13:59:20.000000 types-aiobotocore-payment-cryptography-2.5.2.post2/types_aiobotocore_payment_cryptography.egg-info/PKG-INFO
--rw-r--r--   0 vlad      (1000) vlad      (1000)     1060 2023-08-04 13:59:20.000000 types-aiobotocore-payment-cryptography-2.5.2.post2/types_aiobotocore_payment_cryptography.egg-info/SOURCES.txt
--rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:20.000000 types-aiobotocore-payment-cryptography-2.5.2.post2/types_aiobotocore_payment_cryptography.egg-info/dependency_links.txt
--rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:20.000000 types-aiobotocore-payment-cryptography-2.5.2.post2/types_aiobotocore_payment_cryptography.egg-info/not-zip-safe
--rw-r--r--   0 vlad      (1000) vlad      (1000)       52 2023-08-04 13:59:20.000000 types-aiobotocore-payment-cryptography-2.5.2.post2/types_aiobotocore_payment_cryptography.egg-info/requires.txt
--rw-r--r--   0 vlad      (1000) vlad      (1000)       39 2023-08-04 13:59:20.000000 types-aiobotocore-payment-cryptography-2.5.2.post2/types_aiobotocore_payment_cryptography.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:24:13.158748 types-aiobotocore-payment-cryptography-2.5.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-08 01:16:24.000000 types-aiobotocore-payment-cryptography-2.5.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    14022 2023-08-08 01:24:13.154748 types-aiobotocore-payment-cryptography-2.5.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    12447 2023-08-08 01:16:24.000000 types-aiobotocore-payment-cryptography-2.5.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-08 01:24:13.158748 types-aiobotocore-payment-cryptography-2.5.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2160 2023-08-08 01:16:24.000000 types-aiobotocore-payment-cryptography-2.5.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:24:13.146748 types-aiobotocore-payment-cryptography-2.5.4/types_aiobotocore_payment_cryptography/
+-rw-r--r--   0 runner    (1001) docker     (123)     1173 2023-08-08 01:16:24.000000 types-aiobotocore-payment-cryptography-2.5.4/types_aiobotocore_payment_cryptography/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1172 2023-08-08 01:16:24.000000 types-aiobotocore-payment-cryptography-2.5.4/types_aiobotocore_payment_cryptography/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1005 2023-08-08 01:16:24.000000 types-aiobotocore-payment-cryptography-2.5.4/types_aiobotocore_payment_cryptography/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19845 2023-08-08 01:16:25.000000 types-aiobotocore-payment-cryptography-2.5.4/types_aiobotocore_payment_cryptography/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19813 2023-08-08 01:16:25.000000 types-aiobotocore-payment-cryptography-2.5.4/types_aiobotocore_payment_cryptography/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9922 2023-08-08 01:16:27.000000 types-aiobotocore-payment-cryptography-2.5.4/types_aiobotocore_payment_cryptography/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9920 2023-08-08 01:16:27.000000 types-aiobotocore-payment-cryptography-2.5.4/types_aiobotocore_payment_cryptography/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     4539 2023-08-08 01:16:25.000000 types-aiobotocore-payment-cryptography-2.5.4/types_aiobotocore_payment_cryptography/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4534 2023-08-08 01:16:25.000000 types-aiobotocore-payment-cryptography-2.5.4/types_aiobotocore_payment_cryptography/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 01:16:24.000000 types-aiobotocore-payment-cryptography-2.5.4/types_aiobotocore_payment_cryptography/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    17665 2023-08-08 01:16:27.000000 types-aiobotocore-payment-cryptography-2.5.4/types_aiobotocore_payment_cryptography/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17641 2023-08-08 01:16:27.000000 types-aiobotocore-payment-cryptography-2.5.4/types_aiobotocore_payment_cryptography/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-08-08 01:16:24.000000 types-aiobotocore-payment-cryptography-2.5.4/types_aiobotocore_payment_cryptography/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:24:13.154748 types-aiobotocore-payment-cryptography-2.5.4/types_aiobotocore_payment_cryptography.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    14022 2023-08-08 01:24:12.000000 types-aiobotocore-payment-cryptography-2.5.4/types_aiobotocore_payment_cryptography.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-08-08 01:24:13.000000 types-aiobotocore-payment-cryptography-2.5.4/types_aiobotocore_payment_cryptography.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 01:24:12.000000 types-aiobotocore-payment-cryptography-2.5.4/types_aiobotocore_payment_cryptography.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 01:24:12.000000 types-aiobotocore-payment-cryptography-2.5.4/types_aiobotocore_payment_cryptography.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-08 01:24:12.000000 types-aiobotocore-payment-cryptography-2.5.4/types_aiobotocore_payment_cryptography.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-08-08 01:24:12.000000 types-aiobotocore-payment-cryptography-2.5.4/types_aiobotocore_payment_cryptography.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-payment-cryptography-2.5.2.post2/LICENSE` & `types-aiobotocore-payment-cryptography-2.5.4/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-payment-cryptography-2.5.2.post2/PKG-INFO` & `types-aiobotocore-payment-cryptography-2.5.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-payment-cryptography
-Version: 2.5.2.post2
-Summary: Type annotations for aiobotocore.PaymentCryptographyControlPlane 2.5.2 service generated with mypy-boto3-builder 7.17.2
+Version: 2.5.4
+Summary: Type annotations for aiobotocore.PaymentCryptographyControlPlane 2.5.4 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_payment_cryptography/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-payment-cryptography.svg?color=blue)](https://pypi.org/project/types-aiobotocore-payment-cryptography)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_payment_cryptography/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-payment-cryptography)](https://pepy.tech/project/types-aiobotocore-payment-cryptography)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.PaymentCryptographyControlPlane 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/payment-cryptography.html#PaymentCryptographyControlPlane)
+[aiobotocore.PaymentCryptographyControlPlane 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/payment-cryptography.html#PaymentCryptographyControlPlane)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-payment-cryptography-2.5.2.post2/README.md` & `types-aiobotocore-payment-cryptography-2.5.4/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-payment-cryptography.svg?color=blue)](https://pypi.org/project/types-aiobotocore-payment-cryptography)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_payment_cryptography/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-payment-cryptography)](https://pepy.tech/project/types-aiobotocore-payment-cryptography)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.PaymentCryptographyControlPlane 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/payment-cryptography.html#PaymentCryptographyControlPlane)
+[aiobotocore.PaymentCryptographyControlPlane 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/payment-cryptography.html#PaymentCryptographyControlPlane)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-payment-cryptography-2.5.2.post2/setup.py` & `types-aiobotocore-payment-cryptography-2.5.4/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-payment-cryptography",
-    version="2.5.2.post2",
+    version="2.5.4",
     packages=["types_aiobotocore_payment_cryptography"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.PaymentCryptographyControlPlane 2.5.2 service generated"
+        "Type annotations for aiobotocore.PaymentCryptographyControlPlane 2.5.4 service generated"
         " with mypy-boto3-builder 7.17.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
```

### Comparing `types-aiobotocore-payment-cryptography-2.5.2.post2/types_aiobotocore_payment_cryptography/__init__.py` & `types-aiobotocore-payment-cryptography-2.5.4/types_aiobotocore_payment_cryptography/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-payment-cryptography-2.5.2.post2/types_aiobotocore_payment_cryptography/__init__.pyi` & `types-aiobotocore-payment-cryptography-2.5.4/types_aiobotocore_payment_cryptography/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-payment-cryptography-2.5.2.post2/types_aiobotocore_payment_cryptography/__main__.py` & `types-aiobotocore-payment-cryptography-2.5.4/types_aiobotocore_payment_cryptography/__main__.py`

 * *Files 11% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.PaymentCryptographyControlPlane 2.5.2\nVersion:        "
-        " 2.5.2.post2\nBuilder version: 7.17.2\nDocs:           "
+        "Type annotations for aiobotocore.PaymentCryptographyControlPlane 2.5.4\nVersion:        "
+        " 2.5.4\nBuilder version: 7.17.2\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_payment_cryptography//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/payment-cryptography.html#PaymentCryptographyControlPlane\nOther"
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

### Comparing `types-aiobotocore-payment-cryptography-2.5.2.post2/types_aiobotocore_payment_cryptography/client.py` & `types-aiobotocore-payment-cryptography-2.5.4/types_aiobotocore_payment_cryptography/client.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-payment-cryptography-2.5.2.post2/types_aiobotocore_payment_cryptography/client.pyi` & `types-aiobotocore-payment-cryptography-2.5.4/types_aiobotocore_payment_cryptography/client.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-payment-cryptography-2.5.2.post2/types_aiobotocore_payment_cryptography/literals.py` & `types-aiobotocore-payment-cryptography-2.5.4/types_aiobotocore_payment_cryptography/literals.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-payment-cryptography-2.5.2.post2/types_aiobotocore_payment_cryptography/literals.pyi` & `types-aiobotocore-payment-cryptography-2.5.4/types_aiobotocore_payment_cryptography/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-payment-cryptography-2.5.2.post2/types_aiobotocore_payment_cryptography/paginator.py` & `types-aiobotocore-payment-cryptography-2.5.4/types_aiobotocore_payment_cryptography/paginator.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-payment-cryptography-2.5.2.post2/types_aiobotocore_payment_cryptography/paginator.pyi` & `types-aiobotocore-payment-cryptography-2.5.4/types_aiobotocore_payment_cryptography/paginator.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-payment-cryptography-2.5.2.post2/types_aiobotocore_payment_cryptography/type_defs.py` & `types-aiobotocore-payment-cryptography-2.5.4/types_aiobotocore_payment_cryptography/type_defs.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-payment-cryptography-2.5.2.post2/types_aiobotocore_payment_cryptography/type_defs.pyi` & `types-aiobotocore-payment-cryptography-2.5.4/types_aiobotocore_payment_cryptography/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-payment-cryptography-2.5.2.post2/types_aiobotocore_payment_cryptography.egg-info/PKG-INFO` & `types-aiobotocore-payment-cryptography-2.5.4/types_aiobotocore_payment_cryptography.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-payment-cryptography
-Version: 2.5.2.post2
-Summary: Type annotations for aiobotocore.PaymentCryptographyControlPlane 2.5.2 service generated with mypy-boto3-builder 7.17.2
+Version: 2.5.4
+Summary: Type annotations for aiobotocore.PaymentCryptographyControlPlane 2.5.4 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_payment_cryptography/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-payment-cryptography.svg?color=blue)](https://pypi.org/project/types-aiobotocore-payment-cryptography)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_payment_cryptography/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-payment-cryptography)](https://pepy.tech/project/types-aiobotocore-payment-cryptography)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.PaymentCryptographyControlPlane 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/payment-cryptography.html#PaymentCryptographyControlPlane)
+[aiobotocore.PaymentCryptographyControlPlane 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/payment-cryptography.html#PaymentCryptographyControlPlane)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-payment-cryptography-2.5.2.post2/types_aiobotocore_payment_cryptography.egg-info/SOURCES.txt` & `types-aiobotocore-payment-cryptography-2.5.4/types_aiobotocore_payment_cryptography.egg-info/SOURCES.txt`

 * *Files identical despite different names*


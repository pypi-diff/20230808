# Comparing `tmp/types-aiobotocore-payment-cryptography-data-2.5.2.post2.tar.gz` & `tmp/types-aiobotocore-payment-cryptography-data-2.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-payment-cryptography-data-2.5.2.post2.tar", last modified: Fri Aug  4 13:59:20 2023, max compression
+gzip compressed data, was "types-aiobotocore-payment-cryptography-data-2.5.4.tar", last modified: Tue Aug  8 01:24:13 2023, max compression
```

## Comparing `types-aiobotocore-payment-cryptography-data-2.5.2.post2.tar` & `types-aiobotocore-payment-cryptography-data-2.5.4.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:20.796643 types-aiobotocore-payment-cryptography-data-2.5.2.post2/
--rw-r--r--   0 vlad      (1000) vlad      (1000)     1070 2023-08-04 13:46:27.000000 types-aiobotocore-payment-cryptography-data-2.5.2.post2/LICENSE
--rw-r--r--   0 vlad      (1000) vlad      (1000)    13216 2023-08-04 13:59:20.786643 types-aiobotocore-payment-cryptography-data-2.5.2.post2/PKG-INFO
--rw-r--r--   0 vlad      (1000) vlad      (1000)    11623 2023-08-04 13:46:27.000000 types-aiobotocore-payment-cryptography-data-2.5.2.post2/README.md
--rw-r--r--   0 vlad      (1000) vlad      (1000)       38 2023-08-04 13:59:20.796643 types-aiobotocore-payment-cryptography-data-2.5.2.post2/setup.cfg
--rw-r--r--   0 vlad      (1000) vlad      (1000)     2193 2023-08-04 13:46:27.000000 types-aiobotocore-payment-cryptography-data-2.5.2.post2/setup.py
-drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:20.776643 types-aiobotocore-payment-cryptography-data-2.5.2.post2/types_aiobotocore_payment_cryptography_data/
--rw-r--r--   0 vlad      (1000) vlad      (1000)      601 2023-08-04 13:46:27.000000 types-aiobotocore-payment-cryptography-data-2.5.2.post2/types_aiobotocore_payment_cryptography_data/__init__.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)      600 2023-08-04 13:46:27.000000 types-aiobotocore-payment-cryptography-data-2.5.2.post2/types_aiobotocore_payment_cryptography_data/__init__.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)     1021 2023-08-04 13:46:27.000000 types-aiobotocore-payment-cryptography-data-2.5.2.post2/types_aiobotocore_payment_cryptography_data/__main__.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)    14727 2023-08-04 13:46:28.000000 types-aiobotocore-payment-cryptography-data-2.5.2.post2/types_aiobotocore_payment_cryptography_data/client.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)    14708 2023-08-04 13:46:27.000000 types-aiobotocore-payment-cryptography-data-2.5.2.post2/types_aiobotocore_payment_cryptography_data/client.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)     8822 2023-08-04 13:46:28.000000 types-aiobotocore-payment-cryptography-data-2.5.2.post2/types_aiobotocore_payment_cryptography_data/literals.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)     8820 2023-08-04 13:46:28.000000 types-aiobotocore-payment-cryptography-data-2.5.2.post2/types_aiobotocore_payment_cryptography_data/literals.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:46:27.000000 types-aiobotocore-payment-cryptography-data-2.5.2.post2/types_aiobotocore_payment_cryptography_data/py.typed
--rw-r--r--   0 vlad      (1000) vlad      (1000)    24018 2023-08-04 13:46:28.000000 types-aiobotocore-payment-cryptography-data-2.5.2.post2/types_aiobotocore_payment_cryptography_data/type_defs.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)    23994 2023-08-04 13:46:28.000000 types-aiobotocore-payment-cryptography-data-2.5.2.post2/types_aiobotocore_payment_cryptography_data/type_defs.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)       65 2023-08-04 13:46:27.000000 types-aiobotocore-payment-cryptography-data-2.5.2.post2/types_aiobotocore_payment_cryptography_data/version.py
-drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:20.786643 types-aiobotocore-payment-cryptography-data-2.5.2.post2/types_aiobotocore_payment_cryptography_data.egg-info/
--rw-r--r--   0 vlad      (1000) vlad      (1000)    13216 2023-08-04 13:59:20.000000 types-aiobotocore-payment-cryptography-data-2.5.2.post2/types_aiobotocore_payment_cryptography_data.egg-info/PKG-INFO
--rw-r--r--   0 vlad      (1000) vlad      (1000)     1040 2023-08-04 13:59:20.000000 types-aiobotocore-payment-cryptography-data-2.5.2.post2/types_aiobotocore_payment_cryptography_data.egg-info/SOURCES.txt
--rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:20.000000 types-aiobotocore-payment-cryptography-data-2.5.2.post2/types_aiobotocore_payment_cryptography_data.egg-info/dependency_links.txt
--rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:20.000000 types-aiobotocore-payment-cryptography-data-2.5.2.post2/types_aiobotocore_payment_cryptography_data.egg-info/not-zip-safe
--rw-r--r--   0 vlad      (1000) vlad      (1000)       52 2023-08-04 13:59:20.000000 types-aiobotocore-payment-cryptography-data-2.5.2.post2/types_aiobotocore_payment_cryptography_data.egg-info/requires.txt
--rw-r--r--   0 vlad      (1000) vlad      (1000)       44 2023-08-04 13:59:20.000000 types-aiobotocore-payment-cryptography-data-2.5.2.post2/types_aiobotocore_payment_cryptography_data.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:24:13.010748 types-aiobotocore-payment-cryptography-data-2.5.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-08 01:16:27.000000 types-aiobotocore-payment-cryptography-data-2.5.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    13210 2023-08-08 01:24:13.010748 types-aiobotocore-payment-cryptography-data-2.5.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    11623 2023-08-08 01:16:27.000000 types-aiobotocore-payment-cryptography-data-2.5.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-08 01:24:13.010748 types-aiobotocore-payment-cryptography-data-2.5.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2187 2023-08-08 01:16:27.000000 types-aiobotocore-payment-cryptography-data-2.5.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:24:12.994748 types-aiobotocore-payment-cryptography-data-2.5.4/types_aiobotocore_payment_cryptography_data/
+-rw-r--r--   0 runner    (1001) docker     (123)      601 2023-08-08 01:16:27.000000 types-aiobotocore-payment-cryptography-data-2.5.4/types_aiobotocore_payment_cryptography_data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      600 2023-08-08 01:16:27.000000 types-aiobotocore-payment-cryptography-data-2.5.4/types_aiobotocore_payment_cryptography_data/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1009 2023-08-08 01:16:27.000000 types-aiobotocore-payment-cryptography-data-2.5.4/types_aiobotocore_payment_cryptography_data/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14727 2023-08-08 01:16:28.000000 types-aiobotocore-payment-cryptography-data-2.5.4/types_aiobotocore_payment_cryptography_data/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14708 2023-08-08 01:16:27.000000 types-aiobotocore-payment-cryptography-data-2.5.4/types_aiobotocore_payment_cryptography_data/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8822 2023-08-08 01:16:28.000000 types-aiobotocore-payment-cryptography-data-2.5.4/types_aiobotocore_payment_cryptography_data/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8820 2023-08-08 01:16:28.000000 types-aiobotocore-payment-cryptography-data-2.5.4/types_aiobotocore_payment_cryptography_data/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 01:16:27.000000 types-aiobotocore-payment-cryptography-data-2.5.4/types_aiobotocore_payment_cryptography_data/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    24018 2023-08-08 01:16:28.000000 types-aiobotocore-payment-cryptography-data-2.5.4/types_aiobotocore_payment_cryptography_data/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23994 2023-08-08 01:16:28.000000 types-aiobotocore-payment-cryptography-data-2.5.4/types_aiobotocore_payment_cryptography_data/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-08-08 01:16:27.000000 types-aiobotocore-payment-cryptography-data-2.5.4/types_aiobotocore_payment_cryptography_data/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:24:12.994748 types-aiobotocore-payment-cryptography-data-2.5.4/types_aiobotocore_payment_cryptography_data.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    13210 2023-08-08 01:24:12.000000 types-aiobotocore-payment-cryptography-data-2.5.4/types_aiobotocore_payment_cryptography_data.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-08-08 01:24:12.000000 types-aiobotocore-payment-cryptography-data-2.5.4/types_aiobotocore_payment_cryptography_data.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 01:24:12.000000 types-aiobotocore-payment-cryptography-data-2.5.4/types_aiobotocore_payment_cryptography_data.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 01:24:12.000000 types-aiobotocore-payment-cryptography-data-2.5.4/types_aiobotocore_payment_cryptography_data.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-08 01:24:12.000000 types-aiobotocore-payment-cryptography-data-2.5.4/types_aiobotocore_payment_cryptography_data.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-08-08 01:24:12.000000 types-aiobotocore-payment-cryptography-data-2.5.4/types_aiobotocore_payment_cryptography_data.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-payment-cryptography-data-2.5.2.post2/LICENSE` & `types-aiobotocore-payment-cryptography-data-2.5.4/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-payment-cryptography-data-2.5.2.post2/PKG-INFO` & `types-aiobotocore-payment-cryptography-data-2.5.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-payment-cryptography-data
-Version: 2.5.2.post2
-Summary: Type annotations for aiobotocore.PaymentCryptographyDataPlane 2.5.2 service generated with mypy-boto3-builder 7.17.2
+Version: 2.5.4
+Summary: Type annotations for aiobotocore.PaymentCryptographyDataPlane 2.5.4 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_payment_cryptography_data/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-payment-cryptography-data.svg?color=blue)](https://pypi.org/project/types-aiobotocore-payment-cryptography-data)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_payment_cryptography_data/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-payment-cryptography-data)](https://pepy.tech/project/types-aiobotocore-payment-cryptography-data)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.PaymentCryptographyDataPlane 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/payment-cryptography-data.html#PaymentCryptographyDataPlane)
+[aiobotocore.PaymentCryptographyDataPlane 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/payment-cryptography-data.html#PaymentCryptographyDataPlane)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-payment-cryptography-data-2.5.2.post2/README.md` & `types-aiobotocore-payment-cryptography-data-2.5.4/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-payment-cryptography-data.svg?color=blue)](https://pypi.org/project/types-aiobotocore-payment-cryptography-data)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_payment_cryptography_data/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-payment-cryptography-data)](https://pepy.tech/project/types-aiobotocore-payment-cryptography-data)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.PaymentCryptographyDataPlane 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/payment-cryptography-data.html#PaymentCryptographyDataPlane)
+[aiobotocore.PaymentCryptographyDataPlane 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/payment-cryptography-data.html#PaymentCryptographyDataPlane)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-payment-cryptography-data-2.5.2.post2/setup.py` & `types-aiobotocore-payment-cryptography-data-2.5.4/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-payment-cryptography-data",
-    version="2.5.2.post2",
+    version="2.5.4",
     packages=["types_aiobotocore_payment_cryptography_data"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.PaymentCryptographyDataPlane 2.5.2 service generated with"
+        "Type annotations for aiobotocore.PaymentCryptographyDataPlane 2.5.4 service generated with"
         " mypy-boto3-builder 7.17.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
```

### Comparing `types-aiobotocore-payment-cryptography-data-2.5.2.post2/types_aiobotocore_payment_cryptography_data/__init__.py` & `types-aiobotocore-payment-cryptography-data-2.5.4/types_aiobotocore_payment_cryptography_data/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-payment-cryptography-data-2.5.2.post2/types_aiobotocore_payment_cryptography_data/__init__.pyi` & `types-aiobotocore-payment-cryptography-data-2.5.4/types_aiobotocore_payment_cryptography_data/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-payment-cryptography-data-2.5.2.post2/types_aiobotocore_payment_cryptography_data/__main__.py` & `types-aiobotocore-payment-cryptography-data-2.5.4/types_aiobotocore_payment_cryptography_data/__main__.py`

 * *Files 9% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.PaymentCryptographyDataPlane 2.5.2\nVersion:        "
-        " 2.5.2.post2\nBuilder version: 7.17.2\nDocs:           "
+        "Type annotations for aiobotocore.PaymentCryptographyDataPlane 2.5.4\nVersion:        "
+        " 2.5.4\nBuilder version: 7.17.2\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_payment_cryptography_data//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/payment-cryptography-data.html#PaymentCryptographyDataPlane\nOther"
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

### Comparing `types-aiobotocore-payment-cryptography-data-2.5.2.post2/types_aiobotocore_payment_cryptography_data/client.py` & `types-aiobotocore-payment-cryptography-data-2.5.4/types_aiobotocore_payment_cryptography_data/client.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-payment-cryptography-data-2.5.2.post2/types_aiobotocore_payment_cryptography_data/client.pyi` & `types-aiobotocore-payment-cryptography-data-2.5.4/types_aiobotocore_payment_cryptography_data/client.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-payment-cryptography-data-2.5.2.post2/types_aiobotocore_payment_cryptography_data/literals.py` & `types-aiobotocore-payment-cryptography-data-2.5.4/types_aiobotocore_payment_cryptography_data/literals.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-payment-cryptography-data-2.5.2.post2/types_aiobotocore_payment_cryptography_data/literals.pyi` & `types-aiobotocore-payment-cryptography-data-2.5.4/types_aiobotocore_payment_cryptography_data/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-payment-cryptography-data-2.5.2.post2/types_aiobotocore_payment_cryptography_data/type_defs.py` & `types-aiobotocore-payment-cryptography-data-2.5.4/types_aiobotocore_payment_cryptography_data/type_defs.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-payment-cryptography-data-2.5.2.post2/types_aiobotocore_payment_cryptography_data/type_defs.pyi` & `types-aiobotocore-payment-cryptography-data-2.5.4/types_aiobotocore_payment_cryptography_data/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-payment-cryptography-data-2.5.2.post2/types_aiobotocore_payment_cryptography_data.egg-info/PKG-INFO` & `types-aiobotocore-payment-cryptography-data-2.5.4/types_aiobotocore_payment_cryptography_data.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-payment-cryptography-data
-Version: 2.5.2.post2
-Summary: Type annotations for aiobotocore.PaymentCryptographyDataPlane 2.5.2 service generated with mypy-boto3-builder 7.17.2
+Version: 2.5.4
+Summary: Type annotations for aiobotocore.PaymentCryptographyDataPlane 2.5.4 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_payment_cryptography_data/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-payment-cryptography-data.svg?color=blue)](https://pypi.org/project/types-aiobotocore-payment-cryptography-data)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_payment_cryptography_data/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-payment-cryptography-data)](https://pepy.tech/project/types-aiobotocore-payment-cryptography-data)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.PaymentCryptographyDataPlane 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/payment-cryptography-data.html#PaymentCryptographyDataPlane)
+[aiobotocore.PaymentCryptographyDataPlane 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/payment-cryptography-data.html#PaymentCryptographyDataPlane)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-payment-cryptography-data-2.5.2.post2/types_aiobotocore_payment_cryptography_data.egg-info/SOURCES.txt` & `types-aiobotocore-payment-cryptography-data-2.5.4/types_aiobotocore_payment_cryptography_data.egg-info/SOURCES.txt`

 * *Files identical despite different names*


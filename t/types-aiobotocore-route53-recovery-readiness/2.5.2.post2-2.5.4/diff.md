# Comparing `tmp/types-aiobotocore-route53-recovery-readiness-2.5.2.post2.tar.gz` & `tmp/types-aiobotocore-route53-recovery-readiness-2.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-route53-recovery-readiness-2.5.2.post2.tar", last modified: Fri Aug  4 13:59:23 2023, max compression
+gzip compressed data, was "types-aiobotocore-route53-recovery-readiness-2.5.4.tar", last modified: Tue Aug  8 01:24:20 2023, max compression
```

## Comparing `types-aiobotocore-route53-recovery-readiness-2.5.2.post2.tar` & `types-aiobotocore-route53-recovery-readiness-2.5.4.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:23.876643 types-aiobotocore-route53-recovery-readiness-2.5.2.post2/
--rw-r--r--   0 vlad      (1000) vlad      (1000)     1070 2023-08-04 13:51:10.000000 types-aiobotocore-route53-recovery-readiness-2.5.2.post2/LICENSE
--rw-r--r--   0 vlad      (1000) vlad      (1000)    15606 2023-08-04 13:59:23.876643 types-aiobotocore-route53-recovery-readiness-2.5.2.post2/PKG-INFO
--rw-r--r--   0 vlad      (1000) vlad      (1000)    14014 2023-08-04 13:51:10.000000 types-aiobotocore-route53-recovery-readiness-2.5.2.post2/README.md
--rw-r--r--   0 vlad      (1000) vlad      (1000)       38 2023-08-04 13:59:23.876643 types-aiobotocore-route53-recovery-readiness-2.5.2.post2/setup.cfg
--rw-r--r--   0 vlad      (1000) vlad      (1000)     2206 2023-08-04 13:51:10.000000 types-aiobotocore-route53-recovery-readiness-2.5.2.post2/setup.py
-drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:23.876643 types-aiobotocore-route53-recovery-readiness-2.5.2.post2/types_aiobotocore_route53_recovery_readiness/
--rw-r--r--   0 vlad      (1000) vlad      (1000)     2973 2023-08-04 13:51:10.000000 types-aiobotocore-route53-recovery-readiness-2.5.2.post2/types_aiobotocore_route53_recovery_readiness/__init__.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)     2972 2023-08-04 13:51:10.000000 types-aiobotocore-route53-recovery-readiness-2.5.2.post2/types_aiobotocore_route53_recovery_readiness/__init__.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)     1015 2023-08-04 13:51:10.000000 types-aiobotocore-route53-recovery-readiness-2.5.2.post2/types_aiobotocore_route53_recovery_readiness/__main__.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)    30666 2023-08-04 13:51:11.000000 types-aiobotocore-route53-recovery-readiness-2.5.2.post2/types_aiobotocore_route53_recovery_readiness/client.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)    30615 2023-08-04 13:51:10.000000 types-aiobotocore-route53-recovery-readiness-2.5.2.post2/types_aiobotocore_route53_recovery_readiness/client.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)     9384 2023-08-04 13:51:11.000000 types-aiobotocore-route53-recovery-readiness-2.5.2.post2/types_aiobotocore_route53_recovery_readiness/literals.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)     9382 2023-08-04 13:51:11.000000 types-aiobotocore-route53-recovery-readiness-2.5.2.post2/types_aiobotocore_route53_recovery_readiness/literals.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)    13790 2023-08-04 13:51:11.000000 types-aiobotocore-route53-recovery-readiness-2.5.2.post2/types_aiobotocore_route53_recovery_readiness/paginator.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)    13778 2023-08-04 13:51:11.000000 types-aiobotocore-route53-recovery-readiness-2.5.2.post2/types_aiobotocore_route53_recovery_readiness/paginator.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:51:10.000000 types-aiobotocore-route53-recovery-readiness-2.5.2.post2/types_aiobotocore_route53_recovery_readiness/py.typed
--rw-r--r--   0 vlad      (1000) vlad      (1000)    29773 2023-08-04 13:51:12.000000 types-aiobotocore-route53-recovery-readiness-2.5.2.post2/types_aiobotocore_route53_recovery_readiness/type_defs.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)    29736 2023-08-04 13:51:11.000000 types-aiobotocore-route53-recovery-readiness-2.5.2.post2/types_aiobotocore_route53_recovery_readiness/type_defs.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)       65 2023-08-04 13:51:10.000000 types-aiobotocore-route53-recovery-readiness-2.5.2.post2/types_aiobotocore_route53_recovery_readiness/version.py
-drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:23.876643 types-aiobotocore-route53-recovery-readiness-2.5.2.post2/types_aiobotocore_route53_recovery_readiness.egg-info/
--rw-r--r--   0 vlad      (1000) vlad      (1000)    15606 2023-08-04 13:59:23.000000 types-aiobotocore-route53-recovery-readiness-2.5.2.post2/types_aiobotocore_route53_recovery_readiness.egg-info/PKG-INFO
--rw-r--r--   0 vlad      (1000) vlad      (1000)     1174 2023-08-04 13:59:23.000000 types-aiobotocore-route53-recovery-readiness-2.5.2.post2/types_aiobotocore_route53_recovery_readiness.egg-info/SOURCES.txt
--rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:23.000000 types-aiobotocore-route53-recovery-readiness-2.5.2.post2/types_aiobotocore_route53_recovery_readiness.egg-info/dependency_links.txt
--rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:23.000000 types-aiobotocore-route53-recovery-readiness-2.5.2.post2/types_aiobotocore_route53_recovery_readiness.egg-info/not-zip-safe
--rw-r--r--   0 vlad      (1000) vlad      (1000)       52 2023-08-04 13:59:23.000000 types-aiobotocore-route53-recovery-readiness-2.5.2.post2/types_aiobotocore_route53_recovery_readiness.egg-info/requires.txt
--rw-r--r--   0 vlad      (1000) vlad      (1000)       45 2023-08-04 13:59:23.000000 types-aiobotocore-route53-recovery-readiness-2.5.2.post2/types_aiobotocore_route53_recovery_readiness.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:24:20.622766 types-aiobotocore-route53-recovery-readiness-2.5.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-08 01:19:39.000000 types-aiobotocore-route53-recovery-readiness-2.5.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    15600 2023-08-08 01:24:20.622766 types-aiobotocore-route53-recovery-readiness-2.5.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    14014 2023-08-08 01:19:39.000000 types-aiobotocore-route53-recovery-readiness-2.5.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-08 01:24:20.622766 types-aiobotocore-route53-recovery-readiness-2.5.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2200 2023-08-08 01:19:39.000000 types-aiobotocore-route53-recovery-readiness-2.5.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:24:20.622766 types-aiobotocore-route53-recovery-readiness-2.5.4/types_aiobotocore_route53_recovery_readiness/
+-rw-r--r--   0 runner    (1001) docker     (123)     2973 2023-08-08 01:19:39.000000 types-aiobotocore-route53-recovery-readiness-2.5.4/types_aiobotocore_route53_recovery_readiness/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2972 2023-08-08 01:19:39.000000 types-aiobotocore-route53-recovery-readiness-2.5.4/types_aiobotocore_route53_recovery_readiness/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1003 2023-08-08 01:19:39.000000 types-aiobotocore-route53-recovery-readiness-2.5.4/types_aiobotocore_route53_recovery_readiness/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30666 2023-08-08 01:19:39.000000 types-aiobotocore-route53-recovery-readiness-2.5.4/types_aiobotocore_route53_recovery_readiness/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30615 2023-08-08 01:19:39.000000 types-aiobotocore-route53-recovery-readiness-2.5.4/types_aiobotocore_route53_recovery_readiness/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9384 2023-08-08 01:19:40.000000 types-aiobotocore-route53-recovery-readiness-2.5.4/types_aiobotocore_route53_recovery_readiness/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9382 2023-08-08 01:19:39.000000 types-aiobotocore-route53-recovery-readiness-2.5.4/types_aiobotocore_route53_recovery_readiness/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    13790 2023-08-08 01:19:39.000000 types-aiobotocore-route53-recovery-readiness-2.5.4/types_aiobotocore_route53_recovery_readiness/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13778 2023-08-08 01:19:39.000000 types-aiobotocore-route53-recovery-readiness-2.5.4/types_aiobotocore_route53_recovery_readiness/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 01:19:39.000000 types-aiobotocore-route53-recovery-readiness-2.5.4/types_aiobotocore_route53_recovery_readiness/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    29773 2023-08-08 01:19:40.000000 types-aiobotocore-route53-recovery-readiness-2.5.4/types_aiobotocore_route53_recovery_readiness/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29736 2023-08-08 01:19:40.000000 types-aiobotocore-route53-recovery-readiness-2.5.4/types_aiobotocore_route53_recovery_readiness/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-08-08 01:19:39.000000 types-aiobotocore-route53-recovery-readiness-2.5.4/types_aiobotocore_route53_recovery_readiness/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:24:20.622766 types-aiobotocore-route53-recovery-readiness-2.5.4/types_aiobotocore_route53_recovery_readiness.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    15600 2023-08-08 01:24:20.000000 types-aiobotocore-route53-recovery-readiness-2.5.4/types_aiobotocore_route53_recovery_readiness.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1174 2023-08-08 01:24:20.000000 types-aiobotocore-route53-recovery-readiness-2.5.4/types_aiobotocore_route53_recovery_readiness.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 01:24:20.000000 types-aiobotocore-route53-recovery-readiness-2.5.4/types_aiobotocore_route53_recovery_readiness.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 01:24:20.000000 types-aiobotocore-route53-recovery-readiness-2.5.4/types_aiobotocore_route53_recovery_readiness.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-08 01:24:20.000000 types-aiobotocore-route53-recovery-readiness-2.5.4/types_aiobotocore_route53_recovery_readiness.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-08-08 01:24:20.000000 types-aiobotocore-route53-recovery-readiness-2.5.4/types_aiobotocore_route53_recovery_readiness.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-route53-recovery-readiness-2.5.2.post2/LICENSE` & `types-aiobotocore-route53-recovery-readiness-2.5.4/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-route53-recovery-readiness-2.5.2.post2/PKG-INFO` & `types-aiobotocore-route53-recovery-readiness-2.5.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-route53-recovery-readiness
-Version: 2.5.2.post2
-Summary: Type annotations for aiobotocore.Route53RecoveryReadiness 2.5.2 service generated with mypy-boto3-builder 7.17.2
+Version: 2.5.4
+Summary: Type annotations for aiobotocore.Route53RecoveryReadiness 2.5.4 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_route53_recovery_readiness/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-route53-recovery-readiness.svg?color=blue)](https://pypi.org/project/types-aiobotocore-route53-recovery-readiness)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_route53_recovery_readiness/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-route53-recovery-readiness)](https://pepy.tech/project/types-aiobotocore-route53-recovery-readiness)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.Route53RecoveryReadiness 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53-recovery-readiness.html#Route53RecoveryReadiness)
+[aiobotocore.Route53RecoveryReadiness 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53-recovery-readiness.html#Route53RecoveryReadiness)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-route53-recovery-readiness-2.5.2.post2/README.md` & `types-aiobotocore-route53-recovery-readiness-2.5.4/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-route53-recovery-readiness.svg?color=blue)](https://pypi.org/project/types-aiobotocore-route53-recovery-readiness)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_route53_recovery_readiness/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-route53-recovery-readiness)](https://pepy.tech/project/types-aiobotocore-route53-recovery-readiness)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.Route53RecoveryReadiness 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53-recovery-readiness.html#Route53RecoveryReadiness)
+[aiobotocore.Route53RecoveryReadiness 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53-recovery-readiness.html#Route53RecoveryReadiness)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-route53-recovery-readiness-2.5.2.post2/setup.py` & `types-aiobotocore-route53-recovery-readiness-2.5.4/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-route53-recovery-readiness",
-    version="2.5.2.post2",
+    version="2.5.4",
     packages=["types_aiobotocore_route53_recovery_readiness"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.Route53RecoveryReadiness 2.5.2 service generated with"
+        "Type annotations for aiobotocore.Route53RecoveryReadiness 2.5.4 service generated with"
         " mypy-boto3-builder 7.17.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
```

### Comparing `types-aiobotocore-route53-recovery-readiness-2.5.2.post2/types_aiobotocore_route53_recovery_readiness/__init__.py` & `types-aiobotocore-route53-recovery-readiness-2.5.4/types_aiobotocore_route53_recovery_readiness/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-route53-recovery-readiness-2.5.2.post2/types_aiobotocore_route53_recovery_readiness/__init__.pyi` & `types-aiobotocore-route53-recovery-readiness-2.5.4/types_aiobotocore_route53_recovery_readiness/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-route53-recovery-readiness-2.5.2.post2/types_aiobotocore_route53_recovery_readiness/__main__.py` & `types-aiobotocore-route53-recovery-readiness-2.5.4/types_aiobotocore_route53_recovery_readiness/__main__.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.Route53RecoveryReadiness 2.5.2\nVersion:        "
-        " 2.5.2.post2\nBuilder version: 7.17.2\nDocs:           "
+        "Type annotations for aiobotocore.Route53RecoveryReadiness 2.5.4\nVersion:        "
+        " 2.5.4\nBuilder version: 7.17.2\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_route53_recovery_readiness//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53-recovery-readiness.html#Route53RecoveryReadiness\nOther"
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

### Comparing `types-aiobotocore-route53-recovery-readiness-2.5.2.post2/types_aiobotocore_route53_recovery_readiness/client.py` & `types-aiobotocore-route53-recovery-readiness-2.5.4/types_aiobotocore_route53_recovery_readiness/client.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-route53-recovery-readiness-2.5.2.post2/types_aiobotocore_route53_recovery_readiness/client.pyi` & `types-aiobotocore-route53-recovery-readiness-2.5.4/types_aiobotocore_route53_recovery_readiness/client.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-route53-recovery-readiness-2.5.2.post2/types_aiobotocore_route53_recovery_readiness/literals.py` & `types-aiobotocore-route53-recovery-readiness-2.5.4/types_aiobotocore_route53_recovery_readiness/literals.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-route53-recovery-readiness-2.5.2.post2/types_aiobotocore_route53_recovery_readiness/literals.pyi` & `types-aiobotocore-route53-recovery-readiness-2.5.4/types_aiobotocore_route53_recovery_readiness/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-route53-recovery-readiness-2.5.2.post2/types_aiobotocore_route53_recovery_readiness/paginator.py` & `types-aiobotocore-route53-recovery-readiness-2.5.4/types_aiobotocore_route53_recovery_readiness/paginator.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-route53-recovery-readiness-2.5.2.post2/types_aiobotocore_route53_recovery_readiness/paginator.pyi` & `types-aiobotocore-route53-recovery-readiness-2.5.4/types_aiobotocore_route53_recovery_readiness/paginator.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-route53-recovery-readiness-2.5.2.post2/types_aiobotocore_route53_recovery_readiness/type_defs.py` & `types-aiobotocore-route53-recovery-readiness-2.5.4/types_aiobotocore_route53_recovery_readiness/type_defs.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-route53-recovery-readiness-2.5.2.post2/types_aiobotocore_route53_recovery_readiness/type_defs.pyi` & `types-aiobotocore-route53-recovery-readiness-2.5.4/types_aiobotocore_route53_recovery_readiness/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-route53-recovery-readiness-2.5.2.post2/types_aiobotocore_route53_recovery_readiness.egg-info/PKG-INFO` & `types-aiobotocore-route53-recovery-readiness-2.5.4/types_aiobotocore_route53_recovery_readiness.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-route53-recovery-readiness
-Version: 2.5.2.post2
-Summary: Type annotations for aiobotocore.Route53RecoveryReadiness 2.5.2 service generated with mypy-boto3-builder 7.17.2
+Version: 2.5.4
+Summary: Type annotations for aiobotocore.Route53RecoveryReadiness 2.5.4 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_route53_recovery_readiness/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-route53-recovery-readiness.svg?color=blue)](https://pypi.org/project/types-aiobotocore-route53-recovery-readiness)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_route53_recovery_readiness/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-route53-recovery-readiness)](https://pepy.tech/project/types-aiobotocore-route53-recovery-readiness)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.Route53RecoveryReadiness 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53-recovery-readiness.html#Route53RecoveryReadiness)
+[aiobotocore.Route53RecoveryReadiness 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53-recovery-readiness.html#Route53RecoveryReadiness)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-route53-recovery-readiness-2.5.2.post2/types_aiobotocore_route53_recovery_readiness.egg-info/SOURCES.txt` & `types-aiobotocore-route53-recovery-readiness-2.5.4/types_aiobotocore_route53_recovery_readiness.egg-info/SOURCES.txt`

 * *Files identical despite different names*


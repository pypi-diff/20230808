# Comparing `tmp/types-aiobotocore-route53resolver-2.5.2.post2.tar.gz` & `tmp/types-aiobotocore-route53resolver-2.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-route53resolver-2.5.2.post2.tar", last modified: Fri Aug  4 13:59:23 2023, max compression
+gzip compressed data, was "types-aiobotocore-route53resolver-2.5.4.tar", last modified: Tue Aug  8 01:24:20 2023, max compression
```

## Comparing `types-aiobotocore-route53resolver-2.5.2.post2.tar` & `types-aiobotocore-route53resolver-2.5.4.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:23.956643 types-aiobotocore-route53resolver-2.5.2.post2/
--rw-r--r--   0 vlad      (1000) vlad      (1000)     1070 2023-08-04 13:51:19.000000 types-aiobotocore-route53resolver-2.5.2.post2/LICENSE
--rw-r--r--   0 vlad      (1000) vlad      (1000)    16142 2023-08-04 13:59:23.956643 types-aiobotocore-route53resolver-2.5.2.post2/PKG-INFO
--rw-r--r--   0 vlad      (1000) vlad      (1000)    14592 2023-08-04 13:51:19.000000 types-aiobotocore-route53resolver-2.5.2.post2/README.md
--rw-r--r--   0 vlad      (1000) vlad      (1000)       38 2023-08-04 13:59:23.956643 types-aiobotocore-route53resolver-2.5.2.post2/setup.cfg
--rw-r--r--   0 vlad      (1000) vlad      (1000)     2128 2023-08-04 13:51:19.000000 types-aiobotocore-route53resolver-2.5.2.post2/setup.py
-drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:23.956643 types-aiobotocore-route53resolver-2.5.2.post2/types_aiobotocore_route53resolver/
--rw-r--r--   0 vlad      (1000) vlad      (1000)     4569 2023-08-04 13:51:19.000000 types-aiobotocore-route53resolver-2.5.2.post2/types_aiobotocore_route53resolver/__init__.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)     4568 2023-08-04 13:51:19.000000 types-aiobotocore-route53resolver-2.5.2.post2/types_aiobotocore_route53resolver/__init__.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)      975 2023-08-04 13:51:19.000000 types-aiobotocore-route53resolver-2.5.2.post2/types_aiobotocore_route53resolver/__main__.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)    62209 2023-08-04 13:51:19.000000 types-aiobotocore-route53resolver-2.5.2.post2/types_aiobotocore_route53resolver/client.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)    62116 2023-08-04 13:51:19.000000 types-aiobotocore-route53resolver-2.5.2.post2/types_aiobotocore_route53resolver/client.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)    14396 2023-08-04 13:51:20.000000 types-aiobotocore-route53resolver-2.5.2.post2/types_aiobotocore_route53resolver/literals.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)    14394 2023-08-04 13:51:20.000000 types-aiobotocore-route53resolver-2.5.2.post2/types_aiobotocore_route53resolver/literals.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)    21614 2023-08-04 13:51:20.000000 types-aiobotocore-route53resolver-2.5.2.post2/types_aiobotocore_route53resolver/paginator.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)    21596 2023-08-04 13:51:19.000000 types-aiobotocore-route53resolver-2.5.2.post2/types_aiobotocore_route53resolver/paginator.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:51:19.000000 types-aiobotocore-route53resolver-2.5.2.post2/types_aiobotocore_route53resolver/py.typed
--rw-r--r--   0 vlad      (1000) vlad      (1000)    61169 2023-08-04 13:51:21.000000 types-aiobotocore-route53resolver-2.5.2.post2/types_aiobotocore_route53resolver/type_defs.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)    61124 2023-08-04 13:51:21.000000 types-aiobotocore-route53resolver-2.5.2.post2/types_aiobotocore_route53resolver/type_defs.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)       65 2023-08-04 13:51:19.000000 types-aiobotocore-route53resolver-2.5.2.post2/types_aiobotocore_route53resolver/version.py
-drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:23.956643 types-aiobotocore-route53resolver-2.5.2.post2/types_aiobotocore_route53resolver.egg-info/
--rw-r--r--   0 vlad      (1000) vlad      (1000)    16142 2023-08-04 13:59:23.000000 types-aiobotocore-route53resolver-2.5.2.post2/types_aiobotocore_route53resolver.egg-info/PKG-INFO
--rw-r--r--   0 vlad      (1000) vlad      (1000)      965 2023-08-04 13:59:23.000000 types-aiobotocore-route53resolver-2.5.2.post2/types_aiobotocore_route53resolver.egg-info/SOURCES.txt
--rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:23.000000 types-aiobotocore-route53resolver-2.5.2.post2/types_aiobotocore_route53resolver.egg-info/dependency_links.txt
--rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:23.000000 types-aiobotocore-route53resolver-2.5.2.post2/types_aiobotocore_route53resolver.egg-info/not-zip-safe
--rw-r--r--   0 vlad      (1000) vlad      (1000)       52 2023-08-04 13:59:23.000000 types-aiobotocore-route53resolver-2.5.2.post2/types_aiobotocore_route53resolver.egg-info/requires.txt
--rw-r--r--   0 vlad      (1000) vlad      (1000)       34 2023-08-04 13:59:23.000000 types-aiobotocore-route53resolver-2.5.2.post2/types_aiobotocore_route53resolver.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:24:20.826767 types-aiobotocore-route53resolver-2.5.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-08 01:19:43.000000 types-aiobotocore-route53resolver-2.5.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    16136 2023-08-08 01:24:20.826767 types-aiobotocore-route53resolver-2.5.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    14592 2023-08-08 01:19:43.000000 types-aiobotocore-route53resolver-2.5.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-08 01:24:20.826767 types-aiobotocore-route53resolver-2.5.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2122 2023-08-08 01:19:42.000000 types-aiobotocore-route53resolver-2.5.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:24:20.818767 types-aiobotocore-route53resolver-2.5.4/types_aiobotocore_route53resolver/
+-rw-r--r--   0 runner    (1001) docker     (123)     4569 2023-08-08 01:19:43.000000 types-aiobotocore-route53resolver-2.5.4/types_aiobotocore_route53resolver/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4568 2023-08-08 01:19:43.000000 types-aiobotocore-route53resolver-2.5.4/types_aiobotocore_route53resolver/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      963 2023-08-08 01:19:43.000000 types-aiobotocore-route53resolver-2.5.4/types_aiobotocore_route53resolver/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    62209 2023-08-08 01:19:43.000000 types-aiobotocore-route53resolver-2.5.4/types_aiobotocore_route53resolver/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    62116 2023-08-08 01:19:43.000000 types-aiobotocore-route53resolver-2.5.4/types_aiobotocore_route53resolver/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    14396 2023-08-08 01:19:43.000000 types-aiobotocore-route53resolver-2.5.4/types_aiobotocore_route53resolver/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14394 2023-08-08 01:19:43.000000 types-aiobotocore-route53resolver-2.5.4/types_aiobotocore_route53resolver/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    21614 2023-08-08 01:19:43.000000 types-aiobotocore-route53resolver-2.5.4/types_aiobotocore_route53resolver/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21596 2023-08-08 01:19:43.000000 types-aiobotocore-route53resolver-2.5.4/types_aiobotocore_route53resolver/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 01:19:43.000000 types-aiobotocore-route53resolver-2.5.4/types_aiobotocore_route53resolver/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    61169 2023-08-08 01:19:44.000000 types-aiobotocore-route53resolver-2.5.4/types_aiobotocore_route53resolver/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    61124 2023-08-08 01:19:44.000000 types-aiobotocore-route53resolver-2.5.4/types_aiobotocore_route53resolver/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-08-08 01:19:43.000000 types-aiobotocore-route53resolver-2.5.4/types_aiobotocore_route53resolver/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:24:20.826767 types-aiobotocore-route53resolver-2.5.4/types_aiobotocore_route53resolver.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    16136 2023-08-08 01:24:20.000000 types-aiobotocore-route53resolver-2.5.4/types_aiobotocore_route53resolver.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      965 2023-08-08 01:24:20.000000 types-aiobotocore-route53resolver-2.5.4/types_aiobotocore_route53resolver.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 01:24:20.000000 types-aiobotocore-route53resolver-2.5.4/types_aiobotocore_route53resolver.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 01:24:20.000000 types-aiobotocore-route53resolver-2.5.4/types_aiobotocore_route53resolver.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-08 01:24:20.000000 types-aiobotocore-route53resolver-2.5.4/types_aiobotocore_route53resolver.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-08-08 01:24:20.000000 types-aiobotocore-route53resolver-2.5.4/types_aiobotocore_route53resolver.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-route53resolver-2.5.2.post2/LICENSE` & `types-aiobotocore-route53resolver-2.5.4/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-route53resolver-2.5.2.post2/PKG-INFO` & `types-aiobotocore-route53resolver-2.5.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-route53resolver
-Version: 2.5.2.post2
-Summary: Type annotations for aiobotocore.Route53Resolver 2.5.2 service generated with mypy-boto3-builder 7.17.2
+Version: 2.5.4
+Summary: Type annotations for aiobotocore.Route53Resolver 2.5.4 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_route53resolver/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-route53resolver.svg?color=blue)](https://pypi.org/project/types-aiobotocore-route53resolver)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_route53resolver/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-route53resolver)](https://pepy.tech/project/types-aiobotocore-route53resolver)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.Route53Resolver 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53resolver.html#Route53Resolver)
+[aiobotocore.Route53Resolver 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53resolver.html#Route53Resolver)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-route53resolver-2.5.2.post2/README.md` & `types-aiobotocore-route53resolver-2.5.4/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-route53resolver.svg?color=blue)](https://pypi.org/project/types-aiobotocore-route53resolver)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_route53resolver/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-route53resolver)](https://pepy.tech/project/types-aiobotocore-route53resolver)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.Route53Resolver 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53resolver.html#Route53Resolver)
+[aiobotocore.Route53Resolver 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53resolver.html#Route53Resolver)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-route53resolver-2.5.2.post2/setup.py` & `types-aiobotocore-route53resolver-2.5.4/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-route53resolver",
-    version="2.5.2.post2",
+    version="2.5.4",
     packages=["types_aiobotocore_route53resolver"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.Route53Resolver 2.5.2 service generated with"
+        "Type annotations for aiobotocore.Route53Resolver 2.5.4 service generated with"
         " mypy-boto3-builder 7.17.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
```

### Comparing `types-aiobotocore-route53resolver-2.5.2.post2/types_aiobotocore_route53resolver/__init__.py` & `types-aiobotocore-route53resolver-2.5.4/types_aiobotocore_route53resolver/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-route53resolver-2.5.2.post2/types_aiobotocore_route53resolver/__init__.pyi` & `types-aiobotocore-route53resolver-2.5.4/types_aiobotocore_route53resolver/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-route53resolver-2.5.2.post2/types_aiobotocore_route53resolver/__main__.py` & `types-aiobotocore-route53resolver-2.5.4/types_aiobotocore_route53resolver/__main__.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.Route53Resolver 2.5.2\nVersion:        "
-        " 2.5.2.post2\nBuilder version: 7.17.2\nDocs:           "
+        "Type annotations for aiobotocore.Route53Resolver 2.5.4\nVersion:         2.5.4\nBuilder"
+        " version: 7.17.2\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_route53resolver//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53resolver.html#Route53Resolver\nOther"
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

### Comparing `types-aiobotocore-route53resolver-2.5.2.post2/types_aiobotocore_route53resolver/client.py` & `types-aiobotocore-route53resolver-2.5.4/types_aiobotocore_route53resolver/client.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-route53resolver-2.5.2.post2/types_aiobotocore_route53resolver/client.pyi` & `types-aiobotocore-route53resolver-2.5.4/types_aiobotocore_route53resolver/client.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-route53resolver-2.5.2.post2/types_aiobotocore_route53resolver/literals.py` & `types-aiobotocore-route53resolver-2.5.4/types_aiobotocore_route53resolver/literals.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-route53resolver-2.5.2.post2/types_aiobotocore_route53resolver/literals.pyi` & `types-aiobotocore-route53resolver-2.5.4/types_aiobotocore_route53resolver/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-route53resolver-2.5.2.post2/types_aiobotocore_route53resolver/paginator.py` & `types-aiobotocore-route53resolver-2.5.4/types_aiobotocore_route53resolver/paginator.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-route53resolver-2.5.2.post2/types_aiobotocore_route53resolver/paginator.pyi` & `types-aiobotocore-route53resolver-2.5.4/types_aiobotocore_route53resolver/paginator.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-route53resolver-2.5.2.post2/types_aiobotocore_route53resolver/type_defs.py` & `types-aiobotocore-route53resolver-2.5.4/types_aiobotocore_route53resolver/type_defs.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-route53resolver-2.5.2.post2/types_aiobotocore_route53resolver/type_defs.pyi` & `types-aiobotocore-route53resolver-2.5.4/types_aiobotocore_route53resolver/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-route53resolver-2.5.2.post2/types_aiobotocore_route53resolver.egg-info/PKG-INFO` & `types-aiobotocore-route53resolver-2.5.4/types_aiobotocore_route53resolver.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-route53resolver
-Version: 2.5.2.post2
-Summary: Type annotations for aiobotocore.Route53Resolver 2.5.2 service generated with mypy-boto3-builder 7.17.2
+Version: 2.5.4
+Summary: Type annotations for aiobotocore.Route53Resolver 2.5.4 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_route53resolver/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-route53resolver.svg?color=blue)](https://pypi.org/project/types-aiobotocore-route53resolver)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_route53resolver/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-route53resolver)](https://pepy.tech/project/types-aiobotocore-route53resolver)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.Route53Resolver 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53resolver.html#Route53Resolver)
+[aiobotocore.Route53Resolver 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53resolver.html#Route53Resolver)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-route53resolver-2.5.2.post2/types_aiobotocore_route53resolver.egg-info/SOURCES.txt` & `types-aiobotocore-route53resolver-2.5.4/types_aiobotocore_route53resolver.egg-info/SOURCES.txt`

 * *Files identical despite different names*


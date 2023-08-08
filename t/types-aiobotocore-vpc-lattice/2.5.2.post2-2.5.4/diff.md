# Comparing `tmp/types-aiobotocore-vpc-lattice-2.5.2.post2.tar.gz` & `tmp/types-aiobotocore-vpc-lattice-2.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-vpc-lattice-2.5.2.post2.tar", last modified: Fri Aug  4 13:59:29 2023, max compression
+gzip compressed data, was "types-aiobotocore-vpc-lattice-2.5.4.tar", last modified: Tue Aug  8 01:24:34 2023, max compression
```

## Comparing `types-aiobotocore-vpc-lattice-2.5.2.post2.tar` & `types-aiobotocore-vpc-lattice-2.5.4.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:29.446643 types-aiobotocore-vpc-lattice-2.5.2.post2/
--rw-r--r--   0 vlad      (1000) vlad      (1000)     1070 2023-08-04 13:55:31.000000 types-aiobotocore-vpc-lattice-2.5.2.post2/LICENSE
--rw-r--r--   0 vlad      (1000) vlad      (1000)    14465 2023-08-04 13:59:29.446643 types-aiobotocore-vpc-lattice-2.5.2.post2/PKG-INFO
--rw-r--r--   0 vlad      (1000) vlad      (1000)    12932 2023-08-04 13:55:31.000000 types-aiobotocore-vpc-lattice-2.5.2.post2/README.md
--rw-r--r--   0 vlad      (1000) vlad      (1000)       38 2023-08-04 13:59:29.446643 types-aiobotocore-vpc-lattice-2.5.2.post2/setup.cfg
--rw-r--r--   0 vlad      (1000) vlad      (1000)     2099 2023-08-04 13:55:31.000000 types-aiobotocore-vpc-lattice-2.5.2.post2/setup.py
-drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:29.446643 types-aiobotocore-vpc-lattice-2.5.2.post2/types_aiobotocore_vpc_lattice/
--rw-r--r--   0 vlad      (1000) vlad      (1000)     2538 2023-08-04 13:55:31.000000 types-aiobotocore-vpc-lattice-2.5.2.post2/types_aiobotocore_vpc_lattice/__init__.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)     2537 2023-08-04 13:55:31.000000 types-aiobotocore-vpc-lattice-2.5.2.post2/types_aiobotocore_vpc_lattice/__init__.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)      957 2023-08-04 13:55:31.000000 types-aiobotocore-vpc-lattice-2.5.2.post2/types_aiobotocore_vpc_lattice/__main__.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)    41317 2023-08-04 13:55:32.000000 types-aiobotocore-vpc-lattice-2.5.2.post2/types_aiobotocore_vpc_lattice/client.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)    41247 2023-08-04 13:55:32.000000 types-aiobotocore-vpc-lattice-2.5.2.post2/types_aiobotocore_vpc_lattice/client.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)    10660 2023-08-04 13:55:32.000000 types-aiobotocore-vpc-lattice-2.5.2.post2/types_aiobotocore_vpc_lattice/literals.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)    10658 2023-08-04 13:55:32.000000 types-aiobotocore-vpc-lattice-2.5.2.post2/types_aiobotocore_vpc_lattice/literals.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)    11903 2023-08-04 13:55:32.000000 types-aiobotocore-vpc-lattice-2.5.2.post2/types_aiobotocore_vpc_lattice/paginator.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)    11892 2023-08-04 13:55:32.000000 types-aiobotocore-vpc-lattice-2.5.2.post2/types_aiobotocore_vpc_lattice/paginator.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:55:31.000000 types-aiobotocore-vpc-lattice-2.5.2.post2/types_aiobotocore_vpc_lattice/py.typed
--rw-r--r--   0 vlad      (1000) vlad      (1000)    48595 2023-08-04 13:55:33.000000 types-aiobotocore-vpc-lattice-2.5.2.post2/types_aiobotocore_vpc_lattice/type_defs.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)    48546 2023-08-04 13:55:33.000000 types-aiobotocore-vpc-lattice-2.5.2.post2/types_aiobotocore_vpc_lattice/type_defs.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)       65 2023-08-04 13:55:31.000000 types-aiobotocore-vpc-lattice-2.5.2.post2/types_aiobotocore_vpc_lattice/version.py
-drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:29.446643 types-aiobotocore-vpc-lattice-2.5.2.post2/types_aiobotocore_vpc_lattice.egg-info/
--rw-r--r--   0 vlad      (1000) vlad      (1000)    14465 2023-08-04 13:59:29.000000 types-aiobotocore-vpc-lattice-2.5.2.post2/types_aiobotocore_vpc_lattice.egg-info/PKG-INFO
--rw-r--r--   0 vlad      (1000) vlad      (1000)      889 2023-08-04 13:59:29.000000 types-aiobotocore-vpc-lattice-2.5.2.post2/types_aiobotocore_vpc_lattice.egg-info/SOURCES.txt
--rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:29.000000 types-aiobotocore-vpc-lattice-2.5.2.post2/types_aiobotocore_vpc_lattice.egg-info/dependency_links.txt
--rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:29.000000 types-aiobotocore-vpc-lattice-2.5.2.post2/types_aiobotocore_vpc_lattice.egg-info/not-zip-safe
--rw-r--r--   0 vlad      (1000) vlad      (1000)       52 2023-08-04 13:59:29.000000 types-aiobotocore-vpc-lattice-2.5.2.post2/types_aiobotocore_vpc_lattice.egg-info/requires.txt
--rw-r--r--   0 vlad      (1000) vlad      (1000)       30 2023-08-04 13:59:29.000000 types-aiobotocore-vpc-lattice-2.5.2.post2/types_aiobotocore_vpc_lattice.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:24:34.606800 types-aiobotocore-vpc-lattice-2.5.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-08 01:22:14.000000 types-aiobotocore-vpc-lattice-2.5.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    14459 2023-08-08 01:24:34.598801 types-aiobotocore-vpc-lattice-2.5.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    12932 2023-08-08 01:22:14.000000 types-aiobotocore-vpc-lattice-2.5.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-08 01:24:34.606800 types-aiobotocore-vpc-lattice-2.5.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2093 2023-08-08 01:22:14.000000 types-aiobotocore-vpc-lattice-2.5.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:24:34.598801 types-aiobotocore-vpc-lattice-2.5.4/types_aiobotocore_vpc_lattice/
+-rw-r--r--   0 runner    (1001) docker     (123)     2538 2023-08-08 01:22:14.000000 types-aiobotocore-vpc-lattice-2.5.4/types_aiobotocore_vpc_lattice/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2537 2023-08-08 01:22:14.000000 types-aiobotocore-vpc-lattice-2.5.4/types_aiobotocore_vpc_lattice/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      945 2023-08-08 01:22:14.000000 types-aiobotocore-vpc-lattice-2.5.4/types_aiobotocore_vpc_lattice/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41317 2023-08-08 01:22:14.000000 types-aiobotocore-vpc-lattice-2.5.4/types_aiobotocore_vpc_lattice/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41247 2023-08-08 01:22:14.000000 types-aiobotocore-vpc-lattice-2.5.4/types_aiobotocore_vpc_lattice/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    10660 2023-08-08 01:22:15.000000 types-aiobotocore-vpc-lattice-2.5.4/types_aiobotocore_vpc_lattice/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10658 2023-08-08 01:22:14.000000 types-aiobotocore-vpc-lattice-2.5.4/types_aiobotocore_vpc_lattice/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    11903 2023-08-08 01:22:14.000000 types-aiobotocore-vpc-lattice-2.5.4/types_aiobotocore_vpc_lattice/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11892 2023-08-08 01:22:14.000000 types-aiobotocore-vpc-lattice-2.5.4/types_aiobotocore_vpc_lattice/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 01:22:14.000000 types-aiobotocore-vpc-lattice-2.5.4/types_aiobotocore_vpc_lattice/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    48595 2023-08-08 01:22:19.000000 types-aiobotocore-vpc-lattice-2.5.4/types_aiobotocore_vpc_lattice/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    48546 2023-08-08 01:22:15.000000 types-aiobotocore-vpc-lattice-2.5.4/types_aiobotocore_vpc_lattice/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-08-08 01:22:14.000000 types-aiobotocore-vpc-lattice-2.5.4/types_aiobotocore_vpc_lattice/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:24:34.598801 types-aiobotocore-vpc-lattice-2.5.4/types_aiobotocore_vpc_lattice.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    14459 2023-08-08 01:24:34.000000 types-aiobotocore-vpc-lattice-2.5.4/types_aiobotocore_vpc_lattice.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      889 2023-08-08 01:24:34.000000 types-aiobotocore-vpc-lattice-2.5.4/types_aiobotocore_vpc_lattice.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 01:24:34.000000 types-aiobotocore-vpc-lattice-2.5.4/types_aiobotocore_vpc_lattice.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 01:24:34.000000 types-aiobotocore-vpc-lattice-2.5.4/types_aiobotocore_vpc_lattice.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-08 01:24:34.000000 types-aiobotocore-vpc-lattice-2.5.4/types_aiobotocore_vpc_lattice.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-08-08 01:24:34.000000 types-aiobotocore-vpc-lattice-2.5.4/types_aiobotocore_vpc_lattice.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-vpc-lattice-2.5.2.post2/LICENSE` & `types-aiobotocore-vpc-lattice-2.5.4/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-vpc-lattice-2.5.2.post2/PKG-INFO` & `types-aiobotocore-vpc-lattice-2.5.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-vpc-lattice
-Version: 2.5.2.post2
-Summary: Type annotations for aiobotocore.VPCLattice 2.5.2 service generated with mypy-boto3-builder 7.17.2
+Version: 2.5.4
+Summary: Type annotations for aiobotocore.VPCLattice 2.5.4 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_vpc_lattice/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-vpc-lattice.svg?color=blue)](https://pypi.org/project/types-aiobotocore-vpc-lattice)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_vpc_lattice/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-vpc-lattice)](https://pepy.tech/project/types-aiobotocore-vpc-lattice)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.VPCLattice 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/vpc-lattice.html#VPCLattice)
+[aiobotocore.VPCLattice 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/vpc-lattice.html#VPCLattice)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-vpc-lattice-2.5.2.post2/README.md` & `types-aiobotocore-vpc-lattice-2.5.4/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-vpc-lattice.svg?color=blue)](https://pypi.org/project/types-aiobotocore-vpc-lattice)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_vpc_lattice/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-vpc-lattice)](https://pepy.tech/project/types-aiobotocore-vpc-lattice)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.VPCLattice 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/vpc-lattice.html#VPCLattice)
+[aiobotocore.VPCLattice 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/vpc-lattice.html#VPCLattice)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-vpc-lattice-2.5.2.post2/setup.py` & `types-aiobotocore-vpc-lattice-2.5.4/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-vpc-lattice",
-    version="2.5.2.post2",
+    version="2.5.4",
     packages=["types_aiobotocore_vpc_lattice"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.VPCLattice 2.5.2 service generated with"
+        "Type annotations for aiobotocore.VPCLattice 2.5.4 service generated with"
         " mypy-boto3-builder 7.17.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
```

### Comparing `types-aiobotocore-vpc-lattice-2.5.2.post2/types_aiobotocore_vpc_lattice/__init__.py` & `types-aiobotocore-vpc-lattice-2.5.4/types_aiobotocore_vpc_lattice/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-vpc-lattice-2.5.2.post2/types_aiobotocore_vpc_lattice/__init__.pyi` & `types-aiobotocore-vpc-lattice-2.5.4/types_aiobotocore_vpc_lattice/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-vpc-lattice-2.5.2.post2/types_aiobotocore_vpc_lattice/__main__.py` & `types-aiobotocore-vpc-lattice-2.5.4/types_aiobotocore_vpc_lattice/__main__.py`

 * *Files 22% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.VPCLattice 2.5.2\nVersion:         2.5.2.post2\nBuilder"
+        "Type annotations for aiobotocore.VPCLattice 2.5.4\nVersion:         2.5.4\nBuilder"
         " version: 7.17.2\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_vpc_lattice//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/vpc-lattice.html#VPCLattice\nOther"
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

### Comparing `types-aiobotocore-vpc-lattice-2.5.2.post2/types_aiobotocore_vpc_lattice/client.py` & `types-aiobotocore-vpc-lattice-2.5.4/types_aiobotocore_vpc_lattice/client.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-vpc-lattice-2.5.2.post2/types_aiobotocore_vpc_lattice/client.pyi` & `types-aiobotocore-vpc-lattice-2.5.4/types_aiobotocore_vpc_lattice/client.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-vpc-lattice-2.5.2.post2/types_aiobotocore_vpc_lattice/literals.py` & `types-aiobotocore-vpc-lattice-2.5.4/types_aiobotocore_vpc_lattice/literals.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-vpc-lattice-2.5.2.post2/types_aiobotocore_vpc_lattice/literals.pyi` & `types-aiobotocore-vpc-lattice-2.5.4/types_aiobotocore_vpc_lattice/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-vpc-lattice-2.5.2.post2/types_aiobotocore_vpc_lattice/paginator.py` & `types-aiobotocore-vpc-lattice-2.5.4/types_aiobotocore_vpc_lattice/paginator.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-vpc-lattice-2.5.2.post2/types_aiobotocore_vpc_lattice/paginator.pyi` & `types-aiobotocore-vpc-lattice-2.5.4/types_aiobotocore_vpc_lattice/paginator.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-vpc-lattice-2.5.2.post2/types_aiobotocore_vpc_lattice/type_defs.py` & `types-aiobotocore-vpc-lattice-2.5.4/types_aiobotocore_vpc_lattice/type_defs.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-vpc-lattice-2.5.2.post2/types_aiobotocore_vpc_lattice/type_defs.pyi` & `types-aiobotocore-vpc-lattice-2.5.4/types_aiobotocore_vpc_lattice/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-vpc-lattice-2.5.2.post2/types_aiobotocore_vpc_lattice.egg-info/PKG-INFO` & `types-aiobotocore-vpc-lattice-2.5.4/types_aiobotocore_vpc_lattice.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-vpc-lattice
-Version: 2.5.2.post2
-Summary: Type annotations for aiobotocore.VPCLattice 2.5.2 service generated with mypy-boto3-builder 7.17.2
+Version: 2.5.4
+Summary: Type annotations for aiobotocore.VPCLattice 2.5.4 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_vpc_lattice/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-vpc-lattice.svg?color=blue)](https://pypi.org/project/types-aiobotocore-vpc-lattice)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_vpc_lattice/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-vpc-lattice)](https://pepy.tech/project/types-aiobotocore-vpc-lattice)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.VPCLattice 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/vpc-lattice.html#VPCLattice)
+[aiobotocore.VPCLattice 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/vpc-lattice.html#VPCLattice)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-vpc-lattice-2.5.2.post2/types_aiobotocore_vpc_lattice.egg-info/SOURCES.txt` & `types-aiobotocore-vpc-lattice-2.5.4/types_aiobotocore_vpc_lattice.egg-info/SOURCES.txt`

 * *Files identical despite different names*


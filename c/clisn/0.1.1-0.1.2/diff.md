# Comparing `tmp/clisn-0.1.1.tar.gz` & `tmp/clisn-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "clisn-0.1.1.tar", max compression
+gzip compressed data, was "clisn-0.1.2.tar", max compression
```

## Comparing `clisn-0.1.1.tar` & `clisn-0.1.2.tar`

### file list

```diff
@@ -1,6 +1,7 @@
--rw-r--r--   0        0        0    35149 2023-08-07 07:22:06.852172 clisn-0.1.1/LICENSE
--rw-r--r--   0        0        0     2213 2023-08-08 13:11:40.424029 clisn-0.1.1/README.md
--rw-r--r--   0        0        0       91 2023-08-07 08:43:54.138618 clisn-0.1.1/clisn/__init__.py
--rw-r--r--   0        0        0     1691 2023-08-08 12:45:28.926269 clisn-0.1.1/clisn/clisn.py
--rw-r--r--   0        0        0      275 2023-08-08 13:14:15.831156 clisn-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     2528 1970-01-01 00:00:00.000000 clisn-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-08-07 07:22:06.852172 clisn-0.1.2/LICENSE
+-rw-r--r--   0        0        0     2299 2023-08-08 13:25:23.839896 clisn-0.1.2/README.md
+-rw-r--r--   0        0        0       82 2023-08-08 15:01:04.465348 clisn-0.1.2/clisn/__init__.py
+-rw-r--r--   0        0        0      948 2023-08-08 14:59:45.635093 clisn-0.1.2/clisn/manager.py
+-rw-r--r--   0        0        0      850 2023-08-08 15:00:35.728588 clisn-0.1.2/clisn/namespaces.py
+-rw-r--r--   0        0        0      275 2023-08-08 15:02:24.168940 clisn-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     2614 1970-01-01 00:00:00.000000 clisn-0.1.2/PKG-INFO
```

### Comparing `clisn-0.1.1/LICENSE` & `clisn-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `clisn-0.1.1/README.md` & `clisn-0.1.2/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 # CLiSN <:books:>:sparkles:
 [![License: GPL v3](https://img.shields.io/badge/License-GPLv3-blue.svg)](https://www.gnu.org/licenses/gpl-3.0)
+[![PyPI version](https://badge.fury.io/py/clisn.svg)](https://badge.fury.io/py/clisn)
 
 A collection of [RDFLib](https://rdflib.readthedocs.io/en/stable/) namespaces for the [Computational Literary Studies Infrastructure](https://clsinfra.io/) project.
 
 ## Requirements
 * Python >=3.11
 
 ## Installation
```

### Comparing `clisn-0.1.1/PKG-INFO` & `clisn-0.1.2/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 Metadata-Version: 2.1
 Name: clisn
-Version: 0.1.1
+Version: 0.1.2
 Summary: 
 Author: Lukas Plank
 Author-email: lupl@tuta.io
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: rdflib (>=7.0.0,<8.0.0)
 Description-Content-Type: text/markdown
 
 # CLiSN <:books:>:sparkles:
 [![License: GPL v3](https://img.shields.io/badge/License-GPLv3-blue.svg)](https://www.gnu.org/licenses/gpl-3.0)
+[![PyPI version](https://badge.fury.io/py/clisn.svg)](https://badge.fury.io/py/clisn)
 
 A collection of [RDFLib](https://rdflib.readthedocs.io/en/stable/) namespaces for the [Computational Literary Studies Infrastructure](https://clsinfra.io/) project.
 
 ## Requirements
 * Python >=3.11
 
 ## Installation
```


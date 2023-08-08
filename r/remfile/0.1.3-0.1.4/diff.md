# Comparing `tmp/remfile-0.1.3.tar.gz` & `tmp/remfile-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "remfile-0.1.3.tar", last modified: Tue Aug  8 15:48:20 2023, max compression
+gzip compressed data, was "remfile-0.1.4.tar", last modified: Tue Aug  8 16:38:55 2023, max compression
```

## Comparing `remfile-0.1.3.tar` & `remfile-0.1.4.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxr-x   0 magland   (1000) magland   (1000)        0 2023-08-08 15:48:20.202309 remfile-0.1.3/
--rw-rw-r--   0 magland   (1000) magland   (1000)    11357 2023-08-07 12:41:38.000000 remfile-0.1.3/LICENSE
--rw-rw-r--   0 magland   (1000) magland   (1000)    15545 2023-08-08 15:48:20.202309 remfile-0.1.3/PKG-INFO
--rw-r--r--   0 magland   (1000) magland   (1000)     2031 2023-08-08 15:41:35.000000 remfile-0.1.3/README.md
--rw-r--r--   0 magland   (1000) magland   (1000)      977 2023-08-08 15:10:05.000000 remfile-0.1.3/pyproject.toml
-drwxrwxr-x   0 magland   (1000) magland   (1000)        0 2023-08-08 15:48:20.202309 remfile-0.1.3/remfile/
--rw-r--r--   0 magland   (1000) magland   (1000)    10197 2023-08-08 15:46:29.000000 remfile-0.1.3/remfile/RemFile.py
--rw-r--r--   0 magland   (1000) magland   (1000)       59 2023-08-08 15:47:01.000000 remfile-0.1.3/remfile/__init__.py
-drwxrwxr-x   0 magland   (1000) magland   (1000)        0 2023-08-08 15:48:20.202309 remfile-0.1.3/remfile.egg-info/
--rw-r--r--   0 magland   (1000) magland   (1000)    15545 2023-08-08 15:48:20.000000 remfile-0.1.3/remfile.egg-info/PKG-INFO
--rw-r--r--   0 magland   (1000) magland   (1000)      244 2023-08-08 15:48:20.000000 remfile-0.1.3/remfile.egg-info/SOURCES.txt
--rw-r--r--   0 magland   (1000) magland   (1000)        1 2023-08-08 15:48:20.000000 remfile-0.1.3/remfile.egg-info/dependency_links.txt
--rw-r--r--   0 magland   (1000) magland   (1000)       40 2023-08-08 15:48:20.000000 remfile-0.1.3/remfile.egg-info/requires.txt
--rw-r--r--   0 magland   (1000) magland   (1000)        8 2023-08-08 15:48:20.000000 remfile-0.1.3/remfile.egg-info/top_level.txt
--rw-rw-r--   0 magland   (1000) magland   (1000)       38 2023-08-08 15:48:20.202309 remfile-0.1.3/setup.cfg
-drwxrwxr-x   0 magland   (1000) magland   (1000)        0 2023-08-08 15:48:20.202309 remfile-0.1.3/tests/
--rw-rw-r--   0 magland   (1000) magland   (1000)     1673 2023-08-08 15:43:09.000000 remfile-0.1.3/tests/test_main.py
+drwxrwxr-x   0 magland   (1000) magland   (1000)        0 2023-08-08 16:38:55.663624 remfile-0.1.4/
+-rw-rw-r--   0 magland   (1000) magland   (1000)    11357 2023-08-07 12:41:38.000000 remfile-0.1.4/LICENSE
+-rw-rw-r--   0 magland   (1000) magland   (1000)     2340 2023-08-08 16:38:55.663624 remfile-0.1.4/PKG-INFO
+-rw-r--r--   0 magland   (1000) magland   (1000)     2032 2023-08-08 15:51:03.000000 remfile-0.1.4/README.md
+drwxrwxr-x   0 magland   (1000) magland   (1000)        0 2023-08-08 16:38:55.663624 remfile-0.1.4/remfile/
+-rw-r--r--   0 magland   (1000) magland   (1000)    10197 2023-08-08 15:46:29.000000 remfile-0.1.4/remfile/RemFile.py
+-rw-r--r--   0 magland   (1000) magland   (1000)      115 2023-08-08 16:35:22.000000 remfile-0.1.4/remfile/__init__.py
+drwxrwxr-x   0 magland   (1000) magland   (1000)        0 2023-08-08 16:38:55.663624 remfile-0.1.4/remfile.egg-info/
+-rw-r--r--   0 magland   (1000) magland   (1000)     2340 2023-08-08 16:38:55.000000 remfile-0.1.4/remfile.egg-info/PKG-INFO
+-rw-r--r--   0 magland   (1000) magland   (1000)      238 2023-08-08 16:38:55.000000 remfile-0.1.4/remfile.egg-info/SOURCES.txt
+-rw-r--r--   0 magland   (1000) magland   (1000)        1 2023-08-08 16:38:55.000000 remfile-0.1.4/remfile.egg-info/dependency_links.txt
+-rw-r--r--   0 magland   (1000) magland   (1000)       20 2023-08-08 16:38:55.000000 remfile-0.1.4/remfile.egg-info/requires.txt
+-rw-r--r--   0 magland   (1000) magland   (1000)        8 2023-08-08 16:38:55.000000 remfile-0.1.4/remfile.egg-info/top_level.txt
+-rw-rw-r--   0 magland   (1000) magland   (1000)       38 2023-08-08 16:38:55.663624 remfile-0.1.4/setup.cfg
+-rw-rw-r--   0 magland   (1000) magland   (1000)      764 2023-08-08 16:35:39.000000 remfile-0.1.4/setup.py
+drwxrwxr-x   0 magland   (1000) magland   (1000)        0 2023-08-08 16:38:55.663624 remfile-0.1.4/tests/
+-rw-rw-r--   0 magland   (1000) magland   (1000)     1673 2023-08-08 15:43:09.000000 remfile-0.1.4/tests/test_main.py
```

### Comparing `remfile-0.1.3/LICENSE` & `remfile-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `remfile-0.1.3/README.md` & `remfile-0.1.4/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 # remfile
 
 [![latest-release](https://img.shields.io/pypi/v/remfile.svg)](https://pypi.org/project/remfile)
 ![tests](https://github.com/magland/remfile/actions/workflows/tests.yml/badge.svg)
 [![codecov](https://codecov.io/gh/magland/remfile/branch/main/graph/badge.svg)](https://codecov.io/gh/magland/remfile)
 
+
 Provides a file-like object for reading a remote file over HTTP, optimized for use with h5py.
 
 Example usage:
 
 ```python
 # See examples/example1.py
```

### Comparing `remfile-0.1.3/remfile/RemFile.py` & `remfile-0.1.4/remfile/RemFile.py`

 * *Files identical despite different names*

### Comparing `remfile-0.1.3/tests/test_main.py` & `remfile-0.1.4/tests/test_main.py`

 * *Files identical despite different names*


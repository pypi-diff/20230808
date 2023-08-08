# Comparing `tmp/remfile-0.1.2.tar.gz` & `tmp/remfile-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "remfile-0.1.2.tar", last modified: Mon Aug  7 23:58:09 2023, max compression
+gzip compressed data, was "remfile-0.1.3.tar", last modified: Tue Aug  8 15:48:20 2023, max compression
```

## Comparing `remfile-0.1.2.tar` & `remfile-0.1.3.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxr-x   0 magland   (1000) magland   (1000)        0 2023-08-07 23:58:09.187381 remfile-0.1.2/
--rw-rw-r--   0 magland   (1000) magland   (1000)    11357 2023-08-07 12:41:38.000000 remfile-0.1.2/LICENSE
--rw-rw-r--   0 magland   (1000) magland   (1000)    15245 2023-08-07 23:58:09.187381 remfile-0.1.2/PKG-INFO
--rw-r--r--   0 magland   (1000) magland   (1000)     1731 2023-08-07 19:45:00.000000 remfile-0.1.2/README.md
--rw-r--r--   0 magland   (1000) magland   (1000)      959 2023-08-07 19:14:40.000000 remfile-0.1.2/pyproject.toml
-drwxrwxr-x   0 magland   (1000) magland   (1000)        0 2023-08-07 23:58:09.187381 remfile-0.1.2/remfile/
--rw-r--r--   0 magland   (1000) magland   (1000)     6549 2023-08-07 23:54:25.000000 remfile-0.1.2/remfile/RemFile.py
--rw-r--r--   0 magland   (1000) magland   (1000)       59 2023-08-07 23:57:25.000000 remfile-0.1.2/remfile/__init__.py
-drwxrwxr-x   0 magland   (1000) magland   (1000)        0 2023-08-07 23:58:09.187381 remfile-0.1.2/remfile.egg-info/
--rw-r--r--   0 magland   (1000) magland   (1000)    15245 2023-08-07 23:58:09.000000 remfile-0.1.2/remfile.egg-info/PKG-INFO
--rw-r--r--   0 magland   (1000) magland   (1000)      244 2023-08-07 23:58:09.000000 remfile-0.1.2/remfile.egg-info/SOURCES.txt
--rw-r--r--   0 magland   (1000) magland   (1000)        1 2023-08-07 23:58:09.000000 remfile-0.1.2/remfile.egg-info/dependency_links.txt
--rw-r--r--   0 magland   (1000) magland   (1000)       29 2023-08-07 23:58:09.000000 remfile-0.1.2/remfile.egg-info/requires.txt
--rw-r--r--   0 magland   (1000) magland   (1000)        8 2023-08-07 23:58:09.000000 remfile-0.1.2/remfile.egg-info/top_level.txt
--rw-rw-r--   0 magland   (1000) magland   (1000)       38 2023-08-07 23:58:09.187381 remfile-0.1.2/setup.cfg
-drwxrwxr-x   0 magland   (1000) magland   (1000)        0 2023-08-07 23:58:09.187381 remfile-0.1.2/tests/
--rw-rw-r--   0 magland   (1000) magland   (1000)      363 2023-08-07 19:14:23.000000 remfile-0.1.2/tests/test_main.py
+drwxrwxr-x   0 magland   (1000) magland   (1000)        0 2023-08-08 15:48:20.202309 remfile-0.1.3/
+-rw-rw-r--   0 magland   (1000) magland   (1000)    11357 2023-08-07 12:41:38.000000 remfile-0.1.3/LICENSE
+-rw-rw-r--   0 magland   (1000) magland   (1000)    15545 2023-08-08 15:48:20.202309 remfile-0.1.3/PKG-INFO
+-rw-r--r--   0 magland   (1000) magland   (1000)     2031 2023-08-08 15:41:35.000000 remfile-0.1.3/README.md
+-rw-r--r--   0 magland   (1000) magland   (1000)      977 2023-08-08 15:10:05.000000 remfile-0.1.3/pyproject.toml
+drwxrwxr-x   0 magland   (1000) magland   (1000)        0 2023-08-08 15:48:20.202309 remfile-0.1.3/remfile/
+-rw-r--r--   0 magland   (1000) magland   (1000)    10197 2023-08-08 15:46:29.000000 remfile-0.1.3/remfile/RemFile.py
+-rw-r--r--   0 magland   (1000) magland   (1000)       59 2023-08-08 15:47:01.000000 remfile-0.1.3/remfile/__init__.py
+drwxrwxr-x   0 magland   (1000) magland   (1000)        0 2023-08-08 15:48:20.202309 remfile-0.1.3/remfile.egg-info/
+-rw-r--r--   0 magland   (1000) magland   (1000)    15545 2023-08-08 15:48:20.000000 remfile-0.1.3/remfile.egg-info/PKG-INFO
+-rw-r--r--   0 magland   (1000) magland   (1000)      244 2023-08-08 15:48:20.000000 remfile-0.1.3/remfile.egg-info/SOURCES.txt
+-rw-r--r--   0 magland   (1000) magland   (1000)        1 2023-08-08 15:48:20.000000 remfile-0.1.3/remfile.egg-info/dependency_links.txt
+-rw-r--r--   0 magland   (1000) magland   (1000)       40 2023-08-08 15:48:20.000000 remfile-0.1.3/remfile.egg-info/requires.txt
+-rw-r--r--   0 magland   (1000) magland   (1000)        8 2023-08-08 15:48:20.000000 remfile-0.1.3/remfile.egg-info/top_level.txt
+-rw-rw-r--   0 magland   (1000) magland   (1000)       38 2023-08-08 15:48:20.202309 remfile-0.1.3/setup.cfg
+drwxrwxr-x   0 magland   (1000) magland   (1000)        0 2023-08-08 15:48:20.202309 remfile-0.1.3/tests/
+-rw-rw-r--   0 magland   (1000) magland   (1000)     1673 2023-08-08 15:43:09.000000 remfile-0.1.3/tests/test_main.py
```

### Comparing `remfile-0.1.2/LICENSE` & `remfile-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `remfile-0.1.2/PKG-INFO` & `remfile-0.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: remfile
-Version: 0.1.2
+Version: 0.1.3
 Summary: File-like object from url of remote file, optimized for use with h5py.
 Author-email: Jeremy Magland <jmagland@flatironinstitute.org>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
@@ -213,14 +213,18 @@
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Provides-Extra: test
 License-File: LICENSE
 
 # remfile
 
+[![latest-release](https://img.shields.io/pypi/v/remfile.svg)](https://pypi.org/project/remfile)
+![tests](https://github.com/magland/remfile/actions/workflows/tests.yml/badge.svg)
+[![codecov](https://codecov.io/gh/magland/remfile/branch/main/graph/badge.svg)](https://codecov.io/gh/magland/remfile)
+
 Provides a file-like object for reading a remote file over HTTP, optimized for use with h5py.
 
 Example usage:
 
 ```python
 # See examples/example1.py
```

### Comparing `remfile-0.1.2/README.md` & `remfile-0.1.3/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,9 +1,13 @@
 # remfile
 
+[![latest-release](https://img.shields.io/pypi/v/remfile.svg)](https://pypi.org/project/remfile)
+![tests](https://github.com/magland/remfile/actions/workflows/tests.yml/badge.svg)
+[![codecov](https://codecov.io/gh/magland/remfile/branch/main/graph/badge.svg)](https://codecov.io/gh/magland/remfile)
+
 Provides a file-like object for reading a remote file over HTTP, optimized for use with h5py.
 
 Example usage:
 
 ```python
 # See examples/example1.py
```

### Comparing `remfile-0.1.2/pyproject.toml` & `remfile-0.1.3/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -18,15 +18,16 @@
 dependencies = [
     "requests",
     "h5py"
 ]
 
 [project.optional-dependencies]
 test = [
-    "pytest"
+    "pytest",
+    "pytest-cov"
 ]
 
 [project.urls]
 repository = "https://github.com/magland/remfile"
 
 [tool.setuptools.packages.find]
 include = ["remfile*"]
```

### Comparing `remfile-0.1.2/remfile.egg-info/PKG-INFO` & `remfile-0.1.3/remfile.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: remfile
-Version: 0.1.2
+Version: 0.1.3
 Summary: File-like object from url of remote file, optimized for use with h5py.
 Author-email: Jeremy Magland <jmagland@flatironinstitute.org>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
@@ -213,14 +213,18 @@
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Provides-Extra: test
 License-File: LICENSE
 
 # remfile
 
+[![latest-release](https://img.shields.io/pypi/v/remfile.svg)](https://pypi.org/project/remfile)
+![tests](https://github.com/magland/remfile/actions/workflows/tests.yml/badge.svg)
+[![codecov](https://codecov.io/gh/magland/remfile/branch/main/graph/badge.svg)](https://codecov.io/gh/magland/remfile)
+
 Provides a file-like object for reading a remote file over HTTP, optimized for use with h5py.
 
 Example usage:
 
 ```python
 # See examples/example1.py
```


# Comparing `tmp/thatway-0.4.0.tar.gz` & `tmp/thatway-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "thatway-0.4.0.tar", last modified: Tue Aug  8 15:50:09 2023, max compression
+gzip compressed data, was "thatway-0.4.1.tar", last modified: Tue Aug  8 15:51:56 2023, max compression
```

## Comparing `thatway-0.4.0.tar` & `thatway-0.4.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 jlorieau   (501) staff       (20)        0 2023-08-08 15:50:09.352532 thatway-0.4.0/
--rw-r--r--   0 jlorieau   (501) staff       (20)     1071 2023-08-07 18:07:13.000000 thatway-0.4.0/LICENSE
--rw-r--r--   0 jlorieau   (501) staff       (20)      376 2023-08-08 15:50:09.352319 thatway-0.4.0/PKG-INFO
--rw-r--r--   0 jlorieau   (501) staff       (20)     5630 2023-08-08 15:49:41.000000 thatway-0.4.0/README.rst
--rw-r--r--   0 jlorieau   (501) staff       (20)      818 2023-08-07 21:51:39.000000 thatway-0.4.0/pyproject.toml
--rw-r--r--   0 jlorieau   (501) staff       (20)       38 2023-08-08 15:50:09.352596 thatway-0.4.0/setup.cfg
-drwxr-xr-x   0 jlorieau   (501) staff       (20)        0 2023-08-08 15:50:09.350189 thatway-0.4.0/tests/
--rw-r--r--   0 jlorieau   (501) staff       (20)     6020 2023-08-08 15:17:21.000000 thatway-0.4.0/tests/test_base.py
-drwxr-xr-x   0 jlorieau   (501) staff       (20)        0 2023-08-08 15:50:09.350724 thatway-0.4.0/thatway/
--rw-r--r--   0 jlorieau   (501) staff       (20)      123 2023-08-08 15:46:14.000000 thatway-0.4.0/thatway/__init__.py
--rw-r--r--   0 jlorieau   (501) staff       (20)    11450 2023-08-08 14:44:07.000000 thatway-0.4.0/thatway/base.py
-drwxr-xr-x   0 jlorieau   (501) staff       (20)        0 2023-08-08 15:50:09.352031 thatway-0.4.0/thatway.egg-info/
--rw-r--r--   0 jlorieau   (501) staff       (20)      376 2023-08-08 15:50:09.000000 thatway-0.4.0/thatway.egg-info/PKG-INFO
--rw-r--r--   0 jlorieau   (501) staff       (20)      242 2023-08-08 15:50:09.000000 thatway-0.4.0/thatway.egg-info/SOURCES.txt
--rw-r--r--   0 jlorieau   (501) staff       (20)        1 2023-08-08 15:50:09.000000 thatway-0.4.0/thatway.egg-info/dependency_links.txt
--rw-r--r--   0 jlorieau   (501) staff       (20)       57 2023-08-08 15:50:09.000000 thatway-0.4.0/thatway.egg-info/requires.txt
--rw-r--r--   0 jlorieau   (501) staff       (20)        8 2023-08-08 15:50:09.000000 thatway-0.4.0/thatway.egg-info/top_level.txt
+drwxr-xr-x   0 jlorieau   (501) staff       (20)        0 2023-08-08 15:51:56.954287 thatway-0.4.1/
+-rw-r--r--   0 jlorieau   (501) staff       (20)     1071 2023-08-07 18:07:13.000000 thatway-0.4.1/LICENSE
+-rw-r--r--   0 jlorieau   (501) staff       (20)     6004 2023-08-08 15:51:56.954086 thatway-0.4.1/PKG-INFO
+-rw-r--r--   0 jlorieau   (501) staff       (20)     5630 2023-08-08 15:49:41.000000 thatway-0.4.1/README.rst
+-rw-r--r--   0 jlorieau   (501) staff       (20)      819 2023-08-08 15:51:25.000000 thatway-0.4.1/pyproject.toml
+-rw-r--r--   0 jlorieau   (501) staff       (20)       38 2023-08-08 15:51:56.954372 thatway-0.4.1/setup.cfg
+drwxr-xr-x   0 jlorieau   (501) staff       (20)        0 2023-08-08 15:51:56.951531 thatway-0.4.1/tests/
+-rw-r--r--   0 jlorieau   (501) staff       (20)     6020 2023-08-08 15:17:21.000000 thatway-0.4.1/tests/test_base.py
+drwxr-xr-x   0 jlorieau   (501) staff       (20)        0 2023-08-08 15:51:56.952235 thatway-0.4.1/thatway/
+-rw-r--r--   0 jlorieau   (501) staff       (20)      123 2023-08-08 15:51:14.000000 thatway-0.4.1/thatway/__init__.py
+-rw-r--r--   0 jlorieau   (501) staff       (20)    11450 2023-08-08 14:44:07.000000 thatway-0.4.1/thatway/base.py
+drwxr-xr-x   0 jlorieau   (501) staff       (20)        0 2023-08-08 15:51:56.953746 thatway-0.4.1/thatway.egg-info/
+-rw-r--r--   0 jlorieau   (501) staff       (20)     6004 2023-08-08 15:51:56.000000 thatway-0.4.1/thatway.egg-info/PKG-INFO
+-rw-r--r--   0 jlorieau   (501) staff       (20)      242 2023-08-08 15:51:56.000000 thatway-0.4.1/thatway.egg-info/SOURCES.txt
+-rw-r--r--   0 jlorieau   (501) staff       (20)        1 2023-08-08 15:51:56.000000 thatway-0.4.1/thatway.egg-info/dependency_links.txt
+-rw-r--r--   0 jlorieau   (501) staff       (20)       57 2023-08-08 15:51:56.000000 thatway-0.4.1/thatway.egg-info/requires.txt
+-rw-r--r--   0 jlorieau   (501) staff       (20)        8 2023-08-08 15:51:56.000000 thatway-0.4.1/thatway.egg-info/top_level.txt
```

### Comparing `thatway-0.4.0/LICENSE` & `thatway-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `thatway-0.4.0/README.rst` & `thatway-0.4.1/README.rst`

 * *Files identical despite different names*

### Comparing `thatway-0.4.0/pyproject.toml` & `thatway-0.4.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [project]
 name = "thatway"
 authors = [
     {name = "Justin Lorieau"},
 ]
-readme = "README.md"
+readme = "README.rst"
 requires-python = ">=3.8"
 classifiers = [
     "Programming Language :: Python :: 3 :: Only",
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3.8",
     "Development Status :: 4 - Beta",
     ]
```

### Comparing `thatway-0.4.0/tests/test_base.py` & `thatway-0.4.1/tests/test_base.py`

 * *Files identical despite different names*

### Comparing `thatway-0.4.0/thatway/base.py` & `thatway-0.4.1/thatway/base.py`

 * *Files identical despite different names*


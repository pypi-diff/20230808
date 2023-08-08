# Comparing `tmp/veracross-client-0.0.1.tar.gz` & `tmp/veracross-client-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "veracross-client-0.0.1.tar", last modified: Tue Aug  8 21:03:18 2023, max compression
+gzip compressed data, was "veracross-client-0.0.2.tar", last modified: Tue Aug  8 21:08:12 2023, max compression
```

## Comparing `veracross-client-0.0.1.tar` & `veracross-client-0.0.2.tar`

### file list

```diff
@@ -1,14 +1,17 @@
-drwxrwxr-x   0 hudson    (1000) hudson    (1000)        0 2023-08-08 21:03:18.362916 veracross-client-0.0.1/
--rw-rw-r--   0 hudson    (1000) hudson    (1000)     1074 2023-08-08 20:06:06.000000 veracross-client-0.0.1/LICENSE
--rw-rw-r--   0 hudson    (1000) hudson    (1000)      613 2023-08-08 21:03:18.362916 veracross-client-0.0.1/PKG-INFO
--rw-rw-r--   0 hudson    (1000) hudson    (1000)       18 2023-08-08 20:06:06.000000 veracross-client-0.0.1/README.md
--rw-rw-r--   0 hudson    (1000) hudson    (1000)      648 2023-08-08 21:03:08.000000 veracross-client-0.0.1/pyproject.toml
--rw-rw-r--   0 hudson    (1000) hudson    (1000)      295 2023-08-08 21:03:18.362916 veracross-client-0.0.1/setup.cfg
--rw-rw-r--   0 hudson    (1000) hudson    (1000)      351 2023-08-08 20:23:44.000000 veracross-client-0.0.1/setup.py
-drwxrwxr-x   0 hudson    (1000) hudson    (1000)        0 2023-08-08 21:03:18.362916 veracross-client-0.0.1/src/
-drwxrwxr-x   0 hudson    (1000) hudson    (1000)        0 2023-08-08 21:03:18.362916 veracross-client-0.0.1/src/veracross_client.egg-info/
--rw-rw-r--   0 hudson    (1000) hudson    (1000)      613 2023-08-08 21:03:18.000000 veracross-client-0.0.1/src/veracross_client.egg-info/PKG-INFO
--rw-rw-r--   0 hudson    (1000) hudson    (1000)      270 2023-08-08 21:03:18.000000 veracross-client-0.0.1/src/veracross_client.egg-info/SOURCES.txt
--rw-rw-r--   0 hudson    (1000) hudson    (1000)        1 2023-08-08 21:03:18.000000 veracross-client-0.0.1/src/veracross_client.egg-info/dependency_links.txt
--rw-rw-r--   0 hudson    (1000) hudson    (1000)       16 2023-08-08 21:03:18.000000 veracross-client-0.0.1/src/veracross_client.egg-info/requires.txt
--rw-rw-r--   0 hudson    (1000) hudson    (1000)        1 2023-08-08 21:03:18.000000 veracross-client-0.0.1/src/veracross_client.egg-info/top_level.txt
+drwxrwxr-x   0 hudson    (1000) hudson    (1000)        0 2023-08-08 21:08:12.016316 veracross-client-0.0.2/
+-rw-rw-r--   0 hudson    (1000) hudson    (1000)     1074 2023-08-08 20:06:06.000000 veracross-client-0.0.2/LICENSE
+-rw-rw-r--   0 hudson    (1000) hudson    (1000)      613 2023-08-08 21:08:12.016316 veracross-client-0.0.2/PKG-INFO
+-rw-rw-r--   0 hudson    (1000) hudson    (1000)       18 2023-08-08 20:06:06.000000 veracross-client-0.0.2/README.md
+-rw-rw-r--   0 hudson    (1000) hudson    (1000)      648 2023-08-08 21:08:03.000000 veracross-client-0.0.2/pyproject.toml
+-rw-rw-r--   0 hudson    (1000) hudson    (1000)      295 2023-08-08 21:08:12.016316 veracross-client-0.0.2/setup.cfg
+-rw-rw-r--   0 hudson    (1000) hudson    (1000)      351 2023-08-08 21:07:59.000000 veracross-client-0.0.2/setup.py
+drwxrwxr-x   0 hudson    (1000) hudson    (1000)        0 2023-08-08 21:08:12.016316 veracross-client-0.0.2/src/
+drwxrwxr-x   0 hudson    (1000) hudson    (1000)        0 2023-08-08 21:08:12.016316 veracross-client-0.0.2/src/veracross_client/
+-rw-rw-r--   0 hudson    (1000) hudson    (1000)       45 2023-08-08 21:07:38.000000 veracross-client-0.0.2/src/veracross_client/__init__.py
+-rw-rw-r--   0 hudson    (1000) hudson    (1000)   440433 2023-08-08 20:54:13.000000 veracross-client-0.0.2/src/veracross_client/veracross_client.py
+drwxrwxr-x   0 hudson    (1000) hudson    (1000)        0 2023-08-08 21:08:12.016316 veracross-client-0.0.2/src/veracross_client.egg-info/
+-rw-rw-r--   0 hudson    (1000) hudson    (1000)      613 2023-08-08 21:08:12.000000 veracross-client-0.0.2/src/veracross_client.egg-info/PKG-INFO
+-rw-rw-r--   0 hudson    (1000) hudson    (1000)      344 2023-08-08 21:08:12.000000 veracross-client-0.0.2/src/veracross_client.egg-info/SOURCES.txt
+-rw-rw-r--   0 hudson    (1000) hudson    (1000)        1 2023-08-08 21:08:12.000000 veracross-client-0.0.2/src/veracross_client.egg-info/dependency_links.txt
+-rw-rw-r--   0 hudson    (1000) hudson    (1000)       16 2023-08-08 21:08:12.000000 veracross-client-0.0.2/src/veracross_client.egg-info/requires.txt
+-rw-rw-r--   0 hudson    (1000) hudson    (1000)       17 2023-08-08 21:08:12.000000 veracross-client-0.0.2/src/veracross_client.egg-info/top_level.txt
```

### Comparing `veracross-client-0.0.1/LICENSE` & `veracross-client-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `veracross-client-0.0.1/PKG-INFO` & `veracross-client-0.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: veracross-client
-Version: 0.0.1
+Version: 0.0.2
 Summary: Python wrapper for communicating with the Veracross API
 Author: Hudson Harper
 Author-email: Hudson Harper <hudson@harpertech.io>
 Project-URL: Homepage, https://github.com/hudson-harpertech/veracross-client
 Project-URL: Bug Tracker, https://github.com/hudson-harpertech/veracross-client/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `veracross-client-0.0.1/pyproject.toml` & `veracross-client-0.0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "veracross-client"
-version = "0.0.1"
+version = "0.0.2"
 authors = [
   { name="Hudson Harper", email="hudson@harpertech.io" },
 ]
 description = "Python wrapper for communicating with the Veracross API"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `veracross-client-0.0.1/src/veracross_client.egg-info/PKG-INFO` & `veracross-client-0.0.2/src/veracross_client.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: veracross-client
-Version: 0.0.1
+Version: 0.0.2
 Summary: Python wrapper for communicating with the Veracross API
 Author: Hudson Harper
 Author-email: Hudson Harper <hudson@harpertech.io>
 Project-URL: Homepage, https://github.com/hudson-harpertech/veracross-client
 Project-URL: Bug Tracker, https://github.com/hudson-harpertech/veracross-client/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```


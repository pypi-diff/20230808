# Comparing `tmp/elabapy-1.0.0.tar.gz` & `tmp/elabapy-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "elabapy-1.0.0.tar", last modified: Fri Dec  9 12:41:34 2022, max compression
+gzip compressed data, was "elabapy-1.1.0.tar", last modified: Tue Aug  8 16:31:00 2023, max compression
```

## Comparing `elabapy-1.0.0.tar` & `elabapy-1.1.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-09 12:41:34.538639 elabapy-1.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)    32005 2022-12-09 12:41:26.000000 elabapy-1.0.0/LICENCE
--rw-r--r--   0 runner    (1001) docker     (123)      302 2022-12-09 12:41:34.538639 elabapy-1.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2156 2022-12-09 12:41:26.000000 elabapy-1.0.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-09 12:41:34.538639 elabapy-1.0.0/elabapy/
--rw-r--r--   0 runner    (1001) docker     (123)     5501 2022-12-09 12:41:26.000000 elabapy-1.0.0/elabapy/Manager.py
--rw-r--r--   0 runner    (1001) docker     (123)      317 2022-12-09 12:41:26.000000 elabapy-1.0.0/elabapy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2460 2022-12-09 12:41:26.000000 elabapy-1.0.0/elabapy/baseapi.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-09 12:41:34.538639 elabapy-1.0.0/elabapy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      302 2022-12-09 12:41:34.000000 elabapy-1.0.0/elabapy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      238 2022-12-09 12:41:34.000000 elabapy-1.0.0/elabapy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-09 12:41:34.000000 elabapy-1.0.0/elabapy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2022-12-09 12:41:34.000000 elabapy-1.0.0/elabapy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2022-12-09 12:41:34.000000 elabapy-1.0.0/elabapy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2022-12-09 12:41:34.538639 elabapy-1.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      515 2022-12-09 12:41:26.000000 elabapy-1.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 16:31:00.074812 elabapy-1.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    32005 2023-08-08 16:30:50.000000 elabapy-1.1.0/LICENCE
+-rw-r--r--   0 runner    (1001) docker     (123)      302 2023-08-08 16:31:00.074812 elabapy-1.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2394 2023-08-08 16:30:50.000000 elabapy-1.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 16:31:00.074812 elabapy-1.1.0/elabapy/
+-rw-r--r--   0 runner    (1001) docker     (123)     5501 2023-08-08 16:30:50.000000 elabapy-1.1.0/elabapy/Manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)      317 2023-08-08 16:30:50.000000 elabapy-1.1.0/elabapy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2460 2023-08-08 16:30:50.000000 elabapy-1.1.0/elabapy/baseapi.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 16:31:00.074812 elabapy-1.1.0/elabapy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      302 2023-08-08 16:31:00.000000 elabapy-1.1.0/elabapy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      238 2023-08-08 16:31:00.000000 elabapy-1.1.0/elabapy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 16:31:00.000000 elabapy-1.1.0/elabapy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-08-08 16:31:00.000000 elabapy-1.1.0/elabapy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-08-08 16:31:00.000000 elabapy-1.1.0/elabapy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-08 16:31:00.074812 elabapy-1.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      515 2023-08-08 16:30:50.000000 elabapy-1.1.0/setup.py
```

### Comparing `elabapy-1.0.0/LICENCE` & `elabapy-1.1.0/LICENCE`

 * *Files identical despite different names*

### Comparing `elabapy-1.0.0/README.md` & `elabapy-1.1.0/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -9,14 +9,18 @@
 
 # API Versions
 
 This library works with eLabFTW's API v1. It is recommended to use API v2. A python package is available for API v2, see this repository:
 
 ### APIv2 Python lib: https://github.com/elabftw/elabapi-python/
 
+# WARNING: DEPRECATED LIBRARY
+
+Because this package is for APIv1 and APIv1 is deprecated from eLab, this library is therefore also deprecated and should not be used.
+
 ## Install
 
 You can install elabapy using **pip**:
 
 ~~~bash
 pip install --user elabapy
 ~~~
@@ -78,7 +82,11 @@
 * Update version in `setup.py` and `elabapy/__init__.py`
 * Update changelog
 * Commit
 * Tag
 * Create release on GitHub
 
 A GitHub Action will take care of publishing it to Pypi.org.
+
+### Update requirements.txt
+
+`pipenv requirements > requirements.txt`
```

### Comparing `elabapy-1.0.0/elabapy/Manager.py` & `elabapy-1.1.0/elabapy/Manager.py`

 * *Files identical despite different names*

### Comparing `elabapy-1.0.0/elabapy/baseapi.py` & `elabapy-1.1.0/elabapy/baseapi.py`

 * *Files identical despite different names*

### Comparing `elabapy-1.0.0/setup.py` & `elabapy-1.1.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #!/usr/bin/env python
 from setuptools import setup
 
 long_description = """This library provides easy access to eLabFTW's API."""
 
 setup(
     name='elabapy',
-    version='1.0.0',
+    version='1.1.0',
     description='elabftw API to manage experiments and items',
     author='Nicolas CARPi',
     author_email='nico-git@deltablot.email',
     url='https://github.com/elabftw/elabapy',
     packages=['elabapy'],
     install_requires=['requests'],
     test_suite='elabapy.tests',
```


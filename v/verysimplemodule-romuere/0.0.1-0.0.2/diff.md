# Comparing `tmp/verysimplemodule_romuere-0.0.1.tar.gz` & `tmp/verysimplemodule_romuere-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "verysimplemodule_romuere-0.0.1.tar", last modified: Tue Aug  8 12:51:09 2023, max compression
+gzip compressed data, was "verysimplemodule_romuere-0.0.2.tar", last modified: Tue Aug  8 13:07:41 2023, max compression
```

## Comparing `verysimplemodule_romuere-0.0.1.tar` & `verysimplemodule_romuere-0.0.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 romuere    (501) staff       (20)        0 2023-08-08 12:51:09.705399 verysimplemodule_romuere-0.0.1/
--rw-r--r--   0 romuere    (501) staff       (20)      424 2023-08-08 12:51:09.704806 verysimplemodule_romuere-0.0.1/PKG-INFO
--rw-r--r--   0 romuere    (501) staff       (20)       38 2023-08-08 12:51:09.705637 verysimplemodule_romuere-0.0.1/setup.cfg
--rw-r--r--   0 romuere    (501) staff       (20)      954 2023-08-08 12:49:45.000000 verysimplemodule_romuere-0.0.1/setup.py
-drwxr-xr-x   0 romuere    (501) staff       (20)        0 2023-08-08 12:51:09.698005 verysimplemodule_romuere-0.0.1/verysimplemodule_romuere/
--rw-r--r--   0 romuere    (501) staff       (20)       49 2023-08-08 12:21:18.000000 verysimplemodule_romuere-0.0.1/verysimplemodule_romuere/__init__.py
--rw-r--r--   0 romuere    (501) staff       (20)       29 2023-08-08 12:19:39.000000 verysimplemodule_romuere-0.0.1/verysimplemodule_romuere/add.py
-drwxr-xr-x   0 romuere    (501) staff       (20)        0 2023-08-08 12:51:09.704239 verysimplemodule_romuere-0.0.1/verysimplemodule_romuere/extra/
--rw-r--r--   0 romuere    (501) staff       (20)       55 2023-08-08 12:22:19.000000 verysimplemodule_romuere-0.0.1/verysimplemodule_romuere/extra/__init__.py
--rw-r--r--   0 romuere    (501) staff       (20)       32 2023-08-08 12:19:11.000000 verysimplemodule_romuere-0.0.1/verysimplemodule_romuere/extra/divide.py
--rw-r--r--   0 romuere    (501) staff       (20)       34 2023-08-08 12:19:28.000000 verysimplemodule_romuere-0.0.1/verysimplemodule_romuere/extra/multiple.py
--rw-r--r--   0 romuere    (501) staff       (20)       34 2023-08-08 12:19:55.000000 verysimplemodule_romuere-0.0.1/verysimplemodule_romuere/subtract.py
-drwxr-xr-x   0 romuere    (501) staff       (20)        0 2023-08-08 12:51:09.701708 verysimplemodule_romuere-0.0.1/verysimplemodule_romuere.egg-info/
--rw-r--r--   0 romuere    (501) staff       (20)      424 2023-08-08 12:51:09.000000 verysimplemodule_romuere-0.0.1/verysimplemodule_romuere.egg-info/PKG-INFO
--rw-r--r--   0 romuere    (501) staff       (20)      480 2023-08-08 12:51:09.000000 verysimplemodule_romuere-0.0.1/verysimplemodule_romuere.egg-info/SOURCES.txt
--rw-r--r--   0 romuere    (501) staff       (20)        1 2023-08-08 12:51:09.000000 verysimplemodule_romuere-0.0.1/verysimplemodule_romuere.egg-info/dependency_links.txt
--rw-r--r--   0 romuere    (501) staff       (20)       19 2023-08-08 12:51:09.000000 verysimplemodule_romuere-0.0.1/verysimplemodule_romuere.egg-info/requires.txt
--rw-r--r--   0 romuere    (501) staff       (20)       25 2023-08-08 12:51:09.000000 verysimplemodule_romuere-0.0.1/verysimplemodule_romuere.egg-info/top_level.txt
+drwxr-xr-x   0 romuere    (501) staff       (20)        0 2023-08-08 13:07:41.925541 verysimplemodule_romuere-0.0.2/
+-rw-r--r--   0 romuere    (501) staff       (20)      424 2023-08-08 13:07:41.924771 verysimplemodule_romuere-0.0.2/PKG-INFO
+-rw-r--r--   0 romuere    (501) staff       (20)       38 2023-08-08 13:07:41.925812 verysimplemodule_romuere-0.0.2/setup.cfg
+-rw-r--r--   0 romuere    (501) staff       (20)      954 2023-08-08 13:07:17.000000 verysimplemodule_romuere-0.0.2/setup.py
+drwxr-xr-x   0 romuere    (501) staff       (20)        0 2023-08-08 13:07:41.914420 verysimplemodule_romuere-0.0.2/verysimplemodule_romuere/
+-rw-r--r--   0 romuere    (501) staff       (20)       49 2023-08-08 12:21:18.000000 verysimplemodule_romuere-0.0.2/verysimplemodule_romuere/__init__.py
+-rw-r--r--   0 romuere    (501) staff       (20)       29 2023-08-08 12:19:39.000000 verysimplemodule_romuere-0.0.2/verysimplemodule_romuere/add.py
+drwxr-xr-x   0 romuere    (501) staff       (20)        0 2023-08-08 13:07:41.923767 verysimplemodule_romuere-0.0.2/verysimplemodule_romuere/extra/
+-rw-r--r--   0 romuere    (501) staff       (20)       55 2023-08-08 12:22:19.000000 verysimplemodule_romuere-0.0.2/verysimplemodule_romuere/extra/__init__.py
+-rw-r--r--   0 romuere    (501) staff       (20)       32 2023-08-08 12:19:11.000000 verysimplemodule_romuere-0.0.2/verysimplemodule_romuere/extra/divide.py
+-rw-r--r--   0 romuere    (501) staff       (20)       34 2023-08-08 12:19:28.000000 verysimplemodule_romuere-0.0.2/verysimplemodule_romuere/extra/multiple.py
+-rw-r--r--   0 romuere    (501) staff       (20)       34 2023-08-08 12:19:55.000000 verysimplemodule_romuere-0.0.2/verysimplemodule_romuere/subtract.py
+drwxr-xr-x   0 romuere    (501) staff       (20)        0 2023-08-08 13:07:41.921081 verysimplemodule_romuere-0.0.2/verysimplemodule_romuere.egg-info/
+-rw-r--r--   0 romuere    (501) staff       (20)      424 2023-08-08 13:07:41.000000 verysimplemodule_romuere-0.0.2/verysimplemodule_romuere.egg-info/PKG-INFO
+-rw-r--r--   0 romuere    (501) staff       (20)      480 2023-08-08 13:07:41.000000 verysimplemodule_romuere-0.0.2/verysimplemodule_romuere.egg-info/SOURCES.txt
+-rw-r--r--   0 romuere    (501) staff       (20)        1 2023-08-08 13:07:41.000000 verysimplemodule_romuere-0.0.2/verysimplemodule_romuere.egg-info/dependency_links.txt
+-rw-r--r--   0 romuere    (501) staff       (20)       19 2023-08-08 13:07:41.000000 verysimplemodule_romuere-0.0.2/verysimplemodule_romuere.egg-info/requires.txt
+-rw-r--r--   0 romuere    (501) staff       (20)       25 2023-08-08 13:07:41.000000 verysimplemodule_romuere-0.0.2/verysimplemodule_romuere.egg-info/top_level.txt
```

### Comparing `verysimplemodule_romuere-0.0.1/setup.py` & `verysimplemodule_romuere-0.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '0.0.1' 
+VERSION = '0.0.2' 
 DESCRIPTION = 'My first Python package'
 LONG_DESCRIPTION = 'My first Python package with a slightly longer description'
 
 # Setting up
 setup(
        # the name must match the folder name 'verysimplemodule'
         name="verysimplemodule_romuere",
```


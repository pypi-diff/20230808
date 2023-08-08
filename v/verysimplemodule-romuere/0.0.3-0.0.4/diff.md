# Comparing `tmp/verysimplemodule_romuere-0.0.3.tar.gz` & `tmp/verysimplemodule_romuere-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "verysimplemodule_romuere-0.0.3.tar", last modified: Tue Aug  8 13:13:25 2023, max compression
+gzip compressed data, was "verysimplemodule_romuere-0.0.4.tar", last modified: Tue Aug  8 13:17:54 2023, max compression
```

## Comparing `verysimplemodule_romuere-0.0.3.tar` & `verysimplemodule_romuere-0.0.4.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 romuere    (501) staff       (20)        0 2023-08-08 13:13:25.081816 verysimplemodule_romuere-0.0.3/
--rw-r--r--   0 romuere    (501) staff       (20)      424 2023-08-08 13:13:25.081167 verysimplemodule_romuere-0.0.3/PKG-INFO
--rw-r--r--   0 romuere    (501) staff       (20)       38 2023-08-08 13:13:25.082042 verysimplemodule_romuere-0.0.3/setup.cfg
--rw-r--r--   0 romuere    (501) staff       (20)      954 2023-08-08 13:13:06.000000 verysimplemodule_romuere-0.0.3/setup.py
-drwxr-xr-x   0 romuere    (501) staff       (20)        0 2023-08-08 13:13:25.073417 verysimplemodule_romuere-0.0.3/verysimplemodule_romuere/
--rw-r--r--   0 romuere    (501) staff       (20)       45 2023-08-08 13:12:48.000000 verysimplemodule_romuere-0.0.3/verysimplemodule_romuere/__init__.py
--rw-r--r--   0 romuere    (501) staff       (20)       30 2023-08-08 13:12:23.000000 verysimplemodule_romuere-0.0.3/verysimplemodule_romuere/add.py
-drwxr-xr-x   0 romuere    (501) staff       (20)        0 2023-08-08 13:13:25.080189 verysimplemodule_romuere-0.0.3/verysimplemodule_romuere/extra/
--rw-r--r--   0 romuere    (501) staff       (20)       55 2023-08-08 12:22:19.000000 verysimplemodule_romuere-0.0.3/verysimplemodule_romuere/extra/__init__.py
--rw-r--r--   0 romuere    (501) staff       (20)       32 2023-08-08 12:19:11.000000 verysimplemodule_romuere-0.0.3/verysimplemodule_romuere/extra/divide.py
--rw-r--r--   0 romuere    (501) staff       (20)       34 2023-08-08 12:19:28.000000 verysimplemodule_romuere-0.0.3/verysimplemodule_romuere/extra/multiple.py
--rw-r--r--   0 romuere    (501) staff       (20)       29 2023-08-08 13:12:30.000000 verysimplemodule_romuere-0.0.3/verysimplemodule_romuere/subtract.py
-drwxr-xr-x   0 romuere    (501) staff       (20)        0 2023-08-08 13:13:25.077179 verysimplemodule_romuere-0.0.3/verysimplemodule_romuere.egg-info/
--rw-r--r--   0 romuere    (501) staff       (20)      424 2023-08-08 13:13:24.000000 verysimplemodule_romuere-0.0.3/verysimplemodule_romuere.egg-info/PKG-INFO
--rw-r--r--   0 romuere    (501) staff       (20)      480 2023-08-08 13:13:24.000000 verysimplemodule_romuere-0.0.3/verysimplemodule_romuere.egg-info/SOURCES.txt
--rw-r--r--   0 romuere    (501) staff       (20)        1 2023-08-08 13:13:24.000000 verysimplemodule_romuere-0.0.3/verysimplemodule_romuere.egg-info/dependency_links.txt
--rw-r--r--   0 romuere    (501) staff       (20)       19 2023-08-08 13:13:24.000000 verysimplemodule_romuere-0.0.3/verysimplemodule_romuere.egg-info/requires.txt
--rw-r--r--   0 romuere    (501) staff       (20)       25 2023-08-08 13:13:24.000000 verysimplemodule_romuere-0.0.3/verysimplemodule_romuere.egg-info/top_level.txt
+drwxr-xr-x   0 romuere    (501) staff       (20)        0 2023-08-08 13:17:54.316512 verysimplemodule_romuere-0.0.4/
+-rw-r--r--   0 romuere    (501) staff       (20)      424 2023-08-08 13:17:54.315808 verysimplemodule_romuere-0.0.4/PKG-INFO
+-rw-r--r--   0 romuere    (501) staff       (20)       38 2023-08-08 13:17:54.316748 verysimplemodule_romuere-0.0.4/setup.cfg
+-rw-r--r--   0 romuere    (501) staff       (20)      954 2023-08-08 13:17:43.000000 verysimplemodule_romuere-0.0.4/setup.py
+drwxr-xr-x   0 romuere    (501) staff       (20)        0 2023-08-08 13:17:54.304776 verysimplemodule_romuere-0.0.4/verysimplemodule_romuere/
+-rw-r--r--   0 romuere    (501) staff       (20)      102 2023-08-08 13:16:47.000000 verysimplemodule_romuere-0.0.4/verysimplemodule_romuere/__init__.py
+-rw-r--r--   0 romuere    (501) staff       (20)       30 2023-08-08 13:12:23.000000 verysimplemodule_romuere-0.0.4/verysimplemodule_romuere/add.py
+drwxr-xr-x   0 romuere    (501) staff       (20)        0 2023-08-08 13:17:54.314284 verysimplemodule_romuere-0.0.4/verysimplemodule_romuere/extra/
+-rw-r--r--   0 romuere    (501) staff       (20)       94 2023-08-08 13:17:23.000000 verysimplemodule_romuere-0.0.4/verysimplemodule_romuere/extra/__init__.py
+-rw-r--r--   0 romuere    (501) staff       (20)       32 2023-08-08 12:19:11.000000 verysimplemodule_romuere-0.0.4/verysimplemodule_romuere/extra/divide.py
+-rw-r--r--   0 romuere    (501) staff       (20)       34 2023-08-08 12:19:28.000000 verysimplemodule_romuere-0.0.4/verysimplemodule_romuere/extra/multiple.py
+-rw-r--r--   0 romuere    (501) staff       (20)       29 2023-08-08 13:12:30.000000 verysimplemodule_romuere-0.0.4/verysimplemodule_romuere/subtract.py
+drwxr-xr-x   0 romuere    (501) staff       (20)        0 2023-08-08 13:17:54.309685 verysimplemodule_romuere-0.0.4/verysimplemodule_romuere.egg-info/
+-rw-r--r--   0 romuere    (501) staff       (20)      424 2023-08-08 13:17:53.000000 verysimplemodule_romuere-0.0.4/verysimplemodule_romuere.egg-info/PKG-INFO
+-rw-r--r--   0 romuere    (501) staff       (20)      480 2023-08-08 13:17:54.000000 verysimplemodule_romuere-0.0.4/verysimplemodule_romuere.egg-info/SOURCES.txt
+-rw-r--r--   0 romuere    (501) staff       (20)        1 2023-08-08 13:17:53.000000 verysimplemodule_romuere-0.0.4/verysimplemodule_romuere.egg-info/dependency_links.txt
+-rw-r--r--   0 romuere    (501) staff       (20)       19 2023-08-08 13:17:53.000000 verysimplemodule_romuere-0.0.4/verysimplemodule_romuere.egg-info/requires.txt
+-rw-r--r--   0 romuere    (501) staff       (20)       25 2023-08-08 13:17:53.000000 verysimplemodule_romuere-0.0.4/verysimplemodule_romuere.egg-info/top_level.txt
```

### Comparing `verysimplemodule_romuere-0.0.3/setup.py` & `verysimplemodule_romuere-0.0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '0.0.3' 
+VERSION = '0.0.4' 
 DESCRIPTION = 'My first Python package'
 LONG_DESCRIPTION = 'My first Python package with a slightly longer description'
 
 # Setting up
 setup(
        # the name must match the folder name 'verysimplemodule'
         name="verysimplemodule_romuere",
```


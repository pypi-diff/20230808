# Comparing `tmp/sckan-compare-0.0.3.tar.gz` & `tmp/sckan-compare-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sckan-compare-0.0.3.tar", last modified: Mon Aug  7 23:56:32 2023, max compression
+gzip compressed data, was "sckan-compare-0.0.4.tar", last modified: Tue Aug  8 00:13:47 2023, max compression
```

## Comparing `sckan-compare-0.0.3.tar` & `sckan-compare-0.0.4.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxr-x   0 shailesh  (1000) shailesh  (1000)        0 2023-08-07 23:56:32.950679 sckan-compare-0.0.3/
--rw-rw-r--   0 shailesh  (1000) shailesh  (1000)    11356 2023-08-07 08:19:50.000000 sckan-compare-0.0.3/LICENSE
--rw-rw-r--   0 shailesh  (1000) shailesh  (1000)      412 2023-08-07 23:56:32.950679 sckan-compare-0.0.3/PKG-INFO
--rw-rw-r--   0 shailesh  (1000) shailesh  (1000)     3941 2023-08-07 23:54:51.000000 sckan-compare-0.0.3/README.md
-drwxrwxr-x   0 shailesh  (1000) shailesh  (1000)        0 2023-08-07 23:56:32.946679 sckan-compare-0.0.3/sckan_compare/
--rw-rw-r--   0 shailesh  (1000) shailesh  (1000)    14104 2023-08-07 23:54:51.000000 sckan-compare-0.0.3/sckan_compare/__init__.py
-drwxrwxr-x   0 shailesh  (1000) shailesh  (1000)        0 2023-08-07 23:56:32.946679 sckan-compare-0.0.3/sckan_compare/data/
--rw-rw-r--   0 shailesh  (1000) shailesh  (1000)    10012 2023-08-07 19:02:28.000000 sckan-compare-0.0.3/sckan_compare/data/coords_human.json
--rw-rw-r--   0 shailesh  (1000) shailesh  (1000)     4559 2023-08-07 15:59:15.000000 sckan-compare-0.0.3/sckan_compare/data/coords_mouse.json
--rw-rw-r--   0 shailesh  (1000) shailesh  (1000)    21317 2023-08-07 19:02:28.000000 sckan-compare-0.0.3/sckan_compare/data/coords_rat.json
--rw-rw-r--   0 shailesh  (1000) shailesh  (1000)       73 2023-08-07 09:47:01.000000 sckan-compare-0.0.3/sckan_compare/globals.py
--rw-rw-r--   0 shailesh  (1000) shailesh  (1000)     7040 2023-08-07 14:46:14.000000 sckan-compare-0.0.3/sckan_compare/query.py
--rw-rw-r--   0 shailesh  (1000) shailesh  (1000)     6482 2023-08-07 23:47:35.000000 sckan-compare-0.0.3/sckan_compare/simplevis.py
--rw-rw-r--   0 shailesh  (1000) shailesh  (1000)     1138 2023-08-07 15:11:05.000000 sckan-compare-0.0.3/sckan_compare/utils.py
--rw-rw-r--   0 shailesh  (1000) shailesh  (1000)    11307 2023-08-07 21:29:46.000000 sckan-compare-0.0.3/sckan_compare/visualize.py
-drwxrwxr-x   0 shailesh  (1000) shailesh  (1000)        0 2023-08-07 23:56:32.946679 sckan-compare-0.0.3/sckan_compare.egg-info/
--rw-rw-r--   0 shailesh  (1000) shailesh  (1000)      412 2023-08-07 23:56:32.000000 sckan-compare-0.0.3/sckan_compare.egg-info/PKG-INFO
--rw-rw-r--   0 shailesh  (1000) shailesh  (1000)      434 2023-08-07 23:56:32.000000 sckan-compare-0.0.3/sckan_compare.egg-info/SOURCES.txt
--rw-rw-r--   0 shailesh  (1000) shailesh  (1000)        1 2023-08-07 23:56:32.000000 sckan-compare-0.0.3/sckan_compare.egg-info/dependency_links.txt
--rw-rw-r--   0 shailesh  (1000) shailesh  (1000)       14 2023-08-07 23:56:32.000000 sckan-compare-0.0.3/sckan_compare.egg-info/top_level.txt
--rw-rw-r--   0 shailesh  (1000) shailesh  (1000)       38 2023-08-07 23:56:32.950679 sckan-compare-0.0.3/setup.cfg
--rw-rw-r--   0 shailesh  (1000) shailesh  (1000)      585 2023-08-07 23:47:35.000000 sckan-compare-0.0.3/setup.py
+drwxrwxr-x   0 shailesh  (1000) shailesh  (1000)        0 2023-08-08 00:13:47.824215 sckan-compare-0.0.4/
+-rw-rw-r--   0 shailesh  (1000) shailesh  (1000)    11356 2023-08-07 08:19:50.000000 sckan-compare-0.0.4/LICENSE
+-rw-rw-r--   0 shailesh  (1000) shailesh  (1000)      412 2023-08-08 00:13:47.824215 sckan-compare-0.0.4/PKG-INFO
+-rw-rw-r--   0 shailesh  (1000) shailesh  (1000)     3941 2023-08-07 23:54:51.000000 sckan-compare-0.0.4/README.md
+drwxrwxr-x   0 shailesh  (1000) shailesh  (1000)        0 2023-08-08 00:13:47.824215 sckan-compare-0.0.4/sckan_compare/
+-rw-rw-r--   0 shailesh  (1000) shailesh  (1000)    14104 2023-08-08 00:08:37.000000 sckan-compare-0.0.4/sckan_compare/__init__.py
+drwxrwxr-x   0 shailesh  (1000) shailesh  (1000)        0 2023-08-08 00:13:47.824215 sckan-compare-0.0.4/sckan_compare/data/
+-rw-rw-r--   0 shailesh  (1000) shailesh  (1000)    10012 2023-08-07 19:02:28.000000 sckan-compare-0.0.4/sckan_compare/data/coords_human.json
+-rw-rw-r--   0 shailesh  (1000) shailesh  (1000)     4559 2023-08-07 15:59:15.000000 sckan-compare-0.0.4/sckan_compare/data/coords_mouse.json
+-rw-rw-r--   0 shailesh  (1000) shailesh  (1000)    21317 2023-08-07 19:02:28.000000 sckan-compare-0.0.4/sckan_compare/data/coords_rat.json
+-rw-rw-r--   0 shailesh  (1000) shailesh  (1000)       73 2023-08-07 09:47:01.000000 sckan-compare-0.0.4/sckan_compare/globals.py
+-rw-rw-r--   0 shailesh  (1000) shailesh  (1000)     7040 2023-08-07 14:46:14.000000 sckan-compare-0.0.4/sckan_compare/query.py
+-rw-rw-r--   0 shailesh  (1000) shailesh  (1000)     6482 2023-08-07 23:47:35.000000 sckan-compare-0.0.4/sckan_compare/simplevis.py
+-rw-rw-r--   0 shailesh  (1000) shailesh  (1000)     1138 2023-08-07 15:11:05.000000 sckan-compare-0.0.4/sckan_compare/utils.py
+-rw-rw-r--   0 shailesh  (1000) shailesh  (1000)    11307 2023-08-07 21:29:46.000000 sckan-compare-0.0.4/sckan_compare/visualize.py
+drwxrwxr-x   0 shailesh  (1000) shailesh  (1000)        0 2023-08-08 00:13:47.824215 sckan-compare-0.0.4/sckan_compare.egg-info/
+-rw-rw-r--   0 shailesh  (1000) shailesh  (1000)      412 2023-08-08 00:13:47.000000 sckan-compare-0.0.4/sckan_compare.egg-info/PKG-INFO
+-rw-rw-r--   0 shailesh  (1000) shailesh  (1000)      434 2023-08-08 00:13:47.000000 sckan-compare-0.0.4/sckan_compare.egg-info/SOURCES.txt
+-rw-rw-r--   0 shailesh  (1000) shailesh  (1000)        1 2023-08-08 00:13:47.000000 sckan-compare-0.0.4/sckan_compare.egg-info/dependency_links.txt
+-rw-rw-r--   0 shailesh  (1000) shailesh  (1000)       14 2023-08-08 00:13:47.000000 sckan-compare-0.0.4/sckan_compare.egg-info/top_level.txt
+-rw-rw-r--   0 shailesh  (1000) shailesh  (1000)       38 2023-08-08 00:13:47.824215 sckan-compare-0.0.4/setup.cfg
+-rw-rw-r--   0 shailesh  (1000) shailesh  (1000)      585 2023-08-08 00:13:27.000000 sckan-compare-0.0.4/setup.py
```

### Comparing `sckan-compare-0.0.3/LICENSE` & `sckan-compare-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `sckan-compare-0.0.3/README.md` & `sckan-compare-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `sckan-compare-0.0.3/sckan_compare/__init__.py` & `sckan-compare-0.0.4/sckan_compare/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 import pandas as pd
 
 from . import globals
 from . import query
 from .visualize import Visualizer
 
 
-class sckanCompare(object):
+class SckanCompare(object):
     """
     Base class for accessing functionality
     """
 
     def __init__(self, species="Homo sapiens", endpoint=globals.BLAZEGRAPH_ENDPOINT):
         self.endpoint = endpoint
         self.region_dict = {}
```

### Comparing `sckan-compare-0.0.3/sckan_compare/data/coords_human.json` & `sckan-compare-0.0.4/sckan_compare/data/coords_human.json`

 * *Files identical despite different names*

### Comparing `sckan-compare-0.0.3/sckan_compare/data/coords_mouse.json` & `sckan-compare-0.0.4/sckan_compare/data/coords_mouse.json`

 * *Files identical despite different names*

### Comparing `sckan-compare-0.0.3/sckan_compare/data/coords_rat.json` & `sckan-compare-0.0.4/sckan_compare/data/coords_rat.json`

 * *Files identical despite different names*

### Comparing `sckan-compare-0.0.3/sckan_compare/query.py` & `sckan-compare-0.0.4/sckan_compare/query.py`

 * *Files identical despite different names*

### Comparing `sckan-compare-0.0.3/sckan_compare/simplevis.py` & `sckan-compare-0.0.4/sckan_compare/simplevis.py`

 * *Files identical despite different names*

### Comparing `sckan-compare-0.0.3/sckan_compare/utils.py` & `sckan-compare-0.0.4/sckan_compare/utils.py`

 * *Files identical despite different names*

### Comparing `sckan-compare-0.0.3/sckan_compare/visualize.py` & `sckan-compare-0.0.4/sckan_compare/visualize.py`

 * *Files identical despite different names*

### Comparing `sckan-compare-0.0.3/setup.py` & `sckan-compare-0.0.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 Author: Shailesh Appukuttan
 Date: 07/08/2023
 """
 from setuptools import setup, find_packages
 
 setup(
     name="sckan-compare",
-    version="0.0.3",
+    version="0.0.4",
     description="A package for retrieving and visualizing data contained in     SCKAN (e.g., across species, relationship to spinal segments) to highlight similarities and differences in neuronal pathways",
     author="Shailesh Appukuttan, Hiba Ben Aribi, Pranjal Garg, Gautam Kumar",
     author_email="appukuttan.shailesh@gmail.com",
     license="Apache-2.0",
     package_data={'': ['data/*.json']},
     packages=find_packages(),
 )
```


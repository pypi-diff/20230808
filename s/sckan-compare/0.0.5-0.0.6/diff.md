# Comparing `tmp/sckan-compare-0.0.5.tar.gz` & `tmp/sckan-compare-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sckan-compare-0.0.5.tar", last modified: Tue Aug  8 00:18:06 2023, max compression
+gzip compressed data, was "sckan-compare-0.0.6.tar", last modified: Tue Aug  8 00:25:50 2023, max compression
```

## Comparing `sckan-compare-0.0.5.tar` & `sckan-compare-0.0.6.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxr-x   0 shailesh  (1000) shailesh  (1000)        0 2023-08-08 00:18:06.837507 sckan-compare-0.0.5/
--rw-rw-r--   0 shailesh  (1000) shailesh  (1000)    11356 2023-08-07 08:19:50.000000 sckan-compare-0.0.5/LICENSE
--rw-rw-r--   0 shailesh  (1000) shailesh  (1000)      412 2023-08-08 00:18:06.837507 sckan-compare-0.0.5/PKG-INFO
--rw-rw-r--   0 shailesh  (1000) shailesh  (1000)     3941 2023-08-07 23:54:51.000000 sckan-compare-0.0.5/README.md
-drwxrwxr-x   0 shailesh  (1000) shailesh  (1000)        0 2023-08-08 00:18:06.837507 sckan-compare-0.0.5/sckan_compare/
--rw-rw-r--   0 shailesh  (1000) shailesh  (1000)    14104 2023-08-08 00:08:37.000000 sckan-compare-0.0.5/sckan_compare/__init__.py
-drwxrwxr-x   0 shailesh  (1000) shailesh  (1000)        0 2023-08-08 00:18:06.837507 sckan-compare-0.0.5/sckan_compare/data/
--rw-rw-r--   0 shailesh  (1000) shailesh  (1000)    10012 2023-08-07 19:02:28.000000 sckan-compare-0.0.5/sckan_compare/data/coords_human.json
--rw-rw-r--   0 shailesh  (1000) shailesh  (1000)     4559 2023-08-07 15:59:15.000000 sckan-compare-0.0.5/sckan_compare/data/coords_mouse.json
--rw-rw-r--   0 shailesh  (1000) shailesh  (1000)    21317 2023-08-07 19:02:28.000000 sckan-compare-0.0.5/sckan_compare/data/coords_rat.json
--rw-rw-r--   0 shailesh  (1000) shailesh  (1000)     5874 2023-08-07 18:10:35.000000 sckan-compare-0.0.5/sckan_compare/data/node_A.png
--rw-rw-r--   0 shailesh  (1000) shailesh  (1000)     5805 2023-08-07 18:09:42.000000 sckan-compare-0.0.5/sckan_compare/data/node_B.png
--rw-rw-r--   0 shailesh  (1000) shailesh  (1000)     5128 2023-08-07 18:10:00.000000 sckan-compare-0.0.5/sckan_compare/data/node_C.png
--rw-rw-r--   0 shailesh  (1000) shailesh  (1000)       73 2023-08-07 09:47:01.000000 sckan-compare-0.0.5/sckan_compare/globals.py
--rw-rw-r--   0 shailesh  (1000) shailesh  (1000)     7040 2023-08-07 14:46:14.000000 sckan-compare-0.0.5/sckan_compare/query.py
--rw-rw-r--   0 shailesh  (1000) shailesh  (1000)     6482 2023-08-07 23:47:35.000000 sckan-compare-0.0.5/sckan_compare/simplevis.py
--rw-rw-r--   0 shailesh  (1000) shailesh  (1000)     1138 2023-08-07 15:11:05.000000 sckan-compare-0.0.5/sckan_compare/utils.py
--rw-rw-r--   0 shailesh  (1000) shailesh  (1000)    11307 2023-08-07 21:29:46.000000 sckan-compare-0.0.5/sckan_compare/visualize.py
-drwxrwxr-x   0 shailesh  (1000) shailesh  (1000)        0 2023-08-08 00:18:06.837507 sckan-compare-0.0.5/sckan_compare.egg-info/
--rw-rw-r--   0 shailesh  (1000) shailesh  (1000)      412 2023-08-08 00:18:06.000000 sckan-compare-0.0.5/sckan_compare.egg-info/PKG-INFO
--rw-rw-r--   0 shailesh  (1000) shailesh  (1000)      524 2023-08-08 00:18:06.000000 sckan-compare-0.0.5/sckan_compare.egg-info/SOURCES.txt
--rw-rw-r--   0 shailesh  (1000) shailesh  (1000)        1 2023-08-08 00:18:06.000000 sckan-compare-0.0.5/sckan_compare.egg-info/dependency_links.txt
--rw-rw-r--   0 shailesh  (1000) shailesh  (1000)       14 2023-08-08 00:18:06.000000 sckan-compare-0.0.5/sckan_compare.egg-info/top_level.txt
--rw-rw-r--   0 shailesh  (1000) shailesh  (1000)       38 2023-08-08 00:18:06.837507 sckan-compare-0.0.5/setup.cfg
--rw-rw-r--   0 shailesh  (1000) shailesh  (1000)      582 2023-08-08 00:17:08.000000 sckan-compare-0.0.5/setup.py
+drwxrwxr-x   0 shailesh  (1000) shailesh  (1000)        0 2023-08-08 00:25:50.215792 sckan-compare-0.0.6/
+-rw-rw-r--   0 shailesh  (1000) shailesh  (1000)    11356 2023-08-07 08:19:50.000000 sckan-compare-0.0.6/LICENSE
+-rw-rw-r--   0 shailesh  (1000) shailesh  (1000)      412 2023-08-08 00:25:50.211792 sckan-compare-0.0.6/PKG-INFO
+-rw-rw-r--   0 shailesh  (1000) shailesh  (1000)     3941 2023-08-07 23:54:51.000000 sckan-compare-0.0.6/README.md
+drwxrwxr-x   0 shailesh  (1000) shailesh  (1000)        0 2023-08-08 00:25:50.211792 sckan-compare-0.0.6/sckan_compare/
+-rw-rw-r--   0 shailesh  (1000) shailesh  (1000)    14104 2023-08-08 00:08:37.000000 sckan-compare-0.0.6/sckan_compare/__init__.py
+drwxrwxr-x   0 shailesh  (1000) shailesh  (1000)        0 2023-08-08 00:25:50.211792 sckan-compare-0.0.6/sckan_compare/data/
+-rw-rw-r--   0 shailesh  (1000) shailesh  (1000)    10012 2023-08-07 19:02:28.000000 sckan-compare-0.0.6/sckan_compare/data/coords_human.json
+-rw-rw-r--   0 shailesh  (1000) shailesh  (1000)     4559 2023-08-07 15:59:15.000000 sckan-compare-0.0.6/sckan_compare/data/coords_mouse.json
+-rw-rw-r--   0 shailesh  (1000) shailesh  (1000)    21317 2023-08-07 19:02:28.000000 sckan-compare-0.0.6/sckan_compare/data/coords_rat.json
+-rw-rw-r--   0 shailesh  (1000) shailesh  (1000)     5874 2023-08-07 18:10:35.000000 sckan-compare-0.0.6/sckan_compare/data/node_A.png
+-rw-rw-r--   0 shailesh  (1000) shailesh  (1000)     5805 2023-08-07 18:09:42.000000 sckan-compare-0.0.6/sckan_compare/data/node_B.png
+-rw-rw-r--   0 shailesh  (1000) shailesh  (1000)     5128 2023-08-07 18:10:00.000000 sckan-compare-0.0.6/sckan_compare/data/node_C.png
+-rw-rw-r--   0 shailesh  (1000) shailesh  (1000)       73 2023-08-07 09:47:01.000000 sckan-compare-0.0.6/sckan_compare/globals.py
+-rw-rw-r--   0 shailesh  (1000) shailesh  (1000)     7040 2023-08-07 14:46:14.000000 sckan-compare-0.0.6/sckan_compare/query.py
+-rw-rw-r--   0 shailesh  (1000) shailesh  (1000)     6508 2023-08-08 00:24:48.000000 sckan-compare-0.0.6/sckan_compare/simplevis.py
+-rw-rw-r--   0 shailesh  (1000) shailesh  (1000)     1138 2023-08-07 15:11:05.000000 sckan-compare-0.0.6/sckan_compare/utils.py
+-rw-rw-r--   0 shailesh  (1000) shailesh  (1000)    11307 2023-08-07 21:29:46.000000 sckan-compare-0.0.6/sckan_compare/visualize.py
+drwxrwxr-x   0 shailesh  (1000) shailesh  (1000)        0 2023-08-08 00:25:50.211792 sckan-compare-0.0.6/sckan_compare.egg-info/
+-rw-rw-r--   0 shailesh  (1000) shailesh  (1000)      412 2023-08-08 00:25:50.000000 sckan-compare-0.0.6/sckan_compare.egg-info/PKG-INFO
+-rw-rw-r--   0 shailesh  (1000) shailesh  (1000)      524 2023-08-08 00:25:50.000000 sckan-compare-0.0.6/sckan_compare.egg-info/SOURCES.txt
+-rw-rw-r--   0 shailesh  (1000) shailesh  (1000)        1 2023-08-08 00:25:50.000000 sckan-compare-0.0.6/sckan_compare.egg-info/dependency_links.txt
+-rw-rw-r--   0 shailesh  (1000) shailesh  (1000)       14 2023-08-08 00:25:50.000000 sckan-compare-0.0.6/sckan_compare.egg-info/top_level.txt
+-rw-rw-r--   0 shailesh  (1000) shailesh  (1000)       38 2023-08-08 00:25:50.215792 sckan-compare-0.0.6/setup.cfg
+-rw-rw-r--   0 shailesh  (1000) shailesh  (1000)      582 2023-08-08 00:25:47.000000 sckan-compare-0.0.6/setup.py
```

### Comparing `sckan-compare-0.0.5/LICENSE` & `sckan-compare-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `sckan-compare-0.0.5/README.md` & `sckan-compare-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `sckan-compare-0.0.5/sckan_compare/__init__.py` & `sckan-compare-0.0.6/sckan_compare/__init__.py`

 * *Files identical despite different names*

### Comparing `sckan-compare-0.0.5/sckan_compare/data/coords_human.json` & `sckan-compare-0.0.6/sckan_compare/data/coords_human.json`

 * *Files identical despite different names*

### Comparing `sckan-compare-0.0.5/sckan_compare/data/coords_mouse.json` & `sckan-compare-0.0.6/sckan_compare/data/coords_mouse.json`

 * *Files identical despite different names*

### Comparing `sckan-compare-0.0.5/sckan_compare/data/coords_rat.json` & `sckan-compare-0.0.6/sckan_compare/data/coords_rat.json`

 * *Files identical despite different names*

### Comparing `sckan-compare-0.0.5/sckan_compare/data/node_A.png` & `sckan-compare-0.0.6/sckan_compare/data/node_A.png`

 * *Files identical despite different names*

### Comparing `sckan-compare-0.0.5/sckan_compare/data/node_B.png` & `sckan-compare-0.0.6/sckan_compare/data/node_B.png`

 * *Files identical despite different names*

### Comparing `sckan-compare-0.0.5/sckan_compare/data/node_C.png` & `sckan-compare-0.0.6/sckan_compare/data/node_C.png`

 * *Files identical despite different names*

### Comparing `sckan-compare-0.0.5/sckan_compare/query.py` & `sckan-compare-0.0.6/sckan_compare/query.py`

 * *Files identical despite different names*

### Comparing `sckan-compare-0.0.5/sckan_compare/simplevis.py` & `sckan-compare-0.0.6/sckan_compare/simplevis.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,23 @@
+import os
+import pkg_resources
 import numpy as np
 import plotly.graph_objects as go
 from PIL import Image
 
 class SimpleVisualizer(object):
 
     def __init__(self):
         self.SCALE = 150
         self.MAX_Y = 900
 
-        node_A = Image.open("/home/shailesh/gits/2023-team-4/sckan_compare/data/node_A.png")
-        node_B = Image.open("/home/shailesh/gits/2023-team-4/sckan_compare/data/node_B.png")
-        node_C = Image.open("/home/shailesh/gits/2023-team-4/sckan_compare/data/node_C.png")
+        datapath = pkg_resources.resource_filename("sckan_compare", "data")
+        node_A = Image.open(os.path.join(datapath, "node_A.png"))
+        node_B = Image.open(os.path.join(datapath, "node_B.png"))
+        node_C = Image.open(os.path.join(datapath, "node_C.png"))
         self.icons = {
             "node_A": node_A,
             "node_B": node_B,
             "node_C": node_C
         }
 
         self.fig = go.FigureWidget()
```

### Comparing `sckan-compare-0.0.5/sckan_compare/utils.py` & `sckan-compare-0.0.6/sckan_compare/utils.py`

 * *Files identical despite different names*

### Comparing `sckan-compare-0.0.5/sckan_compare/visualize.py` & `sckan-compare-0.0.6/sckan_compare/visualize.py`

 * *Files identical despite different names*

### Comparing `sckan-compare-0.0.5/sckan_compare.egg-info/SOURCES.txt` & `sckan-compare-0.0.6/sckan_compare.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `sckan-compare-0.0.5/setup.py` & `sckan-compare-0.0.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 Author: Shailesh Appukuttan
 Date: 07/08/2023
 """
 from setuptools import setup, find_packages
 
 setup(
     name="sckan-compare",
-    version="0.0.5",
+    version="0.0.6",
     description="A package for retrieving and visualizing data contained in     SCKAN (e.g., across species, relationship to spinal segments) to highlight similarities and differences in neuronal pathways",
     author="Shailesh Appukuttan, Hiba Ben Aribi, Pranjal Garg, Gautam Kumar",
     author_email="appukuttan.shailesh@gmail.com",
     license="Apache-2.0",
     package_data={'': ['data/*.*']},
     packages=find_packages(),
 )
```


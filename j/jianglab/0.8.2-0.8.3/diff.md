# Comparing `tmp/jianglab-0.8.2.tar.gz` & `tmp/jianglab-0.8.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jianglab-0.8.2.tar", last modified: Tue Aug  8 15:25:01 2023, max compression
+gzip compressed data, was "jianglab-0.8.3.tar", last modified: Tue Aug  8 15:28:48 2023, max compression
```

## Comparing `jianglab-0.8.2.tar` & `jianglab-0.8.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 zhengjiang   (501) staff       (20)        0 2023-08-08 15:25:01.582147 jianglab-0.8.2/
--rw-r--r--   0 zhengjiang   (501) staff       (20)      644 2023-08-08 15:25:01.581782 jianglab-0.8.2/PKG-INFO
--rw-r--r--   0 zhengjiang   (501) staff       (20)     1176 2023-07-12 19:29:04.000000 jianglab-0.8.2/README.md
-drwxr-xr-x   0 zhengjiang   (501) staff       (20)        0 2023-08-08 15:25:01.578800 jianglab-0.8.2/jianglab/
--rw-r--r--   0 zhengjiang   (501) staff       (20)       76 2023-05-30 15:41:31.000000 jianglab-0.8.2/jianglab/__init__.py
--rw-r--r--   0 zhengjiang   (501) staff       (20)    50520 2023-08-07 17:40:56.000000 jianglab-0.8.2/jianglab/common_functions.py
--rw-r--r--   0 zhengjiang   (501) staff       (20)      400 2023-05-30 15:41:33.000000 jianglab-0.8.2/jianglab/params.py
-drwxr-xr-x   0 zhengjiang   (501) staff       (20)        0 2023-08-08 15:25:01.581278 jianglab-0.8.2/jianglab.egg-info/
--rw-r--r--   0 zhengjiang   (501) staff       (20)      644 2023-08-08 15:25:01.000000 jianglab-0.8.2/jianglab.egg-info/PKG-INFO
--rw-r--r--   0 zhengjiang   (501) staff       (20)      246 2023-08-08 15:25:01.000000 jianglab-0.8.2/jianglab.egg-info/SOURCES.txt
--rw-r--r--   0 zhengjiang   (501) staff       (20)        1 2023-08-08 15:25:01.000000 jianglab-0.8.2/jianglab.egg-info/dependency_links.txt
--rw-r--r--   0 zhengjiang   (501) staff       (20)      168 2023-08-08 15:25:01.000000 jianglab-0.8.2/jianglab.egg-info/requires.txt
--rw-r--r--   0 zhengjiang   (501) staff       (20)        9 2023-08-08 15:25:01.000000 jianglab-0.8.2/jianglab.egg-info/top_level.txt
--rw-r--r--   0 zhengjiang   (501) staff       (20)       38 2023-08-08 15:25:01.582287 jianglab-0.8.2/setup.cfg
--rw-r--r--   0 zhengjiang   (501) staff       (20)     1162 2023-08-08 15:24:56.000000 jianglab-0.8.2/setup.py
+drwxr-xr-x   0 zhengjiang   (501) staff       (20)        0 2023-08-08 15:28:48.123522 jianglab-0.8.3/
+-rw-r--r--   0 zhengjiang   (501) staff       (20)      644 2023-08-08 15:28:48.123205 jianglab-0.8.3/PKG-INFO
+-rw-r--r--   0 zhengjiang   (501) staff       (20)     1176 2023-07-12 19:29:04.000000 jianglab-0.8.3/README.md
+drwxr-xr-x   0 zhengjiang   (501) staff       (20)        0 2023-08-08 15:28:48.119420 jianglab-0.8.3/jianglab/
+-rw-r--r--   0 zhengjiang   (501) staff       (20)       76 2023-05-30 15:41:31.000000 jianglab-0.8.3/jianglab/__init__.py
+-rw-r--r--   0 zhengjiang   (501) staff       (20)    50592 2023-08-08 15:28:29.000000 jianglab-0.8.3/jianglab/common_functions.py
+-rw-r--r--   0 zhengjiang   (501) staff       (20)      400 2023-05-30 15:41:33.000000 jianglab-0.8.3/jianglab/params.py
+drwxr-xr-x   0 zhengjiang   (501) staff       (20)        0 2023-08-08 15:28:48.122708 jianglab-0.8.3/jianglab.egg-info/
+-rw-r--r--   0 zhengjiang   (501) staff       (20)      644 2023-08-08 15:28:47.000000 jianglab-0.8.3/jianglab.egg-info/PKG-INFO
+-rw-r--r--   0 zhengjiang   (501) staff       (20)      246 2023-08-08 15:28:48.000000 jianglab-0.8.3/jianglab.egg-info/SOURCES.txt
+-rw-r--r--   0 zhengjiang   (501) staff       (20)        1 2023-08-08 15:28:47.000000 jianglab-0.8.3/jianglab.egg-info/dependency_links.txt
+-rw-r--r--   0 zhengjiang   (501) staff       (20)      168 2023-08-08 15:28:47.000000 jianglab-0.8.3/jianglab.egg-info/requires.txt
+-rw-r--r--   0 zhengjiang   (501) staff       (20)        9 2023-08-08 15:28:47.000000 jianglab-0.8.3/jianglab.egg-info/top_level.txt
+-rw-r--r--   0 zhengjiang   (501) staff       (20)       38 2023-08-08 15:28:48.123647 jianglab-0.8.3/setup.cfg
+-rw-r--r--   0 zhengjiang   (501) staff       (20)     1162 2023-08-08 15:28:35.000000 jianglab-0.8.3/setup.py
```

### Comparing `jianglab-0.8.2/PKG-INFO` & `jianglab-0.8.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jianglab
-Version: 0.8.2
+Version: 0.8.3
 Summary: A package for Jiang lab
 Home-page: https://github.com/jiang-lab-retina/jianglab.git
 Author: Jiang Zheng
 Author-email: zjiang314@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `jianglab-0.8.2/README.md` & `jianglab-0.8.3/README.md`

 * *Files identical despite different names*

### Comparing `jianglab-0.8.2/jianglab/common_functions.py` & `jianglab-0.8.3/jianglab/common_functions.py`

 * *Files 1% similar despite different names*

```diff
@@ -362,14 +362,16 @@
     if pd.isna(bad_lanes).any():
         bad_lanes = []
         print("No bad lanes found")
     # elif len(bad_lanes) == 1:
     #     bad_lanes = bad_lanes
     elif list(bad_lanes)[0] == "":
         bad_lanes = []
+    elif len(list(bad_lanes)) == 1:
+        bad_lanes = list(bad_lanes)
     else:                      
         bad_lanes = [int(x) for x in list(bad_lanes)[0].split(",")]
     return bad_lanes
 
 def clean_centers_all_process(arr, neighbour_size = (6,6,6)):
     def find_3d_local_min_general(arr, neighbor_size = (6,6,6)):
         if arr.shape[0] != 0:
```

### Comparing `jianglab-0.8.2/jianglab.egg-info/PKG-INFO` & `jianglab-0.8.3/jianglab.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jianglab
-Version: 0.8.2
+Version: 0.8.3
 Summary: A package for Jiang lab
 Home-page: https://github.com/jiang-lab-retina/jianglab.git
 Author: Jiang Zheng
 Author-email: zjiang314@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `jianglab-0.8.2/setup.py` & `jianglab-0.8.3/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='jianglab',
-    version='0.8.2',
+    version='0.8.3',
     packages=find_packages(),
     install_requires=[
         "numpy",
         "pandas",
         "matplotlib",
         "treelib",
         "McsPyDataTools",
```


# Comparing `tmp/jianglab-0.8.3.tar.gz` & `tmp/jianglab-0.8.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jianglab-0.8.3.tar", last modified: Tue Aug  8 15:28:48 2023, max compression
+gzip compressed data, was "jianglab-0.8.4.tar", last modified: Tue Aug  8 19:15:21 2023, max compression
```

## Comparing `jianglab-0.8.3.tar` & `jianglab-0.8.4.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 zhengjiang   (501) staff       (20)        0 2023-08-08 15:28:48.123522 jianglab-0.8.3/
--rw-r--r--   0 zhengjiang   (501) staff       (20)      644 2023-08-08 15:28:48.123205 jianglab-0.8.3/PKG-INFO
--rw-r--r--   0 zhengjiang   (501) staff       (20)     1176 2023-07-12 19:29:04.000000 jianglab-0.8.3/README.md
-drwxr-xr-x   0 zhengjiang   (501) staff       (20)        0 2023-08-08 15:28:48.119420 jianglab-0.8.3/jianglab/
--rw-r--r--   0 zhengjiang   (501) staff       (20)       76 2023-05-30 15:41:31.000000 jianglab-0.8.3/jianglab/__init__.py
--rw-r--r--   0 zhengjiang   (501) staff       (20)    50592 2023-08-08 15:28:29.000000 jianglab-0.8.3/jianglab/common_functions.py
--rw-r--r--   0 zhengjiang   (501) staff       (20)      400 2023-05-30 15:41:33.000000 jianglab-0.8.3/jianglab/params.py
-drwxr-xr-x   0 zhengjiang   (501) staff       (20)        0 2023-08-08 15:28:48.122708 jianglab-0.8.3/jianglab.egg-info/
--rw-r--r--   0 zhengjiang   (501) staff       (20)      644 2023-08-08 15:28:47.000000 jianglab-0.8.3/jianglab.egg-info/PKG-INFO
--rw-r--r--   0 zhengjiang   (501) staff       (20)      246 2023-08-08 15:28:48.000000 jianglab-0.8.3/jianglab.egg-info/SOURCES.txt
--rw-r--r--   0 zhengjiang   (501) staff       (20)        1 2023-08-08 15:28:47.000000 jianglab-0.8.3/jianglab.egg-info/dependency_links.txt
--rw-r--r--   0 zhengjiang   (501) staff       (20)      168 2023-08-08 15:28:47.000000 jianglab-0.8.3/jianglab.egg-info/requires.txt
--rw-r--r--   0 zhengjiang   (501) staff       (20)        9 2023-08-08 15:28:47.000000 jianglab-0.8.3/jianglab.egg-info/top_level.txt
--rw-r--r--   0 zhengjiang   (501) staff       (20)       38 2023-08-08 15:28:48.123647 jianglab-0.8.3/setup.cfg
--rw-r--r--   0 zhengjiang   (501) staff       (20)     1162 2023-08-08 15:28:35.000000 jianglab-0.8.3/setup.py
+drwxr-xr-x   0 zhengjiang   (501) staff       (20)        0 2023-08-08 19:15:21.679844 jianglab-0.8.4/
+-rw-r--r--   0 zhengjiang   (501) staff       (20)      644 2023-08-08 19:15:21.679169 jianglab-0.8.4/PKG-INFO
+-rw-r--r--   0 zhengjiang   (501) staff       (20)     1176 2023-07-12 19:29:04.000000 jianglab-0.8.4/README.md
+drwxr-xr-x   0 zhengjiang   (501) staff       (20)        0 2023-08-08 19:15:21.674735 jianglab-0.8.4/jianglab/
+-rw-r--r--   0 zhengjiang   (501) staff       (20)       76 2023-05-30 15:41:31.000000 jianglab-0.8.4/jianglab/__init__.py
+-rw-r--r--   0 zhengjiang   (501) staff       (20)    50698 2023-08-08 19:15:05.000000 jianglab-0.8.4/jianglab/common_functions.py
+-rw-r--r--   0 zhengjiang   (501) staff       (20)      400 2023-05-30 15:41:33.000000 jianglab-0.8.4/jianglab/params.py
+drwxr-xr-x   0 zhengjiang   (501) staff       (20)        0 2023-08-08 19:15:21.678261 jianglab-0.8.4/jianglab.egg-info/
+-rw-r--r--   0 zhengjiang   (501) staff       (20)      644 2023-08-08 19:15:21.000000 jianglab-0.8.4/jianglab.egg-info/PKG-INFO
+-rw-r--r--   0 zhengjiang   (501) staff       (20)      246 2023-08-08 19:15:21.000000 jianglab-0.8.4/jianglab.egg-info/SOURCES.txt
+-rw-r--r--   0 zhengjiang   (501) staff       (20)        1 2023-08-08 19:15:21.000000 jianglab-0.8.4/jianglab.egg-info/dependency_links.txt
+-rw-r--r--   0 zhengjiang   (501) staff       (20)      168 2023-08-08 19:15:21.000000 jianglab-0.8.4/jianglab.egg-info/requires.txt
+-rw-r--r--   0 zhengjiang   (501) staff       (20)        9 2023-08-08 19:15:21.000000 jianglab-0.8.4/jianglab.egg-info/top_level.txt
+-rw-r--r--   0 zhengjiang   (501) staff       (20)       38 2023-08-08 19:15:21.680120 jianglab-0.8.4/setup.cfg
+-rw-r--r--   0 zhengjiang   (501) staff       (20)     1162 2023-08-08 19:15:16.000000 jianglab-0.8.4/setup.py
```

### Comparing `jianglab-0.8.3/PKG-INFO` & `jianglab-0.8.4/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jianglab
-Version: 0.8.3
+Version: 0.8.4
 Summary: A package for Jiang lab
 Home-page: https://github.com/jiang-lab-retina/jianglab.git
 Author: Jiang Zheng
 Author-email: zjiang314@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `jianglab-0.8.3/README.md` & `jianglab-0.8.4/README.md`

 * *Files identical despite different names*

### Comparing `jianglab-0.8.3/jianglab/common_functions.py` & `jianglab-0.8.4/jianglab/common_functions.py`

 * *Files 1% similar despite different names*

```diff
@@ -351,28 +351,31 @@
     with open(filename, "wb") as file_:
         pickle.dump(instance, file_, -1)
 
 def load_instance(filename):
     return pickle.load(open(filename, "rb", -1))
 
 def get_bad_lanes(cmcr_file_path):
-    gsheet = import_gsheet()
+    gsheet = jl.import_gsheet()
     bad_lanes = cmcr_file_path.split("\\")[-1].replace("-",".").split(".")[:6]
     bad_lanes = ".".join(bad_lanes)
     bad_lanes = gsheet[gsheet.File_name.str.contains(bad_lanes)]["Bad_lanes"]
+    #print(list(bad_lanes))
     if pd.isna(bad_lanes).any():
         bad_lanes = []
         print("No bad lanes found")
     # elif len(bad_lanes) == 1:
     #     bad_lanes = bad_lanes
-    elif list(bad_lanes)[0] == "":
+    elif list(bad_lanes) == "":
         bad_lanes = []
-    elif len(list(bad_lanes)) == 1:
-        bad_lanes = list(bad_lanes)
-    else:                      
+    elif "," not in str(list(bad_lanes)[0]):
+        bad_lanes = list(bad_lanes)[0]
+        bad_lanes = [bad_lanes]
+    else:              
+        print(list(bad_lanes)[0])        
         bad_lanes = [int(x) for x in list(bad_lanes)[0].split(",")]
     return bad_lanes
 
 def clean_centers_all_process(arr, neighbour_size = (6,6,6)):
     def find_3d_local_min_general(arr, neighbor_size = (6,6,6)):
         if arr.shape[0] != 0:
             counter = 0
```

### Comparing `jianglab-0.8.3/jianglab.egg-info/PKG-INFO` & `jianglab-0.8.4/jianglab.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jianglab
-Version: 0.8.3
+Version: 0.8.4
 Summary: A package for Jiang lab
 Home-page: https://github.com/jiang-lab-retina/jianglab.git
 Author: Jiang Zheng
 Author-email: zjiang314@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `jianglab-0.8.3/setup.py` & `jianglab-0.8.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='jianglab',
-    version='0.8.3',
+    version='0.8.4',
     packages=find_packages(),
     install_requires=[
         "numpy",
         "pandas",
         "matplotlib",
         "treelib",
         "McsPyDataTools",
```


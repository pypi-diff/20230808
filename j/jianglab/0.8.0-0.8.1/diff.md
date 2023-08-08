# Comparing `tmp/jianglab-0.8.0.tar.gz` & `tmp/jianglab-0.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jianglab-0.8.0.tar", last modified: Mon Aug  7 17:14:06 2023, max compression
+gzip compressed data, was "jianglab-0.8.1.tar", last modified: Mon Aug  7 17:35:01 2023, max compression
```

## Comparing `jianglab-0.8.0.tar` & `jianglab-0.8.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 zhengjiang   (501) staff       (20)        0 2023-08-07 17:14:06.792295 jianglab-0.8.0/
--rw-r--r--   0 zhengjiang   (501) staff       (20)      644 2023-08-07 17:14:06.791972 jianglab-0.8.0/PKG-INFO
--rw-r--r--   0 zhengjiang   (501) staff       (20)     1176 2023-07-12 19:29:04.000000 jianglab-0.8.0/README.md
-drwxr-xr-x   0 zhengjiang   (501) staff       (20)        0 2023-08-07 17:14:06.788652 jianglab-0.8.0/jianglab/
--rw-r--r--   0 zhengjiang   (501) staff       (20)       76 2023-05-30 15:41:31.000000 jianglab-0.8.0/jianglab/__init__.py
--rw-r--r--   0 zhengjiang   (501) staff       (20)    50330 2023-08-07 17:13:50.000000 jianglab-0.8.0/jianglab/common_functions.py
--rw-r--r--   0 zhengjiang   (501) staff       (20)      400 2023-05-30 15:41:33.000000 jianglab-0.8.0/jianglab/params.py
-drwxr-xr-x   0 zhengjiang   (501) staff       (20)        0 2023-08-07 17:14:06.791479 jianglab-0.8.0/jianglab.egg-info/
--rw-r--r--   0 zhengjiang   (501) staff       (20)      644 2023-08-07 17:14:06.000000 jianglab-0.8.0/jianglab.egg-info/PKG-INFO
--rw-r--r--   0 zhengjiang   (501) staff       (20)      246 2023-08-07 17:14:06.000000 jianglab-0.8.0/jianglab.egg-info/SOURCES.txt
--rw-r--r--   0 zhengjiang   (501) staff       (20)        1 2023-08-07 17:14:06.000000 jianglab-0.8.0/jianglab.egg-info/dependency_links.txt
--rw-r--r--   0 zhengjiang   (501) staff       (20)      168 2023-08-07 17:14:06.000000 jianglab-0.8.0/jianglab.egg-info/requires.txt
--rw-r--r--   0 zhengjiang   (501) staff       (20)        9 2023-08-07 17:14:06.000000 jianglab-0.8.0/jianglab.egg-info/top_level.txt
--rw-r--r--   0 zhengjiang   (501) staff       (20)       38 2023-08-07 17:14:06.792416 jianglab-0.8.0/setup.cfg
--rw-r--r--   0 zhengjiang   (501) staff       (20)     1162 2023-08-07 17:13:57.000000 jianglab-0.8.0/setup.py
+drwxr-xr-x   0 zhengjiang   (501) staff       (20)        0 2023-08-07 17:35:01.656036 jianglab-0.8.1/
+-rw-r--r--   0 zhengjiang   (501) staff       (20)      644 2023-08-07 17:35:01.655757 jianglab-0.8.1/PKG-INFO
+-rw-r--r--   0 zhengjiang   (501) staff       (20)     1176 2023-07-12 19:29:04.000000 jianglab-0.8.1/README.md
+drwxr-xr-x   0 zhengjiang   (501) staff       (20)        0 2023-08-07 17:35:01.652825 jianglab-0.8.1/jianglab/
+-rw-r--r--   0 zhengjiang   (501) staff       (20)       76 2023-05-30 15:41:31.000000 jianglab-0.8.1/jianglab/__init__.py
+-rw-r--r--   0 zhengjiang   (501) staff       (20)    50266 2023-08-07 17:34:48.000000 jianglab-0.8.1/jianglab/common_functions.py
+-rw-r--r--   0 zhengjiang   (501) staff       (20)      400 2023-05-30 15:41:33.000000 jianglab-0.8.1/jianglab/params.py
+drwxr-xr-x   0 zhengjiang   (501) staff       (20)        0 2023-08-07 17:35:01.655352 jianglab-0.8.1/jianglab.egg-info/
+-rw-r--r--   0 zhengjiang   (501) staff       (20)      644 2023-08-07 17:35:01.000000 jianglab-0.8.1/jianglab.egg-info/PKG-INFO
+-rw-r--r--   0 zhengjiang   (501) staff       (20)      246 2023-08-07 17:35:01.000000 jianglab-0.8.1/jianglab.egg-info/SOURCES.txt
+-rw-r--r--   0 zhengjiang   (501) staff       (20)        1 2023-08-07 17:35:01.000000 jianglab-0.8.1/jianglab.egg-info/dependency_links.txt
+-rw-r--r--   0 zhengjiang   (501) staff       (20)      168 2023-08-07 17:35:01.000000 jianglab-0.8.1/jianglab.egg-info/requires.txt
+-rw-r--r--   0 zhengjiang   (501) staff       (20)        9 2023-08-07 17:35:01.000000 jianglab-0.8.1/jianglab.egg-info/top_level.txt
+-rw-r--r--   0 zhengjiang   (501) staff       (20)       38 2023-08-07 17:35:01.656133 jianglab-0.8.1/setup.cfg
+-rw-r--r--   0 zhengjiang   (501) staff       (20)     1162 2023-08-07 17:34:54.000000 jianglab-0.8.1/setup.py
```

### Comparing `jianglab-0.8.0/PKG-INFO` & `jianglab-0.8.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jianglab
-Version: 0.8.0
+Version: 0.8.1
 Summary: A package for Jiang lab
 Home-page: https://github.com/jiang-lab-retina/jianglab.git
 Author: Jiang Zheng
 Author-email: zjiang314@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `jianglab-0.8.0/README.md` & `jianglab-0.8.1/README.md`

 * *Files identical despite different names*

### Comparing `jianglab-0.8.0/jianglab/common_functions.py` & `jianglab-0.8.1/jianglab/common_functions.py`

 * *Files 0% similar despite different names*

```diff
@@ -1228,15 +1228,14 @@
     if type(exclude_list) == str:
         exclude_list = [exclude_list]
     if recursive:
         files = glob.glob(location + '/**/*', recursive=True)
     else:
         files = glob.glob(location + '/*', recursive=False)
     final_files = []
-    for keyword in keyword_list:
-        final_files.append([f for f in files if keyword in f])
-    final_files = final_files[0]
-        #print(final_files)
+    for file in files:
+        if all(keyword in file for keyword in keyword_list):
+            final_files.append(file)
     for exclude_word in exclude_list:
-        #print(exclude_word)
+
         final_files = [f for f in final_files if exclude_word not in f]
     return final_files
```

### Comparing `jianglab-0.8.0/jianglab.egg-info/PKG-INFO` & `jianglab-0.8.1/jianglab.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jianglab
-Version: 0.8.0
+Version: 0.8.1
 Summary: A package for Jiang lab
 Home-page: https://github.com/jiang-lab-retina/jianglab.git
 Author: Jiang Zheng
 Author-email: zjiang314@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `jianglab-0.8.0/setup.py` & `jianglab-0.8.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='jianglab',
-    version='0.8.0',
+    version='0.8.1',
     packages=find_packages(),
     install_requires=[
         "numpy",
         "pandas",
         "matplotlib",
         "treelib",
         "McsPyDataTools",
```


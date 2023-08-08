# Comparing `tmp/bayesim-0.9.8.tar.gz` & `tmp/bayesim-0.9.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/bayesim-0.9.8.tar", last modified: Thu May 30 18:50:12 2019, max compression
+gzip compressed data, was "dist/bayesim-0.9.9.tar", last modified: Thu May 30 18:53:59 2019, max compression
```

## Comparing `bayesim-0.9.8.tar` & `bayesim-0.9.9.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 rachelkurchin   (501) staff       (20)        0 2019-05-30 18:50:12.000000 bayesim-0.9.8/
--rw-r--r--   0 rachelkurchin   (501) staff       (20)     1075 2019-05-30 18:50:12.000000 bayesim-0.9.8/PKG-INFO
--rw-r--r--   0 rachelkurchin   (501) staff       (20)      601 2019-05-30 18:50:00.000000 bayesim-0.9.8/README.rst
-drwxr-xr-x   0 rachelkurchin   (501) staff       (20)        0 2019-05-30 18:50:12.000000 bayesim-0.9.8/bayesim/
--rw-r--r--   0 rachelkurchin   (501) staff       (20)        0 2018-08-30 19:23:54.000000 bayesim-0.9.8/bayesim/__init__.py
--rw-r--r--   0 rachelkurchin   (501) staff       (20)     2898 2018-08-01 15:50:07.000000 bayesim-0.9.8/bayesim/__main__.py
--rw-r--r--   0 rachelkurchin   (501) staff       (20)    49354 2018-12-20 17:21:02.000000 bayesim-0.9.8/bayesim/model.py
--rw-r--r--   0 rachelkurchin   (501) staff       (20)    17716 2018-08-16 19:55:01.000000 bayesim-0.9.8/bayesim/params.py
--rw-r--r--   0 rachelkurchin   (501) staff       (20)    39170 2019-05-30 18:11:12.000000 bayesim-0.9.8/bayesim/pmf.py
--rw-r--r--   0 rachelkurchin   (501) staff       (20)    10788 2019-05-30 18:07:21.000000 bayesim-0.9.8/bayesim/utils.py
-drwxr-xr-x   0 rachelkurchin   (501) staff       (20)        0 2019-05-30 18:50:12.000000 bayesim-0.9.8/bayesim.egg-info/
--rw-r--r--   0 rachelkurchin   (501) staff       (20)     1075 2019-05-30 18:50:11.000000 bayesim-0.9.8/bayesim.egg-info/PKG-INFO
--rw-r--r--   0 rachelkurchin   (501) staff       (20)      344 2019-05-30 18:50:11.000000 bayesim-0.9.8/bayesim.egg-info/SOURCES.txt
--rw-r--r--   0 rachelkurchin   (501) staff       (20)       72 2019-05-30 18:50:11.000000 bayesim-0.9.8/bayesim.egg-info/dependency_links.txt
--rw-r--r--   0 rachelkurchin   (501) staff       (20)       51 2019-05-30 18:50:11.000000 bayesim-0.9.8/bayesim.egg-info/entry_points.txt
--rw-r--r--   0 rachelkurchin   (501) staff       (20)        1 2018-07-30 18:58:07.000000 bayesim-0.9.8/bayesim.egg-info/not-zip-safe
--rw-r--r--   0 rachelkurchin   (501) staff       (20)       46 2019-05-30 18:50:11.000000 bayesim-0.9.8/bayesim.egg-info/requires.txt
--rw-r--r--   0 rachelkurchin   (501) staff       (20)        8 2019-05-30 18:50:11.000000 bayesim-0.9.8/bayesim.egg-info/top_level.txt
--rw-r--r--   0 rachelkurchin   (501) staff       (20)       38 2019-05-30 18:50:12.000000 bayesim-0.9.8/setup.cfg
--rw-r--r--   0 rachelkurchin   (501) staff       (20)      886 2019-05-30 18:49:53.000000 bayesim-0.9.8/setup.py
+drwxr-xr-x   0 rachelkurchin   (501) staff       (20)        0 2019-05-30 18:53:59.000000 bayesim-0.9.9/
+-rw-r--r--   0 rachelkurchin   (501) staff       (20)     1075 2019-05-30 18:53:59.000000 bayesim-0.9.9/PKG-INFO
+-rw-r--r--   0 rachelkurchin   (501) staff       (20)      601 2019-05-30 18:50:00.000000 bayesim-0.9.9/README.rst
+drwxr-xr-x   0 rachelkurchin   (501) staff       (20)        0 2019-05-30 18:53:59.000000 bayesim-0.9.9/bayesim/
+-rw-r--r--   0 rachelkurchin   (501) staff       (20)        0 2018-08-30 19:23:54.000000 bayesim-0.9.9/bayesim/__init__.py
+-rw-r--r--   0 rachelkurchin   (501) staff       (20)     2898 2018-08-01 15:50:07.000000 bayesim-0.9.9/bayesim/__main__.py
+-rw-r--r--   0 rachelkurchin   (501) staff       (20)    49354 2018-12-20 17:21:02.000000 bayesim-0.9.9/bayesim/model.py
+-rw-r--r--   0 rachelkurchin   (501) staff       (20)    17716 2018-08-16 19:55:01.000000 bayesim-0.9.9/bayesim/params.py
+-rw-r--r--   0 rachelkurchin   (501) staff       (20)    39170 2019-05-30 18:11:12.000000 bayesim-0.9.9/bayesim/pmf.py
+-rw-r--r--   0 rachelkurchin   (501) staff       (20)    10788 2019-05-30 18:07:21.000000 bayesim-0.9.9/bayesim/utils.py
+drwxr-xr-x   0 rachelkurchin   (501) staff       (20)        0 2019-05-30 18:53:59.000000 bayesim-0.9.9/bayesim.egg-info/
+-rw-r--r--   0 rachelkurchin   (501) staff       (20)     1075 2019-05-30 18:53:59.000000 bayesim-0.9.9/bayesim.egg-info/PKG-INFO
+-rw-r--r--   0 rachelkurchin   (501) staff       (20)      344 2019-05-30 18:53:59.000000 bayesim-0.9.9/bayesim.egg-info/SOURCES.txt
+-rw-r--r--   0 rachelkurchin   (501) staff       (20)       72 2019-05-30 18:53:59.000000 bayesim-0.9.9/bayesim.egg-info/dependency_links.txt
+-rw-r--r--   0 rachelkurchin   (501) staff       (20)       51 2019-05-30 18:53:59.000000 bayesim-0.9.9/bayesim.egg-info/entry_points.txt
+-rw-r--r--   0 rachelkurchin   (501) staff       (20)        1 2018-07-30 18:58:07.000000 bayesim-0.9.9/bayesim.egg-info/not-zip-safe
+-rw-r--r--   0 rachelkurchin   (501) staff       (20)       46 2019-05-30 18:53:59.000000 bayesim-0.9.9/bayesim.egg-info/requires.txt
+-rw-r--r--   0 rachelkurchin   (501) staff       (20)        8 2019-05-30 18:53:59.000000 bayesim-0.9.9/bayesim.egg-info/top_level.txt
+-rw-r--r--   0 rachelkurchin   (501) staff       (20)       38 2019-05-30 18:53:59.000000 bayesim-0.9.9/setup.cfg
+-rw-r--r--   0 rachelkurchin   (501) staff       (20)      886 2019-05-30 18:52:31.000000 bayesim-0.9.9/setup.py
```

### Comparing `bayesim-0.9.8/PKG-INFO` & `bayesim-0.9.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: bayesim
-Version: 0.9.8
+Version: 0.9.9
 Summary: Fast model fitting via Bayesian inference
 Home-page: UNKNOWN
 Author: Rachel Kurchin, Giuseppe Romano
 Author-email: rkurchin@mit.edu, romanog@mit.edu
 License: GPLv2
 Description: Description
         ===========
@@ -25,8 +25,8 @@
         ===========
         :Authors:
             Rachel C. Kurchin and Giuseppe Romano
         
         :Version: 0.9.8 as of May 2019
         
 Platform: UNKNOWN
-Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
```

### Comparing `bayesim-0.9.8/README.rst` & `bayesim-0.9.9/README.rst`

 * *Files identical despite different names*

### Comparing `bayesim-0.9.8/bayesim/__main__.py` & `bayesim-0.9.9/bayesim/__main__.py`

 * *Files identical despite different names*

### Comparing `bayesim-0.9.8/bayesim/model.py` & `bayesim-0.9.9/bayesim/model.py`

 * *Files identical despite different names*

### Comparing `bayesim-0.9.8/bayesim/params.py` & `bayesim-0.9.9/bayesim/params.py`

 * *Files identical despite different names*

### Comparing `bayesim-0.9.8/bayesim/pmf.py` & `bayesim-0.9.9/bayesim/pmf.py`

 * *Files identical despite different names*

### Comparing `bayesim-0.9.8/bayesim/utils.py` & `bayesim-0.9.9/bayesim/utils.py`

 * *Files identical despite different names*

### Comparing `bayesim-0.9.8/bayesim.egg-info/PKG-INFO` & `bayesim-0.9.9/bayesim.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: bayesim
-Version: 0.9.8
+Version: 0.9.9
 Summary: Fast model fitting via Bayesian inference
 Home-page: UNKNOWN
 Author: Rachel Kurchin, Giuseppe Romano
 Author-email: rkurchin@mit.edu, romanog@mit.edu
 License: GPLv2
 Description: Description
         ===========
@@ -25,8 +25,8 @@
         ===========
         :Authors:
             Rachel C. Kurchin and Giuseppe Romano
         
         :Version: 0.9.8 as of May 2019
         
 Platform: UNKNOWN
-Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
```

### Comparing `bayesim-0.9.8/setup.py` & `bayesim-0.9.9/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from setuptools import setup, find_packages
 import os
 
 setup(name='bayesim',
-      version='0.9.8',
+      version='0.9.9',
       description='Fast model fitting via Bayesian inference',
       author='Rachel Kurchin, Giuseppe Romano',
       author_email='rkurchin@mit.edu, romanog@mit.edu',
-      classifiers=['Programming Language :: Python :: 3.6'],
+      classifiers=['Programming Language :: Python :: 3.7'],
       long_description=open('README.rst').read(),
       install_requires=['pandas',
                         'deepdish',
                         'numpy',
                         'scipy',
                         'matplotlib',
                         'joblib'
```


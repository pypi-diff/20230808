# Comparing `tmp/avijit1996iiti_basic_calculator-0.0.2.tar.gz` & `tmp/avijit1996iiti_basic_calculator-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "avijit1996iiti_basic_calculator-0.0.2.tar", last modified: Sun Aug  6 11:11:47 2023, max compression
+gzip compressed data, was "avijit1996iiti_basic_calculator-0.0.3.tar", last modified: Tue Aug  8 12:05:09 2023, max compression
```

## Comparing `avijit1996iiti_basic_calculator-0.0.2.tar` & `avijit1996iiti_basic_calculator-0.0.3.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxr-x   0 avijit    (1000) avijit    (1000)        0 2023-08-06 11:11:47.654969 avijit1996iiti_basic_calculator-0.0.2/
--rw-rw-r--   0 avijit    (1000) avijit    (1000)       51 2023-08-06 09:11:25.000000 avijit1996iiti_basic_calculator-0.0.2/CHANGELOG.txt
--rw-rw-r--   0 avijit    (1000) avijit    (1000)     1077 2023-08-06 08:42:59.000000 avijit1996iiti_basic_calculator-0.0.2/LICENSE.txt
--rw-rw-r--   0 avijit    (1000) avijit    (1000)       25 2023-08-06 09:19:26.000000 avijit1996iiti_basic_calculator-0.0.2/MANIFEST.in
--rw-rw-r--   0 avijit    (1000) avijit    (1000)      599 2023-08-06 11:11:47.654969 avijit1996iiti_basic_calculator-0.0.2/PKG-INFO
--rw-rw-r--   0 avijit    (1000) avijit    (1000)       42 2023-08-06 09:09:31.000000 avijit1996iiti_basic_calculator-0.0.2/README.txt
-drwxrwxr-x   0 avijit    (1000) avijit    (1000)        0 2023-08-06 11:11:47.650969 avijit1996iiti_basic_calculator-0.0.2/avijit1996iiti_basic_calculator.egg-info/
--rw-rw-r--   0 avijit    (1000) avijit    (1000)      599 2023-08-06 11:11:47.000000 avijit1996iiti_basic_calculator-0.0.2/avijit1996iiti_basic_calculator.egg-info/PKG-INFO
--rw-rw-r--   0 avijit    (1000) avijit    (1000)      577 2023-08-06 11:11:47.000000 avijit1996iiti_basic_calculator-0.0.2/avijit1996iiti_basic_calculator.egg-info/SOURCES.txt
--rw-rw-r--   0 avijit    (1000) avijit    (1000)        1 2023-08-06 11:11:47.000000 avijit1996iiti_basic_calculator-0.0.2/avijit1996iiti_basic_calculator.egg-info/dependency_links.txt
--rw-rw-r--   0 avijit    (1000) avijit    (1000)        1 2023-08-06 11:11:47.000000 avijit1996iiti_basic_calculator-0.0.2/avijit1996iiti_basic_calculator.egg-info/top_level.txt
--rw-rw-r--   0 avijit    (1000) avijit    (1000)       38 2023-08-06 11:11:47.654969 avijit1996iiti_basic_calculator-0.0.2/setup.cfg
--rw-rw-r--   0 avijit    (1000) avijit    (1000)      693 2023-08-06 11:11:38.000000 avijit1996iiti_basic_calculator-0.0.2/setup.py
-drwxrwxr-x   0 avijit    (1000) avijit    (1000)        0 2023-08-06 11:11:47.646968 avijit1996iiti_basic_calculator-0.0.2/src/
-drwxrwxr-x   0 avijit    (1000) avijit    (1000)        0 2023-08-06 11:11:47.650969 avijit1996iiti_basic_calculator-0.0.2/src/avijit1996iiti_basic_calculator/
--rw-rw-r--   0 avijit    (1000) avijit    (1000)        0 2023-08-06 11:03:11.000000 avijit1996iiti_basic_calculator-0.0.2/src/avijit1996iiti_basic_calculator/__init__.py
--rw-rw-r--   0 avijit    (1000) avijit    (1000)      211 2023-08-06 09:04:37.000000 avijit1996iiti_basic_calculator-0.0.2/src/avijit1996iiti_basic_calculator/addition.py
--rw-rw-r--   0 avijit    (1000) avijit    (1000)      302 2023-08-06 09:06:37.000000 avijit1996iiti_basic_calculator-0.0.2/src/avijit1996iiti_basic_calculator/calculator.py
--rw-rw-r--   0 avijit    (1000) avijit    (1000)      244 2023-08-06 09:04:43.000000 avijit1996iiti_basic_calculator-0.0.2/src/avijit1996iiti_basic_calculator/division.py
--rw-rw-r--   0 avijit    (1000) avijit    (1000)      256 2023-08-06 08:59:17.000000 avijit1996iiti_basic_calculator-0.0.2/src/avijit1996iiti_basic_calculator/multiplication.py
--rw-rw-r--   0 avijit    (1000) avijit    (1000)      253 2023-08-06 08:59:27.000000 avijit1996iiti_basic_calculator-0.0.2/src/avijit1996iiti_basic_calculator/substraction.py
+drwxrwxr-x   0 avijit    (1000) avijit    (1000)        0 2023-08-08 12:05:09.324433 avijit1996iiti_basic_calculator-0.0.3/
+-rw-rw-r--   0 avijit    (1000) avijit    (1000)       51 2023-08-06 09:11:25.000000 avijit1996iiti_basic_calculator-0.0.3/CHANGELOG.txt
+-rw-rw-r--   0 avijit    (1000) avijit    (1000)     1077 2023-08-06 08:42:59.000000 avijit1996iiti_basic_calculator-0.0.3/LICENSE.txt
+-rw-rw-r--   0 avijit    (1000) avijit    (1000)       25 2023-08-06 09:19:26.000000 avijit1996iiti_basic_calculator-0.0.3/MANIFEST.in
+-rw-rw-r--   0 avijit    (1000) avijit    (1000)      675 2023-08-08 12:05:09.324433 avijit1996iiti_basic_calculator-0.0.3/PKG-INFO
+-rw-rw-r--   0 avijit    (1000) avijit    (1000)       42 2023-08-06 09:09:31.000000 avijit1996iiti_basic_calculator-0.0.3/README.txt
+drwxrwxr-x   0 avijit    (1000) avijit    (1000)        0 2023-08-08 12:05:09.320433 avijit1996iiti_basic_calculator-0.0.3/avijit1996iiti_basic_calculator/
+-rw-rw-r--   0 avijit    (1000) avijit    (1000)      268 2023-08-08 12:02:25.000000 avijit1996iiti_basic_calculator-0.0.3/avijit1996iiti_basic_calculator/__init__.py
+-rw-rw-r--   0 avijit    (1000) avijit    (1000)      211 2023-08-06 09:04:37.000000 avijit1996iiti_basic_calculator-0.0.3/avijit1996iiti_basic_calculator/addition.py
+-rw-rw-r--   0 avijit    (1000) avijit    (1000)      302 2023-08-06 09:06:37.000000 avijit1996iiti_basic_calculator-0.0.3/avijit1996iiti_basic_calculator/calculator.py
+-rw-rw-r--   0 avijit    (1000) avijit    (1000)      244 2023-08-06 09:04:43.000000 avijit1996iiti_basic_calculator-0.0.3/avijit1996iiti_basic_calculator/division.py
+-rw-rw-r--   0 avijit    (1000) avijit    (1000)      256 2023-08-06 08:59:17.000000 avijit1996iiti_basic_calculator-0.0.3/avijit1996iiti_basic_calculator/multiplication.py
+-rw-rw-r--   0 avijit    (1000) avijit    (1000)      253 2023-08-06 08:59:27.000000 avijit1996iiti_basic_calculator-0.0.3/avijit1996iiti_basic_calculator/substraction.py
+drwxrwxr-x   0 avijit    (1000) avijit    (1000)        0 2023-08-08 12:05:09.324433 avijit1996iiti_basic_calculator-0.0.3/avijit1996iiti_basic_calculator.egg-info/
+-rw-rw-r--   0 avijit    (1000) avijit    (1000)      675 2023-08-08 12:05:08.000000 avijit1996iiti_basic_calculator-0.0.3/avijit1996iiti_basic_calculator.egg-info/PKG-INFO
+-rw-rw-r--   0 avijit    (1000) avijit    (1000)      560 2023-08-08 12:05:09.000000 avijit1996iiti_basic_calculator-0.0.3/avijit1996iiti_basic_calculator.egg-info/SOURCES.txt
+-rw-rw-r--   0 avijit    (1000) avijit    (1000)        1 2023-08-08 12:05:08.000000 avijit1996iiti_basic_calculator-0.0.3/avijit1996iiti_basic_calculator.egg-info/dependency_links.txt
+-rw-rw-r--   0 avijit    (1000) avijit    (1000)       32 2023-08-08 12:05:08.000000 avijit1996iiti_basic_calculator-0.0.3/avijit1996iiti_basic_calculator.egg-info/top_level.txt
+-rw-rw-r--   0 avijit    (1000) avijit    (1000)      111 2023-08-08 12:02:23.000000 avijit1996iiti_basic_calculator-0.0.3/run.py
+-rw-rw-r--   0 avijit    (1000) avijit    (1000)       38 2023-08-08 12:05:09.324433 avijit1996iiti_basic_calculator-0.0.3/setup.cfg
+-rw-rw-r--   0 avijit    (1000) avijit    (1000)      693 2023-08-08 12:03:43.000000 avijit1996iiti_basic_calculator-0.0.3/setup.py
```

### Comparing `avijit1996iiti_basic_calculator-0.0.2/LICENSE.txt` & `avijit1996iiti_basic_calculator-0.0.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `avijit1996iiti_basic_calculator-0.0.2/PKG-INFO` & `avijit1996iiti_basic_calculator-0.0.3/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,24 +1,24 @@
-Metadata-Version: 2.1
+Metadata-Version: 1.1
 Name: avijit1996iiti_basic_calculator
-Version: 0.0.2
+Version: 0.0.3
 Summary: A very basic calculator
-Home-page: 
+Home-page: UNKNOWN
 Author: Avijit Bhattacharjee
 Author-email: avijit.bhattacharjee1996@gmail.com
 License: MIT
+Description: # first_python_library
+        A simple calcualtor
+        
+        CHANGE LOG
+        ==================
+        
+        
+        0.0.1 (08/06/2023)
+        
 Keywords: calculator
+Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Education
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
-License-File: LICENSE.txt
-
-# first_python_library
-A simple calcualtor
-
-CHANGE LOG
-==================
-
-
-0.0.1 (08/06/2023)
```

### Comparing `avijit1996iiti_basic_calculator-0.0.2/avijit1996iiti_basic_calculator.egg-info/SOURCES.txt` & `avijit1996iiti_basic_calculator-0.0.3/avijit1996iiti_basic_calculator.egg-info/SOURCES.txt`

 * *Files 18% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 CHANGELOG.txt
 LICENSE.txt
 MANIFEST.in
 README.txt
+run.py
 setup.py
+avijit1996iiti_basic_calculator/__init__.py
+avijit1996iiti_basic_calculator/addition.py
+avijit1996iiti_basic_calculator/calculator.py
+avijit1996iiti_basic_calculator/division.py
+avijit1996iiti_basic_calculator/multiplication.py
+avijit1996iiti_basic_calculator/substraction.py
 avijit1996iiti_basic_calculator.egg-info/PKG-INFO
 avijit1996iiti_basic_calculator.egg-info/SOURCES.txt
 avijit1996iiti_basic_calculator.egg-info/dependency_links.txt
-avijit1996iiti_basic_calculator.egg-info/top_level.txt
-src/avijit1996iiti_basic_calculator/__init__.py
-src/avijit1996iiti_basic_calculator/addition.py
-src/avijit1996iiti_basic_calculator/calculator.py
-src/avijit1996iiti_basic_calculator/division.py
-src/avijit1996iiti_basic_calculator/multiplication.py
-src/avijit1996iiti_basic_calculator/substraction.py
+avijit1996iiti_basic_calculator.egg-info/top_level.txt
```

### Comparing `avijit1996iiti_basic_calculator-0.0.2/setup.py` & `avijit1996iiti_basic_calculator-0.0.3/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -6,15 +6,15 @@
   'Operating System :: OS Independent',
   'License :: OSI Approved :: MIT License',
   'Programming Language :: Python :: 3'
 ]
  
 setup(
   name='avijit1996iiti_basic_calculator',
-  version='0.0.2',
+  version='0.0.3',
   description='A very basic calculator',
   long_description=open('README.txt').read() + '\n\n' + open('CHANGELOG.txt').read(),
   url='',  
   author='Avijit Bhattacharjee',
   author_email='avijit.bhattacharjee1996@gmail.com',
   license='MIT', 
   classifiers=classifiers,
```


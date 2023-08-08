# Comparing `tmp/publishtutorial-0.0.3.tar.gz` & `tmp/publishtutorial-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "publishtutorial-0.0.3.tar", last modified: Tue Aug  8 15:26:21 2023, max compression
+gzip compressed data, was "publishtutorial-0.0.4.tar", last modified: Tue Aug  8 16:04:29 2023, max compression
```

## Comparing `publishtutorial-0.0.3.tar` & `publishtutorial-0.0.4.tar`

### file list

```diff
@@ -1,16 +1,17 @@
-drwxrwxr-x   0 bollettino  (1001) bollettino  (1001)        0 2023-08-08 15:26:21.095490 publishtutorial-0.0.3/
--rw-rw-r--   0 bollettino  (1001) bollettino  (1001)       27 2023-08-08 13:32:38.000000 publishtutorial-0.0.3/MANIFEST.in
--rw-rw-r--   0 bollettino  (1001) bollettino  (1001)     1602 2023-08-08 15:26:21.095490 publishtutorial-0.0.3/PKG-INFO
--rw-rw-r--   0 bollettino  (1001) bollettino  (1001)      680 2023-08-08 15:08:46.000000 publishtutorial-0.0.3/README.md
--rw-rw-r--   0 bollettino  (1001) bollettino  (1001)     1073 2023-08-08 12:34:30.000000 publishtutorial-0.0.3/license.txt
--rw-rw-r--   0 bollettino  (1001) bollettino  (1001)       38 2023-08-08 15:26:21.095490 publishtutorial-0.0.3/setup.cfg
--rw-rw-r--   0 bollettino  (1001) bollettino  (1001)     1376 2023-08-08 15:26:09.000000 publishtutorial-0.0.3/setup.py
-drwxrwxr-x   0 bollettino  (1001) bollettino  (1001)        0 2023-08-08 15:26:21.095490 publishtutorial-0.0.3/src/
--rw-rw-r--   0 bollettino  (1001) bollettino  (1001)      188 2023-08-08 14:47:23.000000 publishtutorial-0.0.3/src/myfunc.py
-drwxrwxr-x   0 bollettino  (1001) bollettino  (1001)        0 2023-08-08 15:26:21.095490 publishtutorial-0.0.3/src/publishtutorial.egg-info/
--rw-rw-r--   0 bollettino  (1001) bollettino  (1001)     1602 2023-08-08 15:26:21.000000 publishtutorial-0.0.3/src/publishtutorial.egg-info/PKG-INFO
--rw-rw-r--   0 bollettino  (1001) bollettino  (1001)      294 2023-08-08 15:26:21.000000 publishtutorial-0.0.3/src/publishtutorial.egg-info/SOURCES.txt
--rw-rw-r--   0 bollettino  (1001) bollettino  (1001)        1 2023-08-08 15:26:21.000000 publishtutorial-0.0.3/src/publishtutorial.egg-info/dependency_links.txt
--rw-rw-r--   0 bollettino  (1001) bollettino  (1001)       77 2023-08-08 15:26:21.000000 publishtutorial-0.0.3/src/publishtutorial.egg-info/requires.txt
--rw-rw-r--   0 bollettino  (1001) bollettino  (1001)        7 2023-08-08 15:26:21.000000 publishtutorial-0.0.3/src/publishtutorial.egg-info/top_level.txt
--rw-rw-r--   0 bollettino  (1001) bollettino  (1001)      337 2023-08-08 14:48:37.000000 publishtutorial-0.0.3/test_publishtutorial.py
+drwxrwxr-x   0 bollettino  (1001) bollettino  (1001)        0 2023-08-08 16:04:29.350067 publishtutorial-0.0.4/
+-rw-rw-r--   0 bollettino  (1001) bollettino  (1001)       27 2023-08-08 13:32:38.000000 publishtutorial-0.0.4/MANIFEST.in
+-rw-rw-r--   0 bollettino  (1001) bollettino  (1001)     1857 2023-08-08 16:04:29.350067 publishtutorial-0.0.4/PKG-INFO
+-rw-rw-r--   0 bollettino  (1001) bollettino  (1001)      935 2023-08-08 15:59:37.000000 publishtutorial-0.0.4/README.md
+-rw-rw-r--   0 bollettino  (1001) bollettino  (1001)     1073 2023-08-08 12:34:30.000000 publishtutorial-0.0.4/license.txt
+-rw-rw-r--   0 bollettino  (1001) bollettino  (1001)       30 2023-08-08 15:36:08.000000 publishtutorial-0.0.4/requirements.txt
+-rw-rw-r--   0 bollettino  (1001) bollettino  (1001)       38 2023-08-08 16:04:29.350067 publishtutorial-0.0.4/setup.cfg
+-rw-rw-r--   0 bollettino  (1001) bollettino  (1001)     1426 2023-08-08 16:04:21.000000 publishtutorial-0.0.4/setup.py
+drwxrwxr-x   0 bollettino  (1001) bollettino  (1001)        0 2023-08-08 16:04:29.350067 publishtutorial-0.0.4/src/
+-rw-rw-r--   0 bollettino  (1001) bollettino  (1001)      188 2023-08-08 14:47:23.000000 publishtutorial-0.0.4/src/myfunc.py
+drwxrwxr-x   0 bollettino  (1001) bollettino  (1001)        0 2023-08-08 16:04:29.350067 publishtutorial-0.0.4/src/publishtutorial.egg-info/
+-rw-rw-r--   0 bollettino  (1001) bollettino  (1001)     1857 2023-08-08 16:04:29.000000 publishtutorial-0.0.4/src/publishtutorial.egg-info/PKG-INFO
+-rw-rw-r--   0 bollettino  (1001) bollettino  (1001)      311 2023-08-08 16:04:29.000000 publishtutorial-0.0.4/src/publishtutorial.egg-info/SOURCES.txt
+-rw-rw-r--   0 bollettino  (1001) bollettino  (1001)        1 2023-08-08 16:04:29.000000 publishtutorial-0.0.4/src/publishtutorial.egg-info/dependency_links.txt
+-rw-rw-r--   0 bollettino  (1001) bollettino  (1001)       84 2023-08-08 16:04:29.000000 publishtutorial-0.0.4/src/publishtutorial.egg-info/requires.txt
+-rw-rw-r--   0 bollettino  (1001) bollettino  (1001)        4 2023-08-08 16:04:29.000000 publishtutorial-0.0.4/src/publishtutorial.egg-info/top_level.txt
+-rw-rw-r--   0 bollettino  (1001) bollettino  (1001)      514 2023-08-08 15:57:04.000000 publishtutorial-0.0.4/test_publishtutorial.py
```

### Comparing `publishtutorial-0.0.3/PKG-INFO` & `publishtutorial-0.0.4/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: publishtutorial
-Version: 0.0.3
+Version: 0.0.4
 Summary: Hello!
 Home-page: https://github.com/matteobollettino/publish_tutorial
 Author: Matteo Bollettino
 Author-email: matteo.bollettino@moxoff.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 1 - Planning
@@ -29,26 +29,33 @@
 ```bash
 pip3 install publishtutorial
 ```
 
 ## Usage
 ```python
 from myfunc import say_hello, average
+from second_script import second_function
 
 # Generate "Hello, World!"
 say_hello()
 
 # Generate "Hello, Everybody!"
 say_hello("Everybody")
 
-# Compute average between two numbers (default values are 1 and 2)
+# Compute average between two numbers (default values are 1 and 2 -> 1.5)
 average()
 
 # Compute average between two numbers (2.5)
 average(2,3)
+
+# Sum to input value the average between the input and 2 (default value is 1 -> 1 + average(1,2) = 2.5)
+second_function()
+
+# Sum to input value the average between the input and 2 (5.5)
+second_function(3)
 ```
 
 ## Developing
 To install publishtutorial,
  along with the tools you need to develop and run tests,
  run the following in your virtualenv:
 ```bash
```

### Comparing `publishtutorial-0.0.3/license.txt` & `publishtutorial-0.0.4/license.txt`

 * *Files identical despite different names*

### Comparing `publishtutorial-0.0.3/setup.py` & `publishtutorial-0.0.4/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,24 +1,24 @@
-from setuptools import setup
+from setuptools import setup, find_packages
 
 with open("README.md", 'r') as f:
     long_description = f.read()
 
+with open('requirements.txt') as f:
+    required = f.read().splitlines()
+
 setup(
     name='publishtutorial', # change this field if you want to create your package
-    version='0.0.3',
+    version='0.0.4',
     description='Hello!',
     long_description=long_description,
     long_description_content_type="text/markdown",
-    py_modules=["myfunc"],
+    py_modules=find_packages(),
     package_dir={'':'src'},
-    install_requires=[
-        'pandas==2.0.3',
-        'meteostat'
-    ],
+    install_requires=required,
     extras_require = {
         "dev": [
             "pytest>=3.7",
             "check-manifest>=0.49",
             "twine>=4.0.2",
         ]
     },
```

### Comparing `publishtutorial-0.0.3/src/publishtutorial.egg-info/PKG-INFO` & `publishtutorial-0.0.4/src/publishtutorial.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: publishtutorial
-Version: 0.0.3
+Version: 0.0.4
 Summary: Hello!
 Home-page: https://github.com/matteobollettino/publish_tutorial
 Author: Matteo Bollettino
 Author-email: matteo.bollettino@moxoff.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 1 - Planning
@@ -29,26 +29,33 @@
 ```bash
 pip3 install publishtutorial
 ```
 
 ## Usage
 ```python
 from myfunc import say_hello, average
+from second_script import second_function
 
 # Generate "Hello, World!"
 say_hello()
 
 # Generate "Hello, Everybody!"
 say_hello("Everybody")
 
-# Compute average between two numbers (default values are 1 and 2)
+# Compute average between two numbers (default values are 1 and 2 -> 1.5)
 average()
 
 # Compute average between two numbers (2.5)
 average(2,3)
+
+# Sum to input value the average between the input and 2 (default value is 1 -> 1 + average(1,2) = 2.5)
+second_function()
+
+# Sum to input value the average between the input and 2 (5.5)
+second_function(3)
 ```
 
 ## Developing
 To install publishtutorial,
  along with the tools you need to develop and run tests,
  run the following in your virtualenv:
 ```bash
```


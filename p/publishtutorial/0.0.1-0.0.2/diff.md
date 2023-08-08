# Comparing `tmp/publishtutorial-0.0.1.tar.gz` & `tmp/publishtutorial-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "publishtutorial-0.0.1.tar", last modified: Tue Aug  8 14:05:25 2023, max compression
+gzip compressed data, was "publishtutorial-0.0.2.tar", last modified: Tue Aug  8 14:38:11 2023, max compression
```

## Comparing `publishtutorial-0.0.1.tar` & `publishtutorial-0.0.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxr-x   0 bollettino  (1001) bollettino  (1001)        0 2023-08-08 14:05:25.258208 publishtutorial-0.0.1/
--rw-rw-r--   0 bollettino  (1001) bollettino  (1001)       27 2023-08-08 13:32:38.000000 publishtutorial-0.0.1/MANIFEST.in
--rw-rw-r--   0 bollettino  (1001) bollettino  (1001)     1330 2023-08-08 14:05:25.258208 publishtutorial-0.0.1/PKG-INFO
--rw-rw-r--   0 bollettino  (1001) bollettino  (1001)      408 2023-08-08 13:41:26.000000 publishtutorial-0.0.1/README.md
--rw-rw-r--   0 bollettino  (1001) bollettino  (1001)     1073 2023-08-08 12:34:30.000000 publishtutorial-0.0.1/license.txt
--rw-rw-r--   0 bollettino  (1001) bollettino  (1001)       38 2023-08-08 14:05:25.258208 publishtutorial-0.0.1/setup.cfg
--rw-rw-r--   0 bollettino  (1001) bollettino  (1001)     1376 2023-08-08 14:05:21.000000 publishtutorial-0.0.1/setup.py
-drwxrwxr-x   0 bollettino  (1001) bollettino  (1001)        0 2023-08-08 14:05:25.258208 publishtutorial-0.0.1/src/
--rw-rw-r--   0 bollettino  (1001) bollettino  (1001)      120 2023-08-08 13:05:11.000000 publishtutorial-0.0.1/src/myfunc.py
-drwxrwxr-x   0 bollettino  (1001) bollettino  (1001)        0 2023-08-08 14:05:25.258208 publishtutorial-0.0.1/src/publishtutorial.egg-info/
--rw-rw-r--   0 bollettino  (1001) bollettino  (1001)     1330 2023-08-08 14:05:25.000000 publishtutorial-0.0.1/src/publishtutorial.egg-info/PKG-INFO
--rw-rw-r--   0 bollettino  (1001) bollettino  (1001)      294 2023-08-08 14:05:25.000000 publishtutorial-0.0.1/src/publishtutorial.egg-info/SOURCES.txt
--rw-rw-r--   0 bollettino  (1001) bollettino  (1001)        1 2023-08-08 14:05:25.000000 publishtutorial-0.0.1/src/publishtutorial.egg-info/dependency_links.txt
--rw-rw-r--   0 bollettino  (1001) bollettino  (1001)       77 2023-08-08 14:05:25.000000 publishtutorial-0.0.1/src/publishtutorial.egg-info/requires.txt
--rw-rw-r--   0 bollettino  (1001) bollettino  (1001)        7 2023-08-08 14:05:25.000000 publishtutorial-0.0.1/src/publishtutorial.egg-info/top_level.txt
--rw-rw-r--   0 bollettino  (1001) bollettino  (1001)      205 2023-08-08 13:03:27.000000 publishtutorial-0.0.1/test_publishtutorial.py
+drwxrwxr-x   0 bollettino  (1001) bollettino  (1001)        0 2023-08-08 14:38:11.575101 publishtutorial-0.0.2/
+-rw-rw-r--   0 bollettino  (1001) bollettino  (1001)       27 2023-08-08 13:32:38.000000 publishtutorial-0.0.2/MANIFEST.in
+-rw-rw-r--   0 bollettino  (1001) bollettino  (1001)     1330 2023-08-08 14:38:11.571101 publishtutorial-0.0.2/PKG-INFO
+-rw-rw-r--   0 bollettino  (1001) bollettino  (1001)      408 2023-08-08 14:30:40.000000 publishtutorial-0.0.2/README.md
+-rw-rw-r--   0 bollettino  (1001) bollettino  (1001)     1073 2023-08-08 12:34:30.000000 publishtutorial-0.0.2/license.txt
+-rw-rw-r--   0 bollettino  (1001) bollettino  (1001)       38 2023-08-08 14:38:11.575101 publishtutorial-0.0.2/setup.cfg
+-rw-rw-r--   0 bollettino  (1001) bollettino  (1001)     1376 2023-08-08 14:37:18.000000 publishtutorial-0.0.2/setup.py
+drwxrwxr-x   0 bollettino  (1001) bollettino  (1001)        0 2023-08-08 14:38:11.571101 publishtutorial-0.0.2/src/
+-rw-rw-r--   0 bollettino  (1001) bollettino  (1001)      184 2023-08-08 14:37:09.000000 publishtutorial-0.0.2/src/myfunc.py
+drwxrwxr-x   0 bollettino  (1001) bollettino  (1001)        0 2023-08-08 14:38:11.571101 publishtutorial-0.0.2/src/publishtutorial.egg-info/
+-rw-rw-r--   0 bollettino  (1001) bollettino  (1001)     1330 2023-08-08 14:38:11.000000 publishtutorial-0.0.2/src/publishtutorial.egg-info/PKG-INFO
+-rw-rw-r--   0 bollettino  (1001) bollettino  (1001)      294 2023-08-08 14:38:11.000000 publishtutorial-0.0.2/src/publishtutorial.egg-info/SOURCES.txt
+-rw-rw-r--   0 bollettino  (1001) bollettino  (1001)        1 2023-08-08 14:38:11.000000 publishtutorial-0.0.2/src/publishtutorial.egg-info/dependency_links.txt
+-rw-rw-r--   0 bollettino  (1001) bollettino  (1001)       77 2023-08-08 14:38:11.000000 publishtutorial-0.0.2/src/publishtutorial.egg-info/requires.txt
+-rw-rw-r--   0 bollettino  (1001) bollettino  (1001)        7 2023-08-08 14:38:11.000000 publishtutorial-0.0.2/src/publishtutorial.egg-info/top_level.txt
+-rw-rw-r--   0 bollettino  (1001) bollettino  (1001)      266 2023-08-08 14:37:04.000000 publishtutorial-0.0.2/test_publishtutorial.py
```

### Comparing `publishtutorial-0.0.1/PKG-INFO` & `publishtutorial-0.0.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: publishtutorial
-Version: 0.0.1
+Version: 0.0.2
 Summary: Hello!
 Home-page: https://github.com/matteobollettino/publish_tutorial
 Author: Matteo Bollettino
 Author-email: matteo.bollettino@moxoff.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 1 - Planning
@@ -32,15 +32,15 @@
 ## Usage
 ```python
 from myfunc import say_hello
 
 # Generate "Hello, World!"
 say_hello()
 
-# Generate "Hello, everybody!"
+# Generate "Hello, Everybody!"
 say_hello("Everybody")
 ```
 
 ## Developing
 To install publishtutorial,
  along with the tools you need to develop and run tests,
  run the following in your virtualenv:
```

### Comparing `publishtutorial-0.0.1/license.txt` & `publishtutorial-0.0.2/license.txt`

 * *Files identical despite different names*

### Comparing `publishtutorial-0.0.1/setup.py` & `publishtutorial-0.0.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup
 
 with open("README.md", 'r') as f:
     long_description = f.read()
 
 setup(
     name='publishtutorial', # change this field if you want to create your package
-    version='0.0.1',
+    version='0.0.2',
     description='Hello!',
     long_description=long_description,
     long_description_content_type="text/markdown",
     py_modules=["myfunc"],
     package_dir={'':'src'},
     install_requires=[
         'pandas==2.0.3',
```

### Comparing `publishtutorial-0.0.1/src/publishtutorial.egg-info/PKG-INFO` & `publishtutorial-0.0.2/src/publishtutorial.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: publishtutorial
-Version: 0.0.1
+Version: 0.0.2
 Summary: Hello!
 Home-page: https://github.com/matteobollettino/publish_tutorial
 Author: Matteo Bollettino
 Author-email: matteo.bollettino@moxoff.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 1 - Planning
@@ -32,15 +32,15 @@
 ## Usage
 ```python
 from myfunc import say_hello
 
 # Generate "Hello, World!"
 say_hello()
 
-# Generate "Hello, everybody!"
+# Generate "Hello, Everybody!"
 say_hello("Everybody")
 ```
 
 ## Developing
 To install publishtutorial,
  along with the tools you need to develop and run tests,
  run the following in your virtualenv:
```


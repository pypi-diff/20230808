# Comparing `tmp/fracsuite-0.1.5a1.tar.gz` & `tmp/fracsuite-0.1.5a2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fracsuite-0.1.5a1.tar", last modified: Mon Aug  7 09:46:54 2023, max compression
+gzip compressed data, was "fracsuite-0.1.5a2.tar", last modified: Tue Aug  8 17:11:59 2023, max compression
```

## Comparing `fracsuite-0.1.5a1.tar` & `fracsuite-0.1.5a2.tar`

### file list

```diff
@@ -1,16 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 09:46:54.981504 fracsuite-0.1.5a1/
--rw-r--r--   0 runner    (1001) docker     (123)     2823 2023-08-07 09:46:54.981504 fracsuite-0.1.5a1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2287 2023-08-07 09:46:42.000000 fracsuite-0.1.5a1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 09:46:54.981504 fracsuite-0.1.5a1/fracsuite/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 09:46:42.000000 fracsuite-0.1.5a1/fracsuite/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      700 2023-08-07 09:46:42.000000 fracsuite-0.1.5a1/fracsuite/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16182 2023-08-07 09:46:42.000000 fracsuite-0.1.5a1/fracsuite/analyzer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1517 2023-08-07 09:46:42.000000 fracsuite-0.1.5a1/fracsuite/splinter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 09:46:54.981504 fracsuite-0.1.5a1/fracsuite.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2823 2023-08-07 09:46:54.000000 fracsuite-0.1.5a1/fracsuite.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      276 2023-08-07 09:46:54.000000 fracsuite-0.1.5a1/fracsuite.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-07 09:46:54.000000 fracsuite-0.1.5a1/fracsuite.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-08-07 09:46:54.000000 fracsuite-0.1.5a1/fracsuite.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-08-07 09:46:54.000000 fracsuite-0.1.5a1/fracsuite.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      710 2023-08-07 09:46:42.000000 fracsuite-0.1.5a1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-07 09:46:54.981504 fracsuite-0.1.5a1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 17:11:59.593892 fracsuite-0.1.5a2/
+-rw-r--r--   0 runner    (1001) docker     (123)     2843 2023-08-08 17:11:59.589892 fracsuite-0.1.5a2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2307 2023-08-08 17:11:48.000000 fracsuite-0.1.5a2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 17:11:59.589892 fracsuite-0.1.5a2/fracsuite/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 17:11:48.000000 fracsuite-0.1.5a2/fracsuite/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 17:11:59.589892 fracsuite-0.1.5a2/fracsuite/dynamic/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 17:11:48.000000 fracsuite-0.1.5a2/fracsuite/dynamic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1491 2023-08-08 17:11:48.000000 fracsuite-0.1.5a2/fracsuite/dynamic/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 17:11:59.589892 fracsuite-0.1.5a2/fracsuite/splinters/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 17:11:48.000000 fracsuite-0.1.5a2/fracsuite/splinters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6187 2023-08-08 17:11:48.000000 fracsuite-0.1.5a2/fracsuite/splinters/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24114 2023-08-08 17:11:48.000000 fracsuite-0.1.5a2/fracsuite/splinters/analyzer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1517 2023-08-08 17:11:48.000000 fracsuite-0.1.5a2/fracsuite/splinters/splinter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 17:11:59.589892 fracsuite-0.1.5a2/fracsuite.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2843 2023-08-08 17:11:59.000000 fracsuite-0.1.5a2/fracsuite.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      398 2023-08-08 17:11:59.000000 fracsuite-0.1.5a2/fracsuite.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 17:11:59.000000 fracsuite-0.1.5a2/fracsuite.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-08-08 17:11:59.000000 fracsuite-0.1.5a2/fracsuite.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-08-08 17:11:59.000000 fracsuite-0.1.5a2/fracsuite.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      710 2023-08-08 17:11:48.000000 fracsuite-0.1.5a2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-08 17:11:59.593892 fracsuite-0.1.5a2/setup.cfg
```

### Comparing `fracsuite-0.1.5a1/PKG-INFO` & `fracsuite-0.1.5a2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fracsuite
-Version: 0.1.5a1
+Version: 0.1.5a2
 Summary: Package to help analyze fracture patterns on broken glass plys.
 Author-email: Leon Bohmann <mail@leonbohmann.de>
 Project-URL: Homepage, https://github.com/leonbohmann/fracture-suite
 Project-URL: Bug Tracker, https://github.com/leonbohmann/fracture-suite/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -54,29 +54,29 @@
 ## Usage
 
 For details see: [API Docs](fracsuite.md)
 
 ### Use the module directly
 
 ```bat
-py -m fracsuite -image "path/to/image" [--crop]
+py -m fracsuite.splinters -image "path/to/image" [--crop]
 ```
 
 #### `-image`
 
 The path to the image
 
 #### `--crop`
 
 If the image contains unfiltered area around the ply, use this to crop the image to the ply.
 
 ### Create a script
 
 ```python
-from fracsuite.analyzer import Analyzer
+from fracsuite.splinters.analyzer import Analyzer
 
 image = r"Path/to/some/image.bmp"
 crop = True
 
 analyzer = Analyzer(image, crop)
 
 analyzer.plot()
```

### Comparing `fracsuite-0.1.5a1/README.md` & `fracsuite-0.1.5a2/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -41,29 +41,29 @@
 ## Usage
 
 For details see: [API Docs](fracsuite.md)
 
 ### Use the module directly
 
 ```bat
-py -m fracsuite -image "path/to/image" [--crop]
+py -m fracsuite.splinters -image "path/to/image" [--crop]
 ```
 
 #### `-image`
 
 The path to the image
 
 #### `--crop`
 
 If the image contains unfiltered area around the ply, use this to crop the image to the ply.
 
 ### Create a script
 
 ```python
-from fracsuite.analyzer import Analyzer
+from fracsuite.splinters.analyzer import Analyzer
 
 image = r"Path/to/some/image.bmp"
 crop = True
 
 analyzer = Analyzer(image, crop)
 
 analyzer.plot()
```

### Comparing `fracsuite-0.1.5a1/fracsuite/splinter.py` & `fracsuite-0.1.5a2/fracsuite/splinters/splinter.py`

 * *Files identical despite different names*

### Comparing `fracsuite-0.1.5a1/fracsuite.egg-info/PKG-INFO` & `fracsuite-0.1.5a2/fracsuite.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fracsuite
-Version: 0.1.5a1
+Version: 0.1.5a2
 Summary: Package to help analyze fracture patterns on broken glass plys.
 Author-email: Leon Bohmann <mail@leonbohmann.de>
 Project-URL: Homepage, https://github.com/leonbohmann/fracture-suite
 Project-URL: Bug Tracker, https://github.com/leonbohmann/fracture-suite/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -54,29 +54,29 @@
 ## Usage
 
 For details see: [API Docs](fracsuite.md)
 
 ### Use the module directly
 
 ```bat
-py -m fracsuite -image "path/to/image" [--crop]
+py -m fracsuite.splinters -image "path/to/image" [--crop]
 ```
 
 #### `-image`
 
 The path to the image
 
 #### `--crop`
 
 If the image contains unfiltered area around the ply, use this to crop the image to the ply.
 
 ### Create a script
 
 ```python
-from fracsuite.analyzer import Analyzer
+from fracsuite.splinters.analyzer import Analyzer
 
 image = r"Path/to/some/image.bmp"
 crop = True
 
 analyzer = Analyzer(image, crop)
 
 analyzer.plot()
```

### Comparing `fracsuite-0.1.5a1/pyproject.toml` & `fracsuite-0.1.5a2/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 dependencies = ["matplotlib", "opencv-python", "numpy", "tqdm", "scikit-image"]
 name = "fracsuite"
-version = "0.1.5a1"
+version = "0.1.5a2"
 authors = [
   { name="Leon Bohmann", email="mail@leonbohmann.de" },
 ]
 description = "Package to help analyze fracture patterns on broken glass plys."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```


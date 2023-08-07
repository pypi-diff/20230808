# Comparing `tmp/pymikro-0.14.tar.gz` & `tmp/pymikro-0.15.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pymikro-0.14.tar", last modified: Sun Aug  6 20:53:54 2023, max compression
+gzip compressed data, was "pymikro-0.15.tar", last modified: Mon Aug  7 23:02:18 2023, max compression
```

## Comparing `pymikro-0.14.tar` & `pymikro-0.15.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 ze        (1000) ze        (1000)        0 2023-08-06 20:53:54.224860 pymikro-0.14/
--rw-r--r--   0 ze        (1000) ze        (1000)    26526 2023-08-06 20:45:02.000000 pymikro-0.14/LICENSE
--rw-r--r--   0 ze        (1000) ze        (1000)      320 2023-08-06 20:53:54.224860 pymikro-0.14/PKG-INFO
--rw-r--r--   0 ze        (1000) ze        (1000)     6625 2023-08-06 20:45:02.000000 pymikro-0.14/README.md
--rw-r--r--   0 ze        (1000) ze        (1000)       38 2023-08-06 20:53:54.224860 pymikro-0.14/setup.cfg
--rw-r--r--   0 ze        (1000) ze        (1000)      586 2023-08-06 20:53:41.000000 pymikro-0.14/setup.py
-drwxr-xr-x   0 ze        (1000) ze        (1000)        0 2023-08-06 20:53:54.224860 pymikro-0.14/src/
-drwxr-xr-x   0 ze        (1000) ze        (1000)        0 2023-08-06 20:53:54.224860 pymikro-0.14/src/pymikro/
--rw-r--r--   0 ze        (1000) ze        (1000)   756072 2023-08-06 20:45:02.000000 pymikro-0.14/src/pymikro/DejaVuSans.ttf
--rw-r--r--   0 ze        (1000) ze        (1000)     5299 2023-08-06 20:45:02.000000 pymikro-0.14/src/pymikro/__init__.py
--rw-r--r--   0 ze        (1000) ze        (1000)     1456 2023-08-06 20:45:02.000000 pymikro-0.14/src/pymikro/maschine_mikro_mk3.json
-drwxr-xr-x   0 ze        (1000) ze        (1000)        0 2023-08-06 20:53:54.224860 pymikro-0.14/src/pymikro.egg-info/
--rw-r--r--   0 ze        (1000) ze        (1000)      320 2023-08-06 20:53:54.000000 pymikro-0.14/src/pymikro.egg-info/PKG-INFO
--rw-r--r--   0 ze        (1000) ze        (1000)      287 2023-08-06 20:53:54.000000 pymikro-0.14/src/pymikro.egg-info/SOURCES.txt
--rw-r--r--   0 ze        (1000) ze        (1000)        1 2023-08-06 20:53:54.000000 pymikro-0.14/src/pymikro.egg-info/dependency_links.txt
--rw-r--r--   0 ze        (1000) ze        (1000)       11 2023-08-06 20:53:54.000000 pymikro-0.14/src/pymikro.egg-info/requires.txt
--rw-r--r--   0 ze        (1000) ze        (1000)        8 2023-08-06 20:53:54.000000 pymikro-0.14/src/pymikro.egg-info/top_level.txt
+drwxr-xr-x   0 ze        (1000) ze        (1000)        0 2023-08-07 23:02:18.715923 pymikro-0.15/
+-rw-r--r--   0 ze        (1000) ze        (1000)    26526 2023-08-06 20:45:02.000000 pymikro-0.15/LICENSE
+-rw-r--r--   0 ze        (1000) ze        (1000)      320 2023-08-07 23:02:18.715923 pymikro-0.15/PKG-INFO
+-rw-r--r--   0 ze        (1000) ze        (1000)     6621 2023-08-07 15:01:03.000000 pymikro-0.15/README.md
+-rw-r--r--   0 ze        (1000) ze        (1000)       38 2023-08-07 23:02:18.715923 pymikro-0.15/setup.cfg
+-rw-r--r--   0 ze        (1000) ze        (1000)      586 2023-08-07 23:02:08.000000 pymikro-0.15/setup.py
+drwxr-xr-x   0 ze        (1000) ze        (1000)        0 2023-08-07 23:02:18.715923 pymikro-0.15/src/
+drwxr-xr-x   0 ze        (1000) ze        (1000)        0 2023-08-07 23:02:18.715923 pymikro-0.15/src/pymikro/
+-rw-r--r--   0 ze        (1000) ze        (1000)   756072 2023-08-06 20:45:02.000000 pymikro-0.15/src/pymikro/DejaVuSans.ttf
+-rw-r--r--   0 ze        (1000) ze        (1000)     5299 2023-08-07 23:00:01.000000 pymikro-0.15/src/pymikro/__init__.py
+-rw-r--r--   0 ze        (1000) ze        (1000)     1455 2023-08-07 22:57:04.000000 pymikro-0.15/src/pymikro/maschine_mikro_mk3.json
+drwxr-xr-x   0 ze        (1000) ze        (1000)        0 2023-08-07 23:02:18.715923 pymikro-0.15/src/pymikro.egg-info/
+-rw-r--r--   0 ze        (1000) ze        (1000)      320 2023-08-07 23:02:18.000000 pymikro-0.15/src/pymikro.egg-info/PKG-INFO
+-rw-r--r--   0 ze        (1000) ze        (1000)      287 2023-08-07 23:02:18.000000 pymikro-0.15/src/pymikro.egg-info/SOURCES.txt
+-rw-r--r--   0 ze        (1000) ze        (1000)        1 2023-08-07 23:02:18.000000 pymikro-0.15/src/pymikro.egg-info/dependency_links.txt
+-rw-r--r--   0 ze        (1000) ze        (1000)       11 2023-08-07 23:02:18.000000 pymikro-0.15/src/pymikro.egg-info/requires.txt
+-rw-r--r--   0 ze        (1000) ze        (1000)        8 2023-08-07 23:02:18.000000 pymikro-0.15/src/pymikro.egg-info/top_level.txt
```

### Comparing `pymikro-0.14/LICENSE` & `pymikro-0.15/LICENSE`

 * *Files identical despite different names*

### Comparing `pymikro-0.14/README.md` & `pymikro-0.15/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -85,15 +85,15 @@
 
 1. Donwload the latest version of `hidapi-win.zip` from https://github.com/libusb/hidapi/releases
 
 2. Extract the zip file and copy the `hidapi.dll` corresponding to your architecture to `C:\Users\<Username>\AppData\Local\Programs\Python`
 
 
 
-Install the hid package
+Install the package
 
 ```
 pip3 install pymikro
 ```
```

### Comparing `pymikro-0.14/setup.py` & `pymikro-0.15/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup, find_packages
 
 
 setup(
     include_package_data=True,
     name='pymikro',
-    version='0.14',
+    version='0.15',
     description='API to control the Maschine Mikro MK3',
     url='https://github.com/flokapi/pymikro',
     author='flokapi',
     author_email='flokapi@pm.me',
     package_dir={'': 'src'},
     packages=find_packages(where='src'),
     package_data={"pymikro": ["*.json", "*.ttf"]},
```

### Comparing `pymikro-0.14/src/pymikro/DejaVuSans.ttf` & `pymikro-0.15/src/pymikro/DejaVuSans.ttf`

 * *Files identical despite different names*

### Comparing `pymikro-0.14/src/pymikro/__init__.py` & `pymikro-0.15/src/pymikro/__init__.py`

 * *Files identical despite different names*

### Comparing `pymikro-0.14/src/pymikro/maschine_mikro_mk3.json` & `pymikro-0.15/src/pymikro/maschine_mikro_mk3.json`

 * *Files 12% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9800000000000001%*

 * *Differences: {"'pad'": "{'order': {insert: [(0, 12), (4, 8), (8, 4), (12, 0)], delete: [15, 11, 7, 3]}}"}*

```diff
@@ -68,28 +68,28 @@
         "purple",
         "magenta",
         "fuchsia",
         "white"
     ],
     "pad": {
         "order": [
+            12,
             13,
             14,
             15,
-            16,
+            8,
             9,
             10,
             11,
-            12,
+            4,
             5,
             6,
             7,
-            8,
+            0,
             1,
             2,
-            3,
-            4
+            3
         ]
     },
     "pid": "0x1700",
     "vid": "0x17cc"
 }
```


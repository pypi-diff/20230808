# Comparing `tmp/ler-0.2.4.tar.gz` & `tmp/ler-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ler-0.2.4.tar", last modified: Tue Aug  8 12:56:31 2023, max compression
+gzip compressed data, was "ler-0.2.5.tar", last modified: Tue Aug  8 13:00:29 2023, max compression
```

## Comparing `ler-0.2.4.tar` & `ler-0.2.5.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 phurailatpamhemantakumar   (502) staff       (20)        0 2023-08-08 12:56:31.959778 ler-0.2.4/
--rw-r--r--   0 phurailatpamhemantakumar   (502) staff       (20)     1081 2023-08-08 12:33:01.000000 ler-0.2.4/LICENSE
--rw-r--r--   0 phurailatpamhemantakumar   (502) staff       (20)     4252 2023-08-08 12:56:31.959586 ler-0.2.4/PKG-INFO
--rw-r--r--   0 phurailatpamhemantakumar   (502) staff       (20)     3953 2023-07-18 11:18:01.000000 ler-0.2.4/README.md
-drwxr-xr-x   0 phurailatpamhemantakumar   (502) staff       (20)        0 2023-08-08 12:56:31.958173 ler-0.2.4/ler/
--rw-r--r--   0 phurailatpamhemantakumar   (502) staff       (20)      313 2023-08-06 15:04:54.000000 ler-0.2.4/ler/__init__.py
--rw-r--r--   0 phurailatpamhemantakumar   (502) staff       (20)     6411 2023-06-28 19:43:19.000000 ler-0.2.4/ler/helperroutines.py
--rw-r--r--   0 phurailatpamhemantakumar   (502) staff       (20)    44403 2023-07-31 11:56:54.000000 ler-0.2.4/ler/lens_galaxy_population.py
--rw-r--r--   0 phurailatpamhemantakumar   (502) staff       (20)    69959 2023-08-04 07:40:52.000000 ler-0.2.4/ler/ler.py
--rw-r--r--   0 phurailatpamhemantakumar   (502) staff       (20)    16064 2023-06-21 13:48:36.000000 ler-0.2.4/ler/multiprocessing_routine.py
--rw-r--r--   0 phurailatpamhemantakumar   (502) staff       (20)    38054 2023-06-28 21:19:22.000000 ler-0.2.4/ler/source_population.py
-drwxr-xr-x   0 phurailatpamhemantakumar   (502) staff       (20)        0 2023-08-08 12:56:31.959235 ler-0.2.4/ler.egg-info/
--rw-r--r--   0 phurailatpamhemantakumar   (502) staff       (20)     4252 2023-08-08 12:56:31.000000 ler-0.2.4/ler.egg-info/PKG-INFO
--rw-r--r--   0 phurailatpamhemantakumar   (502) staff       (20)      295 2023-08-08 12:56:31.000000 ler-0.2.4/ler.egg-info/SOURCES.txt
--rw-r--r--   0 phurailatpamhemantakumar   (502) staff       (20)        1 2023-08-08 12:56:31.000000 ler-0.2.4/ler.egg-info/dependency_links.txt
--rw-r--r--   0 phurailatpamhemantakumar   (502) staff       (20)      219 2023-08-08 12:56:31.000000 ler-0.2.4/ler.egg-info/requires.txt
--rw-r--r--   0 phurailatpamhemantakumar   (502) staff       (20)        4 2023-08-08 12:56:31.000000 ler-0.2.4/ler.egg-info/top_level.txt
--rw-r--r--   0 phurailatpamhemantakumar   (502) staff       (20)       38 2023-08-08 12:56:31.959904 ler-0.2.4/setup.cfg
--rw-r--r--   0 phurailatpamhemantakumar   (502) staff       (20)     1184 2023-08-08 12:56:21.000000 ler-0.2.4/setup.py
+drwxr-xr-x   0 phurailatpamhemantakumar   (502) staff       (20)        0 2023-08-08 13:00:29.354257 ler-0.2.5/
+-rw-r--r--   0 phurailatpamhemantakumar   (502) staff       (20)     1081 2023-08-08 12:33:01.000000 ler-0.2.5/LICENSE
+-rw-r--r--   0 phurailatpamhemantakumar   (502) staff       (20)     4252 2023-08-08 13:00:29.354063 ler-0.2.5/PKG-INFO
+-rw-r--r--   0 phurailatpamhemantakumar   (502) staff       (20)     3953 2023-07-18 11:18:01.000000 ler-0.2.5/README.md
+drwxr-xr-x   0 phurailatpamhemantakumar   (502) staff       (20)        0 2023-08-08 13:00:29.351960 ler-0.2.5/ler/
+-rw-r--r--   0 phurailatpamhemantakumar   (502) staff       (20)      313 2023-08-06 15:04:54.000000 ler-0.2.5/ler/__init__.py
+-rw-r--r--   0 phurailatpamhemantakumar   (502) staff       (20)     6411 2023-06-28 19:43:19.000000 ler-0.2.5/ler/helperroutines.py
+-rw-r--r--   0 phurailatpamhemantakumar   (502) staff       (20)    44403 2023-07-31 11:56:54.000000 ler-0.2.5/ler/lens_galaxy_population.py
+-rw-r--r--   0 phurailatpamhemantakumar   (502) staff       (20)    69959 2023-08-04 07:40:52.000000 ler-0.2.5/ler/ler.py
+-rw-r--r--   0 phurailatpamhemantakumar   (502) staff       (20)    16064 2023-06-21 13:48:36.000000 ler-0.2.5/ler/multiprocessing_routine.py
+-rw-r--r--   0 phurailatpamhemantakumar   (502) staff       (20)    38054 2023-06-28 21:19:22.000000 ler-0.2.5/ler/source_population.py
+drwxr-xr-x   0 phurailatpamhemantakumar   (502) staff       (20)        0 2023-08-08 13:00:29.353674 ler-0.2.5/ler.egg-info/
+-rw-r--r--   0 phurailatpamhemantakumar   (502) staff       (20)     4252 2023-08-08 13:00:29.000000 ler-0.2.5/ler.egg-info/PKG-INFO
+-rw-r--r--   0 phurailatpamhemantakumar   (502) staff       (20)      295 2023-08-08 13:00:29.000000 ler-0.2.5/ler.egg-info/SOURCES.txt
+-rw-r--r--   0 phurailatpamhemantakumar   (502) staff       (20)        1 2023-08-08 13:00:29.000000 ler-0.2.5/ler.egg-info/dependency_links.txt
+-rw-r--r--   0 phurailatpamhemantakumar   (502) staff       (20)      158 2023-08-08 13:00:29.000000 ler-0.2.5/ler.egg-info/requires.txt
+-rw-r--r--   0 phurailatpamhemantakumar   (502) staff       (20)        4 2023-08-08 13:00:29.000000 ler-0.2.5/ler.egg-info/top_level.txt
+-rw-r--r--   0 phurailatpamhemantakumar   (502) staff       (20)       38 2023-08-08 13:00:29.354401 ler-0.2.5/setup.cfg
+-rw-r--r--   0 phurailatpamhemantakumar   (502) staff       (20)     1187 2023-08-08 13:00:23.000000 ler-0.2.5/setup.py
```

### Comparing `ler-0.2.4/LICENSE` & `ler-0.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `ler-0.2.4/PKG-INFO` & `ler-0.2.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ler
-Version: 0.2.4
+Version: 0.2.5
 Summary: Gravitational waves Lensing Rates
 Home-page: https://github.com/hemantaph/ler
 Author: Hemantakumar
 Author-email: hemantaphurailatpam@gmail.com
 License: MIT
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
```

### Comparing `ler-0.2.4/README.md` & `ler-0.2.5/README.md`

 * *Files identical despite different names*

### Comparing `ler-0.2.4/ler/helperroutines.py` & `ler-0.2.5/ler/helperroutines.py`

 * *Files identical despite different names*

### Comparing `ler-0.2.4/ler/lens_galaxy_population.py` & `ler-0.2.5/ler/lens_galaxy_population.py`

 * *Files identical despite different names*

### Comparing `ler-0.2.4/ler/ler.py` & `ler-0.2.5/ler/ler.py`

 * *Files identical despite different names*

### Comparing `ler-0.2.4/ler/multiprocessing_routine.py` & `ler-0.2.5/ler/multiprocessing_routine.py`

 * *Files identical despite different names*

### Comparing `ler-0.2.4/ler/source_population.py` & `ler-0.2.5/ler/source_population.py`

 * *Files identical despite different names*

### Comparing `ler-0.2.4/ler.egg-info/PKG-INFO` & `ler-0.2.5/ler.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ler
-Version: 0.2.4
+Version: 0.2.5
 Summary: Gravitational waves Lensing Rates
 Home-page: https://github.com/hemantaph/ler
 Author: Hemantakumar
 Author-email: hemantaphurailatpam@gmail.com
 License: MIT
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
```

### Comparing `ler-0.2.4/setup.py` & `ler-0.2.5/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 # check that python version is 3.7 or above
 python_version = sys.version_info
 if python_version < (3, 10):
     sys.exit("Python < 3.10 is not supported, aborting setup")
 
 setup(
     name="ler",
-    version="0.2.4",
+    version="0.2.5",
     description="Gravitational waves Lensing Rates",
     long_description=long_description,
     long_description_content_type='text/markdown',
     author="Hemantakumar",
     license="MIT",
     author_email="hemantaphurailatpam@gmail.com",
     url="https://github.com/hemantaph/ler",
@@ -31,10 +31,10 @@
         "gwsnr>=0.1",
         "scipy>=1.9.0",
         "lenstronomy>=1.10.4",
         "astropy>=5.1",
         "tqdm>=4.64.1",
         "pointpats>=2.3",
         "shapely>=2.0.1",
-        "gwcosmo@git+https://git.ligo.org/lscsoft/gwcosmo.git@v1.0.0",
+        #"gwcosmo @ git+https://git.ligo.org/lscsoft/gwcosmo.git@v1.0.0",
     ],
 )
```


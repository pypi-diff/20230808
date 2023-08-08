# Comparing `tmp/ler-0.2.0.tar.gz` & `tmp/ler-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ler-0.2.0.tar", last modified: Fri Aug  4 10:37:38 2023, max compression
+gzip compressed data, was "ler-0.2.3.tar", last modified: Tue Aug  8 08:27:44 2023, max compression
```

## Comparing `ler-0.2.0.tar` & `ler-0.2.3.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 phurailatpamhemantakumar   (502) staff       (20)        0 2023-08-04 10:37:38.612339 ler-0.2.0/
--rw-r--r--   0 phurailatpamhemantakumar   (502) staff       (20)     4206 2023-08-04 10:37:38.612146 ler-0.2.0/PKG-INFO
--rw-r--r--   0 phurailatpamhemantakumar   (502) staff       (20)     3953 2023-07-18 11:18:01.000000 ler-0.2.0/README.md
-drwxr-xr-x   0 phurailatpamhemantakumar   (502) staff       (20)        0 2023-08-04 10:37:38.610272 ler-0.2.0/ler/
--rw-r--r--   0 phurailatpamhemantakumar   (502) staff       (20)      315 2023-06-21 13:48:36.000000 ler-0.2.0/ler/__init__.py
--rw-r--r--   0 phurailatpamhemantakumar   (502) staff       (20)     6411 2023-06-28 19:43:19.000000 ler-0.2.0/ler/helperroutines.py
--rw-r--r--   0 phurailatpamhemantakumar   (502) staff       (20)    44403 2023-07-31 11:56:54.000000 ler-0.2.0/ler/lens_galaxy_population.py
--rw-r--r--   0 phurailatpamhemantakumar   (502) staff       (20)    69959 2023-08-04 07:40:52.000000 ler-0.2.0/ler/ler.py
--rw-r--r--   0 phurailatpamhemantakumar   (502) staff       (20)    16064 2023-06-21 13:48:36.000000 ler-0.2.0/ler/multiprocessing_routine.py
--rw-r--r--   0 phurailatpamhemantakumar   (502) staff       (20)    38054 2023-06-28 21:19:22.000000 ler-0.2.0/ler/source_population.py
-drwxr-xr-x   0 phurailatpamhemantakumar   (502) staff       (20)        0 2023-08-04 10:37:38.611749 ler-0.2.0/ler.egg-info/
--rw-r--r--   0 phurailatpamhemantakumar   (502) staff       (20)     4206 2023-08-04 10:37:38.000000 ler-0.2.0/ler.egg-info/PKG-INFO
--rw-r--r--   0 phurailatpamhemantakumar   (502) staff       (20)      287 2023-08-04 10:37:38.000000 ler-0.2.0/ler.egg-info/SOURCES.txt
--rw-r--r--   0 phurailatpamhemantakumar   (502) staff       (20)        1 2023-08-04 10:37:38.000000 ler-0.2.0/ler.egg-info/dependency_links.txt
--rw-r--r--   0 phurailatpamhemantakumar   (502) staff       (20)      158 2023-08-04 10:37:38.000000 ler-0.2.0/ler.egg-info/requires.txt
--rw-r--r--   0 phurailatpamhemantakumar   (502) staff       (20)        4 2023-08-04 10:37:38.000000 ler-0.2.0/ler.egg-info/top_level.txt
--rw-r--r--   0 phurailatpamhemantakumar   (502) staff       (20)       38 2023-08-04 10:37:38.612423 ler-0.2.0/setup.cfg
--rw-r--r--   0 phurailatpamhemantakumar   (502) staff       (20)      901 2023-08-04 10:12:42.000000 ler-0.2.0/setup.py
+drwxr-xr-x   0 phurailatpamhemantakumar   (502) staff       (20)        0 2023-08-08 08:27:44.772600 ler-0.2.3/
+-rw-r--r--   0 phurailatpamhemantakumar   (502) staff       (20)     4230 2023-08-08 08:27:44.772395 ler-0.2.3/PKG-INFO
+-rw-r--r--   0 phurailatpamhemantakumar   (502) staff       (20)     3953 2023-07-18 11:18:01.000000 ler-0.2.3/README.md
+drwxr-xr-x   0 phurailatpamhemantakumar   (502) staff       (20)        0 2023-08-08 08:27:44.770319 ler-0.2.3/ler/
+-rw-r--r--   0 phurailatpamhemantakumar   (502) staff       (20)      313 2023-08-06 15:04:54.000000 ler-0.2.3/ler/__init__.py
+-rw-r--r--   0 phurailatpamhemantakumar   (502) staff       (20)     6411 2023-06-28 19:43:19.000000 ler-0.2.3/ler/helperroutines.py
+-rw-r--r--   0 phurailatpamhemantakumar   (502) staff       (20)    44403 2023-07-31 11:56:54.000000 ler-0.2.3/ler/lens_galaxy_population.py
+-rw-r--r--   0 phurailatpamhemantakumar   (502) staff       (20)    69959 2023-08-04 07:40:52.000000 ler-0.2.3/ler/ler.py
+-rw-r--r--   0 phurailatpamhemantakumar   (502) staff       (20)    16064 2023-06-21 13:48:36.000000 ler-0.2.3/ler/multiprocessing_routine.py
+-rw-r--r--   0 phurailatpamhemantakumar   (502) staff       (20)    38054 2023-06-28 21:19:22.000000 ler-0.2.3/ler/source_population.py
+drwxr-xr-x   0 phurailatpamhemantakumar   (502) staff       (20)        0 2023-08-08 08:27:44.772126 ler-0.2.3/ler.egg-info/
+-rw-r--r--   0 phurailatpamhemantakumar   (502) staff       (20)     4230 2023-08-08 08:27:44.000000 ler-0.2.3/ler.egg-info/PKG-INFO
+-rw-r--r--   0 phurailatpamhemantakumar   (502) staff       (20)      287 2023-08-08 08:27:44.000000 ler-0.2.3/ler.egg-info/SOURCES.txt
+-rw-r--r--   0 phurailatpamhemantakumar   (502) staff       (20)        1 2023-08-08 08:27:44.000000 ler-0.2.3/ler.egg-info/dependency_links.txt
+-rw-r--r--   0 phurailatpamhemantakumar   (502) staff       (20)      158 2023-08-08 08:27:44.000000 ler-0.2.3/ler.egg-info/requires.txt
+-rw-r--r--   0 phurailatpamhemantakumar   (502) staff       (20)        4 2023-08-08 08:27:44.000000 ler-0.2.3/ler.egg-info/top_level.txt
+-rw-r--r--   0 phurailatpamhemantakumar   (502) staff       (20)       38 2023-08-08 08:27:44.772646 ler-0.2.3/setup.cfg
+-rw-r--r--   0 phurailatpamhemantakumar   (502) staff       (20)      931 2023-08-08 08:26:55.000000 ler-0.2.3/setup.py
```

### Comparing `ler-0.2.0/PKG-INFO` & `ler-0.2.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 Metadata-Version: 2.1
 Name: ler
-Version: 0.2.0
+Version: 0.2.3
 Summary: Gravitational waves Lensing Rates
 Home-page: https://github.com/hemantaph/ler
 Author: Hemantakumar
 Author-email: hemantaphurailatpam@gmail.com
 License: MIT
+Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 
 # LeR
 [![DOI](https://zenodo.org/badge/626733473.svg)](https://zenodo.org/badge/latestdoi/626733473)
 
 `LeR` is a statistical-based python package whose core function is to calculate detectable rates of both lensing and unlensed GW events. This calculation is very much dependent on the other functionality of the package, which can be subdivided into three parts; 1. Sampling of compact-binary source properties, 2. Sampling of lens galaxy characteristics and 3. Solving the lens equation to get image properties of the source. The package as a whole relies on `numpy` array operation and linear algebra, `scipy` interpolation and `multiprocessing` functionality of python to increase speed and functionality without compromising on the ease of use. The API of `LeR` is structured such that each functionality mentioned stands in its own right for scientific research but also can be used together as needed. Key features of `LeR` and its dependencies can be summarized as follows,
```

### Comparing `ler-0.2.0/README.md` & `ler-0.2.3/README.md`

 * *Files identical despite different names*

### Comparing `ler-0.2.0/ler/helperroutines.py` & `ler-0.2.3/ler/helperroutines.py`

 * *Files identical despite different names*

### Comparing `ler-0.2.0/ler/lens_galaxy_population.py` & `ler-0.2.3/ler/lens_galaxy_population.py`

 * *Files identical despite different names*

### Comparing `ler-0.2.0/ler/ler.py` & `ler-0.2.3/ler/ler.py`

 * *Files identical despite different names*

### Comparing `ler-0.2.0/ler/multiprocessing_routine.py` & `ler-0.2.3/ler/multiprocessing_routine.py`

 * *Files identical despite different names*

### Comparing `ler-0.2.0/ler/source_population.py` & `ler-0.2.3/ler/source_population.py`

 * *Files identical despite different names*

### Comparing `ler-0.2.0/ler.egg-info/PKG-INFO` & `ler-0.2.3/ler.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 Metadata-Version: 2.1
 Name: ler
-Version: 0.2.0
+Version: 0.2.3
 Summary: Gravitational waves Lensing Rates
 Home-page: https://github.com/hemantaph/ler
 Author: Hemantakumar
 Author-email: hemantaphurailatpam@gmail.com
 License: MIT
+Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 
 # LeR
 [![DOI](https://zenodo.org/badge/626733473.svg)](https://zenodo.org/badge/latestdoi/626733473)
 
 `LeR` is a statistical-based python package whose core function is to calculate detectable rates of both lensing and unlensed GW events. This calculation is very much dependent on the other functionality of the package, which can be subdivided into three parts; 1. Sampling of compact-binary source properties, 2. Sampling of lens galaxy characteristics and 3. Solving the lens equation to get image properties of the source. The package as a whole relies on `numpy` array operation and linear algebra, `scipy` interpolation and `multiprocessing` functionality of python to increase speed and functionality without compromising on the ease of use. The API of `LeR` is structured such that each functionality mentioned stands in its own right for scientific research but also can be used together as needed. Key features of `LeR` and its dependencies can be summarized as follows,
```

### Comparing `ler-0.2.0/setup.py` & `ler-0.2.3/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -3,27 +3,28 @@
 # read the contents of your README file
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
     name="ler",
-    version="0.2.0",
+    version="0.2.3",
     description="Gravitational waves Lensing Rates",
     long_description=long_description,
     long_description_content_type='text/markdown',
     author="Hemantakumar",
     license="MIT",
     author_email="hemantaphurailatpam@gmail.com",
     url="https://github.com/hemantaph/ler",
     packages=find_packages(),
+    python_requires='>=3.10',
     install_requires=[
         "setuptools>=67.8.0",
         "numpy>=1.18",
-        "numba>=0.56.4",
+        "numba>=0.57.1",
         "bilby>=1.0.2",
         "gwsnr>=0.1",
         "scipy>=1.9.0",
         "lenstronomy>=1.10.4",
         "astropy>=5.1",
         "tqdm>=4.64.1",
         "pointpats>=2.3",
```


# Comparing `tmp/spyderwebb-1.0.2.tar.gz` & `tmp/spyderwebb-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/spyderwebb-1.0.2.tar", last modified: Sat Nov 26 03:59:14 2022, max compression
+gzip compressed data, was "dist/spyderwebb-1.0.3.tar", last modified: Tue Aug  8 19:11:11 2023, max compression
```

## Comparing `spyderwebb-1.0.2.tar` & `spyderwebb-1.0.3.tar`

### file list

```diff
@@ -1,36 +1,48 @@
-drwxr-xr-x   0 nidever    (503) staff       (20)        0 2022-11-26 03:59:14.000000 spyderwebb-1.0.2/
--rw-r--r--   0 nidever    (503) staff       (20)     1070 2022-11-23 16:27:48.000000 spyderwebb-1.0.2/LICENSE
--rw-r--r--   0 nidever    (503) staff       (20)       59 2022-11-23 16:30:43.000000 spyderwebb-1.0.2/MANIFEST.in
--rw-r--r--   0 nidever    (503) staff       (20)     1131 2022-11-26 03:59:14.000000 spyderwebb-1.0.2/PKG-INFO
--rw-r--r--   0 nidever    (503) staff       (20)      719 2022-11-23 16:30:20.000000 spyderwebb-1.0.2/README.rst
-drwxr-xr-x   0 nidever    (503) staff       (20)        0 2022-11-26 03:59:14.000000 spyderwebb-1.0.2/bin/
--rwxr-xr-x   0 nidever    (503) staff       (20)    11751 2022-11-23 16:26:40.000000 spyderwebb-1.0.2/bin/spyderwebb
-drwxr-xr-x   0 nidever    (503) staff       (20)        0 2022-11-26 03:59:14.000000 spyderwebb-1.0.2/docs/
--rw-r--r--   0 nidever    (503) staff       (20)      634 2021-06-04 00:23:25.000000 spyderwebb-1.0.2/docs/Makefile
-drwxr-xr-x   0 nidever    (503) staff       (20)        0 2022-11-26 03:59:14.000000 spyderwebb-1.0.2/docs/_static/
--rw-r--r--   0 nidever    (503) staff       (20)      331 2021-06-04 00:24:28.000000 spyderwebb-1.0.2/docs/_static/spyderwebb.css
--rw-r--r--   0 nidever    (503) staff       (20)     7989 2022-11-23 16:34:02.000000 spyderwebb-1.0.2/docs/conf.py
--rw-r--r--   0 nidever    (503) staff       (20)    14771 2021-06-05 21:25:39.000000 spyderwebb-1.0.2/docs/examples.rst
--rw-r--r--   0 nidever    (503) staff       (20)    12185 2021-06-05 18:20:14.000000 spyderwebb-1.0.2/docs/gettingstarted.rst
--rw-r--r--   0 nidever    (503) staff       (20)     5469 2021-09-26 03:48:35.000000 spyderwebb-1.0.2/docs/index.rst
--rw-r--r--   0 nidever    (503) staff       (20)      402 2022-11-23 16:33:13.000000 spyderwebb-1.0.2/docs/install.rst
--rw-r--r--   0 nidever    (503) staff       (20)      795 2021-06-04 00:23:25.000000 spyderwebb-1.0.2/docs/make.bat
--rw-r--r--   0 nidever    (503) staff       (20)       69 2021-06-04 00:23:25.000000 spyderwebb-1.0.2/docs/requirements.txt
--rw-r--r--   0 nidever    (503) staff       (20)      149 2022-11-23 16:26:33.000000 spyderwebb-1.0.2/environment.yml
-drwxr-xr-x   0 nidever    (503) staff       (20)        0 2022-11-26 03:59:14.000000 spyderwebb-1.0.2/python/
-drwxr-xr-x   0 nidever    (503) staff       (20)        0 2022-11-26 03:59:14.000000 spyderwebb-1.0.2/python/spyderwebb/
--rw-r--r--   0 nidever    (503) staff       (20)       61 2022-11-26 03:59:11.000000 spyderwebb-1.0.2/python/spyderwebb/__init__.py
--rw-r--r--   0 nidever    (503) staff       (20)    16185 2022-11-26 03:58:12.000000 spyderwebb-1.0.2/python/spyderwebb/extract.py
--rw-r--r--   0 nidever    (503) staff       (20)     6016 2022-11-25 20:35:50.000000 spyderwebb-1.0.2/python/spyderwebb/reduce.py
--rw-r--r--   0 nidever    (503) staff       (20)     2968 2022-11-26 03:58:54.000000 spyderwebb-1.0.2/python/spyderwebb/utils.py
-drwxr-xr-x   0 nidever    (503) staff       (20)        0 2022-11-26 03:59:14.000000 spyderwebb-1.0.2/python/spyderwebb.egg-info/
--rw-r--r--   0 nidever    (503) staff       (20)     1131 2022-11-26 03:59:14.000000 spyderwebb-1.0.2/python/spyderwebb.egg-info/PKG-INFO
--rw-r--r--   0 nidever    (503) staff       (20)      641 2022-11-26 03:59:14.000000 spyderwebb-1.0.2/python/spyderwebb.egg-info/SOURCES.txt
--rw-r--r--   0 nidever    (503) staff       (20)        1 2022-11-26 03:59:14.000000 spyderwebb-1.0.2/python/spyderwebb.egg-info/dependency_links.txt
--rw-r--r--   0 nidever    (503) staff       (20)        1 2022-11-23 17:22:17.000000 spyderwebb-1.0.2/python/spyderwebb.egg-info/not-zip-safe
--rw-r--r--   0 nidever    (503) staff       (20)      125 2022-11-26 03:59:14.000000 spyderwebb-1.0.2/python/spyderwebb.egg-info/requires.txt
--rw-r--r--   0 nidever    (503) staff       (20)       11 2022-11-26 03:59:14.000000 spyderwebb-1.0.2/python/spyderwebb.egg-info/top_level.txt
--rw-r--r--   0 nidever    (503) staff       (20)       49 2022-11-23 16:26:33.000000 spyderwebb-1.0.2/requirements-dev.txt
--rw-r--r--   0 nidever    (503) staff       (20)       36 2022-11-23 16:31:02.000000 spyderwebb-1.0.2/requirements.txt
--rw-r--r--   0 nidever    (503) staff       (20)     1147 2022-11-26 03:59:14.000000 spyderwebb-1.0.2/setup.cfg
--rw-r--r--   0 nidever    (503) staff       (20)      624 2022-11-26 03:59:13.000000 spyderwebb-1.0.2/setup.py
+drwxr-xr-x   0 nidever    (503) staff       (20)        0 2023-08-08 19:11:11.000000 spyderwebb-1.0.3/
+-rw-r--r--   0 nidever    (503) staff       (20)     1070 2022-11-23 16:27:48.000000 spyderwebb-1.0.3/LICENSE
+-rw-r--r--   0 nidever    (503) staff       (20)       59 2022-11-23 16:30:43.000000 spyderwebb-1.0.3/MANIFEST.in
+-rw-r--r--   0 nidever    (503) staff       (20)     1131 2023-08-08 19:11:11.000000 spyderwebb-1.0.3/PKG-INFO
+-rw-r--r--   0 nidever    (503) staff       (20)      719 2022-11-23 16:30:20.000000 spyderwebb-1.0.3/README.rst
+drwxr-xr-x   0 nidever    (503) staff       (20)        0 2023-08-08 19:11:11.000000 spyderwebb-1.0.3/bin/
+-rwxr-xr-x   0 nidever    (503) staff       (20)    11751 2022-11-23 16:26:40.000000 spyderwebb-1.0.3/bin/spyderwebb
+drwxr-xr-x   0 nidever    (503) staff       (20)        0 2023-08-08 19:11:11.000000 spyderwebb-1.0.3/docs/
+-rw-r--r--   0 nidever    (503) staff       (20)      634 2021-06-04 00:23:25.000000 spyderwebb-1.0.3/docs/Makefile
+drwxr-xr-x   0 nidever    (503) staff       (20)        0 2023-08-08 19:11:11.000000 spyderwebb-1.0.3/docs/_static/
+-rw-r--r--   0 nidever    (503) staff       (20)      331 2021-06-04 00:24:28.000000 spyderwebb-1.0.3/docs/_static/spyderwebb.css
+-rw-r--r--   0 nidever    (503) staff       (20)     7989 2022-11-23 16:34:02.000000 spyderwebb-1.0.3/docs/conf.py
+-rw-r--r--   0 nidever    (503) staff       (20)    14771 2021-06-05 21:25:39.000000 spyderwebb-1.0.3/docs/examples.rst
+-rw-r--r--   0 nidever    (503) staff       (20)    12185 2021-06-05 18:20:14.000000 spyderwebb-1.0.3/docs/gettingstarted.rst
+-rw-r--r--   0 nidever    (503) staff       (20)     5469 2021-09-26 03:48:35.000000 spyderwebb-1.0.3/docs/index.rst
+-rw-r--r--   0 nidever    (503) staff       (20)      402 2022-11-23 16:33:13.000000 spyderwebb-1.0.3/docs/install.rst
+-rw-r--r--   0 nidever    (503) staff       (20)      795 2021-06-04 00:23:25.000000 spyderwebb-1.0.3/docs/make.bat
+-rw-r--r--   0 nidever    (503) staff       (20)       69 2021-06-04 00:23:25.000000 spyderwebb-1.0.3/docs/requirements.txt
+-rw-r--r--   0 nidever    (503) staff       (20)      149 2022-11-23 16:26:33.000000 spyderwebb-1.0.3/environment.yml
+drwxr-xr-x   0 nidever    (503) staff       (20)        0 2023-08-08 19:11:11.000000 spyderwebb-1.0.3/python/
+drwxr-xr-x   0 nidever    (503) staff       (20)        0 2023-08-08 19:11:11.000000 spyderwebb-1.0.3/python/spyderwebb/
+-rw-r--r--   0 nidever    (503) staff       (20)      150 2023-08-08 19:11:06.000000 spyderwebb-1.0.3/python/spyderwebb/__init__.py
+-rw-r--r--   0 nidever    (503) staff       (20)    30707 2023-02-09 05:28:50.000000 spyderwebb-1.0.3/python/spyderwebb/analyze.py
+drwxr-xr-x   0 nidever    (503) staff       (20)        0 2023-08-08 19:11:11.000000 spyderwebb-1.0.3/python/spyderwebb/data/
+-rw-r--r--   0 nidever    (503) staff       (20)  2327450 2023-02-08 01:40:12.000000 spyderwebb-1.0.3/python/spyderwebb/data/apogeedr17_rgb_feh_ann.npz
+-rw-r--r--   0 nidever    (503) staff       (20)  2382482 2023-02-08 01:40:12.000000 spyderwebb-1.0.3/python/spyderwebb/data/apogeedr17_rgb_logg_ann.npz
+-rw-r--r--   0 nidever    (503) staff       (20)     2874 2023-02-05 22:14:19.000000 spyderwebb-1.0.3/python/spyderwebb/data/extinctions.txt
+-rw-r--r--   0 nidever    (503) staff       (20)     1970 2023-02-05 22:16:03.000000 spyderwebb-1.0.3/python/spyderwebb/extinction.py
+-rw-r--r--   0 nidever    (503) staff       (20)    54515 2023-07-14 05:36:33.000000 spyderwebb-1.0.3/python/spyderwebb/extract.py
+-rw-r--r--   0 nidever    (503) staff       (20)    37815 2023-02-08 18:29:32.000000 spyderwebb-1.0.3/python/spyderwebb/ferre.py
+-rw-r--r--   0 nidever    (503) staff       (20)    13724 2022-12-15 05:46:52.000000 spyderwebb-1.0.3/python/spyderwebb/fluxing.py
+-rw-r--r--   0 nidever    (503) staff       (20)    11621 2023-02-06 18:17:04.000000 spyderwebb-1.0.3/python/spyderwebb/photter.py
+-rw-r--r--   0 nidever    (503) staff       (20)     9997 2022-12-11 17:15:34.000000 spyderwebb-1.0.3/python/spyderwebb/qa.py
+-rw-r--r--   0 nidever    (503) staff       (20)    33186 2023-07-29 07:19:02.000000 spyderwebb-1.0.3/python/spyderwebb/reduce.py
+-rw-r--r--   0 nidever    (503) staff       (20)     1332 2023-01-25 20:54:10.000000 spyderwebb-1.0.3/python/spyderwebb/simulate.py
+-rw-r--r--   0 nidever    (503) staff       (20)     1719 2022-11-26 21:15:39.000000 spyderwebb-1.0.3/python/spyderwebb/sincint.py
+-rw-r--r--   0 nidever    (503) staff       (20)     9582 2023-02-05 22:22:04.000000 spyderwebb-1.0.3/python/spyderwebb/utils.py
+drwxr-xr-x   0 nidever    (503) staff       (20)        0 2023-08-08 19:11:11.000000 spyderwebb-1.0.3/python/spyderwebb.egg-info/
+-rw-r--r--   0 nidever    (503) staff       (20)     1131 2023-08-08 19:11:10.000000 spyderwebb-1.0.3/python/spyderwebb.egg-info/PKG-INFO
+-rw-r--r--   0 nidever    (503) staff       (20)     1010 2023-08-08 19:11:10.000000 spyderwebb-1.0.3/python/spyderwebb.egg-info/SOURCES.txt
+-rw-r--r--   0 nidever    (503) staff       (20)        1 2023-08-08 19:11:10.000000 spyderwebb-1.0.3/python/spyderwebb.egg-info/dependency_links.txt
+-rw-r--r--   0 nidever    (503) staff       (20)        1 2023-08-08 19:11:10.000000 spyderwebb-1.0.3/python/spyderwebb.egg-info/not-zip-safe
+-rw-r--r--   0 nidever    (503) staff       (20)      125 2023-08-08 19:11:10.000000 spyderwebb-1.0.3/python/spyderwebb.egg-info/requires.txt
+-rw-r--r--   0 nidever    (503) staff       (20)       11 2023-08-08 19:11:10.000000 spyderwebb-1.0.3/python/spyderwebb.egg-info/top_level.txt
+-rw-r--r--   0 nidever    (503) staff       (20)       49 2022-11-23 16:26:33.000000 spyderwebb-1.0.3/requirements-dev.txt
+-rw-r--r--   0 nidever    (503) staff       (20)       36 2022-11-23 16:31:02.000000 spyderwebb-1.0.3/requirements.txt
+-rw-r--r--   0 nidever    (503) staff       (20)     1147 2023-08-08 19:11:11.000000 spyderwebb-1.0.3/setup.cfg
+-rw-r--r--   0 nidever    (503) staff       (20)      624 2023-08-08 19:11:09.000000 spyderwebb-1.0.3/setup.py
```

### Comparing `spyderwebb-1.0.2/LICENSE` & `spyderwebb-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `spyderwebb-1.0.2/PKG-INFO` & `spyderwebb-1.0.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spyderwebb
-Version: 1.0.2
+Version: 1.0.3
 Summary: JWST NIRSpec reduction software
 Home-page: https://github.com/dnidever/spyderwebb
 Author: David Nidever
 Author-email: dnidever@montana.edu
 License: MIT
 Requires: numpy
 Requires: astropy(>=4.0)
```

### Comparing `spyderwebb-1.0.2/README.rst` & `spyderwebb-1.0.3/README.rst`

 * *Files identical despite different names*

### Comparing `spyderwebb-1.0.2/bin/spyderwebb` & `spyderwebb-1.0.3/bin/spyderwebb`

 * *Files identical despite different names*

### Comparing `spyderwebb-1.0.2/docs/Makefile` & `spyderwebb-1.0.3/docs/Makefile`

 * *Files identical despite different names*

### Comparing `spyderwebb-1.0.2/docs/conf.py` & `spyderwebb-1.0.3/docs/conf.py`

 * *Files identical despite different names*

### Comparing `spyderwebb-1.0.2/docs/examples.rst` & `spyderwebb-1.0.3/docs/examples.rst`

 * *Files identical despite different names*

### Comparing `spyderwebb-1.0.2/docs/gettingstarted.rst` & `spyderwebb-1.0.3/docs/gettingstarted.rst`

 * *Files identical despite different names*

### Comparing `spyderwebb-1.0.2/docs/index.rst` & `spyderwebb-1.0.3/docs/index.rst`

 * *Files identical despite different names*

### Comparing `spyderwebb-1.0.2/docs/make.bat` & `spyderwebb-1.0.3/docs/make.bat`

 * *Files identical despite different names*

### Comparing `spyderwebb-1.0.2/python/spyderwebb.egg-info/PKG-INFO` & `spyderwebb-1.0.3/python/spyderwebb.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spyderwebb
-Version: 1.0.2
+Version: 1.0.3
 Summary: JWST NIRSpec reduction software
 Home-page: https://github.com/dnidever/spyderwebb
 Author: David Nidever
 Author-email: dnidever@montana.edu
 License: MIT
 Requires: numpy
 Requires: astropy(>=4.0)
```

### Comparing `spyderwebb-1.0.2/setup.cfg` & `spyderwebb-1.0.3/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 license_file = LICENSE
 url = https://github.com/dnidever/spyderwebb
 description = JWST NIRSpec reduction software
 long_description = file: README.rst
 long_description_content_type = text/x-rst
 edit_on_github = False
 github_project = dnidever/spyderwebb
-version = 1.0.2
+version = 1.0.3
 
 [options]
 zip_safe = False
 packages = find:
 python_requires = >=3.6
 setup_requires = 
 	setuptools_scm
```

### Comparing `spyderwebb-1.0.2/setup.py` & `spyderwebb-1.0.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import os
 import sys
 import shutil
 from setuptools import setup, find_packages, find_namespace_packages
 from setuptools.command.install import install
 
 setup(name='spyderwebb',
-      version='1.0.2',
+      version='1.0.3',
       description='JWST NIRSpec reduction software',
       author='David Nidever',
       author_email='dnidever@montana.edu',
       url='https://github.com/dnidever/spyderwebb',
       scripts=['bin/spyderwebb'],
       requires=['numpy','astropy(>=4.0)','scipy','jwst'],
       zip_safe = False,
```


# Comparing `tmp/coffea_casa-2023.4.5.tar.gz` & `tmp/coffea_casa-2023.8.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "coffea_casa-2023.4.5.tar", last modified: Wed Apr  5 16:24:40 2023, max compression
+gzip compressed data, was "coffea_casa-2023.8.8.tar", last modified: Tue Aug  8 16:20:50 2023, max compression
```

## Comparing `coffea_casa-2023.4.5.tar` & `coffea_casa-2023.8.8.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 16:24:40.717076 coffea_casa-2023.4.5/
--rw-r--r--   0 runner    (1001) docker     (123)     1507 2023-04-05 16:24:20.000000 coffea_casa-2023.4.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      250 2023-04-05 16:24:20.000000 coffea_casa-2023.4.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     7592 2023-04-05 16:24:40.717076 coffea_casa-2023.4.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6401 2023-04-05 16:24:20.000000 coffea_casa-2023.4.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 16:24:40.717076 coffea_casa-2023.4.5/coffea_casa/
--rw-r--r--   0 runner    (1001) docker     (123)      429 2023-04-05 16:24:20.000000 coffea_casa-2023.4.5/coffea_casa/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      502 2023-04-05 16:24:40.717076 coffea_casa-2023.4.5/coffea_casa/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     8496 2023-04-05 16:24:20.000000 coffea_casa-2023.4.5/coffea_casa/coffea_casa.py
--rw-r--r--   0 runner    (1001) docker     (123)      344 2023-04-05 16:24:20.000000 coffea_casa-2023.4.5/coffea_casa/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1289 2023-04-05 16:24:20.000000 coffea_casa-2023.4.5/coffea_casa/jobqueue-coffea-casa.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     4595 2023-04-05 16:24:20.000000 coffea_casa-2023.4.5/coffea_casa/plugin.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 16:24:40.717076 coffea_casa-2023.4.5/coffea_casa.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7592 2023-04-05 16:24:40.000000 coffea_casa-2023.4.5/coffea_casa.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      444 2023-04-05 16:24:40.000000 coffea_casa-2023.4.5/coffea_casa.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-04-05 16:24:40.000000 coffea_casa-2023.4.5/coffea_casa.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-05 16:24:40.000000 coffea_casa-2023.4.5/coffea_casa.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      325 2023-04-05 16:24:40.000000 coffea_casa-2023.4.5/coffea_casa.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-05 16:24:40.000000 coffea_casa-2023.4.5/coffea_casa.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-05 16:24:20.000000 coffea_casa-2023.4.5/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      484 2023-04-05 16:24:40.717076 coffea_casa-2023.4.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2453 2023-04-05 16:24:20.000000 coffea_casa-2023.4.5/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)    68611 2023-04-05 16:24:20.000000 coffea_casa-2023.4.5/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 16:20:50.380602 coffea_casa-2023.8.8/
+-rw-r--r--   0 runner    (1001) docker     (123)     1507 2023-08-08 16:20:37.000000 coffea_casa-2023.8.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      250 2023-08-08 16:20:37.000000 coffea_casa-2023.8.8/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     7592 2023-08-08 16:20:50.380602 coffea_casa-2023.8.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6401 2023-08-08 16:20:37.000000 coffea_casa-2023.8.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 16:20:50.380602 coffea_casa-2023.8.8/coffea_casa/
+-rw-r--r--   0 runner    (1001) docker     (123)      429 2023-08-08 16:20:37.000000 coffea_casa-2023.8.8/coffea_casa/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      502 2023-08-08 16:20:50.380602 coffea_casa-2023.8.8/coffea_casa/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8496 2023-08-08 16:20:37.000000 coffea_casa-2023.8.8/coffea_casa/coffea_casa.py
+-rw-r--r--   0 runner    (1001) docker     (123)      344 2023-08-08 16:20:37.000000 coffea_casa-2023.8.8/coffea_casa/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1289 2023-08-08 16:20:37.000000 coffea_casa-2023.8.8/coffea_casa/jobqueue-coffea-casa.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     4595 2023-08-08 16:20:37.000000 coffea_casa-2023.8.8/coffea_casa/plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 16:20:50.380602 coffea_casa-2023.8.8/coffea_casa.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7592 2023-08-08 16:20:50.000000 coffea_casa-2023.8.8/coffea_casa.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      444 2023-08-08 16:20:50.000000 coffea_casa-2023.8.8/coffea_casa.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-08-08 16:20:50.000000 coffea_casa-2023.8.8/coffea_casa.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 16:20:50.000000 coffea_casa-2023.8.8/coffea_casa.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      325 2023-08-08 16:20:50.000000 coffea_casa-2023.8.8/coffea_casa.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-08-08 16:20:50.000000 coffea_casa-2023.8.8/coffea_casa.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 16:20:37.000000 coffea_casa-2023.8.8/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      484 2023-08-08 16:20:50.380602 coffea_casa-2023.8.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2453 2023-08-08 16:20:37.000000 coffea_casa-2023.8.8/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)    68611 2023-08-08 16:20:37.000000 coffea_casa-2023.8.8/versioneer.py
```

### Comparing `coffea_casa-2023.4.5/LICENSE` & `coffea_casa-2023.8.8/LICENSE`

 * *Files identical despite different names*

### Comparing `coffea_casa-2023.4.5/PKG-INFO` & `coffea_casa-2023.8.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: coffea_casa
-Version: 2023.4.5
+Version: 2023.8.8
 Summary: A Prototype U.S. CMS analysis facility
 Home-page: http://github.com/CoffeaTeam/coffea-casa.git
 Author: UNL
 Author-email: oksana.shadura@cern.ch
 License: BSD-3-Clause License
 Platform: Any
 Classifier: Development Status :: 4 - Beta
```

### Comparing `coffea_casa-2023.4.5/README.md` & `coffea_casa-2023.8.8/README.md`

 * *Files identical despite different names*

### Comparing `coffea_casa-2023.4.5/coffea_casa/coffea_casa.py` & `coffea_casa-2023.8.8/coffea_casa/coffea_casa.py`

 * *Files identical despite different names*

### Comparing `coffea_casa-2023.4.5/coffea_casa/jobqueue-coffea-casa.yaml` & `coffea_casa-2023.8.8/coffea_casa/jobqueue-coffea-casa.yaml`

 * *Files identical despite different names*

### Comparing `coffea_casa-2023.4.5/coffea_casa/plugin.py` & `coffea_casa-2023.8.8/coffea_casa/plugin.py`

 * *Files identical despite different names*

### Comparing `coffea_casa-2023.4.5/coffea_casa.egg-info/PKG-INFO` & `coffea_casa-2023.8.8/coffea_casa.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: coffea-casa
-Version: 2023.4.5
+Version: 2023.8.8
 Summary: A Prototype U.S. CMS analysis facility
 Home-page: http://github.com/CoffeaTeam/coffea-casa.git
 Author: UNL
 Author-email: oksana.shadura@cern.ch
 License: BSD-3-Clause License
 Platform: Any
 Classifier: Development Status :: 4 - Beta
```

### Comparing `coffea_casa-2023.4.5/setup.py` & `coffea_casa-2023.8.8/setup.py`

 * *Files identical despite different names*

### Comparing `coffea_casa-2023.4.5/versioneer.py` & `coffea_casa-2023.8.8/versioneer.py`

 * *Files identical despite different names*


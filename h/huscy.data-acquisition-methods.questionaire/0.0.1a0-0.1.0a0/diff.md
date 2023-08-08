# Comparing `tmp/huscy.data-acquisition-methods.questionaire-0.0.1a0.tar.gz` & `tmp/huscy.data-acquisition-methods.questionaire-0.1.0a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "huscy.data-acquisition-methods.questionaire-0.0.1a0.tar", last modified: Tue Aug  8 09:34:04 2023, max compression
+gzip compressed data, was "huscy.data-acquisition-methods.questionaire-0.1.0a0.tar", last modified: Tue Aug  8 13:55:58 2023, max compression
```

## Comparing `huscy.data-acquisition-methods.questionaire-0.0.1a0.tar` & `huscy.data-acquisition-methods.questionaire-0.1.0a0.tar`

### file list

```diff
@@ -1,16 +1,24 @@
-drwxrwxr-x   0 lotus     (1000) lotus     (1000)        0 2023-08-08 09:34:03.991515 huscy.data-acquisition-methods.questionaire-0.0.1a0/
--rw-rw-r--   0 lotus     (1000) lotus     (1000)     1104 2023-08-08 09:34:03.991515 huscy.data-acquisition-methods.questionaire-0.0.1a0/PKG-INFO
--rw-rw-r--   0 lotus     (1000) lotus     (1000)       46 2023-08-04 10:51:53.000000 huscy.data-acquisition-methods.questionaire-0.0.1a0/README.md
-drwxrwxr-x   0 lotus     (1000) lotus     (1000)        0 2023-08-08 09:34:03.991515 huscy.data-acquisition-methods.questionaire-0.0.1a0/huscy/
-drwxrwxr-x   0 lotus     (1000) lotus     (1000)        0 2023-08-08 09:34:03.991515 huscy.data-acquisition-methods.questionaire-0.0.1a0/huscy/data_acquisition_methods/
-drwxrwxr-x   0 lotus     (1000) lotus     (1000)        0 2023-08-08 09:34:03.991515 huscy.data-acquisition-methods.questionaire-0.0.1a0/huscy/data_acquisition_methods/questionaire/
--rw-rw-r--   0 lotus     (1000) lotus     (1000)      166 2023-08-08 09:34:00.000000 huscy.data-acquisition-methods.questionaire-0.0.1a0/huscy/data_acquisition_methods/questionaire/__init__.py
--rw-rw-r--   0 lotus     (1000) lotus     (1000)      215 2023-08-08 09:33:33.000000 huscy.data-acquisition-methods.questionaire-0.0.1a0/huscy/data_acquisition_methods/questionaire/apps.py
-drwxrwxr-x   0 lotus     (1000) lotus     (1000)        0 2023-08-08 09:34:03.991515 huscy.data-acquisition-methods.questionaire-0.0.1a0/huscy.data_acquisition_methods.questionaire.egg-info/
--rw-rw-r--   0 lotus     (1000) lotus     (1000)     1104 2023-08-08 09:34:03.000000 huscy.data-acquisition-methods.questionaire-0.0.1a0/huscy.data_acquisition_methods.questionaire.egg-info/PKG-INFO
--rw-rw-r--   0 lotus     (1000) lotus     (1000)      460 2023-08-08 09:34:03.000000 huscy.data-acquisition-methods.questionaire-0.0.1a0/huscy.data_acquisition_methods.questionaire.egg-info/SOURCES.txt
--rw-rw-r--   0 lotus     (1000) lotus     (1000)        1 2023-08-08 09:34:03.000000 huscy.data-acquisition-methods.questionaire-0.0.1a0/huscy.data_acquisition_methods.questionaire.egg-info/dependency_links.txt
--rw-rw-r--   0 lotus     (1000) lotus     (1000)       81 2023-08-08 09:34:03.000000 huscy.data-acquisition-methods.questionaire-0.0.1a0/huscy.data_acquisition_methods.questionaire.egg-info/requires.txt
--rw-rw-r--   0 lotus     (1000) lotus     (1000)        6 2023-08-08 09:34:03.000000 huscy.data-acquisition-methods.questionaire-0.0.1a0/huscy.data_acquisition_methods.questionaire.egg-info/top_level.txt
--rw-rw-r--   0 lotus     (1000) lotus     (1000)       38 2023-08-08 09:34:03.991515 huscy.data-acquisition-methods.questionaire-0.0.1a0/setup.cfg
--rw-rw-r--   0 lotus     (1000) lotus     (1000)     1588 2023-08-07 07:55:53.000000 huscy.data-acquisition-methods.questionaire-0.0.1a0/setup.py
+drwxr-xr-x   0 jenkins    (111) jenkins    (115)        0 2023-08-08 13:55:58.968506 huscy.data-acquisition-methods.questionaire-0.1.0a0/
+-rw-r--r--   0 jenkins    (111) jenkins    (115)     1123 2023-08-08 13:55:58.968506 huscy.data-acquisition-methods.questionaire-0.1.0a0/PKG-INFO
+-rw-r--r--   0 jenkins    (111) jenkins    (115)       46 2023-08-08 12:21:09.000000 huscy.data-acquisition-methods.questionaire-0.1.0a0/README.md
+drwxr-xr-x   0 jenkins    (111) jenkins    (115)        0 2023-08-08 13:55:58.968506 huscy.data-acquisition-methods.questionaire-0.1.0a0/huscy/
+drwxr-xr-x   0 jenkins    (111) jenkins    (115)        0 2023-08-08 13:55:58.968506 huscy.data-acquisition-methods.questionaire-0.1.0a0/huscy/data_acquisition_methods/
+drwxr-xr-x   0 jenkins    (111) jenkins    (115)        0 2023-08-08 13:55:58.968506 huscy.data-acquisition-methods.questionaire-0.1.0a0/huscy/data_acquisition_methods/questionaire/
+-rw-r--r--   0 jenkins    (111) jenkins    (115)      166 2023-08-08 12:21:09.000000 huscy.data-acquisition-methods.questionaire-0.1.0a0/huscy/data_acquisition_methods/questionaire/__init__.py
+-rw-r--r--   0 jenkins    (111) jenkins    (115)      497 2023-08-08 12:21:09.000000 huscy.data-acquisition-methods.questionaire-0.1.0a0/huscy/data_acquisition_methods/questionaire/apps.py
+drwxr-xr-x   0 jenkins    (111) jenkins    (115)        0 2023-08-08 13:55:58.968506 huscy.data-acquisition-methods.questionaire-0.1.0a0/huscy/data_acquisition_methods/questionaire/migrations/
+-rw-r--r--   0 jenkins    (111) jenkins    (115)     1115 2023-08-08 13:55:57.000000 huscy.data-acquisition-methods.questionaire-0.1.0a0/huscy/data_acquisition_methods/questionaire/migrations/0001_initial.py
+-rw-r--r--   0 jenkins    (111) jenkins    (115)        0 2023-08-08 12:21:09.000000 huscy.data-acquisition-methods.questionaire-0.1.0a0/huscy/data_acquisition_methods/questionaire/migrations/__init__.py
+-rw-r--r--   0 jenkins    (111) jenkins    (115)      779 2023-08-08 12:21:09.000000 huscy.data-acquisition-methods.questionaire-0.1.0a0/huscy/data_acquisition_methods/questionaire/models.py
+-rw-r--r--   0 jenkins    (111) jenkins    (115)     1038 2023-08-08 12:21:09.000000 huscy.data-acquisition-methods.questionaire-0.1.0a0/huscy/data_acquisition_methods/questionaire/serializer.py
+-rw-r--r--   0 jenkins    (111) jenkins    (115)     1160 2023-08-08 12:21:09.000000 huscy.data-acquisition-methods.questionaire-0.1.0a0/huscy/data_acquisition_methods/questionaire/services.py
+-rw-r--r--   0 jenkins    (111) jenkins    (115)      279 2023-08-08 12:21:09.000000 huscy.data-acquisition-methods.questionaire-0.1.0a0/huscy/data_acquisition_methods/questionaire/urls.py
+-rw-r--r--   0 jenkins    (111) jenkins    (115)     1129 2023-08-08 12:21:09.000000 huscy.data-acquisition-methods.questionaire-0.1.0a0/huscy/data_acquisition_methods/questionaire/views.py
+drwxr-xr-x   0 jenkins    (111) jenkins    (115)        0 2023-08-08 13:55:58.968506 huscy.data-acquisition-methods.questionaire-0.1.0a0/huscy.data_acquisition_methods.questionaire.egg-info/
+-rw-r--r--   0 jenkins    (111) jenkins    (115)     1123 2023-08-08 13:55:58.000000 huscy.data-acquisition-methods.questionaire-0.1.0a0/huscy.data_acquisition_methods.questionaire.egg-info/PKG-INFO
+-rw-r--r--   0 jenkins    (111) jenkins    (115)      871 2023-08-08 13:55:58.000000 huscy.data-acquisition-methods.questionaire-0.1.0a0/huscy.data_acquisition_methods.questionaire.egg-info/SOURCES.txt
+-rw-r--r--   0 jenkins    (111) jenkins    (115)        1 2023-08-08 13:55:58.000000 huscy.data-acquisition-methods.questionaire-0.1.0a0/huscy.data_acquisition_methods.questionaire.egg-info/dependency_links.txt
+-rw-r--r--   0 jenkins    (111) jenkins    (115)       81 2023-08-08 13:55:58.000000 huscy.data-acquisition-methods.questionaire-0.1.0a0/huscy.data_acquisition_methods.questionaire.egg-info/requires.txt
+-rw-r--r--   0 jenkins    (111) jenkins    (115)        6 2023-08-08 13:55:58.000000 huscy.data-acquisition-methods.questionaire-0.1.0a0/huscy.data_acquisition_methods.questionaire.egg-info/top_level.txt
+-rw-r--r--   0 jenkins    (111) jenkins    (115)       38 2023-08-08 13:55:58.968506 huscy.data-acquisition-methods.questionaire-0.1.0a0/setup.cfg
+-rw-r--r--   0 jenkins    (111) jenkins    (115)     1588 2023-08-08 12:21:09.000000 huscy.data-acquisition-methods.questionaire-0.1.0a0/setup.py
```

### Comparing `huscy.data-acquisition-methods.questionaire-0.0.1a0/PKG-INFO` & `huscy.data-acquisition-methods.questionaire-0.1.0a0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 Metadata-Version: 2.1
 Name: huscy.data-acquisition-methods.questionaire
-Version: 0.0.1a0
+Version: 0.1.0a0
 Summary: UNKNOWN
 Home-page: https://bitbucket.org/huscy/data_acquisition_methods.questionaire
 Author: Stefan Bunde
 Author-email: stefanbunde+git@posteo.de
 License: AGPLv3+
+Description: # huscy.data-acquisition-methods.questionaire
+        
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
@@ -20,11 +22,7 @@
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 3.2
 Classifier: Framework :: Django :: 4.1
 Classifier: Framework :: Django :: 4.2
 Description-Content-Type: text/markdown
 Provides-Extra: development
 Provides-Extra: testing
-
-# huscy.data-acquisition-methods.questionaire
-
-
```

### Comparing `huscy.data-acquisition-methods.questionaire-0.0.1a0/huscy.data_acquisition_methods.questionaire.egg-info/PKG-INFO` & `huscy.data-acquisition-methods.questionaire-0.1.0a0/huscy.data_acquisition_methods.questionaire.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 Metadata-Version: 2.1
 Name: huscy.data-acquisition-methods.questionaire
-Version: 0.0.1a0
+Version: 0.1.0a0
 Summary: UNKNOWN
 Home-page: https://bitbucket.org/huscy/data_acquisition_methods.questionaire
 Author: Stefan Bunde
 Author-email: stefanbunde+git@posteo.de
 License: AGPLv3+
+Description: # huscy.data-acquisition-methods.questionaire
+        
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
@@ -20,11 +22,7 @@
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 3.2
 Classifier: Framework :: Django :: 4.1
 Classifier: Framework :: Django :: 4.2
 Description-Content-Type: text/markdown
 Provides-Extra: development
 Provides-Extra: testing
-
-# huscy.data-acquisition-methods.questionaire
-
-
```

### Comparing `huscy.data-acquisition-methods.questionaire-0.0.1a0/setup.py` & `huscy.data-acquisition-methods.questionaire-0.1.0a0/setup.py`

 * *Files identical despite different names*


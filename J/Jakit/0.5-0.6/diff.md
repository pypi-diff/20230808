# Comparing `tmp/Jakit-0.5.tar.gz` & `tmp/Jakit-0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Jakit-0.5.tar", last modified: Fri Aug  4 11:24:40 2023, max compression
+gzip compressed data, was "Jakit-0.6.tar", last modified: Tue Aug  8 09:11:02 2023, max compression
```

## Comparing `Jakit-0.5.tar` & `Jakit-0.6.tar`

### file list

```diff
@@ -1,14 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-08-04 11:24:40.483662 Jakit-0.5/
-drwxrwxrwx   0        0        0        0 2023-08-04 11:24:40.461665 Jakit-0.5/Jakit/
--rw-rw-rw-   0        0        0       33 2023-08-01 16:54:21.000000 Jakit-0.5/Jakit/__init__.py
--rw-rw-rw-   0        0        0     2984 2023-08-04 11:23:54.000000 Jakit-0.5/Jakit/jakit_jobs.py
-drwxrwxrwx   0        0        0        0 2023-08-04 11:24:40.476658 Jakit-0.5/Jakit.egg-info/
--rw-rw-rw-   0        0        0      523 2023-08-04 11:24:40.000000 Jakit-0.5/Jakit.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      180 2023-08-04 11:24:40.000000 Jakit-0.5/Jakit.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-04 11:24:40.000000 Jakit-0.5/Jakit.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2023-08-04 11:24:40.000000 Jakit-0.5/Jakit.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1065 2023-07-31 10:27:48.000000 Jakit-0.5/LICENSE
--rw-rw-rw-   0        0        0      523 2023-08-04 11:24:40.482662 Jakit-0.5/PKG-INFO
--rw-rw-rw-   0        0        0       69 2023-07-31 10:27:48.000000 Jakit-0.5/README.md
--rw-rw-rw-   0        0        0       42 2023-08-04 11:24:40.484663 Jakit-0.5/setup.cfg
--rw-rw-rw-   0        0        0      658 2023-08-04 11:24:17.000000 Jakit-0.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-08 09:11:02.570613 Jakit-0.6/
+drwxrwxrwx   0        0        0        0 2023-08-08 09:11:02.546615 Jakit-0.6/Jakit/
+-rw-rw-rw-   0        0        0       33 2023-08-01 16:54:21.000000 Jakit-0.6/Jakit/__init__.py
+-rw-rw-rw-   0        0        0      139 2023-08-08 09:04:41.000000 Jakit-0.6/Jakit/app.py
+-rw-rw-rw-   0        0        0        0 2023-08-08 09:04:41.000000 Jakit-0.6/Jakit/error_handler.py
+-rw-rw-rw-   0        0        0     5429 2023-08-08 09:04:41.000000 Jakit-0.6/Jakit/jakit_jobs.py
+drwxrwxrwx   0        0        0        0 2023-08-08 09:11:02.567615 Jakit-0.6/Jakit.egg-info/
+-rw-rw-rw-   0        0        0      523 2023-08-08 09:11:02.000000 Jakit-0.6/Jakit.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      244 2023-08-08 09:11:02.000000 Jakit-0.6/Jakit.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-08 09:11:02.000000 Jakit-0.6/Jakit.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      420 2023-08-08 09:11:02.000000 Jakit-0.6/Jakit.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-08-08 09:11:02.000000 Jakit-0.6/Jakit.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1065 2023-07-31 10:27:48.000000 Jakit-0.6/LICENSE
+-rw-rw-rw-   0        0        0      523 2023-08-08 09:11:02.569613 Jakit-0.6/PKG-INFO
+-rw-rw-rw-   0        0        0       69 2023-07-31 10:27:48.000000 Jakit-0.6/README.md
+-rw-rw-rw-   0        0        0       42 2023-08-08 09:11:02.570613 Jakit-0.6/setup.cfg
+-rw-rw-rw-   0        0        0     1595 2023-08-08 09:10:55.000000 Jakit-0.6/setup.py
```

### Comparing `Jakit-0.5/Jakit.egg-info/PKG-INFO` & `Jakit-0.6/Jakit.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Jakit
-Version: 0.5
+Version: 0.6
 Summary: Just Another Kappa Information Tool
 Home-page: https://github.com/iddy-ani/Jakit
 Author: Idriss Animashaun
 Author-email: idriss.animashaun@intel.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `Jakit-0.5/LICENSE` & `Jakit-0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `Jakit-0.5/PKG-INFO` & `Jakit-0.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Jakit
-Version: 0.5
+Version: 0.6
 Summary: Just Another Kappa Information Tool
 Home-page: https://github.com/iddy-ani/Jakit
 Author: Idriss Animashaun
 Author-email: idriss.animashaun@intel.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```


# Comparing `tmp/mantellum-1.0.3.tar.gz` & `tmp/mantellum-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mantellum-1.0.3.tar", last modified: Wed Apr  5 14:01:17 2023, max compression
+gzip compressed data, was "mantellum-1.0.4.tar", last modified: Tue Aug  8 11:18:18 2023, max compression
```

## Comparing `mantellum-1.0.3.tar` & `mantellum-1.0.4.tar`

### file list

```diff
@@ -1,17 +1,21 @@
-drwxrwxr-x   0 nicc777   (1000) nicc777   (1000)        0 2023-04-05 14:01:17.219144 mantellum-1.0.3/
--rw-rw-r--   0 nicc777   (1000) nicc777   (1000)     1069 2023-04-05 05:14:26.000000 mantellum-1.0.3/LICENSE
--rw-rw-r--   0 nicc777   (1000) nicc777   (1000)     1112 2023-04-05 14:01:17.219144 mantellum-1.0.3/PKG-INFO
--rw-rw-r--   0 nicc777   (1000) nicc777   (1000)      155 2023-04-05 09:28:05.000000 mantellum-1.0.3/README.md
--rw-rw-r--   0 nicc777   (1000) nicc777   (1000)       80 2023-04-05 09:20:26.000000 mantellum-1.0.3/pyproject.toml
--rw-rw-r--   0 nicc777   (1000) nicc777   (1000)      983 2023-04-05 14:01:17.219144 mantellum-1.0.3/setup.cfg
-drwxrwxr-x   0 nicc777   (1000) nicc777   (1000)        0 2023-04-05 14:01:17.215144 mantellum-1.0.3/src/
-drwxrwxr-x   0 nicc777   (1000) nicc777   (1000)        0 2023-04-05 14:01:17.219144 mantellum-1.0.3/src/mantellum/
--rw-rw-r--   0 nicc777   (1000) nicc777   (1000)        0 2023-04-05 05:14:26.000000 mantellum-1.0.3/src/mantellum/__init__.py
--rw-rw-r--   0 nicc777   (1000) nicc777   (1000)      263 2023-04-05 05:14:26.000000 mantellum-1.0.3/src/mantellum/date_and_time_utils.py
--rw-rw-r--   0 nicc777   (1000) nicc777   (1000)     2303 2023-04-05 05:14:26.000000 mantellum-1.0.3/src/mantellum/decorators.py
--rw-rw-r--   0 nicc777   (1000) nicc777   (1000)     1461 2023-04-05 14:00:47.000000 mantellum-1.0.3/src/mantellum/logging_utils.py
-drwxrwxr-x   0 nicc777   (1000) nicc777   (1000)        0 2023-04-05 14:01:17.219144 mantellum-1.0.3/src/mantellum.egg-info/
--rw-rw-r--   0 nicc777   (1000) nicc777   (1000)     1112 2023-04-05 14:01:17.000000 mantellum-1.0.3/src/mantellum.egg-info/PKG-INFO
--rw-rw-r--   0 nicc777   (1000) nicc777   (1000)      312 2023-04-05 14:01:17.000000 mantellum-1.0.3/src/mantellum.egg-info/SOURCES.txt
--rw-rw-r--   0 nicc777   (1000) nicc777   (1000)        1 2023-04-05 14:01:17.000000 mantellum-1.0.3/src/mantellum.egg-info/dependency_links.txt
--rw-rw-r--   0 nicc777   (1000) nicc777   (1000)       10 2023-04-05 14:01:17.000000 mantellum-1.0.3/src/mantellum.egg-info/top_level.txt
+drwxrwxr-x   0 nicc777   (1000) nicc777   (1000)        0 2023-08-08 11:18:18.919011 mantellum-1.0.4/
+-rw-rw-r--   0 nicc777   (1000) nicc777   (1000)     1069 2023-04-05 05:14:26.000000 mantellum-1.0.4/LICENSE
+-rw-rw-r--   0 nicc777   (1000) nicc777   (1000)     1112 2023-08-08 11:18:18.919011 mantellum-1.0.4/PKG-INFO
+-rw-rw-r--   0 nicc777   (1000) nicc777   (1000)      155 2023-04-05 09:28:05.000000 mantellum-1.0.4/README.md
+-rw-rw-r--   0 nicc777   (1000) nicc777   (1000)       80 2023-04-05 09:20:26.000000 mantellum-1.0.4/pyproject.toml
+-rw-rw-r--   0 nicc777   (1000) nicc777   (1000)      983 2023-08-08 11:18:18.919011 mantellum-1.0.4/setup.cfg
+drwxrwxr-x   0 nicc777   (1000) nicc777   (1000)        0 2023-08-08 11:18:18.911011 mantellum-1.0.4/src/
+drwxrwxr-x   0 nicc777   (1000) nicc777   (1000)        0 2023-08-08 11:18:18.915011 mantellum-1.0.4/src/mantellum/
+-rw-rw-r--   0 nicc777   (1000) nicc777   (1000)      375 2023-08-08 11:17:12.000000 mantellum-1.0.4/src/mantellum/__init__.py
+-rw-rw-r--   0 nicc777   (1000) nicc777   (1000)      639 2023-08-08 11:17:12.000000 mantellum-1.0.4/src/mantellum/date_and_time_utils.py
+-rw-rw-r--   0 nicc777   (1000) nicc777   (1000)     4745 2023-08-08 11:17:12.000000 mantellum-1.0.4/src/mantellum/decorators.py
+-rw-rw-r--   0 nicc777   (1000) nicc777   (1000)     1837 2023-08-08 11:17:12.000000 mantellum-1.0.4/src/mantellum/logging_utils.py
+-rw-rw-r--   0 nicc777   (1000) nicc777   (1000)    15500 2023-08-08 11:17:12.000000 mantellum-1.0.4/src/mantellum/metrics.py
+drwxrwxr-x   0 nicc777   (1000) nicc777   (1000)        0 2023-08-08 11:18:18.919011 mantellum-1.0.4/src/mantellum.egg-info/
+-rw-rw-r--   0 nicc777   (1000) nicc777   (1000)     1112 2023-08-08 11:18:18.000000 mantellum-1.0.4/src/mantellum.egg-info/PKG-INFO
+-rw-rw-r--   0 nicc777   (1000) nicc777   (1000)      384 2023-08-08 11:18:18.000000 mantellum-1.0.4/src/mantellum.egg-info/SOURCES.txt
+-rw-rw-r--   0 nicc777   (1000) nicc777   (1000)        1 2023-08-08 11:18:18.000000 mantellum-1.0.4/src/mantellum.egg-info/dependency_links.txt
+-rw-rw-r--   0 nicc777   (1000) nicc777   (1000)       10 2023-08-08 11:18:18.000000 mantellum-1.0.4/src/mantellum.egg-info/top_level.txt
+drwxrwxr-x   0 nicc777   (1000) nicc777   (1000)        0 2023-08-08 11:18:18.919011 mantellum-1.0.4/tests/
+-rw-rw-r--   0 nicc777   (1000) nicc777   (1000)     3935 2023-08-08 11:17:12.000000 mantellum-1.0.4/tests/test_decorators.py
+-rw-rw-r--   0 nicc777   (1000) nicc777   (1000)     3008 2023-08-08 11:17:12.000000 mantellum-1.0.4/tests/test_metrics.py
```

### Comparing `mantellum-1.0.3/LICENSE` & `mantellum-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `mantellum-1.0.3/PKG-INFO` & `mantellum-1.0.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mantellum
-Version: 1.0.3
+Version: 1.0.4
 Summary: Some common utils that might be useful to many Python projects
 Home-page: https://github.com/nicc777/mantellum
 Author: Nico Coetzee
 Author-email: nicc777@gmail.com
 Project-URL: Bug Tracker, https://github.com/nicc777/mantellum/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `mantellum-1.0.3/setup.cfg` & `mantellum-1.0.4/setup.cfg`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = mantellum
-version = 1.0.3
+version = 1.0.4
 author = Nico Coetzee
 author_email = nicc777@gmail.com
 description = Some common utils that might be useful to many Python projects
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/nicc777/mantellum
 project_urls =
```

### Comparing `mantellum-1.0.3/src/mantellum.egg-info/PKG-INFO` & `mantellum-1.0.4/src/mantellum.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mantellum
-Version: 1.0.3
+Version: 1.0.4
 Summary: Some common utils that might be useful to many Python projects
 Home-page: https://github.com/nicc777/mantellum
 Author: Nico Coetzee
 Author-email: nicc777@gmail.com
 Project-URL: Bug Tracker, https://github.com/nicc777/mantellum/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```


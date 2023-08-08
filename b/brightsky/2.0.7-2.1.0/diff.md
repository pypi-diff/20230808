# Comparing `tmp/brightsky-2.0.7.tar.gz` & `tmp/brightsky-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "brightsky-2.0.7.tar", last modified: Mon Jul 10 14:09:30 2023, max compression
+gzip compressed data, was "brightsky-2.1.0.tar", last modified: Tue Aug  8 15:20:44 2023, max compression
```

## Comparing `brightsky-2.0.7.tar` & `brightsky-2.1.0.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 14:09:30.263547 brightsky-2.0.7/
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-07-10 14:09:21.000000 brightsky-2.0.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     8318 2023-07-10 14:09:30.263547 brightsky-2.0.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7713 2023-07-10 14:09:21.000000 brightsky-2.0.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 14:09:30.259547 brightsky-2.0.7/brightsky/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-10 14:09:21.000000 brightsky-2.0.7/brightsky/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      651 2023-07-10 14:09:21.000000 brightsky-2.0.7/brightsky/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4898 2023-07-10 14:09:21.000000 brightsky-2.0.7/brightsky/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     2578 2023-07-10 14:09:21.000000 brightsky-2.0.7/brightsky/db.py
--rw-r--r--   0 runner    (1001) docker     (123)    13531 2023-07-10 14:09:21.000000 brightsky-2.0.7/brightsky/export.py
--rw-r--r--   0 runner    (1001) docker     (123)     7147 2023-07-10 14:09:21.000000 brightsky-2.0.7/brightsky/parsers.py
--rw-r--r--   0 runner    (1001) docker     (123)     4400 2023-07-10 14:09:21.000000 brightsky-2.0.7/brightsky/polling.py
--rw-r--r--   0 runner    (1001) docker     (123)    16542 2023-07-10 14:09:21.000000 brightsky-2.0.7/brightsky/query.py
--rw-r--r--   0 runner    (1001) docker     (123)     2156 2023-07-10 14:09:21.000000 brightsky-2.0.7/brightsky/settings.py
--rw-r--r--   0 runner    (1001) docker     (123)     5001 2023-07-10 14:09:21.000000 brightsky-2.0.7/brightsky/tasks.py
--rw-r--r--   0 runner    (1001) docker     (123)     2504 2023-07-10 14:09:21.000000 brightsky-2.0.7/brightsky/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    13778 2023-07-10 14:09:21.000000 brightsky-2.0.7/brightsky/web.py
--rw-r--r--   0 runner    (1001) docker     (123)     2160 2023-07-10 14:09:21.000000 brightsky-2.0.7/brightsky/worker.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 14:09:30.259547 brightsky-2.0.7/brightsky.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8318 2023-07-10 14:09:30.000000 brightsky-2.0.7/brightsky.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      623 2023-07-10 14:09:30.000000 brightsky-2.0.7/brightsky.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-10 14:09:30.000000 brightsky-2.0.7/brightsky.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-07-10 14:09:30.000000 brightsky-2.0.7/brightsky.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-10 14:09:30.000000 brightsky-2.0.7/brightsky.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-07-10 14:09:21.000000 brightsky-2.0.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-10 14:09:30.263547 brightsky-2.0.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1250 2023-07-10 14:09:21.000000 brightsky-2.0.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 14:09:30.263547 brightsky-2.0.7/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-07-10 14:09:21.000000 brightsky-2.0.7/tests/test_db.py
--rw-r--r--   0 runner    (1001) docker     (123)     5341 2023-07-10 14:09:21.000000 brightsky-2.0.7/tests/test_export.py
--rw-r--r--   0 runner    (1001) docker     (123)     4680 2023-07-10 14:09:21.000000 brightsky-2.0.7/tests/test_parsers.py
--rw-r--r--   0 runner    (1001) docker     (123)     3430 2023-07-10 14:09:21.000000 brightsky-2.0.7/tests/test_polling.py
--rw-r--r--   0 runner    (1001) docker     (123)     1730 2023-07-10 14:09:21.000000 brightsky-2.0.7/tests/test_settings.py
--rw-r--r--   0 runner    (1001) docker     (123)     3130 2023-07-10 14:09:21.000000 brightsky-2.0.7/tests/test_tasks.py
--rw-r--r--   0 runner    (1001) docker     (123)     1344 2023-07-10 14:09:21.000000 brightsky-2.0.7/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    22552 2023-07-10 14:09:21.000000 brightsky-2.0.7/tests/test_web.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 15:20:44.731148 brightsky-2.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-08-08 15:20:37.000000 brightsky-2.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     8323 2023-08-08 15:20:44.731148 brightsky-2.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7713 2023-08-08 15:20:37.000000 brightsky-2.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 15:20:44.727148 brightsky-2.1.0/brightsky/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-08-08 15:20:37.000000 brightsky-2.1.0/brightsky/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      651 2023-08-08 15:20:37.000000 brightsky-2.1.0/brightsky/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4898 2023-08-08 15:20:37.000000 brightsky-2.1.0/brightsky/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2578 2023-08-08 15:20:37.000000 brightsky-2.1.0/brightsky/db.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13531 2023-08-08 15:20:37.000000 brightsky-2.1.0/brightsky/export.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7147 2023-08-08 15:20:37.000000 brightsky-2.1.0/brightsky/parsers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4400 2023-08-08 15:20:37.000000 brightsky-2.1.0/brightsky/polling.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16542 2023-08-08 15:20:37.000000 brightsky-2.1.0/brightsky/query.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2156 2023-08-08 15:20:37.000000 brightsky-2.1.0/brightsky/settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5001 2023-08-08 15:20:37.000000 brightsky-2.1.0/brightsky/tasks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2504 2023-08-08 15:20:37.000000 brightsky-2.1.0/brightsky/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13778 2023-08-08 15:20:37.000000 brightsky-2.1.0/brightsky/web.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2160 2023-08-08 15:20:37.000000 brightsky-2.1.0/brightsky/worker.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 15:20:44.731148 brightsky-2.1.0/brightsky.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8323 2023-08-08 15:20:44.000000 brightsky-2.1.0/brightsky.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      623 2023-08-08 15:20:44.000000 brightsky-2.1.0/brightsky.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 15:20:44.000000 brightsky-2.1.0/brightsky.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-08-08 15:20:44.000000 brightsky-2.1.0/brightsky.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-08-08 15:20:44.000000 brightsky-2.1.0/brightsky.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-08-08 15:20:37.000000 brightsky-2.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-08 15:20:44.731148 brightsky-2.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1255 2023-08-08 15:20:37.000000 brightsky-2.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 15:20:44.731148 brightsky-2.1.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-08-08 15:20:37.000000 brightsky-2.1.0/tests/test_db.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5341 2023-08-08 15:20:37.000000 brightsky-2.1.0/tests/test_export.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4680 2023-08-08 15:20:37.000000 brightsky-2.1.0/tests/test_parsers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3430 2023-08-08 15:20:37.000000 brightsky-2.1.0/tests/test_polling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1730 2023-08-08 15:20:37.000000 brightsky-2.1.0/tests/test_settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3130 2023-08-08 15:20:37.000000 brightsky-2.1.0/tests/test_tasks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1344 2023-08-08 15:20:37.000000 brightsky-2.1.0/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22552 2023-08-08 15:20:37.000000 brightsky-2.1.0/tests/test_web.py
```

### Comparing `brightsky-2.0.7/LICENSE` & `brightsky-2.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `brightsky-2.0.7/PKG-INFO` & `brightsky-2.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: brightsky
-Version: 2.0.7
+Version: 2.1.0
 Summary: JSON API for DWD's open weather data.
 Home-page: https://brightsky.dev/
 Author: Jakob de Maeyer
-Author-email: jakob@naboa.de
+Author-email: jakob@brightsky.dev
 Project-URL: Documentation, https://brightsky.dev/docs/
 Project-URL: Source, https://github.com/jdemaeyer/brightsky/
 Project-URL: Tracker, https://github.com/jdemaeyer/brightsky/issues/
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
```

### Comparing `brightsky-2.0.7/README.md` & `brightsky-2.1.0/README.md`

 * *Files identical despite different names*

### Comparing `brightsky-2.0.7/brightsky/__main__.py` & `brightsky-2.1.0/brightsky/__main__.py`

 * *Files identical despite different names*

### Comparing `brightsky-2.0.7/brightsky/cli.py` & `brightsky-2.1.0/brightsky/cli.py`

 * *Files identical despite different names*

### Comparing `brightsky-2.0.7/brightsky/db.py` & `brightsky-2.1.0/brightsky/db.py`

 * *Files identical despite different names*

### Comparing `brightsky-2.0.7/brightsky/export.py` & `brightsky-2.1.0/brightsky/export.py`

 * *Files identical despite different names*

### Comparing `brightsky-2.0.7/brightsky/parsers.py` & `brightsky-2.1.0/brightsky/parsers.py`

 * *Files identical despite different names*

### Comparing `brightsky-2.0.7/brightsky/polling.py` & `brightsky-2.1.0/brightsky/polling.py`

 * *Files identical despite different names*

### Comparing `brightsky-2.0.7/brightsky/query.py` & `brightsky-2.1.0/brightsky/query.py`

 * *Files identical despite different names*

### Comparing `brightsky-2.0.7/brightsky/settings.py` & `brightsky-2.1.0/brightsky/settings.py`

 * *Files identical despite different names*

### Comparing `brightsky-2.0.7/brightsky/tasks.py` & `brightsky-2.1.0/brightsky/tasks.py`

 * *Files identical despite different names*

### Comparing `brightsky-2.0.7/brightsky/utils.py` & `brightsky-2.1.0/brightsky/utils.py`

 * *Files identical despite different names*

### Comparing `brightsky-2.0.7/brightsky/web.py` & `brightsky-2.1.0/brightsky/web.py`

 * *Files identical despite different names*

### Comparing `brightsky-2.0.7/brightsky/worker.py` & `brightsky-2.1.0/brightsky/worker.py`

 * *Files identical despite different names*

### Comparing `brightsky-2.0.7/brightsky.egg-info/PKG-INFO` & `brightsky-2.1.0/brightsky.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: brightsky
-Version: 2.0.7
+Version: 2.1.0
 Summary: JSON API for DWD's open weather data.
 Home-page: https://brightsky.dev/
 Author: Jakob de Maeyer
-Author-email: jakob@naboa.de
+Author-email: jakob@brightsky.dev
 Project-URL: Documentation, https://brightsky.dev/docs/
 Project-URL: Source, https://github.com/jdemaeyer/brightsky/
 Project-URL: Tracker, https://github.com/jdemaeyer/brightsky/issues/
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
```

### Comparing `brightsky-2.0.7/brightsky.egg-info/SOURCES.txt` & `brightsky-2.1.0/brightsky.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `brightsky-2.0.7/setup.py` & `brightsky-2.1.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 with open('README.md') as f:
     long_description = f.read()
 
 setup(
     name='brightsky',
     version=brightsky.__version__,
     author='Jakob de Maeyer',
-    author_email='jakob@naboa.de',
+    author_email='jakob@brightsky.dev',
     description="JSON API for DWD's open weather data.",
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://brightsky.dev/',
     project_urls={
         'Documentation': 'https://brightsky.dev/docs/',
         'Source': 'https://github.com/jdemaeyer/brightsky/',
```

### Comparing `brightsky-2.0.7/tests/test_export.py` & `brightsky-2.1.0/tests/test_export.py`

 * *Files identical despite different names*

### Comparing `brightsky-2.0.7/tests/test_parsers.py` & `brightsky-2.1.0/tests/test_parsers.py`

 * *Files identical despite different names*

### Comparing `brightsky-2.0.7/tests/test_polling.py` & `brightsky-2.1.0/tests/test_polling.py`

 * *Files identical despite different names*

### Comparing `brightsky-2.0.7/tests/test_settings.py` & `brightsky-2.1.0/tests/test_settings.py`

 * *Files identical despite different names*

### Comparing `brightsky-2.0.7/tests/test_tasks.py` & `brightsky-2.1.0/tests/test_tasks.py`

 * *Files identical despite different names*

### Comparing `brightsky-2.0.7/tests/test_utils.py` & `brightsky-2.1.0/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `brightsky-2.0.7/tests/test_web.py` & `brightsky-2.1.0/tests/test_web.py`

 * *Files identical despite different names*


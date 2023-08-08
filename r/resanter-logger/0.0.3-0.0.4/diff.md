# Comparing `tmp/resanter_logger-0.0.3.tar.gz` & `tmp/resanter_logger-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "resanter_logger-0.0.3.tar", last modified: Tue Aug  8 15:16:24 2023, max compression
+gzip compressed data, was "resanter_logger-0.0.4.tar", last modified: Tue Aug  8 15:19:35 2023, max compression
```

## Comparing `resanter_logger-0.0.3.tar` & `resanter_logger-0.0.4.tar`

### file list

```diff
@@ -1,14 +1,15 @@
-drwxrwxr-x   0 santer    (1000) santer    (1000)        0 2023-08-08 15:16:24.326269 resanter_logger-0.0.3/
--rw-rw-r--   0 santer    (1000) santer    (1000)     1068 2023-08-06 20:22:46.000000 resanter_logger-0.0.3/LICENSE
--rw-rw-r--   0 santer    (1000) santer    (1000)      559 2023-08-08 15:16:24.326269 resanter_logger-0.0.3/PKG-INFO
--rw-rw-r--   0 santer    (1000) santer    (1000)       64 2023-08-06 20:04:00.000000 resanter_logger-0.0.3/README.md
--rw-rw-r--   0 santer    (1000) santer    (1000)      568 2023-08-08 15:16:20.000000 resanter_logger-0.0.3/pyproject.toml
--rw-rw-r--   0 santer    (1000) santer    (1000)       38 2023-08-08 15:16:24.326269 resanter_logger-0.0.3/setup.cfg
-drwxrwxr-x   0 santer    (1000) santer    (1000)        0 2023-08-08 15:16:24.326269 resanter_logger-0.0.3/src/
-drwxrwxr-x   0 santer    (1000) santer    (1000)        0 2023-08-08 15:16:24.326269 resanter_logger-0.0.3/src/resanter_logger/
--rw-rw-r--   0 santer    (1000) santer    (1000)     1276 2023-08-07 20:14:28.000000 resanter_logger-0.0.3/src/resanter_logger/re_logger.py
-drwxrwxr-x   0 santer    (1000) santer    (1000)        0 2023-08-08 15:16:24.326269 resanter_logger-0.0.3/src/resanter_logger.egg-info/
--rw-rw-r--   0 santer    (1000) santer    (1000)      559 2023-08-08 15:16:24.000000 resanter_logger-0.0.3/src/resanter_logger.egg-info/PKG-INFO
--rw-rw-r--   0 santer    (1000) santer    (1000)      237 2023-08-08 15:16:24.000000 resanter_logger-0.0.3/src/resanter_logger.egg-info/SOURCES.txt
--rw-rw-r--   0 santer    (1000) santer    (1000)        1 2023-08-08 15:16:24.000000 resanter_logger-0.0.3/src/resanter_logger.egg-info/dependency_links.txt
--rw-rw-r--   0 santer    (1000) santer    (1000)       16 2023-08-08 15:16:24.000000 resanter_logger-0.0.3/src/resanter_logger.egg-info/top_level.txt
+drwxrwxr-x   0 santer    (1000) santer    (1000)        0 2023-08-08 15:19:35.363968 resanter_logger-0.0.4/
+-rw-rw-r--   0 santer    (1000) santer    (1000)     1068 2023-08-06 20:22:46.000000 resanter_logger-0.0.4/LICENSE
+-rw-rw-r--   0 santer    (1000) santer    (1000)      559 2023-08-08 15:19:35.363968 resanter_logger-0.0.4/PKG-INFO
+-rw-rw-r--   0 santer    (1000) santer    (1000)       64 2023-08-06 20:04:00.000000 resanter_logger-0.0.4/README.md
+-rw-rw-r--   0 santer    (1000) santer    (1000)      568 2023-08-08 15:19:31.000000 resanter_logger-0.0.4/pyproject.toml
+-rw-rw-r--   0 santer    (1000) santer    (1000)       38 2023-08-08 15:19:35.363968 resanter_logger-0.0.4/setup.cfg
+drwxrwxr-x   0 santer    (1000) santer    (1000)        0 2023-08-08 15:19:35.363968 resanter_logger-0.0.4/src/
+drwxrwxr-x   0 santer    (1000) santer    (1000)        0 2023-08-08 15:19:35.363968 resanter_logger-0.0.4/src/resanter_logger/
+-rw-rw-r--   0 santer    (1000) santer    (1000)       31 2023-08-08 15:19:21.000000 resanter_logger-0.0.4/src/resanter_logger/__init__.py
+-rw-rw-r--   0 santer    (1000) santer    (1000)     1276 2023-08-07 20:14:28.000000 resanter_logger-0.0.4/src/resanter_logger/re_logger.py
+drwxrwxr-x   0 santer    (1000) santer    (1000)        0 2023-08-08 15:19:35.363968 resanter_logger-0.0.4/src/resanter_logger.egg-info/
+-rw-rw-r--   0 santer    (1000) santer    (1000)      559 2023-08-08 15:19:35.000000 resanter_logger-0.0.4/src/resanter_logger.egg-info/PKG-INFO
+-rw-rw-r--   0 santer    (1000) santer    (1000)      269 2023-08-08 15:19:35.000000 resanter_logger-0.0.4/src/resanter_logger.egg-info/SOURCES.txt
+-rw-rw-r--   0 santer    (1000) santer    (1000)        1 2023-08-08 15:19:35.000000 resanter_logger-0.0.4/src/resanter_logger.egg-info/dependency_links.txt
+-rw-rw-r--   0 santer    (1000) santer    (1000)       16 2023-08-08 15:19:35.000000 resanter_logger-0.0.4/src/resanter_logger.egg-info/top_level.txt
```

### Comparing `resanter_logger-0.0.3/LICENSE` & `resanter_logger-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `resanter_logger-0.0.3/PKG-INFO` & `resanter_logger-0.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: resanter_logger
-Version: 0.0.3
+Version: 0.0.4
 Summary: Simple logger
 Author-email: resanter <reoskaro434@gmail.com>
 Project-URL: Homepage, https://github.com/reoskaro434/logger
 Project-URL: Bug Tracker, https://github.com/reoskaro434/logger/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `resanter_logger-0.0.3/pyproject.toml` & `resanter_logger-0.0.4/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "resanter_logger"
-version = "0.0.3"
+version = "0.0.4"
 authors = [
   { name="resanter", email="reoskaro434@gmail.com" },
 ]
 description = "Simple logger"
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
```

### Comparing `resanter_logger-0.0.3/src/resanter_logger/re_logger.py` & `resanter_logger-0.0.4/src/resanter_logger/re_logger.py`

 * *Files identical despite different names*

### Comparing `resanter_logger-0.0.3/src/resanter_logger.egg-info/PKG-INFO` & `resanter_logger-0.0.4/src/resanter_logger.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: resanter-logger
-Version: 0.0.3
+Version: 0.0.4
 Summary: Simple logger
 Author-email: resanter <reoskaro434@gmail.com>
 Project-URL: Homepage, https://github.com/reoskaro434/logger
 Project-URL: Bug Tracker, https://github.com/reoskaro434/logger/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```


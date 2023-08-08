# Comparing `tmp/resanter_logger-0.0.2.tar.gz` & `tmp/resanter_logger-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "resanter_logger-0.0.2.tar", last modified: Mon Aug  7 20:19:27 2023, max compression
+gzip compressed data, was "resanter_logger-0.0.3.tar", last modified: Tue Aug  8 15:16:24 2023, max compression
```

## Comparing `resanter_logger-0.0.2.tar` & `resanter_logger-0.0.3.tar`

### file list

```diff
@@ -1,16 +1,14 @@
-drwxrwxr-x   0 santer    (1000) santer    (1000)        0 2023-08-07 20:19:27.309808 resanter_logger-0.0.2/
--rw-rw-r--   0 santer    (1000) santer    (1000)     1068 2023-08-06 20:22:46.000000 resanter_logger-0.0.2/LICENSE
--rw-rw-r--   0 santer    (1000) santer    (1000)      559 2023-08-07 20:19:27.309808 resanter_logger-0.0.2/PKG-INFO
--rw-rw-r--   0 santer    (1000) santer    (1000)       64 2023-08-06 20:04:00.000000 resanter_logger-0.0.2/README.md
--rw-rw-r--   0 santer    (1000) santer    (1000)      568 2023-08-07 20:18:55.000000 resanter_logger-0.0.2/pyproject.toml
--rw-rw-r--   0 santer    (1000) santer    (1000)       38 2023-08-07 20:19:27.309808 resanter_logger-0.0.2/setup.cfg
-drwxrwxr-x   0 santer    (1000) santer    (1000)        0 2023-08-07 20:19:27.309808 resanter_logger-0.0.2/src/
--rw-rw-r--   0 santer    (1000) santer    (1000)        0 2023-08-06 20:02:12.000000 resanter_logger-0.0.2/src/__init__.py
-drwxrwxr-x   0 santer    (1000) santer    (1000)        0 2023-08-07 20:19:27.309808 resanter_logger-0.0.2/src/resanter_logger/
--rw-rw-r--   0 santer    (1000) santer    (1000)        0 2023-08-07 19:47:52.000000 resanter_logger-0.0.2/src/resanter_logger/__init__.py
--rw-rw-r--   0 santer    (1000) santer    (1000)     1276 2023-08-07 20:14:28.000000 resanter_logger-0.0.2/src/resanter_logger/re_logger.py
-drwxrwxr-x   0 santer    (1000) santer    (1000)        0 2023-08-07 20:19:27.309808 resanter_logger-0.0.2/src/resanter_logger.egg-info/
--rw-rw-r--   0 santer    (1000) santer    (1000)      559 2023-08-07 20:19:27.000000 resanter_logger-0.0.2/src/resanter_logger.egg-info/PKG-INFO
--rw-rw-r--   0 santer    (1000) santer    (1000)      285 2023-08-07 20:19:27.000000 resanter_logger-0.0.2/src/resanter_logger.egg-info/SOURCES.txt
--rw-rw-r--   0 santer    (1000) santer    (1000)        1 2023-08-07 20:19:27.000000 resanter_logger-0.0.2/src/resanter_logger.egg-info/dependency_links.txt
--rw-rw-r--   0 santer    (1000) santer    (1000)       25 2023-08-07 20:19:27.000000 resanter_logger-0.0.2/src/resanter_logger.egg-info/top_level.txt
+drwxrwxr-x   0 santer    (1000) santer    (1000)        0 2023-08-08 15:16:24.326269 resanter_logger-0.0.3/
+-rw-rw-r--   0 santer    (1000) santer    (1000)     1068 2023-08-06 20:22:46.000000 resanter_logger-0.0.3/LICENSE
+-rw-rw-r--   0 santer    (1000) santer    (1000)      559 2023-08-08 15:16:24.326269 resanter_logger-0.0.3/PKG-INFO
+-rw-rw-r--   0 santer    (1000) santer    (1000)       64 2023-08-06 20:04:00.000000 resanter_logger-0.0.3/README.md
+-rw-rw-r--   0 santer    (1000) santer    (1000)      568 2023-08-08 15:16:20.000000 resanter_logger-0.0.3/pyproject.toml
+-rw-rw-r--   0 santer    (1000) santer    (1000)       38 2023-08-08 15:16:24.326269 resanter_logger-0.0.3/setup.cfg
+drwxrwxr-x   0 santer    (1000) santer    (1000)        0 2023-08-08 15:16:24.326269 resanter_logger-0.0.3/src/
+drwxrwxr-x   0 santer    (1000) santer    (1000)        0 2023-08-08 15:16:24.326269 resanter_logger-0.0.3/src/resanter_logger/
+-rw-rw-r--   0 santer    (1000) santer    (1000)     1276 2023-08-07 20:14:28.000000 resanter_logger-0.0.3/src/resanter_logger/re_logger.py
+drwxrwxr-x   0 santer    (1000) santer    (1000)        0 2023-08-08 15:16:24.326269 resanter_logger-0.0.3/src/resanter_logger.egg-info/
+-rw-rw-r--   0 santer    (1000) santer    (1000)      559 2023-08-08 15:16:24.000000 resanter_logger-0.0.3/src/resanter_logger.egg-info/PKG-INFO
+-rw-rw-r--   0 santer    (1000) santer    (1000)      237 2023-08-08 15:16:24.000000 resanter_logger-0.0.3/src/resanter_logger.egg-info/SOURCES.txt
+-rw-rw-r--   0 santer    (1000) santer    (1000)        1 2023-08-08 15:16:24.000000 resanter_logger-0.0.3/src/resanter_logger.egg-info/dependency_links.txt
+-rw-rw-r--   0 santer    (1000) santer    (1000)       16 2023-08-08 15:16:24.000000 resanter_logger-0.0.3/src/resanter_logger.egg-info/top_level.txt
```

### Comparing `resanter_logger-0.0.2/LICENSE` & `resanter_logger-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `resanter_logger-0.0.2/PKG-INFO` & `resanter_logger-0.0.3/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: resanter_logger
-Version: 0.0.2
+Version: 0.0.3
 Summary: Simple logger
 Author-email: resanter <reoskaro434@gmail.com>
 Project-URL: Homepage, https://github.com/reoskaro434/logger
 Project-URL: Bug Tracker, https://github.com/reoskaro434/logger/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `resanter_logger-0.0.2/pyproject.toml` & `resanter_logger-0.0.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "resanter_logger"
-version = "0.0.2"
+version = "0.0.3"
 authors = [
   { name="resanter", email="reoskaro434@gmail.com" },
 ]
 description = "Simple logger"
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
```

### Comparing `resanter_logger-0.0.2/src/resanter_logger/re_logger.py` & `resanter_logger-0.0.3/src/resanter_logger/re_logger.py`

 * *Files identical despite different names*

### Comparing `resanter_logger-0.0.2/src/resanter_logger.egg-info/PKG-INFO` & `resanter_logger-0.0.3/src/resanter_logger.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: resanter-logger
-Version: 0.0.2
+Version: 0.0.3
 Summary: Simple logger
 Author-email: resanter <reoskaro434@gmail.com>
 Project-URL: Homepage, https://github.com/reoskaro434/logger
 Project-URL: Bug Tracker, https://github.com/reoskaro434/logger/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```


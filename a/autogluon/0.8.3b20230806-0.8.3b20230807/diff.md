# Comparing `tmp/autogluon-0.8.3b20230806.tar.gz` & `tmp/autogluon-0.8.3b20230807.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autogluon-0.8.3b20230806.tar", last modified: Sun Aug  6 09:04:18 2023, max compression
+gzip compressed data, was "autogluon-0.8.3b20230807.tar", last modified: Mon Aug  7 09:04:42 2023, max compression
```

## Comparing `autogluon-0.8.3b20230806.tar` & `autogluon-0.8.3b20230807.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 09:04:18.253781 autogluon-0.8.3b20230806/
--rw-r--r--   0 runner    (1001) docker     (123)    12860 2023-08-06 09:04:18.253781 autogluon-0.8.3b20230806/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-06 09:04:18.253781 autogluon-0.8.3b20230806/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1537 2023-08-06 09:03:33.000000 autogluon-0.8.3b20230806/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 09:04:18.253781 autogluon-0.8.3b20230806/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 09:04:18.253781 autogluon-0.8.3b20230806/src/autogluon/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 09:04:18.253781 autogluon-0.8.3b20230806/src/autogluon/_internal_/
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-06 09:03:33.000000 autogluon-0.8.3b20230806/src/autogluon/_internal_/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 09:04:18.253781 autogluon-0.8.3b20230806/src/autogluon.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    12860 2023-08-06 09:04:18.000000 autogluon-0.8.3b20230806/src/autogluon.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      307 2023-08-06 09:04:18.000000 autogluon-0.8.3b20230806/src/autogluon.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-06 09:04:18.000000 autogluon-0.8.3b20230806/src/autogluon.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-08-06 09:04:18.000000 autogluon-0.8.3b20230806/src/autogluon.egg-info/namespace_packages.txt
--rw-r--r--   0 runner    (1001) docker     (123)      189 2023-08-06 09:04:18.000000 autogluon-0.8.3b20230806/src/autogluon.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-08-06 09:04:18.000000 autogluon-0.8.3b20230806/src/autogluon.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-06 09:04:18.000000 autogluon-0.8.3b20230806/src/autogluon.egg-info/zip-safe
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 09:04:42.010697 autogluon-0.8.3b20230807/
+-rw-r--r--   0 runner    (1001) docker     (123)    12860 2023-08-07 09:04:42.010697 autogluon-0.8.3b20230807/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-07 09:04:42.010697 autogluon-0.8.3b20230807/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1537 2023-08-07 09:04:04.000000 autogluon-0.8.3b20230807/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 09:04:42.006696 autogluon-0.8.3b20230807/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 09:04:42.006696 autogluon-0.8.3b20230807/src/autogluon/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 09:04:42.010697 autogluon-0.8.3b20230807/src/autogluon/_internal_/
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-07 09:04:04.000000 autogluon-0.8.3b20230807/src/autogluon/_internal_/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 09:04:42.010697 autogluon-0.8.3b20230807/src/autogluon.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    12860 2023-08-07 09:04:41.000000 autogluon-0.8.3b20230807/src/autogluon.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      307 2023-08-07 09:04:41.000000 autogluon-0.8.3b20230807/src/autogluon.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-07 09:04:41.000000 autogluon-0.8.3b20230807/src/autogluon.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-08-07 09:04:41.000000 autogluon-0.8.3b20230807/src/autogluon.egg-info/namespace_packages.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      189 2023-08-07 09:04:41.000000 autogluon-0.8.3b20230807/src/autogluon.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-08-07 09:04:41.000000 autogluon-0.8.3b20230807/src/autogluon.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-07 09:04:41.000000 autogluon-0.8.3b20230807/src/autogluon.egg-info/zip-safe
```

### Comparing `autogluon-0.8.3b20230806/PKG-INFO` & `autogluon-0.8.3b20230807/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autogluon
-Version: 0.8.3b20230806
+Version: 0.8.3b20230807
 Summary: AutoML for Image, Text, and Tabular Data
 Home-page: https://github.com/autogluon/autogluon
 Author: AutoGluon Community
 License: Apache-2.0
 Project-URL: Documentation, https://auto.gluon.ai
 Project-URL: Bug Reports, https://github.com/autogluon/autogluon/issues
 Project-URL: Source, https://github.com/autogluon/autogluon/
```

### Comparing `autogluon-0.8.3b20230806/setup.py` & `autogluon-0.8.3b20230807/setup.py`

 * *Files identical despite different names*

### Comparing `autogluon-0.8.3b20230806/src/autogluon.egg-info/PKG-INFO` & `autogluon-0.8.3b20230807/src/autogluon.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autogluon
-Version: 0.8.3b20230806
+Version: 0.8.3b20230807
 Summary: AutoML for Image, Text, and Tabular Data
 Home-page: https://github.com/autogluon/autogluon
 Author: AutoGluon Community
 License: Apache-2.0
 Project-URL: Documentation, https://auto.gluon.ai
 Project-URL: Bug Reports, https://github.com/autogluon/autogluon/issues
 Project-URL: Source, https://github.com/autogluon/autogluon/
```


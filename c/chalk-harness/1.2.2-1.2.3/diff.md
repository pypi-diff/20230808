# Comparing `tmp/chalk-harness-1.2.2.tar.gz` & `tmp/chalk-harness-1.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chalk-harness-1.2.2.tar", last modified: Mon Aug  7 02:30:22 2023, max compression
+gzip compressed data, was "chalk-harness-1.2.3.tar", last modified: Mon Aug  7 22:43:24 2023, max compression
```

## Comparing `chalk-harness-1.2.2.tar` & `chalk-harness-1.2.3.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 02:30:22.278518 chalk-harness-1.2.2/
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-08-07 02:30:07.000000 chalk-harness-1.2.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      967 2023-08-07 02:30:22.278518 chalk-harness-1.2.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      612 2023-08-07 02:30:07.000000 chalk-harness-1.2.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 02:30:07.000000 chalk-harness-1.2.2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-08-07 02:30:07.000000 chalk-harness-1.2.2/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 02:30:22.278518 chalk-harness-1.2.2/chalk_harness.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      967 2023-08-07 02:30:22.000000 chalk-harness-1.2.2/chalk_harness.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      343 2023-08-07 02:30:22.000000 chalk-harness-1.2.2/chalk_harness.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-07 02:30:22.000000 chalk-harness-1.2.2/chalk_harness.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-08-07 02:30:22.000000 chalk-harness-1.2.2/chalk_harness.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-08-07 02:30:22.000000 chalk-harness-1.2.2/chalk_harness.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 02:30:22.278518 chalk-harness-1.2.2/chalkharness/
--rw-r--r--   0 runner    (1001) docker     (123)     6548 2023-08-07 02:30:07.000000 chalk-harness-1.2.2/chalkharness/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 02:30:07.000000 chalk-harness-1.2.2/chalkharness/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-08-07 02:30:07.000000 chalk-harness-1.2.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-07 02:30:22.278518 chalk-harness-1.2.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1479 2023-08-07 02:30:07.000000 chalk-harness-1.2.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 02:30:22.278518 chalk-harness-1.2.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1019 2023-08-07 02:30:07.000000 chalk-harness-1.2.2/tests/SanityTestCase.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 02:30:07.000000 chalk-harness-1.2.2/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 22:43:24.063546 chalk-harness-1.2.3/
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-08-07 22:43:02.000000 chalk-harness-1.2.3/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      967 2023-08-07 22:43:24.063546 chalk-harness-1.2.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      612 2023-08-07 22:43:02.000000 chalk-harness-1.2.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 22:43:02.000000 chalk-harness-1.2.3/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-08-07 22:43:02.000000 chalk-harness-1.2.3/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 22:43:24.063546 chalk-harness-1.2.3/chalk_harness.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      967 2023-08-07 22:43:23.000000 chalk-harness-1.2.3/chalk_harness.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      343 2023-08-07 22:43:24.000000 chalk-harness-1.2.3/chalk_harness.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-07 22:43:23.000000 chalk-harness-1.2.3/chalk_harness.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-08-07 22:43:23.000000 chalk-harness-1.2.3/chalk_harness.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-08-07 22:43:23.000000 chalk-harness-1.2.3/chalk_harness.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 22:43:24.063546 chalk-harness-1.2.3/chalkharness/
+-rw-r--r--   0 runner    (1001) docker     (123)     6548 2023-08-07 22:43:02.000000 chalk-harness-1.2.3/chalkharness/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 22:43:02.000000 chalk-harness-1.2.3/chalkharness/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-08-07 22:43:02.000000 chalk-harness-1.2.3/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-07 22:43:24.063546 chalk-harness-1.2.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1479 2023-08-07 22:43:02.000000 chalk-harness-1.2.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 22:43:24.063546 chalk-harness-1.2.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1019 2023-08-07 22:43:02.000000 chalk-harness-1.2.3/tests/SanityTestCase.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 22:43:02.000000 chalk-harness-1.2.3/tests/__init__.py
```

### Comparing `chalk-harness-1.2.2/PKG-INFO` & `chalk-harness-1.2.3/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chalk-harness
-Version: 1.2.2
+Version: 1.2.3
 Summary: Python wrapper for Chalk's CLI
 Home-page: https://chalk.ai
 Author: Chalk AI, Inc.
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Requires-Python: >=3.8.0
```

### Comparing `chalk-harness-1.2.2/README.md` & `chalk-harness-1.2.3/README.md`

 * *Files identical despite different names*

### Comparing `chalk-harness-1.2.2/chalk_harness.egg-info/PKG-INFO` & `chalk-harness-1.2.3/chalk_harness.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chalk-harness
-Version: 1.2.2
+Version: 1.2.3
 Summary: Python wrapper for Chalk's CLI
 Home-page: https://chalk.ai
 Author: Chalk AI, Inc.
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Requires-Python: >=3.8.0
```

### Comparing `chalk-harness-1.2.2/chalkharness/__init__.py` & `chalk-harness-1.2.3/chalkharness/__init__.py`

 * *Files identical despite different names*

### Comparing `chalk-harness-1.2.2/setup.py` & `chalk-harness-1.2.3/setup.py`

 * *Files identical despite different names*

### Comparing `chalk-harness-1.2.2/tests/SanityTestCase.py` & `chalk-harness-1.2.3/tests/SanityTestCase.py`

 * *Files identical despite different names*


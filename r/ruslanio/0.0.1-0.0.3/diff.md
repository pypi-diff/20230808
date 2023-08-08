# Comparing `tmp/ruslanio-0.0.1.tar.gz` & `tmp/ruslanio-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ruslanio-0.0.1.tar", last modified: Tue Aug  8 21:04:17 2023, max compression
+gzip compressed data, was "ruslanio-0.0.3.tar", last modified: Tue Aug  8 21:30:59 2023, max compression
```

## Comparing `ruslanio-0.0.1.tar` & `ruslanio-0.0.3.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 ruslan    (1000) ruslan    (1001)        0 2023-08-08 21:04:17.617281 ruslanio-0.0.1/
--rw-r--r--   0 ruslan    (1000) ruslan    (1001)     1073 2023-08-08 20:54:20.000000 ruslanio-0.0.1/LICENSE
--rw-r--r--   0 ruslan    (1000) ruslan    (1001)       24 2023-08-08 21:04:06.000000 ruslanio-0.0.1/MANIFEST.in
--rw-r--r--   0 ruslan    (1000) ruslan    (1001)      679 2023-08-08 21:04:17.617281 ruslanio-0.0.1/PKG-INFO
--rw-r--r--   0 ruslan    (1000) ruslan    (1001)      422 2023-08-08 20:42:36.000000 ruslanio-0.0.1/README.md
--rw-r--r--   0 ruslan    (1000) ruslan    (1001)       24 2023-08-08 20:29:18.000000 ruslanio-0.0.1/requirements.txt
-drwxr-xr-x   0 ruslan    (1000) ruslan    (1001)        0 2023-08-08 21:04:17.617281 ruslanio-0.0.1/ruslanio/
--rw-r--r--   0 ruslan    (1000) ruslan    (1001)       80 2023-08-08 20:39:03.000000 ruslanio-0.0.1/ruslanio/__init__.py
--rw-r--r--   0 ruslan    (1000) ruslan    (1001)     2669 2023-08-08 20:21:29.000000 ruslanio-0.0.1/ruslanio/beam_search.py
--rw-r--r--   0 ruslan    (1000) ruslan    (1001)     5579 2023-08-08 19:59:32.000000 ruslanio-0.0.1/ruslanio/cacher.py
--rw-r--r--   0 ruslan    (1000) ruslan    (1001)      222 2023-08-08 19:50:08.000000 ruslanio-0.0.1/ruslanio/image.py
-drwxr-xr-x   0 ruslan    (1000) ruslan    (1001)        0 2023-08-08 21:04:17.617281 ruslanio-0.0.1/ruslanio.egg-info/
--rw-r--r--   0 ruslan    (1000) ruslan    (1001)      679 2023-08-08 21:04:17.000000 ruslanio-0.0.1/ruslanio.egg-info/PKG-INFO
--rw-r--r--   0 ruslan    (1000) ruslan    (1001)      296 2023-08-08 21:04:17.000000 ruslanio-0.0.1/ruslanio.egg-info/SOURCES.txt
--rw-r--r--   0 ruslan    (1000) ruslan    (1001)        1 2023-08-08 21:04:17.000000 ruslanio-0.0.1/ruslanio.egg-info/dependency_links.txt
--rw-r--r--   0 ruslan    (1000) ruslan    (1001)       25 2023-08-08 21:04:17.000000 ruslanio-0.0.1/ruslanio.egg-info/requires.txt
--rw-r--r--   0 ruslan    (1000) ruslan    (1001)        9 2023-08-08 21:04:17.000000 ruslanio-0.0.1/ruslanio.egg-info/top_level.txt
--rw-r--r--   0 ruslan    (1000) ruslan    (1001)       38 2023-08-08 21:04:17.617281 ruslanio-0.0.1/setup.cfg
--rw-r--r--   0 ruslan    (1000) ruslan    (1001)     1417 2023-08-08 21:04:11.000000 ruslanio-0.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 21:30:59.700692 ruslanio-0.0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-08-08 21:30:48.000000 ruslanio-0.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-08-08 21:30:48.000000 ruslanio-0.0.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      654 2023-08-08 21:30:59.700692 ruslanio-0.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      397 2023-08-08 21:30:48.000000 ruslanio-0.0.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-08-08 21:30:48.000000 ruslanio-0.0.3/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 21:30:59.700692 ruslanio-0.0.3/ruslanio/
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-08-08 21:30:48.000000 ruslanio-0.0.3/ruslanio/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2669 2023-08-08 21:30:48.000000 ruslanio-0.0.3/ruslanio/beam_search.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5579 2023-08-08 21:30:48.000000 ruslanio-0.0.3/ruslanio/cacher.py
+-rw-r--r--   0 runner    (1001) docker     (123)      222 2023-08-08 21:30:48.000000 ruslanio-0.0.3/ruslanio/image.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 21:30:59.700692 ruslanio-0.0.3/ruslanio.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      654 2023-08-08 21:30:59.000000 ruslanio-0.0.3/ruslanio.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      296 2023-08-08 21:30:59.000000 ruslanio-0.0.3/ruslanio.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 21:30:59.000000 ruslanio-0.0.3/ruslanio.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-08-08 21:30:59.000000 ruslanio-0.0.3/ruslanio.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-08-08 21:30:59.000000 ruslanio-0.0.3/ruslanio.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-08 21:30:59.700692 ruslanio-0.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1417 2023-08-08 21:30:48.000000 ruslanio-0.0.3/setup.py
```

### Comparing `ruslanio-0.0.1/LICENSE` & `ruslanio-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `ruslanio-0.0.1/ruslanio/beam_search.py` & `ruslanio-0.0.3/ruslanio/beam_search.py`

 * *Files identical despite different names*

### Comparing `ruslanio-0.0.1/ruslanio/cacher.py` & `ruslanio-0.0.3/ruslanio/cacher.py`

 * *Files identical despite different names*

### Comparing `ruslanio-0.0.1/setup.py` & `ruslanio-0.0.3/setup.py`

 * *Files identical despite different names*


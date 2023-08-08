# Comparing `tmp/TensorFlow1-2.3.8.tar.gz` & `tmp/TensorFlow1-2.4.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "TensorFlow1-2.3.8.tar", last modified: Tue Aug  8 14:25:41 2023, max compression
+gzip compressed data, was "TensorFlow1-2.4.8.tar", last modified: Tue Aug  8 14:29:52 2023, max compression
```

## Comparing `TensorFlow1-2.3.8.tar` & `TensorFlow1-2.4.8.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-08-08 14:25:41.841468 TensorFlow1-2.3.8/
--rw-rw-rw-   0        0        0      193 2023-08-08 14:25:41.841468 TensorFlow1-2.3.8/PKG-INFO
--rw-rw-rw-   0        0        0        0 2023-07-25 12:12:58.000000 TensorFlow1-2.3.8/README.md
-drwxrwxrwx   0        0        0        0 2023-08-08 14:25:41.800370 TensorFlow1-2.3.8/TensorFlow1/
--rw-rw-rw-   0        0        0    18355 2023-08-08 14:24:51.000000 TensorFlow1-2.3.8/TensorFlow1/TensorFlow.py
--rw-rw-rw-   0        0        0       40 2023-07-25 14:53:10.000000 TensorFlow1-2.3.8/TensorFlow1/__init__.py
-drwxrwxrwx   0        0        0        0 2023-08-08 14:25:41.840471 TensorFlow1-2.3.8/TensorFlow1.egg-info/
--rw-rw-rw-   0        0        0      193 2023-08-08 14:25:41.000000 TensorFlow1-2.3.8/TensorFlow1.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      230 2023-08-08 14:25:41.000000 TensorFlow1-2.3.8/TensorFlow1.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-08 14:25:41.000000 TensorFlow1-2.3.8/TensorFlow1.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       12 2023-08-08 14:25:41.000000 TensorFlow1-2.3.8/TensorFlow1.egg-info/top_level.txt
--rw-rw-rw-   0        0        0        0 2023-07-25 12:13:11.000000 TensorFlow1-2.3.8/license.txt
--rw-rw-rw-   0        0        0      158 2023-08-08 14:25:41.844463 TensorFlow1-2.3.8/setup.cfg
--rw-rw-rw-   0        0        0      304 2023-08-08 14:25:15.000000 TensorFlow1-2.3.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-08 14:29:52.600750 TensorFlow1-2.4.8/
+-rw-rw-rw-   0        0        0      193 2023-08-08 14:29:52.600750 TensorFlow1-2.4.8/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2023-07-25 12:12:58.000000 TensorFlow1-2.4.8/README.md
+drwxrwxrwx   0        0        0        0 2023-08-08 14:29:52.585404 TensorFlow1-2.4.8/TensorFlow1/
+-rw-rw-rw-   0        0        0    18355 2023-08-08 14:24:51.000000 TensorFlow1-2.4.8/TensorFlow1/TensorFlow.py
+-rw-rw-rw-   0        0        0       42 2023-08-08 14:28:06.000000 TensorFlow1-2.4.8/TensorFlow1/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-08 14:29:52.598755 TensorFlow1-2.4.8/TensorFlow1.egg-info/
+-rw-rw-rw-   0        0        0      193 2023-08-08 14:29:52.000000 TensorFlow1-2.4.8/TensorFlow1.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      230 2023-08-08 14:29:52.000000 TensorFlow1-2.4.8/TensorFlow1.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-08 14:29:52.000000 TensorFlow1-2.4.8/TensorFlow1.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       12 2023-08-08 14:29:52.000000 TensorFlow1-2.4.8/TensorFlow1.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0        0 2023-07-25 12:13:11.000000 TensorFlow1-2.4.8/license.txt
+-rw-rw-rw-   0        0        0      158 2023-08-08 14:29:52.603090 TensorFlow1-2.4.8/setup.cfg
+-rw-rw-rw-   0        0        0      304 2023-08-08 14:28:59.000000 TensorFlow1-2.4.8/setup.py
```

### Comparing `TensorFlow1-2.3.8/TensorFlow1/TensorFlow.py` & `TensorFlow1-2.4.8/TensorFlow1/TensorFlow.py`

 * *Files identical despite different names*


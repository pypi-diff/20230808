# Comparing `tmp/zlgsendcan-1.2.1.tar.gz` & `tmp/zlgsendcan-1.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zlgsendcan-1.2.1.tar", last modified: Fri Jul 28 03:12:49 2023, max compression
+gzip compressed data, was "zlgsendcan-1.2.2.tar", last modified: Tue Aug  8 03:14:19 2023, max compression
```

## Comparing `zlgsendcan-1.2.1.tar` & `zlgsendcan-1.2.2.tar`

### file list

```diff
@@ -1,19 +1,20 @@
-drwxrwxrwx   0        0        0        0 2023-07-28 03:12:49.332455 zlgsendcan-1.2.1/
--rw-rw-rw-   0        0        0      221 2023-07-28 03:12:49.331460 zlgsendcan-1.2.1/PKG-INFO
--rw-rw-rw-   0        0        0       42 2023-07-28 03:12:49.332455 zlgsendcan-1.2.1/setup.cfg
--rw-rw-rw-   0        0        0      438 2023-07-28 03:12:39.000000 zlgsendcan-1.2.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-28 03:12:49.321457 zlgsendcan-1.2.1/zlgsendcan/
--rw-rw-rw-   0        0        0        0 2023-07-26 06:34:10.000000 zlgsendcan-1.2.1/zlgsendcan/__init__.py
--rw-rw-rw-   0        0        0     2076 2023-07-27 04:16:37.000000 zlgsendcan-1.2.1/zlgsendcan/example_test.py
--rw-rw-rw-   0        0        0      237 2023-02-14 03:41:12.000000 zlgsendcan-1.2.1/zlgsendcan/frozen_dir.py
--rw-rw-rw-   0        0        0     3026 2023-07-26 09:03:48.000000 zlgsendcan-1.2.1/zlgsendcan/get_conf_info.py
--rw-rw-rw-   0        0        0     5271 2023-07-27 02:13:20.000000 zlgsendcan-1.2.1/zlgsendcan/parseDBC.py
--rw-rw-rw-   0        0        0     1122 2023-07-26 08:41:01.000000 zlgsendcan-1.2.1/zlgsendcan/yaml_util.py
--rw-rw-rw-   0        0        0    25707 2023-07-27 05:06:39.000000 zlgsendcan-1.2.1/zlgsendcan/zlgcan1.py
--rw-rw-rw-   0        0        0    19479 2023-07-28 03:12:11.000000 zlgsendcan-1.2.1/zlgsendcan/zlgserver.py
-drwxrwxrwx   0        0        0        0 2023-07-28 03:12:49.329458 zlgsendcan-1.2.1/zlgsendcan.egg-info/
--rw-rw-rw-   0        0        0      221 2023-07-28 03:12:49.000000 zlgsendcan-1.2.1/zlgsendcan.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      373 2023-07-28 03:12:49.000000 zlgsendcan-1.2.1/zlgsendcan.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-28 03:12:49.000000 zlgsendcan-1.2.1/zlgsendcan.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       16 2023-07-28 03:12:49.000000 zlgsendcan-1.2.1/zlgsendcan.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-07-28 03:12:49.000000 zlgsendcan-1.2.1/zlgsendcan.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-08-08 03:14:19.105899 zlgsendcan-1.2.2/
+-rw-rw-rw-   0        0        0      221 2023-08-08 03:14:19.105899 zlgsendcan-1.2.2/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2023-08-08 03:14:19.105899 zlgsendcan-1.2.2/setup.cfg
+-rw-rw-rw-   0        0        0      458 2023-08-08 03:07:12.000000 zlgsendcan-1.2.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-08 03:14:19.096906 zlgsendcan-1.2.2/zlgsendcan/
+-rw-rw-rw-   0        0        0        0 2023-07-26 06:34:10.000000 zlgsendcan-1.2.2/zlgsendcan/__init__.py
+-rw-rw-rw-   0        0        0     2076 2023-07-27 04:16:37.000000 zlgsendcan-1.2.2/zlgsendcan/example_test.py
+-rw-rw-rw-   0        0        0      237 2023-02-14 03:41:12.000000 zlgsendcan-1.2.2/zlgsendcan/frozen_dir.py
+-rw-rw-rw-   0        0        0     3026 2023-07-26 09:03:48.000000 zlgsendcan-1.2.2/zlgsendcan/get_conf_info.py
+-rw-rw-rw-   0        0        0      744 2023-08-08 03:07:39.000000 zlgsendcan-1.2.2/zlgsendcan/img_compare.py
+-rw-rw-rw-   0        0        0     5271 2023-07-27 02:13:20.000000 zlgsendcan-1.2.2/zlgsendcan/parseDBC.py
+-rw-rw-rw-   0        0        0     1122 2023-07-26 08:41:01.000000 zlgsendcan-1.2.2/zlgsendcan/yaml_util.py
+-rw-rw-rw-   0        0        0    25707 2023-07-27 05:06:39.000000 zlgsendcan-1.2.2/zlgsendcan/zlgcan1.py
+-rw-rw-rw-   0        0        0    19479 2023-07-28 03:12:11.000000 zlgsendcan-1.2.2/zlgsendcan/zlgserver.py
+drwxrwxrwx   0        0        0        0 2023-08-08 03:14:19.103980 zlgsendcan-1.2.2/zlgsendcan.egg-info/
+-rw-rw-rw-   0        0        0      221 2023-08-08 03:14:18.000000 zlgsendcan-1.2.2/zlgsendcan.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      399 2023-08-08 03:14:19.000000 zlgsendcan-1.2.2/zlgsendcan.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-08 03:14:18.000000 zlgsendcan-1.2.2/zlgsendcan.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       24 2023-08-08 03:14:18.000000 zlgsendcan-1.2.2/zlgsendcan.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-08-08 03:14:18.000000 zlgsendcan-1.2.2/zlgsendcan.egg-info/top_level.txt
```

### Comparing `zlgsendcan-1.2.1/zlgsendcan/example_test.py` & `zlgsendcan-1.2.2/zlgsendcan/example_test.py`

 * *Files identical despite different names*

### Comparing `zlgsendcan-1.2.1/zlgsendcan/get_conf_info.py` & `zlgsendcan-1.2.2/zlgsendcan/get_conf_info.py`

 * *Files identical despite different names*

### Comparing `zlgsendcan-1.2.1/zlgsendcan/parseDBC.py` & `zlgsendcan-1.2.2/zlgsendcan/parseDBC.py`

 * *Files identical despite different names*

### Comparing `zlgsendcan-1.2.1/zlgsendcan/yaml_util.py` & `zlgsendcan-1.2.2/zlgsendcan/yaml_util.py`

 * *Files identical despite different names*

### Comparing `zlgsendcan-1.2.1/zlgsendcan/zlgcan1.py` & `zlgsendcan-1.2.2/zlgsendcan/zlgcan1.py`

 * *Files identical despite different names*

### Comparing `zlgsendcan-1.2.1/zlgsendcan/zlgserver.py` & `zlgsendcan-1.2.2/zlgsendcan/zlgserver.py`

 * *Files identical despite different names*


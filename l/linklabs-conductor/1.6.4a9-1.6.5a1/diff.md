# Comparing `tmp/linklabs-conductor-1.6.4a9.tar.gz` & `tmp/linklabs-conductor-1.6.5a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/linklabs-conductor-1.6.4a9.tar", last modified: Mon Mar  6 18:06:39 2023, max compression
+gzip compressed data, was "dist/linklabs-conductor-1.6.5a1.tar", last modified: Tue Aug  8 16:28:40 2023, max compression
```

## Comparing `linklabs-conductor-1.6.4a9.tar` & `linklabs-conductor-1.6.5a1.tar`

### file list

```diff
@@ -1,53 +1,53 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-06 18:06:39.000000 linklabs-conductor-1.6.4a9/
--rw-rw-rw-   0 root         (0) root         (0)     1069 2023-03-06 18:06:18.000000 linklabs-conductor-1.6.4a9/LICENSE.txt
--rw-rw-rw-   0 root         (0) root         (0)       41 2023-03-06 18:06:18.000000 linklabs-conductor-1.6.4a9/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2717 2023-03-06 18:06:39.000000 linklabs-conductor-1.6.4a9/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     1759 2023-03-06 18:06:18.000000 linklabs-conductor-1.6.4a9/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-06 18:06:39.000000 linklabs-conductor-1.6.4a9/conductor/
--rw-rw-rw-   0 root         (0) root         (0)      749 2023-03-06 18:06:18.000000 linklabs-conductor-1.6.4a9/conductor/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    12874 2023-03-06 18:06:18.000000 linklabs-conductor-1.6.4a9/conductor/account.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-06 18:06:39.000000 linklabs-conductor-1.6.4a9/conductor/airfinder/
--rw-rw-rw-   0 root         (0) root         (0)      575 2023-03-06 18:06:18.000000 linklabs-conductor-1.6.4a9/conductor/airfinder/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3922 2023-03-06 18:06:18.000000 linklabs-conductor-1.6.4a9/conductor/airfinder/area.py
--rw-rw-rw-   0 root         (0) root         (0)     6954 2023-03-06 18:06:18.000000 linklabs-conductor-1.6.4a9/conductor/airfinder/base.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-06 18:06:39.000000 linklabs-conductor-1.6.4a9/conductor/airfinder/devices/
--rw-rw-rw-   0 root         (0) root         (0)      710 2023-03-06 18:06:18.000000 linklabs-conductor-1.6.4a9/conductor/airfinder/devices/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    82030 2023-03-06 18:06:18.000000 linklabs-conductor-1.6.4a9/conductor/airfinder/devices/access_point.py
--rw-rw-rw-   0 root         (0) root         (0)      535 2023-03-06 18:06:18.000000 linklabs-conductor-1.6.4a9/conductor/airfinder/devices/af3_location.py
--rw-rw-rw-   0 root         (0) root         (0)    14056 2023-03-06 18:06:18.000000 linklabs-conductor-1.6.4a9/conductor/airfinder/devices/alert_tag.py
--rw-rw-rw-   0 root         (0) root         (0)    15829 2023-03-06 18:06:18.000000 linklabs-conductor-1.6.4a9/conductor/airfinder/devices/location.py
--rw-rw-rw-   0 root         (0) root         (0)    12155 2023-03-06 18:06:18.000000 linklabs-conductor-1.6.4a9/conductor/airfinder/devices/node.py
--rw-rw-rw-   0 root         (0) root         (0)    82649 2023-03-06 18:06:18.000000 linklabs-conductor-1.6.4a9/conductor/airfinder/devices/nordic_access_point.py
--rw-rw-rw-   0 root         (0) root         (0)      549 2023-03-06 18:06:18.000000 linklabs-conductor-1.6.4a9/conductor/airfinder/devices/rpi_access_point.py
--rw-rw-rw-   0 root         (0) root         (0)    31258 2023-03-06 18:06:18.000000 linklabs-conductor-1.6.4a9/conductor/airfinder/devices/sercomm_supertag.py
--rw-rw-rw-   0 root         (0) root         (0)     2896 2023-03-06 18:06:18.000000 linklabs-conductor-1.6.4a9/conductor/airfinder/devices/ssf.py
--rw-rw-rw-   0 root         (0) root         (0)     7506 2023-03-06 18:06:18.000000 linklabs-conductor-1.6.4a9/conductor/airfinder/devices/supertag.py
--rw-rw-rw-   0 root         (0) root         (0)     7395 2023-03-06 18:06:18.000000 linklabs-conductor-1.6.4a9/conductor/airfinder/devices/tag.py
--rw-rw-rw-   0 root         (0) root         (0)     1824 2023-03-06 18:06:18.000000 linklabs-conductor-1.6.4a9/conductor/airfinder/devices/test_tag.py
--rw-rw-rw-   0 root         (0) root         (0)     1286 2023-03-06 18:06:18.000000 linklabs-conductor-1.6.4a9/conductor/airfinder/devices/xle_access_point.py
--rw-rw-rw-   0 root         (0) root         (0)    14368 2023-03-06 18:06:18.000000 linklabs-conductor-1.6.4a9/conductor/airfinder/messages.py
--rw-rw-rw-   0 root         (0) root         (0)     1023 2023-03-06 18:06:18.000000 linklabs-conductor-1.6.4a9/conductor/airfinder/organization.py
--rw-rw-rw-   0 root         (0) root         (0)    17518 2023-03-06 18:06:18.000000 linklabs-conductor-1.6.4a9/conductor/airfinder/site.py
--rw-rw-rw-   0 root         (0) root         (0)     6711 2023-03-06 18:06:18.000000 linklabs-conductor-1.6.4a9/conductor/airfinder/user.py
--rw-rw-rw-   0 root         (0) root         (0)     1034 2023-03-06 18:06:18.000000 linklabs-conductor-1.6.4a9/conductor/airfinder/util.py
--rw-rw-rw-   0 root         (0) root         (0)     3556 2023-03-06 18:06:18.000000 linklabs-conductor-1.6.4a9/conductor/airfinder/zone.py
--rw-rw-rw-   0 root         (0) root         (0)     6020 2023-03-06 18:06:18.000000 linklabs-conductor-1.6.4a9/conductor/asset_group.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-06 18:06:39.000000 linklabs-conductor-1.6.4a9/conductor/devices/
--rw-rw-rw-   0 root         (0) root         (0)      119 2023-03-06 18:06:18.000000 linklabs-conductor-1.6.4a9/conductor/devices/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5413 2023-03-06 18:06:18.000000 linklabs-conductor-1.6.4a9/conductor/devices/gateway.py
--rw-rw-rw-   0 root         (0) root         (0)     5775 2023-03-06 18:06:18.000000 linklabs-conductor-1.6.4a9/conductor/devices/lte_module.py
--rw-rw-rw-   0 root         (0) root         (0)     5143 2023-03-06 18:06:18.000000 linklabs-conductor-1.6.4a9/conductor/devices/module.py
--rw-rw-rw-   0 root         (0) root         (0)     2735 2023-03-06 18:06:18.000000 linklabs-conductor-1.6.4a9/conductor/event_count.py
--rw-rw-rw-   0 root         (0) root         (0)    19420 2023-03-06 18:06:18.000000 linklabs-conductor-1.6.4a9/conductor/subject.py
--rw-rw-rw-   0 root         (0) root         (0)    12636 2023-03-06 18:06:18.000000 linklabs-conductor-1.6.4a9/conductor/subscriptions.py
--rw-rw-rw-   0 root         (0) root         (0)     3360 2023-03-06 18:06:18.000000 linklabs-conductor-1.6.4a9/conductor/tokens.py
--rw-rw-rw-   0 root         (0) root         (0)     6949 2023-03-06 18:06:18.000000 linklabs-conductor-1.6.4a9/conductor/util.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-06 18:06:39.000000 linklabs-conductor-1.6.4a9/linklabs_conductor.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2717 2023-03-06 18:06:39.000000 linklabs-conductor-1.6.4a9/linklabs_conductor.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1433 2023-03-06 18:06:39.000000 linklabs-conductor-1.6.4a9/linklabs_conductor.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-03-06 18:06:39.000000 linklabs-conductor-1.6.4a9/linklabs_conductor.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       25 2023-03-06 18:06:39.000000 linklabs-conductor-1.6.4a9/linklabs_conductor.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       10 2023-03-06 18:06:39.000000 linklabs-conductor-1.6.4a9/linklabs_conductor.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)      119 2023-03-06 18:06:18.000000 linklabs-conductor-1.6.4a9/pyproject.toml
--rw-rw-rw-   0 root         (0) root         (0)       67 2023-03-06 18:06:39.000000 linklabs-conductor-1.6.4a9/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1027 2023-03-06 18:06:18.000000 linklabs-conductor-1.6.4a9/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-08 16:28:40.000000 linklabs-conductor-1.6.5a1/
+-rw-rw-rw-   0 root         (0) root         (0)     1062 2023-08-08 16:28:11.000000 linklabs-conductor-1.6.5a1/LICENSE.txt
+-rw-rw-rw-   0 root         (0) root         (0)       41 2023-08-08 16:28:11.000000 linklabs-conductor-1.6.5a1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2717 2023-08-08 16:28:40.000000 linklabs-conductor-1.6.5a1/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     1759 2023-08-08 16:28:11.000000 linklabs-conductor-1.6.5a1/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-08 16:28:40.000000 linklabs-conductor-1.6.5a1/conductor/
+-rw-rw-rw-   0 root         (0) root         (0)      749 2023-08-08 16:28:11.000000 linklabs-conductor-1.6.5a1/conductor/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    12874 2023-08-08 16:28:11.000000 linklabs-conductor-1.6.5a1/conductor/account.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-08 16:28:40.000000 linklabs-conductor-1.6.5a1/conductor/airfinder/
+-rw-rw-rw-   0 root         (0) root         (0)      575 2023-08-08 16:28:11.000000 linklabs-conductor-1.6.5a1/conductor/airfinder/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3922 2023-08-08 16:28:11.000000 linklabs-conductor-1.6.5a1/conductor/airfinder/area.py
+-rw-rw-rw-   0 root         (0) root         (0)     6954 2023-08-08 16:28:11.000000 linklabs-conductor-1.6.5a1/conductor/airfinder/base.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-08 16:28:40.000000 linklabs-conductor-1.6.5a1/conductor/airfinder/devices/
+-rw-rw-rw-   0 root         (0) root         (0)      710 2023-08-08 16:28:11.000000 linklabs-conductor-1.6.5a1/conductor/airfinder/devices/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    82030 2023-08-08 16:28:11.000000 linklabs-conductor-1.6.5a1/conductor/airfinder/devices/access_point.py
+-rw-rw-rw-   0 root         (0) root         (0)      535 2023-08-08 16:28:11.000000 linklabs-conductor-1.6.5a1/conductor/airfinder/devices/af3_location.py
+-rw-rw-rw-   0 root         (0) root         (0)    14056 2023-08-08 16:28:11.000000 linklabs-conductor-1.6.5a1/conductor/airfinder/devices/alert_tag.py
+-rw-rw-rw-   0 root         (0) root         (0)    15829 2023-08-08 16:28:11.000000 linklabs-conductor-1.6.5a1/conductor/airfinder/devices/location.py
+-rw-rw-rw-   0 root         (0) root         (0)    12155 2023-08-08 16:28:11.000000 linklabs-conductor-1.6.5a1/conductor/airfinder/devices/node.py
+-rw-rw-rw-   0 root         (0) root         (0)    82649 2023-08-08 16:28:11.000000 linklabs-conductor-1.6.5a1/conductor/airfinder/devices/nordic_access_point.py
+-rw-rw-rw-   0 root         (0) root         (0)      549 2023-08-08 16:28:11.000000 linklabs-conductor-1.6.5a1/conductor/airfinder/devices/rpi_access_point.py
+-rw-rw-rw-   0 root         (0) root         (0)    31258 2023-08-08 16:28:11.000000 linklabs-conductor-1.6.5a1/conductor/airfinder/devices/sercomm_supertag.py
+-rw-rw-rw-   0 root         (0) root         (0)     2896 2023-08-08 16:28:11.000000 linklabs-conductor-1.6.5a1/conductor/airfinder/devices/ssf.py
+-rw-rw-rw-   0 root         (0) root         (0)     7506 2023-08-08 16:28:11.000000 linklabs-conductor-1.6.5a1/conductor/airfinder/devices/supertag.py
+-rw-rw-rw-   0 root         (0) root         (0)     7395 2023-08-08 16:28:11.000000 linklabs-conductor-1.6.5a1/conductor/airfinder/devices/tag.py
+-rw-rw-rw-   0 root         (0) root         (0)     1824 2023-08-08 16:28:11.000000 linklabs-conductor-1.6.5a1/conductor/airfinder/devices/test_tag.py
+-rw-rw-rw-   0 root         (0) root         (0)     1286 2023-08-08 16:28:11.000000 linklabs-conductor-1.6.5a1/conductor/airfinder/devices/xle_access_point.py
+-rw-rw-rw-   0 root         (0) root         (0)    14368 2023-08-08 16:28:11.000000 linklabs-conductor-1.6.5a1/conductor/airfinder/messages.py
+-rw-rw-rw-   0 root         (0) root         (0)     1023 2023-08-08 16:28:11.000000 linklabs-conductor-1.6.5a1/conductor/airfinder/organization.py
+-rw-rw-rw-   0 root         (0) root         (0)    17518 2023-08-08 16:28:11.000000 linklabs-conductor-1.6.5a1/conductor/airfinder/site.py
+-rw-rw-rw-   0 root         (0) root         (0)     6711 2023-08-08 16:28:11.000000 linklabs-conductor-1.6.5a1/conductor/airfinder/user.py
+-rw-rw-rw-   0 root         (0) root         (0)     1034 2023-08-08 16:28:11.000000 linklabs-conductor-1.6.5a1/conductor/airfinder/util.py
+-rw-rw-rw-   0 root         (0) root         (0)     3556 2023-08-08 16:28:11.000000 linklabs-conductor-1.6.5a1/conductor/airfinder/zone.py
+-rw-rw-rw-   0 root         (0) root         (0)     6020 2023-08-08 16:28:11.000000 linklabs-conductor-1.6.5a1/conductor/asset_group.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-08 16:28:40.000000 linklabs-conductor-1.6.5a1/conductor/devices/
+-rw-rw-rw-   0 root         (0) root         (0)      119 2023-08-08 16:28:11.000000 linklabs-conductor-1.6.5a1/conductor/devices/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     6380 2023-08-08 16:28:11.000000 linklabs-conductor-1.6.5a1/conductor/devices/gateway.py
+-rw-rw-rw-   0 root         (0) root         (0)     5775 2023-08-08 16:28:11.000000 linklabs-conductor-1.6.5a1/conductor/devices/lte_module.py
+-rw-rw-rw-   0 root         (0) root         (0)     5143 2023-08-08 16:28:11.000000 linklabs-conductor-1.6.5a1/conductor/devices/module.py
+-rw-rw-rw-   0 root         (0) root         (0)     2735 2023-08-08 16:28:11.000000 linklabs-conductor-1.6.5a1/conductor/event_count.py
+-rw-rw-rw-   0 root         (0) root         (0)    19676 2023-08-08 16:28:11.000000 linklabs-conductor-1.6.5a1/conductor/subject.py
+-rw-rw-rw-   0 root         (0) root         (0)    12636 2023-08-08 16:28:11.000000 linklabs-conductor-1.6.5a1/conductor/subscriptions.py
+-rw-rw-rw-   0 root         (0) root         (0)     3360 2023-08-08 16:28:11.000000 linklabs-conductor-1.6.5a1/conductor/tokens.py
+-rw-rw-rw-   0 root         (0) root         (0)     6949 2023-08-08 16:28:11.000000 linklabs-conductor-1.6.5a1/conductor/util.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-08 16:28:40.000000 linklabs-conductor-1.6.5a1/linklabs_conductor.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2717 2023-08-08 16:28:39.000000 linklabs-conductor-1.6.5a1/linklabs_conductor.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1433 2023-08-08 16:28:39.000000 linklabs-conductor-1.6.5a1/linklabs_conductor.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-08-08 16:28:39.000000 linklabs-conductor-1.6.5a1/linklabs_conductor.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       25 2023-08-08 16:28:39.000000 linklabs-conductor-1.6.5a1/linklabs_conductor.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       10 2023-08-08 16:28:39.000000 linklabs-conductor-1.6.5a1/linklabs_conductor.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)      119 2023-08-08 16:28:11.000000 linklabs-conductor-1.6.5a1/pyproject.toml
+-rw-rw-rw-   0 root         (0) root         (0)       67 2023-08-08 16:28:40.000000 linklabs-conductor-1.6.5a1/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1027 2023-08-08 16:28:11.000000 linklabs-conductor-1.6.5a1/setup.py
```

### Comparing `linklabs-conductor-1.6.4a9/LICENSE.txt` & `linklabs-conductor-1.6.5a1/LICENSE.txt`

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-Copyright (c) 2016, 2017, 2018 Link Labs LLC
+Copyright (c) 2016-2023 Link Labs LLC
 
 Permission is hereby granted, free of charge, to any person obtaining a copy of
 this software and associated documentation files (the "Software"), to deal in
 the Software without restriction, including without limitation the rights to
 use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies
 of the Software, and to permit persons to whom the Software is furnished to do
 so, subject to the following conditions:
```

### Comparing `linklabs-conductor-1.6.4a9/PKG-INFO` & `linklabs-conductor-1.6.5a1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: linklabs-conductor
-Version: 1.6.4a9
+Version: 1.6.5a1
 Summary: Linklabs Conductor API Wrapper
 Home-page: https://www.link-labs.com
 Author: Linklabs, LLC
 Author-email: support@link-labs.com
 License: MIT
 Description: ***********************************
         Conductor+Airfinder Python Library
```

### Comparing `linklabs-conductor-1.6.4a9/README.rst` & `linklabs-conductor-1.6.5a1/README.rst`

 * *Files identical despite different names*

### Comparing `linklabs-conductor-1.6.4a9/conductor/__init__.py` & `linklabs-conductor-1.6.5a1/conductor/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """ This module wraps the Conductor API. """
-CONDUCTOR_LIBRARY_VERSION = '1.6.4a9'
+CONDUCTOR_LIBRARY_VERSION = '1.6.5a1'
 
 PRODUCTION = 'conductor.link-labs'
 HOSPITALITY = 'hospitality.airfinder'
 UAT = 'hospitality-uat.airfinder'
 TEST = 'test.airfinder'
 DEVELOP = 'dev.link-labs'
```

### Comparing `linklabs-conductor-1.6.4a9/conductor/account.py` & `linklabs-conductor-1.6.5a1/conductor/account.py`

 * *Files identical despite different names*

### Comparing `linklabs-conductor-1.6.4a9/conductor/airfinder/__init__.py` & `linklabs-conductor-1.6.5a1/conductor/airfinder/__init__.py`

 * *Files identical despite different names*

### Comparing `linklabs-conductor-1.6.4a9/conductor/airfinder/area.py` & `linklabs-conductor-1.6.5a1/conductor/airfinder/area.py`

 * *Files identical despite different names*

### Comparing `linklabs-conductor-1.6.4a9/conductor/airfinder/base.py` & `linklabs-conductor-1.6.5a1/conductor/airfinder/base.py`

 * *Files identical despite different names*

### Comparing `linklabs-conductor-1.6.4a9/conductor/airfinder/devices/__init__.py` & `linklabs-conductor-1.6.5a1/conductor/airfinder/devices/__init__.py`

 * *Files identical despite different names*

### Comparing `linklabs-conductor-1.6.4a9/conductor/airfinder/devices/access_point.py` & `linklabs-conductor-1.6.5a1/conductor/airfinder/devices/access_point.py`

 * *Files identical despite different names*

### Comparing `linklabs-conductor-1.6.4a9/conductor/airfinder/devices/af3_location.py` & `linklabs-conductor-1.6.5a1/conductor/airfinder/devices/af3_location.py`

 * *Files identical despite different names*

### Comparing `linklabs-conductor-1.6.4a9/conductor/airfinder/devices/alert_tag.py` & `linklabs-conductor-1.6.5a1/conductor/airfinder/devices/alert_tag.py`

 * *Files identical despite different names*

### Comparing `linklabs-conductor-1.6.4a9/conductor/airfinder/devices/location.py` & `linklabs-conductor-1.6.5a1/conductor/airfinder/devices/location.py`

 * *Files identical despite different names*

### Comparing `linklabs-conductor-1.6.4a9/conductor/airfinder/devices/node.py` & `linklabs-conductor-1.6.5a1/conductor/airfinder/devices/node.py`

 * *Files identical despite different names*

### Comparing `linklabs-conductor-1.6.4a9/conductor/airfinder/devices/nordic_access_point.py` & `linklabs-conductor-1.6.5a1/conductor/airfinder/devices/nordic_access_point.py`

 * *Files identical despite different names*

### Comparing `linklabs-conductor-1.6.4a9/conductor/airfinder/devices/rpi_access_point.py` & `linklabs-conductor-1.6.5a1/conductor/airfinder/devices/rpi_access_point.py`

 * *Files identical despite different names*

### Comparing `linklabs-conductor-1.6.4a9/conductor/airfinder/devices/sercomm_supertag.py` & `linklabs-conductor-1.6.5a1/conductor/airfinder/devices/sercomm_supertag.py`

 * *Files identical despite different names*

### Comparing `linklabs-conductor-1.6.4a9/conductor/airfinder/devices/ssf.py` & `linklabs-conductor-1.6.5a1/conductor/airfinder/devices/ssf.py`

 * *Files identical despite different names*

### Comparing `linklabs-conductor-1.6.4a9/conductor/airfinder/devices/supertag.py` & `linklabs-conductor-1.6.5a1/conductor/airfinder/devices/supertag.py`

 * *Files identical despite different names*

### Comparing `linklabs-conductor-1.6.4a9/conductor/airfinder/devices/tag.py` & `linklabs-conductor-1.6.5a1/conductor/airfinder/devices/tag.py`

 * *Files identical despite different names*

### Comparing `linklabs-conductor-1.6.4a9/conductor/airfinder/devices/test_tag.py` & `linklabs-conductor-1.6.5a1/conductor/airfinder/devices/test_tag.py`

 * *Files identical despite different names*

### Comparing `linklabs-conductor-1.6.4a9/conductor/airfinder/devices/xle_access_point.py` & `linklabs-conductor-1.6.5a1/conductor/airfinder/devices/xle_access_point.py`

 * *Files identical despite different names*

### Comparing `linklabs-conductor-1.6.4a9/conductor/airfinder/messages.py` & `linklabs-conductor-1.6.5a1/conductor/airfinder/messages.py`

 * *Files identical despite different names*

### Comparing `linklabs-conductor-1.6.4a9/conductor/airfinder/organization.py` & `linklabs-conductor-1.6.5a1/conductor/airfinder/organization.py`

 * *Files identical despite different names*

### Comparing `linklabs-conductor-1.6.4a9/conductor/airfinder/site.py` & `linklabs-conductor-1.6.5a1/conductor/airfinder/site.py`

 * *Files identical despite different names*

### Comparing `linklabs-conductor-1.6.4a9/conductor/airfinder/user.py` & `linklabs-conductor-1.6.5a1/conductor/airfinder/user.py`

 * *Files identical despite different names*

### Comparing `linklabs-conductor-1.6.4a9/conductor/airfinder/util.py` & `linklabs-conductor-1.6.5a1/conductor/airfinder/util.py`

 * *Files identical despite different names*

### Comparing `linklabs-conductor-1.6.4a9/conductor/airfinder/zone.py` & `linklabs-conductor-1.6.5a1/conductor/airfinder/zone.py`

 * *Files identical despite different names*

### Comparing `linklabs-conductor-1.6.4a9/conductor/asset_group.py` & `linklabs-conductor-1.6.5a1/conductor/asset_group.py`

 * *Files identical despite different names*

### Comparing `linklabs-conductor-1.6.4a9/conductor/devices/gateway.py` & `linklabs-conductor-1.6.5a1/conductor/devices/gateway.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import struct
+import warnings
 
-from datetime import datetime
+from datetime import datetime, timedelta
 
 from ..event_count import EventCount
-from ..subject import UplinkSubject, DownlinkSubject, UplinkMessage
+from ..subject import UplinkSubject, DownlinkSubject, UplinkMessage, FailedAPICallException
 from ..util import format_time
 
 # TODO: Format Documentation.
 # TODO: Supply properties for all avalible values.
 # TODO: Unittest functionality.
 # TODO: See what additional functionality can be added.
 # TODO: Don't require net token.
@@ -16,14 +17,26 @@
 def flatten_status(results):
     """Flattens the status message's 'properties' dictionary."""
     for status in results:
         status["value"]["properties"] = {d["name"]: d["value"] for d in status["value"]["properties"]}
     return results
 
 
+def compare_min_version(version_string, major, minor, tag):
+    version = [int(v) for v in version_string.split(".")]
+    if version[0] < major:
+        return False
+    elif version[0] == major:
+        if version[1] < minor:
+            return False
+        elif version[1] == minor and version[2] < tag:
+            return False
+    return True
+
+
 class GatewayUplinkMessage(UplinkMessage):
     """Represents an uplink message from a gateway."""
 
     pass
 
 
 class Gateway(UplinkSubject, DownlinkSubject, EventCount):
@@ -31,33 +44,40 @@
 
     subject_name = "node"  # TODO: gateway????
     msgObj = GatewayUplinkMessage
 
     def get_status(self):
         """Returns the most recent gateway status dictionary"""
         url = "{}/data/gatewayStatus/node/{}/mostRecentEvents".format(self.client_edge_url, self.subject_id)
-        params = {"f.__prop.type": "EQ.status", "maxResults": 1}
+        params = {"maxResults": 1}
         return flatten_status(self._get(url, params=params)["results"])
 
-    def get_config(self):
-        url = "{}/data/gatewayStatus/node/{}/mostRecentEvents".format(self.client_edge_url, self.subject_id)
-        params = {"f.__prop.type": "EQ.config", "maxResults": 1}
-        return flatten_status(self._get(url, params=params)["results"])
+    def get_config(self, query_interval_m=60):
+        # Perform a query and filter to get the most recent config message
+        _now = datetime.utcnow()
+        _stati = self.get_statuses(_now - timedelta(minutes=query_interval_m), _now)
+        _filtered = [_s for _s in _stati if _s["metadata"]["props"]["type"] == "config"]
+        if len(_filtered) == 0:
+            raise FailedAPICallException(
+                "No config messages sent in the provided interval ({} mins), retry with a longer interval".format(
+                    query_interval_m
+                )
+            )
+        return _filtered[0]
 
-    def get_last_gw_uplink(self, num):
-        url = "{}/data/gatewayStatus/node/{}/mostRecentEvents".format(self.client_edge_url, self.subject_id)
-        params = {"f.linkType": "EQ.4094-GW_Customer", "maxResults": num}
-        return flatten_status(self._get(url, params=params)["results"])
+    def get_last_gw_uplink(self, num=1):
+        warnings.warn("This method has been deprecated")
 
     def get_cell_status(self):
-        """Returns the most recent gateway cellular status dictionary if
-        exists"""
-        url = "{}/data/gatewayStatus/node/{}/mostRecentEvents".format(self.client_edge_url, self.subject_id)
-        params = {"f.__prop.type": "EQ.status", "maxResults": 1}
-        return flatten_status(self._get(url, params=params)["results"])
+        # Retrieve the most recent status and filter by cell signal data
+        _status = self.get_status()
+        if len(_status) == 0:
+            raise FailedAPICallException("Could not retrieve gateway status")
+        signal_data = {k: v for k, v in _status[0]["value"]["properties"].items() if "network_signal" in k}
+        return signal_data
 
     def get_statuses(self, start_time, stop_time):
         """Returns the status messages for a particular time range."""
         url = "{}/data/gatewayStatus/node/{}/events/{}/{}".format(
             self.client_edge_url, self.subject_id, format_time(stop_time), format_time(start_time)
         )
         return flatten_status(self._get(url)["results"])
@@ -113,14 +133,23 @@
             auto_mode(bool): True to set downlink channel auto.
             channel(int): A channel number when downlink is manual.
             ttl_s(float): Time to live in seconds.
 
         Returns:
             :class`.DownlinkMessage`
         """
+        # Check version
+        _version = self._data.get("gatewayConfig").get("gateway_release_version")
+        if _version is None:
+            warnings.warn(
+                "Cannot retrieve gateway release version, this function will not work if the gateway release < 2.1.1"
+            )
+        elif not compare_min_version(_version, 2, 1, 1):
+            warnings.warn("Gateway version too old, this function will not work")
+
         if auto_mode is False:
             if channel is None:
                 raise ValueError("When auto_mode is manual (False), a channel number must be provided")
             elif channel < 0 or channel > 47:
                 raise ValueError("Channel value must fall within the range 0-47")
         else:
             channel = 0
```

### Comparing `linklabs-conductor-1.6.4a9/conductor/devices/lte_module.py` & `linklabs-conductor-1.6.5a1/conductor/devices/lte_module.py`

 * *Files identical despite different names*

### Comparing `linklabs-conductor-1.6.4a9/conductor/devices/module.py` & `linklabs-conductor-1.6.5a1/conductor/devices/module.py`

 * *Files identical despite different names*

### Comparing `linklabs-conductor-1.6.4a9/conductor/event_count.py` & `linklabs-conductor-1.6.5a1/conductor/event_count.py`

 * *Files identical despite different names*

### Comparing `linklabs-conductor-1.6.4a9/conductor/subject.py` & `linklabs-conductor-1.6.5a1/conductor/subject.py`

 * *Files 2% similar despite different names*

```diff
@@ -364,26 +364,29 @@
             for k, v in md.items():
                 if self._data and k in self._data:
                     self._data[k] = v
         return self.msgObj(*args)
 
     # TODO: create more generic get message method.
 
-    def get_messages_time_range(self, start, stop=None):
+    def get_messages_time_range(self, start, stop=None, slack=1.0):
         """Retrieves all messages within a start and stop time.
+        NOTE: The slack parameter was added to compensate for server errors when local machine time is slightly ahead
+         of server machine time.
 
         Args:
             start (:class:`.datetime.datetime`): Start Time.
             stop (:class:`datetime.datetime`): [Optional] Stop Time, will
                 default to the current time of when the method is called.
+            slack (:float:): [Optional] slack from current time.
 
         Returns:
             A list of :obj:`UplinkMessage` objects.
         """
-        stop = stop or datetime.utcnow()
+        stop = stop or (datetime.utcnow() - timedelta(seconds=slack))
         base_url = "{}/data/{}/{}/{}/events/{}/{}".format(
             self.client_edge_url,
             self.uplink_type,
             self.subject_name,
             self.subject_id,
             format_time(stop),
             format_time(start),
```

### Comparing `linklabs-conductor-1.6.4a9/conductor/subscriptions.py` & `linklabs-conductor-1.6.5a1/conductor/subscriptions.py`

 * *Files identical despite different names*

### Comparing `linklabs-conductor-1.6.4a9/conductor/tokens.py` & `linklabs-conductor-1.6.5a1/conductor/tokens.py`

 * *Files identical despite different names*

### Comparing `linklabs-conductor-1.6.4a9/conductor/util.py` & `linklabs-conductor-1.6.5a1/conductor/util.py`

 * *Files identical despite different names*

### Comparing `linklabs-conductor-1.6.4a9/linklabs_conductor.egg-info/PKG-INFO` & `linklabs-conductor-1.6.5a1/linklabs_conductor.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: linklabs-conductor
-Version: 1.6.4a9
+Version: 1.6.5a1
 Summary: Linklabs Conductor API Wrapper
 Home-page: https://www.link-labs.com
 Author: Linklabs, LLC
 Author-email: support@link-labs.com
 License: MIT
 Description: ***********************************
         Conductor+Airfinder Python Library
```

### Comparing `linklabs-conductor-1.6.4a9/linklabs_conductor.egg-info/SOURCES.txt` & `linklabs-conductor-1.6.5a1/linklabs_conductor.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `linklabs-conductor-1.6.4a9/setup.py` & `linklabs-conductor-1.6.5a1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from codecs import open
 from os import path
 
 here = path.abspath(path.dirname(__file__))
 
 setup(
     name='linklabs-conductor',
-    version='1.6.4a9',
+    version='1.6.5a1',
     description='Linklabs Conductor API Wrapper',
     long_description_content_type='text/x-rst',
     long_description=open('README.rst', encoding='utf-8').read(),
     url='https://www.link-labs.com',
     author='Linklabs, LLC',
     author_email='support@link-labs.com',
     license='MIT',
```


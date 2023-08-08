# Comparing `tmp/alibabacloud_cbn20170912-1.0.31.tar.gz` & `tmp/alibabacloud_cbn20170912-1.0.32.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/alibabacloud_cbn20170912-1.0.31.tar", last modified: Tue Aug  8 01:38:36 2023, max compression
+gzip compressed data, was "dist/alibabacloud_cbn20170912-1.0.32.tar", last modified: Tue Aug  8 08:03:49 2023, max compression
```

## Comparing `alibabacloud_cbn20170912-1.0.31.tar` & `alibabacloud_cbn20170912-1.0.32.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-08 01:38:36.000000 alibabacloud_cbn20170912-1.0.31/
--rw-r--r--   0 root         (0) root         (0)     5779 2023-08-08 01:38:35.000000 alibabacloud_cbn20170912-1.0.31/ChangeLog.md
--rw-r--r--   0 root         (0) root         (0)      600 2023-08-08 01:38:35.000000 alibabacloud_cbn20170912-1.0.31/LICENSE
--rw-r--r--   0 root         (0) root         (0)       29 2023-08-08 01:38:35.000000 alibabacloud_cbn20170912-1.0.31/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2350 2023-08-08 01:38:36.000000 alibabacloud_cbn20170912-1.0.31/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1022 2023-08-08 01:38:35.000000 alibabacloud_cbn20170912-1.0.31/README-CN.md
--rw-r--r--   0 root         (0) root         (0)     1107 2023-08-08 01:38:35.000000 alibabacloud_cbn20170912-1.0.31/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-08 01:38:36.000000 alibabacloud_cbn20170912-1.0.31/alibabacloud_cbn20170912/
--rw-r--r--   0 root         (0) root         (0)       22 2023-08-08 01:38:35.000000 alibabacloud_cbn20170912-1.0.31/alibabacloud_cbn20170912/__init__.py
--rw-r--r--   0 root         (0) root         (0)  1024624 2023-08-08 01:38:35.000000 alibabacloud_cbn20170912-1.0.31/alibabacloud_cbn20170912/client.py
--rw-r--r--   0 root         (0) root         (0)  1354160 2023-08-08 01:38:35.000000 alibabacloud_cbn20170912-1.0.31/alibabacloud_cbn20170912/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-08 01:38:36.000000 alibabacloud_cbn20170912-1.0.31/alibabacloud_cbn20170912.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2350 2023-08-08 01:38:36.000000 alibabacloud_cbn20170912-1.0.31/alibabacloud_cbn20170912.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      420 2023-08-08 01:38:36.000000 alibabacloud_cbn20170912-1.0.31/alibabacloud_cbn20170912.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-08-08 01:38:36.000000 alibabacloud_cbn20170912-1.0.31/alibabacloud_cbn20170912.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      157 2023-08-08 01:38:36.000000 alibabacloud_cbn20170912-1.0.31/alibabacloud_cbn20170912.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       25 2023-08-08 01:38:36.000000 alibabacloud_cbn20170912-1.0.31/alibabacloud_cbn20170912.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       73 2023-08-08 01:38:36.000000 alibabacloud_cbn20170912-1.0.31/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2632 2023-08-08 01:38:35.000000 alibabacloud_cbn20170912-1.0.31/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-08 08:03:49.000000 alibabacloud_cbn20170912-1.0.32/
+-rw-r--r--   0 root         (0) root         (0)     5846 2023-08-08 08:03:49.000000 alibabacloud_cbn20170912-1.0.32/ChangeLog.md
+-rw-r--r--   0 root         (0) root         (0)      600 2023-08-08 08:03:49.000000 alibabacloud_cbn20170912-1.0.32/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       29 2023-08-08 08:03:49.000000 alibabacloud_cbn20170912-1.0.32/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2350 2023-08-08 08:03:49.000000 alibabacloud_cbn20170912-1.0.32/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1022 2023-08-08 08:03:49.000000 alibabacloud_cbn20170912-1.0.32/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)     1107 2023-08-08 08:03:49.000000 alibabacloud_cbn20170912-1.0.32/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-08 08:03:49.000000 alibabacloud_cbn20170912-1.0.32/alibabacloud_cbn20170912/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-08-08 08:03:49.000000 alibabacloud_cbn20170912-1.0.32/alibabacloud_cbn20170912/__init__.py
+-rw-r--r--   0 root         (0) root         (0)  1024624 2023-08-08 08:03:49.000000 alibabacloud_cbn20170912-1.0.32/alibabacloud_cbn20170912/client.py
+-rw-r--r--   0 root         (0) root         (0)  1354160 2023-08-08 08:03:49.000000 alibabacloud_cbn20170912-1.0.32/alibabacloud_cbn20170912/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-08 08:03:49.000000 alibabacloud_cbn20170912-1.0.32/alibabacloud_cbn20170912.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2350 2023-08-08 08:03:49.000000 alibabacloud_cbn20170912-1.0.32/alibabacloud_cbn20170912.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      420 2023-08-08 08:03:49.000000 alibabacloud_cbn20170912-1.0.32/alibabacloud_cbn20170912.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-08-08 08:03:49.000000 alibabacloud_cbn20170912-1.0.32/alibabacloud_cbn20170912.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      157 2023-08-08 08:03:49.000000 alibabacloud_cbn20170912-1.0.32/alibabacloud_cbn20170912.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       25 2023-08-08 08:03:49.000000 alibabacloud_cbn20170912-1.0.32/alibabacloud_cbn20170912.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2023-08-08 08:03:49.000000 alibabacloud_cbn20170912-1.0.32/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2632 2023-08-08 08:03:49.000000 alibabacloud_cbn20170912-1.0.32/setup.py
```

### Comparing `alibabacloud_cbn20170912-1.0.31/ChangeLog.md` & `alibabacloud_cbn20170912-1.0.32/ChangeLog.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+2023-08-08 Version: 1.0.31
+- Generated python 2017-09-12 for Cbn.
+
 2023-07-13 Version: 1.0.30
 - Update API ListTransitRouterRouteEntries to support PathAttributes.
 
 2023-05-23 Version: 1.0.29
 - Update API DescribeGrantRulesToCen support ChildInstanceOwnerId and ChildInstanceId.
 
 2023-04-27 Version: 1.0.28
```

### Comparing `alibabacloud_cbn20170912-1.0.31/LICENSE` & `alibabacloud_cbn20170912-1.0.32/LICENSE`

 * *Files identical despite different names*

### Comparing `alibabacloud_cbn20170912-1.0.31/PKG-INFO` & `alibabacloud_cbn20170912-1.0.32/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud_cbn20170912
-Version: 1.0.31
+Version: 1.0.32
 Summary: Alibaba Cloud Cloud Enterprise Network (20170912) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_cbn20170912-1.0.31/README-CN.md` & `alibabacloud_cbn20170912-1.0.32/README-CN.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_cbn20170912-1.0.31/README.md` & `alibabacloud_cbn20170912-1.0.32/README.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_cbn20170912-1.0.31/alibabacloud_cbn20170912/client.py` & `alibabacloud_cbn20170912-1.0.32/alibabacloud_cbn20170912/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_cbn20170912-1.0.31/alibabacloud_cbn20170912/models.py` & `alibabacloud_cbn20170912-1.0.32/alibabacloud_cbn20170912/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_cbn20170912-1.0.31/alibabacloud_cbn20170912.egg-info/PKG-INFO` & `alibabacloud_cbn20170912-1.0.32/alibabacloud_cbn20170912.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud-cbn20170912
-Version: 1.0.31
+Version: 1.0.32
 Summary: Alibaba Cloud Cloud Enterprise Network (20170912) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_cbn20170912-1.0.31/setup.py` & `alibabacloud_cbn20170912-1.0.32/setup.py`

 * *Files identical despite different names*


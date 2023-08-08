# Comparing `tmp/antchain_securitytech-1.1.12.tar.gz` & `tmp/antchain_securitytech-1.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/antchain_securitytech-1.1.12.tar", last modified: Tue Aug  8 02:50:45 2023, max compression
+gzip compressed data, was "dist/antchain_securitytech-1.1.4.tar", last modified: Wed May 24 02:53:36 2023, max compression
```

## Comparing `antchain_securitytech-1.1.12.tar` & `antchain_securitytech-1.1.4.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-08 02:50:45.000000 antchain_securitytech-1.1.12/
--rw-r--r--   0 root         (0) root         (0)      600 2023-08-08 02:50:45.000000 antchain_securitytech-1.1.12/LICENSE
--rw-r--r--   0 root         (0) root         (0)       29 2023-08-08 02:50:45.000000 antchain_securitytech-1.1.12/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2217 2023-08-08 02:50:45.000000 antchain_securitytech-1.1.12/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      831 2023-08-08 02:50:45.000000 antchain_securitytech-1.1.12/README-CN.md
--rw-r--r--   0 root         (0) root         (0)     1017 2023-08-08 02:50:45.000000 antchain_securitytech-1.1.12/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-08 02:50:45.000000 antchain_securitytech-1.1.12/antchain_sdk_securitytech/
--rw-r--r--   0 root         (0) root         (0)       22 2023-08-08 02:50:45.000000 antchain_securitytech-1.1.12/antchain_sdk_securitytech/__init__.py
--rw-r--r--   0 root         (0) root         (0)    47099 2023-08-08 02:50:45.000000 antchain_securitytech-1.1.12/antchain_sdk_securitytech/client.py
--rw-r--r--   0 root         (0) root         (0)    78323 2023-08-08 02:50:45.000000 antchain_securitytech-1.1.12/antchain_sdk_securitytech/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-08 02:50:45.000000 antchain_securitytech-1.1.12/antchain_securitytech.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2217 2023-08-08 02:50:45.000000 antchain_securitytech-1.1.12/antchain_securitytech.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      395 2023-08-08 02:50:45.000000 antchain_securitytech-1.1.12/antchain_securitytech.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-08-08 02:50:45.000000 antchain_securitytech-1.1.12/antchain_securitytech.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      108 2023-08-08 02:50:45.000000 antchain_securitytech-1.1.12/antchain_securitytech.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       26 2023-08-08 02:50:45.000000 antchain_securitytech-1.1.12/antchain_securitytech.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       73 2023-08-08 02:50:45.000000 antchain_securitytech-1.1.12/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2534 2023-08-08 02:50:45.000000 antchain_securitytech-1.1.12/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 02:53:36.000000 antchain_securitytech-1.1.4/
+-rw-r--r--   0 root         (0) root         (0)      600 2023-05-24 02:53:35.000000 antchain_securitytech-1.1.4/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       29 2023-05-24 02:53:35.000000 antchain_securitytech-1.1.4/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2216 2023-05-24 02:53:36.000000 antchain_securitytech-1.1.4/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      831 2023-05-24 02:53:35.000000 antchain_securitytech-1.1.4/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)     1017 2023-05-24 02:53:35.000000 antchain_securitytech-1.1.4/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 02:53:36.000000 antchain_securitytech-1.1.4/antchain_sdk_securitytech/
+-rw-r--r--   0 root         (0) root         (0)       21 2023-05-24 02:53:35.000000 antchain_securitytech-1.1.4/antchain_sdk_securitytech/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    26551 2023-05-24 02:53:35.000000 antchain_securitytech-1.1.4/antchain_sdk_securitytech/client.py
+-rw-r--r--   0 root         (0) root         (0)    44321 2023-05-24 02:53:35.000000 antchain_securitytech-1.1.4/antchain_sdk_securitytech/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 02:53:36.000000 antchain_securitytech-1.1.4/antchain_securitytech.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2216 2023-05-24 02:53:36.000000 antchain_securitytech-1.1.4/antchain_securitytech.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      395 2023-05-24 02:53:36.000000 antchain_securitytech-1.1.4/antchain_securitytech.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-24 02:53:36.000000 antchain_securitytech-1.1.4/antchain_securitytech.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      107 2023-05-24 02:53:36.000000 antchain_securitytech-1.1.4/antchain_securitytech.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       26 2023-05-24 02:53:36.000000 antchain_securitytech-1.1.4/antchain_securitytech.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2023-05-24 02:53:36.000000 antchain_securitytech-1.1.4/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2533 2023-05-24 02:53:35.000000 antchain_securitytech-1.1.4/setup.py
```

### Comparing `antchain_securitytech-1.1.12/LICENSE` & `antchain_securitytech-1.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `antchain_securitytech-1.1.12/PKG-INFO` & `antchain_securitytech-1.1.4/antchain_securitytech.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: antchain_securitytech
-Version: 1.1.12
+Name: antchain-securitytech
+Version: 1.1.4
 Summary: Ant Chain SECURITYTECH SDK Library for Python
 Home-page: https://github.com/alipay/antchain-openapi-prod-sdk
 Author: Ant Chain SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
```

### Comparing `antchain_securitytech-1.1.12/README-CN.md` & `antchain_securitytech-1.1.4/README-CN.md`

 * *Files identical despite different names*

### Comparing `antchain_securitytech-1.1.12/README.md` & `antchain_securitytech-1.1.4/README.md`

 * *Files identical despite different names*

### Comparing `antchain_securitytech-1.1.12/antchain_securitytech.egg-info/PKG-INFO` & `antchain_securitytech-1.1.4/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: antchain-securitytech
-Version: 1.1.12
+Name: antchain_securitytech
+Version: 1.1.4
 Summary: Ant Chain SECURITYTECH SDK Library for Python
 Home-page: https://github.com/alipay/antchain-openapi-prod-sdk
 Author: Ant Chain SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
```

### Comparing `antchain_securitytech-1.1.12/setup.py` & `antchain_securitytech-1.1.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,29 +20,29 @@
 
 import os
 from setuptools import setup, find_packages
 
 """
 setup module for antchain_securitytech.
 
-Created on 08/08/2023
+Created on 24/05/2023
 
 @author: Ant Chain SDK
 """
 
 PACKAGE = "antchain_sdk_securitytech"
 NAME = "antchain_securitytech" or "alibabacloud-package"
 DESCRIPTION = "Ant Chain SECURITYTECH SDK Library for Python"
 AUTHOR = "Ant Chain SDK"
 AUTHOR_EMAIL = "sdk-team@alibabacloud.com"
 URL = "https://github.com/alipay/antchain-openapi-prod-sdk"
 VERSION = __import__(PACKAGE).__version__
 REQUIRES = [
     "antchain_alipay_util>=1.0.1, <2.0.0",
-    "alibabacloud_tea_util>=0.3.11, <1.0.0",
+    "alibabacloud_tea_util>=0.3.8, <1.0.0",
     "alibabacloud_rpc_util>=0.0.4, <1.0.0"
 ]
 
 LONG_DESCRIPTION = ''
 if os.path.exists('./README.md'):
     with open("README.md", encoding='utf-8') as fp:
         LONG_DESCRIPTION = fp.read()
```


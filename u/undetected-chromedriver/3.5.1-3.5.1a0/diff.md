# Comparing `tmp/undetected-chromedriver-3.5.1.tar.gz` & `tmp/undetected-chromedriver-3.5.1a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "undetected-chromedriver-3.5.1.tar", last modified: Mon Aug  7 22:57:43 2023, max compression
+gzip compressed data, was "undetected-chromedriver-3.5.1a0.tar", last modified: Mon Aug  7 23:04:00 2023, max compression
```

## Comparing `undetected-chromedriver-3.5.1.tar` & `undetected-chromedriver-3.5.1a0.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0        0        0        0 2023-08-07 22:57:43.469900 undetected-chromedriver-3.5.1/
--rw-rw-rw-   0        0        0    35823 2023-08-07 18:26:15.000000 undetected-chromedriver-3.5.1/LICENSE
--rw-rw-rw-   0        0        0    78555 2023-08-07 22:57:43.469399 undetected-chromedriver-3.5.1/PKG-INFO
--rw-rw-rw-   0        0        0    77539 2023-08-07 18:26:15.000000 undetected-chromedriver-3.5.1/README.md
--rw-rw-rw-   0        0        0       42 2023-08-07 22:57:43.469900 undetected-chromedriver-3.5.1/setup.cfg
--rw-rw-rw-   0        0        0     2670 2023-08-07 18:26:15.000000 undetected-chromedriver-3.5.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-08-07 22:57:43.443115 undetected-chromedriver-3.5.1/undetected_chromedriver/
--rw-rw-rw-   0        0        0    35365 2023-08-07 22:57:23.000000 undetected-chromedriver-3.5.1/undetected_chromedriver/__init__.py
--rw-rw-rw-   0        0        0     3498 2023-08-07 18:26:15.000000 undetected-chromedriver-3.5.1/undetected_chromedriver/cdp.py
--rw-rw-rw-   0        0        0     5937 2023-08-07 18:26:15.000000 undetected-chromedriver-3.5.1/undetected_chromedriver/devtool.py
--rw-rw-rw-   0        0        0     1837 2023-08-07 18:26:15.000000 undetected-chromedriver-3.5.1/undetected_chromedriver/dprocess.py
--rw-rw-rw-   0        0        0     2751 2023-08-07 18:26:15.000000 undetected-chromedriver-3.5.1/undetected_chromedriver/options.py
--rw-rw-rw-   0        0        0    11938 2023-08-07 22:57:23.000000 undetected-chromedriver-3.5.1/undetected_chromedriver/patcher.py
--rw-rw-rw-   0        0        0     3065 2023-08-07 18:26:15.000000 undetected-chromedriver-3.5.1/undetected_chromedriver/reactor.py
--rw-rw-rw-   0        0        0     2900 2023-08-07 18:26:15.000000 undetected-chromedriver-3.5.1/undetected_chromedriver/webelement.py
-drwxrwxrwx   0        0        0        0 2023-08-07 22:57:43.468398 undetected-chromedriver-3.5.1/undetected_chromedriver.egg-info/
--rw-rw-rw-   0        0        0    78555 2023-08-07 22:57:42.000000 undetected-chromedriver-3.5.1/undetected_chromedriver.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      541 2023-08-07 22:57:43.000000 undetected-chromedriver-3.5.1/undetected_chromedriver.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-07 22:57:42.000000 undetected-chromedriver-3.5.1/undetected_chromedriver.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       36 2023-08-07 22:57:43.000000 undetected-chromedriver-3.5.1/undetected_chromedriver.egg-info/requires.txt
--rw-rw-rw-   0        0        0       24 2023-08-07 22:57:43.000000 undetected-chromedriver-3.5.1/undetected_chromedriver.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-08-07 23:04:00.657165 undetected-chromedriver-3.5.1a0/
+-rw-rw-rw-   0        0        0    35823 2023-08-07 18:26:15.000000 undetected-chromedriver-3.5.1a0/LICENSE
+-rw-rw-rw-   0        0        0    78557 2023-08-07 23:04:00.656665 undetected-chromedriver-3.5.1a0/PKG-INFO
+-rw-rw-rw-   0        0        0    77539 2023-08-07 18:26:15.000000 undetected-chromedriver-3.5.1a0/README.md
+-rw-rw-rw-   0        0        0       42 2023-08-07 23:04:00.657165 undetected-chromedriver-3.5.1a0/setup.cfg
+-rw-rw-rw-   0        0        0     2670 2023-08-07 18:26:15.000000 undetected-chromedriver-3.5.1a0/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-07 23:04:00.641166 undetected-chromedriver-3.5.1a0/undetected_chromedriver/
+-rw-rw-rw-   0        0        0    35366 2023-08-07 23:03:41.000000 undetected-chromedriver-3.5.1a0/undetected_chromedriver/__init__.py
+-rw-rw-rw-   0        0        0     3498 2023-08-07 18:26:15.000000 undetected-chromedriver-3.5.1a0/undetected_chromedriver/cdp.py
+-rw-rw-rw-   0        0        0     5937 2023-08-07 18:26:15.000000 undetected-chromedriver-3.5.1a0/undetected_chromedriver/devtool.py
+-rw-rw-rw-   0        0        0     1837 2023-08-07 18:26:15.000000 undetected-chromedriver-3.5.1a0/undetected_chromedriver/dprocess.py
+-rw-rw-rw-   0        0        0     2751 2023-08-07 18:26:15.000000 undetected-chromedriver-3.5.1a0/undetected_chromedriver/options.py
+-rw-rw-rw-   0        0        0    11939 2023-08-07 23:03:41.000000 undetected-chromedriver-3.5.1a0/undetected_chromedriver/patcher.py
+-rw-rw-rw-   0        0        0     3065 2023-08-07 18:26:15.000000 undetected-chromedriver-3.5.1a0/undetected_chromedriver/reactor.py
+-rw-rw-rw-   0        0        0     2900 2023-08-07 18:26:15.000000 undetected-chromedriver-3.5.1a0/undetected_chromedriver/webelement.py
+drwxrwxrwx   0        0        0        0 2023-08-07 23:04:00.655666 undetected-chromedriver-3.5.1a0/undetected_chromedriver.egg-info/
+-rw-rw-rw-   0        0        0    78557 2023-08-07 23:04:00.000000 undetected-chromedriver-3.5.1a0/undetected_chromedriver.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      541 2023-08-07 23:04:00.000000 undetected-chromedriver-3.5.1a0/undetected_chromedriver.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-07 23:04:00.000000 undetected-chromedriver-3.5.1a0/undetected_chromedriver.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       36 2023-08-07 23:04:00.000000 undetected-chromedriver-3.5.1a0/undetected_chromedriver.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       24 2023-08-07 23:04:00.000000 undetected-chromedriver-3.5.1a0/undetected_chromedriver.egg-info/top_level.txt
```

### Comparing `undetected-chromedriver-3.5.1/LICENSE` & `undetected-chromedriver-3.5.1a0/LICENSE`

 * *Files identical despite different names*

### Comparing `undetected-chromedriver-3.5.1/PKG-INFO` & `undetected-chromedriver-3.5.1a0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: undetected-chromedriver
-Version: 3.5.1
+Version: 3.5.1a0
 Summary: ('Selenium.webdriver.Chrome replacement with compatiblity for Brave, and other Chromium based browsers.', 'Not triggered by CloudFlare/Imperva/hCaptcha and such.', 'NOTE: results may vary due to many factors. No guarantees are given, except for ongoing efforts in understanding detection algorithms.')
 Home-page: https://github.com/ultrafunkamsterdam/undetected-chromedriver
 Author: UltrafunkAmsterdam
 Author-email: info@blackhat-security.nl
 License: GPL-3.0
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `undetected-chromedriver-3.5.1/README.md` & `undetected-chromedriver-3.5.1a0/README.md`

 * *Files identical despite different names*

### Comparing `undetected-chromedriver-3.5.1/setup.py` & `undetected-chromedriver-3.5.1a0/setup.py`

 * *Files identical despite different names*

### Comparing `undetected-chromedriver-3.5.1/undetected_chromedriver/__init__.py` & `undetected-chromedriver-3.5.1a0/undetected_chromedriver/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 by UltrafunkAmsterdam (https://github.com/ultrafunkamsterdam)
 
 """
 from __future__ import annotations
 
 
-__version__ = "3.5.1"
+__version__ = "3.5.1a"
 
 import json
 import logging
 import os
 import re
 import shutil
 import subprocess
```

### Comparing `undetected-chromedriver-3.5.1/undetected_chromedriver/cdp.py` & `undetected-chromedriver-3.5.1a0/undetected_chromedriver/cdp.py`

 * *Files identical despite different names*

### Comparing `undetected-chromedriver-3.5.1/undetected_chromedriver/devtool.py` & `undetected-chromedriver-3.5.1a0/undetected_chromedriver/devtool.py`

 * *Files identical despite different names*

### Comparing `undetected-chromedriver-3.5.1/undetected_chromedriver/dprocess.py` & `undetected-chromedriver-3.5.1a0/undetected_chromedriver/dprocess.py`

 * *Files identical despite different names*

### Comparing `undetected-chromedriver-3.5.1/undetected_chromedriver/options.py` & `undetected-chromedriver-3.5.1a0/undetected_chromedriver/options.py`

 * *Files identical despite different names*

### Comparing `undetected-chromedriver-3.5.1/undetected_chromedriver/patcher.py` & `undetected-chromedriver-3.5.1a0/undetected_chromedriver/patcher.py`

 * *Files 0% similar despite different names*

```diff
@@ -112,15 +112,15 @@
 
         """
         # if self.user_multi_procs and \
         #         self.user_multi_procs != -1:
         #     # -1 being a skip value used later in this block
         #
         p = pathlib.Path(self.data_path)
-        if self.user_multiprocs:
+        if self.user_multi_procs:
             with Lock():
                 files = list(p.rglob("*chromedriver*?"))
                 for file in files:
                     if self.is_binary_patched(file):
                         self.executable_path = str(file)
                         return True
```

### Comparing `undetected-chromedriver-3.5.1/undetected_chromedriver/reactor.py` & `undetected-chromedriver-3.5.1a0/undetected_chromedriver/reactor.py`

 * *Files identical despite different names*

### Comparing `undetected-chromedriver-3.5.1/undetected_chromedriver/webelement.py` & `undetected-chromedriver-3.5.1a0/undetected_chromedriver/webelement.py`

 * *Files identical despite different names*

### Comparing `undetected-chromedriver-3.5.1/undetected_chromedriver.egg-info/PKG-INFO` & `undetected-chromedriver-3.5.1a0/undetected_chromedriver.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: undetected-chromedriver
-Version: 3.5.1
+Version: 3.5.1a0
 Summary: ('Selenium.webdriver.Chrome replacement with compatiblity for Brave, and other Chromium based browsers.', 'Not triggered by CloudFlare/Imperva/hCaptcha and such.', 'NOTE: results may vary due to many factors. No guarantees are given, except for ongoing efforts in understanding detection algorithms.')
 Home-page: https://github.com/ultrafunkamsterdam/undetected-chromedriver
 Author: UltrafunkAmsterdam
 Author-email: info@blackhat-security.nl
 License: GPL-3.0
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `undetected-chromedriver-3.5.1/undetected_chromedriver.egg-info/SOURCES.txt` & `undetected-chromedriver-3.5.1a0/undetected_chromedriver.egg-info/SOURCES.txt`

 * *Files identical despite different names*


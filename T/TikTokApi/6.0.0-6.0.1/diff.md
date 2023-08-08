# Comparing `tmp/TikTokApi-6.0.0.tar.gz` & `tmp/TikTokApi-6.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "TikTokApi-6.0.0.tar", last modified: Tue Aug  8 06:51:53 2023, max compression
+gzip compressed data, was "TikTokApi-6.0.1.tar", last modified: Tue Aug  8 15:55:42 2023, max compression
```

## Comparing `TikTokApi-6.0.0.tar` & `TikTokApi-6.0.1.tar`

### file list

```diff
@@ -1,40 +1,60 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 06:51:53.956604 TikTokApi-6.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-08-08 06:51:41.000000 TikTokApi-6.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-08-08 06:51:41.000000 TikTokApi-6.0.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     8895 2023-08-08 06:51:53.956604 TikTokApi-6.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8083 2023-08-08 06:51:41.000000 TikTokApi-6.0.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 06:51:53.948604 TikTokApi-6.0.0/TikTokApi/
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-08-08 06:51:41.000000 TikTokApi-6.0.0/TikTokApi/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 06:51:53.952604 TikTokApi-6.0.0/TikTokApi/api/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 06:51:41.000000 TikTokApi-6.0.0/TikTokApi/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1511 2023-08-08 06:51:41.000000 TikTokApi-6.0.0/TikTokApi/api/comment.py
--rw-r--r--   0 runner    (1001) docker     (123)     4893 2023-08-08 06:51:41.000000 TikTokApi-6.0.0/TikTokApi/api/hashtag.py
--rw-r--r--   0 runner    (1001) docker     (123)     3769 2023-08-08 06:51:41.000000 TikTokApi-6.0.0/TikTokApi/api/search.py
--rw-r--r--   0 runner    (1001) docker     (123)     5789 2023-08-08 06:51:41.000000 TikTokApi-6.0.0/TikTokApi/api/sound.py
--rw-r--r--   0 runner    (1001) docker     (123)     1715 2023-08-08 06:51:41.000000 TikTokApi-6.0.0/TikTokApi/api/trending.py
--rw-r--r--   0 runner    (1001) docker     (123)     5636 2023-08-08 06:51:41.000000 TikTokApi-6.0.0/TikTokApi/api/user.py
--rw-r--r--   0 runner    (1001) docker     (123)     9522 2023-08-08 06:51:41.000000 TikTokApi-6.0.0/TikTokApi/api/video.py
--rw-r--r--   0 runner    (1001) docker     (123)      980 2023-08-08 06:51:41.000000 TikTokApi-6.0.0/TikTokApi/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)      726 2023-08-08 06:51:41.000000 TikTokApi-6.0.0/TikTokApi/helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 06:51:53.952604 TikTokApi-6.0.0/TikTokApi/stealth/
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-08-08 06:51:41.000000 TikTokApi-6.0.0/TikTokApi/stealth/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5297 2023-08-08 06:51:41.000000 TikTokApi-6.0.0/TikTokApi/stealth/stealth.py
--rw-r--r--   0 runner    (1001) docker     (123)    16194 2023-08-08 06:51:41.000000 TikTokApi-6.0.0/TikTokApi/tiktok.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 06:51:53.948604 TikTokApi-6.0.0/TikTokApi.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8895 2023-08-08 06:51:53.000000 TikTokApi-6.0.0/TikTokApi.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      744 2023-08-08 06:51:53.000000 TikTokApi-6.0.0/TikTokApi.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 06:51:53.000000 TikTokApi-6.0.0/TikTokApi.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-08-08 06:51:53.000000 TikTokApi-6.0.0/TikTokApi.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-08-08 06:51:53.000000 TikTokApi-6.0.0/TikTokApi.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-08-08 06:51:53.956604 TikTokApi-6.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1142 2023-08-08 06:51:41.000000 TikTokApi-6.0.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 06:51:53.956604 TikTokApi-6.0.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 06:51:41.000000 TikTokApi-6.0.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      480 2023-08-08 06:51:41.000000 TikTokApi-6.0.0/tests/test_comments.py
--rw-r--r--   0 runner    (1001) docker     (123)     1608 2023-08-08 06:51:41.000000 TikTokApi-6.0.0/tests/test_hashtag.py
--rw-r--r--   0 runner    (1001) docker     (123)      931 2023-08-08 06:51:41.000000 TikTokApi-6.0.0/tests/test_integration.py
--rw-r--r--   0 runner    (1001) docker     (123)      411 2023-08-08 06:51:41.000000 TikTokApi-6.0.0/tests/test_search.py
--rw-r--r--   0 runner    (1001) docker     (123)      869 2023-08-08 06:51:41.000000 TikTokApi-6.0.0/tests/test_sound.py
--rw-r--r--   0 runner    (1001) docker     (123)      410 2023-08-08 06:51:41.000000 TikTokApi-6.0.0/tests/test_trending.py
--rw-r--r--   0 runner    (1001) docker     (123)     1381 2023-08-08 06:51:41.000000 TikTokApi-6.0.0/tests/test_user.py
--rw-r--r--   0 runner    (1001) docker     (123)     1914 2023-08-08 06:51:41.000000 TikTokApi-6.0.0/tests/test_video.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 15:55:42.047891 TikTokApi-6.0.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-08-08 15:55:27.000000 TikTokApi-6.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-08-08 15:55:27.000000 TikTokApi-6.0.1/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     8895 2023-08-08 15:55:42.047891 TikTokApi-6.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8083 2023-08-08 15:55:27.000000 TikTokApi-6.0.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 15:55:42.039892 TikTokApi-6.0.1/TikTokApi/
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-08-08 15:55:27.000000 TikTokApi-6.0.1/TikTokApi/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 15:55:42.039892 TikTokApi-6.0.1/TikTokApi/api/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 15:55:27.000000 TikTokApi-6.0.1/TikTokApi/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1511 2023-08-08 15:55:27.000000 TikTokApi-6.0.1/TikTokApi/api/comment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4893 2023-08-08 15:55:27.000000 TikTokApi-6.0.1/TikTokApi/api/hashtag.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3769 2023-08-08 15:55:27.000000 TikTokApi-6.0.1/TikTokApi/api/search.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5789 2023-08-08 15:55:27.000000 TikTokApi-6.0.1/TikTokApi/api/sound.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1715 2023-08-08 15:55:27.000000 TikTokApi-6.0.1/TikTokApi/api/trending.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5636 2023-08-08 15:55:27.000000 TikTokApi-6.0.1/TikTokApi/api/user.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9522 2023-08-08 15:55:27.000000 TikTokApi-6.0.1/TikTokApi/api/video.py
+-rw-r--r--   0 runner    (1001) docker     (123)      980 2023-08-08 15:55:27.000000 TikTokApi-6.0.1/TikTokApi/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      726 2023-08-08 15:55:27.000000 TikTokApi-6.0.1/TikTokApi/helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 15:55:42.039892 TikTokApi-6.0.1/TikTokApi/stealth/
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-08-08 15:55:27.000000 TikTokApi-6.0.1/TikTokApi/stealth/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 15:55:42.043892 TikTokApi-6.0.1/TikTokApi/stealth/js/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 15:55:27.000000 TikTokApi-6.0.1/TikTokApi/stealth/js/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2042 2023-08-08 15:55:27.000000 TikTokApi-6.0.1/TikTokApi/stealth/js/chrome_app.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1008 2023-08-08 15:55:27.000000 TikTokApi-6.0.1/TikTokApi/stealth/js/chrome_csi.py
+-rw-r--r--   0 runner    (1001) docker     (123)      496 2023-08-08 15:55:27.000000 TikTokApi-6.0.1/TikTokApi/stealth/js/chrome_hairline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4429 2023-08-08 15:55:27.000000 TikTokApi-6.0.1/TikTokApi/stealth/js/chrome_load_times.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9607 2023-08-08 15:55:27.000000 TikTokApi-6.0.1/TikTokApi/stealth/js/chrome_runtime.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5924 2023-08-08 15:55:27.000000 TikTokApi-6.0.1/TikTokApi/stealth/js/generate_magic_arrays.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3512 2023-08-08 15:55:27.000000 TikTokApi-6.0.1/TikTokApi/stealth/js/iframe_contentWindow.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1710 2023-08-08 15:55:27.000000 TikTokApi-6.0.1/TikTokApi/stealth/js/media_codecs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      287 2023-08-08 15:55:27.000000 TikTokApi-6.0.1/TikTokApi/stealth/js/navigator_hardwareConcurrency.py
+-rw-r--r--   0 runner    (1001) docker     (123)      153 2023-08-08 15:55:27.000000 TikTokApi-6.0.1/TikTokApi/stealth/js/navigator_languages.py
+-rw-r--r--   0 runner    (1001) docker     (123)      575 2023-08-08 15:55:27.000000 TikTokApi-6.0.1/TikTokApi/stealth/js/navigator_permissions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      186 2023-08-08 15:55:27.000000 TikTokApi-6.0.1/TikTokApi/stealth/js/navigator_platform.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2886 2023-08-08 15:55:27.000000 TikTokApi-6.0.1/TikTokApi/stealth/js/navigator_plugins.py
+-rw-r--r--   0 runner    (1001) docker     (123)      288 2023-08-08 15:55:27.000000 TikTokApi-6.0.1/TikTokApi/stealth/js/navigator_userAgent.py
+-rw-r--r--   0 runner    (1001) docker     (123)      153 2023-08-08 15:55:27.000000 TikTokApi-6.0.1/TikTokApi/stealth/js/navigator_vendor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17590 2023-08-08 15:55:27.000000 TikTokApi-6.0.1/TikTokApi/stealth/js/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1173 2023-08-08 15:55:27.000000 TikTokApi-6.0.1/TikTokApi/stealth/js/webgl_vendor.py
+-rw-r--r--   0 runner    (1001) docker     (123)      445 2023-08-08 15:55:27.000000 TikTokApi-6.0.1/TikTokApi/stealth/js/window_outerdimensions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5767 2023-08-08 15:55:27.000000 TikTokApi-6.0.1/TikTokApi/stealth/stealth.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16194 2023-08-08 15:55:27.000000 TikTokApi-6.0.1/TikTokApi/tiktok.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 15:55:42.039892 TikTokApi-6.0.1/TikTokApi.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8895 2023-08-08 15:55:41.000000 TikTokApi-6.0.1/TikTokApi.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1524 2023-08-08 15:55:42.000000 TikTokApi-6.0.1/TikTokApi.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 15:55:41.000000 TikTokApi-6.0.1/TikTokApi.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-08-08 15:55:41.000000 TikTokApi-6.0.1/TikTokApi.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-08-08 15:55:41.000000 TikTokApi-6.0.1/TikTokApi.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-08-08 15:55:42.047891 TikTokApi-6.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1142 2023-08-08 15:55:27.000000 TikTokApi-6.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 15:55:42.047891 TikTokApi-6.0.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 15:55:27.000000 TikTokApi-6.0.1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      480 2023-08-08 15:55:27.000000 TikTokApi-6.0.1/tests/test_comments.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1608 2023-08-08 15:55:27.000000 TikTokApi-6.0.1/tests/test_hashtag.py
+-rw-r--r--   0 runner    (1001) docker     (123)      931 2023-08-08 15:55:27.000000 TikTokApi-6.0.1/tests/test_integration.py
+-rw-r--r--   0 runner    (1001) docker     (123)      411 2023-08-08 15:55:27.000000 TikTokApi-6.0.1/tests/test_search.py
+-rw-r--r--   0 runner    (1001) docker     (123)      869 2023-08-08 15:55:27.000000 TikTokApi-6.0.1/tests/test_sound.py
+-rw-r--r--   0 runner    (1001) docker     (123)      410 2023-08-08 15:55:27.000000 TikTokApi-6.0.1/tests/test_trending.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1381 2023-08-08 15:55:27.000000 TikTokApi-6.0.1/tests/test_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1914 2023-08-08 15:55:27.000000 TikTokApi-6.0.1/tests/test_video.py
```

### Comparing `TikTokApi-6.0.0/LICENSE` & `TikTokApi-6.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `TikTokApi-6.0.0/LICENSE.txt` & `TikTokApi-6.0.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `TikTokApi-6.0.0/PKG-INFO` & `TikTokApi-6.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: TikTokApi
-Version: 6.0.0
+Version: 6.0.1
 Summary: The Unofficial TikTok API Wrapper in Python 3.
 Home-page: https://github.com/davidteather/tiktok-api
 Download-URL: https://github.com/davidteather/TikTok-Api/tarball/main
 Author: David Teather
 Author-email: contact.davidteather@gmail.com
 License: MIT
 Keywords: tiktok,python3,api,unofficial,tiktok-api,tiktok api
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: TikTokApi Version: 6.0.0 Summary: The Unofficial
+Metadata-Version: 2.1 Name: TikTokApi Version: 6.0.1 Summary: The Unofficial
 TikTok API Wrapper in Python 3. Home-page: https://github.com/davidteather/
 tiktok-api Download-URL: https://github.com/davidteather/TikTok-Api/tarball/
 main Author: David Teather Author-email: contact.davidteather@gmail.com
 License: MIT Keywords: tiktok,python3,api,unofficial,tiktok-api,tiktok api
 Classifier: Development Status :: 3 - Alpha Classifier: Intended Audience ::
 Developers Classifier: Topic :: Software Development :: Build Tools Classifier:
 License :: OSI Approved :: MIT License Classifier: Programming Language ::
```

### Comparing `TikTokApi-6.0.0/README.md` & `TikTokApi-6.0.1/README.md`

 * *Files identical despite different names*

### Comparing `TikTokApi-6.0.0/TikTokApi/api/comment.py` & `TikTokApi-6.0.1/TikTokApi/api/comment.py`

 * *Files identical despite different names*

### Comparing `TikTokApi-6.0.0/TikTokApi/api/hashtag.py` & `TikTokApi-6.0.1/TikTokApi/api/hashtag.py`

 * *Files identical despite different names*

### Comparing `TikTokApi-6.0.0/TikTokApi/api/search.py` & `TikTokApi-6.0.1/TikTokApi/api/search.py`

 * *Files identical despite different names*

### Comparing `TikTokApi-6.0.0/TikTokApi/api/sound.py` & `TikTokApi-6.0.1/TikTokApi/api/sound.py`

 * *Files identical despite different names*

### Comparing `TikTokApi-6.0.0/TikTokApi/api/trending.py` & `TikTokApi-6.0.1/TikTokApi/api/trending.py`

 * *Files identical despite different names*

### Comparing `TikTokApi-6.0.0/TikTokApi/api/user.py` & `TikTokApi-6.0.1/TikTokApi/api/user.py`

 * *Files identical despite different names*

### Comparing `TikTokApi-6.0.0/TikTokApi/api/video.py` & `TikTokApi-6.0.1/TikTokApi/api/video.py`

 * *Files identical despite different names*

### Comparing `TikTokApi-6.0.0/TikTokApi/exceptions.py` & `TikTokApi-6.0.1/TikTokApi/exceptions.py`

 * *Files identical despite different names*

### Comparing `TikTokApi-6.0.0/TikTokApi/helpers.py` & `TikTokApi-6.0.1/TikTokApi/helpers.py`

 * *Files identical despite different names*

### Comparing `TikTokApi-6.0.0/TikTokApi/stealth/stealth.py` & `TikTokApi-6.0.1/TikTokApi/stealth/stealth.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,41 +1,53 @@
 # -*- coding: utf-8 -*-
 import json
 from dataclasses import dataclass
 from typing import Tuple, Optional, Dict
 
-import pkg_resources
 from playwright.async_api import Page as AsyncPage
 
-
-def from_file(name):
-    """Read script from ./js directory"""
-    return pkg_resources.resource_string(__name__, f"js/{name}").decode()
-
+from .js.chrome_app import chrome_app
+from .js.chrome_csi import chrome_csi
+from .js.chrome_hairline import chrome_hairline
+from .js.chrome_load_times import chrome_load_times
+from .js.chrome_runtime import chrome_runtime
+from .js.generate_magic_arrays import generate_magic_arrays
+from .js.iframe_contentWindow import iframe_contentWindow
+from .js.media_codecs import media_codecs
+from .js.navigator_hardwareConcurrency import navigator_hardwareConcurrency
+from .js.navigator_languages import navigator_languages
+from .js.navigator_permissions import navigator_permissions
+from .js.navigator_platform import navigator_platform
+from .js.navigator_plugins import navigator_plugins
+from .js.navigator_userAgent import navigator_userAgent
+from .js.navigator_vendor import navigator_vendor
+from .js.webgl_vendor import webgl_vendor
+from .js.window_outerdimensions import window_outerdimensions
+from .js.utils import utils
 
 SCRIPTS: Dict[str, str] = {
-    "chrome_csi": from_file("chrome.csi.js"),
-    "chrome_app": from_file("chrome.app.js"),
-    "chrome_runtime": from_file("chrome.runtime.js"),
-    "chrome_load_times": from_file("chrome.load.times.js"),
-    "chrome_hairline": from_file("chrome.hairline.js"),
-    "generate_magic_arrays": from_file("generate.magic.arrays.js"),
-    "iframe_content_window": from_file("iframe.contentWindow.js"),
-    "media_codecs": from_file("media.codecs.js"),
-    "navigator_vendor": from_file("navigator.vendor.js"),
-    "navigator_plugins": from_file("navigator.plugins.js"),
-    "navigator_permissions": from_file("navigator.permissions.js"),
-    "navigator_languages": from_file("navigator.languages.js"),
-    "navigator_platform": from_file("navigator.platform.js"),
-    "navigator_user_agent": from_file("navigator.userAgent.js"),
-    "navigator_hardware_concurrency": from_file("navigator.hardwareConcurrency.js"),
-    "outerdimensions": from_file("window.outerdimensions.js"),
-    "utils": from_file("utils.js"),
+    "chrome_csi": chrome_csi,
+    "chrome_app": chrome_app,
+    "chrome_runtime": chrome_runtime,
+    "chrome_load_times": chrome_load_times,
+    "chrome_hairline": chrome_hairline,
+    "generate_magic_arrays": generate_magic_arrays,
+    "iframe_content_window": iframe_contentWindow,
+    "media_codecs": media_codecs,
+    "navigator_vendor": navigator_vendor,
+    "navigator_plugins": navigator_plugins,
+    "navigator_permissions": navigator_permissions,
+    "navigator_languages": navigator_languages,
+    "navigator_platform": navigator_platform,
+    "navigator_user_agent": navigator_userAgent,
+    "navigator_hardware_concurrency": navigator_hardwareConcurrency,
+    "outerdimensions": window_outerdimensions,
+    "utils": utils,
     "webdriver": "delete Object.getPrototypeOf(navigator).webdriver",
-    "webgl_vendor": from_file("webgl.vendor.js"),
+    "webgl_vendor": webgl_vendor,
 }
 
 
 @dataclass
 class StealthConfig:
     """
     Playwright stealth configuration that applies stealth strategies to playwright page objects.
```

### Comparing `TikTokApi-6.0.0/TikTokApi/tiktok.py` & `TikTokApi-6.0.1/TikTokApi/tiktok.py`

 * *Files identical despite different names*

### Comparing `TikTokApi-6.0.0/TikTokApi.egg-info/PKG-INFO` & `TikTokApi-6.0.1/TikTokApi.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: TikTokApi
-Version: 6.0.0
+Version: 6.0.1
 Summary: The Unofficial TikTok API Wrapper in Python 3.
 Home-page: https://github.com/davidteather/tiktok-api
 Download-URL: https://github.com/davidteather/TikTok-Api/tarball/main
 Author: David Teather
 Author-email: contact.davidteather@gmail.com
 License: MIT
 Keywords: tiktok,python3,api,unofficial,tiktok-api,tiktok api
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: TikTokApi Version: 6.0.0 Summary: The Unofficial
+Metadata-Version: 2.1 Name: TikTokApi Version: 6.0.1 Summary: The Unofficial
 TikTok API Wrapper in Python 3. Home-page: https://github.com/davidteather/
 tiktok-api Download-URL: https://github.com/davidteather/TikTok-Api/tarball/
 main Author: David Teather Author-email: contact.davidteather@gmail.com
 License: MIT Keywords: tiktok,python3,api,unofficial,tiktok-api,tiktok api
 Classifier: Development Status :: 3 - Alpha Classifier: Intended Audience ::
 Developers Classifier: Topic :: Software Development :: Build Tools Classifier:
 License :: OSI Approved :: MIT License Classifier: Programming Language ::
```

### Comparing `TikTokApi-6.0.0/setup.py` & `TikTokApi-6.0.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="TikTokApi",
     packages=setuptools.find_packages(),
-    version="6.0.0",
+    version="6.0.1",
     license="MIT",
     description="The Unofficial TikTok API Wrapper in Python 3.",
     author="David Teather",
     author_email="contact.davidteather@gmail.com",
     url="https://github.com/davidteather/tiktok-api",
     long_description=long_description,
     long_description_content_type="text/markdown",
```

### Comparing `TikTokApi-6.0.0/tests/test_hashtag.py` & `TikTokApi-6.0.1/tests/test_hashtag.py`

 * *Files identical despite different names*

### Comparing `TikTokApi-6.0.0/tests/test_integration.py` & `TikTokApi-6.0.1/tests/test_integration.py`

 * *Files identical despite different names*

### Comparing `TikTokApi-6.0.0/tests/test_sound.py` & `TikTokApi-6.0.1/tests/test_sound.py`

 * *Files identical despite different names*

### Comparing `TikTokApi-6.0.0/tests/test_user.py` & `TikTokApi-6.0.1/tests/test_user.py`

 * *Files identical despite different names*

### Comparing `TikTokApi-6.0.0/tests/test_video.py` & `TikTokApi-6.0.1/tests/test_video.py`

 * *Files identical despite different names*


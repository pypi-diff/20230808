# Comparing `tmp/pygifconvt_daun-1.0.1.tar.gz` & `tmp/pygifconvt_daun-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pygifconvt_daun-1.0.1.tar", last modified: Fri Jul 28 00:27:00 2023, max compression
+gzip compressed data, was "pygifconvt_daun-1.0.2.tar", last modified: Tue Aug  8 05:07:49 2023, max compression
```

## Comparing `pygifconvt_daun-1.0.1.tar` & `pygifconvt_daun-1.0.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-07-28 00:27:00.658864 pygifconvt_daun-1.0.1/
--rw-rw-rw-   0        0        0     1167 2023-07-27 07:55:58.000000 pygifconvt_daun-1.0.1/LICENSE
--rw-rw-rw-   0        0        0       58 2020-12-14 06:55:04.000000 pygifconvt_daun-1.0.1/MANIFEST.in
--rw-rw-rw-   0        0        0      410 2023-07-28 00:27:00.658864 pygifconvt_daun-1.0.1/PKG-INFO
--rw-rw-rw-   0        0        0      614 2020-11-26 04:54:04.000000 pygifconvt_daun-1.0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-07-28 00:27:00.638931 pygifconvt_daun-1.0.1/pygifconvt_daun/
--rw-rw-rw-   0        0        0        0 2023-07-27 07:52:34.000000 pygifconvt_daun-1.0.1/pygifconvt_daun/__init__.py
--rw-rw-rw-   0        0        0     1196 2023-07-28 00:19:50.000000 pygifconvt_daun-1.0.1/pygifconvt_daun/converter.py
-drwxrwxrwx   0        0        0        0 2023-07-28 00:27:00.657875 pygifconvt_daun-1.0.1/pygifconvt_daun.egg-info/
--rw-rw-rw-   0        0        0      410 2023-07-28 00:27:00.000000 pygifconvt_daun-1.0.1/pygifconvt_daun.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      354 2023-07-28 00:27:00.000000 pygifconvt_daun-1.0.1/pygifconvt_daun.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-28 00:27:00.000000 pygifconvt_daun-1.0.1/pygifconvt_daun.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-07-28 00:27:00.000000 pygifconvt_daun-1.0.1/pygifconvt_daun.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0        7 2023-07-28 00:27:00.000000 pygifconvt_daun-1.0.1/pygifconvt_daun.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2023-07-28 00:27:00.000000 pygifconvt_daun-1.0.1/pygifconvt_daun.egg-info/top_level.txt
--rw-rw-rw-   0        0        0        0 2020-12-14 06:33:38.000000 pygifconvt_daun-1.0.1/requirements.txt
--rw-rw-rw-   0        0        0       86 2023-07-28 00:27:00.661862 pygifconvt_daun-1.0.1/setup.cfg
--rw-rw-rw-   0        0        0      684 2023-07-28 00:20:39.000000 pygifconvt_daun-1.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-08 05:07:49.418130 pygifconvt_daun-1.0.2/
+-rw-rw-rw-   0        0        0     1167 2023-07-27 07:55:58.000000 pygifconvt_daun-1.0.2/LICENSE
+-rw-rw-rw-   0        0        0       58 2020-12-14 06:55:04.000000 pygifconvt_daun-1.0.2/MANIFEST.in
+-rw-rw-rw-   0        0        0      410 2023-08-08 05:07:49.418130 pygifconvt_daun-1.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0      614 2020-11-26 04:54:04.000000 pygifconvt_daun-1.0.2/README.md
+drwxrwxrwx   0        0        0        0 2023-08-08 05:07:49.378130 pygifconvt_daun-1.0.2/pygifconvt_daun/
+-rw-rw-rw-   0        0        0        0 2023-07-27 07:52:34.000000 pygifconvt_daun-1.0.2/pygifconvt_daun/__init__.py
+-rw-rw-rw-   0        0        0     1196 2023-07-28 00:19:50.000000 pygifconvt_daun-1.0.2/pygifconvt_daun/converter.py
+drwxrwxrwx   0        0        0        0 2023-08-08 05:07:49.415135 pygifconvt_daun-1.0.2/pygifconvt_daun.egg-info/
+-rw-rw-rw-   0        0        0      410 2023-08-08 05:07:49.000000 pygifconvt_daun-1.0.2/pygifconvt_daun.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      354 2023-08-08 05:07:49.000000 pygifconvt_daun-1.0.2/pygifconvt_daun.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-08 05:07:49.000000 pygifconvt_daun-1.0.2/pygifconvt_daun.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-07-28 00:27:00.000000 pygifconvt_daun-1.0.2/pygifconvt_daun.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0        7 2023-08-08 05:07:49.000000 pygifconvt_daun-1.0.2/pygifconvt_daun.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2023-08-08 05:07:49.000000 pygifconvt_daun-1.0.2/pygifconvt_daun.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0        0 2020-12-14 06:33:38.000000 pygifconvt_daun-1.0.2/requirements.txt
+-rw-rw-rw-   0        0        0       86 2023-08-08 05:07:49.419129 pygifconvt_daun-1.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      684 2023-08-08 05:02:00.000000 pygifconvt_daun-1.0.2/setup.py
```

### Comparing `pygifconvt_daun-1.0.1/LICENSE` & `pygifconvt_daun-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pygifconvt_daun-1.0.1/README.md` & `pygifconvt_daun-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `pygifconvt_daun-1.0.1/pygifconvt_daun/converter.py` & `pygifconvt_daun-1.0.2/pygifconvt_daun/converter.py`

 * *Files identical despite different names*

### Comparing `pygifconvt_daun-1.0.1/setup.py` & `pygifconvt_daun-1.0.2/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name             = 'pygifconvt_daun',
-    version          = '1.0.1',
+    version          = '1.0.2',
     description      = 'Test package for distribution',
     author           = 'daunj ',
     author_email     = 'otl267@naver.com',
     url              = '',
     download_url     = '',
     install_requires = ['pillow'],
 	include_package_data=True,
```


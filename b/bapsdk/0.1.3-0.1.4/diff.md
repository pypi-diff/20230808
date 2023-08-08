# Comparing `tmp/bapsdk-0.1.3.tar.gz` & `tmp/bapsdk-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bapsdk-0.1.3.tar", last modified: Tue Aug  8 06:38:41 2023, max compression
+gzip compressed data, was "bapsdk-0.1.4.tar", last modified: Tue Aug  8 15:02:46 2023, max compression
```

## Comparing `bapsdk-0.1.3.tar` & `bapsdk-0.1.4.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxr-x   0 kirill    (1000) kirill    (1000)        0 2023-08-08 06:38:41.009852 bapsdk-0.1.3/
--rw-rw-r--   0 kirill    (1000) kirill    (1000)     1053 2023-06-07 19:03:22.000000 bapsdk-0.1.3/LICENSE
--rw-rw-r--   0 kirill    (1000) kirill    (1000)      399 2023-08-08 06:38:41.009852 bapsdk-0.1.3/PKG-INFO
--rw-rw-r--   0 kirill    (1000) kirill    (1000)     1606 2023-08-08 06:38:21.000000 bapsdk-0.1.3/README.md
-drwxrwxr-x   0 kirill    (1000) kirill    (1000)        0 2023-08-08 06:38:41.005852 bapsdk-0.1.3/bap/
--rw-rw-r--   0 kirill    (1000) kirill    (1000)       58 2023-06-07 18:51:08.000000 bapsdk-0.1.3/bap/__init__.py
--rw-rw-r--   0 kirill    (1000) kirill    (1000)      516 2023-08-08 06:38:21.000000 bapsdk-0.1.3/bap/_aiogram.py
--rw-rw-r--   0 kirill    (1000) kirill    (1000)     1329 2023-08-08 06:38:21.000000 bapsdk-0.1.3/bap/_bap.py
-drwxrwxr-x   0 kirill    (1000) kirill    (1000)        0 2023-08-08 06:38:41.009852 bapsdk-0.1.3/bapsdk.egg-info/
--rw-rw-r--   0 kirill    (1000) kirill    (1000)      399 2023-08-08 06:38:41.000000 bapsdk-0.1.3/bapsdk.egg-info/PKG-INFO
--rw-rw-r--   0 kirill    (1000) kirill    (1000)      219 2023-08-08 06:38:41.000000 bapsdk-0.1.3/bapsdk.egg-info/SOURCES.txt
--rw-rw-r--   0 kirill    (1000) kirill    (1000)        1 2023-08-08 06:38:41.000000 bapsdk-0.1.3/bapsdk.egg-info/dependency_links.txt
--rw-rw-r--   0 kirill    (1000) kirill    (1000)       34 2023-08-08 06:38:41.000000 bapsdk-0.1.3/bapsdk.egg-info/requires.txt
--rw-rw-r--   0 kirill    (1000) kirill    (1000)        4 2023-08-08 06:38:41.000000 bapsdk-0.1.3/bapsdk.egg-info/top_level.txt
--rw-rw-r--   0 kirill    (1000) kirill    (1000)       38 2023-08-08 06:38:41.009852 bapsdk-0.1.3/setup.cfg
--rw-rw-r--   0 kirill    (1000) kirill    (1000)      549 2023-08-08 06:38:21.000000 bapsdk-0.1.3/setup.py
+drwxrwxr-x   0 kirill    (1000) kirill    (1000)        0 2023-08-08 15:02:46.619850 bapsdk-0.1.4/
+-rw-rw-r--   0 kirill    (1000) kirill    (1000)     1053 2023-06-07 19:03:22.000000 bapsdk-0.1.4/LICENSE
+-rw-rw-r--   0 kirill    (1000) kirill    (1000)      399 2023-08-08 15:02:46.619850 bapsdk-0.1.4/PKG-INFO
+-rw-rw-r--   0 kirill    (1000) kirill    (1000)     1762 2023-08-08 15:02:39.000000 bapsdk-0.1.4/README.md
+drwxrwxr-x   0 kirill    (1000) kirill    (1000)        0 2023-08-08 15:02:46.619850 bapsdk-0.1.4/bap/
+-rw-rw-r--   0 kirill    (1000) kirill    (1000)       58 2023-06-07 18:51:08.000000 bapsdk-0.1.4/bap/__init__.py
+-rw-rw-r--   0 kirill    (1000) kirill    (1000)      516 2023-08-08 06:38:21.000000 bapsdk-0.1.4/bap/_aiogram.py
+-rw-rw-r--   0 kirill    (1000) kirill    (1000)     2599 2023-08-08 15:02:39.000000 bapsdk-0.1.4/bap/_bap.py
+drwxrwxr-x   0 kirill    (1000) kirill    (1000)        0 2023-08-08 15:02:46.619850 bapsdk-0.1.4/bapsdk.egg-info/
+-rw-rw-r--   0 kirill    (1000) kirill    (1000)      399 2023-08-08 15:02:46.000000 bapsdk-0.1.4/bapsdk.egg-info/PKG-INFO
+-rw-rw-r--   0 kirill    (1000) kirill    (1000)      219 2023-08-08 15:02:46.000000 bapsdk-0.1.4/bapsdk.egg-info/SOURCES.txt
+-rw-rw-r--   0 kirill    (1000) kirill    (1000)        1 2023-08-08 15:02:46.000000 bapsdk-0.1.4/bapsdk.egg-info/dependency_links.txt
+-rw-rw-r--   0 kirill    (1000) kirill    (1000)       34 2023-08-08 15:02:46.000000 bapsdk-0.1.4/bapsdk.egg-info/requires.txt
+-rw-rw-r--   0 kirill    (1000) kirill    (1000)        4 2023-08-08 15:02:46.000000 bapsdk-0.1.4/bapsdk.egg-info/top_level.txt
+-rw-rw-r--   0 kirill    (1000) kirill    (1000)       38 2023-08-08 15:02:46.619850 bapsdk-0.1.4/setup.cfg
+-rw-rw-r--   0 kirill    (1000) kirill    (1000)      549 2023-08-08 15:02:39.000000 bapsdk-0.1.4/setup.py
```

### Comparing `bapsdk-0.1.3/LICENSE` & `bapsdk-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `bapsdk-0.1.3/README.md` & `bapsdk-0.1.4/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -31,14 +31,20 @@
 
 At times, BAP may introduce telegram updates within its advertisement flow. To maintain the logical consistency of your bot, it is necessary to ignore such updates.
 
 The `BAP.handle_update` method returns a boolean value indicating whether you should proceed with handling the request or skip it as an internal BAP request.
 
 When the method returns `false`, it signifies that the current request should not be processed by your bot.
 
+For manual advertisement mode (Should be turned on in settings) call following in the desired ad placements.
+
+```python
+bap.send_advertisement(update)
+```
+
 ### API Key
 
 **API key is not your Telegram bot token.**
 
 API key must be obtained from [socialjet.pro](https://publisher.socialjet.pro/)
 
 ## About
```

### Comparing `bapsdk-0.1.3/bap/_aiogram.py` & `bapsdk-0.1.4/bap/_aiogram.py`

 * *Files identical despite different names*

### Comparing `bapsdk-0.1.3/setup.py` & `bapsdk-0.1.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup
 
 setup(
     name='bapsdk',
     packages=['bap'],
-    version='0.1.3',
+    version='0.1.4',
     description='Bot Advertising Platform SDK',
     long_description_content_type="text/markdown",
     python_requires='>=3.7',
     classifiers=[
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
```


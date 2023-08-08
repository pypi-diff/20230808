# Comparing `tmp/bapsdk-0.1.2.tar.gz` & `tmp/bapsdk-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bapsdk-0.1.2.tar", last modified: Wed Jun  7 19:31:57 2023, max compression
+gzip compressed data, was "bapsdk-0.1.3.tar", last modified: Tue Aug  8 06:38:41 2023, max compression
```

## Comparing `bapsdk-0.1.2.tar` & `bapsdk-0.1.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxr-x   0 kirill    (1000) kirill    (1000)        0 2023-06-07 19:31:57.403482 bapsdk-0.1.2/
--rw-rw-r--   0 kirill    (1000) kirill    (1000)     1053 2023-06-07 19:03:22.000000 bapsdk-0.1.2/LICENSE
--rw-rw-r--   0 kirill    (1000) kirill    (1000)      399 2023-06-07 19:31:57.399482 bapsdk-0.1.2/PKG-INFO
--rw-rw-r--   0 kirill    (1000) kirill    (1000)     1140 2023-06-07 19:00:05.000000 bapsdk-0.1.2/README.md
-drwxrwxr-x   0 kirill    (1000) kirill    (1000)        0 2023-06-07 19:31:57.399482 bapsdk-0.1.2/bap/
--rw-rw-r--   0 kirill    (1000) kirill    (1000)       58 2023-06-07 18:51:08.000000 bapsdk-0.1.2/bap/__init__.py
--rw-rw-r--   0 kirill    (1000) kirill    (1000)      388 2023-06-07 18:51:08.000000 bapsdk-0.1.2/bap/_aiogram.py
--rw-rw-r--   0 kirill    (1000) kirill    (1000)      519 2023-06-07 18:56:14.000000 bapsdk-0.1.2/bap/_bap.py
-drwxrwxr-x   0 kirill    (1000) kirill    (1000)        0 2023-06-07 19:31:57.399482 bapsdk-0.1.2/bapsdk.egg-info/
--rw-rw-r--   0 kirill    (1000) kirill    (1000)      399 2023-06-07 19:31:57.000000 bapsdk-0.1.2/bapsdk.egg-info/PKG-INFO
--rw-rw-r--   0 kirill    (1000) kirill    (1000)      219 2023-06-07 19:31:57.000000 bapsdk-0.1.2/bapsdk.egg-info/SOURCES.txt
--rw-rw-r--   0 kirill    (1000) kirill    (1000)        1 2023-06-07 19:31:57.000000 bapsdk-0.1.2/bapsdk.egg-info/dependency_links.txt
--rw-rw-r--   0 kirill    (1000) kirill    (1000)       34 2023-06-07 19:31:57.000000 bapsdk-0.1.2/bapsdk.egg-info/requires.txt
--rw-rw-r--   0 kirill    (1000) kirill    (1000)        4 2023-06-07 19:31:57.000000 bapsdk-0.1.2/bapsdk.egg-info/top_level.txt
--rw-rw-r--   0 kirill    (1000) kirill    (1000)       38 2023-06-07 19:31:57.403482 bapsdk-0.1.2/setup.cfg
--rw-rw-r--   0 kirill    (1000) kirill    (1000)      549 2023-06-07 19:31:50.000000 bapsdk-0.1.2/setup.py
+drwxrwxr-x   0 kirill    (1000) kirill    (1000)        0 2023-08-08 06:38:41.009852 bapsdk-0.1.3/
+-rw-rw-r--   0 kirill    (1000) kirill    (1000)     1053 2023-06-07 19:03:22.000000 bapsdk-0.1.3/LICENSE
+-rw-rw-r--   0 kirill    (1000) kirill    (1000)      399 2023-08-08 06:38:41.009852 bapsdk-0.1.3/PKG-INFO
+-rw-rw-r--   0 kirill    (1000) kirill    (1000)     1606 2023-08-08 06:38:21.000000 bapsdk-0.1.3/README.md
+drwxrwxr-x   0 kirill    (1000) kirill    (1000)        0 2023-08-08 06:38:41.005852 bapsdk-0.1.3/bap/
+-rw-rw-r--   0 kirill    (1000) kirill    (1000)       58 2023-06-07 18:51:08.000000 bapsdk-0.1.3/bap/__init__.py
+-rw-rw-r--   0 kirill    (1000) kirill    (1000)      516 2023-08-08 06:38:21.000000 bapsdk-0.1.3/bap/_aiogram.py
+-rw-rw-r--   0 kirill    (1000) kirill    (1000)     1329 2023-08-08 06:38:21.000000 bapsdk-0.1.3/bap/_bap.py
+drwxrwxr-x   0 kirill    (1000) kirill    (1000)        0 2023-08-08 06:38:41.009852 bapsdk-0.1.3/bapsdk.egg-info/
+-rw-rw-r--   0 kirill    (1000) kirill    (1000)      399 2023-08-08 06:38:41.000000 bapsdk-0.1.3/bapsdk.egg-info/PKG-INFO
+-rw-rw-r--   0 kirill    (1000) kirill    (1000)      219 2023-08-08 06:38:41.000000 bapsdk-0.1.3/bapsdk.egg-info/SOURCES.txt
+-rw-rw-r--   0 kirill    (1000) kirill    (1000)        1 2023-08-08 06:38:41.000000 bapsdk-0.1.3/bapsdk.egg-info/dependency_links.txt
+-rw-rw-r--   0 kirill    (1000) kirill    (1000)       34 2023-08-08 06:38:41.000000 bapsdk-0.1.3/bapsdk.egg-info/requires.txt
+-rw-rw-r--   0 kirill    (1000) kirill    (1000)        4 2023-08-08 06:38:41.000000 bapsdk-0.1.3/bapsdk.egg-info/top_level.txt
+-rw-rw-r--   0 kirill    (1000) kirill    (1000)       38 2023-08-08 06:38:41.009852 bapsdk-0.1.3/setup.cfg
+-rw-rw-r--   0 kirill    (1000) kirill    (1000)      549 2023-08-08 06:38:21.000000 bapsdk-0.1.3/setup.py
```

### Comparing `bapsdk-0.1.2/LICENSE` & `bapsdk-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `bapsdk-0.1.2/setup.py` & `bapsdk-0.1.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup
 
 setup(
     name='bapsdk',
     packages=['bap'],
-    version='0.1.2',
+    version='0.1.3',
     description='Bot Advertising Platform SDK',
     long_description_content_type="text/markdown",
     python_requires='>=3.7',
     classifiers=[
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
```


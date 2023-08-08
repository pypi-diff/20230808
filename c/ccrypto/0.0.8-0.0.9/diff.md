# Comparing `tmp/ccrypto-0.0.8.tar.gz` & `tmp/ccrypto-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ccrypto-0.0.8.tar", last modified: Tue Aug  8 13:06:16 2023, max compression
+gzip compressed data, was "ccrypto-0.0.9.tar", last modified: Tue Aug  8 13:13:31 2023, max compression
```

## Comparing `ccrypto-0.0.8.tar` & `ccrypto-0.0.9.tar`

### file list

```diff
@@ -1,15 +1,16 @@
-drwxr-xr-x   0 pawel      (501) staff       (20)        0 2023-08-08 13:06:16.627523 ccrypto-0.0.8/
--rw-r--r--   0 pawel      (501) staff       (20)     1059 2023-08-03 12:17:20.000000 ccrypto-0.0.8/LICENCE
--rw-r--r--   0 pawel      (501) staff       (20)      487 2023-08-08 13:06:16.627275 ccrypto-0.0.8/PKG-INFO
--rw-r--r--   0 pawel      (501) staff       (20)      145 2023-08-03 16:11:15.000000 ccrypto-0.0.8/README.md
-drwxr-xr-x   0 pawel      (501) staff       (20)        0 2023-08-08 13:06:16.625417 ccrypto-0.0.8/ccrypto/
--rw-r--r--   0 pawel      (501) staff       (20)        2 2023-08-03 16:45:00.000000 ccrypto-0.0.8/ccrypto/__init__.py
--rw-r--r--   0 pawel      (501) staff       (20)     2662 2023-08-08 13:04:28.000000 ccrypto-0.0.8/ccrypto/cmc.py
-drwxr-xr-x   0 pawel      (501) staff       (20)        0 2023-08-08 13:06:16.626966 ccrypto-0.0.8/ccrypto.egg-info/
--rw-r--r--   0 pawel      (501) staff       (20)      487 2023-08-08 13:06:16.000000 ccrypto-0.0.8/ccrypto.egg-info/PKG-INFO
--rw-r--r--   0 pawel      (501) staff       (20)      215 2023-08-08 13:06:16.000000 ccrypto-0.0.8/ccrypto.egg-info/SOURCES.txt
--rw-r--r--   0 pawel      (501) staff       (20)        1 2023-08-08 13:06:16.000000 ccrypto-0.0.8/ccrypto.egg-info/dependency_links.txt
--rw-r--r--   0 pawel      (501) staff       (20)       56 2023-08-08 13:06:16.000000 ccrypto-0.0.8/ccrypto.egg-info/requires.txt
--rw-r--r--   0 pawel      (501) staff       (20)        8 2023-08-08 13:06:16.000000 ccrypto-0.0.8/ccrypto.egg-info/top_level.txt
--rw-r--r--   0 pawel      (501) staff       (20)       38 2023-08-08 13:06:16.627592 ccrypto-0.0.8/setup.cfg
--rw-r--r--   0 pawel      (501) staff       (20)      937 2023-08-08 13:04:53.000000 ccrypto-0.0.8/setup.py
+drwxr-xr-x   0 pawel      (501) staff       (20)        0 2023-08-08 13:13:31.494122 ccrypto-0.0.9/
+-rw-r--r--   0 pawel      (501) staff       (20)     1059 2023-08-03 12:17:20.000000 ccrypto-0.0.9/LICENCE
+-rw-r--r--   0 pawel      (501) staff       (20)      487 2023-08-08 13:13:31.493829 ccrypto-0.0.9/PKG-INFO
+-rw-r--r--   0 pawel      (501) staff       (20)      145 2023-08-03 16:11:15.000000 ccrypto-0.0.9/README.md
+drwxr-xr-x   0 pawel      (501) staff       (20)        0 2023-08-08 13:13:31.492127 ccrypto-0.0.9/ccrypto/
+-rw-r--r--   0 pawel      (501) staff       (20)        2 2023-08-03 16:45:00.000000 ccrypto-0.0.9/ccrypto/__init__.py
+-rw-r--r--   0 pawel      (501) staff       (20)     2662 2023-08-08 13:04:28.000000 ccrypto-0.0.9/ccrypto/cmc.py
+-rw-r--r--   0 pawel      (501) staff       (20)      226 2023-07-25 12:00:04.000000 ccrypto-0.0.9/ccrypto/mycryptokeys.py
+drwxr-xr-x   0 pawel      (501) staff       (20)        0 2023-08-08 13:13:31.493542 ccrypto-0.0.9/ccrypto.egg-info/
+-rw-r--r--   0 pawel      (501) staff       (20)      487 2023-08-08 13:13:31.000000 ccrypto-0.0.9/ccrypto.egg-info/PKG-INFO
+-rw-r--r--   0 pawel      (501) staff       (20)      239 2023-08-08 13:13:31.000000 ccrypto-0.0.9/ccrypto.egg-info/SOURCES.txt
+-rw-r--r--   0 pawel      (501) staff       (20)        1 2023-08-08 13:13:31.000000 ccrypto-0.0.9/ccrypto.egg-info/dependency_links.txt
+-rw-r--r--   0 pawel      (501) staff       (20)       56 2023-08-08 13:13:31.000000 ccrypto-0.0.9/ccrypto.egg-info/requires.txt
+-rw-r--r--   0 pawel      (501) staff       (20)        8 2023-08-08 13:13:31.000000 ccrypto-0.0.9/ccrypto.egg-info/top_level.txt
+-rw-r--r--   0 pawel      (501) staff       (20)       38 2023-08-08 13:13:31.494201 ccrypto-0.0.9/setup.cfg
+-rw-r--r--   0 pawel      (501) staff       (20)      937 2023-08-08 13:13:12.000000 ccrypto-0.0.9/setup.py
```

### Comparing `ccrypto-0.0.8/LICENCE` & `ccrypto-0.0.9/LICENCE`

 * *Files identical despite different names*

### Comparing `ccrypto-0.0.8/ccrypto/cmc.py` & `ccrypto-0.0.9/ccrypto/cmc.py`

 * *Files identical despite different names*

### Comparing `ccrypto-0.0.8/setup.py` & `ccrypto-0.0.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import pathlib
 from setuptools import setup, find_packages
 
 HERE = pathlib.Path(__file__).parent
 
-VERSION = '0.0.8'
+VERSION = '0.0.9'
 PACKAGE_NAME = 'ccrypto'
 AUTHOR = 'Pawel Lachowicz'
 AUTHOR_EMAIL = 'pawel.lachowicz@quantatrisk.com'
 URL = 'https://github.com/quantatrisk/ccrypto'
 
 LICENSE = 'MIT'
 DESCRIPTION = 'Crypto-Finance Python library for crypto markets and data analysis by QuantAtRisk.com'
```


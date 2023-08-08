# Comparing `tmp/ccrypto-0.0.6.tar.gz` & `tmp/ccrypto-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ccrypto-0.0.6.tar", last modified: Thu Aug  3 16:54:14 2023, max compression
+gzip compressed data, was "ccrypto-0.0.7.tar", last modified: Tue Aug  8 12:55:35 2023, max compression
```

## Comparing `ccrypto-0.0.6.tar` & `ccrypto-0.0.7.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 pawel      (501) staff       (20)        0 2023-08-03 16:54:14.642465 ccrypto-0.0.6/
--rw-r--r--   0 pawel      (501) staff       (20)      350 2023-08-03 16:54:14.642556 ccrypto-0.0.6/PKG-INFO
--rw-r--r--   0 pawel      (501) staff       (20)      145 2023-08-03 16:11:15.000000 ccrypto-0.0.6/README.rst
--rw-r--r--   0 pawel      (501) staff       (20)      107 2023-08-03 16:54:14.642930 ccrypto-0.0.6/setup.cfg
--rw-r--r--   0 pawel      (501) staff       (20)      669 2023-08-03 16:53:09.000000 ccrypto-0.0.6/setup.py
-drwxr-xr-x   0 pawel      (501) staff       (20)        0 2023-08-03 16:54:14.639150 ccrypto-0.0.6/src/
-drwxr-xr-x   0 pawel      (501) staff       (20)        0 2023-08-03 16:54:14.640756 ccrypto-0.0.6/src/ccrypto/
--rw-r--r--   0 pawel      (501) staff       (20)        2 2023-08-03 16:45:00.000000 ccrypto-0.0.6/src/ccrypto/__init__.py
--rw-r--r--   0 pawel      (501) staff       (20)     2672 2023-08-03 16:19:35.000000 ccrypto-0.0.6/src/ccrypto/get_cmc_coins_by_mcap.py
-drwxr-xr-x   0 pawel      (501) staff       (20)        0 2023-08-03 16:54:14.642222 ccrypto-0.0.6/src/ccrypto.egg-info/
--rw-r--r--   0 pawel      (501) staff       (20)      350 2023-08-03 16:54:14.000000 ccrypto-0.0.6/src/ccrypto.egg-info/PKG-INFO
--rw-r--r--   0 pawel      (501) staff       (20)      264 2023-08-03 16:54:14.000000 ccrypto-0.0.6/src/ccrypto.egg-info/SOURCES.txt
--rw-r--r--   0 pawel      (501) staff       (20)        1 2023-08-03 16:54:14.000000 ccrypto-0.0.6/src/ccrypto.egg-info/dependency_links.txt
--rw-r--r--   0 pawel      (501) staff       (20)       56 2023-08-03 16:54:14.000000 ccrypto-0.0.6/src/ccrypto.egg-info/requires.txt
--rw-r--r--   0 pawel      (501) staff       (20)        8 2023-08-03 16:54:14.000000 ccrypto-0.0.6/src/ccrypto.egg-info/top_level.txt
+drwxr-xr-x   0 pawel      (501) staff       (20)        0 2023-08-08 12:55:35.792567 ccrypto-0.0.7/
+-rw-r--r--   0 pawel      (501) staff       (20)     1059 2023-08-03 12:17:20.000000 ccrypto-0.0.7/LICENCE
+-rw-r--r--   0 pawel      (501) staff       (20)      487 2023-08-08 12:55:35.792320 ccrypto-0.0.7/PKG-INFO
+-rw-r--r--   0 pawel      (501) staff       (20)      145 2023-08-03 16:11:15.000000 ccrypto-0.0.7/README.md
+drwxr-xr-x   0 pawel      (501) staff       (20)        0 2023-08-08 12:55:35.790578 ccrypto-0.0.7/ccrypto/
+-rw-r--r--   0 pawel      (501) staff       (20)        2 2023-08-03 16:45:00.000000 ccrypto-0.0.7/ccrypto/__init__.py
+-rw-r--r--   0 pawel      (501) staff       (20)     2672 2023-08-03 16:19:35.000000 ccrypto-0.0.7/ccrypto/get_cmc_coins_by_mcap.py
+drwxr-xr-x   0 pawel      (501) staff       (20)        0 2023-08-08 12:55:35.791999 ccrypto-0.0.7/ccrypto.egg-info/
+-rw-r--r--   0 pawel      (501) staff       (20)      487 2023-08-08 12:55:35.000000 ccrypto-0.0.7/ccrypto.egg-info/PKG-INFO
+-rw-r--r--   0 pawel      (501) staff       (20)      233 2023-08-08 12:55:35.000000 ccrypto-0.0.7/ccrypto.egg-info/SOURCES.txt
+-rw-r--r--   0 pawel      (501) staff       (20)        1 2023-08-08 12:55:35.000000 ccrypto-0.0.7/ccrypto.egg-info/dependency_links.txt
+-rw-r--r--   0 pawel      (501) staff       (20)       56 2023-08-08 12:55:35.000000 ccrypto-0.0.7/ccrypto.egg-info/requires.txt
+-rw-r--r--   0 pawel      (501) staff       (20)        8 2023-08-08 12:55:35.000000 ccrypto-0.0.7/ccrypto.egg-info/top_level.txt
+-rw-r--r--   0 pawel      (501) staff       (20)       38 2023-08-08 12:55:35.792637 ccrypto-0.0.7/setup.cfg
+-rw-r--r--   0 pawel      (501) staff       (20)      937 2023-08-08 12:45:54.000000 ccrypto-0.0.7/setup.py
```

### Comparing `ccrypto-0.0.6/src/ccrypto/get_cmc_coins_by_mcap.py` & `ccrypto-0.0.7/ccrypto/get_cmc_coins_by_mcap.py`

 * *Files identical despite different names*


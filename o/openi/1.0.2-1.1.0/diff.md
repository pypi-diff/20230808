# Comparing `tmp/openi-1.0.2.tar.gz` & `tmp/openi-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openi-1.0.2.tar", last modified: Tue Jun 20 07:05:45 2023, max compression
+gzip compressed data, was "openi-1.1.0.tar", last modified: Tue Aug  8 09:53:45 2023, max compression
```

## Comparing `openi-1.0.2.tar` & `openi-1.1.0.tar`

### file list

```diff
@@ -1,22 +1,27 @@
-drwxr-xr-x   0 jochen10518   (501) staff       (20)        0 2023-06-20 07:05:45.470581 openi-1.0.2/
--rw-r--r--   0 jochen10518   (501) staff       (20)     2097 2023-06-20 07:05:45.470425 openi-1.0.2/PKG-INFO
--rw-r--r--   0 jochen10518   (501) staff       (20)     1473 2023-06-20 03:39:14.000000 openi-1.0.2/README.md
--rw-r--r--   0 jochen10518   (501) staff       (20)       38 2023-06-20 07:05:45.470637 openi-1.0.2/setup.cfg
--rw-r--r--   0 jochen10518   (501) staff       (20)     1140 2023-06-20 07:05:40.000000 openi-1.0.2/setup.py
-drwxr-xr-x   0 jochen10518   (501) staff       (20)        0 2023-06-20 07:05:45.467519 openi-1.0.2/src/
-drwxr-xr-x   0 jochen10518   (501) staff       (20)        0 2023-06-20 07:05:45.468479 openi-1.0.2/src/openi/
--rw-r--r--   0 jochen10518   (501) staff       (20)       48 2023-06-20 03:39:14.000000 openi-1.0.2/src/openi/__init__.py
--rw-r--r--   0 jochen10518   (501) staff       (20)      356 2023-06-20 03:40:01.000000 openi-1.0.2/src/openi/constants.py
-drwxr-xr-x   0 jochen10518   (501) staff       (20)        0 2023-06-20 07:05:45.469628 openi-1.0.2/src/openi/dataset/
--rw-r--r--   0 jochen10518   (501) staff       (20)       22 2023-06-20 03:39:14.000000 openi-1.0.2/src/openi/dataset/__init__.py
--rw-r--r--   0 jochen10518   (501) staff       (20)    12649 2023-06-20 06:57:23.000000 openi-1.0.2/src/openi/dataset/dataset.py
-drwxr-xr-x   0 jochen10518   (501) staff       (20)        0 2023-06-20 07:05:45.469884 openi-1.0.2/src/openi/utils/
--rw-r--r--   0 jochen10518   (501) staff       (20)      419 2023-06-20 03:40:01.000000 openi-1.0.2/src/openi/utils/logger.py
-drwxr-xr-x   0 jochen10518   (501) staff       (20)        0 2023-06-20 07:05:45.469276 openi-1.0.2/src/openi.egg-info/
--rw-r--r--   0 jochen10518   (501) staff       (20)     2097 2023-06-20 07:05:45.000000 openi-1.0.2/src/openi.egg-info/PKG-INFO
--rw-r--r--   0 jochen10518   (501) staff       (20)      338 2023-06-20 07:05:45.000000 openi-1.0.2/src/openi.egg-info/SOURCES.txt
--rw-r--r--   0 jochen10518   (501) staff       (20)        1 2023-06-20 07:05:45.000000 openi-1.0.2/src/openi.egg-info/dependency_links.txt
--rw-r--r--   0 jochen10518   (501) staff       (20)       14 2023-06-20 07:05:45.000000 openi-1.0.2/src/openi.egg-info/requires.txt
--rw-r--r--   0 jochen10518   (501) staff       (20)        6 2023-06-20 07:05:45.000000 openi-1.0.2/src/openi.egg-info/top_level.txt
-drwxr-xr-x   0 jochen10518   (501) staff       (20)        0 2023-06-20 07:05:45.470125 openi-1.0.2/test/
--rw-r--r--   0 jochen10518   (501) staff       (20)      627 2023-06-20 03:39:14.000000 openi-1.0.2/test/test_upload_multi.py
+drwxrwxrwx   0        0        0        0 2023-08-08 09:53:45.806083 openi-1.1.0/
+-rw-rw-rw-   0        0        0     2083 2023-08-08 09:53:45.805069 openi-1.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0     1442 2023-08-08 09:50:10.000000 openi-1.1.0/README.md
+-rw-rw-rw-   0        0        0       42 2023-08-08 09:53:45.806083 openi-1.1.0/setup.cfg
+-rw-rw-rw-   0        0        0      953 2023-08-08 09:53:07.000000 openi-1.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-08 09:53:45.771096 openi-1.1.0/src/
+drwxrwxrwx   0        0        0        0 2023-08-08 09:53:45.779381 openi-1.1.0/src/openi/
+-rw-rw-rw-   0        0        0      146 2023-08-08 09:49:34.000000 openi-1.1.0/src/openi/__init__.py
+-rw-rw-rw-   0        0        0     6456 2023-08-08 09:49:34.000000 openi-1.1.0/src/openi/apis.py
+-rw-rw-rw-   0        0        0     5238 2023-08-08 09:49:34.000000 openi-1.1.0/src/openi/cli.py
+drwxrwxrwx   0        0        0        0 2023-08-08 09:53:45.802558 openi-1.1.0/src/openi/dataset/
+-rw-rw-rw-   0        0        0      109 2023-08-08 09:49:34.000000 openi-1.1.0/src/openi/dataset/__init__.py
+-rw-rw-rw-   0        0        0     2752 2023-08-08 09:49:34.000000 openi-1.1.0/src/openi/dataset/dataset_file.py
+-rw-rw-rw-   0        0        0     2671 2023-08-08 09:49:34.000000 openi-1.1.0/src/openi/dataset/download.py
+-rw-rw-rw-   0        0        0     4570 2023-08-08 09:49:34.000000 openi-1.1.0/src/openi/dataset/upload.py
+-rw-rw-rw-   0        0        0     3029 2023-08-08 09:49:34.000000 openi-1.1.0/src/openi/login.py
+-rw-rw-rw-   0        0        0     4078 2023-08-08 09:49:34.000000 openi-1.1.0/src/openi/settings.py
+drwxrwxrwx   0        0        0        0 2023-08-08 09:53:45.804064 openi-1.1.0/src/openi/utils/
+-rw-rw-rw-   0        0        0       50 2023-08-08 09:49:34.000000 openi-1.1.0/src/openi/utils/__init__.py
+-rw-rw-rw-   0        0        0     1400 2023-08-08 09:49:34.000000 openi-1.1.0/src/openi/utils/file_utils.py
+-rw-rw-rw-   0        0        0      723 2023-08-08 09:49:34.000000 openi-1.1.0/src/openi/utils/logger.py
+drwxrwxrwx   0        0        0        0 2023-08-08 09:53:45.797759 openi-1.1.0/src/openi.egg-info/
+-rw-rw-rw-   0        0        0     2083 2023-08-08 09:53:45.000000 openi-1.1.0/src/openi.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      486 2023-08-08 09:53:45.000000 openi-1.1.0/src/openi.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-08 09:53:45.000000 openi-1.1.0/src/openi.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       14 2023-08-08 09:53:45.000000 openi-1.1.0/src/openi.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-08-08 09:53:45.000000 openi-1.1.0/src/openi.egg-info/top_level.txt
```


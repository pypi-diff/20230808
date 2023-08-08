# Comparing `tmp/HeST-0.0.7.tar.gz` & `tmp/HeST-0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/grischbi/Tesseract/hest_repo/dist/.tmp-tidb405_/HeST-0.0.7.tar", last modified: Tue Mar 28 17:31:57 2023, max compression
+gzip compressed data, was "/home/grischbi/Tesseract/HeST_Dev_082023/HeST/dist/.tmp-shmr0jbc/HeST-0.1.tar", last modified: Tue Aug  8 19:21:01 2023, max compression
```

## Comparing `HeST-0.0.7.tar` & `HeST-0.1.tar`

### file list

```diff
@@ -1,15 +1,20 @@
-drwxr-xr-x   0 grischbi  (1000) grischbi  (1000)        0 2023-03-28 17:31:57.143595 HeST-0.0.7/
--rw-r--r--   0 grischbi  (1000) grischbi  (1000)     1074 2023-03-28 16:21:00.000000 HeST-0.0.7/LICENSE
--rw-r--r--   0 grischbi  (1000) grischbi  (1000)      655 2023-03-28 17:31:57.143595 HeST-0.0.7/PKG-INFO
--rw-r--r--   0 grischbi  (1000) grischbi  (1000)       78 2023-03-28 16:21:23.000000 HeST-0.0.7/README.md
--rw-r--r--   0 grischbi  (1000) grischbi  (1000)      681 2023-03-28 17:31:29.000000 HeST-0.0.7/pyproject.toml
--rw-r--r--   0 grischbi  (1000) grischbi  (1000)       38 2023-03-28 17:31:57.143595 HeST-0.0.7/setup.cfg
-drwxr-xr-x   0 grischbi  (1000) grischbi  (1000)        0 2023-03-28 17:31:57.143595 HeST-0.0.7/src/
-drwxr-xr-x   0 grischbi  (1000) grischbi  (1000)        0 2023-03-28 17:31:57.143595 HeST-0.0.7/src/HeST/
--rw-r--r--   0 grischbi  (1000) grischbi  (1000)    24823 2023-03-28 17:31:03.000000 HeST-0.0.7/src/HeST/HeST.py
--rw-r--r--   0 grischbi  (1000) grischbi  (1000)       19 2023-03-28 17:30:54.000000 HeST-0.0.7/src/HeST/__init__.py
-drwxr-xr-x   0 grischbi  (1000) grischbi  (1000)        0 2023-03-28 17:31:57.143595 HeST-0.0.7/src/HeST.egg-info/
--rw-r--r--   0 grischbi  (1000) grischbi  (1000)      655 2023-03-28 17:31:57.000000 HeST-0.0.7/src/HeST.egg-info/PKG-INFO
--rw-r--r--   0 grischbi  (1000) grischbi  (1000)      198 2023-03-28 17:31:57.000000 HeST-0.0.7/src/HeST.egg-info/SOURCES.txt
--rw-r--r--   0 grischbi  (1000) grischbi  (1000)        1 2023-03-28 17:31:57.000000 HeST-0.0.7/src/HeST.egg-info/dependency_links.txt
--rw-r--r--   0 grischbi  (1000) grischbi  (1000)        5 2023-03-28 17:31:57.000000 HeST-0.0.7/src/HeST.egg-info/top_level.txt
+drwxr-xr-x   0 grischbi  (1000) grischbi  (1000)        0 2023-08-08 19:21:01.962602 HeST-0.1/
+drwxr-xr-x   0 grischbi  (1000) grischbi  (1000)        0 2023-08-08 19:21:01.962602 HeST-0.1/HeST/
+-rw-r--r--   0 grischbi  (1000) grischbi  (1000)     2022 2023-08-08 18:48:32.000000 HeST-0.1/HeST/Amherst_Example_Detector.py
+-rw-r--r--   0 grischbi  (1000) grischbi  (1000)    22520 2023-08-08 18:59:47.000000 HeST-0.1/HeST/Detection.py
+-rw-r--r--   0 grischbi  (1000) grischbi  (1000)     8671 2023-08-08 19:04:39.000000 HeST-0.1/HeST/HeST_Core.py
+-rw-r--r--   0 grischbi  (1000) grischbi  (1000)   403568 2023-08-08 18:48:17.000000 HeST-0.1/HeST/LCE_map_amherstExample_41x41x30_noReflections.npy
+-rw-r--r--   0 grischbi  (1000) grischbi  (1000)   403568 2023-08-08 18:48:17.000000 HeST-0.1/HeST/QP_map_amherstExample_41x41x30_noReflections.npy
+-rw-r--r--   0 grischbi  (1000) grischbi  (1000)     5979 2023-08-08 17:44:23.000000 HeST-0.1/HeST/WIMP_Generation.py
+-rw-r--r--   0 grischbi  (1000) grischbi  (1000)      140 2023-08-08 18:40:28.000000 HeST-0.1/HeST/__init__.py
+drwxr-xr-x   0 grischbi  (1000) grischbi  (1000)        0 2023-08-08 19:21:01.962602 HeST-0.1/HeST.egg-info/
+-rw-r--r--   0 grischbi  (1000) grischbi  (1000)       68 2023-08-08 19:21:01.000000 HeST-0.1/HeST.egg-info/PKG-INFO
+-rw-r--r--   0 grischbi  (1000) grischbi  (1000)      384 2023-08-08 19:21:01.000000 HeST-0.1/HeST.egg-info/SOURCES.txt
+-rw-r--r--   0 grischbi  (1000) grischbi  (1000)        1 2023-08-08 19:21:01.000000 HeST-0.1/HeST.egg-info/dependency_links.txt
+-rw-r--r--   0 grischbi  (1000) grischbi  (1000)       12 2023-08-08 19:21:01.000000 HeST-0.1/HeST.egg-info/requires.txt
+-rw-r--r--   0 grischbi  (1000) grischbi  (1000)        5 2023-08-08 19:21:01.000000 HeST-0.1/HeST.egg-info/top_level.txt
+-rw-r--r--   0 grischbi  (1000) grischbi  (1000)     1074 2023-08-08 17:57:23.000000 HeST-0.1/LICENSE
+-rw-r--r--   0 grischbi  (1000) grischbi  (1000)       68 2023-08-08 19:21:01.962602 HeST-0.1/PKG-INFO
+-rw-r--r--   0 grischbi  (1000) grischbi  (1000)      626 2023-08-08 19:16:59.000000 HeST-0.1/README.md
+-rw-r--r--   0 grischbi  (1000) grischbi  (1000)       38 2023-08-08 19:21:01.962602 HeST-0.1/setup.cfg
+-rw-r--r--   0 grischbi  (1000) grischbi  (1000)      214 2023-08-08 18:48:08.000000 HeST-0.1/setup.py
```

### Comparing `HeST-0.0.7/LICENSE` & `HeST-0.1/LICENSE`

 * *Files identical despite different names*


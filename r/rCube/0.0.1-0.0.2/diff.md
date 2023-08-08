# Comparing `tmp/rCube-0.0.1.tar.gz` & `tmp/rCube-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rCube-0.0.1.tar", last modified: Tue Aug  8 03:40:35 2023, max compression
+gzip compressed data, was "rCube-0.0.2.tar", last modified: Tue Aug  8 04:13:02 2023, max compression
```

## Comparing `rCube-0.0.1.tar` & `rCube-0.0.2.tar`

### file list

```diff
@@ -1,11 +1,12 @@
-drwxrwxrwx   0        0        0        0 2023-08-08 03:40:35.001240 rCube-0.0.1/
--rw-rw-rw-   0        0        0     1081 2023-08-08 03:27:44.000000 rCube-0.0.1/License.txt
--rw-rw-rw-   0        0        0      197 2023-08-08 03:40:35.000151 rCube-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0      390 2023-08-08 03:26:09.000000 rCube-0.0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-08-08 03:40:34.999154 rCube-0.0.1/rCube.egg-info/
--rw-rw-rw-   0        0        0      197 2023-08-08 03:40:34.000000 rCube-0.0.1/rCube.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      146 2023-08-08 03:40:34.000000 rCube-0.0.1/rCube.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-08 03:40:34.000000 rCube-0.0.1/rCube.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        1 2023-08-08 03:40:34.000000 rCube-0.0.1/rCube.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-08-08 03:40:35.002242 rCube-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0      298 2023-08-08 03:17:22.000000 rCube-0.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-08 04:13:02.366603 rCube-0.0.2/
+-rw-rw-rw-   0        0        0     1081 2023-08-08 03:27:44.000000 rCube-0.0.2/License.txt
+-rw-rw-rw-   0        0        0      196 2023-08-08 04:13:02.365605 rCube-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0      390 2023-08-08 03:26:09.000000 rCube-0.0.2/README.md
+drwxrwxrwx   0        0        0        0 2023-08-08 04:13:02.364610 rCube-0.0.2/rCube.egg-info/
+-rw-rw-rw-   0        0        0      196 2023-08-08 04:13:02.000000 rCube-0.0.2/rCube.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      174 2023-08-08 04:13:02.000000 rCube-0.0.2/rCube.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-08 04:13:02.000000 rCube-0.0.2/rCube.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       17 2023-08-08 04:13:02.000000 rCube-0.0.2/rCube.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        1 2023-08-08 04:13:02.000000 rCube-0.0.2/rCube.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-08-08 04:13:02.366603 rCube-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      375 2023-08-08 04:12:59.000000 rCube-0.0.2/setup.py
```

### Comparing `rCube-0.0.1/License.txt` & `rCube-0.0.2/License.txt`

 * *Files identical despite different names*


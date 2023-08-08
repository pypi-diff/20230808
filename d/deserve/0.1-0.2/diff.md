# Comparing `tmp/deserve-0.1.tar.gz` & `tmp/deserve-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "deserve-0.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "deserve-0.2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `deserve-0.1.tar` & `deserve-0.2.tar`

### file list

```diff
@@ -1,6 +1,7 @@
--rw-r--r--   0        0        0     3078 2023-08-03 15:56:48.516560 deserve-0.1/.gitignore
--rw-r--r--   0        0        0     1505 2023-08-03 15:56:48.516560 deserve-0.1/LICENSE
--rw-r--r--   0        0        0     1060 2023-08-04 01:03:31.036654 deserve-0.1/README.md
--rw-r--r--   0        0        0      311 2023-08-04 01:29:41.359273 deserve-0.1/pyproject.toml
--rw-r--r--   0        0        0     1224 2023-08-03 22:31:30.980697 deserve-0.1/src/deserve.py
--rw-r--r--   0        0        0     1324 1970-01-01 00:00:00.000000 deserve-0.1/PKG-INFO
+-rw-r--r--   0        0        0      526 2023-08-08 17:46:16.347283 deserve-0.2/.github/workflows/publish.yml
+-rw-r--r--   0        0        0     3078 2023-08-08 17:46:16.347283 deserve-0.2/.gitignore
+-rw-r--r--   0        0        0     1505 2023-08-08 17:46:16.347283 deserve-0.2/LICENSE
+-rw-r--r--   0        0        0     2035 2023-08-08 17:46:16.347283 deserve-0.2/README.md
+-rw-r--r--   0        0        0      311 2023-08-08 17:46:16.347283 deserve-0.2/pyproject.toml
+-rw-r--r--   0        0        0     2062 2023-08-08 17:46:16.347283 deserve-0.2/src/deserve.py
+-rw-r--r--   0        0        0     2299 1970-01-01 00:00:00.000000 deserve-0.2/PKG-INFO
```

### Comparing `deserve-0.1/.gitignore` & `deserve-0.2/.gitignore`

 * *Files identical despite different names*

### Comparing `deserve-0.1/LICENSE` & `deserve-0.2/LICENSE`

 * *Files identical despite different names*


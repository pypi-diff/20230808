# Comparing `tmp/digdata-0.1.0.tar.gz` & `tmp/digdata-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "digdata-0.1.0.tar", max compression
+gzip compressed data, was "digdata-0.1.1.tar", max compression
```

## Comparing `digdata-0.1.0.tar` & `digdata-0.1.1.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0        0 2023-08-07 21:00:05.016842 digdata-0.1.0/README.md
--rw-r--r--   0        0        0       78 2023-08-07 19:08:14.967063 digdata-0.1.0/digdata/checkpoint/__init__.py
--rw-r--r--   0        0        0      734 2023-08-07 19:05:40.350108 digdata-0.1.0/digdata/checkpoint/checkpoint.py
--rw-r--r--   0        0        0      424 2023-08-07 19:09:24.671486 digdata-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      438 1970-01-01 00:00:00.000000 digdata-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-08-08 09:03:18.713840 digdata-0.1.1/README.md
+-rw-r--r--   0        0        0       78 2023-08-08 09:03:18.713840 digdata-0.1.1/digdata/checkpoint/__init__.py
+-rw-r--r--   0        0        0      734 2023-08-08 09:03:18.713840 digdata-0.1.1/digdata/checkpoint/checkpoint.py
+-rw-r--r--   0        0        0      424 2023-08-08 09:03:18.713840 digdata-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0      438 1970-01-01 00:00:00.000000 digdata-0.1.1/PKG-INFO
```

### Comparing `digdata-0.1.0/digdata/checkpoint/checkpoint.py` & `digdata-0.1.1/digdata/checkpoint/checkpoint.py`

 * *Files identical despite different names*


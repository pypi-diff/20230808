# Comparing `tmp/wnsap-0.1.0.tar.gz` & `tmp/wnsap-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wnsap-0.1.0.tar", max compression
+gzip compressed data, was "wnsap-0.1.1.tar", max compression
```

## Comparing `wnsap-0.1.0.tar` & `wnsap-0.1.1.tar`

### file list

```diff
@@ -1,4 +1,4 @@
--rw-r--r--   0        0        0        0 2023-08-08 09:03:42.302169 wnsap-0.1.0/README.md
--rw-r--r--   0        0        0      254 2023-08-08 09:03:42.302169 wnsap-0.1.0/pyproject.toml
--rw-r--r--   0        0        0    10266 2023-08-08 09:14:01.012023 wnsap-0.1.0/wnsap/__init__.py
--rw-r--r--   0        0        0      324 1970-01-01 00:00:00.000000 wnsap-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-08-08 09:03:42.302169 wnsap-0.1.1/README.md
+-rw-r--r--   0        0        0      253 2023-08-08 09:15:59.501996 wnsap-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0    10266 2023-08-08 09:14:01.012023 wnsap-0.1.1/wnsap/__init__.py
+-rw-r--r--   0        0        0      473 1970-01-01 00:00:00.000000 wnsap-0.1.1/PKG-INFO
```

### Comparing `wnsap-0.1.0/wnsap/__init__.py` & `wnsap-0.1.1/wnsap/__init__.py`

 * *Files identical despite different names*


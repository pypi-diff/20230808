# Comparing `tmp/freeplay-0.1.9.tar.gz` & `tmp/freeplay-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "freeplay-0.1.9.tar", max compression
+gzip compressed data, was "freeplay-0.2.0.tar", max compression
```

## Comparing `freeplay-0.1.9.tar` & `freeplay-0.2.0.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0        0 2023-05-18 13:19:32.515553 freeplay-0.1.9/README.md
--rw-r--r--   0        0        0       61 2023-06-29 11:36:19.640171 freeplay-0.1.9/freeplay/__init__.py
--rw-r--r--   0        0        0     1834 2023-06-09 01:58:55.719111 freeplay-0.1.9/freeplay/api_support.py
--rw-r--r--   0        0        0      833 2023-07-19 21:25:17.786018 freeplay-0.1.9/freeplay/completions.py
--rw-r--r--   0        0        0      188 2023-06-15 16:32:13.004072 freeplay-0.1.9/freeplay/errors.py
--rw-r--r--   0        0        0    11304 2023-07-28 17:22:38.916745 freeplay-0.1.9/freeplay/flavors.py
--rw-r--r--   0        0        0    24684 2023-07-19 21:25:17.787170 freeplay-0.1.9/freeplay/freeplay.py
--rw-r--r--   0        0        0      828 2023-06-27 18:52:46.171090 freeplay-0.1.9/freeplay/llm_parameters.py
--rw-r--r--   0        0        0      955 2023-07-19 21:25:17.787505 freeplay-0.1.9/freeplay/provider_config.py
--rw-r--r--   0        0        0      369 2023-07-19 21:25:17.788071 freeplay-0.1.9/freeplay/utils.py
--rw-r--r--   0        0        0      391 2023-08-01 20:46:50.027798 freeplay-0.1.9/pyproject.toml
--rw-r--r--   0        0        0      679 1970-01-01 00:00:00.000000 freeplay-0.1.9/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-05-15 03:23:13.376261 freeplay-0.2.0/README.md
+-rw-r--r--   0        0        0       61 2023-06-28 22:11:30.981007 freeplay-0.2.0/freeplay/__init__.py
+-rw-r--r--   0        0        0     1834 2023-06-08 17:54:13.585930 freeplay-0.2.0/freeplay/api_support.py
+-rw-r--r--   0        0        0      833 2023-07-17 22:42:12.899464 freeplay-0.2.0/freeplay/completions.py
+-rw-r--r--   0        0        0      188 2023-07-11 16:57:31.087747 freeplay-0.2.0/freeplay/errors.py
+-rw-r--r--   0        0        0    11304 2023-07-17 22:42:12.899849 freeplay-0.2.0/freeplay/flavors.py
+-rw-r--r--   0        0        0    24684 2023-08-01 20:26:39.610252 freeplay-0.2.0/freeplay/freeplay.py
+-rw-r--r--   0        0        0      828 2023-07-12 17:07:23.373407 freeplay-0.2.0/freeplay/llm_parameters.py
+-rw-r--r--   0        0        0      955 2023-07-17 22:42:12.900529 freeplay-0.2.0/freeplay/provider_config.py
+-rw-r--r--   0        0        0      369 2023-07-17 22:42:12.900966 freeplay-0.2.0/freeplay/utils.py
+-rw-r--r--   0        0        0      391 2023-08-08 15:35:05.118967 freeplay-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0      679 1970-01-01 00:00:00.000000 freeplay-0.2.0/PKG-INFO
```

### Comparing `freeplay-0.1.9/freeplay/api_support.py` & `freeplay-0.2.0/freeplay/api_support.py`

 * *Files identical despite different names*

### Comparing `freeplay-0.1.9/freeplay/completions.py` & `freeplay-0.2.0/freeplay/completions.py`

 * *Files identical despite different names*

### Comparing `freeplay-0.1.9/freeplay/flavors.py` & `freeplay-0.2.0/freeplay/flavors.py`

 * *Files identical despite different names*

### Comparing `freeplay-0.1.9/freeplay/freeplay.py` & `freeplay-0.2.0/freeplay/freeplay.py`

 * *Files identical despite different names*

### Comparing `freeplay-0.1.9/freeplay/llm_parameters.py` & `freeplay-0.2.0/freeplay/llm_parameters.py`

 * *Files identical despite different names*

### Comparing `freeplay-0.1.9/freeplay/provider_config.py` & `freeplay-0.2.0/freeplay/provider_config.py`

 * *Files identical despite different names*

### Comparing `freeplay-0.1.9/PKG-INFO` & `freeplay-0.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: freeplay
-Version: 0.1.9
+Version: 0.2.0
 Summary: 
 License: MIT
 Author: FreePlay Engineering
 Author-email: engineering@freeplay.ai
 Requires-Python: >=3.8,<4
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```


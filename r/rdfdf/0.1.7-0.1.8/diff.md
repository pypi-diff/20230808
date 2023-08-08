# Comparing `tmp/rdfdf-0.1.7.tar.gz` & `tmp/rdfdf-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rdfdf-0.1.7.tar", max compression
+gzip compressed data, was "rdfdf-0.1.8.tar", max compression
```

## Comparing `rdfdf-0.1.7.tar` & `rdfdf-0.1.8.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0    35149 2023-05-08 07:12:58.000000 rdfdf-0.1.7/LICENSE
--rw-r--r--   0        0        0     5569 2023-07-06 09:06:07.378355 rdfdf-0.1.7/README.md
--rw-r--r--   0        0        0      459 2023-08-08 13:53:47.363555 rdfdf-0.1.7/pyproject.toml
--rw-r--r--   0        0        0        0 2023-06-26 10:17:54.081795 rdfdf-0.1.7/rdfdf/__init__.py
--rw-r--r--   0        0        0        0 2023-05-23 08:11:06.000000 rdfdf-0.1.7/rdfdf/helpers/__init__.py
--rw-r--r--   0        0        0     1323 2023-06-20 14:36:07.751495 rdfdf-0.1.7/rdfdf/helpers/importers.py
--rw-r--r--   0        0        0     1010 2023-07-05 09:33:18.189851 rdfdf-0.1.7/rdfdf/helpers/rdfdf_utils.py
--rw-r--r--   0        0        0     3933 2023-07-06 08:36:25.219082 rdfdf-0.1.7/rdfdf/rdfdf.py
--rw-r--r--   0        0        0      328 2023-07-05 08:35:59.657869 rdfdf-0.1.7/rdfdf/rdfdf_types.py
--rw-r--r--   0        0        0     6126 1970-01-01 00:00:00.000000 rdfdf-0.1.7/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-05-08 07:12:58.000000 rdfdf-0.1.8/LICENSE
+-rw-r--r--   0        0        0     5569 2023-07-06 09:06:07.378355 rdfdf-0.1.8/README.md
+-rw-r--r--   0        0        0      459 2023-08-08 14:09:21.559253 rdfdf-0.1.8/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-06-26 10:17:54.081795 rdfdf-0.1.8/rdfdf/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-23 08:11:06.000000 rdfdf-0.1.8/rdfdf/helpers/__init__.py
+-rw-r--r--   0        0        0     1323 2023-06-20 14:36:07.751495 rdfdf-0.1.8/rdfdf/helpers/importers.py
+-rw-r--r--   0        0        0     1010 2023-07-05 09:33:18.189851 rdfdf-0.1.8/rdfdf/helpers/rdfdf_utils.py
+-rw-r--r--   0        0        0     3933 2023-07-06 08:36:25.219082 rdfdf-0.1.8/rdfdf/rdfdf.py
+-rw-r--r--   0        0        0      328 2023-07-05 08:35:59.657869 rdfdf-0.1.8/rdfdf/rdfdf_types.py
+-rw-r--r--   0        0        0     6126 1970-01-01 00:00:00.000000 rdfdf-0.1.8/PKG-INFO
```

### Comparing `rdfdf-0.1.7/LICENSE` & `rdfdf-0.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `rdfdf-0.1.7/README.md` & `rdfdf-0.1.8/README.md`

 * *Files identical despite different names*

### Comparing `rdfdf-0.1.7/rdfdf/helpers/importers.py` & `rdfdf-0.1.8/rdfdf/helpers/importers.py`

 * *Files identical despite different names*

### Comparing `rdfdf-0.1.7/rdfdf/helpers/rdfdf_utils.py` & `rdfdf-0.1.8/rdfdf/helpers/rdfdf_utils.py`

 * *Files identical despite different names*

### Comparing `rdfdf-0.1.7/rdfdf/rdfdf.py` & `rdfdf-0.1.8/rdfdf/rdfdf.py`

 * *Files identical despite different names*

### Comparing `rdfdf-0.1.7/PKG-INFO` & `rdfdf-0.1.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rdfdf
-Version: 0.1.7
+Version: 0.1.8
 Summary: 
 License: GPL3
 Author: Lukas Plank
 Author-email: lupl@tuta.io
 Requires-Python: >=3.10,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
```


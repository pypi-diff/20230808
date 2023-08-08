# Comparing `tmp/cybrex-1.4.1.tar.gz` & `tmp/cybrex-1.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cybrex-1.4.1.tar", last modified: Tue Aug  8 14:18:39 2023, max compression
+gzip compressed data, was "cybrex-1.4.2.tar", last modified: Tue Aug  8 14:39:25 2023, max compression
```

## Comparing `cybrex-1.4.1.tar` & `cybrex-1.4.2.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 pasha      (501) staff       (20)        0 2023-08-08 14:18:39.835056 cybrex-1.4.1/
--rw-r--r--   0 pasha      (501) staff       (20)       24 2022-12-01 11:19:40.000000 cybrex-1.4.1/MANIFEST.in
--rw-r--r--   0 pasha      (501) staff       (20)     4815 2023-08-08 14:18:39.834105 cybrex-1.4.1/PKG-INFO
--rw-r--r--   0 pasha      (501) staff       (20)     4539 2023-08-08 10:28:15.000000 cybrex-1.4.1/README.md
-drwxr-xr-x   0 pasha      (501) staff       (20)        0 2023-08-08 14:18:39.811567 cybrex-1.4.1/cybrex/
--rw-r--r--   0 pasha      (501) staff       (20)        0 2023-08-07 10:20:27.000000 cybrex-1.4.1/cybrex/__init__.py
-drwxr-xr-x   0 pasha      (501) staff       (20)        0 2023-08-08 14:18:39.820932 cybrex-1.4.1/cybrex/chains/
--rw-r--r--   0 pasha      (501) staff       (20)        0 2023-08-07 10:20:28.000000 cybrex-1.4.1/cybrex/chains/__init__.py
--rw-r--r--   0 pasha      (501) staff       (20)        0 2023-08-07 10:17:49.000000 cybrex-1.4.1/cybrex/chains/base.py
--rw-r--r--   0 pasha      (501) staff       (20)     2389 2023-08-07 14:15:31.000000 cybrex-1.4.1/cybrex/chains/map_reduce.py
--rw-r--r--   0 pasha      (501) staff       (20)     5475 2023-08-08 12:09:00.000000 cybrex-1.4.1/cybrex/cli.py
--rw-r--r--   0 pasha      (501) staff       (20)    12223 2023-08-08 13:44:49.000000 cybrex-1.4.1/cybrex/cybrex_ai.py
-drwxr-xr-x   0 pasha      (501) staff       (20)        0 2023-08-08 14:18:39.824186 cybrex-1.4.1/cybrex/data_source/
--rw-r--r--   0 pasha      (501) staff       (20)      329 2023-08-08 08:33:51.000000 cybrex-1.4.1/cybrex/data_source/base.py
--rw-r--r--   0 pasha      (501) staff       (20)     1293 2023-08-08 13:14:00.000000 cybrex-1.4.1/cybrex/data_source/geck_data_source.py
--rw-r--r--   0 pasha      (501) staff       (20)     1750 2023-08-08 10:22:36.000000 cybrex-1.4.1/cybrex/document_chunker.py
--rw-r--r--   0 pasha      (501) staff       (20)     4843 2023-08-07 14:38:25.000000 cybrex-1.4.1/cybrex/models.py
-drwxr-xr-x   0 pasha      (501) staff       (20)        0 2023-08-08 14:18:39.827238 cybrex-1.4.1/cybrex/prompts/
--rw-r--r--   0 pasha      (501) staff       (20)        0 2023-08-07 10:20:28.000000 cybrex-1.4.1/cybrex/prompts/__init__.py
--rw-r--r--   0 pasha      (501) staff       (20)     9847 2023-08-08 11:30:06.000000 cybrex-1.4.1/cybrex/prompts/base.py
-drwxr-xr-x   0 pasha      (501) staff       (20)        0 2023-08-08 14:18:39.831733 cybrex-1.4.1/cybrex/vector_storage/
--rw-r--r--   0 pasha      (501) staff       (20)        0 2023-08-07 10:20:28.000000 cybrex-1.4.1/cybrex/vector_storage/__init__.py
--rw-r--r--   0 pasha      (501) staff       (20)      213 2023-08-07 15:07:49.000000 cybrex-1.4.1/cybrex/vector_storage/base.py
--rw-r--r--   0 pasha      (501) staff       (20)     2782 2023-08-08 13:45:08.000000 cybrex-1.4.1/cybrex/vector_storage/chroma.py
-drwxr-xr-x   0 pasha      (501) staff       (20)        0 2023-08-08 14:18:39.818466 cybrex-1.4.1/cybrex.egg-info/
--rw-r--r--   0 pasha      (501) staff       (20)     4815 2023-08-08 14:18:39.000000 cybrex-1.4.1/cybrex.egg-info/PKG-INFO
--rw-r--r--   0 pasha      (501) staff       (20)      620 2023-08-08 14:18:39.000000 cybrex-1.4.1/cybrex.egg-info/SOURCES.txt
--rw-r--r--   0 pasha      (501) staff       (20)        1 2023-08-08 14:18:39.000000 cybrex-1.4.1/cybrex.egg-info/dependency_links.txt
--rw-r--r--   0 pasha      (501) staff       (20)       43 2023-08-08 14:18:39.000000 cybrex-1.4.1/cybrex.egg-info/entry_points.txt
--rw-r--r--   0 pasha      (501) staff       (20)      277 2023-08-08 14:18:39.000000 cybrex-1.4.1/cybrex.egg-info/requires.txt
--rw-r--r--   0 pasha      (501) staff       (20)        7 2023-08-08 14:18:39.000000 cybrex-1.4.1/cybrex.egg-info/top_level.txt
--rw-r--r--   0 pasha      (501) staff       (20)      531 2023-08-08 14:17:59.000000 cybrex-1.4.1/pyproject.toml
--rw-r--r--   0 pasha      (501) staff       (20)      277 2023-08-08 14:17:56.000000 cybrex-1.4.1/requirements.txt
--rw-r--r--   0 pasha      (501) staff       (20)       38 2023-08-08 14:18:39.835447 cybrex-1.4.1/setup.cfg
+drwxr-xr-x   0 pasha      (501) staff       (20)        0 2023-08-08 14:39:25.854473 cybrex-1.4.2/
+-rw-r--r--   0 pasha      (501) staff       (20)       24 2022-12-01 11:19:40.000000 cybrex-1.4.2/MANIFEST.in
+-rw-r--r--   0 pasha      (501) staff       (20)     4815 2023-08-08 14:39:25.852880 cybrex-1.4.2/PKG-INFO
+-rw-r--r--   0 pasha      (501) staff       (20)     4539 2023-08-08 10:28:15.000000 cybrex-1.4.2/README.md
+drwxr-xr-x   0 pasha      (501) staff       (20)        0 2023-08-08 14:39:25.805012 cybrex-1.4.2/cybrex/
+-rw-r--r--   0 pasha      (501) staff       (20)        0 2023-08-07 10:20:27.000000 cybrex-1.4.2/cybrex/__init__.py
+drwxr-xr-x   0 pasha      (501) staff       (20)        0 2023-08-08 14:39:25.828515 cybrex-1.4.2/cybrex/chains/
+-rw-r--r--   0 pasha      (501) staff       (20)        0 2023-08-07 10:20:28.000000 cybrex-1.4.2/cybrex/chains/__init__.py
+-rw-r--r--   0 pasha      (501) staff       (20)        0 2023-08-07 10:17:49.000000 cybrex-1.4.2/cybrex/chains/base.py
+-rw-r--r--   0 pasha      (501) staff       (20)     2389 2023-08-07 14:15:31.000000 cybrex-1.4.2/cybrex/chains/map_reduce.py
+-rw-r--r--   0 pasha      (501) staff       (20)     5475 2023-08-08 12:09:00.000000 cybrex-1.4.2/cybrex/cli.py
+-rw-r--r--   0 pasha      (501) staff       (20)    12223 2023-08-08 13:44:49.000000 cybrex-1.4.2/cybrex/cybrex_ai.py
+drwxr-xr-x   0 pasha      (501) staff       (20)        0 2023-08-08 14:39:25.833423 cybrex-1.4.2/cybrex/data_source/
+-rw-r--r--   0 pasha      (501) staff       (20)      329 2023-08-08 08:33:51.000000 cybrex-1.4.2/cybrex/data_source/base.py
+-rw-r--r--   0 pasha      (501) staff       (20)     1293 2023-08-08 13:14:00.000000 cybrex-1.4.2/cybrex/data_source/geck_data_source.py
+-rw-r--r--   0 pasha      (501) staff       (20)     1750 2023-08-08 10:22:36.000000 cybrex-1.4.2/cybrex/document_chunker.py
+-rw-r--r--   0 pasha      (501) staff       (20)     4843 2023-08-07 14:38:25.000000 cybrex-1.4.2/cybrex/models.py
+drwxr-xr-x   0 pasha      (501) staff       (20)        0 2023-08-08 14:39:25.842994 cybrex-1.4.2/cybrex/prompts/
+-rw-r--r--   0 pasha      (501) staff       (20)        0 2023-08-07 10:20:28.000000 cybrex-1.4.2/cybrex/prompts/__init__.py
+-rw-r--r--   0 pasha      (501) staff       (20)     9847 2023-08-08 11:30:06.000000 cybrex-1.4.2/cybrex/prompts/base.py
+drwxr-xr-x   0 pasha      (501) staff       (20)        0 2023-08-08 14:39:25.849583 cybrex-1.4.2/cybrex/vector_storage/
+-rw-r--r--   0 pasha      (501) staff       (20)        0 2023-08-07 10:20:28.000000 cybrex-1.4.2/cybrex/vector_storage/__init__.py
+-rw-r--r--   0 pasha      (501) staff       (20)      213 2023-08-07 15:07:49.000000 cybrex-1.4.2/cybrex/vector_storage/base.py
+-rw-r--r--   0 pasha      (501) staff       (20)     2782 2023-08-08 13:45:08.000000 cybrex-1.4.2/cybrex/vector_storage/chroma.py
+drwxr-xr-x   0 pasha      (501) staff       (20)        0 2023-08-08 14:39:25.823045 cybrex-1.4.2/cybrex.egg-info/
+-rw-r--r--   0 pasha      (501) staff       (20)     4815 2023-08-08 14:39:25.000000 cybrex-1.4.2/cybrex.egg-info/PKG-INFO
+-rw-r--r--   0 pasha      (501) staff       (20)      620 2023-08-08 14:39:25.000000 cybrex-1.4.2/cybrex.egg-info/SOURCES.txt
+-rw-r--r--   0 pasha      (501) staff       (20)        1 2023-08-08 14:39:25.000000 cybrex-1.4.2/cybrex.egg-info/dependency_links.txt
+-rw-r--r--   0 pasha      (501) staff       (20)       43 2023-08-08 14:39:25.000000 cybrex-1.4.2/cybrex.egg-info/entry_points.txt
+-rw-r--r--   0 pasha      (501) staff       (20)      252 2023-08-08 14:39:25.000000 cybrex-1.4.2/cybrex.egg-info/requires.txt
+-rw-r--r--   0 pasha      (501) staff       (20)        7 2023-08-08 14:39:25.000000 cybrex-1.4.2/cybrex.egg-info/top_level.txt
+-rw-r--r--   0 pasha      (501) staff       (20)      531 2023-08-08 14:38:38.000000 cybrex-1.4.2/pyproject.toml
+-rw-r--r--   0 pasha      (501) staff       (20)      252 2023-08-08 14:38:34.000000 cybrex-1.4.2/requirements.txt
+-rw-r--r--   0 pasha      (501) staff       (20)       38 2023-08-08 14:39:25.855048 cybrex-1.4.2/setup.cfg
```

### Comparing `cybrex-1.4.1/PKG-INFO` & `cybrex-1.4.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cybrex
-Version: 1.4.1
+Version: 1.4.2
 Summary: Researching AI
 Author: Interdimensional Walker
 Project-URL: Homepage, https://github.com/nexus-stc/stc
 Classifier: Programming Language :: Python :: 3.8
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `cybrex-1.4.1/README.md` & `cybrex-1.4.2/README.md`

 * *Files identical despite different names*

### Comparing `cybrex-1.4.1/cybrex/chains/map_reduce.py` & `cybrex-1.4.2/cybrex/chains/map_reduce.py`

 * *Files identical despite different names*

### Comparing `cybrex-1.4.1/cybrex/cli.py` & `cybrex-1.4.2/cybrex/cli.py`

 * *Files identical despite different names*

### Comparing `cybrex-1.4.1/cybrex/cybrex_ai.py` & `cybrex-1.4.2/cybrex/cybrex_ai.py`

 * *Files identical despite different names*

### Comparing `cybrex-1.4.1/cybrex/data_source/geck_data_source.py` & `cybrex-1.4.2/cybrex/data_source/geck_data_source.py`

 * *Files identical despite different names*

### Comparing `cybrex-1.4.1/cybrex/document_chunker.py` & `cybrex-1.4.2/cybrex/document_chunker.py`

 * *Files identical despite different names*

### Comparing `cybrex-1.4.1/cybrex/models.py` & `cybrex-1.4.2/cybrex/models.py`

 * *Files identical despite different names*

### Comparing `cybrex-1.4.1/cybrex/prompts/base.py` & `cybrex-1.4.2/cybrex/prompts/base.py`

 * *Files identical despite different names*

### Comparing `cybrex-1.4.1/cybrex/vector_storage/chroma.py` & `cybrex-1.4.2/cybrex/vector_storage/chroma.py`

 * *Files identical despite different names*

### Comparing `cybrex-1.4.1/cybrex.egg-info/PKG-INFO` & `cybrex-1.4.2/cybrex.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cybrex
-Version: 1.4.1
+Version: 1.4.2
 Summary: Researching AI
 Author: Interdimensional Walker
 Project-URL: Homepage, https://github.com/nexus-stc/stc
 Classifier: Programming Language :: Python :: 3.8
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `cybrex-1.4.1/cybrex.egg-info/SOURCES.txt` & `cybrex-1.4.2/cybrex.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cybrex-1.4.1/pyproject.toml` & `cybrex-1.4.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools<65.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "cybrex"
-version = "1.4.1"
+version = "1.4.2"
 authors = [{ name = "Interdimensional Walker" }]
 description = "Researching AI"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
     "Programming Language :: Python :: 3.8",
 ]
```


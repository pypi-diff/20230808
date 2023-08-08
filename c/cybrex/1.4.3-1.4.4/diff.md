# Comparing `tmp/cybrex-1.4.3.tar.gz` & `tmp/cybrex-1.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cybrex-1.4.3.tar", last modified: Tue Aug  8 15:03:19 2023, max compression
+gzip compressed data, was "cybrex-1.4.4.tar", last modified: Tue Aug  8 16:55:52 2023, max compression
```

## Comparing `cybrex-1.4.3.tar` & `cybrex-1.4.4.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 pasha      (501) staff       (20)        0 2023-08-08 15:03:19.219465 cybrex-1.4.3/
--rw-r--r--   0 pasha      (501) staff       (20)       24 2022-12-01 11:19:40.000000 cybrex-1.4.3/MANIFEST.in
--rw-r--r--   0 pasha      (501) staff       (20)     4815 2023-08-08 15:03:19.218458 cybrex-1.4.3/PKG-INFO
--rw-r--r--   0 pasha      (501) staff       (20)     4539 2023-08-08 10:28:15.000000 cybrex-1.4.3/README.md
-drwxr-xr-x   0 pasha      (501) staff       (20)        0 2023-08-08 15:03:19.190035 cybrex-1.4.3/cybrex/
--rw-r--r--   0 pasha      (501) staff       (20)        0 2023-08-07 10:20:27.000000 cybrex-1.4.3/cybrex/__init__.py
-drwxr-xr-x   0 pasha      (501) staff       (20)        0 2023-08-08 15:03:19.203886 cybrex-1.4.3/cybrex/chains/
--rw-r--r--   0 pasha      (501) staff       (20)        0 2023-08-07 10:20:28.000000 cybrex-1.4.3/cybrex/chains/__init__.py
--rw-r--r--   0 pasha      (501) staff       (20)        0 2023-08-07 10:17:49.000000 cybrex-1.4.3/cybrex/chains/base.py
--rw-r--r--   0 pasha      (501) staff       (20)     2389 2023-08-07 14:15:31.000000 cybrex-1.4.3/cybrex/chains/map_reduce.py
--rw-r--r--   0 pasha      (501) staff       (20)     5475 2023-08-08 12:09:00.000000 cybrex-1.4.3/cybrex/cli.py
--rw-r--r--   0 pasha      (501) staff       (20)    12223 2023-08-08 13:44:49.000000 cybrex-1.4.3/cybrex/cybrex_ai.py
-drwxr-xr-x   0 pasha      (501) staff       (20)        0 2023-08-08 15:03:19.207432 cybrex-1.4.3/cybrex/data_source/
--rw-r--r--   0 pasha      (501) staff       (20)      329 2023-08-08 08:33:51.000000 cybrex-1.4.3/cybrex/data_source/base.py
--rw-r--r--   0 pasha      (501) staff       (20)     1293 2023-08-08 13:14:00.000000 cybrex-1.4.3/cybrex/data_source/geck_data_source.py
--rw-r--r--   0 pasha      (501) staff       (20)     1750 2023-08-08 10:22:36.000000 cybrex-1.4.3/cybrex/document_chunker.py
--rw-r--r--   0 pasha      (501) staff       (20)     4843 2023-08-07 14:38:25.000000 cybrex-1.4.3/cybrex/models.py
-drwxr-xr-x   0 pasha      (501) staff       (20)        0 2023-08-08 15:03:19.210404 cybrex-1.4.3/cybrex/prompts/
--rw-r--r--   0 pasha      (501) staff       (20)        0 2023-08-07 10:20:28.000000 cybrex-1.4.3/cybrex/prompts/__init__.py
--rw-r--r--   0 pasha      (501) staff       (20)     9847 2023-08-08 11:30:06.000000 cybrex-1.4.3/cybrex/prompts/base.py
-drwxr-xr-x   0 pasha      (501) staff       (20)        0 2023-08-08 15:03:19.215767 cybrex-1.4.3/cybrex/vector_storage/
--rw-r--r--   0 pasha      (501) staff       (20)        0 2023-08-07 10:20:28.000000 cybrex-1.4.3/cybrex/vector_storage/__init__.py
--rw-r--r--   0 pasha      (501) staff       (20)      213 2023-08-07 15:07:49.000000 cybrex-1.4.3/cybrex/vector_storage/base.py
--rw-r--r--   0 pasha      (501) staff       (20)     2782 2023-08-08 13:45:08.000000 cybrex-1.4.3/cybrex/vector_storage/chroma.py
-drwxr-xr-x   0 pasha      (501) staff       (20)        0 2023-08-08 15:03:19.200250 cybrex-1.4.3/cybrex.egg-info/
--rw-r--r--   0 pasha      (501) staff       (20)     4815 2023-08-08 15:03:19.000000 cybrex-1.4.3/cybrex.egg-info/PKG-INFO
--rw-r--r--   0 pasha      (501) staff       (20)      620 2023-08-08 15:03:19.000000 cybrex-1.4.3/cybrex.egg-info/SOURCES.txt
--rw-r--r--   0 pasha      (501) staff       (20)        1 2023-08-08 15:03:19.000000 cybrex-1.4.3/cybrex.egg-info/dependency_links.txt
--rw-r--r--   0 pasha      (501) staff       (20)       43 2023-08-08 15:03:19.000000 cybrex-1.4.3/cybrex.egg-info/entry_points.txt
--rw-r--r--   0 pasha      (501) staff       (20)      271 2023-08-08 15:03:19.000000 cybrex-1.4.3/cybrex.egg-info/requires.txt
--rw-r--r--   0 pasha      (501) staff       (20)        7 2023-08-08 15:03:19.000000 cybrex-1.4.3/cybrex.egg-info/top_level.txt
--rw-r--r--   0 pasha      (501) staff       (20)      531 2023-08-08 15:02:24.000000 cybrex-1.4.3/pyproject.toml
--rw-r--r--   0 pasha      (501) staff       (20)      271 2023-08-08 15:02:21.000000 cybrex-1.4.3/requirements.txt
--rw-r--r--   0 pasha      (501) staff       (20)       38 2023-08-08 15:03:19.219883 cybrex-1.4.3/setup.cfg
+drwxr-xr-x   0 pasha      (501) staff       (20)        0 2023-08-08 16:55:52.386861 cybrex-1.4.4/
+-rw-r--r--   0 pasha      (501) staff       (20)       24 2022-12-01 11:19:40.000000 cybrex-1.4.4/MANIFEST.in
+-rw-r--r--   0 pasha      (501) staff       (20)     4815 2023-08-08 16:55:52.386594 cybrex-1.4.4/PKG-INFO
+-rw-r--r--   0 pasha      (501) staff       (20)     4539 2023-08-08 10:28:15.000000 cybrex-1.4.4/README.md
+drwxr-xr-x   0 pasha      (501) staff       (20)        0 2023-08-08 16:55:52.379433 cybrex-1.4.4/cybrex/
+-rw-r--r--   0 pasha      (501) staff       (20)        0 2023-08-07 10:20:27.000000 cybrex-1.4.4/cybrex/__init__.py
+drwxr-xr-x   0 pasha      (501) staff       (20)        0 2023-08-08 16:55:52.382406 cybrex-1.4.4/cybrex/chains/
+-rw-r--r--   0 pasha      (501) staff       (20)        0 2023-08-07 10:20:28.000000 cybrex-1.4.4/cybrex/chains/__init__.py
+-rw-r--r--   0 pasha      (501) staff       (20)        0 2023-08-07 10:17:49.000000 cybrex-1.4.4/cybrex/chains/base.py
+-rw-r--r--   0 pasha      (501) staff       (20)     2389 2023-08-07 14:15:31.000000 cybrex-1.4.4/cybrex/chains/map_reduce.py
+-rw-r--r--   0 pasha      (501) staff       (20)     5475 2023-08-08 12:09:00.000000 cybrex-1.4.4/cybrex/cli.py
+-rw-r--r--   0 pasha      (501) staff       (20)    12231 2023-08-08 16:55:32.000000 cybrex-1.4.4/cybrex/cybrex_ai.py
+drwxr-xr-x   0 pasha      (501) staff       (20)        0 2023-08-08 16:55:52.383368 cybrex-1.4.4/cybrex/data_source/
+-rw-r--r--   0 pasha      (501) staff       (20)      329 2023-08-08 08:33:51.000000 cybrex-1.4.4/cybrex/data_source/base.py
+-rw-r--r--   0 pasha      (501) staff       (20)     1293 2023-08-08 13:14:00.000000 cybrex-1.4.4/cybrex/data_source/geck_data_source.py
+-rw-r--r--   0 pasha      (501) staff       (20)     1750 2023-08-08 10:22:36.000000 cybrex-1.4.4/cybrex/document_chunker.py
+-rw-r--r--   0 pasha      (501) staff       (20)     4843 2023-08-07 14:38:25.000000 cybrex-1.4.4/cybrex/models.py
+drwxr-xr-x   0 pasha      (501) staff       (20)        0 2023-08-08 16:55:52.384258 cybrex-1.4.4/cybrex/prompts/
+-rw-r--r--   0 pasha      (501) staff       (20)        0 2023-08-07 10:20:28.000000 cybrex-1.4.4/cybrex/prompts/__init__.py
+-rw-r--r--   0 pasha      (501) staff       (20)     9847 2023-08-08 11:30:06.000000 cybrex-1.4.4/cybrex/prompts/base.py
+drwxr-xr-x   0 pasha      (501) staff       (20)        0 2023-08-08 16:55:52.385782 cybrex-1.4.4/cybrex/vector_storage/
+-rw-r--r--   0 pasha      (501) staff       (20)        0 2023-08-07 10:20:28.000000 cybrex-1.4.4/cybrex/vector_storage/__init__.py
+-rw-r--r--   0 pasha      (501) staff       (20)      213 2023-08-07 15:07:49.000000 cybrex-1.4.4/cybrex/vector_storage/base.py
+-rw-r--r--   0 pasha      (501) staff       (20)     2782 2023-08-08 13:45:08.000000 cybrex-1.4.4/cybrex/vector_storage/chroma.py
+drwxr-xr-x   0 pasha      (501) staff       (20)        0 2023-08-08 16:55:52.381667 cybrex-1.4.4/cybrex.egg-info/
+-rw-r--r--   0 pasha      (501) staff       (20)     4815 2023-08-08 16:55:52.000000 cybrex-1.4.4/cybrex.egg-info/PKG-INFO
+-rw-r--r--   0 pasha      (501) staff       (20)      620 2023-08-08 16:55:52.000000 cybrex-1.4.4/cybrex.egg-info/SOURCES.txt
+-rw-r--r--   0 pasha      (501) staff       (20)        1 2023-08-08 16:55:52.000000 cybrex-1.4.4/cybrex.egg-info/dependency_links.txt
+-rw-r--r--   0 pasha      (501) staff       (20)       43 2023-08-08 16:55:52.000000 cybrex-1.4.4/cybrex.egg-info/entry_points.txt
+-rw-r--r--   0 pasha      (501) staff       (20)      271 2023-08-08 16:55:52.000000 cybrex-1.4.4/cybrex.egg-info/requires.txt
+-rw-r--r--   0 pasha      (501) staff       (20)        7 2023-08-08 16:55:52.000000 cybrex-1.4.4/cybrex.egg-info/top_level.txt
+-rw-r--r--   0 pasha      (501) staff       (20)      531 2023-08-08 16:55:38.000000 cybrex-1.4.4/pyproject.toml
+-rw-r--r--   0 pasha      (501) staff       (20)      271 2023-08-08 15:02:21.000000 cybrex-1.4.4/requirements.txt
+-rw-r--r--   0 pasha      (501) staff       (20)       38 2023-08-08 16:55:52.386963 cybrex-1.4.4/setup.cfg
```

### Comparing `cybrex-1.4.3/PKG-INFO` & `cybrex-1.4.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cybrex
-Version: 1.4.3
+Version: 1.4.4
 Summary: Researching AI
 Author: Interdimensional Walker
 Project-URL: Homepage, https://github.com/nexus-stc/stc
 Classifier: Programming Language :: Python :: 3.8
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `cybrex-1.4.3/README.md` & `cybrex-1.4.4/README.md`

 * *Files identical despite different names*

### Comparing `cybrex-1.4.3/cybrex/chains/map_reduce.py` & `cybrex-1.4.4/cybrex/chains/map_reduce.py`

 * *Files identical despite different names*

### Comparing `cybrex-1.4.3/cybrex/cli.py` & `cybrex-1.4.4/cybrex/cli.py`

 * *Files identical despite different names*

### Comparing `cybrex-1.4.3/cybrex/cybrex_ai.py` & `cybrex-1.4.4/cybrex/cybrex_ai.py`

 * *Files 0% similar despite different names*

```diff
@@ -149,15 +149,15 @@
             logging.getLogger('statbox').info({
                 'action': 'add_full_documents',
                 'mode': 'cybrex',
                 'n': len(chunks),
             })
             await asyncio.get_running_loop().run_in_executor(
                 None,
-                self.vector_storage.upsert(chunks)
+                lambda: self.vector_storage.upsert(chunks)
             )
             logging.getLogger('statbox').info({
                 'action': 'added_full_documents',
                 'mode': 'cybrex',
                 'n': len(chunks),
             })
```

### Comparing `cybrex-1.4.3/cybrex/data_source/geck_data_source.py` & `cybrex-1.4.4/cybrex/data_source/geck_data_source.py`

 * *Files identical despite different names*

### Comparing `cybrex-1.4.3/cybrex/document_chunker.py` & `cybrex-1.4.4/cybrex/document_chunker.py`

 * *Files identical despite different names*

### Comparing `cybrex-1.4.3/cybrex/models.py` & `cybrex-1.4.4/cybrex/models.py`

 * *Files identical despite different names*

### Comparing `cybrex-1.4.3/cybrex/prompts/base.py` & `cybrex-1.4.4/cybrex/prompts/base.py`

 * *Files identical despite different names*

### Comparing `cybrex-1.4.3/cybrex/vector_storage/chroma.py` & `cybrex-1.4.4/cybrex/vector_storage/chroma.py`

 * *Files identical despite different names*

### Comparing `cybrex-1.4.3/cybrex.egg-info/PKG-INFO` & `cybrex-1.4.4/cybrex.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cybrex
-Version: 1.4.3
+Version: 1.4.4
 Summary: Researching AI
 Author: Interdimensional Walker
 Project-URL: Homepage, https://github.com/nexus-stc/stc
 Classifier: Programming Language :: Python :: 3.8
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `cybrex-1.4.3/cybrex.egg-info/SOURCES.txt` & `cybrex-1.4.4/cybrex.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cybrex-1.4.3/pyproject.toml` & `cybrex-1.4.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools<65.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "cybrex"
-version = "1.4.3"
+version = "1.4.4"
 authors = [{ name = "Interdimensional Walker" }]
 description = "Researching AI"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
     "Programming Language :: Python :: 3.8",
 ]
```


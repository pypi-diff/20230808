# Comparing `tmp/stc-geck-1.3.5.tar.gz` & `tmp/stc-geck-1.3.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stc-geck-1.3.5.tar", last modified: Mon Aug  7 17:12:04 2023, max compression
+gzip compressed data, was "stc-geck-1.3.6.tar", last modified: Mon Aug  7 19:19:44 2023, max compression
```

## Comparing `stc-geck-1.3.5.tar` & `stc-geck-1.3.6.tar`

### file list

```diff
@@ -1,20 +1,21 @@
-drwxr-xr-x   0 pasha      (501) staff       (20)        0 2023-08-07 17:12:04.986117 stc-geck-1.3.5/
--rw-r--r--   0 pasha      (501) staff       (20)       24 2022-12-01 11:19:40.000000 stc-geck-1.3.5/MANIFEST.in
--rw-r--r--   0 pasha      (501) staff       (20)     7330 2023-08-07 17:12:04.985904 stc-geck-1.3.5/PKG-INFO
--rw-r--r--   0 pasha      (501) staff       (20)     6985 2023-07-23 19:18:57.000000 stc-geck-1.3.5/README.md
--rw-r--r--   0 pasha      (501) staff       (20)      600 2023-08-07 17:11:41.000000 stc-geck-1.3.5/pyproject.toml
--rw-r--r--   0 pasha      (501) staff       (20)      161 2023-07-30 14:20:06.000000 stc-geck-1.3.5/requirements.txt
--rw-r--r--   0 pasha      (501) staff       (20)       38 2023-08-07 17:12:04.986201 stc-geck-1.3.5/setup.cfg
-drwxr-xr-x   0 pasha      (501) staff       (20)        0 2023-08-07 17:12:04.983183 stc-geck-1.3.5/stc_geck/
--rw-r--r--   0 pasha      (501) staff       (20)        0 2023-07-19 19:56:31.000000 stc-geck-1.3.5/stc_geck/__init__.py
--rw-r--r--   0 pasha      (501) staff       (20)     1451 2023-08-07 17:11:41.000000 stc-geck-1.3.5/stc_geck/advices.py
--rw-r--r--   0 pasha      (501) staff       (20)     7337 2023-08-06 13:26:45.000000 stc-geck-1.3.5/stc_geck/cli.py
--rw-r--r--   0 pasha      (501) staff       (20)     7257 2023-08-07 14:38:25.000000 stc-geck-1.3.5/stc_geck/client.py
--rw-r--r--   0 pasha      (501) staff       (20)     1877 2023-07-22 08:16:03.000000 stc-geck-1.3.5/stc_geck/utils.py
-drwxr-xr-x   0 pasha      (501) staff       (20)        0 2023-08-07 17:12:04.985527 stc-geck-1.3.5/stc_geck.egg-info/
--rw-r--r--   0 pasha      (501) staff       (20)     7330 2023-08-07 17:12:04.000000 stc-geck-1.3.5/stc_geck.egg-info/PKG-INFO
--rw-r--r--   0 pasha      (501) staff       (20)      341 2023-08-07 17:12:04.000000 stc-geck-1.3.5/stc_geck.egg-info/SOURCES.txt
--rw-r--r--   0 pasha      (501) staff       (20)        1 2023-08-07 17:12:04.000000 stc-geck-1.3.5/stc_geck.egg-info/dependency_links.txt
--rw-r--r--   0 pasha      (501) staff       (20)       43 2023-08-07 17:12:04.000000 stc-geck-1.3.5/stc_geck.egg-info/entry_points.txt
--rw-r--r--   0 pasha      (501) staff       (20)      162 2023-08-07 17:12:04.000000 stc-geck-1.3.5/stc_geck.egg-info/requires.txt
--rw-r--r--   0 pasha      (501) staff       (20)        9 2023-08-07 17:12:04.000000 stc-geck-1.3.5/stc_geck.egg-info/top_level.txt
+drwxr-xr-x   0 pasha      (501) staff       (20)        0 2023-08-07 19:19:44.942263 stc-geck-1.3.6/
+-rw-r--r--   0 pasha      (501) staff       (20)       24 2022-12-01 11:19:40.000000 stc-geck-1.3.6/MANIFEST.in
+-rw-r--r--   0 pasha      (501) staff       (20)     7330 2023-08-07 19:19:44.942002 stc-geck-1.3.6/PKG-INFO
+-rw-r--r--   0 pasha      (501) staff       (20)     6985 2023-07-23 19:18:57.000000 stc-geck-1.3.6/README.md
+-rw-r--r--   0 pasha      (501) staff       (20)      600 2023-08-07 19:06:22.000000 stc-geck-1.3.6/pyproject.toml
+-rw-r--r--   0 pasha      (501) staff       (20)      171 2023-08-07 18:22:54.000000 stc-geck-1.3.6/requirements.txt
+-rw-r--r--   0 pasha      (501) staff       (20)       38 2023-08-07 19:19:44.942379 stc-geck-1.3.6/setup.cfg
+drwxr-xr-x   0 pasha      (501) staff       (20)        0 2023-08-07 19:19:44.938911 stc-geck-1.3.6/stc_geck/
+-rw-r--r--   0 pasha      (501) staff       (20)        0 2023-07-19 19:56:31.000000 stc-geck-1.3.6/stc_geck/__init__.py
+-rw-r--r--   0 pasha      (501) staff       (20)     1464 2023-08-07 18:24:50.000000 stc-geck-1.3.6/stc_geck/advices.py
+-rw-r--r--   0 pasha      (501) staff       (20)     7261 2023-08-07 19:06:08.000000 stc-geck-1.3.6/stc_geck/cli.py
+-rw-r--r--   0 pasha      (501) staff       (20)     7257 2023-08-07 14:38:25.000000 stc-geck-1.3.6/stc_geck/client.py
+-rw-r--r--   0 pasha      (501) staff       (20)    10465 2023-08-07 19:04:16.000000 stc-geck-1.3.6/stc_geck/query_builder.py
+-rw-r--r--   0 pasha      (501) staff       (20)     3254 2023-08-07 18:22:54.000000 stc-geck-1.3.6/stc_geck/utils.py
+drwxr-xr-x   0 pasha      (501) staff       (20)        0 2023-08-07 19:19:44.941463 stc-geck-1.3.6/stc_geck.egg-info/
+-rw-r--r--   0 pasha      (501) staff       (20)     7330 2023-08-07 19:19:44.000000 stc-geck-1.3.6/stc_geck.egg-info/PKG-INFO
+-rw-r--r--   0 pasha      (501) staff       (20)      367 2023-08-07 19:19:44.000000 stc-geck-1.3.6/stc_geck.egg-info/SOURCES.txt
+-rw-r--r--   0 pasha      (501) staff       (20)        1 2023-08-07 19:19:44.000000 stc-geck-1.3.6/stc_geck.egg-info/dependency_links.txt
+-rw-r--r--   0 pasha      (501) staff       (20)       43 2023-08-07 19:19:44.000000 stc-geck-1.3.6/stc_geck.egg-info/entry_points.txt
+-rw-r--r--   0 pasha      (501) staff       (20)      172 2023-08-07 19:19:44.000000 stc-geck-1.3.6/stc_geck.egg-info/requires.txt
+-rw-r--r--   0 pasha      (501) staff       (20)        9 2023-08-07 19:19:44.000000 stc-geck-1.3.6/stc_geck.egg-info/top_level.txt
```

### Comparing `stc-geck-1.3.5/PKG-INFO` & `stc-geck-1.3.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stc-geck
-Version: 1.3.5
+Version: 1.3.6
 Summary: GECK (Garden Of Eden Creation Kit) is a toolkit for setting up and maintaning STC
 Author: Interdimensional Walker
 Project-URL: Homepage, https://github.com/nexus-stc/stc
 Classifier: Programming Language :: Python :: 3.8
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `stc-geck-1.3.5/README.md` & `stc-geck-1.3.6/README.md`

 * *Files identical despite different names*

### Comparing `stc-geck-1.3.5/pyproject.toml` & `stc-geck-1.3.6/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools<65.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "stc-geck"
-version = "1.3.5"
+version = "1.3.6"
 authors = [{ name = "Interdimensional Walker" }]
 description = "GECK (Garden Of Eden Creation Kit) is a toolkit for setting up and maintaning STC"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
     "Programming Language :: Python :: 3.8",
 ]
```

### Comparing `stc-geck-1.3.5/stc_geck/advices.py` & `stc-geck-1.3.6/stc_geck/advices.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,11 @@
-from typing import Optional, List
+from typing import (
+    List,
+    Optional,
+)
 
 from aiosumma import SummaClient
 
 TEMPORAL_RANKING_FORMULA = "original_score * custom_score * fastsigm(abs(now - issued_at) / (86400 * 3) + 5, -1)"
 PR_TEMPORAL_RANKING_FORMULA = f"{TEMPORAL_RANKING_FORMULA} * 1.96 * fastsigm(iqpr(quantized_page_rank), 0.15)"
```

### Comparing `stc-geck-1.3.5/stc_geck/cli.py` & `stc-geck-1.3.6/stc_geck/cli.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 from typing import Optional
 
 import fire
 import humanfriendly
 from termcolor import colored
 
 from .client import StcGeck
+from .query_builder import QueryProcessor
 
 
 class ItemNotFound(Exception):
     def __init__(self, query):
         self.query = query
 
     def __str__(self):
@@ -118,22 +119,16 @@
         :param limit: how many results to return, higher values incurs LARGE performance penalty.
 
         :return: metadata records
         """
         print(f"{colored('INFO', 'green')}: Setting up indices: {self.index_name}...")
         async with self.geck as geck:
             print(f"{colored('INFO', 'green')}: Searching {query}...")
-            response = await geck.get_summa_client().search([{
-                "index_alias": self.index_name,
-                "query": {
-                    "match": {"value": query}
-                },
-                "collectors": [{"top_docs": {"limit": limit}}],
-                "is_fieldnorms_scoring_enabled": False,
-            }])
+            query_processor = QueryProcessor('light' if geck.is_embed else 'full')
+            response = await geck.get_summa_client().search(query_processor.process(query, limit=limit, index_aliases=[self.index_name]))
             documents = list(map(lambda x: json.loads(x.document), response.collector_outputs[0].documents.scored_documents))
             return documents
 
     async def serve(self):
         """
         Start serving Summa
         """
```

### Comparing `stc-geck-1.3.5/stc_geck/client.py` & `stc-geck-1.3.6/stc_geck/client.py`

 * *Files identical despite different names*

### Comparing `stc-geck-1.3.5/stc_geck.egg-info/PKG-INFO` & `stc-geck-1.3.6/stc_geck.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stc-geck
-Version: 1.3.5
+Version: 1.3.6
 Summary: GECK (Garden Of Eden Creation Kit) is a toolkit for setting up and maintaning STC
 Author: Interdimensional Walker
 Project-URL: Homepage, https://github.com/nexus-stc/stc
 Classifier: Programming Language :: Python :: 3.8
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```


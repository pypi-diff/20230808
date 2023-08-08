# Comparing `tmp/quaxa-0.1.0.tar.gz` & `tmp/quaxa-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "quaxa-0.1.0.tar", last modified: Tue Jul 25 11:47:40 2023, max compression
+gzip compressed data, was "quaxa-0.1.1.tar", last modified: Tue Aug  8 20:04:12 2023, max compression
```

## Comparing `quaxa-0.1.0.tar` & `quaxa-0.1.1.tar`

### file list

```diff
@@ -1,21 +1,20 @@
-drwxrwxr-x   0 hamster   (1000) hamster   (1000)        0 2023-07-25 11:47:40.654722 quaxa-0.1.0/
--rw-rw-r--   0 hamster   (1000) hamster   (1000)    11355 2023-07-25 11:40:58.000000 quaxa-0.1.0/LICENSE
--rw-rw-r--   0 hamster   (1000) hamster   (1000)       65 2023-07-25 11:40:58.000000 quaxa-0.1.0/MANIFEST.in
--rw-rw-r--   0 hamster   (1000) hamster   (1000)     5966 2023-07-25 11:47:40.654722 quaxa-0.1.0/PKG-INFO
--rw-rw-r--   0 hamster   (1000) hamster   (1000)     5646 2023-07-25 11:40:58.000000 quaxa-0.1.0/README.md
-drwxrwxr-x   0 hamster   (1000) hamster   (1000)        0 2023-07-25 11:47:40.650723 quaxa-0.1.0/quaxa/
--rw-rw-r--   0 hamster   (1000) hamster   (1000)      531 2023-07-25 11:40:58.000000 quaxa-0.1.0/quaxa/__init__.py
--rw-rw-r--   0 hamster   (1000) hamster   (1000)    16022 2023-07-25 11:40:58.000000 quaxa-0.1.0/quaxa/quaxa.py
--rw-rw-r--   0 hamster   (1000) hamster   (1000)      958 2023-07-25 11:40:58.000000 quaxa-0.1.0/quaxa/reader.py
-drwxrwxr-x   0 hamster   (1000) hamster   (1000)        0 2023-07-25 11:47:40.654722 quaxa-0.1.0/quaxa.egg-info/
--rw-rw-r--   0 hamster   (1000) hamster   (1000)     5966 2023-07-25 11:47:40.000000 quaxa-0.1.0/quaxa.egg-info/PKG-INFO
--rw-rw-r--   0 hamster   (1000) hamster   (1000)      291 2023-07-25 11:47:40.000000 quaxa-0.1.0/quaxa.egg-info/SOURCES.txt
--rw-rw-r--   0 hamster   (1000) hamster   (1000)        1 2023-07-25 11:47:40.000000 quaxa-0.1.0/quaxa.egg-info/dependency_links.txt
--rw-rw-r--   0 hamster   (1000) hamster   (1000)       14 2023-07-25 11:47:40.000000 quaxa-0.1.0/quaxa.egg-info/requires.txt
--rw-rw-r--   0 hamster   (1000) hamster   (1000)        6 2023-07-25 11:47:40.000000 quaxa-0.1.0/quaxa.egg-info/top_level.txt
--rw-rw-r--   0 hamster   (1000) hamster   (1000)        1 2023-07-25 11:47:40.000000 quaxa-0.1.0/quaxa.egg-info/zip-safe
--rw-rw-r--   0 hamster   (1000) hamster   (1000)       38 2023-07-25 11:47:40.654722 quaxa-0.1.0/setup.cfg
--rw-rw-r--   0 hamster   (1000) hamster   (1000)      952 2023-07-25 11:40:58.000000 quaxa-0.1.0/setup.py
-drwxrwxr-x   0 hamster   (1000) hamster   (1000)        0 2023-07-25 11:47:40.654722 quaxa-0.1.0/test/
--rw-rw-r--   0 hamster   (1000) hamster   (1000)        0 2023-07-25 11:40:58.000000 quaxa-0.1.0/test/__init__.py
--rw-rw-r--   0 hamster   (1000) hamster   (1000)    19167 2023-07-25 11:40:58.000000 quaxa-0.1.0/test/test_quaxa.py
+drwxrwxr-x   0 hamster   (1000) hamster   (1000)        0 2023-08-08 20:04:12.775848 quaxa-0.1.1/
+-rw-rw-r--   0 hamster   (1000) hamster   (1000)    11355 2023-07-25 11:40:58.000000 quaxa-0.1.1/LICENSE
+-rw-rw-r--   0 hamster   (1000) hamster   (1000)       65 2023-07-25 11:40:58.000000 quaxa-0.1.1/MANIFEST.in
+-rw-rw-r--   0 hamster   (1000) hamster   (1000)     6061 2023-08-08 20:04:12.775848 quaxa-0.1.1/PKG-INFO
+-rw-rw-r--   0 hamster   (1000) hamster   (1000)     5741 2023-07-25 11:49:14.000000 quaxa-0.1.1/README.md
+drwxrwxr-x   0 hamster   (1000) hamster   (1000)        0 2023-08-08 20:04:12.775848 quaxa-0.1.1/quaxa/
+-rw-rw-r--   0 hamster   (1000) hamster   (1000)      531 2023-08-08 20:02:10.000000 quaxa-0.1.1/quaxa/__init__.py
+-rw-rw-r--   0 hamster   (1000) hamster   (1000)    16040 2023-08-08 20:02:46.000000 quaxa-0.1.1/quaxa/quaxa.py
+drwxrwxr-x   0 hamster   (1000) hamster   (1000)        0 2023-08-08 20:04:12.775848 quaxa-0.1.1/quaxa.egg-info/
+-rw-rw-r--   0 hamster   (1000) hamster   (1000)     6061 2023-08-08 20:04:12.000000 quaxa-0.1.1/quaxa.egg-info/PKG-INFO
+-rw-rw-r--   0 hamster   (1000) hamster   (1000)      275 2023-08-08 20:04:12.000000 quaxa-0.1.1/quaxa.egg-info/SOURCES.txt
+-rw-rw-r--   0 hamster   (1000) hamster   (1000)        1 2023-08-08 20:04:12.000000 quaxa-0.1.1/quaxa.egg-info/dependency_links.txt
+-rw-rw-r--   0 hamster   (1000) hamster   (1000)       14 2023-08-08 20:04:12.000000 quaxa-0.1.1/quaxa.egg-info/requires.txt
+-rw-rw-r--   0 hamster   (1000) hamster   (1000)        6 2023-08-08 20:04:12.000000 quaxa-0.1.1/quaxa.egg-info/top_level.txt
+-rw-rw-r--   0 hamster   (1000) hamster   (1000)        1 2023-07-25 11:47:40.000000 quaxa-0.1.1/quaxa.egg-info/zip-safe
+-rw-rw-r--   0 hamster   (1000) hamster   (1000)       38 2023-08-08 20:04:12.775848 quaxa-0.1.1/setup.cfg
+-rw-rw-r--   0 hamster   (1000) hamster   (1000)      952 2023-07-25 11:40:58.000000 quaxa-0.1.1/setup.py
+drwxrwxr-x   0 hamster   (1000) hamster   (1000)        0 2023-08-08 20:04:12.775848 quaxa-0.1.1/test/
+-rw-rw-r--   0 hamster   (1000) hamster   (1000)        0 2023-07-25 11:40:58.000000 quaxa-0.1.1/test/__init__.py
+-rw-rw-r--   0 hamster   (1000) hamster   (1000)    19167 2023-07-25 11:40:58.000000 quaxa-0.1.1/test/test_quaxa.py
```

### Comparing `quaxa-0.1.0/LICENSE` & `quaxa-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `quaxa-0.1.0/PKG-INFO` & `quaxa-0.1.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 Metadata-Version: 2.1
 Name: quaxa
-Version: 0.1.0
+Version: 0.1.1
 Summary: QUAlity of sentence eXAmples scoring
 Home-page: http://github.com/ulf1/quaxa
 Author: Ulf Hamster
 Author-email: 554c46@gmail.com
 License: Apache License 2.0
 Platform: UNKNOWN
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 [![PyPI version](https://badge.fury.io/py/quaxa.svg)](https://badge.fury.io/py/quaxa)
 [![PyPi downloads](https://img.shields.io/pypi/dm/quaxa)](https://img.shields.io/pypi/dm/quaxa)
+[![DOI](https://zenodo.org/badge/667310199.svg)](https://zenodo.org/badge/latestdoi/667310199)
 
 # QUAXA: QUAlity of sentence eXAmples scoring
 Rule-based sentence scoring algorithm based on GDEX.
 
 
 ## Rules
```

### Comparing `quaxa-0.1.0/README.md` & `quaxa-0.1.1/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 [![PyPI version](https://badge.fury.io/py/quaxa.svg)](https://badge.fury.io/py/quaxa)
 [![PyPi downloads](https://img.shields.io/pypi/dm/quaxa)](https://img.shields.io/pypi/dm/quaxa)
+[![DOI](https://zenodo.org/badge/667310199.svg)](https://zenodo.org/badge/latestdoi/667310199)
 
 # QUAXA: QUAlity of sentence eXAmples scoring
 Rule-based sentence scoring algorithm based on GDEX.
 
 
 ## Rules
```

### Comparing `quaxa-0.1.0/quaxa/__init__.py` & `quaxa-0.1.1/quaxa/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = '0.1.0'
+__version__ = '0.1.1'
 
 from .quaxa import (
     total_score,
     isa_knockout_criteria,
     factor_gradual_criteria,
     has_finite_verb_and_subject,
     is_misparsed,
```

### Comparing `quaxa-0.1.0/quaxa/quaxa.py` & `quaxa-0.1.1/quaxa/quaxa.py`

 * *Files 1% similar despite different names*

```diff
@@ -93,15 +93,16 @@
 def has_finite_verb_and_subject(annotation: List[dict]) -> bool:
     """Has finite verb as root and subject as one of its children.
 
     It is a knockout criterion.
     """
     # find the root of the dependency tree
     root = [token for token in annotation if token['deprel'].lower() == 'root']
-    assert len(root) == 1
+    if len(root) != 1:
+        return False
     root = root[0]
     root_id = root['id']
 
     # find finite verb
     def is_finite_verb(tok):
         if tok.get('upos', '') in {'AUX', 'VERB'}:
             flag = tok.get('feats', '').get('VerbForm', '') == 'Fin'
```

### Comparing `quaxa-0.1.0/quaxa.egg-info/PKG-INFO` & `quaxa-0.1.1/quaxa.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 Metadata-Version: 2.1
 Name: quaxa
-Version: 0.1.0
+Version: 0.1.1
 Summary: QUAlity of sentence eXAmples scoring
 Home-page: http://github.com/ulf1/quaxa
 Author: Ulf Hamster
 Author-email: 554c46@gmail.com
 License: Apache License 2.0
 Platform: UNKNOWN
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 [![PyPI version](https://badge.fury.io/py/quaxa.svg)](https://badge.fury.io/py/quaxa)
 [![PyPi downloads](https://img.shields.io/pypi/dm/quaxa)](https://img.shields.io/pypi/dm/quaxa)
+[![DOI](https://zenodo.org/badge/667310199.svg)](https://zenodo.org/badge/latestdoi/667310199)
 
 # QUAXA: QUAlity of sentence eXAmples scoring
 Rule-based sentence scoring algorithm based on GDEX.
 
 
 ## Rules
```

### Comparing `quaxa-0.1.0/setup.py` & `quaxa-0.1.1/setup.py`

 * *Files identical despite different names*

### Comparing `quaxa-0.1.0/test/test_quaxa.py` & `quaxa-0.1.1/test/test_quaxa.py`

 * *Files identical despite different names*


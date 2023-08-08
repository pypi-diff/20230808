# Comparing `tmp/pyvoikko-0.4.tar.gz` & `tmp/pyvoikko-0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyvoikko-0.4.tar", last modified: Tue Jul 18 10:49:54 2023, max compression
+gzip compressed data, was "pyvoikko-0.5.tar", last modified: Tue Aug  8 11:45:25 2023, max compression
```

## Comparing `pyvoikko-0.4.tar` & `pyvoikko-0.5.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 iikka      (501) staff       (20)        0 2023-07-18 10:49:54.992191 pyvoikko-0.4/
--rw-r--r--   0 iikka      (501) staff       (20)    35140 2023-07-06 21:40:03.000000 pyvoikko-0.4/LICENSE
--rw-r--r--   0 iikka      (501) staff       (20)     1750 2023-07-18 10:49:54.992234 pyvoikko-0.4/PKG-INFO
--rw-r--r--   0 iikka      (501) staff       (20)     1098 2023-07-06 22:23:41.000000 pyvoikko-0.4/README.md
--rw-r--r--   0 iikka      (501) staff       (20)       81 2023-07-05 14:02:43.000000 pyvoikko-0.4/pyproject.toml
-drwxr-xr-x   0 iikka      (501) staff       (20)        0 2023-07-18 10:49:54.991098 pyvoikko-0.4/pyvoikko/
--rw-r--r--   0 iikka      (501) staff       (20)      594 2023-07-07 10:42:45.000000 pyvoikko-0.4/pyvoikko/__init__.py
--rw-r--r--   0 iikka      (501) staff       (20)     5329 2023-07-18 10:49:05.000000 pyvoikko-0.4/pyvoikko/analysis.py
--rw-r--r--   0 iikka      (501) staff       (20)     2010 2023-07-06 21:59:47.000000 pyvoikko-0.4/pyvoikko/constants.py
--rw-r--r--   0 iikka      (501) staff       (20)  1071442 2023-07-06 20:45:08.000000 pyvoikko-0.4/pyvoikko/voikko.kfst
-drwxr-xr-x   0 iikka      (501) staff       (20)        0 2023-07-18 10:49:54.992079 pyvoikko-0.4/pyvoikko.egg-info/
--rw-r--r--   0 iikka      (501) staff       (20)     1750 2023-07-18 10:49:54.000000 pyvoikko-0.4/pyvoikko.egg-info/PKG-INFO
--rw-r--r--   0 iikka      (501) staff       (20)      286 2023-07-18 10:49:54.000000 pyvoikko-0.4/pyvoikko.egg-info/SOURCES.txt
--rw-r--r--   0 iikka      (501) staff       (20)        1 2023-07-18 10:49:54.000000 pyvoikko-0.4/pyvoikko.egg-info/dependency_links.txt
--rw-r--r--   0 iikka      (501) staff       (20)        5 2023-07-18 10:49:54.000000 pyvoikko-0.4/pyvoikko.egg-info/requires.txt
--rw-r--r--   0 iikka      (501) staff       (20)        9 2023-07-18 10:49:54.000000 pyvoikko-0.4/pyvoikko.egg-info/top_level.txt
--rw-r--r--   0 iikka      (501) staff       (20)      816 2023-07-18 10:49:54.992446 pyvoikko-0.4/setup.cfg
+drwxr-xr-x   0 iikka      (501) staff       (20)        0 2023-08-08 11:45:25.109561 pyvoikko-0.5/
+-rw-r--r--   0 iikka      (501) staff       (20)    35140 2023-07-06 21:40:03.000000 pyvoikko-0.5/LICENSE
+-rw-r--r--   0 iikka      (501) staff       (20)     1750 2023-08-08 11:45:25.109602 pyvoikko-0.5/PKG-INFO
+-rw-r--r--   0 iikka      (501) staff       (20)     1098 2023-07-06 22:23:41.000000 pyvoikko-0.5/README.md
+-rw-r--r--   0 iikka      (501) staff       (20)       81 2023-07-05 14:02:43.000000 pyvoikko-0.5/pyproject.toml
+drwxr-xr-x   0 iikka      (501) staff       (20)        0 2023-08-08 11:45:25.107414 pyvoikko-0.5/pyvoikko/
+-rw-r--r--   0 iikka      (501) staff       (20)      681 2023-08-08 11:44:59.000000 pyvoikko-0.5/pyvoikko/__init__.py
+-rw-r--r--   0 iikka      (501) staff       (20)     5329 2023-07-18 10:49:05.000000 pyvoikko-0.5/pyvoikko/analysis.py
+-rw-r--r--   0 iikka      (501) staff       (20)     2010 2023-07-06 21:59:47.000000 pyvoikko-0.5/pyvoikko/constants.py
+-rw-r--r--   0 iikka      (501) staff       (20)  1071442 2023-07-06 20:45:08.000000 pyvoikko-0.5/pyvoikko/voikko.kfst
+drwxr-xr-x   0 iikka      (501) staff       (20)        0 2023-08-08 11:45:25.109482 pyvoikko-0.5/pyvoikko.egg-info/
+-rw-r--r--   0 iikka      (501) staff       (20)     1750 2023-08-08 11:45:25.000000 pyvoikko-0.5/pyvoikko.egg-info/PKG-INFO
+-rw-r--r--   0 iikka      (501) staff       (20)      286 2023-08-08 11:45:25.000000 pyvoikko-0.5/pyvoikko.egg-info/SOURCES.txt
+-rw-r--r--   0 iikka      (501) staff       (20)        1 2023-08-08 11:45:25.000000 pyvoikko-0.5/pyvoikko.egg-info/dependency_links.txt
+-rw-r--r--   0 iikka      (501) staff       (20)        5 2023-08-08 11:45:25.000000 pyvoikko-0.5/pyvoikko.egg-info/requires.txt
+-rw-r--r--   0 iikka      (501) staff       (20)        9 2023-08-08 11:45:25.000000 pyvoikko-0.5/pyvoikko.egg-info/top_level.txt
+-rw-r--r--   0 iikka      (501) staff       (20)      816 2023-08-08 11:45:25.109812 pyvoikko-0.5/setup.cfg
```

### Comparing `pyvoikko-0.4/LICENSE` & `pyvoikko-0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `pyvoikko-0.4/PKG-INFO` & `pyvoikko-0.5/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyvoikko
-Version: 0.4
+Version: 0.5
 Summary: A pure-python implementation of the Voikko library that provides Finnish morphological analysis
 Home-page: https://github.com/fergusq/fst-python
 Author: Iikka Hauhio
 Author-email: iikka.hauhio@helsinki.fi
 License: GNU GPLv3
 Project-URL: Bug Tracker, https://github.com/fergusq/fst-python/issues
 Keywords: finnish nlp morphology
```

### Comparing `pyvoikko-0.4/README.md` & `pyvoikko-0.5/README.md`

 * *Files identical despite different names*

### Comparing `pyvoikko-0.4/pyvoikko/__init__.py` & `pyvoikko-0.5/pyvoikko/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from __future__ import annotations
 
 import os.path
 
-from kfst import FST
+from kfst import FST, TokenizationException
 
 from .analysis import VoikkoAnalysis
 
 SCRIPT_DIR = os.path.dirname(os.path.realpath(__file__))
 
 VOIKKO_FST = FST.from_kfst_file(os.path.join(SCRIPT_DIR, "voikko.kfst"))
 
@@ -17,11 +17,14 @@
     Args:
         word: word to analyse
     
     Returns:
         list of `VoikkoAnalysis` objects
     """
     ans = []
-    for analysis, _weight in VOIKKO_FST.lookup(word):
-        ans.append(VoikkoAnalysis.from_voikko_analysis(analysis))
+    try:
+        for analysis, _weight in VOIKKO_FST.lookup(word):
+            ans.append(VoikkoAnalysis.from_voikko_analysis(analysis))
+    except TokenizationException:
+        pass
     
     return ans
```

### Comparing `pyvoikko-0.4/pyvoikko/analysis.py` & `pyvoikko-0.5/pyvoikko/analysis.py`

 * *Files identical despite different names*

### Comparing `pyvoikko-0.4/pyvoikko/constants.py` & `pyvoikko-0.5/pyvoikko/constants.py`

 * *Files identical despite different names*

### Comparing `pyvoikko-0.4/pyvoikko/voikko.kfst` & `pyvoikko-0.5/pyvoikko/voikko.kfst`

 * *Files identical despite different names*

### Comparing `pyvoikko-0.4/pyvoikko.egg-info/PKG-INFO` & `pyvoikko-0.5/pyvoikko.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyvoikko
-Version: 0.4
+Version: 0.5
 Summary: A pure-python implementation of the Voikko library that provides Finnish morphological analysis
 Home-page: https://github.com/fergusq/fst-python
 Author: Iikka Hauhio
 Author-email: iikka.hauhio@helsinki.fi
 License: GNU GPLv3
 Project-URL: Bug Tracker, https://github.com/fergusq/fst-python/issues
 Keywords: finnish nlp morphology
```

### Comparing `pyvoikko-0.4/setup.cfg` & `pyvoikko-0.5/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = pyvoikko
-version = 0.4
+version = 0.5
 author = Iikka Hauhio
 author_email = iikka.hauhio@helsinki.fi
 description = A pure-python implementation of the Voikko library that provides Finnish morphological analysis
 long_description = file: README.md
 long_description_content_type = text/markdown
 keywords = finnish nlp morphology
 license = GNU GPLv3
```


# Comparing `tmp/graphtage-0.2.9.tar.gz` & `tmp/graphtage-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "graphtage-0.2.9.tar", last modified: Wed Jun 28 13:13:41 2023, max compression
+gzip compressed data, was "graphtage-0.3.0.tar", last modified: Tue Aug  8 20:58:36 2023, max compression
```

## Comparing `graphtage-0.2.9.tar` & `graphtage-0.3.0.tar`

### file list

```diff
@@ -1,54 +1,54 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 13:13:41.725187 graphtage-0.2.9/
--rw-r--r--   0 runner    (1001) docker     (123)     7652 2023-06-28 13:13:29.000000 graphtage-0.2.9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-06-28 13:13:29.000000 graphtage-0.2.9/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     7718 2023-06-28 13:13:41.725187 graphtage-0.2.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6883 2023-06-28 13:13:29.000000 graphtage-0.2.9/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 13:13:41.725187 graphtage-0.2.9/graphtage/
--rw-r--r--   0 runner    (1001) docker     (123)     1012 2023-06-28 13:13:29.000000 graphtage-0.2.9/graphtage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14789 2023-06-28 13:13:29.000000 graphtage-0.2.9/graphtage/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15059 2023-06-28 13:13:29.000000 graphtage-0.2.9/graphtage/bounds.py
--rw-r--r--   0 runner    (1001) docker     (123)     1570 2023-06-28 13:13:29.000000 graphtage-0.2.9/graphtage/constraints.py
--rw-r--r--   0 runner    (1001) docker     (123)     5261 2023-06-28 13:13:29.000000 graphtage-0.2.9/graphtage/csv.py
--rw-r--r--   0 runner    (1001) docker     (123)    18505 2023-06-28 13:13:29.000000 graphtage-0.2.9/graphtage/edits.py
--rw-r--r--   0 runner    (1001) docker     (123)    30535 2023-06-28 13:13:29.000000 graphtage-0.2.9/graphtage/expressions.py
--rw-r--r--   0 runner    (1001) docker     (123)    11969 2023-06-28 13:13:29.000000 graphtage-0.2.9/graphtage/fibonacci.py
--rw-r--r--   0 runner    (1001) docker     (123)    16882 2023-06-28 13:13:29.000000 graphtage-0.2.9/graphtage/formatter.py
--rw-r--r--   0 runner    (1001) docker     (123)    37993 2023-06-28 13:13:29.000000 graphtage-0.2.9/graphtage/graphtage.py
--rw-r--r--   0 runner    (1001) docker     (123)     9933 2023-06-28 13:13:29.000000 graphtage-0.2.9/graphtage/json.py
--rw-r--r--   0 runner    (1001) docker     (123)    16443 2023-06-28 13:13:29.000000 graphtage-0.2.9/graphtage/levenshtein.py
--rw-r--r--   0 runner    (1001) docker     (123)    28141 2023-06-28 13:13:29.000000 graphtage-0.2.9/graphtage/matching.py
--rw-r--r--   0 runner    (1001) docker     (123)     5498 2023-06-28 13:13:29.000000 graphtage-0.2.9/graphtage/multiset.py
--rw-r--r--   0 runner    (1001) docker     (123)     5617 2023-06-28 13:13:29.000000 graphtage-0.2.9/graphtage/plist.py
--rw-r--r--   0 runner    (1001) docker     (123)    22582 2023-06-28 13:13:29.000000 graphtage-0.2.9/graphtage/printer.py
--rw-r--r--   0 runner    (1001) docker     (123)     6020 2023-06-28 13:13:29.000000 graphtage-0.2.9/graphtage/progress.py
--rw-r--r--   0 runner    (1001) docker     (123)    10319 2023-06-28 13:13:29.000000 graphtage-0.2.9/graphtage/pydiff.py
--rw-r--r--   0 runner    (1001) docker     (123)    11128 2023-06-28 13:13:29.000000 graphtage-0.2.9/graphtage/search.py
--rw-r--r--   0 runner    (1001) docker     (123)    12812 2023-06-28 13:13:29.000000 graphtage-0.2.9/graphtage/sequences.py
--rw-r--r--   0 runner    (1001) docker     (123)    24417 2023-06-28 13:13:29.000000 graphtage-0.2.9/graphtage/tree.py
--rw-r--r--   0 runner    (1001) docker     (123)    14573 2023-06-28 13:13:29.000000 graphtage-0.2.9/graphtage/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2844 2023-06-28 13:13:29.000000 graphtage-0.2.9/graphtage/version.py
--rw-r--r--   0 runner    (1001) docker     (123)    16277 2023-06-28 13:13:29.000000 graphtage-0.2.9/graphtage/xml.py
--rw-r--r--   0 runner    (1001) docker     (123)     8391 2023-06-28 13:13:29.000000 graphtage-0.2.9/graphtage/yaml.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 13:13:41.725187 graphtage-0.2.9/graphtage.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7718 2023-06-28 13:13:41.000000 graphtage-0.2.9/graphtage.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1042 2023-06-28 13:13:41.000000 graphtage-0.2.9/graphtage.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-28 13:13:41.000000 graphtage-0.2.9/graphtage.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-06-28 13:13:41.000000 graphtage-0.2.9/graphtage.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      211 2023-06-28 13:13:41.000000 graphtage-0.2.9/graphtage.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-28 13:13:41.000000 graphtage-0.2.9/graphtage.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-28 13:13:41.725187 graphtage-0.2.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2131 2023-06-28 13:13:29.000000 graphtage-0.2.9/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 13:13:41.725187 graphtage-0.2.9/test/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-28 13:13:29.000000 graphtage-0.2.9/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4307 2023-06-28 13:13:29.000000 graphtage-0.2.9/test/test_bounds.py
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-06-28 13:13:29.000000 graphtage-0.2.9/test/test_constraints.py
--rw-r--r--   0 runner    (1001) docker     (123)     2469 2023-06-28 13:13:29.000000 graphtage-0.2.9/test/test_expressions.py
--rw-r--r--   0 runner    (1001) docker     (123)     4161 2023-06-28 13:13:29.000000 graphtage-0.2.9/test/test_fibonacci.py
--rw-r--r--   0 runner    (1001) docker     (123)    10748 2023-06-28 13:13:29.000000 graphtage-0.2.9/test/test_formatting.py
--rw-r--r--   0 runner    (1001) docker     (123)     6887 2023-06-28 13:13:29.000000 graphtage-0.2.9/test/test_graphtage.py
--rw-r--r--   0 runner    (1001) docker     (123)     2978 2023-06-28 13:13:29.000000 graphtage-0.2.9/test/test_levenshtein.py
--rw-r--r--   0 runner    (1001) docker     (123)     3151 2023-06-28 13:13:29.000000 graphtage-0.2.9/test/test_matching.py
--rw-r--r--   0 runner    (1001) docker     (123)      831 2023-06-28 13:13:29.000000 graphtage-0.2.9/test/test_pydiff.py
--rw-r--r--   0 runner    (1001) docker     (123)     1475 2023-06-28 13:13:29.000000 graphtage-0.2.9/test/test_search.py
--rw-r--r--   0 runner    (1001) docker     (123)     1835 2023-06-28 13:13:29.000000 graphtage-0.2.9/test/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      755 2023-06-28 13:13:29.000000 graphtage-0.2.9/test/test_xml.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 20:58:36.710697 graphtage-0.3.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     7652 2023-08-08 20:58:28.000000 graphtage-0.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-08-08 20:58:28.000000 graphtage-0.3.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     7708 2023-08-08 20:58:36.710697 graphtage-0.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6873 2023-08-08 20:58:28.000000 graphtage-0.3.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 20:58:36.710697 graphtage-0.3.0/graphtage/
+-rw-r--r--   0 runner    (1001) docker     (123)     1012 2023-08-08 20:58:28.000000 graphtage-0.3.0/graphtage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14789 2023-08-08 20:58:28.000000 graphtage-0.3.0/graphtage/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15059 2023-08-08 20:58:28.000000 graphtage-0.3.0/graphtage/bounds.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1570 2023-08-08 20:58:28.000000 graphtage-0.3.0/graphtage/constraints.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5261 2023-08-08 20:58:28.000000 graphtage-0.3.0/graphtage/csv.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18505 2023-08-08 20:58:28.000000 graphtage-0.3.0/graphtage/edits.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30535 2023-08-08 20:58:28.000000 graphtage-0.3.0/graphtage/expressions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11969 2023-08-08 20:58:28.000000 graphtage-0.3.0/graphtage/fibonacci.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16882 2023-08-08 20:58:28.000000 graphtage-0.3.0/graphtage/formatter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37993 2023-08-08 20:58:28.000000 graphtage-0.3.0/graphtage/graphtage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9933 2023-08-08 20:58:28.000000 graphtage-0.3.0/graphtage/json.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16443 2023-08-08 20:58:28.000000 graphtage-0.3.0/graphtage/levenshtein.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28141 2023-08-08 20:58:28.000000 graphtage-0.3.0/graphtage/matching.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5498 2023-08-08 20:58:28.000000 graphtage-0.3.0/graphtage/multiset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5617 2023-08-08 20:58:28.000000 graphtage-0.3.0/graphtage/plist.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22582 2023-08-08 20:58:28.000000 graphtage-0.3.0/graphtage/printer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6020 2023-08-08 20:58:28.000000 graphtage-0.3.0/graphtage/progress.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10305 2023-08-08 20:58:28.000000 graphtage-0.3.0/graphtage/pydiff.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11128 2023-08-08 20:58:28.000000 graphtage-0.3.0/graphtage/search.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12812 2023-08-08 20:58:28.000000 graphtage-0.3.0/graphtage/sequences.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24417 2023-08-08 20:58:28.000000 graphtage-0.3.0/graphtage/tree.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14573 2023-08-08 20:58:28.000000 graphtage-0.3.0/graphtage/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2844 2023-08-08 20:58:28.000000 graphtage-0.3.0/graphtage/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16277 2023-08-08 20:58:28.000000 graphtage-0.3.0/graphtage/xml.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8391 2023-08-08 20:58:28.000000 graphtage-0.3.0/graphtage/yaml.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 20:58:36.710697 graphtage-0.3.0/graphtage.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7708 2023-08-08 20:58:36.000000 graphtage-0.3.0/graphtage.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1042 2023-08-08 20:58:36.000000 graphtage-0.3.0/graphtage.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 20:58:36.000000 graphtage-0.3.0/graphtage.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-08-08 20:58:36.000000 graphtage-0.3.0/graphtage.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      211 2023-08-08 20:58:36.000000 graphtage-0.3.0/graphtage.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-08-08 20:58:36.000000 graphtage-0.3.0/graphtage.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-08 20:58:36.710697 graphtage-0.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2131 2023-08-08 20:58:28.000000 graphtage-0.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 20:58:36.710697 graphtage-0.3.0/test/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 20:58:28.000000 graphtage-0.3.0/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4307 2023-08-08 20:58:28.000000 graphtage-0.3.0/test/test_bounds.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-08-08 20:58:28.000000 graphtage-0.3.0/test/test_constraints.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2469 2023-08-08 20:58:28.000000 graphtage-0.3.0/test/test_expressions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4161 2023-08-08 20:58:28.000000 graphtage-0.3.0/test/test_fibonacci.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10748 2023-08-08 20:58:28.000000 graphtage-0.3.0/test/test_formatting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6887 2023-08-08 20:58:28.000000 graphtage-0.3.0/test/test_graphtage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2978 2023-08-08 20:58:28.000000 graphtage-0.3.0/test/test_levenshtein.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3151 2023-08-08 20:58:28.000000 graphtage-0.3.0/test/test_matching.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1256 2023-08-08 20:58:28.000000 graphtage-0.3.0/test/test_pydiff.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1475 2023-08-08 20:58:28.000000 graphtage-0.3.0/test/test_search.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1835 2023-08-08 20:58:28.000000 graphtage-0.3.0/test/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      755 2023-08-08 20:58:28.000000 graphtage-0.3.0/test/test_xml.py
```

### Comparing `graphtage-0.2.9/LICENSE` & `graphtage-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `graphtage-0.2.9/PKG-INFO` & `graphtage-0.3.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: graphtage
-Version: 0.2.9
+Version: 0.3.0
 Summary: A utility to diff tree-like files such as JSON and XML.
 Home-page: https://github.com/trailofbits/graphtage
 Author: Trail of Bits
 License: LGPL-3.0-or-later
 Project-URL: Documentation, https://trailofbits.github.io/graphtage
 Project-URL: Source, https://github.com/trailofbits/graphtage
 Project-URL: Tracker, https://github.com/trailofbits/graphtage/issues
@@ -19,15 +19,15 @@
 Provides-Extra: dev
 License-File: LICENSE
 
 # Graphtage
 
 [![PyPI version](https://badge.fury.io/py/graphtage.svg)](https://badge.fury.io/py/graphtage)
 [![Tests](https://github.com/trailofbits/graphtage/workflows/Python%20package/badge.svg)](https://github.com/trailofbits/graphtage/actions)
-[![Slack Status](https://empireslacking.herokuapp.com/badge.svg)](https://empireslacking.herokuapp.com)
+[![Slack Status](https://slack.empirehacking.nyc/badge.svg)](https://slack.empirehacking.nyc)
 
 Graphtage is a command-line utility and [underlying library](https://trailofbits.github.io/graphtage/latest/library.html)
 for semantically comparing and merging tree-like structures, such as JSON, XML, HTML, YAML, plist, and CSS files. Its name is a
 portmanteau of “graph” and “graftage”—the latter being the horticultural practice of joining two trees together such
 that they grow as one.
 
 ```console
```

### Comparing `graphtage-0.2.9/README.md` & `graphtage-0.3.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # Graphtage
 
 [![PyPI version](https://badge.fury.io/py/graphtage.svg)](https://badge.fury.io/py/graphtage)
 [![Tests](https://github.com/trailofbits/graphtage/workflows/Python%20package/badge.svg)](https://github.com/trailofbits/graphtage/actions)
-[![Slack Status](https://empireslacking.herokuapp.com/badge.svg)](https://empireslacking.herokuapp.com)
+[![Slack Status](https://slack.empirehacking.nyc/badge.svg)](https://slack.empirehacking.nyc)
 
 Graphtage is a command-line utility and [underlying library](https://trailofbits.github.io/graphtage/latest/library.html)
 for semantically comparing and merging tree-like structures, such as JSON, XML, HTML, YAML, plist, and CSS files. Its name is a
 portmanteau of “graph” and “graftage”—the latter being the horticultural practice of joining two trees together such
 that they grow as one.
 
 ```console
```

### Comparing `graphtage-0.2.9/graphtage/__init__.py` & `graphtage-0.3.0/graphtage/__init__.py`

 * *Files identical despite different names*

### Comparing `graphtage-0.2.9/graphtage/__main__.py` & `graphtage-0.3.0/graphtage/__main__.py`

 * *Files identical despite different names*

### Comparing `graphtage-0.2.9/graphtage/bounds.py` & `graphtage-0.3.0/graphtage/bounds.py`

 * *Files identical despite different names*

### Comparing `graphtage-0.2.9/graphtage/constraints.py` & `graphtage-0.3.0/graphtage/constraints.py`

 * *Files identical despite different names*

### Comparing `graphtage-0.2.9/graphtage/csv.py` & `graphtage-0.3.0/graphtage/csv.py`

 * *Files identical despite different names*

### Comparing `graphtage-0.2.9/graphtage/edits.py` & `graphtage-0.3.0/graphtage/edits.py`

 * *Files identical despite different names*

### Comparing `graphtage-0.2.9/graphtage/expressions.py` & `graphtage-0.3.0/graphtage/expressions.py`

 * *Files identical despite different names*

### Comparing `graphtage-0.2.9/graphtage/fibonacci.py` & `graphtage-0.3.0/graphtage/fibonacci.py`

 * *Files identical despite different names*

### Comparing `graphtage-0.2.9/graphtage/formatter.py` & `graphtage-0.3.0/graphtage/formatter.py`

 * *Files identical despite different names*

### Comparing `graphtage-0.2.9/graphtage/graphtage.py` & `graphtage-0.3.0/graphtage/graphtage.py`

 * *Files identical despite different names*

### Comparing `graphtage-0.2.9/graphtage/json.py` & `graphtage-0.3.0/graphtage/json.py`

 * *Files identical despite different names*

### Comparing `graphtage-0.2.9/graphtage/levenshtein.py` & `graphtage-0.3.0/graphtage/levenshtein.py`

 * *Files identical despite different names*

### Comparing `graphtage-0.2.9/graphtage/matching.py` & `graphtage-0.3.0/graphtage/matching.py`

 * *Files identical despite different names*

### Comparing `graphtage-0.2.9/graphtage/multiset.py` & `graphtage-0.3.0/graphtage/multiset.py`

 * *Files identical despite different names*

### Comparing `graphtage-0.2.9/graphtage/plist.py` & `graphtage-0.3.0/graphtage/plist.py`

 * *Files identical despite different names*

### Comparing `graphtage-0.2.9/graphtage/printer.py` & `graphtage-0.3.0/graphtage/printer.py`

 * *Files identical despite different names*

### Comparing `graphtage-0.2.9/graphtage/progress.py` & `graphtage-0.3.0/graphtage/progress.py`

 * *Files identical despite different names*

### Comparing `graphtage-0.2.9/graphtage/pydiff.py` & `graphtage-0.3.0/graphtage/pydiff.py`

 * *Files 0% similar despite different names*

```diff
@@ -208,17 +208,17 @@
                 new_node = ListNode(map(IntegerNode, obj))
         elif isinstance(obj, DictValue):
             stack.append((obj, [], [obj.value, obj.key]))
         elif isinstance(obj, PyObjMember):
             stack.append((obj, [], [obj.value]))
         elif isinstance(obj, dict):
             stack.append(({}, [], [DictValue(key=k, value=v) for k, v in reversed(list(obj.items()))]))
-        elif isinstance(python_obj, (list, tuple)):
+        elif isinstance(obj, (list, tuple)):
             stack.append(([], [], list(reversed(obj))))
-        elif python_obj is None:
+        elif obj is None:
             new_node = NullNode()
         else:
             pyobj = PyObj(class_name=StringNode(obj.__class__.__name__, quoted=False), attrs=None)  # type: ignore
             stack.append((pyobj, [], [
                 PyObjMember(attr=attr, value=getattr(obj, attr))
                 for attr in reversed(dir(obj))
                 if not attr.startswith("__")
```

### Comparing `graphtage-0.2.9/graphtage/search.py` & `graphtage-0.3.0/graphtage/search.py`

 * *Files identical despite different names*

### Comparing `graphtage-0.2.9/graphtage/sequences.py` & `graphtage-0.3.0/graphtage/sequences.py`

 * *Files identical despite different names*

### Comparing `graphtage-0.2.9/graphtage/tree.py` & `graphtage-0.3.0/graphtage/tree.py`

 * *Files identical despite different names*

### Comparing `graphtage-0.2.9/graphtage/utils.py` & `graphtage-0.3.0/graphtage/utils.py`

 * *Files identical despite different names*

### Comparing `graphtage-0.2.9/graphtage/version.py` & `graphtage-0.3.0/graphtage/version.py`

 * *Files 0% similar despite different names*

```diff
@@ -55,15 +55,15 @@
 deploying to PyPI.
 
 If :const:`True`, the git branch will be included in the version string.
 
 """
 
 
-__version__: Tuple[Union[int, str], ...] = (0, 2, 9)
+__version__: Tuple[Union[int, str], ...] = (0, 3, 0)
 
 if DEV_BUILD:
     branch_name = git_branch()
     if branch_name is None:
         __version__ = __version__ + ('git',)
     else:
         __version__ = __version__ + ('git', branch_name)
```

### Comparing `graphtage-0.2.9/graphtage/xml.py` & `graphtage-0.3.0/graphtage/xml.py`

 * *Files identical despite different names*

### Comparing `graphtage-0.2.9/graphtage/yaml.py` & `graphtage-0.3.0/graphtage/yaml.py`

 * *Files identical despite different names*

### Comparing `graphtage-0.2.9/graphtage.egg-info/PKG-INFO` & `graphtage-0.3.0/graphtage.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: graphtage
-Version: 0.2.9
+Version: 0.3.0
 Summary: A utility to diff tree-like files such as JSON and XML.
 Home-page: https://github.com/trailofbits/graphtage
 Author: Trail of Bits
 License: LGPL-3.0-or-later
 Project-URL: Documentation, https://trailofbits.github.io/graphtage
 Project-URL: Source, https://github.com/trailofbits/graphtage
 Project-URL: Tracker, https://github.com/trailofbits/graphtage/issues
@@ -19,15 +19,15 @@
 Provides-Extra: dev
 License-File: LICENSE
 
 # Graphtage
 
 [![PyPI version](https://badge.fury.io/py/graphtage.svg)](https://badge.fury.io/py/graphtage)
 [![Tests](https://github.com/trailofbits/graphtage/workflows/Python%20package/badge.svg)](https://github.com/trailofbits/graphtage/actions)
-[![Slack Status](https://empireslacking.herokuapp.com/badge.svg)](https://empireslacking.herokuapp.com)
+[![Slack Status](https://slack.empirehacking.nyc/badge.svg)](https://slack.empirehacking.nyc)
 
 Graphtage is a command-line utility and [underlying library](https://trailofbits.github.io/graphtage/latest/library.html)
 for semantically comparing and merging tree-like structures, such as JSON, XML, HTML, YAML, plist, and CSS files. Its name is a
 portmanteau of “graph” and “graftage”—the latter being the horticultural practice of joining two trees together such
 that they grow as one.
 
 ```console
```

### Comparing `graphtage-0.2.9/graphtage.egg-info/SOURCES.txt` & `graphtage-0.3.0/graphtage.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `graphtage-0.2.9/setup.py` & `graphtage-0.3.0/setup.py`

 * *Files identical despite different names*

### Comparing `graphtage-0.2.9/test/test_bounds.py` & `graphtage-0.3.0/test/test_bounds.py`

 * *Files identical despite different names*

### Comparing `graphtage-0.2.9/test/test_constraints.py` & `graphtage-0.3.0/test/test_constraints.py`

 * *Files identical despite different names*

### Comparing `graphtage-0.2.9/test/test_expressions.py` & `graphtage-0.3.0/test/test_expressions.py`

 * *Files identical despite different names*

### Comparing `graphtage-0.2.9/test/test_fibonacci.py` & `graphtage-0.3.0/test/test_fibonacci.py`

 * *Files identical despite different names*

### Comparing `graphtage-0.2.9/test/test_formatting.py` & `graphtage-0.3.0/test/test_formatting.py`

 * *Files identical despite different names*

### Comparing `graphtage-0.2.9/test/test_graphtage.py` & `graphtage-0.3.0/test/test_graphtage.py`

 * *Files identical despite different names*

### Comparing `graphtage-0.2.9/test/test_levenshtein.py` & `graphtage-0.3.0/test/test_levenshtein.py`

 * *Files identical despite different names*

### Comparing `graphtage-0.2.9/test/test_matching.py` & `graphtage-0.3.0/test/test_matching.py`

 * *Files identical despite different names*

### Comparing `graphtage-0.2.9/test/test_search.py` & `graphtage-0.3.0/test/test_search.py`

 * *Files identical despite different names*

### Comparing `graphtage-0.2.9/test/test_utils.py` & `graphtage-0.3.0/test/test_utils.py`

 * *Files identical despite different names*

### Comparing `graphtage-0.2.9/test/test_xml.py` & `graphtage-0.3.0/test/test_xml.py`

 * *Files identical despite different names*


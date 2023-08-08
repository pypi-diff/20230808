# Comparing `tmp/sqlwhat-3.9.1.tar.gz` & `tmp/sqlwhat-3.9.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/sqlwhat-3.9.1.tar", last modified: Thu Jul 27 14:26:30 2023, max compression
+gzip compressed data, was "dist/sqlwhat-3.9.3.tar", last modified: Tue Aug  8 12:36:09 2023, max compression
```

## Comparing `sqlwhat-3.9.1.tar` & `sqlwhat-3.9.3.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-07-27 14:26:30.000000 sqlwhat-3.9.1/
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-07-27 14:26:30.000000 sqlwhat-3.9.1/sqlwhat/
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-07-27 14:26:30.000000 sqlwhat-3.9.1/sqlwhat/checks/
--rw-r--r--   0 circleci  (3434) circleci  (3434)      674 2023-07-27 14:26:29.000000 sqlwhat-3.9.1/sqlwhat/checks/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    12948 2023-07-27 14:26:29.000000 sqlwhat-3.9.1/sqlwhat/checks/check_funcs.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     7787 2023-07-27 14:26:29.000000 sqlwhat-3.9.1/sqlwhat/checks/has_funcs.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1589 2023-07-27 14:26:29.000000 sqlwhat-3.9.1/sqlwhat/State.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)       64 2023-07-27 14:26:29.000000 sqlwhat-3.9.1/sqlwhat/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      516 2023-07-27 14:26:29.000000 sqlwhat-3.9.1/sqlwhat/sct_syntax.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      973 2023-07-27 14:26:29.000000 sqlwhat-3.9.1/sqlwhat/test_exercise.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-07-27 14:26:30.000000 sqlwhat-3.9.1/sqlwhat.egg-info/
--rw-r--r--   0 circleci  (3434) circleci  (3434)     4027 2023-07-27 14:26:30.000000 sqlwhat-3.9.1/sqlwhat.egg-info/PKG-INFO
--rw-r--r--   0 circleci  (3434) circleci  (3434)      378 2023-07-27 14:26:30.000000 sqlwhat-3.9.1/sqlwhat.egg-info/SOURCES.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)        1 2023-07-27 14:26:30.000000 sqlwhat-3.9.1/sqlwhat.egg-info/dependency_links.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)       56 2023-07-27 14:26:30.000000 sqlwhat-3.9.1/sqlwhat.egg-info/requires.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)        8 2023-07-27 14:26:30.000000 sqlwhat-3.9.1/sqlwhat.egg-info/top_level.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)    34523 2023-07-27 14:26:29.000000 sqlwhat-3.9.1/LICENSE
--rw-r--r--   0 circleci  (3434) circleci  (3434)       41 2023-07-27 14:26:29.000000 sqlwhat-3.9.1/MANIFEST.in
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2717 2023-07-27 14:26:29.000000 sqlwhat-3.9.1/README.md
--rw-r--r--   0 circleci  (3434) circleci  (3434)      158 2023-07-27 14:26:29.000000 sqlwhat-3.9.1/requirements.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1658 2023-07-27 14:26:29.000000 sqlwhat-3.9.1/setup.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     4027 2023-07-27 14:26:30.000000 sqlwhat-3.9.1/PKG-INFO
--rw-r--r--   0 circleci  (3434) circleci  (3434)       38 2023-07-27 14:26:30.000000 sqlwhat-3.9.1/setup.cfg
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-08-08 12:36:09.000000 sqlwhat-3.9.3/
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-08-08 12:36:09.000000 sqlwhat-3.9.3/sqlwhat/
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-08-08 12:36:09.000000 sqlwhat-3.9.3/sqlwhat/checks/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      674 2023-08-08 12:36:09.000000 sqlwhat-3.9.3/sqlwhat/checks/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    12948 2023-08-08 12:36:09.000000 sqlwhat-3.9.3/sqlwhat/checks/check_funcs.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     7787 2023-08-08 12:36:09.000000 sqlwhat-3.9.3/sqlwhat/checks/has_funcs.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1656 2023-08-08 12:36:09.000000 sqlwhat-3.9.3/sqlwhat/State.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       64 2023-08-08 12:36:09.000000 sqlwhat-3.9.3/sqlwhat/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      516 2023-08-08 12:36:09.000000 sqlwhat-3.9.3/sqlwhat/sct_syntax.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      973 2023-08-08 12:36:09.000000 sqlwhat-3.9.3/sqlwhat/test_exercise.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-08-08 12:36:09.000000 sqlwhat-3.9.3/sqlwhat.egg-info/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     4027 2023-08-08 12:36:09.000000 sqlwhat-3.9.3/sqlwhat.egg-info/PKG-INFO
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      378 2023-08-08 12:36:09.000000 sqlwhat-3.9.3/sqlwhat.egg-info/SOURCES.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        1 2023-08-08 12:36:09.000000 sqlwhat-3.9.3/sqlwhat.egg-info/dependency_links.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       56 2023-08-08 12:36:09.000000 sqlwhat-3.9.3/sqlwhat.egg-info/requires.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        8 2023-08-08 12:36:09.000000 sqlwhat-3.9.3/sqlwhat.egg-info/top_level.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    34523 2023-08-08 12:36:09.000000 sqlwhat-3.9.3/LICENSE
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       41 2023-08-08 12:36:09.000000 sqlwhat-3.9.3/MANIFEST.in
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2717 2023-08-08 12:36:09.000000 sqlwhat-3.9.3/README.md
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      158 2023-08-08 12:36:09.000000 sqlwhat-3.9.3/requirements.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1658 2023-08-08 12:36:09.000000 sqlwhat-3.9.3/setup.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     4027 2023-08-08 12:36:09.000000 sqlwhat-3.9.3/PKG-INFO
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       38 2023-08-08 12:36:09.000000 sqlwhat-3.9.3/setup.cfg
```

### Comparing `sqlwhat-3.9.1/sqlwhat/checks/__init__.py` & `sqlwhat-3.9.3/sqlwhat/checks/__init__.py`

 * *Files identical despite different names*

### Comparing `sqlwhat-3.9.1/sqlwhat/checks/check_funcs.py` & `sqlwhat-3.9.3/sqlwhat/checks/check_funcs.py`

 * *Files identical despite different names*

### Comparing `sqlwhat-3.9.1/sqlwhat/checks/has_funcs.py` & `sqlwhat-3.9.3/sqlwhat/checks/has_funcs.py`

 * *Files identical despite different names*

### Comparing `sqlwhat-3.9.1/sqlwhat/State.py` & `sqlwhat-3.9.3/sqlwhat/State.py`

 * *Files 9% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 
 PARSER_MODULES = {
     "postgresql": "antlr_plsql.ast",
     "sqlite": "antlr_plsql.ast",  # uses postgres parser for now
     "oracle": "antlr_plsql.ast",  # uses postgres parser for now
     "mssql": "antlr_tsql.ast",
     "snowflake": "antlr_plsql.ast",  # uses postgres parser for now
+    "bigquery": "antlr_plsql.ast",  # uses postgres parser for now
 }
 
 
 def lower_case(f):
     """Decorator specifically for turning mssql AST into lowercase"""
     # if it has already been wrapped, we return original
     if hasattr(f, "lower_cased"):
```

### Comparing `sqlwhat-3.9.1/sqlwhat/sct_syntax.py` & `sqlwhat-3.9.3/sqlwhat/sct_syntax.py`

 * *Files identical despite different names*

### Comparing `sqlwhat-3.9.1/sqlwhat/test_exercise.py` & `sqlwhat-3.9.3/sqlwhat/test_exercise.py`

 * *Files identical despite different names*

### Comparing `sqlwhat-3.9.1/sqlwhat.egg-info/PKG-INFO` & `sqlwhat-3.9.3/sqlwhat.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sqlwhat
-Version: 3.9.1
+Version: 3.9.3
 Summary: Submission correctness tests for SQL
 Home-page: https://github.com/datacamp/sqlwhat
 Author: Michael Chow, Filip Schouwenaars
 Author-email: michael@datacamp.com
 Maintainer: Jeroen Hermans
 Maintainer-email: content-engineering@datacamp.com
 License: UNKNOWN
```

### Comparing `sqlwhat-3.9.1/LICENSE` & `sqlwhat-3.9.3/LICENSE`

 * *Files identical despite different names*

### Comparing `sqlwhat-3.9.1/README.md` & `sqlwhat-3.9.3/README.md`

 * *Files identical despite different names*

### Comparing `sqlwhat-3.9.1/setup.py` & `sqlwhat-3.9.3/setup.py`

 * *Files identical despite different names*

### Comparing `sqlwhat-3.9.1/PKG-INFO` & `sqlwhat-3.9.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sqlwhat
-Version: 3.9.1
+Version: 3.9.3
 Summary: Submission correctness tests for SQL
 Home-page: https://github.com/datacamp/sqlwhat
 Author: Michael Chow, Filip Schouwenaars
 Author-email: michael@datacamp.com
 Maintainer: Jeroen Hermans
 Maintainer-email: content-engineering@datacamp.com
 License: UNKNOWN
```


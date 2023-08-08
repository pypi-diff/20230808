# Comparing `tmp/leetquery-0.1.15.tar.gz` & `tmp/leetquery-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "leetquery-0.1.15.tar", last modified: Tue Aug  8 14:24:28 2023, max compression
+gzip compressed data, was "leetquery-0.1.5.tar", last modified: Mon Aug  7 14:31:24 2023, max compression
```

## Comparing `leetquery-0.1.15.tar` & `leetquery-0.1.5.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 14:24:28.897881 leetquery-0.1.15/
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-08-08 14:24:13.000000 leetquery-0.1.15/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      861 2023-08-08 14:24:28.897881 leetquery-0.1.15/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      384 2023-08-08 14:24:13.000000 leetquery-0.1.15/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 14:24:28.893881 leetquery-0.1.15/leetquery/
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-08-08 14:24:13.000000 leetquery-0.1.15/leetquery/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-08-08 14:24:13.000000 leetquery-0.1.15/leetquery/__version__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1009 2023-08-08 14:24:13.000000 leetquery-0.1.15/leetquery/user.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 14:24:28.893881 leetquery-0.1.15/leetquery.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      861 2023-08-08 14:24:28.000000 leetquery-0.1.15/leetquery.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      274 2023-08-08 14:24:28.000000 leetquery-0.1.15/leetquery.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 14:24:28.000000 leetquery-0.1.15/leetquery.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-08-08 14:24:28.000000 leetquery-0.1.15/leetquery.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-08-08 14:24:28.000000 leetquery-0.1.15/leetquery.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-08 14:24:28.897881 leetquery-0.1.15/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3848 2023-08-08 14:24:13.000000 leetquery-0.1.15/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 14:24:28.893881 leetquery-0.1.15/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      174 2023-08-08 14:24:13.000000 leetquery-0.1.15/tests/test_user.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 14:31:24.568527 leetquery-0.1.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-08-07 14:31:13.000000 leetquery-0.1.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      821 2023-08-07 14:31:24.568527 leetquery-0.1.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      340 2023-08-07 14:31:13.000000 leetquery-0.1.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 14:31:24.568527 leetquery-0.1.5/leetquery/
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-08-07 14:31:13.000000 leetquery-0.1.5/leetquery/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-08-07 14:31:13.000000 leetquery-0.1.5/leetquery/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1009 2023-08-07 14:31:13.000000 leetquery-0.1.5/leetquery/user.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 14:31:24.568527 leetquery-0.1.5/leetquery.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      821 2023-08-07 14:31:24.000000 leetquery-0.1.5/leetquery.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      274 2023-08-07 14:31:24.000000 leetquery-0.1.5/leetquery.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-07 14:31:24.000000 leetquery-0.1.5/leetquery.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-08-07 14:31:24.000000 leetquery-0.1.5/leetquery.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-08-07 14:31:24.000000 leetquery-0.1.5/leetquery.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-07 14:31:24.568527 leetquery-0.1.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3853 2023-08-07 14:31:13.000000 leetquery-0.1.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 14:31:24.568527 leetquery-0.1.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      171 2023-08-07 14:31:13.000000 leetquery-0.1.5/tests/test_user.py
```

### Comparing `leetquery-0.1.15/LICENSE` & `leetquery-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `leetquery-0.1.15/PKG-INFO` & `leetquery-0.1.5/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: leetquery
-Version: 0.1.15
+Version: 0.1.5
 Summary: Query and analyze data from leetcode
-Home-page: https://github.com/ShuYuHuang/leetquery
+Home-page: https://github.com/ShuYuHuang/leetcode-query
 Author: Shu-Yu Huang
 Author-email: b123767195@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7.0
@@ -20,17 +20,16 @@
 
 ## Install
 ``` shell
     pip install leetquery
 ```
 ## Usage
 ### Retriving User Submissions
-Just enter user name and limit of query!
 ``` python
 from leetquery import get_submissions
 
-submissions = get_submissions(username="syhaung", limits=12)
+submissions = get_submissions(username="syhaung", limits)
 ```
 return value:
 ```
 ["question1", "question2", ...]
 ```
```

### Comparing `leetquery-0.1.15/leetquery/user.py` & `leetquery-0.1.5/leetquery/user.py`

 * *Files identical despite different names*

### Comparing `leetquery-0.1.15/leetquery.egg-info/PKG-INFO` & `leetquery-0.1.5/leetquery.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: leetquery
-Version: 0.1.15
+Version: 0.1.5
 Summary: Query and analyze data from leetcode
-Home-page: https://github.com/ShuYuHuang/leetquery
+Home-page: https://github.com/ShuYuHuang/leetcode-query
 Author: Shu-Yu Huang
 Author-email: b123767195@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7.0
@@ -20,17 +20,16 @@
 
 ## Install
 ``` shell
     pip install leetquery
 ```
 ## Usage
 ### Retriving User Submissions
-Just enter user name and limit of query!
 ``` python
 from leetquery import get_submissions
 
-submissions = get_submissions(username="syhaung", limits=12)
+submissions = get_submissions(username="syhaung", limits)
 ```
 return value:
 ```
 ["question1", "question2", ...]
 ```
```

### Comparing `leetquery-0.1.15/setup.py` & `leetquery-0.1.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 from shutil import rmtree
 
 from setuptools import find_packages, setup, Command
 
 # Package meta-data.
 NAME = "leetquery"
 DESCRIPTION = "Query and analyze data from leetcode"
-URL = "https://github.com/ShuYuHuang/leetquery"
+URL = "https://github.com/ShuYuHuang/leetcode-query"
 EMAIL = "b123767195@gmail.com"
 AUTHOR = "Shu-Yu Huang"
 REQUIRES_PYTHON = ">=3.7.0"
 VERSION = None
 
 # The rest you shouldn't have to touch too much :)
 # ------------------------------------------------
```


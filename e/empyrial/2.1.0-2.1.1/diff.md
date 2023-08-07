# Comparing `tmp/empyrial-2.1.0.tar.gz` & `tmp/empyrial-2.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "empyrial-2.1.0.tar", last modified: Mon Aug  7 22:35:44 2023, max compression
+gzip compressed data, was "empyrial-2.1.1.tar", last modified: Mon Aug  7 22:51:32 2023, max compression
```

## Comparing `empyrial-2.1.0.tar` & `empyrial-2.1.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 22:35:44.546123 empyrial-2.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)      394 2023-08-07 22:35:44.546123 empyrial-2.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    14470 2023-08-07 22:35:08.000000 empyrial-2.1.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      280 2023-08-07 22:35:08.000000 empyrial-2.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      737 2023-08-07 22:35:44.546123 empyrial-2.1.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 22:35:44.542123 empyrial-2.1.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 22:35:44.546123 empyrial-2.1.0/src/empyrial/
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-08-07 22:35:08.000000 empyrial-2.1.0/src/empyrial/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    38569 2023-08-07 22:35:08.000000 empyrial-2.1.0/src/empyrial/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 22:35:44.546123 empyrial-2.1.0/src/empyrial.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      394 2023-08-07 22:35:44.000000 empyrial-2.1.0/src/empyrial.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      298 2023-08-07 22:35:44.000000 empyrial-2.1.0/src/empyrial.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-07 22:35:44.000000 empyrial-2.1.0/src/empyrial.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-08-07 22:35:44.000000 empyrial-2.1.0/src/empyrial.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-08-07 22:35:44.000000 empyrial-2.1.0/src/empyrial.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-08-07 22:35:44.000000 empyrial-2.1.0/src/empyrial.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 22:51:32.048905 empyrial-2.1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)      394 2023-08-07 22:51:32.048905 empyrial-2.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    14470 2023-08-07 22:50:53.000000 empyrial-2.1.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      280 2023-08-07 22:50:53.000000 empyrial-2.1.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      737 2023-08-07 22:51:32.048905 empyrial-2.1.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 22:51:32.048905 empyrial-2.1.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 22:51:32.048905 empyrial-2.1.1/src/empyrial/
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-08-07 22:50:53.000000 empyrial-2.1.1/src/empyrial/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38617 2023-08-07 22:50:53.000000 empyrial-2.1.1/src/empyrial/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 22:51:32.048905 empyrial-2.1.1/src/empyrial.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      394 2023-08-07 22:51:32.000000 empyrial-2.1.1/src/empyrial.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      298 2023-08-07 22:51:32.000000 empyrial-2.1.1/src/empyrial.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-07 22:51:32.000000 empyrial-2.1.1/src/empyrial.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-08-07 22:51:32.000000 empyrial-2.1.1/src/empyrial.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-08-07 22:51:32.000000 empyrial-2.1.1/src/empyrial.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-08-07 22:51:32.000000 empyrial-2.1.1/src/empyrial.egg-info/top_level.txt
```

### Comparing `empyrial-2.1.0/README.md` & `empyrial-2.1.1/README.md`

 * *Files identical despite different names*

### Comparing `empyrial-2.1.0/setup.cfg` & `empyrial-2.1.1/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = empyrial
-version = 2.1.0
+version = 2.1.1
 description = An Open Source Portfolio Management Framework for Everyone 投资组合管理
 url = https://github.com/ssantoshp/Empyrial
 long_description_content_type = text/markdown
 long_descript = # Empyrial
 classifiers = 
 	Programming Language :: Python :: 3
 	License :: OSI Approved :: BSD License
```

### Comparing `empyrial-2.1.0/src/empyrial/main.py` & `empyrial-2.1.1/src/empyrial/main.py`

 * *Files 0% similar despite different names*

```diff
@@ -760,15 +760,18 @@
     start_date = dt.datetime.strptime(start_date, "%Y-%m-%d")
 
     # custom dates don't need further chekings
     if type(rebalance) is list:
         return start_date, rebalance[-1]
     
     # make the end date to a datetime
-    end_date = dt.datetime.strptime(end_date, "%Y-%m-%d")
+    try:
+        end_date = dt.datetime.strptime(end_date, "%Y-%m-%d")
+    except TypeError:
+        pass
 
 
     # gets the number of days
     days = (end_date - start_date).days
 
     # checking that date range covers rebalance period
     if rebalance in rebalance_periods.keys() and days <= (int(rebalance_periods[rebalance])):
```


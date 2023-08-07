# Comparing `tmp/score_regression-0.0.15.tar.gz` & `tmp/score_regression-0.0.16.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "score_regression-0.0.15.tar", last modified: Sat Aug  5 05:10:23 2023, max compression
+gzip compressed data, was "score_regression-0.0.16.tar", last modified: Mon Aug  7 23:25:14 2023, max compression
```

## Comparing `score_regression-0.0.15.tar` & `score_regression-0.0.16.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxr-x   0 rolf      (1000) rolf      (1000)        0 2023-08-05 05:10:23.530275 score_regression-0.0.15/
--rw-rw-r--   0 rolf      (1000) rolf      (1000)     1529 2023-08-02 15:42:42.000000 score_regression-0.0.15/LICENSE
--rw-rw-r--   0 rolf      (1000) rolf      (1000)       25 2023-08-02 15:42:42.000000 score_regression-0.0.15/MANIFEST.in
--rw-rw-r--   0 rolf      (1000) rolf      (1000)     3058 2023-08-05 05:10:23.530275 score_regression-0.0.15/PKG-INFO
--rw-rw-r--   0 rolf      (1000) rolf      (1000)     2243 2023-08-05 02:45:31.000000 score_regression-0.0.15/README.rst
--rw-rw-r--   0 rolf      (1000) rolf      (1000)      133 2023-08-03 00:34:01.000000 score_regression-0.0.15/requirements.txt
-drwxrwxr-x   0 rolf      (1000) rolf      (1000)        0 2023-08-05 05:10:23.530275 score_regression-0.0.15/score_regression/
--rw-rw-r--   0 rolf      (1000) rolf      (1000)      200 2023-08-04 02:00:42.000000 score_regression-0.0.15/score_regression/__init__.py
--rw-rw-r--   0 rolf      (1000) rolf      (1000)       23 2023-08-05 05:08:42.000000 score_regression-0.0.15/score_regression/_version.py
--rw-rw-r--   0 rolf      (1000) rolf      (1000)    12046 2023-08-05 02:37:52.000000 score_regression-0.0.15/score_regression/score_regression.py
-drwxrwxr-x   0 rolf      (1000) rolf      (1000)        0 2023-08-05 05:10:23.530275 score_regression-0.0.15/score_regression/tests/
--rw-rw-r--   0 rolf      (1000) rolf      (1000)        0 2023-08-02 15:42:42.000000 score_regression-0.0.15/score_regression/tests/__init__.py
--rw-rw-r--   0 rolf      (1000) rolf      (1000)      321 2023-08-04 02:03:02.000000 score_regression-0.0.15/score_regression/tests/test_common.py
--rw-rw-r--   0 rolf      (1000) rolf      (1000)     1241 2023-08-04 17:23:29.000000 score_regression-0.0.15/score_regression/tests/test_template.py
-drwxrwxr-x   0 rolf      (1000) rolf      (1000)        0 2023-08-05 05:10:23.530275 score_regression-0.0.15/score_regression.egg-info/
--rw-rw-r--   0 rolf      (1000) rolf      (1000)     3058 2023-08-05 05:10:23.000000 score_regression-0.0.15/score_regression.egg-info/PKG-INFO
--rw-rw-r--   0 rolf      (1000) rolf      (1000)      512 2023-08-05 05:10:23.000000 score_regression-0.0.15/score_regression.egg-info/SOURCES.txt
--rw-rw-r--   0 rolf      (1000) rolf      (1000)        1 2023-08-05 05:10:23.000000 score_regression-0.0.15/score_regression.egg-info/dependency_links.txt
--rw-rw-r--   0 rolf      (1000) rolf      (1000)        1 2023-08-05 02:40:22.000000 score_regression-0.0.15/score_regression.egg-info/not-zip-safe
--rw-rw-r--   0 rolf      (1000) rolf      (1000)      119 2023-08-05 05:10:23.000000 score_regression-0.0.15/score_regression.egg-info/requires.txt
--rw-rw-r--   0 rolf      (1000) rolf      (1000)       17 2023-08-05 05:10:23.000000 score_regression-0.0.15/score_regression.egg-info/top_level.txt
--rw-rw-r--   0 rolf      (1000) rolf      (1000)      148 2023-08-05 05:10:23.534275 score_regression-0.0.15/setup.cfg
--rw-rw-r--   0 rolf      (1000) rolf      (1000)     2631 2023-08-05 02:26:20.000000 score_regression-0.0.15/setup.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-07 23:25:14.709840 score_regression-0.0.16/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1529 2023-08-07 23:22:15.000000 score_regression-0.0.16/LICENSE
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       25 2023-08-07 23:22:15.000000 score_regression-0.0.16/MANIFEST.in
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3058 2023-08-07 23:25:14.709840 score_regression-0.0.16/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2243 2023-08-07 23:22:15.000000 score_regression-0.0.16/README.rst
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      133 2023-08-07 23:22:15.000000 score_regression-0.0.16/requirements.txt
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-07 23:25:14.709840 score_regression-0.0.16/score_regression/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      200 2023-08-07 23:22:15.000000 score_regression-0.0.16/score_regression/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       23 2023-08-07 23:22:15.000000 score_regression-0.0.16/score_regression/_version.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    21229 2023-08-07 23:22:15.000000 score_regression-0.0.16/score_regression/score_regression.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-07 23:25:14.709840 score_regression-0.0.16/score_regression/tests/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-08-07 23:22:15.000000 score_regression-0.0.16/score_regression/tests/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      321 2023-08-07 23:22:15.000000 score_regression-0.0.16/score_regression/tests/test_common.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1241 2023-08-07 23:22:15.000000 score_regression-0.0.16/score_regression/tests/test_template.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-07 23:25:14.709840 score_regression-0.0.16/score_regression.egg-info/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3058 2023-08-07 23:25:14.000000 score_regression-0.0.16/score_regression.egg-info/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      512 2023-08-07 23:25:14.000000 score_regression-0.0.16/score_regression.egg-info/SOURCES.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2023-08-07 23:25:14.000000 score_regression-0.0.16/score_regression.egg-info/dependency_links.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2023-08-07 23:23:01.000000 score_regression-0.0.16/score_regression.egg-info/not-zip-safe
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      119 2023-08-07 23:25:14.000000 score_regression-0.0.16/score_regression.egg-info/requires.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       17 2023-08-07 23:25:14.000000 score_regression-0.0.16/score_regression.egg-info/top_level.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      148 2023-08-07 23:25:14.713840 score_regression-0.0.16/setup.cfg
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2631 2023-08-07 23:22:15.000000 score_regression-0.0.16/setup.py
```

### Comparing `score_regression-0.0.15/LICENSE` & `score_regression-0.0.16/LICENSE`

 * *Files identical despite different names*

### Comparing `score_regression-0.0.15/PKG-INFO` & `score_regression-0.0.16/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: score_regression
-Version: 0.0.15
+Version: 0.0.16
 Summary: A classifier that maximizes AUC
 Home-page: https://github.com/hrolfrc/score_regression
 Download-URL: https://github.com/hrolfrc/score_regression
 Maintainer: Carlson Research, LLC
 Maintainer-email: hrolfrc@gmail.com
 License: new BSD
 Classifier: Intended Audience :: Science/Research
```

### Comparing `score_regression-0.0.15/README.rst` & `score_regression-0.0.16/README.rst`

 * *Files identical despite different names*

### Comparing `score_regression-0.0.15/score_regression/tests/test_template.py` & `score_regression-0.0.16/score_regression/tests/test_template.py`

 * *Files identical despite different names*

### Comparing `score_regression-0.0.15/score_regression.egg-info/PKG-INFO` & `score_regression-0.0.16/score_regression.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: score-regression
-Version: 0.0.15
+Version: 0.0.16
 Summary: A classifier that maximizes AUC
 Home-page: https://github.com/hrolfrc/score_regression
 Download-URL: https://github.com/hrolfrc/score_regression
 Maintainer: Carlson Research, LLC
 Maintainer-email: hrolfrc@gmail.com
 License: new BSD
 Classifier: Intended Audience :: Science/Research
```

### Comparing `score_regression-0.0.15/score_regression.egg-info/SOURCES.txt` & `score_regression-0.0.16/score_regression.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `score_regression-0.0.15/setup.py` & `score_regression-0.0.16/setup.py`

 * *Files identical despite different names*


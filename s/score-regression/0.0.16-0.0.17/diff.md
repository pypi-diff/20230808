# Comparing `tmp/score_regression-0.0.16.tar.gz` & `tmp/score_regression-0.0.17.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "score_regression-0.0.16.tar", last modified: Mon Aug  7 23:25:14 2023, max compression
+gzip compressed data, was "score_regression-0.0.17.tar", last modified: Mon Aug  7 23:39:34 2023, max compression
```

## Comparing `score_regression-0.0.16.tar` & `score_regression-0.0.17.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-07 23:25:14.709840 score_regression-0.0.16/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1529 2023-08-07 23:22:15.000000 score_regression-0.0.16/LICENSE
--rw-r--r--   0 circleci  (1001) circleci  (1002)       25 2023-08-07 23:22:15.000000 score_regression-0.0.16/MANIFEST.in
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3058 2023-08-07 23:25:14.709840 score_regression-0.0.16/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2243 2023-08-07 23:22:15.000000 score_regression-0.0.16/README.rst
--rw-r--r--   0 circleci  (1001) circleci  (1002)      133 2023-08-07 23:22:15.000000 score_regression-0.0.16/requirements.txt
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-07 23:25:14.709840 score_regression-0.0.16/score_regression/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      200 2023-08-07 23:22:15.000000 score_regression-0.0.16/score_regression/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)       23 2023-08-07 23:22:15.000000 score_regression-0.0.16/score_regression/_version.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    21229 2023-08-07 23:22:15.000000 score_regression-0.0.16/score_regression/score_regression.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-07 23:25:14.709840 score_regression-0.0.16/score_regression/tests/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-08-07 23:22:15.000000 score_regression-0.0.16/score_regression/tests/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      321 2023-08-07 23:22:15.000000 score_regression-0.0.16/score_regression/tests/test_common.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1241 2023-08-07 23:22:15.000000 score_regression-0.0.16/score_regression/tests/test_template.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-07 23:25:14.709840 score_regression-0.0.16/score_regression.egg-info/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3058 2023-08-07 23:25:14.000000 score_regression-0.0.16/score_regression.egg-info/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)      512 2023-08-07 23:25:14.000000 score_regression-0.0.16/score_regression.egg-info/SOURCES.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2023-08-07 23:25:14.000000 score_regression-0.0.16/score_regression.egg-info/dependency_links.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2023-08-07 23:23:01.000000 score_regression-0.0.16/score_regression.egg-info/not-zip-safe
--rw-r--r--   0 circleci  (1001) circleci  (1002)      119 2023-08-07 23:25:14.000000 score_regression-0.0.16/score_regression.egg-info/requires.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)       17 2023-08-07 23:25:14.000000 score_regression-0.0.16/score_regression.egg-info/top_level.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)      148 2023-08-07 23:25:14.713840 score_regression-0.0.16/setup.cfg
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2631 2023-08-07 23:22:15.000000 score_regression-0.0.16/setup.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-07 23:39:34.298074 score_regression-0.0.17/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1486 2023-08-07 23:36:01.000000 score_regression-0.0.17/LICENSE
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       25 2023-08-07 23:36:01.000000 score_regression-0.0.17/MANIFEST.in
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3058 2023-08-07 23:39:34.298074 score_regression-0.0.17/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2243 2023-08-07 23:36:01.000000 score_regression-0.0.17/README.rst
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      133 2023-08-07 23:36:01.000000 score_regression-0.0.17/requirements.txt
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-07 23:39:34.294074 score_regression-0.0.17/score_regression/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      200 2023-08-07 23:36:01.000000 score_regression-0.0.17/score_regression/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       23 2023-08-07 23:36:01.000000 score_regression-0.0.17/score_regression/_version.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    21229 2023-08-07 23:36:01.000000 score_regression-0.0.17/score_regression/score_regression.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-07 23:39:34.298074 score_regression-0.0.17/score_regression/tests/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-08-07 23:36:01.000000 score_regression-0.0.17/score_regression/tests/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      321 2023-08-07 23:36:01.000000 score_regression-0.0.17/score_regression/tests/test_common.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1241 2023-08-07 23:36:01.000000 score_regression-0.0.17/score_regression/tests/test_template.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-07 23:39:34.298074 score_regression-0.0.17/score_regression.egg-info/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3058 2023-08-07 23:39:34.000000 score_regression-0.0.17/score_regression.egg-info/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      512 2023-08-07 23:39:34.000000 score_regression-0.0.17/score_regression.egg-info/SOURCES.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2023-08-07 23:39:34.000000 score_regression-0.0.17/score_regression.egg-info/dependency_links.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2023-08-07 23:36:49.000000 score_regression-0.0.17/score_regression.egg-info/not-zip-safe
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      119 2023-08-07 23:39:34.000000 score_regression-0.0.17/score_regression.egg-info/requires.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       17 2023-08-07 23:39:34.000000 score_regression-0.0.17/score_regression.egg-info/top_level.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      148 2023-08-07 23:39:34.298074 score_regression-0.0.17/setup.cfg
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2631 2023-08-07 23:36:01.000000 score_regression-0.0.17/setup.py
```

### Comparing `score_regression-0.0.16/LICENSE` & `score_regression-0.0.17/LICENSE`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-Copyright (c) 2016, Vighnesh Birodkar and scikit-learn-contrib contributors
+Copyright (c) 2023, Rolf Carlson
 All rights reserved.
 
 Redistribution and use in source and binary forms, with or without
 modification, are permitted provided that the following conditions are met:
 
 * Redistributions of source code must retain the above copyright notice, this
   list of conditions and the following disclaimer.
```

### Comparing `score_regression-0.0.16/PKG-INFO` & `score_regression-0.0.17/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: score_regression
-Version: 0.0.16
+Version: 0.0.17
 Summary: A classifier that maximizes AUC
 Home-page: https://github.com/hrolfrc/score_regression
 Download-URL: https://github.com/hrolfrc/score_regression
 Maintainer: Carlson Research, LLC
 Maintainer-email: hrolfrc@gmail.com
 License: new BSD
 Classifier: Intended Audience :: Science/Research
```

### Comparing `score_regression-0.0.16/README.rst` & `score_regression-0.0.17/README.rst`

 * *Files identical despite different names*

### Comparing `score_regression-0.0.16/score_regression/score_regression.py` & `score_regression-0.0.17/score_regression/score_regression.py`

 * *Files identical despite different names*

### Comparing `score_regression-0.0.16/score_regression/tests/test_template.py` & `score_regression-0.0.17/score_regression/tests/test_template.py`

 * *Files identical despite different names*

### Comparing `score_regression-0.0.16/score_regression.egg-info/PKG-INFO` & `score_regression-0.0.17/score_regression.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: score-regression
-Version: 0.0.16
+Version: 0.0.17
 Summary: A classifier that maximizes AUC
 Home-page: https://github.com/hrolfrc/score_regression
 Download-URL: https://github.com/hrolfrc/score_regression
 Maintainer: Carlson Research, LLC
 Maintainer-email: hrolfrc@gmail.com
 License: new BSD
 Classifier: Intended Audience :: Science/Research
```

### Comparing `score_regression-0.0.16/score_regression.egg-info/SOURCES.txt` & `score_regression-0.0.17/score_regression.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `score_regression-0.0.16/setup.py` & `score_regression-0.0.17/setup.py`

 * *Files identical despite different names*


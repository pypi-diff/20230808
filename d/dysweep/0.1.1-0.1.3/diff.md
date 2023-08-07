# Comparing `tmp/dysweep-0.1.1.tar.gz` & `tmp/dysweep-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dysweep-0.1.1.tar", last modified: Fri Jun 30 19:42:32 2023, max compression
+gzip compressed data, was "dysweep-0.1.3.tar", last modified: Fri Jun 30 20:17:26 2023, max compression
```

## Comparing `dysweep-0.1.1.tar` & `dysweep-0.1.3.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 19:42:32.927796 dysweep-0.1.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-06-30 19:40:04.000000 dysweep-0.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2378 2023-06-30 19:42:32.927796 dysweep-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8259 2023-06-30 19:40:04.000000 dysweep-0.1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 19:42:32.927796 dysweep-0.1.1/dysweep/
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-06-30 19:40:04.000000 dysweep-0.1.1/dysweep/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3819 2023-06-30 19:40:04.000000 dysweep-0.1.1/dysweep/console.py
--rw-r--r--   0 runner    (1001) docker     (123)    22831 2023-06-30 19:40:04.000000 dysweep-0.1.1/dysweep/parallel.py
--rw-r--r--   0 runner    (1001) docker     (123)    21897 2023-06-30 19:40:04.000000 dysweep-0.1.1/dysweep/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4456 2023-06-30 19:40:04.000000 dysweep-0.1.1/dysweep/wandbX.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 19:42:32.927796 dysweep-0.1.1/dysweep.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2378 2023-06-30 19:42:32.000000 dysweep-0.1.1/dysweep.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      278 2023-06-30 19:42:32.000000 dysweep-0.1.1/dysweep.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-30 19:42:32.000000 dysweep-0.1.1/dysweep.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      119 2023-06-30 19:42:32.000000 dysweep-0.1.1/dysweep.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-30 19:42:32.000000 dysweep-0.1.1/dysweep.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-30 19:42:32.927796 dysweep-0.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1739 2023-06-30 19:40:04.000000 dysweep-0.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 20:17:26.311248 dysweep-0.1.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-06-30 20:15:10.000000 dysweep-0.1.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2378 2023-06-30 20:17:26.311248 dysweep-0.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8354 2023-06-30 20:15:10.000000 dysweep-0.1.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 20:17:26.311248 dysweep-0.1.3/dysweep/
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-06-30 20:15:10.000000 dysweep-0.1.3/dysweep/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3819 2023-06-30 20:15:10.000000 dysweep-0.1.3/dysweep/console.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22831 2023-06-30 20:15:10.000000 dysweep-0.1.3/dysweep/parallel.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21897 2023-06-30 20:15:10.000000 dysweep-0.1.3/dysweep/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4456 2023-06-30 20:15:10.000000 dysweep-0.1.3/dysweep/wandbX.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 20:17:26.311248 dysweep-0.1.3/dysweep.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2378 2023-06-30 20:17:26.000000 dysweep-0.1.3/dysweep.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      278 2023-06-30 20:17:26.000000 dysweep-0.1.3/dysweep.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-30 20:17:26.000000 dysweep-0.1.3/dysweep.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      119 2023-06-30 20:17:26.000000 dysweep-0.1.3/dysweep.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-30 20:17:26.000000 dysweep-0.1.3/dysweep.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-30 20:17:26.311248 dysweep-0.1.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1739 2023-06-30 20:15:10.000000 dysweep-0.1.3/setup.py
```

### Comparing `dysweep-0.1.1/LICENSE` & `dysweep-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `dysweep-0.1.1/PKG-INFO` & `dysweep-0.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dysweep
-Version: 0.1.1
+Version: 0.1.3
 Summary: Use Weights and Biases Sweeps for Dynamic Configuration generation.
 Home-page: https://github.com/HamidrezaKmK/dysweep
 Author: Hamid Kamkari
 Author-email: hamidrezakamkari@gmail.com
 License: MIT
 Description: # Dysweep
```

### Comparing `dysweep-0.1.1/README.md` & `dysweep-0.1.3/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 <i>Generic hierarchical configurations and resumable runs on Weights & Biases for Research</i>
 </h4>
 
 
 
 
 [![PyPI version](https://badge.fury.io/py/dysweep.svg)](https://pypi.org/project/dysweep/)
+[![DOI](https://zenodo.org/badge/643277847.svg)](https://zenodo.org/badge/latestdoi/643277847)
 [![Slack](https://img.shields.io/badge/chat-on%20slack-red.svg)](https://join.slack.com/t/dysweep/shared_invite/zt-1ynkfdpdc-wiYHkiLzjrZ8yGqYkM9brQ)
 
 </div>
 
 ![Bird's Eye View](./images/main-figure.svg)
 Use the extended capabilities of *Dysweep* library on top of Weights & Biases for fast and comprehensive experimentation in your research projects.
```

### Comparing `dysweep-0.1.1/dysweep/console.py` & `dysweep-0.1.3/dysweep/console.py`

 * *Files identical despite different names*

### Comparing `dysweep-0.1.1/dysweep/parallel.py` & `dysweep-0.1.3/dysweep/parallel.py`

 * *Files identical despite different names*

### Comparing `dysweep-0.1.1/dysweep/utils.py` & `dysweep-0.1.3/dysweep/utils.py`

 * *Files identical despite different names*

### Comparing `dysweep-0.1.1/dysweep/wandbX.py` & `dysweep-0.1.3/dysweep/wandbX.py`

 * *Files identical despite different names*

### Comparing `dysweep-0.1.1/dysweep.egg-info/PKG-INFO` & `dysweep-0.1.3/dysweep.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dysweep
-Version: 0.1.1
+Version: 0.1.3
 Summary: Use Weights and Biases Sweeps for Dynamic Configuration generation.
 Home-page: https://github.com/HamidrezaKmK/dysweep
 Author: Hamid Kamkari
 Author-email: hamidrezakamkari@gmail.com
 License: MIT
 Description: # Dysweep
```

### Comparing `dysweep-0.1.1/setup.py` & `dysweep-0.1.3/setup.py`

 * *Files identical despite different names*


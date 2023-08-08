# Comparing `tmp/botocore-a-la-carte-keyspaces-1.31.8.tar.gz` & `tmp/botocore-a-la-carte-keyspaces-1.31.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "botocore-a-la-carte-keyspaces-1.31.8.tar", last modified: Fri Jul 21 01:21:35 2023, max compression
+gzip compressed data, was "botocore-a-la-carte-keyspaces-1.31.9.tar", last modified: Sat Jul 22 01:20:37 2023, max compression
```

## Comparing `botocore-a-la-carte-keyspaces-1.31.8.tar` & `botocore-a-la-carte-keyspaces-1.31.9.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 01:21:35.051172 botocore-a-la-carte-keyspaces-1.31.8/
--rw-r--r--   0 runner    (1001) docker     (123)    10174 2023-07-21 01:21:34.000000 botocore-a-la-carte-keyspaces-1.31.8/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      961 2023-07-21 01:21:35.051172 botocore-a-la-carte-keyspaces-1.31.8/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 01:21:35.047172 botocore-a-la-carte-keyspaces-1.31.8/botocore/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 01:21:35.047172 botocore-a-la-carte-keyspaces-1.31.8/botocore/data/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 01:21:35.047172 botocore-a-la-carte-keyspaces-1.31.8/botocore/data/keyspaces/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 01:21:35.051172 botocore-a-la-carte-keyspaces-1.31.8/botocore/data/keyspaces/2022-02-10/
--rw-r--r--   0 runner    (1001) docker     (123)    19605 2023-07-21 01:21:06.000000 botocore-a-la-carte-keyspaces-1.31.8/botocore/data/keyspaces/2022-02-10/endpoint-rule-set-1.json
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-07-21 01:21:06.000000 botocore-a-la-carte-keyspaces-1.31.8/botocore/data/keyspaces/2022-02-10/examples-1.json
--rw-r--r--   0 runner    (1001) docker     (123)      512 2023-07-21 01:21:06.000000 botocore-a-la-carte-keyspaces-1.31.8/botocore/data/keyspaces/2022-02-10/paginators-1.json
--rw-r--r--   0 runner    (1001) docker     (123)    63076 2023-07-21 01:21:06.000000 botocore-a-la-carte-keyspaces-1.31.8/botocore/data/keyspaces/2022-02-10/service-2.json
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-21 01:21:06.000000 botocore-a-la-carte-keyspaces-1.31.8/botocore/data/keyspaces/2022-02-10/waiters-2.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 01:21:35.051172 botocore-a-la-carte-keyspaces-1.31.8/botocore_a_la_carte_keyspaces.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      961 2023-07-21 01:21:35.000000 botocore-a-la-carte-keyspaces-1.31.8/botocore_a_la_carte_keyspaces.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      496 2023-07-21 01:21:35.000000 botocore-a-la-carte-keyspaces-1.31.8/botocore_a_la_carte_keyspaces.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-21 01:21:35.000000 botocore-a-la-carte-keyspaces-1.31.8/botocore_a_la_carte_keyspaces.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-21 01:21:35.000000 botocore-a-la-carte-keyspaces-1.31.8/botocore_a_la_carte_keyspaces.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-21 01:21:35.051172 botocore-a-la-carte-keyspaces-1.31.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1147 2023-07-21 01:21:34.000000 botocore-a-la-carte-keyspaces-1.31.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 01:20:37.065105 botocore-a-la-carte-keyspaces-1.31.9/
+-rw-r--r--   0 runner    (1001) docker     (123)    10174 2023-07-22 01:20:36.000000 botocore-a-la-carte-keyspaces-1.31.9/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      961 2023-07-22 01:20:37.065105 botocore-a-la-carte-keyspaces-1.31.9/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 01:20:37.065105 botocore-a-la-carte-keyspaces-1.31.9/botocore/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 01:20:37.065105 botocore-a-la-carte-keyspaces-1.31.9/botocore/data/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 01:20:37.065105 botocore-a-la-carte-keyspaces-1.31.9/botocore/data/keyspaces/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 01:20:37.065105 botocore-a-la-carte-keyspaces-1.31.9/botocore/data/keyspaces/2022-02-10/
+-rw-r--r--   0 runner    (1001) docker     (123)    19605 2023-07-22 01:20:09.000000 botocore-a-la-carte-keyspaces-1.31.9/botocore/data/keyspaces/2022-02-10/endpoint-rule-set-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-07-22 01:20:09.000000 botocore-a-la-carte-keyspaces-1.31.9/botocore/data/keyspaces/2022-02-10/examples-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)      512 2023-07-22 01:20:09.000000 botocore-a-la-carte-keyspaces-1.31.9/botocore/data/keyspaces/2022-02-10/paginators-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)    63076 2023-07-22 01:20:09.000000 botocore-a-la-carte-keyspaces-1.31.9/botocore/data/keyspaces/2022-02-10/service-2.json
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-22 01:20:09.000000 botocore-a-la-carte-keyspaces-1.31.9/botocore/data/keyspaces/2022-02-10/waiters-2.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 01:20:37.065105 botocore-a-la-carte-keyspaces-1.31.9/botocore_a_la_carte_keyspaces.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      961 2023-07-22 01:20:37.000000 botocore-a-la-carte-keyspaces-1.31.9/botocore_a_la_carte_keyspaces.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      496 2023-07-22 01:20:37.000000 botocore-a-la-carte-keyspaces-1.31.9/botocore_a_la_carte_keyspaces.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-22 01:20:37.000000 botocore-a-la-carte-keyspaces-1.31.9/botocore_a_la_carte_keyspaces.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-22 01:20:37.000000 botocore-a-la-carte-keyspaces-1.31.9/botocore_a_la_carte_keyspaces.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-22 01:20:37.065105 botocore-a-la-carte-keyspaces-1.31.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1147 2023-07-22 01:20:36.000000 botocore-a-la-carte-keyspaces-1.31.9/setup.py
```

### Comparing `botocore-a-la-carte-keyspaces-1.31.8/LICENSE.txt` & `botocore-a-la-carte-keyspaces-1.31.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-keyspaces-1.31.8/PKG-INFO` & `botocore-a-la-carte-keyspaces-1.31.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: botocore-a-la-carte-keyspaces
-Version: 1.31.8
+Version: 1.31.9
 Summary: keyspaces data for botocore. See the `botocore-a-la-carte` package for more info.
 Home-page: https://github.com/thejcannon/botocore-a-la-carte
 Author: Amazon Web Services
 License: Apache License 2.0
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `botocore-a-la-carte-keyspaces-1.31.8/botocore/data/keyspaces/2022-02-10/endpoint-rule-set-1.json` & `botocore-a-la-carte-keyspaces-1.31.9/botocore/data/keyspaces/2022-02-10/endpoint-rule-set-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-keyspaces-1.31.8/botocore/data/keyspaces/2022-02-10/paginators-1.json` & `botocore-a-la-carte-keyspaces-1.31.9/botocore/data/keyspaces/2022-02-10/paginators-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-keyspaces-1.31.8/botocore/data/keyspaces/2022-02-10/service-2.json` & `botocore-a-la-carte-keyspaces-1.31.9/botocore/data/keyspaces/2022-02-10/service-2.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-keyspaces-1.31.8/botocore_a_la_carte_keyspaces.egg-info/PKG-INFO` & `botocore-a-la-carte-keyspaces-1.31.9/botocore_a_la_carte_keyspaces.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: botocore-a-la-carte-keyspaces
-Version: 1.31.8
+Version: 1.31.9
 Summary: keyspaces data for botocore. See the `botocore-a-la-carte` package for more info.
 Home-page: https://github.com/thejcannon/botocore-a-la-carte
 Author: Amazon Web Services
 License: Apache License 2.0
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `botocore-a-la-carte-keyspaces-1.31.8/setup.py` & `botocore-a-la-carte-keyspaces-1.31.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #!/usr/bin/env python
 from setuptools import setup
 
 setup(
     name='botocore-a-la-carte-keyspaces',
-    version="1.31.8",
+    version="1.31.9",
     description='keyspaces data for botocore. See the `botocore-a-la-carte` package for more info.',
     author='Amazon Web Services',
     url='https://github.com/thejcannon/botocore-a-la-carte',
     scripts=[],
     packages=["botocore"],
     package_data={
         'botocore': ['data/keyspaces/*/*.json'],
```

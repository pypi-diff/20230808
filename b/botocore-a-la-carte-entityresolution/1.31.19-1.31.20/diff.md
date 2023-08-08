# Comparing `tmp/botocore-a-la-carte-entityresolution-1.31.19.tar.gz` & `tmp/botocore-a-la-carte-entityresolution-1.31.20.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "botocore-a-la-carte-entityresolution-1.31.19.tar", last modified: Fri Aug  4 01:16:27 2023, max compression
+gzip compressed data, was "botocore-a-la-carte-entityresolution-1.31.20.tar", last modified: Sat Aug  5 01:13:12 2023, max compression
```

## Comparing `botocore-a-la-carte-entityresolution-1.31.19.tar` & `botocore-a-la-carte-entityresolution-1.31.20.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 01:16:27.968512 botocore-a-la-carte-entityresolution-1.31.19/
--rw-r--r--   0 runner    (1001) docker     (123)    10174 2023-08-04 01:16:27.000000 botocore-a-la-carte-entityresolution-1.31.19/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      976 2023-08-04 01:16:27.968512 botocore-a-la-carte-entityresolution-1.31.19/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 01:16:27.968512 botocore-a-la-carte-entityresolution-1.31.19/botocore/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 01:16:27.968512 botocore-a-la-carte-entityresolution-1.31.19/botocore/data/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 01:16:27.968512 botocore-a-la-carte-entityresolution-1.31.19/botocore/data/entityresolution/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 01:16:27.968512 botocore-a-la-carte-entityresolution-1.31.19/botocore/data/entityresolution/2018-05-10/
--rw-r--r--   0 runner    (1001) docker     (123)    17664 2023-08-04 01:15:59.000000 botocore-a-la-carte-entityresolution-1.31.19/botocore/data/entityresolution/2018-05-10/endpoint-rule-set-1.json
--rw-r--r--   0 runner    (1001) docker     (123)      537 2023-08-04 01:15:59.000000 botocore-a-la-carte-entityresolution-1.31.19/botocore/data/entityresolution/2018-05-10/paginators-1.json
--rw-r--r--   0 runner    (1001) docker     (123)    57680 2023-08-04 01:15:59.000000 botocore-a-la-carte-entityresolution-1.31.19/botocore/data/entityresolution/2018-05-10/service-2.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 01:16:27.968512 botocore-a-la-carte-entityresolution-1.31.19/botocore_a_la_carte_entityresolution.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      976 2023-08-04 01:16:27.000000 botocore-a-la-carte-entityresolution-1.31.19/botocore_a_la_carte_entityresolution.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      444 2023-08-04 01:16:27.000000 botocore-a-la-carte-entityresolution-1.31.19/botocore_a_la_carte_entityresolution.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 01:16:27.000000 botocore-a-la-carte-entityresolution-1.31.19/botocore_a_la_carte_entityresolution.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-08-04 01:16:27.000000 botocore-a-la-carte-entityresolution-1.31.19/botocore_a_la_carte_entityresolution.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-04 01:16:27.968512 botocore-a-la-carte-entityresolution-1.31.19/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1169 2023-08-04 01:16:27.000000 botocore-a-la-carte-entityresolution-1.31.19/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 01:13:12.939040 botocore-a-la-carte-entityresolution-1.31.20/
+-rw-r--r--   0 runner    (1001) docker     (123)    10174 2023-08-05 01:13:12.000000 botocore-a-la-carte-entityresolution-1.31.20/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      976 2023-08-05 01:13:12.939040 botocore-a-la-carte-entityresolution-1.31.20/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 01:13:12.939040 botocore-a-la-carte-entityresolution-1.31.20/botocore/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 01:13:12.939040 botocore-a-la-carte-entityresolution-1.31.20/botocore/data/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 01:13:12.939040 botocore-a-la-carte-entityresolution-1.31.20/botocore/data/entityresolution/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 01:13:12.939040 botocore-a-la-carte-entityresolution-1.31.20/botocore/data/entityresolution/2018-05-10/
+-rw-r--r--   0 runner    (1001) docker     (123)    17664 2023-08-05 01:12:40.000000 botocore-a-la-carte-entityresolution-1.31.20/botocore/data/entityresolution/2018-05-10/endpoint-rule-set-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)      537 2023-08-05 01:12:40.000000 botocore-a-la-carte-entityresolution-1.31.20/botocore/data/entityresolution/2018-05-10/paginators-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)    57680 2023-08-05 01:12:40.000000 botocore-a-la-carte-entityresolution-1.31.20/botocore/data/entityresolution/2018-05-10/service-2.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 01:13:12.939040 botocore-a-la-carte-entityresolution-1.31.20/botocore_a_la_carte_entityresolution.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      976 2023-08-05 01:13:12.000000 botocore-a-la-carte-entityresolution-1.31.20/botocore_a_la_carte_entityresolution.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      444 2023-08-05 01:13:12.000000 botocore-a-la-carte-entityresolution-1.31.20/botocore_a_la_carte_entityresolution.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-05 01:13:12.000000 botocore-a-la-carte-entityresolution-1.31.20/botocore_a_la_carte_entityresolution.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-08-05 01:13:12.000000 botocore-a-la-carte-entityresolution-1.31.20/botocore_a_la_carte_entityresolution.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-05 01:13:12.939040 botocore-a-la-carte-entityresolution-1.31.20/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1169 2023-08-05 01:13:12.000000 botocore-a-la-carte-entityresolution-1.31.20/setup.py
```

### Comparing `botocore-a-la-carte-entityresolution-1.31.19/LICENSE.txt` & `botocore-a-la-carte-entityresolution-1.31.20/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-entityresolution-1.31.19/PKG-INFO` & `botocore-a-la-carte-entityresolution-1.31.20/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: botocore-a-la-carte-entityresolution
-Version: 1.31.19
+Version: 1.31.20
 Summary: entityresolution data for botocore. See the `botocore-a-la-carte` package for more info.
 Home-page: https://github.com/thejcannon/botocore-a-la-carte
 Author: Amazon Web Services
 License: Apache License 2.0
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `botocore-a-la-carte-entityresolution-1.31.19/botocore/data/entityresolution/2018-05-10/endpoint-rule-set-1.json` & `botocore-a-la-carte-entityresolution-1.31.20/botocore/data/entityresolution/2018-05-10/endpoint-rule-set-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-entityresolution-1.31.19/botocore/data/entityresolution/2018-05-10/paginators-1.json` & `botocore-a-la-carte-entityresolution-1.31.20/botocore/data/entityresolution/2018-05-10/paginators-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-entityresolution-1.31.19/botocore/data/entityresolution/2018-05-10/service-2.json` & `botocore-a-la-carte-entityresolution-1.31.20/botocore/data/entityresolution/2018-05-10/service-2.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-entityresolution-1.31.19/botocore_a_la_carte_entityresolution.egg-info/PKG-INFO` & `botocore-a-la-carte-entityresolution-1.31.20/botocore_a_la_carte_entityresolution.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: botocore-a-la-carte-entityresolution
-Version: 1.31.19
+Version: 1.31.20
 Summary: entityresolution data for botocore. See the `botocore-a-la-carte` package for more info.
 Home-page: https://github.com/thejcannon/botocore-a-la-carte
 Author: Amazon Web Services
 License: Apache License 2.0
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `botocore-a-la-carte-entityresolution-1.31.19/setup.py` & `botocore-a-la-carte-entityresolution-1.31.20/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #!/usr/bin/env python
 from setuptools import setup
 
 setup(
     name='botocore-a-la-carte-entityresolution',
-    version="1.31.19",
+    version="1.31.20",
     description='entityresolution data for botocore. See the `botocore-a-la-carte` package for more info.',
     author='Amazon Web Services',
     url='https://github.com/thejcannon/botocore-a-la-carte',
     scripts=[],
     packages=["botocore"],
     package_data={
         'botocore': ['data/entityresolution/*/*.json'],
```


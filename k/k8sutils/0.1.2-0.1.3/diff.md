# Comparing `tmp/k8sutils-0.1.2.tar.gz` & `tmp/k8sutils-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "k8sutils-0.1.2.tar", last modified: Sat Aug  5 21:29:54 2023, max compression
+gzip compressed data, was "k8sutils-0.1.3.tar", last modified: Tue Aug  8 21:33:57 2023, max compression
```

## Comparing `k8sutils-0.1.2.tar` & `k8sutils-0.1.3.tar`

### file list

```diff
@@ -1,27 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 21:29:54.867170 k8sutils-0.1.2/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-08-05 21:29:46.000000 k8sutils-0.1.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      471 2023-08-05 21:29:54.863170 k8sutils-0.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-08-05 21:29:46.000000 k8sutils-0.1.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 21:29:54.863170 k8sutils-0.1.2/k8sutils/
--rw-r--r--   0 runner    (1001) docker     (123)     2877 2023-08-05 21:29:46.000000 k8sutils-0.1.2/k8sutils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 21:29:54.863170 k8sutils-0.1.2/k8sutils/crds/
--rw-r--r--   0 runner    (1001) docker     (123)      255 2023-08-05 21:29:46.000000 k8sutils-0.1.2/k8sutils/crds/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      812 2023-08-05 21:29:46.000000 k8sutils-0.1.2/k8sutils/crds/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 21:29:54.863170 k8sutils-0.1.2/k8sutils/deployments/
--rw-r--r--   0 runner    (1001) docker     (123)      354 2023-08-05 21:29:46.000000 k8sutils-0.1.2/k8sutils/deployments/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1031 2023-08-05 21:29:46.000000 k8sutils-0.1.2/k8sutils/deployments/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 21:29:54.863170 k8sutils-0.1.2/k8sutils/local/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-05 21:29:46.000000 k8sutils-0.1.2/k8sutils/local/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      464 2023-08-05 21:29:46.000000 k8sutils-0.1.2/k8sutils/local/minikube.py
--rw-r--r--   0 runner    (1001) docker     (123)      398 2023-08-05 21:29:46.000000 k8sutils-0.1.2/k8sutils/namespace.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 21:29:54.863170 k8sutils-0.1.2/k8sutils/pods/
--rw-r--r--   0 runner    (1001) docker     (123)      839 2023-08-05 21:29:46.000000 k8sutils-0.1.2/k8sutils/pods/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      944 2023-08-05 21:29:46.000000 k8sutils-0.1.2/k8sutils/pods/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 21:29:54.863170 k8sutils-0.1.2/k8sutils.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      471 2023-08-05 21:29:54.000000 k8sutils-0.1.2/k8sutils.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      449 2023-08-05 21:29:54.000000 k8sutils-0.1.2/k8sutils.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-05 21:29:54.000000 k8sutils-0.1.2/k8sutils.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-08-05 21:29:54.000000 k8sutils-0.1.2/k8sutils.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-08-05 21:29:54.000000 k8sutils-0.1.2/k8sutils.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      663 2023-08-05 21:29:46.000000 k8sutils-0.1.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-05 21:29:54.867170 k8sutils-0.1.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 21:33:57.242173 k8sutils-0.1.3/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-08-08 21:33:48.000000 k8sutils-0.1.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      471 2023-08-08 21:33:57.238172 k8sutils-0.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-08-08 21:33:48.000000 k8sutils-0.1.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 21:33:57.238172 k8sutils-0.1.3/k8sutils/
+-rw-r--r--   0 runner    (1001) docker     (123)     3862 2023-08-08 21:33:48.000000 k8sutils-0.1.3/k8sutils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 21:33:57.238172 k8sutils-0.1.3/k8sutils/crds/
+-rw-r--r--   0 runner    (1001) docker     (123)      255 2023-08-08 21:33:48.000000 k8sutils-0.1.3/k8sutils/crds/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      812 2023-08-08 21:33:48.000000 k8sutils-0.1.3/k8sutils/crds/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 21:33:57.238172 k8sutils-0.1.3/k8sutils/deployments/
+-rw-r--r--   0 runner    (1001) docker     (123)      354 2023-08-08 21:33:48.000000 k8sutils-0.1.3/k8sutils/deployments/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1031 2023-08-08 21:33:48.000000 k8sutils-0.1.3/k8sutils/deployments/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 21:33:57.238172 k8sutils-0.1.3/k8sutils/local/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 21:33:48.000000 k8sutils-0.1.3/k8sutils/local/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      464 2023-08-08 21:33:48.000000 k8sutils-0.1.3/k8sutils/local/minikube.py
+-rw-r--r--   0 runner    (1001) docker     (123)      398 2023-08-08 21:33:48.000000 k8sutils-0.1.3/k8sutils/namespace.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 21:33:57.238172 k8sutils-0.1.3/k8sutils/pods/
+-rw-r--r--   0 runner    (1001) docker     (123)      839 2023-08-08 21:33:48.000000 k8sutils-0.1.3/k8sutils/pods/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      944 2023-08-08 21:33:48.000000 k8sutils-0.1.3/k8sutils/pods/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 21:33:57.238172 k8sutils-0.1.3/k8sutils.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      471 2023-08-08 21:33:57.000000 k8sutils-0.1.3/k8sutils.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      468 2023-08-08 21:33:57.000000 k8sutils-0.1.3/k8sutils.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 21:33:57.000000 k8sutils-0.1.3/k8sutils.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-08-08 21:33:57.000000 k8sutils-0.1.3/k8sutils.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-08-08 21:33:57.000000 k8sutils-0.1.3/k8sutils.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      709 2023-08-08 21:33:48.000000 k8sutils-0.1.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-08 21:33:57.242173 k8sutils-0.1.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 21:33:57.238172 k8sutils-0.1.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1023 2023-08-08 21:33:48.000000 k8sutils-0.1.3/tests/test_yaml.py
```

### Comparing `k8sutils-0.1.2/LICENSE` & `k8sutils-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `k8sutils-0.1.2/k8sutils/__init__.py` & `k8sutils-0.1.3/k8sutils/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -2,14 +2,17 @@
 import os
 from typing import Optional
 
 import requests
 import subprocess
 import tempfile
 from urllib.parse import urlparse
+import yaml
+from dotty_dict import Dotty
+
 
 
 # Configure the logger
 logging.basicConfig(level=logging.DEBUG,
                     format="%(asctime)s %(filename)s %(lineno)d> %(message)s",
                     datefmt="%Y-%m-%d %H:%M:%S")
 
@@ -91,7 +94,37 @@
 
     @staticmethod
     def delete(cluster='kind'):
         logging.info(f"Deleting the kind cluster")
         subprocess.run(f"kind delete cluster --name {cluster}", shell=True, check=True)
 
 
+class Yaml:
+    def __init__(self, path):
+        with open(path, 'r') as file:
+            self.data = Dotty(yaml.safe_load(file))
+
+    def set(self, key, value):
+        keys = key.split(".")
+        item = self.data
+        for i in range(len(keys)):
+            part = keys[i]
+            if "[" in part and "]" in part:
+                sub_key, index_str = part.split("[")
+                index = int(index_str[:-1])  # Convert the index to an integer
+                if sub_key:
+                    item = item[sub_key]
+                if i == len(keys) - 1:
+                    item[index] = value
+                else:
+                    item = item[index]
+            else:
+                if i == len(keys) - 1:
+                    item[part] = value
+                else:
+                    item = item[part]
+
+
+
+    def save(self, path):
+        with open(path, 'w') as file:
+            yaml.safe_dump(self.data.to_dict(), file)
```

### Comparing `k8sutils-0.1.2/k8sutils/crds/utils.py` & `k8sutils-0.1.3/k8sutils/crds/utils.py`

 * *Files identical despite different names*

### Comparing `k8sutils-0.1.2/k8sutils/deployments/utils.py` & `k8sutils-0.1.3/k8sutils/deployments/utils.py`

 * *Files identical despite different names*

### Comparing `k8sutils-0.1.2/k8sutils/pods/__init__.py` & `k8sutils-0.1.3/k8sutils/pods/__init__.py`

 * *Files identical despite different names*

### Comparing `k8sutils-0.1.2/k8sutils/pods/utils.py` & `k8sutils-0.1.3/k8sutils/pods/utils.py`

 * *Files identical despite different names*

### Comparing `k8sutils-0.1.2/pyproject.toml` & `k8sutils-0.1.3/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,26 +1,28 @@
 [build-system]
 requires = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "k8sutils"
-version = "0.1.2"
+version = "0.1.3"
 description = "Kubernetes helper module for Python"
 authors = [{ name = "Rui Vieira", email = "ruidevieira@googlemail.com" }]
 license = { text = "Apache License Version 2.0" }
 readme = "README.md"
 classifiers = [
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
 ]
 keywords = ["k8s", "kubernetes", "utilities"]
 dependencies = [
-    "requests==2.25.1",
+    "requests==2.28.0",
     "termcolor==1.1.0",
-    "prettytable==2.1.0"
+    "prettytable==2.1.0",
+    "PyYAML==6.0.1",
+    "dotty-dict==1.3.1"
 ]
 requires-python = ">=3.8"
 
 
 [project.optional-dependencies]
 dev = ["pytest==6.2.2"]
```


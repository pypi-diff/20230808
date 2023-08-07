# Comparing `tmp/metricsoperator-0.0.11.tar.gz` & `tmp/metricsoperator-0.0.12.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "metricsoperator-0.0.11.tar", last modified: Mon Aug  7 05:12:33 2023, max compression
+gzip compressed data, was "metricsoperator-0.0.12.tar", last modified: Mon Aug  7 12:53:34 2023, max compression
```

## Comparing `metricsoperator-0.0.11.tar` & `metricsoperator-0.0.12.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 05:12:33.733519 metricsoperator-0.0.11/
--rw-r--r--   0 runner    (1001) docker     (123)      169 2023-08-07 05:12:02.000000 metricsoperator-0.0.11/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1935 2023-08-07 05:12:33.733519 metricsoperator-0.0.11/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1100 2023-08-07 05:12:02.000000 metricsoperator-0.0.11/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 05:12:33.733519 metricsoperator-0.0.11/metricsoperator/
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-08-07 05:12:02.000000 metricsoperator-0.0.11/metricsoperator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1535 2023-08-07 05:12:02.000000 metricsoperator-0.0.11/metricsoperator/client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 05:12:33.733519 metricsoperator-0.0.11/metricsoperator/metrics/
--rw-r--r--   0 runner    (1001) docker     (123)      482 2023-08-07 05:12:02.000000 metricsoperator-0.0.11/metricsoperator/metrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6678 2023-08-07 05:12:02.000000 metricsoperator-0.0.11/metricsoperator/metrics/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2406 2023-08-07 05:12:02.000000 metricsoperator-0.0.11/metricsoperator/metrics/network.py
--rw-r--r--   0 runner    (1001) docker     (123)      930 2023-08-07 05:12:02.000000 metricsoperator-0.0.11/metricsoperator/metrics/storage.py
--rw-r--r--   0 runner    (1001) docker     (123)      613 2023-08-07 05:12:02.000000 metricsoperator-0.0.11/metricsoperator/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 05:12:33.733519 metricsoperator-0.0.11/metricsoperator.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1935 2023-08-07 05:12:33.000000 metricsoperator-0.0.11/metricsoperator.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      494 2023-08-07 05:12:33.000000 metricsoperator-0.0.11/metricsoperator.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-07 05:12:33.000000 metricsoperator-0.0.11/metricsoperator.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-07 05:12:33.000000 metricsoperator-0.0.11/metricsoperator.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-08-07 05:12:33.000000 metricsoperator-0.0.11/metricsoperator.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-08-07 05:12:33.000000 metricsoperator-0.0.11/metricsoperator.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      132 2023-08-07 05:12:02.000000 metricsoperator-0.0.11/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-07 05:12:33.733519 metricsoperator-0.0.11/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2257 2023-08-07 05:12:02.000000 metricsoperator-0.0.11/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 12:53:34.910854 metricsoperator-0.0.12/
+-rw-r--r--   0 runner    (1001) docker     (123)      169 2023-08-07 12:53:07.000000 metricsoperator-0.0.12/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1935 2023-08-07 12:53:34.910854 metricsoperator-0.0.12/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1100 2023-08-07 12:53:07.000000 metricsoperator-0.0.12/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 12:53:34.910854 metricsoperator-0.0.12/metricsoperator/
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-08-07 12:53:07.000000 metricsoperator-0.0.12/metricsoperator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1535 2023-08-07 12:53:07.000000 metricsoperator-0.0.12/metricsoperator/client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 12:53:34.910854 metricsoperator-0.0.12/metricsoperator/metrics/
+-rw-r--r--   0 runner    (1001) docker     (123)      539 2023-08-07 12:53:07.000000 metricsoperator-0.0.12/metricsoperator/metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6678 2023-08-07 12:53:07.000000 metricsoperator-0.0.12/metricsoperator/metrics/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4453 2023-08-07 12:53:07.000000 metricsoperator-0.0.12/metricsoperator/metrics/network.py
+-rw-r--r--   0 runner    (1001) docker     (123)      930 2023-08-07 12:53:07.000000 metricsoperator-0.0.12/metricsoperator/metrics/storage.py
+-rw-r--r--   0 runner    (1001) docker     (123)      613 2023-08-07 12:53:07.000000 metricsoperator-0.0.12/metricsoperator/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 12:53:34.910854 metricsoperator-0.0.12/metricsoperator.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1935 2023-08-07 12:53:34.000000 metricsoperator-0.0.12/metricsoperator.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      494 2023-08-07 12:53:34.000000 metricsoperator-0.0.12/metricsoperator.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-07 12:53:34.000000 metricsoperator-0.0.12/metricsoperator.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-07 12:53:34.000000 metricsoperator-0.0.12/metricsoperator.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-08-07 12:53:34.000000 metricsoperator-0.0.12/metricsoperator.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-08-07 12:53:34.000000 metricsoperator-0.0.12/metricsoperator.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      132 2023-08-07 12:53:07.000000 metricsoperator-0.0.12/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-07 12:53:34.910854 metricsoperator-0.0.12/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2257 2023-08-07 12:53:07.000000 metricsoperator-0.0.12/setup.py
```

### Comparing `metricsoperator-0.0.11/PKG-INFO` & `metricsoperator-0.0.12/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: metricsoperator
-Version: 0.0.11
+Version: 0.0.12
 Summary: Python helpers for the Metrics Operator
 Home-page: https://github.com/converged-computing/metrics-operator/tree/main/python-sdk/v1alpha1
 Author: Vanessasaurus
 Author-email: vsoch@users.noreply.github.com
 Maintainer: Vanessasaurus
 License: MIT
 Keywords: metrics-operator,hpc,kubernetes,metrics,storage,applications
```

### Comparing `metricsoperator-0.0.11/README.md` & `metricsoperator-0.0.12/README.md`

 * *Files identical despite different names*

### Comparing `metricsoperator-0.0.11/metricsoperator/client.py` & `metricsoperator-0.0.12/metricsoperator/client.py`

 * *Files identical despite different names*

### Comparing `metricsoperator-0.0.11/metricsoperator/metrics/base.py` & `metricsoperator-0.0.12/metricsoperator/metrics/base.py`

 * *Files identical despite different names*

### Comparing `metricsoperator-0.0.11/metricsoperator/metrics/storage.py` & `metricsoperator-0.0.12/metricsoperator/metrics/storage.py`

 * *Files identical despite different names*

### Comparing `metricsoperator-0.0.11/metricsoperator/utils.py` & `metricsoperator-0.0.12/metricsoperator/utils.py`

 * *Files identical despite different names*

### Comparing `metricsoperator-0.0.11/metricsoperator.egg-info/PKG-INFO` & `metricsoperator-0.0.12/metricsoperator.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: metricsoperator
-Version: 0.0.11
+Version: 0.0.12
 Summary: Python helpers for the Metrics Operator
 Home-page: https://github.com/converged-computing/metrics-operator/tree/main/python-sdk/v1alpha1
 Author: Vanessasaurus
 Author-email: vsoch@users.noreply.github.com
 Maintainer: Vanessasaurus
 License: MIT
 Keywords: metrics-operator,hpc,kubernetes,metrics,storage,applications
```

### Comparing `metricsoperator-0.0.11/setup.py` & `metricsoperator-0.0.12/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 ################################################################################
 # MAIN #########################################################################
 ################################################################################
 
 if __name__ == "__main__":
     setup(
         name="metricsoperator",
-        version="0.0.11",
+        version="0.0.12",
         author="Vanessasaurus",
         author_email="vsoch@users.noreply.github.com",
         maintainer="Vanessasaurus",
         packages=find_packages(),
         include_package_data=True,
         zip_safe=False,
         url="https://github.com/converged-computing/metrics-operator/tree/main/python-sdk/v1alpha1",
```


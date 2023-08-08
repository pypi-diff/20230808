# Comparing `tmp/scikit-datasets-0.2.3.tar.gz` & `tmp/scikit-datasets-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scikit-datasets-0.2.3.tar", last modified: Mon Jun 19 21:43:22 2023, max compression
+gzip compressed data, was "scikit-datasets-0.2.4.tar", last modified: Tue Aug  8 14:00:26 2023, max compression
```

## Comparing `scikit-datasets-0.2.3.tar` & `scikit-datasets-0.2.4.tar`

### file list

```diff
@@ -1,56 +1,56 @@
-drwxr-xr-x   0 david     (1000) david     (1000)        0 2023-06-19 21:43:22.228542 scikit-datasets-0.2.3/
--rw-------   0 david     (1000) david     (1000)     1094 2023-03-23 22:36:09.000000 scikit-datasets-0.2.3/LICENSE
--rw-r--r--   0 david     (1000) david     (1000)     4060 2023-06-19 21:43:22.229545 scikit-datasets-0.2.3/PKG-INFO
--rw-------   0 david     (1000) david     (1000)     1451 2023-03-23 22:36:09.000000 scikit-datasets-0.2.3/README.md
--rw-r--r--   0 david     (1000) david     (1000)     1788 2023-06-19 21:40:43.000000 scikit-datasets-0.2.3/pyproject.toml
-drwxr-xr-x   0 david     (1000) david     (1000)        0 2023-06-19 21:43:20.844542 scikit-datasets-0.2.3/scikit_datasets.egg-info/
--rw-r--r--   0 david     (1000) david     (1000)     4060 2023-06-19 21:43:20.000000 scikit-datasets-0.2.3/scikit_datasets.egg-info/PKG-INFO
--rw-r--r--   0 david     (1000) david     (1000)     1596 2023-06-19 21:43:20.000000 scikit-datasets-0.2.3/scikit_datasets.egg-info/SOURCES.txt
--rw-r--r--   0 david     (1000) david     (1000)        1 2023-06-19 21:43:20.000000 scikit-datasets-0.2.3/scikit_datasets.egg-info/dependency_links.txt
--rw-r--r--   0 david     (1000) david     (1000)      391 2023-06-19 21:43:20.000000 scikit-datasets-0.2.3/scikit_datasets.egg-info/requires.txt
--rw-r--r--   0 david     (1000) david     (1000)       11 2023-06-19 21:43:20.000000 scikit-datasets-0.2.3/scikit_datasets.egg-info/top_level.txt
--rw-------   0 david     (1000) david     (1000)      377 2023-06-19 21:43:22.236544 scikit-datasets-0.2.3/setup.cfg
--rwx------   0 david     (1000) david     (1000)      132 2023-03-23 22:36:09.000000 scikit-datasets-0.2.3/setup.py
-drwxr-xr-x   0 david     (1000) david     (1000)        0 2023-06-19 21:43:20.866542 scikit-datasets-0.2.3/skdatasets/
--rw-------   0 david     (1000) david     (1000)      115 2023-03-23 22:36:09.000000 scikit-datasets-0.2.3/skdatasets/__init__.py
-drwxr-xr-x   0 david     (1000) david     (1000)        0 2023-06-19 21:43:21.233543 scikit-datasets-0.2.3/skdatasets/repositories/
--rw-------   0 david     (1000) david     (1000)      918 2023-03-23 22:36:09.000000 scikit-datasets-0.2.3/skdatasets/repositories/__init__.py
--rw-------   0 david     (1000) david     (1000)     3039 2023-03-23 22:36:09.000000 scikit-datasets-0.2.3/skdatasets/repositories/aneurisk.py
--rw-------   0 david     (1000) david     (1000)     9085 2023-03-23 22:36:09.000000 scikit-datasets-0.2.3/skdatasets/repositories/base.py
--rw-------   0 david     (1000) david     (1000)    11861 2023-03-23 22:36:09.000000 scikit-datasets-0.2.3/skdatasets/repositories/cran.py
--rw-------   0 david     (1000) david     (1000)     2774 2023-03-23 22:36:09.000000 scikit-datasets-0.2.3/skdatasets/repositories/forex.py
--rw-------   0 david     (1000) david     (1000)     9579 2023-03-23 22:36:09.000000 scikit-datasets-0.2.3/skdatasets/repositories/keel.py
--rw-------   0 david     (1000) david     (1000)     2426 2023-03-23 22:36:09.000000 scikit-datasets-0.2.3/skdatasets/repositories/keras.py
--rw-------   0 david     (1000) david     (1000)     6645 2023-03-23 22:36:09.000000 scikit-datasets-0.2.3/skdatasets/repositories/libsvm.py
--rw-------   0 david     (1000) david     (1000)     6713 2023-03-23 22:36:09.000000 scikit-datasets-0.2.3/skdatasets/repositories/physionet.py
--rw-------   0 david     (1000) david     (1000)     4939 2023-03-23 22:36:09.000000 scikit-datasets-0.2.3/skdatasets/repositories/raetsch.py
--rw-------   0 david     (1000) david     (1000)     3244 2023-03-23 22:36:10.000000 scikit-datasets-0.2.3/skdatasets/repositories/sklearn.py
--rw-------   0 david     (1000) david     (1000)     4960 2023-03-23 22:36:10.000000 scikit-datasets-0.2.3/skdatasets/repositories/uci.py
--rw-r--r--   0 david     (1000) david     (1000)     4852 2023-06-19 21:36:27.000000 scikit-datasets-0.2.3/skdatasets/repositories/ucr.py
-drwxr-xr-x   0 david     (1000) david     (1000)        0 2023-06-19 21:43:21.261553 scikit-datasets-0.2.3/skdatasets/tests/
--rw-------   0 david     (1000) david     (1000)        0 2023-03-23 22:36:10.000000 scikit-datasets-0.2.3/skdatasets/tests/__init__.py
-drwxr-xr-x   0 david     (1000) david     (1000)        0 2023-06-19 21:43:21.720542 scikit-datasets-0.2.3/skdatasets/tests/repositories/
--rw-------   0 david     (1000) david     (1000)     1254 2023-03-23 22:36:10.000000 scikit-datasets-0.2.3/skdatasets/tests/repositories/__init__.py
--rw-------   0 david     (1000) david     (1000)      310 2023-03-23 22:36:10.000000 scikit-datasets-0.2.3/skdatasets/tests/repositories/test_cran.py
--rw-------   0 david     (1000) david     (1000)      928 2023-03-23 22:36:10.000000 scikit-datasets-0.2.3/skdatasets/tests/repositories/test_forex.py
--rw-------   0 david     (1000) david     (1000)     1655 2023-03-23 22:36:10.000000 scikit-datasets-0.2.3/skdatasets/tests/repositories/test_keel.py
--rw-------   0 david     (1000) david     (1000)      867 2023-03-23 22:36:10.000000 scikit-datasets-0.2.3/skdatasets/tests/repositories/test_keras.py
--rw-------   0 david     (1000) david     (1000)     2776 2023-03-23 22:36:10.000000 scikit-datasets-0.2.3/skdatasets/tests/repositories/test_libsvm.py
--rw-------   0 david     (1000) david     (1000)     1259 2023-03-23 22:36:10.000000 scikit-datasets-0.2.3/skdatasets/tests/repositories/test_physionet.py
--rw-------   0 david     (1000) david     (1000)      728 2023-03-23 22:36:10.000000 scikit-datasets-0.2.3/skdatasets/tests/repositories/test_raetsch.py
--rw-------   0 david     (1000) david     (1000)      503 2023-03-23 22:36:10.000000 scikit-datasets-0.2.3/skdatasets/tests/repositories/test_sklearn.py
--rw-------   0 david     (1000) david     (1000)      647 2023-03-23 22:36:10.000000 scikit-datasets-0.2.3/skdatasets/tests/repositories/test_uci.py
--rw-------   0 david     (1000) david     (1000)      754 2023-03-23 22:36:10.000000 scikit-datasets-0.2.3/skdatasets/tests/repositories/test_ucr.py
-drwxr-xr-x   0 david     (1000) david     (1000)        0 2023-06-19 21:43:22.049544 scikit-datasets-0.2.3/skdatasets/tests/utils/
--rw-------   0 david     (1000) david     (1000)        0 2023-03-23 22:36:10.000000 scikit-datasets-0.2.3/skdatasets/tests/utils/__init__.py
--rw-------   0 david     (1000) david     (1000)      142 2023-03-23 22:36:10.000000 scikit-datasets-0.2.3/skdatasets/tests/utils/linear_model.py
--rwx------   0 david     (1000) david     (1000)     1180 2023-03-23 22:36:10.000000 scikit-datasets-0.2.3/skdatasets/tests/utils/run.py
--rw-------   0 david     (1000) david     (1000)      609 2023-03-23 22:36:10.000000 scikit-datasets-0.2.3/skdatasets/tests/utils/test_estimator.py
--rw-r--r--   0 david     (1000) david     (1000)     6083 2023-06-19 21:36:27.000000 scikit-datasets-0.2.3/skdatasets/tests/utils/test_experiment.py
--rw-------   0 david     (1000) david     (1000)     2714 2023-03-23 22:36:10.000000 scikit-datasets-0.2.3/skdatasets/tests/utils/test_run.py
--rw-------   0 david     (1000) david     (1000)     2303 2023-03-23 22:36:10.000000 scikit-datasets-0.2.3/skdatasets/tests/utils/test_scores.py
-drwxr-xr-x   0 david     (1000) david     (1000)        0 2023-06-19 21:43:22.198543 scikit-datasets-0.2.3/skdatasets/utils/
--rw-------   0 david     (1000) david     (1000)        0 2023-03-23 22:36:10.000000 scikit-datasets-0.2.3/skdatasets/utils/__init__.py
--rw-------   0 david     (1000) david     (1000)      760 2023-03-23 22:36:10.000000 scikit-datasets-0.2.3/skdatasets/utils/estimator.py
--rwxr-xr-x   0 david     (1000) david     (1000)    26235 2023-06-19 21:36:27.000000 scikit-datasets-0.2.3/skdatasets/utils/experiment.py
--rw-r--r--   0 david     (1000) david     (1000)    19341 2023-06-19 21:36:27.000000 scikit-datasets-0.2.3/skdatasets/utils/scores.py
+drwxr-xr-x   0 david     (1000) david     (1000)        0 2023-08-08 14:00:26.515160 scikit-datasets-0.2.4/
+-rw-------   0 david     (1000) david     (1000)     1094 2023-06-29 22:39:52.000000 scikit-datasets-0.2.4/LICENSE
+-rw-r--r--   0 david     (1000) david     (1000)     4060 2023-08-08 14:00:26.517157 scikit-datasets-0.2.4/PKG-INFO
+-rw-------   0 david     (1000) david     (1000)     1451 2023-06-29 22:39:52.000000 scikit-datasets-0.2.4/README.md
+-rw-------   0 david     (1000) david     (1000)     1788 2023-08-08 13:52:57.000000 scikit-datasets-0.2.4/pyproject.toml
+drwxr-xr-x   0 david     (1000) david     (1000)        0 2023-08-08 14:00:25.190424 scikit-datasets-0.2.4/scikit_datasets.egg-info/
+-rw-r--r--   0 david     (1000) david     (1000)     4060 2023-08-08 14:00:24.000000 scikit-datasets-0.2.4/scikit_datasets.egg-info/PKG-INFO
+-rw-r--r--   0 david     (1000) david     (1000)     1596 2023-08-08 14:00:24.000000 scikit-datasets-0.2.4/scikit_datasets.egg-info/SOURCES.txt
+-rw-r--r--   0 david     (1000) david     (1000)        1 2023-08-08 14:00:24.000000 scikit-datasets-0.2.4/scikit_datasets.egg-info/dependency_links.txt
+-rw-r--r--   0 david     (1000) david     (1000)      391 2023-08-08 14:00:24.000000 scikit-datasets-0.2.4/scikit_datasets.egg-info/requires.txt
+-rw-r--r--   0 david     (1000) david     (1000)       11 2023-08-08 14:00:24.000000 scikit-datasets-0.2.4/scikit_datasets.egg-info/top_level.txt
+-rw-------   0 david     (1000) david     (1000)      377 2023-08-08 14:00:26.523686 scikit-datasets-0.2.4/setup.cfg
+-rwx------   0 david     (1000) david     (1000)      132 2023-06-29 22:39:52.000000 scikit-datasets-0.2.4/setup.py
+drwxr-xr-x   0 david     (1000) david     (1000)        0 2023-08-08 14:00:25.220389 scikit-datasets-0.2.4/skdatasets/
+-rw-------   0 david     (1000) david     (1000)      115 2023-06-29 22:39:52.000000 scikit-datasets-0.2.4/skdatasets/__init__.py
+drwxr-xr-x   0 david     (1000) david     (1000)        0 2023-08-08 14:00:25.611973 scikit-datasets-0.2.4/skdatasets/repositories/
+-rw-------   0 david     (1000) david     (1000)      918 2023-06-29 22:39:52.000000 scikit-datasets-0.2.4/skdatasets/repositories/__init__.py
+-rw-------   0 david     (1000) david     (1000)     3039 2023-06-29 22:39:52.000000 scikit-datasets-0.2.4/skdatasets/repositories/aneurisk.py
+-rw-------   0 david     (1000) david     (1000)     9085 2023-06-29 22:39:52.000000 scikit-datasets-0.2.4/skdatasets/repositories/base.py
+-rw-------   0 david     (1000) david     (1000)    11861 2023-06-29 22:39:52.000000 scikit-datasets-0.2.4/skdatasets/repositories/cran.py
+-rw-------   0 david     (1000) david     (1000)     2774 2023-06-29 22:39:52.000000 scikit-datasets-0.2.4/skdatasets/repositories/forex.py
+-rw-------   0 david     (1000) david     (1000)     9579 2023-06-29 22:39:52.000000 scikit-datasets-0.2.4/skdatasets/repositories/keel.py
+-rw-------   0 david     (1000) david     (1000)     2426 2023-06-29 22:39:52.000000 scikit-datasets-0.2.4/skdatasets/repositories/keras.py
+-rw-------   0 david     (1000) david     (1000)     6645 2023-06-29 22:39:52.000000 scikit-datasets-0.2.4/skdatasets/repositories/libsvm.py
+-rw-------   0 david     (1000) david     (1000)     6713 2023-06-29 22:39:52.000000 scikit-datasets-0.2.4/skdatasets/repositories/physionet.py
+-rw-------   0 david     (1000) david     (1000)     4939 2023-06-29 22:39:52.000000 scikit-datasets-0.2.4/skdatasets/repositories/raetsch.py
+-rw-------   0 david     (1000) david     (1000)     3244 2023-06-29 22:39:52.000000 scikit-datasets-0.2.4/skdatasets/repositories/sklearn.py
+-rw-------   0 david     (1000) david     (1000)     4960 2023-06-29 22:39:52.000000 scikit-datasets-0.2.4/skdatasets/repositories/uci.py
+-rw-r--r--   0 david     (1000) david     (1000)     4842 2023-08-08 13:49:33.000000 scikit-datasets-0.2.4/skdatasets/repositories/ucr.py
+drwxr-xr-x   0 david     (1000) david     (1000)        0 2023-08-08 14:00:25.638641 scikit-datasets-0.2.4/skdatasets/tests/
+-rw-------   0 david     (1000) david     (1000)        0 2023-06-29 22:39:52.000000 scikit-datasets-0.2.4/skdatasets/tests/__init__.py
+drwxr-xr-x   0 david     (1000) david     (1000)        0 2023-08-08 14:00:26.061967 scikit-datasets-0.2.4/skdatasets/tests/repositories/
+-rw-------   0 david     (1000) david     (1000)     1254 2023-06-29 22:39:52.000000 scikit-datasets-0.2.4/skdatasets/tests/repositories/__init__.py
+-rw-------   0 david     (1000) david     (1000)      310 2023-06-29 22:39:53.000000 scikit-datasets-0.2.4/skdatasets/tests/repositories/test_cran.py
+-rw-------   0 david     (1000) david     (1000)      928 2023-06-29 22:39:53.000000 scikit-datasets-0.2.4/skdatasets/tests/repositories/test_forex.py
+-rw-------   0 david     (1000) david     (1000)     1655 2023-06-29 22:39:53.000000 scikit-datasets-0.2.4/skdatasets/tests/repositories/test_keel.py
+-rw-------   0 david     (1000) david     (1000)      867 2023-06-29 22:39:53.000000 scikit-datasets-0.2.4/skdatasets/tests/repositories/test_keras.py
+-rw-------   0 david     (1000) david     (1000)     2776 2023-06-29 22:39:53.000000 scikit-datasets-0.2.4/skdatasets/tests/repositories/test_libsvm.py
+-rw-------   0 david     (1000) david     (1000)     1259 2023-06-29 22:39:53.000000 scikit-datasets-0.2.4/skdatasets/tests/repositories/test_physionet.py
+-rw-------   0 david     (1000) david     (1000)      728 2023-06-29 22:39:53.000000 scikit-datasets-0.2.4/skdatasets/tests/repositories/test_raetsch.py
+-rw-------   0 david     (1000) david     (1000)      503 2023-06-29 22:39:53.000000 scikit-datasets-0.2.4/skdatasets/tests/repositories/test_sklearn.py
+-rw-------   0 david     (1000) david     (1000)      647 2023-06-29 22:39:53.000000 scikit-datasets-0.2.4/skdatasets/tests/repositories/test_uci.py
+-rw-------   0 david     (1000) david     (1000)      754 2023-06-29 22:39:53.000000 scikit-datasets-0.2.4/skdatasets/tests/repositories/test_ucr.py
+drwxr-xr-x   0 david     (1000) david     (1000)        0 2023-08-08 14:00:26.363405 scikit-datasets-0.2.4/skdatasets/tests/utils/
+-rw-------   0 david     (1000) david     (1000)        0 2023-06-29 22:39:53.000000 scikit-datasets-0.2.4/skdatasets/tests/utils/__init__.py
+-rw-------   0 david     (1000) david     (1000)      142 2023-06-29 22:39:53.000000 scikit-datasets-0.2.4/skdatasets/tests/utils/linear_model.py
+-rwx------   0 david     (1000) david     (1000)     1180 2023-06-29 22:39:53.000000 scikit-datasets-0.2.4/skdatasets/tests/utils/run.py
+-rw-------   0 david     (1000) david     (1000)      609 2023-06-29 22:39:53.000000 scikit-datasets-0.2.4/skdatasets/tests/utils/test_estimator.py
+-rw-------   0 david     (1000) david     (1000)     6083 2023-06-29 22:39:53.000000 scikit-datasets-0.2.4/skdatasets/tests/utils/test_experiment.py
+-rw-------   0 david     (1000) david     (1000)     2714 2023-06-29 22:39:53.000000 scikit-datasets-0.2.4/skdatasets/tests/utils/test_run.py
+-rw-------   0 david     (1000) david     (1000)     2303 2023-06-29 22:39:53.000000 scikit-datasets-0.2.4/skdatasets/tests/utils/test_scores.py
+drwxr-xr-x   0 david     (1000) david     (1000)        0 2023-08-08 14:00:26.488520 scikit-datasets-0.2.4/skdatasets/utils/
+-rw-------   0 david     (1000) david     (1000)        0 2023-06-29 22:39:53.000000 scikit-datasets-0.2.4/skdatasets/utils/__init__.py
+-rw-------   0 david     (1000) david     (1000)      760 2023-06-29 22:39:53.000000 scikit-datasets-0.2.4/skdatasets/utils/estimator.py
+-rwx------   0 david     (1000) david     (1000)    26235 2023-06-29 22:39:53.000000 scikit-datasets-0.2.4/skdatasets/utils/experiment.py
+-rw-------   0 david     (1000) david     (1000)    19341 2023-06-29 22:39:53.000000 scikit-datasets-0.2.4/skdatasets/utils/scores.py
```

### Comparing `scikit-datasets-0.2.3/LICENSE` & `scikit-datasets-0.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `scikit-datasets-0.2.3/PKG-INFO` & `scikit-datasets-0.2.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scikit-datasets
-Version: 0.2.3
+Version: 0.2.4
 Summary: Scikit-learn-compatible datasets
 Author-email: David Diaz Vico <david.diaz.vico@outlook.com>, Carlos Ramos Carreño <vnmabus@gmail.com>
 Maintainer-email: David Diaz Vico <david.diaz.vico@outlook.com>, Carlos Ramos Carreño <vnmabus@gmail.com>
 License: MIT License
         
         Copyright (c) 2017 David Díaz Vico
```

### Comparing `scikit-datasets-0.2.3/README.md` & `scikit-datasets-0.2.4/README.md`

 * *Files identical despite different names*

### Comparing `scikit-datasets-0.2.3/pyproject.toml` & `scikit-datasets-0.2.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "scikit-datasets"
-version = "0.2.3"
+version = "0.2.4"
 description = "Scikit-learn-compatible datasets"
 readme = "README.md"
 requires-python = ">=3.8"
 license = {file = "LICENSE"}
 keywords = ["scikit-learn", "datasets", "repository", "benchmark", "Python"]
 authors = [
   {name = "David Diaz Vico", email = "david.diaz.vico@outlook.com"},
```

### Comparing `scikit-datasets-0.2.3/scikit_datasets.egg-info/PKG-INFO` & `scikit-datasets-0.2.4/scikit_datasets.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scikit-datasets
-Version: 0.2.3
+Version: 0.2.4
 Summary: Scikit-learn-compatible datasets
 Author-email: David Diaz Vico <david.diaz.vico@outlook.com>, Carlos Ramos Carreño <vnmabus@gmail.com>
 Maintainer-email: David Diaz Vico <david.diaz.vico@outlook.com>, Carlos Ramos Carreño <vnmabus@gmail.com>
 License: MIT License
         
         Copyright (c) 2017 David Díaz Vico
```

### Comparing `scikit-datasets-0.2.3/scikit_datasets.egg-info/SOURCES.txt` & `scikit-datasets-0.2.4/scikit_datasets.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `scikit-datasets-0.2.3/skdatasets/repositories/__init__.py` & `scikit-datasets-0.2.4/skdatasets/repositories/__init__.py`

 * *Files identical despite different names*

### Comparing `scikit-datasets-0.2.3/skdatasets/repositories/aneurisk.py` & `scikit-datasets-0.2.4/skdatasets/repositories/aneurisk.py`

 * *Files identical despite different names*

### Comparing `scikit-datasets-0.2.3/skdatasets/repositories/base.py` & `scikit-datasets-0.2.4/skdatasets/repositories/base.py`

 * *Files identical despite different names*

### Comparing `scikit-datasets-0.2.3/skdatasets/repositories/cran.py` & `scikit-datasets-0.2.4/skdatasets/repositories/cran.py`

 * *Files identical despite different names*

### Comparing `scikit-datasets-0.2.3/skdatasets/repositories/forex.py` & `scikit-datasets-0.2.4/skdatasets/repositories/forex.py`

 * *Files identical despite different names*

### Comparing `scikit-datasets-0.2.3/skdatasets/repositories/keel.py` & `scikit-datasets-0.2.4/skdatasets/repositories/keel.py`

 * *Files identical despite different names*

### Comparing `scikit-datasets-0.2.3/skdatasets/repositories/keras.py` & `scikit-datasets-0.2.4/skdatasets/repositories/keras.py`

 * *Files identical despite different names*

### Comparing `scikit-datasets-0.2.3/skdatasets/repositories/libsvm.py` & `scikit-datasets-0.2.4/skdatasets/repositories/libsvm.py`

 * *Files identical despite different names*

### Comparing `scikit-datasets-0.2.3/skdatasets/repositories/physionet.py` & `scikit-datasets-0.2.4/skdatasets/repositories/physionet.py`

 * *Files identical despite different names*

### Comparing `scikit-datasets-0.2.3/skdatasets/repositories/raetsch.py` & `scikit-datasets-0.2.4/skdatasets/repositories/raetsch.py`

 * *Files identical despite different names*

### Comparing `scikit-datasets-0.2.3/skdatasets/repositories/sklearn.py` & `scikit-datasets-0.2.4/skdatasets/repositories/sklearn.py`

 * *Files identical despite different names*

### Comparing `scikit-datasets-0.2.3/skdatasets/repositories/uci.py` & `scikit-datasets-0.2.4/skdatasets/repositories/uci.py`

 * *Files identical despite different names*

### Comparing `scikit-datasets-0.2.3/skdatasets/repositories/ucr.py` & `scikit-datasets-0.2.4/skdatasets/repositories/ucr.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
 import numpy as np
 import scipy.io.arff
 from sklearn.utils import Bunch
 
 from .base import fetch_zip as _fetch_zip
 
-BASE_URL: Final = "http://www.timeseriesclassification.com/ClassificationDownloads/"
+BASE_URL: Final = "https://www.timeseriesclassification.com/aeon-toolkit/"
 
 
 def _target_conversion(
     target: np.typing.NDArray[Union[int, str]],
 ) -> Tuple[np.typing.NDArray[int], Sequence[str]]:
     try:
         target_data = target.astype(int)
```

### Comparing `scikit-datasets-0.2.3/skdatasets/tests/repositories/__init__.py` & `scikit-datasets-0.2.4/skdatasets/tests/repositories/__init__.py`

 * *Files identical despite different names*

### Comparing `scikit-datasets-0.2.3/skdatasets/tests/repositories/test_forex.py` & `scikit-datasets-0.2.4/skdatasets/tests/repositories/test_forex.py`

 * *Files identical despite different names*

### Comparing `scikit-datasets-0.2.3/skdatasets/tests/repositories/test_keel.py` & `scikit-datasets-0.2.4/skdatasets/tests/repositories/test_keel.py`

 * *Files identical despite different names*

### Comparing `scikit-datasets-0.2.3/skdatasets/tests/repositories/test_keras.py` & `scikit-datasets-0.2.4/skdatasets/tests/repositories/test_keras.py`

 * *Files identical despite different names*

### Comparing `scikit-datasets-0.2.3/skdatasets/tests/repositories/test_libsvm.py` & `scikit-datasets-0.2.4/skdatasets/tests/repositories/test_libsvm.py`

 * *Files identical despite different names*

### Comparing `scikit-datasets-0.2.3/skdatasets/tests/repositories/test_physionet.py` & `scikit-datasets-0.2.4/skdatasets/tests/repositories/test_physionet.py`

 * *Files identical despite different names*

### Comparing `scikit-datasets-0.2.3/skdatasets/tests/repositories/test_raetsch.py` & `scikit-datasets-0.2.4/skdatasets/tests/repositories/test_raetsch.py`

 * *Files identical despite different names*

### Comparing `scikit-datasets-0.2.3/skdatasets/tests/repositories/test_uci.py` & `scikit-datasets-0.2.4/skdatasets/tests/repositories/test_uci.py`

 * *Files identical despite different names*

### Comparing `scikit-datasets-0.2.3/skdatasets/tests/repositories/test_ucr.py` & `scikit-datasets-0.2.4/skdatasets/tests/repositories/test_ucr.py`

 * *Files identical despite different names*

### Comparing `scikit-datasets-0.2.3/skdatasets/tests/utils/run.py` & `scikit-datasets-0.2.4/skdatasets/tests/utils/run.py`

 * *Files identical despite different names*

### Comparing `scikit-datasets-0.2.3/skdatasets/tests/utils/test_estimator.py` & `scikit-datasets-0.2.4/skdatasets/tests/utils/test_estimator.py`

 * *Files identical despite different names*

### Comparing `scikit-datasets-0.2.3/skdatasets/tests/utils/test_experiment.py` & `scikit-datasets-0.2.4/skdatasets/tests/utils/test_experiment.py`

 * *Files identical despite different names*

### Comparing `scikit-datasets-0.2.3/skdatasets/tests/utils/test_run.py` & `scikit-datasets-0.2.4/skdatasets/tests/utils/test_run.py`

 * *Files identical despite different names*

### Comparing `scikit-datasets-0.2.3/skdatasets/tests/utils/test_scores.py` & `scikit-datasets-0.2.4/skdatasets/tests/utils/test_scores.py`

 * *Files identical despite different names*

### Comparing `scikit-datasets-0.2.3/skdatasets/utils/estimator.py` & `scikit-datasets-0.2.4/skdatasets/utils/estimator.py`

 * *Files identical despite different names*

### Comparing `scikit-datasets-0.2.3/skdatasets/utils/experiment.py` & `scikit-datasets-0.2.4/skdatasets/utils/experiment.py`

 * *Files identical despite different names*

### Comparing `scikit-datasets-0.2.3/skdatasets/utils/scores.py` & `scikit-datasets-0.2.4/skdatasets/utils/scores.py`

 * *Files identical despite different names*


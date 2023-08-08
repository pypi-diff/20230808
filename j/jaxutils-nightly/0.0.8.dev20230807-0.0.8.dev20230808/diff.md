# Comparing `tmp/jaxutils-nightly-0.0.8.dev20230807.tar.gz` & `tmp/jaxutils-nightly-0.0.8.dev20230808.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/jaxutils-nightly-0.0.8.dev20230807.tar", last modified: Mon Aug  7 00:06:35 2023, max compression
+gzip compressed data, was "dist/jaxutils-nightly-0.0.8.dev20230808.tar", last modified: Tue Aug  8 00:06:33 2023, max compression
```

## Comparing `jaxutils-nightly-0.0.8.dev20230807.tar` & `jaxutils-nightly-0.0.8.dev20230808.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-08-07 00:06:35.052914 jaxutils-nightly-0.0.8.dev20230807/
--rw-r--r--   0 circleci  (3434) circleci  (3434)     4582 2023-08-07 00:06:35.052914 jaxutils-nightly-0.0.8.dev20230807/PKG-INFO
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3004 2023-08-07 00:06:29.000000 jaxutils-nightly-0.0.8.dev20230807/README.md
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-08-07 00:06:35.052914 jaxutils-nightly-0.0.8.dev20230807/jaxutils/
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1701 2023-08-07 00:06:29.000000 jaxutils-nightly-0.0.8.dev20230807/jaxutils/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      509 2023-08-07 00:06:35.052914 jaxutils-nightly-0.0.8.dev20230807/jaxutils/_version.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     4944 2023-08-07 00:06:29.000000 jaxutils-nightly-0.0.8.dev20230807/jaxutils/config.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3831 2023-08-07 00:06:29.000000 jaxutils-nightly-0.0.8.dev20230807/jaxutils/data.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3536 2023-08-07 00:06:29.000000 jaxutils-nightly-0.0.8.dev20230807/jaxutils/dict.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    13713 2023-08-07 00:06:29.000000 jaxutils-nightly-0.0.8.dev20230807/jaxutils/parameters.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2802 2023-08-07 00:06:29.000000 jaxutils-nightly-0.0.8.dev20230807/jaxutils/pytree.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-08-07 00:06:35.052914 jaxutils-nightly-0.0.8.dev20230807/jaxutils_nightly.egg-info/
--rw-r--r--   0 circleci  (3434) circleci  (3434)     4582 2023-08-07 00:06:35.000000 jaxutils-nightly-0.0.8.dev20230807/jaxutils_nightly.egg-info/PKG-INFO
--rw-r--r--   0 circleci  (3434) circleci  (3434)      378 2023-08-07 00:06:35.000000 jaxutils-nightly-0.0.8.dev20230807/jaxutils_nightly.egg-info/SOURCES.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)        1 2023-08-07 00:06:35.000000 jaxutils-nightly-0.0.8.dev20230807/jaxutils_nightly.egg-info/dependency_links.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)      141 2023-08-07 00:06:35.000000 jaxutils-nightly-0.0.8.dev20230807/jaxutils_nightly.egg-info/requires.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)        9 2023-08-07 00:06:35.000000 jaxutils-nightly-0.0.8.dev20230807/jaxutils_nightly.egg-info/top_level.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)      233 2023-08-07 00:06:35.052914 jaxutils-nightly-0.0.8.dev20230807/setup.cfg
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2389 2023-08-07 00:06:29.000000 jaxutils-nightly-0.0.8.dev20230807/setup.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    83607 2023-08-07 00:06:29.000000 jaxutils-nightly-0.0.8.dev20230807/versioneer.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-08-08 00:06:33.073049 jaxutils-nightly-0.0.8.dev20230808/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     4582 2023-08-08 00:06:33.073049 jaxutils-nightly-0.0.8.dev20230808/PKG-INFO
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3004 2023-08-08 00:06:26.000000 jaxutils-nightly-0.0.8.dev20230808/README.md
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-08-08 00:06:33.073049 jaxutils-nightly-0.0.8.dev20230808/jaxutils/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1701 2023-08-08 00:06:26.000000 jaxutils-nightly-0.0.8.dev20230808/jaxutils/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      509 2023-08-08 00:06:33.073049 jaxutils-nightly-0.0.8.dev20230808/jaxutils/_version.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     4944 2023-08-08 00:06:26.000000 jaxutils-nightly-0.0.8.dev20230808/jaxutils/config.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3831 2023-08-08 00:06:26.000000 jaxutils-nightly-0.0.8.dev20230808/jaxutils/data.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3536 2023-08-08 00:06:26.000000 jaxutils-nightly-0.0.8.dev20230808/jaxutils/dict.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    13713 2023-08-08 00:06:26.000000 jaxutils-nightly-0.0.8.dev20230808/jaxutils/parameters.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2802 2023-08-08 00:06:26.000000 jaxutils-nightly-0.0.8.dev20230808/jaxutils/pytree.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-08-08 00:06:33.073049 jaxutils-nightly-0.0.8.dev20230808/jaxutils_nightly.egg-info/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     4582 2023-08-08 00:06:33.000000 jaxutils-nightly-0.0.8.dev20230808/jaxutils_nightly.egg-info/PKG-INFO
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      378 2023-08-08 00:06:33.000000 jaxutils-nightly-0.0.8.dev20230808/jaxutils_nightly.egg-info/SOURCES.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        1 2023-08-08 00:06:33.000000 jaxutils-nightly-0.0.8.dev20230808/jaxutils_nightly.egg-info/dependency_links.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      141 2023-08-08 00:06:33.000000 jaxutils-nightly-0.0.8.dev20230808/jaxutils_nightly.egg-info/requires.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        9 2023-08-08 00:06:33.000000 jaxutils-nightly-0.0.8.dev20230808/jaxutils_nightly.egg-info/top_level.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      233 2023-08-08 00:06:33.073049 jaxutils-nightly-0.0.8.dev20230808/setup.cfg
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2389 2023-08-08 00:06:26.000000 jaxutils-nightly-0.0.8.dev20230808/setup.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    83607 2023-08-08 00:06:26.000000 jaxutils-nightly-0.0.8.dev20230808/versioneer.py
```

### Comparing `jaxutils-nightly-0.0.8.dev20230807/PKG-INFO` & `jaxutils-nightly-0.0.8.dev20230808/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jaxutils-nightly
-Version: 0.0.8.dev20230807
+Version: 0.0.8.dev20230808
 Summary: Utility functions for JaxGaussianProcesses
 Home-page: UNKNOWN
 Author: Daniel Dodd and Thomas Pinder
 Author-email: tompinder@live.co.uk
 License: LICENSE
 Project-URL: Documentation, https://JaxUitls.readthedocs.io/en/latest/
 Project-URL: Source, https://github.com/JaxGaussianProcesses/JaxUitls
```

### Comparing `jaxutils-nightly-0.0.8.dev20230807/README.md` & `jaxutils-nightly-0.0.8.dev20230808/README.md`

 * *Files identical despite different names*

### Comparing `jaxutils-nightly-0.0.8.dev20230807/jaxutils/__init__.py` & `jaxutils-nightly-0.0.8.dev20230808/jaxutils/__init__.py`

 * *Files identical despite different names*

### Comparing `jaxutils-nightly-0.0.8.dev20230807/jaxutils/config.py` & `jaxutils-nightly-0.0.8.dev20230808/jaxutils/config.py`

 * *Files identical despite different names*

### Comparing `jaxutils-nightly-0.0.8.dev20230807/jaxutils/data.py` & `jaxutils-nightly-0.0.8.dev20230808/jaxutils/data.py`

 * *Files identical despite different names*

### Comparing `jaxutils-nightly-0.0.8.dev20230807/jaxutils/dict.py` & `jaxutils-nightly-0.0.8.dev20230808/jaxutils/dict.py`

 * *Files identical despite different names*

### Comparing `jaxutils-nightly-0.0.8.dev20230807/jaxutils/parameters.py` & `jaxutils-nightly-0.0.8.dev20230808/jaxutils/parameters.py`

 * *Files identical despite different names*

### Comparing `jaxutils-nightly-0.0.8.dev20230807/jaxutils/pytree.py` & `jaxutils-nightly-0.0.8.dev20230808/jaxutils/pytree.py`

 * *Files identical despite different names*

### Comparing `jaxutils-nightly-0.0.8.dev20230807/jaxutils_nightly.egg-info/PKG-INFO` & `jaxutils-nightly-0.0.8.dev20230808/jaxutils_nightly.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jaxutils-nightly
-Version: 0.0.8.dev20230807
+Version: 0.0.8.dev20230808
 Summary: Utility functions for JaxGaussianProcesses
 Home-page: UNKNOWN
 Author: Daniel Dodd and Thomas Pinder
 Author-email: tompinder@live.co.uk
 License: LICENSE
 Project-URL: Documentation, https://JaxUitls.readthedocs.io/en/latest/
 Project-URL: Source, https://github.com/JaxGaussianProcesses/JaxUitls
```

### Comparing `jaxutils-nightly-0.0.8.dev20230807/setup.py` & `jaxutils-nightly-0.0.8.dev20230808/setup.py`

 * *Files identical despite different names*

### Comparing `jaxutils-nightly-0.0.8.dev20230807/versioneer.py` & `jaxutils-nightly-0.0.8.dev20230808/versioneer.py`

 * *Files identical despite different names*


# Comparing `tmp/firex-bundle-ci-1.4.1.tar.gz` & `tmp/firex-bundle-ci-1.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "firex-bundle-ci-1.4.1.tar", last modified: Tue Aug  8 16:26:18 2023, max compression
+gzip compressed data, was "firex-bundle-ci-1.4.2.tar", last modified: Tue Aug  8 16:54:19 2023, max compression
```

## Comparing `firex-bundle-ci-1.4.1.tar` & `firex-bundle-ci-1.4.2.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 firex      (101) nogroup  (65533)        0 2023-08-08 16:26:18.280448 firex-bundle-ci-1.4.1/
--rw-rw-rw-   0 firex      (101) nogroup  (65533)     1505 2023-08-08 16:26:07.000000 firex-bundle-ci-1.4.1/LICENSE
--rw-rw-rw-   0 firex      (101) nogroup  (65533)       80 2023-08-08 16:26:07.000000 firex-bundle-ci-1.4.1/MANIFEST.in
--rw-r--r--   0 firex      (101) nogroup  (65533)      277 2023-08-08 16:26:18.280448 firex-bundle-ci-1.4.1/PKG-INFO
-drwxr-xr-x   0 firex      (101) nogroup  (65533)        0 2023-08-08 16:26:18.280448 firex-bundle-ci-1.4.1/firex_bundle_ci/
--rw-rw-rw-   0 firex      (101) nogroup  (65533)       93 2023-08-08 16:26:07.000000 firex-bundle-ci-1.4.1/firex_bundle_ci/__init__.py
--rw-r--r--   0 firex      (101) nogroup  (65533)      497 2023-08-08 16:26:18.280448 firex-bundle-ci-1.4.1/firex_bundle_ci/_version.py
--rw-rw-rw-   0 firex      (101) nogroup  (65533)     9791 2023-08-08 16:26:07.000000 firex-bundle-ci-1.4.1/firex_bundle_ci/tasks.py
--rw-rw-rw-   0 firex      (101) nogroup  (65533)    70144 2023-08-08 16:26:07.000000 firex-bundle-ci-1.4.1/firex_bundle_ci/versioneer.py
-drwxr-xr-x   0 firex      (101) nogroup  (65533)        0 2023-08-08 16:26:18.279532 firex-bundle-ci-1.4.1/firex_bundle_ci.egg-info/
--rw-r--r--   0 firex      (101) nogroup  (65533)      277 2023-08-08 16:26:18.000000 firex-bundle-ci-1.4.1/firex_bundle_ci.egg-info/PKG-INFO
--rw-r--r--   0 firex      (101) nogroup  (65533)      433 2023-08-08 16:26:18.000000 firex-bundle-ci-1.4.1/firex_bundle_ci.egg-info/SOURCES.txt
--rw-r--r--   0 firex      (101) nogroup  (65533)        1 2023-08-08 16:26:18.000000 firex-bundle-ci-1.4.1/firex_bundle_ci.egg-info/dependency_links.txt
--rw-r--r--   0 firex      (101) nogroup  (65533)       51 2023-08-08 16:26:18.000000 firex-bundle-ci-1.4.1/firex_bundle_ci.egg-info/entry_points.txt
--rw-r--r--   0 firex      (101) nogroup  (65533)       73 2023-08-08 16:26:18.000000 firex-bundle-ci-1.4.1/firex_bundle_ci.egg-info/requires.txt
--rw-r--r--   0 firex      (101) nogroup  (65533)       16 2023-08-08 16:26:18.000000 firex-bundle-ci-1.4.1/firex_bundle_ci.egg-info/top_level.txt
--rw-r--r--   0 firex      (101) nogroup  (65533)        1 2023-08-08 16:26:18.000000 firex-bundle-ci-1.4.1/firex_bundle_ci.egg-info/zip-safe
--rw-rw-rw-   0 firex      (101) nogroup  (65533)      289 2023-08-08 16:26:18.280448 firex-bundle-ci-1.4.1/setup.cfg
--rw-rw-rw-   0 firex      (101) nogroup  (65533)      690 2023-08-08 16:26:07.000000 firex-bundle-ci-1.4.1/setup.py
--rw-rw-rw-   0 firex      (101) nogroup  (65533)    70144 2023-08-08 16:26:07.000000 firex-bundle-ci-1.4.1/versioneer.py
+drwxr-xr-x   0 firex      (101) nogroup  (65533)        0 2023-08-08 16:54:19.757373 firex-bundle-ci-1.4.2/
+-rw-rw-rw-   0 firex      (101) nogroup  (65533)     1505 2023-08-08 16:54:05.000000 firex-bundle-ci-1.4.2/LICENSE
+-rw-rw-rw-   0 firex      (101) nogroup  (65533)       80 2023-08-08 16:54:05.000000 firex-bundle-ci-1.4.2/MANIFEST.in
+-rw-r--r--   0 firex      (101) nogroup  (65533)      249 2023-08-08 16:54:19.757373 firex-bundle-ci-1.4.2/PKG-INFO
+drwxr-xr-x   0 firex      (101) nogroup  (65533)        0 2023-08-08 16:54:19.758374 firex-bundle-ci-1.4.2/firex_bundle_ci/
+-rw-rw-rw-   0 firex      (101) nogroup  (65533)       93 2023-08-08 16:54:05.000000 firex-bundle-ci-1.4.2/firex_bundle_ci/__init__.py
+-rw-r--r--   0 firex      (101) nogroup  (65533)      497 2023-08-08 16:54:19.758374 firex-bundle-ci-1.4.2/firex_bundle_ci/_version.py
+-rw-rw-rw-   0 firex      (101) nogroup  (65533)     9796 2023-08-08 16:54:05.000000 firex-bundle-ci-1.4.2/firex_bundle_ci/tasks.py
+-rw-rw-rw-   0 firex      (101) nogroup  (65533)    70144 2023-08-08 16:54:05.000000 firex-bundle-ci-1.4.2/firex_bundle_ci/versioneer.py
+drwxr-xr-x   0 firex      (101) nogroup  (65533)        0 2023-08-08 16:54:19.757373 firex-bundle-ci-1.4.2/firex_bundle_ci.egg-info/
+-rw-r--r--   0 firex      (101) nogroup  (65533)      249 2023-08-08 16:54:19.000000 firex-bundle-ci-1.4.2/firex_bundle_ci.egg-info/PKG-INFO
+-rw-r--r--   0 firex      (101) nogroup  (65533)      433 2023-08-08 16:54:19.000000 firex-bundle-ci-1.4.2/firex_bundle_ci.egg-info/SOURCES.txt
+-rw-r--r--   0 firex      (101) nogroup  (65533)        1 2023-08-08 16:54:19.000000 firex-bundle-ci-1.4.2/firex_bundle_ci.egg-info/dependency_links.txt
+-rw-r--r--   0 firex      (101) nogroup  (65533)       50 2023-08-08 16:54:19.000000 firex-bundle-ci-1.4.2/firex_bundle_ci.egg-info/entry_points.txt
+-rw-r--r--   0 firex      (101) nogroup  (65533)       73 2023-08-08 16:54:19.000000 firex-bundle-ci-1.4.2/firex_bundle_ci.egg-info/requires.txt
+-rw-r--r--   0 firex      (101) nogroup  (65533)       16 2023-08-08 16:54:19.000000 firex-bundle-ci-1.4.2/firex_bundle_ci.egg-info/top_level.txt
+-rw-r--r--   0 firex      (101) nogroup  (65533)        1 2023-08-08 16:54:19.000000 firex-bundle-ci-1.4.2/firex_bundle_ci.egg-info/zip-safe
+-rw-rw-rw-   0 firex      (101) nogroup  (65533)      289 2023-08-08 16:54:19.758374 firex-bundle-ci-1.4.2/setup.cfg
+-rw-rw-rw-   0 firex      (101) nogroup  (65533)      690 2023-08-08 16:54:05.000000 firex-bundle-ci-1.4.2/setup.py
+-rw-rw-rw-   0 firex      (101) nogroup  (65533)    70144 2023-08-08 16:54:05.000000 firex-bundle-ci-1.4.2/versioneer.py
```

### Comparing `firex-bundle-ci-1.4.1/LICENSE` & `firex-bundle-ci-1.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `firex-bundle-ci-1.4.1/firex_bundle_ci/tasks.py` & `firex-bundle-ci-1.4.2/firex_bundle_ci/tasks.py`

 * *Files 0% similar despite different names*

```diff
@@ -111,15 +111,15 @@
                                                     flow_tests_configs=test_config_name,
                                                     flow_tests_file=test_config_filepath,
                                                     test_output_dir=test_config_output_dir,
                                                     xunit_file_name=xunit_file_name,
                                                     public_runs=public_runs,
                                                     coverage=coverage))
     if parallel_tasks:
-        promises = self.enqueue_in_parallel(parallel_tasks, max_parallel_chains=max_parallel_tests)
+        promises = self.enqueue_in_parallel(parallel_tasks, max_parallel_chains=int(max_parallel_tests))
         if not all([promise.successful() for promise in promises]):
             raise AssertionError('Some tests failed')
     else:
         raise AssertionError('No Integrations tests to run')
 
     return integration_tests_xunits, integration_tests_coverage_dats
```

### Comparing `firex-bundle-ci-1.4.1/firex_bundle_ci/versioneer.py` & `firex-bundle-ci-1.4.2/firex_bundle_ci/versioneer.py`

 * *Files identical despite different names*

### Comparing `firex-bundle-ci-1.4.1/setup.py` & `firex-bundle-ci-1.4.2/setup.py`

 * *Files identical despite different names*

### Comparing `firex-bundle-ci-1.4.1/versioneer.py` & `firex-bundle-ci-1.4.2/versioneer.py`

 * *Files identical despite different names*


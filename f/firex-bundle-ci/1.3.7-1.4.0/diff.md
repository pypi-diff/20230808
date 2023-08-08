# Comparing `tmp/firex-bundle-ci-1.3.7.tar.gz` & `tmp/firex-bundle-ci-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/firex-bundle-ci-1.3.7.tar", last modified: Wed Mar 10 20:26:02 2021, max compression
+gzip compressed data, was "firex-bundle-ci-1.4.0.tar", last modified: Tue Aug  8 15:36:03 2023, max compression
```

## Comparing `firex-bundle-ci-1.3.7.tar` & `firex-bundle-ci-1.4.0.tar`

### file list

```diff
@@ -1,20 +1,19 @@
-drwxr-xr-x   0 firex      (101) nogroup  (65533)        0 2021-03-10 20:26:02.000000 firex-bundle-ci-1.3.7/
--rw-rw-rw-   0 firex      (101) nogroup  (65533)     1505 2021-03-10 20:25:48.000000 firex-bundle-ci-1.3.7/LICENSE
--rw-rw-rw-   0 firex      (101) nogroup  (65533)       80 2021-03-10 20:25:48.000000 firex-bundle-ci-1.3.7/MANIFEST.in
--rw-r--r--   0 firex      (101) nogroup  (65533)      266 2021-03-10 20:26:02.000000 firex-bundle-ci-1.3.7/PKG-INFO
-drwxr-xr-x   0 firex      (101) nogroup  (65533)        0 2021-03-10 20:26:02.000000 firex-bundle-ci-1.3.7/firex_bundle_ci/
--rw-rw-rw-   0 firex      (101) nogroup  (65533)       93 2021-03-10 20:25:48.000000 firex-bundle-ci-1.3.7/firex_bundle_ci/__init__.py
--rw-r--r--   0 firex      (101) nogroup  (65533)      497 2021-03-10 20:26:02.000000 firex-bundle-ci-1.3.7/firex_bundle_ci/_version.py
--rw-rw-rw-   0 firex      (101) nogroup  (65533)     9728 2021-03-10 20:25:48.000000 firex-bundle-ci-1.3.7/firex_bundle_ci/tasks.py
--rw-rw-rw-   0 firex      (101) nogroup  (65533)    70144 2021-03-10 20:25:48.000000 firex-bundle-ci-1.3.7/firex_bundle_ci/versioneer.py
-drwxr-xr-x   0 firex      (101) nogroup  (65533)        0 2021-03-10 20:26:02.000000 firex-bundle-ci-1.3.7/firex_bundle_ci.egg-info/
--rw-r--r--   0 firex      (101) nogroup  (65533)      266 2021-03-10 20:26:01.000000 firex-bundle-ci-1.3.7/firex_bundle_ci.egg-info/PKG-INFO
--rw-r--r--   0 firex      (101) nogroup  (65533)      433 2021-03-10 20:26:01.000000 firex-bundle-ci-1.3.7/firex_bundle_ci.egg-info/SOURCES.txt
--rw-r--r--   0 firex      (101) nogroup  (65533)        1 2021-03-10 20:26:01.000000 firex-bundle-ci-1.3.7/firex_bundle_ci.egg-info/dependency_links.txt
--rw-r--r--   0 firex      (101) nogroup  (65533)       51 2021-03-10 20:26:01.000000 firex-bundle-ci-1.3.7/firex_bundle_ci.egg-info/entry_points.txt
--rw-r--r--   0 firex      (101) nogroup  (65533)       73 2021-03-10 20:26:01.000000 firex-bundle-ci-1.3.7/firex_bundle_ci.egg-info/requires.txt
--rw-r--r--   0 firex      (101) nogroup  (65533)       16 2021-03-10 20:26:01.000000 firex-bundle-ci-1.3.7/firex_bundle_ci.egg-info/top_level.txt
--rw-r--r--   0 firex      (101) nogroup  (65533)        1 2021-03-10 20:26:01.000000 firex-bundle-ci-1.3.7/firex_bundle_ci.egg-info/zip-safe
--rw-rw-rw-   0 firex      (101) nogroup  (65533)      288 2021-03-10 20:26:02.000000 firex-bundle-ci-1.3.7/setup.cfg
--rw-rw-rw-   0 firex      (101) nogroup  (65533)      690 2021-03-10 20:25:48.000000 firex-bundle-ci-1.3.7/setup.py
--rw-rw-rw-   0 firex      (101) nogroup  (65533)    70144 2021-03-10 20:25:48.000000 firex-bundle-ci-1.3.7/versioneer.py
+drwxr-xr-x   0 firex      (101) nogroup  (65533)        0 2023-08-08 15:36:03.015538 firex-bundle-ci-1.4.0/
+-rw-rw-rw-   0 firex      (101) nogroup  (65533)     1505 2023-08-08 15:35:41.000000 firex-bundle-ci-1.4.0/LICENSE
+-rw-rw-rw-   0 firex      (101) nogroup  (65533)       80 2023-08-08 15:35:41.000000 firex-bundle-ci-1.4.0/MANIFEST.in
+-rw-r--r--   0 firex      (101) nogroup  (65533)      277 2023-08-08 15:36:03.015538 firex-bundle-ci-1.4.0/PKG-INFO
+drwxr-xr-x   0 firex      (101) nogroup  (65533)        0 2023-08-08 15:36:03.016538 firex-bundle-ci-1.4.0/firex_bundle_ci/
+-rw-rw-rw-   0 firex      (101) nogroup  (65533)       93 2023-08-08 15:35:41.000000 firex-bundle-ci-1.4.0/firex_bundle_ci/__init__.py
+-rw-r--r--   0 firex      (101) nogroup  (65533)      497 2023-08-08 15:36:03.016538 firex-bundle-ci-1.4.0/firex_bundle_ci/_version.py
+-rw-rw-rw-   0 firex      (101) nogroup  (65533)     9791 2023-08-08 15:35:41.000000 firex-bundle-ci-1.4.0/firex_bundle_ci/tasks.py
+-rw-rw-rw-   0 firex      (101) nogroup  (65533)    70144 2023-08-08 15:35:41.000000 firex-bundle-ci-1.4.0/firex_bundle_ci/versioneer.py
+drwxr-xr-x   0 firex      (101) nogroup  (65533)        0 2023-08-08 15:36:03.015538 firex-bundle-ci-1.4.0/firex_bundle_ci.egg-info/
+-rw-r--r--   0 firex      (101) nogroup  (65533)      277 2023-08-08 15:36:02.000000 firex-bundle-ci-1.4.0/firex_bundle_ci.egg-info/PKG-INFO
+-rw-r--r--   0 firex      (101) nogroup  (65533)      391 2023-08-08 15:36:02.000000 firex-bundle-ci-1.4.0/firex_bundle_ci.egg-info/SOURCES.txt
+-rw-r--r--   0 firex      (101) nogroup  (65533)        1 2023-08-08 15:36:02.000000 firex-bundle-ci-1.4.0/firex_bundle_ci.egg-info/dependency_links.txt
+-rw-r--r--   0 firex      (101) nogroup  (65533)       61 2023-08-08 15:36:02.000000 firex-bundle-ci-1.4.0/firex_bundle_ci.egg-info/requires.txt
+-rw-r--r--   0 firex      (101) nogroup  (65533)       16 2023-08-08 15:36:02.000000 firex-bundle-ci-1.4.0/firex_bundle_ci.egg-info/top_level.txt
+-rw-r--r--   0 firex      (101) nogroup  (65533)        1 2023-08-08 15:36:02.000000 firex-bundle-ci-1.4.0/firex_bundle_ci.egg-info/zip-safe
+-rw-rw-rw-   0 firex      (101) nogroup  (65533)      289 2023-08-08 15:36:03.015538 firex-bundle-ci-1.4.0/setup.cfg
+-rw-rw-rw-   0 firex      (101) nogroup  (65533)      590 2023-08-08 15:35:41.000000 firex-bundle-ci-1.4.0/setup.py
+-rw-rw-rw-   0 firex      (101) nogroup  (65533)    70144 2023-08-08 15:35:41.000000 firex-bundle-ci-1.4.0/versioneer.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `firex-bundle-ci-1.3.7/LICENSE` & `firex-bundle-ci-1.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `firex-bundle-ci-1.3.7/firex_bundle_ci/tasks.py` & `firex-bundle-ci-1.4.0/firex_bundle_ci/tasks.py`

 * *Files 2% similar despite different names*

```diff
@@ -86,15 +86,15 @@
                        GenerateHtmlCoverage.s(coverage_dat_file='@aggregated_coverage_dat'))
     self.wait_for_children()
 
 
 @app.task(bind=True, returns=('integration_tests_xunits', 'integration_tests_coverage_dats'))
 def RunAllIntegrationTests(self, uid,
                            integration_tests_dir='tests/integration_tests/',
-                           integration_tests_logs=None, coverage=True, public_runs=False):
+                           integration_tests_logs=None, coverage=True, public_runs=False, max_parallel_tests=15):
     if not integration_tests_logs and uid:
         test_output_dir = os.path.join(uid.logs_dir, 'integration_tests_logs')
     else:
         test_output_dir = integration_tests_logs
 
     parallel_tasks = []
     integration_tests_xunits = []
@@ -111,15 +111,15 @@
                                                     flow_tests_configs=test_config_name,
                                                     flow_tests_file=test_config_filepath,
                                                     test_output_dir=test_config_output_dir,
                                                     xunit_file_name=xunit_file_name,
                                                     public_runs=public_runs,
                                                     coverage=coverage))
     if parallel_tasks:
-        promises = self.enqueue_in_parallel(parallel_tasks)
+        promises = self.enqueue_in_parallel(parallel_tasks, max_parallel_chains=max_parallel_tests)
         if not all([promise.successful() for promise in promises]):
             raise AssertionError('Some tests failed')
     else:
         raise AssertionError('No Integrations tests to run')
 
     return integration_tests_xunits, integration_tests_coverage_dats
```

### Comparing `firex-bundle-ci-1.3.7/firex_bundle_ci/versioneer.py` & `firex-bundle-ci-1.4.0/firex_bundle_ci/versioneer.py`

 * *Files identical despite different names*

### Comparing `firex-bundle-ci-1.3.7/setup.py` & `firex-bundle-ci-1.4.0/setup.py`

 * *Files 25% similar despite different names*

```diff
@@ -10,14 +10,12 @@
       author_email='firex-dev@gmail.com',
       license='BSD-3-Clause',
       packages=['firex_bundle_ci'],
       zip_safe=True,
       install_requires=[
           "firexapp",
           "firex-keeper",
-          "firex-flame",
           "lxml",
           "xunitmerge",
           "unittest-xml-reporting"
       ],
-      entry_points={'firex.bundles': 'firex-bundle-ci = firex_bundle_ci'},
       )
```

### Comparing `firex-bundle-ci-1.3.7/versioneer.py` & `firex-bundle-ci-1.4.0/versioneer.py`

 * *Files identical despite different names*


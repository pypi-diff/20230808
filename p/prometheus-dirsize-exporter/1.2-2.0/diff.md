# Comparing `tmp/prometheus-dirsize-exporter-1.2.tar.gz` & `tmp/prometheus-dirsize-exporter-2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prometheus-dirsize-exporter-1.2.tar", last modified: Tue Jun  6 16:34:04 2023, max compression
+gzip compressed data, was "prometheus-dirsize-exporter-2.0.tar", last modified: Mon Aug  7 23:33:39 2023, max compression
```

## Comparing `prometheus-dirsize-exporter-1.2.tar` & `prometheus-dirsize-exporter-2.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 16:34:04.303625 prometheus-dirsize-exporter-1.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1497 2023-06-06 16:33:51.000000 prometheus-dirsize-exporter-1.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1888 2023-06-06 16:34:04.303625 prometheus-dirsize-exporter-1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1689 2023-06-06 16:33:51.000000 prometheus-dirsize-exporter-1.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 16:34:04.299625 prometheus-dirsize-exporter-1.2/prometheus_dirsize_exporter/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 16:33:51.000000 prometheus-dirsize-exporter-1.2/prometheus_dirsize_exporter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6056 2023-06-06 16:33:51.000000 prometheus-dirsize-exporter-1.2/prometheus_dirsize_exporter/exporter.py
--rw-r--r--   0 runner    (1001) docker     (123)      912 2023-06-06 16:33:51.000000 prometheus-dirsize-exporter-1.2/prometheus_dirsize_exporter/metrics.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 16:34:04.303625 prometheus-dirsize-exporter-1.2/prometheus_dirsize_exporter.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1888 2023-06-06 16:34:04.000000 prometheus-dirsize-exporter-1.2/prometheus_dirsize_exporter.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      453 2023-06-06 16:34:04.000000 prometheus-dirsize-exporter-1.2/prometheus_dirsize_exporter.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-06 16:34:04.000000 prometheus-dirsize-exporter-1.2/prometheus_dirsize_exporter.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-06-06 16:34:04.000000 prometheus-dirsize-exporter-1.2/prometheus_dirsize_exporter.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-06 16:34:04.000000 prometheus-dirsize-exporter-1.2/prometheus_dirsize_exporter.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-06 16:34:04.000000 prometheus-dirsize-exporter-1.2/prometheus_dirsize_exporter.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-06 16:34:04.303625 prometheus-dirsize-exporter-1.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      579 2023-06-06 16:33:51.000000 prometheus-dirsize-exporter-1.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 23:33:39.757021 prometheus-dirsize-exporter-2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1497 2023-08-07 23:33:29.000000 prometheus-dirsize-exporter-2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2638 2023-08-07 23:33:39.757021 prometheus-dirsize-exporter-2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2439 2023-08-07 23:33:29.000000 prometheus-dirsize-exporter-2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 23:33:39.757021 prometheus-dirsize-exporter-2.0/prometheus_dirsize_exporter/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 23:33:29.000000 prometheus-dirsize-exporter-2.0/prometheus_dirsize_exporter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6569 2023-08-07 23:33:29.000000 prometheus-dirsize-exporter-2.0/prometheus_dirsize_exporter/exporter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      912 2023-08-07 23:33:29.000000 prometheus-dirsize-exporter-2.0/prometheus_dirsize_exporter/metrics.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 23:33:39.757021 prometheus-dirsize-exporter-2.0/prometheus_dirsize_exporter.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2638 2023-08-07 23:33:39.000000 prometheus-dirsize-exporter-2.0/prometheus_dirsize_exporter.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      453 2023-08-07 23:33:39.000000 prometheus-dirsize-exporter-2.0/prometheus_dirsize_exporter.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-07 23:33:39.000000 prometheus-dirsize-exporter-2.0/prometheus_dirsize_exporter.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-08-07 23:33:39.000000 prometheus-dirsize-exporter-2.0/prometheus_dirsize_exporter.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-08-07 23:33:39.000000 prometheus-dirsize-exporter-2.0/prometheus_dirsize_exporter.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-08-07 23:33:39.000000 prometheus-dirsize-exporter-2.0/prometheus_dirsize_exporter.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-07 23:33:39.757021 prometheus-dirsize-exporter-2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      579 2023-08-07 23:33:29.000000 prometheus-dirsize-exporter-2.0/setup.py
```

### Comparing `prometheus-dirsize-exporter-1.2/LICENSE` & `prometheus-dirsize-exporter-2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `prometheus-dirsize-exporter-1.2/PKG-INFO` & `prometheus-dirsize-exporter-2.0/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 Metadata-Version: 2.1
 Name: prometheus-dirsize-exporter
-Version: 1.2
+Version: 2.0
 Author: yuvipanda
 Author-email: yuvipanda@gmail.com
 License: 3-BSD
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # prometheus-dirsize-exporter
 
+[![PyPI version](https://badge.fury.io/py/prometheus-dirsize-exporter.svg)](https://badge.fury.io/py/prometheus-dirsize-exporter)
+
 Export directory size metrics efficiently.
 
 ## Why?
 
 When providing multi-user interactive computing services (with a HPC cluster
 or with JupyterHub), it's very helpful to know the home directory sizes of
 each user over time. However, as NFS is often used, running `du` constantly
@@ -20,23 +22,14 @@
 plain inefficient.
 
 This project provides a way to keep track of directory sizes with a *budgeted*
 amount of IOPS. You can ask it to take however much time it needs but not
 use more than 100 IOPS, and it will do that. We do not necessarily need very
 up to date directory size metrics, so this is ok.
 
-## Limitations
-
-- As directory contents might change in the course of a single run as we wait
-  for budgets to become available, information about a directory may not be
-  exactly correct immediately.
-- Because we do not spread the IOPS through time, the IO usage is 'spiky' -
-  all IOPS get done at the beginning of a second, and then it goes silent.
-  If you have a big IOPS budget, this can cause performance degradation.
-
 ## Installation
 
 Install the package from PyPI:
 
 ```bash
 pip install prometheus-dirsize-exporter
 ```
@@ -55,8 +48,30 @@
 ```bash
 dirsize-exporter /home 200 60
 ```
 
 You can check out the metrics by hitting `http://localhost:8000`. The port can
 be controlled via a `--port` argument.
 
+## Metrics recorded
 
+The following metrics are recorded for all top level subidrectories of the
+parent directory:
+
+- Total Size (in bytes)
+- Last Modified (including all the descendents)
+- Total Number of Entries (Files, directories & symlinks)
+- Processing Time required to gather this information
+  This is only reported if `--enable-detailed-processing-time-metric` flag is
+  passed, to prevent possible explosion of stored size of prometheus metrics
+  when collected. This information is also not particularly useful outside
+  of debugging this exporter, and as it varies each run, compresses poorly.
+- Last updated
+
+## Limitations
+
+- As directory contents might change in the course of a single run as we wait
+  for budgets to become available, information about a directory may not be
+  exactly correct immediately.
+- Because we do not spread the IOPS through time, the IO usage is 'spiky' -
+  all IOPS get done at the beginning of a second, and then it goes silent.
+  If you have a big IOPS budget, this can cause performance degradation.
```

### Comparing `prometheus-dirsize-exporter-1.2/README.md` & `prometheus-dirsize-exporter-2.0/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 # prometheus-dirsize-exporter
 
+[![PyPI version](https://badge.fury.io/py/prometheus-dirsize-exporter.svg)](https://badge.fury.io/py/prometheus-dirsize-exporter)
+
 Export directory size metrics efficiently.
 
 ## Why?
 
 When providing multi-user interactive computing services (with a HPC cluster
 or with JupyterHub), it's very helpful to know the home directory sizes of
 each user over time. However, as NFS is often used, running `du` constantly
@@ -11,23 +13,14 @@
 plain inefficient.
 
 This project provides a way to keep track of directory sizes with a *budgeted*
 amount of IOPS. You can ask it to take however much time it needs but not
 use more than 100 IOPS, and it will do that. We do not necessarily need very
 up to date directory size metrics, so this is ok.
 
-## Limitations
-
-- As directory contents might change in the course of a single run as we wait
-  for budgets to become available, information about a directory may not be
-  exactly correct immediately.
-- Because we do not spread the IOPS through time, the IO usage is 'spiky' -
-  all IOPS get done at the beginning of a second, and then it goes silent.
-  If you have a big IOPS budget, this can cause performance degradation.
-
 ## Installation
 
 Install the package from PyPI:
 
 ```bash
 pip install prometheus-dirsize-exporter
 ```
@@ -46,8 +39,30 @@
 ```bash
 dirsize-exporter /home 200 60
 ```
 
 You can check out the metrics by hitting `http://localhost:8000`. The port can
 be controlled via a `--port` argument.
 
+## Metrics recorded
 
+The following metrics are recorded for all top level subidrectories of the
+parent directory:
+
+- Total Size (in bytes)
+- Last Modified (including all the descendents)
+- Total Number of Entries (Files, directories & symlinks)
+- Processing Time required to gather this information
+  This is only reported if `--enable-detailed-processing-time-metric` flag is
+  passed, to prevent possible explosion of stored size of prometheus metrics
+  when collected. This information is also not particularly useful outside
+  of debugging this exporter, and as it varies each run, compresses poorly.
+- Last updated
+
+## Limitations
+
+- As directory contents might change in the course of a single run as we wait
+  for budgets to become available, information about a directory may not be
+  exactly correct immediately.
+- Because we do not spread the IOPS through time, the IO usage is 'spiky' -
+  all IOPS get done at the beginning of a second, and then it goes silent.
+  If you have a big IOPS budget, this can cause performance degradation.
```

### Comparing `prometheus-dirsize-exporter-1.2/prometheus_dirsize_exporter/exporter.py` & `prometheus-dirsize-exporter-2.0/prometheus_dirsize_exporter/exporter.py`

 * *Files 4% similar despite different names*

```diff
@@ -132,14 +132,23 @@
         "iops_budget", help="Number of IO operations allowed per second", type=int
     )
     argparser.add_argument(
         "wait_time_minutes",
         help="Number of minutes to wait before data collection runs",
         type=int,
     )
+    # Don't report amount of time it took to process each directory by
+    # default. This is highly variable, and probably causes prometheus to
+    # not compress metrics very well. Not particularly useful outside of
+    # debugging the exporter itself.
+    argparser.add_argument(
+        "--enable-detailed-processing-time-metric",
+        help="Report amount of time it took to process each directory",
+        action="store_true"
+    )
     argparser.add_argument(
         "--port", help="Port for the server to listen on", type=int, default=8000
     )
 
     args = argparser.parse_args()
 
     start_http_server(args.port)
@@ -147,17 +156,18 @@
         walker = BudgetedDirInfoWalker(args.iops_budget)
         for subdir_info in walker.get_subdirs_info(args.parent_dir):
             metrics.TOTAL_SIZE.labels(subdir_info.path).set(subdir_info.size)
             metrics.LATEST_MTIME.labels(subdir_info.path).set(subdir_info.latest_mtime)
             metrics.ENTRIES_COUNT.labels(subdir_info.path).set(
                 subdir_info.entries_count
             )
-            metrics.PROCESSING_TIME.labels(subdir_info.path).set(
-                subdir_info.processing_time
-            )
+            if args.enable_detailed_processing_time_metric:
+                metrics.PROCESSING_TIME.labels(subdir_info.path).set(
+                    subdir_info.processing_time
+                )
             metrics.LAST_UPDATED.labels(subdir_info.path).set(time.time())
             print(f"Updated values for {subdir_info.path}")
         time.sleep(args.wait_time_minutes * 60)
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `prometheus-dirsize-exporter-1.2/prometheus_dirsize_exporter/metrics.py` & `prometheus-dirsize-exporter-2.0/prometheus_dirsize_exporter/metrics.py`

 * *Files identical despite different names*

### Comparing `prometheus-dirsize-exporter-1.2/prometheus_dirsize_exporter.egg-info/PKG-INFO` & `prometheus-dirsize-exporter-2.0/prometheus_dirsize_exporter.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 Metadata-Version: 2.1
 Name: prometheus-dirsize-exporter
-Version: 1.2
+Version: 2.0
 Author: yuvipanda
 Author-email: yuvipanda@gmail.com
 License: 3-BSD
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # prometheus-dirsize-exporter
 
+[![PyPI version](https://badge.fury.io/py/prometheus-dirsize-exporter.svg)](https://badge.fury.io/py/prometheus-dirsize-exporter)
+
 Export directory size metrics efficiently.
 
 ## Why?
 
 When providing multi-user interactive computing services (with a HPC cluster
 or with JupyterHub), it's very helpful to know the home directory sizes of
 each user over time. However, as NFS is often used, running `du` constantly
@@ -20,23 +22,14 @@
 plain inefficient.
 
 This project provides a way to keep track of directory sizes with a *budgeted*
 amount of IOPS. You can ask it to take however much time it needs but not
 use more than 100 IOPS, and it will do that. We do not necessarily need very
 up to date directory size metrics, so this is ok.
 
-## Limitations
-
-- As directory contents might change in the course of a single run as we wait
-  for budgets to become available, information about a directory may not be
-  exactly correct immediately.
-- Because we do not spread the IOPS through time, the IO usage is 'spiky' -
-  all IOPS get done at the beginning of a second, and then it goes silent.
-  If you have a big IOPS budget, this can cause performance degradation.
-
 ## Installation
 
 Install the package from PyPI:
 
 ```bash
 pip install prometheus-dirsize-exporter
 ```
@@ -55,8 +48,30 @@
 ```bash
 dirsize-exporter /home 200 60
 ```
 
 You can check out the metrics by hitting `http://localhost:8000`. The port can
 be controlled via a `--port` argument.
 
+## Metrics recorded
 
+The following metrics are recorded for all top level subidrectories of the
+parent directory:
+
+- Total Size (in bytes)
+- Last Modified (including all the descendents)
+- Total Number of Entries (Files, directories & symlinks)
+- Processing Time required to gather this information
+  This is only reported if `--enable-detailed-processing-time-metric` flag is
+  passed, to prevent possible explosion of stored size of prometheus metrics
+  when collected. This information is also not particularly useful outside
+  of debugging this exporter, and as it varies each run, compresses poorly.
+- Last updated
+
+## Limitations
+
+- As directory contents might change in the course of a single run as we wait
+  for budgets to become available, information about a directory may not be
+  exactly correct immediately.
+- Because we do not spread the IOPS through time, the IO usage is 'spiky' -
+  all IOPS get done at the beginning of a second, and then it goes silent.
+  If you have a big IOPS budget, this can cause performance degradation.
```

### Comparing `prometheus-dirsize-exporter-1.2/setup.py` & `prometheus-dirsize-exporter-2.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md") as f:
     long_description = f.read()
 
 setup(
     name="prometheus-dirsize-exporter",
-    version="1.2",
+    version="2.0",
     packages=find_packages(),
     license="3-BSD",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="yuvipanda",
     author_email="yuvipanda@gmail.com",
     install_requires=[
```


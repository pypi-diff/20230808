# Comparing `tmp/ngcpp-0.0.3.tar.gz` & `tmp/ngcpp-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ngcpp-0.0.3.tar", max compression
+gzip compressed data, was "ngcpp-0.0.4.tar", max compression
```

## Comparing `ngcpp-0.0.3.tar` & `ngcpp-0.0.4.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0      574 2023-08-08 03:18:20.306765 ngcpp-0.0.3/README.md
--rw-r--r--   0        0        0     1331 2023-08-08 03:18:20.307765 ngcpp-0.0.3/ngcpp/cli/cluster_info.py
--rw-r--r--   0        0        0     6920 2023-08-08 03:18:20.307765 ngcpp-0.0.3/ngcpp/cli/job_info.py
--rw-r--r--   0        0        0     4656 2023-08-08 03:18:20.307765 ngcpp-0.0.3/ngcpp/cluster.py
--rw-r--r--   0        0        0     1154 2023-08-08 03:18:20.307765 ngcpp-0.0.3/ngcpp/cluster.yaml
--rw-r--r--   0        0        0      383 2023-08-08 03:18:20.307765 ngcpp-0.0.3/ngcpp/utils.py
--rw-r--r--   0        0        0      717 2023-08-08 03:18:24.076802 ngcpp-0.0.3/pyproject.toml
--rw-r--r--   0        0        0     1298 1970-01-01 00:00:00.000000 ngcpp-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0      590 2023-08-08 03:30:47.859995 ngcpp-0.0.4/README.md
+-rw-r--r--   0        0        0     1331 2023-08-08 03:30:47.859995 ngcpp-0.0.4/ngcpp/cli/cluster_info.py
+-rw-r--r--   0        0        0     6920 2023-08-08 03:30:47.859995 ngcpp-0.0.4/ngcpp/cli/job_info.py
+-rw-r--r--   0        0        0     4656 2023-08-08 03:30:47.859995 ngcpp-0.0.4/ngcpp/cluster.py
+-rw-r--r--   0        0        0     1154 2023-08-08 03:30:47.860995 ngcpp-0.0.4/ngcpp/cluster.yaml
+-rw-r--r--   0        0        0      383 2023-08-08 03:30:47.860995 ngcpp-0.0.4/ngcpp/utils.py
+-rw-r--r--   0        0        0      717 2023-08-08 03:30:51.474989 ngcpp-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0     1314 1970-01-01 00:00:00.000000 ngcpp-0.0.4/PKG-INFO
```

### Comparing `ngcpp-0.0.3/README.md` & `ngcpp-0.0.4/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -6,16 +6,16 @@
 ```
 
 # Feature
 
 ## cluster `ngc_cluster --help`
 
 * `ngc_cluster usage --help`: List user usage
-* `ngc_cluster hang --help`: List all hanging jobs
-* `ngc_cluster list --help`: List all jobs in one cluster
+* `ngc_cluster hang --help`: List your all hanging jobs
+* `ngc_cluster list --help`: List your jobs in one cluster
 * `ngc_cluster alias --help`: List all available cluster aliases
 
 ## job `ngc_job --help`
 
-* `ngc_job kill --help`: kill jobs interactively
-* `ngc_job result --help`: download results for jobs interactively
+* `ngc_job kill --help`: kill your jobs interactively
+* `ngc_job result --help`: download results for your jobs interactively
 * `ngc_job bash --help`: exec bash for one selected job~(support autoresuming)
```

### Comparing `ngcpp-0.0.3/ngcpp/cli/cluster_info.py` & `ngcpp-0.0.4/ngcpp/cli/cluster_info.py`

 * *Files identical despite different names*

### Comparing `ngcpp-0.0.3/ngcpp/cli/job_info.py` & `ngcpp-0.0.4/ngcpp/cli/job_info.py`

 * *Files identical despite different names*

### Comparing `ngcpp-0.0.3/ngcpp/cluster.py` & `ngcpp-0.0.4/ngcpp/cluster.py`

 * *Files identical despite different names*

### Comparing `ngcpp-0.0.3/ngcpp/cluster.yaml` & `ngcpp-0.0.4/ngcpp/cluster.yaml`

 * *Files identical despite different names*

### Comparing `ngcpp-0.0.3/pyproject.toml` & `ngcpp-0.0.4/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ngcpp"
-version = "0.0.3"
+version = "0.0.4"
 description = "A toolkit for ngc"
 authors = ["Qinsheng <qsh.zh27@gmail.com>"]
 readme = "README.md"
 keywords = ["jam", "experiment", "ngc"]
 license = "MIT"
 packages = [
     {include = "ngcpp"},
```

### Comparing `ngcpp-0.0.3/PKG-INFO` & `ngcpp-0.0.4/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ngcpp
-Version: 0.0.3
+Version: 0.0.4
 Summary: A toolkit for ngc
 License: MIT
 Keywords: jam,experiment,ngc
 Author: Qinsheng
 Author-email: qsh.zh27@gmail.com
 Requires-Python: >=3.8,<3.11
 Classifier: License :: OSI Approved :: MIT License
@@ -28,17 +28,17 @@
 ```
 
 # Feature
 
 ## cluster `ngc_cluster --help`
 
 * `ngc_cluster usage --help`: List user usage
-* `ngc_cluster hang --help`: List all hanging jobs
-* `ngc_cluster list --help`: List all jobs in one cluster
+* `ngc_cluster hang --help`: List your all hanging jobs
+* `ngc_cluster list --help`: List your jobs in one cluster
 * `ngc_cluster alias --help`: List all available cluster aliases
 
 ## job `ngc_job --help`
 
-* `ngc_job kill --help`: kill jobs interactively
-* `ngc_job result --help`: download results for jobs interactively
+* `ngc_job kill --help`: kill your jobs interactively
+* `ngc_job result --help`: download results for your jobs interactively
 * `ngc_job bash --help`: exec bash for one selected job~(support autoresuming)
```


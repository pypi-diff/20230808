# Comparing `tmp/metricsoperator-0.0.12.tar.gz` & `tmp/metricsoperator-0.0.12.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "metricsoperator-0.0.12.tar", last modified: Mon Aug  7 12:53:34 2023, max compression
+gzip compressed data, was "metricsoperator-0.0.12.1.tar", last modified: Mon Aug  7 23:24:43 2023, max compression
```

## Comparing `metricsoperator-0.0.12.tar` & `metricsoperator-0.0.12.1.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 12:53:34.910854 metricsoperator-0.0.12/
--rw-r--r--   0 runner    (1001) docker     (123)      169 2023-08-07 12:53:07.000000 metricsoperator-0.0.12/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1935 2023-08-07 12:53:34.910854 metricsoperator-0.0.12/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1100 2023-08-07 12:53:07.000000 metricsoperator-0.0.12/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 12:53:34.910854 metricsoperator-0.0.12/metricsoperator/
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-08-07 12:53:07.000000 metricsoperator-0.0.12/metricsoperator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1535 2023-08-07 12:53:07.000000 metricsoperator-0.0.12/metricsoperator/client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 12:53:34.910854 metricsoperator-0.0.12/metricsoperator/metrics/
--rw-r--r--   0 runner    (1001) docker     (123)      539 2023-08-07 12:53:07.000000 metricsoperator-0.0.12/metricsoperator/metrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6678 2023-08-07 12:53:07.000000 metricsoperator-0.0.12/metricsoperator/metrics/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     4453 2023-08-07 12:53:07.000000 metricsoperator-0.0.12/metricsoperator/metrics/network.py
--rw-r--r--   0 runner    (1001) docker     (123)      930 2023-08-07 12:53:07.000000 metricsoperator-0.0.12/metricsoperator/metrics/storage.py
--rw-r--r--   0 runner    (1001) docker     (123)      613 2023-08-07 12:53:07.000000 metricsoperator-0.0.12/metricsoperator/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 12:53:34.910854 metricsoperator-0.0.12/metricsoperator.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1935 2023-08-07 12:53:34.000000 metricsoperator-0.0.12/metricsoperator.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      494 2023-08-07 12:53:34.000000 metricsoperator-0.0.12/metricsoperator.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-07 12:53:34.000000 metricsoperator-0.0.12/metricsoperator.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-07 12:53:34.000000 metricsoperator-0.0.12/metricsoperator.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-08-07 12:53:34.000000 metricsoperator-0.0.12/metricsoperator.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-08-07 12:53:34.000000 metricsoperator-0.0.12/metricsoperator.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      132 2023-08-07 12:53:07.000000 metricsoperator-0.0.12/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-07 12:53:34.910854 metricsoperator-0.0.12/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2257 2023-08-07 12:53:07.000000 metricsoperator-0.0.12/setup.py
+drwxrwxr-x   0 vanessa   (1000) vanessa   (1000)        0 2023-08-07 23:24:43.988249 metricsoperator-0.0.12.1/
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      169 2023-08-06 22:03:40.000000 metricsoperator-0.0.12.1/MANIFEST.in
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1957 2023-08-07 23:24:43.988249 metricsoperator-0.0.12.1/PKG-INFO
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1100 2023-08-06 22:12:21.000000 metricsoperator-0.0.12.1/README.md
+drwxrwxr-x   0 vanessa   (1000) vanessa   (1000)        0 2023-08-07 23:24:43.988249 metricsoperator-0.0.12.1/metricsoperator/
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)       44 2023-08-06 22:03:40.000000 metricsoperator-0.0.12.1/metricsoperator/__init__.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1542 2023-08-07 23:24:08.000000 metricsoperator-0.0.12.1/metricsoperator/client.py
+drwxrwxr-x   0 vanessa   (1000) vanessa   (1000)        0 2023-08-07 23:24:43.988249 metricsoperator-0.0.12.1/metricsoperator/metrics/
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      539 2023-08-07 19:31:15.000000 metricsoperator-0.0.12.1/metricsoperator/metrics/__init__.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     7156 2023-08-07 23:24:08.000000 metricsoperator-0.0.12.1/metricsoperator/metrics/base.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     4171 2023-08-07 23:24:08.000000 metricsoperator-0.0.12.1/metricsoperator/metrics/network.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      799 2023-08-07 23:24:08.000000 metricsoperator-0.0.12.1/metricsoperator/metrics/storage.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      613 2023-08-07 05:09:52.000000 metricsoperator-0.0.12.1/metricsoperator/utils.py
+drwxrwxr-x   0 vanessa   (1000) vanessa   (1000)        0 2023-08-07 23:24:43.988249 metricsoperator-0.0.12.1/metricsoperator.egg-info/
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1957 2023-08-07 23:24:43.000000 metricsoperator-0.0.12.1/metricsoperator.egg-info/PKG-INFO
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      494 2023-08-07 23:24:43.000000 metricsoperator-0.0.12.1/metricsoperator.egg-info/SOURCES.txt
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)        1 2023-08-07 23:24:43.000000 metricsoperator-0.0.12.1/metricsoperator.egg-info/dependency_links.txt
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)        1 2023-08-06 04:14:56.000000 metricsoperator-0.0.12.1/metricsoperator.egg-info/not-zip-safe
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)       27 2023-08-07 23:24:43.000000 metricsoperator-0.0.12.1/metricsoperator.egg-info/requires.txt
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)       16 2023-08-07 23:24:43.000000 metricsoperator-0.0.12.1/metricsoperator.egg-info/top_level.txt
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      132 2023-08-06 22:03:40.000000 metricsoperator-0.0.12.1/pyproject.toml
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)       38 2023-08-07 23:24:43.988249 metricsoperator-0.0.12.1/setup.cfg
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     2259 2023-08-07 23:24:08.000000 metricsoperator-0.0.12.1/setup.py
```

### Comparing `metricsoperator-0.0.12/PKG-INFO` & `metricsoperator-0.0.12.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 Metadata-Version: 2.1
 Name: metricsoperator
-Version: 0.0.12
+Version: 0.0.12.1
 Summary: Python helpers for the Metrics Operator
 Home-page: https://github.com/converged-computing/metrics-operator/tree/main/python-sdk/v1alpha1
 Author: Vanessasaurus
 Author-email: vsoch@users.noreply.github.com
 Maintainer: Vanessasaurus
 License: MIT
 Keywords: metrics-operator,hpc,kubernetes,metrics,storage,applications
+Platform: UNKNOWN
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: C
 Classifier: Programming Language :: Python
 Classifier: Topic :: Software Development
 Classifier: Topic :: Scientific/Engineering
@@ -37,7 +38,9 @@
 See [LICENSE](https://github.com/converged-computing/cloud-select/blob/main/LICENSE),
 [COPYRIGHT](https://github.com/converged-computing/cloud-select/blob/main/COPYRIGHT), and
 [NOTICE](https://github.com/converged-computing/cloud-select/blob/main/NOTICE) for details.
 
 SPDX-License-Identifier: (MIT)
 
 LLNL-CODE- 842614
+
+
```

### Comparing `metricsoperator-0.0.12/README.md` & `metricsoperator-0.0.12.1/README.md`

 * *Files identical despite different names*

### Comparing `metricsoperator-0.0.12/metricsoperator/client.py` & `metricsoperator-0.0.12.1/metricsoperator/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,26 +6,25 @@
 import os
 
 from kubernetes import client, config
 
 import metricsoperator.metrics as mutils
 import metricsoperator.utils as utils
 
-config.load_kube_config()
-
 
 class MetricsOperator:
     def __init__(self, yaml_file):
         """
         Given a YAML file with one or more metrics, apply
         to create it and stream logs for each metric of interest.
         """
         self._core_v1 = None
         self.yaml_file = os.path.abspath(yaml_file)
         self.spec = utils.read_yaml(self.yaml_file)
+        config.load_kube_config()
 
     def watch(self):
         """
         Wait for (and yield parsed) metric logs.
         """
         for metric in self.spec["spec"]["metrics"]:
             parser = mutils.get_metric(metric["name"])(self.spec)
```

### Comparing `metricsoperator-0.0.12/metricsoperator/metrics/__init__.py` & `metricsoperator-0.0.12.1/metricsoperator/metrics/__init__.py`

 * *Files identical despite different names*

### Comparing `metricsoperator-0.0.12/metricsoperator/metrics/base.py` & `metricsoperator-0.0.12.1/metricsoperator/metrics/base.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,48 +2,63 @@
 import time
 
 from kubernetes import client, config, watch
 from kubernetes.client.api import core_v1_api
 from kubernetes.client.exceptions import ApiException
 from kubernetes.client.models.v1_pod_list import V1PodList
 
-config.load_kube_config()
-
 
 class MetricBase:
     separator = "METRICS OPERATOR TIMEPOINT"
     collection_start = "METRICS OPERATOR COLLECTION START"
     collection_end = "METRICS OPERATOR COLLECTION END"
     metadata_start = "METADATA START"
     metadata_end = "METADATA END"
 
-    def __init__(self, spec, **kwargs):
+    def __init__(self, spec=None, **kwargs):
         """
         Create a persistent client to interact with a MiniCluster
 
         This currently assumes the namespace exists.
         """
         self.spec = spec
         self._core_v1 = kwargs.get("core_v1_api")
 
+        # Load kubeconfig on Metricbase init only
+        if self.spec is not None:
+            config.load_kube_config()
+
     @property
     def namespace(self):
+        if not self.spec:
+            return
         return self.spec["metadata"].get("namespace") or "default"
 
     @property
     def name(self):
+        if not self.spec:
+            return
         return self.spec["metadata"]["name"]
 
     @property
     def classname(self):
         return self.__class__.__name__
 
     def container(self):
         return self.classname.replace("-", "_")
 
+    def parse(self, pod, container):
+        """
+        Retrieve logs output and call parsing function
+        """
+        lines = self.stream_output(
+            name=pod.metadata.name, namespace=self.namespace, container=container.name
+        )
+        return self.parse_log(lines)
+
     @property
     def core_v1(self):
         """
         Instantiate a core_v1 api (if not done yet)
         """
         if self._core_v1 is not None:
             return self._core_v1
```

### Comparing `metricsoperator-0.0.12/metricsoperator/metrics/network.py` & `metricsoperator-0.0.12.1/metricsoperator/metrics/network.py`

 * *Files 4% similar despite different names*

```diff
@@ -19,22 +19,18 @@
     def parse_row(self, row):
         """
         Given a row of two values with spaces, parse.
         """
         row = row.split(" ", 1)
         return [x.strip() for x in row]
 
-    def parse(self, pod, container):
+    def parse_log(self, lines):
         """
-        Parse osu benchmark output log and return json
+        Given lines of output, parse and return json
         """
-        lines = self.stream_output(
-            name=pod.metadata.name, namespace=self.namespace, container=container.name
-        )
-
         # Get the log metadata
         metadata = self.get_log_metadata(lines)
 
         # Split lines by separator
         results = []
         sections = self.get_log_sections(lines)
         for section in sections:
@@ -90,22 +86,18 @@
     def parse_row(self, row):
         """
         Given a row of netmark output, parse!
         """
         row = row.split(" ", 1)
         return [x.strip() for x in row]
 
-    def parse(self, pod, container):
+    def parse_log(self, lines):
         """
-        Parse osu benchmark output log and return json
+        Given lines of output, parse and return json
         """
-        lines = self.stream_output(
-            name=pod.metadata.name, namespace=self.namespace, container=container.name
-        )
-
         # Get the log metadata
         metadata = self.get_log_metadata(lines)
 
         # Split lines by separator
         results = []
         sections = self.get_log_sections(lines)
```

### Comparing `metricsoperator-0.0.12/metricsoperator/metrics/storage.py` & `metricsoperator-0.0.12.1/metricsoperator/metrics/storage.py`

 * *Files 23% similar despite different names*

```diff
@@ -9,22 +9,18 @@
 class io_sysstat(MetricBase):
     container_name = "io-sysstat"
 
     @property
     def pod_prefix(self):
         return f"{self.name}-m-0"
 
-    def parse(self, pod, container):
+    def parse_log(self, lines):
         """
-        Parse io_sysstat log and return json
+        Given lines of output, parse and return json
         """
-        lines = self.stream_output(
-            name=pod.metadata.name, namespace=self.namespace, container=container.name
-        )
-
         # Get the log metadata
         metadata = self.get_log_metadata(lines)
 
         # Split lines by IOSTAT TIMEPOINT
         results = []
         sections = self.get_log_sections(lines)
         for section in sections:
```

### Comparing `metricsoperator-0.0.12/metricsoperator/utils.py` & `metricsoperator-0.0.12.1/metricsoperator/utils.py`

 * *Files identical despite different names*

### Comparing `metricsoperator-0.0.12/metricsoperator.egg-info/PKG-INFO` & `metricsoperator-0.0.12.1/metricsoperator.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 Metadata-Version: 2.1
 Name: metricsoperator
-Version: 0.0.12
+Version: 0.0.12.1
 Summary: Python helpers for the Metrics Operator
 Home-page: https://github.com/converged-computing/metrics-operator/tree/main/python-sdk/v1alpha1
 Author: Vanessasaurus
 Author-email: vsoch@users.noreply.github.com
 Maintainer: Vanessasaurus
 License: MIT
 Keywords: metrics-operator,hpc,kubernetes,metrics,storage,applications
+Platform: UNKNOWN
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: C
 Classifier: Programming Language :: Python
 Classifier: Topic :: Software Development
 Classifier: Topic :: Scientific/Engineering
@@ -37,7 +38,9 @@
 See [LICENSE](https://github.com/converged-computing/cloud-select/blob/main/LICENSE),
 [COPYRIGHT](https://github.com/converged-computing/cloud-select/blob/main/COPYRIGHT), and
 [NOTICE](https://github.com/converged-computing/cloud-select/blob/main/NOTICE) for details.
 
 SPDX-License-Identifier: (MIT)
 
 LLNL-CODE- 842614
+
+
```

### Comparing `metricsoperator-0.0.12/setup.py` & `metricsoperator-0.0.12.1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 ################################################################################
 # MAIN #########################################################################
 ################################################################################
 
 if __name__ == "__main__":
     setup(
         name="metricsoperator",
-        version="0.0.12",
+        version="0.0.12.1",
         author="Vanessasaurus",
         author_email="vsoch@users.noreply.github.com",
         maintainer="Vanessasaurus",
         packages=find_packages(),
         include_package_data=True,
         zip_safe=False,
         url="https://github.com/converged-computing/metrics-operator/tree/main/python-sdk/v1alpha1",
```


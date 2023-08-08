# Comparing `tmp/prosimos-1.2.7.tar.gz` & `tmp/prosimos-1.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prosimos-1.2.7.tar", max compression
+gzip compressed data, was "prosimos-1.2.8.tar", max compression
```

## Comparing `prosimos-1.2.7.tar` & `prosimos-1.2.8.tar`

### file list

```diff
@@ -1,32 +1,32 @@
--rw-r--r--   0        0        0    15559 2023-06-27 12:32:18.241897 prosimos-1.2.7/README.md
--rw-r--r--   0        0        0        0 2023-06-27 12:32:18.257897 prosimos-1.2.7/bpdfr_discovery/__init__.py
--rw-r--r--   0        0        0     3478 2023-06-27 12:32:18.257897 prosimos-1.2.7/bpdfr_discovery/emd_metric.py
--rw-r--r--   0        0        0      489 2023-06-27 12:32:18.257897 prosimos-1.2.7/bpdfr_discovery/exceptions.py
--rw-r--r--   0        0        0     7248 2023-06-27 12:32:18.257897 prosimos-1.2.7/bpdfr_discovery/inter_arrival_cases_discovery.py
--rw-r--r--   0        0        0     5615 2023-06-27 12:32:18.257897 prosimos-1.2.7/bpdfr_discovery/log_comparison_metrics.py
--rw-r--r--   0        0        0    44127 2023-06-27 12:32:18.257897 prosimos-1.2.7/bpdfr_discovery/log_parser.py
--rw-r--r--   0        0        0        0 2023-06-27 12:32:18.257897 prosimos-1.2.7/cli/__init__.py
--rw-r--r--   0        0        0     3539 2023-06-27 12:32:18.257897 prosimos-1.2.7/cli/diff_res_bpsim.py
--rw-r--r--   0        0        0        0 2023-06-27 12:32:18.361896 prosimos-1.2.7/prosimos/__init__.py
--rw-r--r--   0        0        0    44604 2023-06-27 12:32:18.361896 prosimos-1.2.7/prosimos/batch_processing.py
--rw-r--r--   0        0        0     4401 2023-06-27 12:32:18.361896 prosimos-1.2.7/prosimos/batch_processing_parser.py
--rw-r--r--   0        0        0     2409 2023-06-27 12:32:18.361896 prosimos-1.2.7/prosimos/case_attributes.py
--rw-r--r--   0        0        0    48417 2023-06-27 12:32:18.361896 prosimos-1.2.7/prosimos/control_flow_manager.py
--rw-r--r--   0        0        0      623 2023-06-27 12:32:18.361896 prosimos-1.2.7/prosimos/exceptions.py
--rw-r--r--   0        0        0     7340 2023-06-27 12:32:18.361896 prosimos-1.2.7/prosimos/execution_info.py
--rw-r--r--   0        0        0     1109 2023-06-27 12:32:18.361896 prosimos-1.2.7/prosimos/file_manager.py
--rw-r--r--   0        0        0      555 2023-06-27 12:32:18.361896 prosimos-1.2.7/prosimos/histogram_distribution.py
--rw-r--r--   0        0        0     3147 2023-06-27 12:32:18.361896 prosimos-1.2.7/prosimos/prioritisation.py
--rw-r--r--   0        0        0     1345 2023-06-27 12:32:18.361896 prosimos-1.2.7/prosimos/prioritisation_parser.py
--rw-r--r--   0        0        0     3009 2023-06-27 12:32:18.361896 prosimos-1.2.7/prosimos/prioritisation_rules.py
--rw-r--r--   0        0        0     7010 2023-06-27 12:32:18.361896 prosimos-1.2.7/prosimos/probability_distributions.py
--rw-r--r--   0        0        0      467 2023-06-27 12:32:18.361896 prosimos-1.2.7/prosimos/resource_profile.py
--rw-r--r--   0        0        0    29277 2023-06-27 12:32:18.361896 prosimos-1.2.7/prosimos/simulation_engine.py
--rw-r--r--   0        0        0    21739 2023-06-27 12:32:18.361896 prosimos-1.2.7/prosimos/simulation_properties_parser.py
--rw-r--r--   0        0        0     6298 2023-06-27 12:32:18.361896 prosimos-1.2.7/prosimos/simulation_queues_ds.py
--rw-r--r--   0        0        0     6584 2023-06-27 12:32:18.361896 prosimos-1.2.7/prosimos/simulation_setup.py
--rw-r--r--   0        0        0    15565 2023-06-27 12:32:18.361896 prosimos-1.2.7/prosimos/simulation_stats.py
--rw-r--r--   0        0        0    14171 2023-06-27 12:32:18.361896 prosimos-1.2.7/prosimos/simulation_stats_calculator.py
--rw-r--r--   0        0        0     1730 2023-06-27 12:32:18.361896 prosimos-1.2.7/prosimos/weekday_helper.py
--rw-r--r--   0        0        0      669 2023-06-27 12:32:18.361896 prosimos-1.2.7/pyproject.toml
--rw-r--r--   0        0        0    16306 1970-01-01 00:00:00.000000 prosimos-1.2.7/PKG-INFO
+-rw-r--r--   0        0        0    10398 2023-08-08 13:38:16.816498 prosimos-1.2.8/README.md
+-rw-r--r--   0        0        0        0 2023-08-08 13:38:16.832498 prosimos-1.2.8/bpdfr_discovery/__init__.py
+-rw-r--r--   0        0        0     3478 2023-08-08 13:38:16.832498 prosimos-1.2.8/bpdfr_discovery/emd_metric.py
+-rw-r--r--   0        0        0      489 2023-08-08 13:38:16.832498 prosimos-1.2.8/bpdfr_discovery/exceptions.py
+-rw-r--r--   0        0        0     7248 2023-08-08 13:38:16.832498 prosimos-1.2.8/bpdfr_discovery/inter_arrival_cases_discovery.py
+-rw-r--r--   0        0        0     5615 2023-08-08 13:38:16.832498 prosimos-1.2.8/bpdfr_discovery/log_comparison_metrics.py
+-rw-r--r--   0        0        0    44127 2023-08-08 13:38:16.832498 prosimos-1.2.8/bpdfr_discovery/log_parser.py
+-rw-r--r--   0        0        0        0 2023-08-08 13:38:16.832498 prosimos-1.2.8/cli/__init__.py
+-rw-r--r--   0        0        0     3539 2023-08-08 13:38:16.832498 prosimos-1.2.8/cli/diff_res_bpsim.py
+-rw-r--r--   0        0        0        0 2023-08-08 13:38:16.928500 prosimos-1.2.8/prosimos/__init__.py
+-rw-r--r--   0        0        0    44604 2023-08-08 13:38:16.928500 prosimos-1.2.8/prosimos/batch_processing.py
+-rw-r--r--   0        0        0     4401 2023-08-08 13:38:16.928500 prosimos-1.2.8/prosimos/batch_processing_parser.py
+-rw-r--r--   0        0        0     2409 2023-08-08 13:38:16.928500 prosimos-1.2.8/prosimos/case_attributes.py
+-rw-r--r--   0        0        0    48417 2023-08-08 13:38:16.932500 prosimos-1.2.8/prosimos/control_flow_manager.py
+-rw-r--r--   0        0        0      623 2023-08-08 13:38:16.932500 prosimos-1.2.8/prosimos/exceptions.py
+-rw-r--r--   0        0        0     7340 2023-08-08 13:38:16.932500 prosimos-1.2.8/prosimos/execution_info.py
+-rw-r--r--   0        0        0     1109 2023-08-08 13:38:16.932500 prosimos-1.2.8/prosimos/file_manager.py
+-rw-r--r--   0        0        0      555 2023-08-08 13:38:16.932500 prosimos-1.2.8/prosimos/histogram_distribution.py
+-rw-r--r--   0        0        0     3147 2023-08-08 13:38:16.932500 prosimos-1.2.8/prosimos/prioritisation.py
+-rw-r--r--   0        0        0     1345 2023-08-08 13:38:16.932500 prosimos-1.2.8/prosimos/prioritisation_parser.py
+-rw-r--r--   0        0        0     3009 2023-08-08 13:38:16.932500 prosimos-1.2.8/prosimos/prioritisation_rules.py
+-rw-r--r--   0        0        0     7010 2023-08-08 13:38:16.932500 prosimos-1.2.8/prosimos/probability_distributions.py
+-rw-r--r--   0        0        0      467 2023-08-08 13:38:16.932500 prosimos-1.2.8/prosimos/resource_profile.py
+-rw-r--r--   0        0        0    29277 2023-08-08 13:38:16.932500 prosimos-1.2.8/prosimos/simulation_engine.py
+-rw-r--r--   0        0        0    21739 2023-08-08 13:38:16.932500 prosimos-1.2.8/prosimos/simulation_properties_parser.py
+-rw-r--r--   0        0        0     6298 2023-08-08 13:38:16.932500 prosimos-1.2.8/prosimos/simulation_queues_ds.py
+-rw-r--r--   0        0        0     6584 2023-08-08 13:38:16.932500 prosimos-1.2.8/prosimos/simulation_setup.py
+-rw-r--r--   0        0        0    15565 2023-08-08 13:38:16.932500 prosimos-1.2.8/prosimos/simulation_stats.py
+-rw-r--r--   0        0        0    14171 2023-08-08 13:38:16.932500 prosimos-1.2.8/prosimos/simulation_stats_calculator.py
+-rw-r--r--   0        0        0     1730 2023-08-08 13:38:16.932500 prosimos-1.2.8/prosimos/weekday_helper.py
+-rw-r--r--   0        0        0      733 2023-08-08 13:38:16.932500 prosimos-1.2.8/pyproject.toml
+-rw-r--r--   0        0        0    11155 1970-01-01 00:00:00.000000 prosimos-1.2.8/PKG-INFO
```

### Comparing `prosimos-1.2.7/bpdfr_discovery/emd_metric.py` & `prosimos-1.2.8/bpdfr_discovery/emd_metric.py`

 * *Files identical despite different names*

### Comparing `prosimos-1.2.7/bpdfr_discovery/inter_arrival_cases_discovery.py` & `prosimos-1.2.8/bpdfr_discovery/inter_arrival_cases_discovery.py`

 * *Files identical despite different names*

### Comparing `prosimos-1.2.7/bpdfr_discovery/log_comparison_metrics.py` & `prosimos-1.2.8/bpdfr_discovery/log_comparison_metrics.py`

 * *Files identical despite different names*

### Comparing `prosimos-1.2.7/bpdfr_discovery/log_parser.py` & `prosimos-1.2.8/bpdfr_discovery/log_parser.py`

 * *Files identical despite different names*

### Comparing `prosimos-1.2.7/cli/diff_res_bpsim.py` & `prosimos-1.2.8/cli/diff_res_bpsim.py`

 * *Files identical despite different names*

### Comparing `prosimos-1.2.7/prosimos/batch_processing.py` & `prosimos-1.2.8/prosimos/batch_processing.py`

 * *Files identical despite different names*

### Comparing `prosimos-1.2.7/prosimos/batch_processing_parser.py` & `prosimos-1.2.8/prosimos/batch_processing_parser.py`

 * *Files identical despite different names*

### Comparing `prosimos-1.2.7/prosimos/case_attributes.py` & `prosimos-1.2.8/prosimos/case_attributes.py`

 * *Files identical despite different names*

### Comparing `prosimos-1.2.7/prosimos/control_flow_manager.py` & `prosimos-1.2.8/prosimos/control_flow_manager.py`

 * *Files identical despite different names*

### Comparing `prosimos-1.2.7/prosimos/exceptions.py` & `prosimos-1.2.8/prosimos/exceptions.py`

 * *Files identical despite different names*

### Comparing `prosimos-1.2.7/prosimos/execution_info.py` & `prosimos-1.2.8/prosimos/execution_info.py`

 * *Files identical despite different names*

### Comparing `prosimos-1.2.7/prosimos/file_manager.py` & `prosimos-1.2.8/prosimos/file_manager.py`

 * *Files identical despite different names*

### Comparing `prosimos-1.2.7/prosimos/histogram_distribution.py` & `prosimos-1.2.8/prosimos/histogram_distribution.py`

 * *Files identical despite different names*

### Comparing `prosimos-1.2.7/prosimos/prioritisation.py` & `prosimos-1.2.8/prosimos/prioritisation.py`

 * *Files identical despite different names*

### Comparing `prosimos-1.2.7/prosimos/prioritisation_parser.py` & `prosimos-1.2.8/prosimos/prioritisation_parser.py`

 * *Files identical despite different names*

### Comparing `prosimos-1.2.7/prosimos/prioritisation_rules.py` & `prosimos-1.2.8/prosimos/prioritisation_rules.py`

 * *Files identical despite different names*

### Comparing `prosimos-1.2.7/prosimos/probability_distributions.py` & `prosimos-1.2.8/prosimos/probability_distributions.py`

 * *Files identical despite different names*

### Comparing `prosimos-1.2.7/prosimos/simulation_engine.py` & `prosimos-1.2.8/prosimos/simulation_engine.py`

 * *Files identical despite different names*

### Comparing `prosimos-1.2.7/prosimos/simulation_properties_parser.py` & `prosimos-1.2.8/prosimos/simulation_properties_parser.py`

 * *Files identical despite different names*

### Comparing `prosimos-1.2.7/prosimos/simulation_queues_ds.py` & `prosimos-1.2.8/prosimos/simulation_queues_ds.py`

 * *Files identical despite different names*

### Comparing `prosimos-1.2.7/prosimos/simulation_setup.py` & `prosimos-1.2.8/prosimos/simulation_setup.py`

 * *Files identical despite different names*

### Comparing `prosimos-1.2.7/prosimos/simulation_stats.py` & `prosimos-1.2.8/prosimos/simulation_stats.py`

 * *Files identical despite different names*

### Comparing `prosimos-1.2.7/prosimos/simulation_stats_calculator.py` & `prosimos-1.2.8/prosimos/simulation_stats_calculator.py`

 * *Files identical despite different names*

### Comparing `prosimos-1.2.7/prosimos/weekday_helper.py` & `prosimos-1.2.8/prosimos/weekday_helper.py`

 * *Files identical despite different names*

### Comparing `prosimos-1.2.7/pyproject.toml` & `prosimos-1.2.8/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,29 +1,32 @@
 [tool.poetry]
 name = "prosimos"
-version = "1.2.7"
+version = "1.2.8"
 description = ""
-authors = ["Iryna Halenok, Orlenys López Pintado"]
+authors = [
+    "Iryna Halenok <iryna.halenok@ut.ee>",
+    "Orlenys López Pintado <orlenyslp@gmail.com>",
+]
 readme = "README.md"
 packages = [
-    {include = "cli"},
-    {include = "prosimos"},
-    {include = "bpdfr_discovery"}
+    { include = "cli" },
+    { include = "prosimos" },
+    { include = "bpdfr_discovery" },
 ]
 
 [tool.poetry.dependencies]
 python = ">=3.9,<3.12"
 click = "^8.1.3"
 numpy = "^1.24.3"
 pandas = "^2.0.1"
 python-dateutil = "^2.8.2"
 pytz = "^2023.3"
 scipy = "^1.10.1"
 pm4py = "^2.7.4"
-pix-framework = "^0.10.0"
+pix-framework = "^0.11.3"
 pylint = "^2.17.4"
 
 [tool.poetry.dev-dependencies]
 pytest = "^7.3.1"
 
 [tool.poetry.scripts]
 prosimos = "cli.diff_res_bpsim:cli"
```


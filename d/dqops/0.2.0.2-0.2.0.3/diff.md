# Comparing `tmp/dqops-0.2.0.2.tar.gz` & `tmp/dqops-0.2.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dqops-0.2.0.2.tar", last modified: Fri Jul 21 17:09:05 2023, max compression
+gzip compressed data, was "dqops-0.2.0.3.tar", last modified: Tue Aug  8 14:34:52 2023, max compression
```

## Comparing `dqops-0.2.0.2.tar` & `dqops-0.2.0.3.tar`

### file list

```diff
@@ -1,21 +1,1095 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 17:09:05.184929 dqops-0.2.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)    11353 2023-07-21 17:02:57.000000 dqops-0.2.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     7725 2023-07-21 17:09:05.184929 dqops-0.2.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6184 2023-07-21 17:02:57.000000 dqops-0.2.0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 17:09:05.184929 dqops-0.2.0.2/dqops/
--rw-r--r--   0 runner    (1001) docker     (123)      782 2023-07-21 17:02:57.000000 dqops-0.2.0.2/dqops/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      890 2023-07-21 17:02:57.000000 dqops-0.2.0.2/dqops/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3480 2023-07-21 17:02:57.000000 dqops-0.2.0.2/dqops/install.py
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-21 17:02:57.000000 dqops-0.2.0.2/dqops/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     2959 2023-07-21 17:02:57.000000 dqops-0.2.0.2/dqops/startdqo.py
--rw-r--r--   0 runner    (1001) docker     (123)     1117 2023-07-21 17:02:57.000000 dqops-0.2.0.2/dqops/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 17:09:05.184929 dqops-0.2.0.2/dqops.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7725 2023-07-21 17:09:05.000000 dqops-0.2.0.2/dqops.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      330 2023-07-21 17:09:05.000000 dqops-0.2.0.2/dqops.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-21 17:09:05.000000 dqops-0.2.0.2/dqops.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-07-21 17:09:05.000000 dqops-0.2.0.2/dqops.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      164 2023-07-21 17:09:05.000000 dqops-0.2.0.2/dqops.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-21 17:09:05.000000 dqops-0.2.0.2/dqops.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      161 2023-07-21 17:02:57.000000 dqops-0.2.0.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-07-21 17:09:05.184929 dqops-0.2.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     6456 2023-07-21 17:02:57.000000 dqops-0.2.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 14:34:52.623105 dqops-0.2.0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)    11353 2023-08-08 14:28:25.000000 dqops-0.2.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     7721 2023-08-08 14:34:52.623105 dqops-0.2.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6180 2023-08-08 14:28:25.000000 dqops-0.2.0.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 14:34:52.035098 dqops-0.2.0.3/dqops/
+-rw-r--r--   0 runner    (1001) docker     (123)      782 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      890 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 14:34:52.039098 dqops-0.2.0.3/dqops/client/
+-rw-r--r--   0 runner    (1001) docker     (123)      149 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 14:34:52.039098 dqops-0.2.0.3/dqops/client/api/
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/api/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 14:34:52.043098 dqops-0.2.0.3/dqops/client/api/check_results/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/api/check_results/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12292 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/api/check_results/get_column_partitioned_checks_results.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11469 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/api/check_results/get_column_profiling_checks_results.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12288 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/api/check_results/get_column_recurring_checks_results.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10080 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/api/check_results/get_table_data_quality_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11862 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/api/check_results/get_table_partitioned_checks_results.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11086 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/api/check_results/get_table_profiling_checks_results.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11902 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/api/check_results/get_table_recurring_checks_results.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 14:34:52.047098 dqops-0.2.0.3/dqops/client/api/check_results_overview/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/api/check_results_overview/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7152 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/api/check_results_overview/get_column_partitioned_checks_overview.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6318 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/api/check_results_overview/get_column_profiling_checks_overview.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7152 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/api/check_results_overview/get_column_recurring_checks_overview.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6726 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/api/check_results_overview/get_table_partitioned_checks_overview.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5899 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/api/check_results_overview/get_table_profiling_checks_overview.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6726 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/api/check_results_overview/get_table_recurring_checks_overview.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 14:34:52.051098 dqops-0.2.0.3/dqops/client/api/checks/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/api/checks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4902 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/api/checks/create_check.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4134 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/api/checks/delete_check.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4287 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/api/checks/get_all_checks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4103 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/api/checks/get_check.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4109 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/api/checks/get_check_folder_tree.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4893 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/api/checks/update_check.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 14:34:52.071098 dqops-0.2.0.3/dqops/client/api/columns/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/api/columns/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5913 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/api/columns/create_column.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5346 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/api/columns/delete_column.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5327 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/api/columns/get_column.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5399 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/api/columns/get_column_basic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5685 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/api/columns/get_column_comments.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5321 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/api/columns/get_column_labels.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6757 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/api/columns/get_column_partitioned_checks_basic_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6070 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/api/columns/get_column_partitioned_checks_daily.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6565 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/api/columns/get_column_partitioned_checks_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7665 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/api/columns/get_column_partitioned_checks_model_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6114 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/api/columns/get_column_partitioned_checks_monthly.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5888 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/api/columns/get_column_profiling_checks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5852 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/api/columns/get_column_profiling_checks_basic_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5664 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/api/columns/get_column_profiling_checks_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6693 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/api/columns/get_column_profiling_checks_model_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6689 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/api/columns/get_column_recurring_checks_basic_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5998 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/api/columns/get_column_recurring_checks_daily.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6497 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/api/columns/get_column_recurring_checks_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7593 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/api/columns/get_column_recurring_checks_model_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6042 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/api/columns/get_column_recurring_checks_monthly.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5761 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/api/columns/get_column_statistics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5283 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/api/columns/get_columns.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5493 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/api/columns/get_columns_statistics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6136 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/api/columns/update_column.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6841 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/api/columns/update_column_basic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6137 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/api/columns/update_column_comments.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5845 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/api/columns/update_column_labels.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6492 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/api/columns/update_column_partitioned_checks_daily.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7790 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/api/columns/update_column_partitioned_checks_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6532 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/api/columns/update_column_partitioned_checks_monthly.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6346 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/api/columns/update_column_profiling_checks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6808 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/api/columns/update_column_profiling_checks_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6424 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/api/columns/update_column_recurring_checks_daily.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7722 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/api/columns/update_column_recurring_checks_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6492 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/api/columns/update_column_recurring_checks_monthly.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 14:34:52.083098 dqops-0.2.0.3/dqops/client/api/connections/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/api/connections/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5715 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/api/connections/bulk_disable_connection_checks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5768 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/api/connections/bulk_enable_connection_checks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4628 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/api/connections/create_connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5213 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/api/connections/create_connection_basic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4109 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/api/connections/delete_connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4040 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/api/connections/get_all_connections.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4298 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/api/connections/get_connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4394 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/api/connections/get_connection_basic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4444 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/api/connections/get_connection_comments.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4932 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/api/connections/get_connection_common_columns.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4615 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/api/connections/get_connection_default_grouping_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4668 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/api/connections/get_connection_incident_grouping.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4080 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/api/connections/get_connection_labels.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5415 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/api/connections/get_connection_scheduling_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4651 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/api/connections/update_connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5180 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/api/connections/update_connection_basic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4964 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/api/connections/update_connection_comments.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5079 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/api/connections/update_connection_default_grouping_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5238 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/api/connections/update_connection_incident_grouping.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4628 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/api/connections/update_connection_labels.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6232 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/api/connections/update_connection_scheduling_group.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 14:34:52.087098 dqops-0.2.0.3/dqops/client/api/dashboards/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/api/dashboards/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4043 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/api/dashboards/get_all_dashboards.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5772 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/api/dashboards/get_dashboard_level_1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6109 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/api/dashboards/get_dashboard_level_2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6463 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/api/dashboards/get_dashboard_level_3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6784 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/api/dashboards/get_dashboard_level_4.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 14:34:52.091098 dqops-0.2.0.3/dqops/client/api/data_grouping_configurations/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/api/data_grouping_configurations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6161 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/api/data_grouping_configurations/create_table_grouping_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5879 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/api/data_grouping_configurations/delete_table_grouping_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6028 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/api/data_grouping_configurations/get_table_grouping_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5729 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/api/data_grouping_configurations/get_table_grouping_configurations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6142 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/api/data_grouping_configurations/set_table_default_grouping_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7019 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/api/data_grouping_configurations/update_table_grouping_configuration.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 14:34:52.091098 dqops-0.2.0.3/dqops/client/api/data_sources/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/api/data_sources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4841 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/api/data_sources/get_remote_data_source_schemas.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5388 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/api/data_sources/get_remote_data_source_tables.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5966 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/api/data_sources/test_connection.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 14:34:52.091098 dqops-0.2.0.3/dqops/client/api/environment/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/api/environment/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3732 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/api/environment/get_dqo_settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3735 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/api/environment/get_user_profile.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 14:34:52.099099 dqops-0.2.0.3/dqops/client/api/errors/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/api/errors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12114 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/api/errors/get_column_partitioned_errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11369 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/api/errors/get_column_profiling_errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12098 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/api/errors/get_column_recurring_errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11672 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/api/errors/get_table_partitioned_errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10970 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/api/errors/get_table_profiling_errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11708 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/api/errors/get_table_recurring_errors.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 14:34:52.103098 dqops-0.2.0.3/dqops/client/api/incidents/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/api/incidents/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4415 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/api/incidents/find_connection_incident_stats.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11222 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/api/incidents/find_recent_incidents_on_connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5144 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/api/incidents/get_incident.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8882 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/api/incidents/get_incident_histogram.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11697 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/api/incidents/get_incident_issues.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5692 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/api/incidents/set_incident_issue_url.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5868 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/api/incidents/set_incident_status.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 14:34:52.111099 dqops-0.2.0.3/dqops/client/api/jobs/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/api/jobs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3848 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/api/jobs/cancel_job.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4945 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/api/jobs/collect_statistics_on_data_groups.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4722 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/api/jobs/collect_statistics_on_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4723 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/api/jobs/delete_stored_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3948 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/api/jobs/get_all_jobs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4197 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/api/jobs/get_job.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4648 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/api/jobs/get_job_changes_since.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4501 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/api/jobs/import_tables.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3811 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/api/jobs/is_cron_scheduler_running.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6293 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/api/jobs/run_checks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3877 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/api/jobs/start_cron_scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3868 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/api/jobs/stop_cron_scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5466 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/api/jobs/synchronize_folders.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5330 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/api/jobs/wait_for_job.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5371 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/api/jobs/wait_for_run_checks_job.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 14:34:52.111099 dqops-0.2.0.3/dqops/client/api/log_shipping/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/api/log_shipping/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4429 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/api/log_shipping/log_debug.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4433 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/api/log_shipping/log_error.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4424 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/api/log_shipping/log_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4420 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/api/log_shipping/log_warn.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 14:34:52.115099 dqops-0.2.0.3/dqops/client/api/rules/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/api/rules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4705 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/api/rules/create_rule.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4064 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/api/rules/delete_rule.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4204 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/api/rules/get_all_rules.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3996 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/api/rules/get_rule.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4026 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/api/rules/get_rule_folder_tree.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4780 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/api/rules/update_rule.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 14:34:52.119099 dqops-0.2.0.3/dqops/client/api/schemas/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/api/schemas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12533 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/api/schemas/get_schema_partitioned_checks_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8751 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/api/schemas/get_schema_partitioned_checks_templates.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11491 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/api/schemas/get_schema_profiling_checks_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7827 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/api/schemas/get_schema_profiling_checks_templates.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12401 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/api/schemas/get_schema_recurring_checks_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8697 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/api/schemas/get_schema_recurring_checks_templates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4435 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/api/schemas/get_schemas.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 14:34:52.123099 dqops-0.2.0.3/dqops/client/api/sensor_readouts/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/api/sensor_readouts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12383 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/api/sensor_readouts/get_column_partitioned_sensor_readouts.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11501 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/api/sensor_readouts/get_column_profiling_sensor_readouts.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12419 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/api/sensor_readouts/get_column_recurring_sensor_readouts.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11977 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/api/sensor_readouts/get_table_partitioned_sensor_readouts.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11126 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/api/sensor_readouts/get_table_profiling_sensor_readouts.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11953 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/api/sensor_readouts/get_table_recurring_sensor_readouts.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 14:34:52.127099 dqops-0.2.0.3/dqops/client/api/sensors/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/api/sensors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4765 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/api/sensors/create_sensor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4122 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/api/sensors/delete_sensor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4264 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/api/sensors/get_all_sensors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4072 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/api/sensors/get_sensor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4086 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/api/sensors/get_sensor_folder_tree.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5152 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/api/sensors/update_sensor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 14:34:52.127099 dqops-0.2.0.3/dqops/client/api/table_comparison_results/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/api/table_comparison_results/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7439 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/api/table_comparison_results/get_table_comparison_partitioned_results.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6435 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/api/table_comparison_results/get_table_comparison_profiling_results.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7247 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/api/table_comparison_results/get_table_comparison_recurring_results.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 14:34:52.139099 dqops-0.2.0.3/dqops/client/api/table_comparisons/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/api/table_comparisons/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6820 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/api/table_comparisons/create_table_comparison_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6300 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/api/table_comparisons/create_table_comparison_partitioned_daily.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6318 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/api/table_comparisons/create_table_comparison_partitioned_monthly.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6268 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/api/table_comparisons/create_table_comparison_profiling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6282 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/api/table_comparisons/create_table_comparison_recurring_daily.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6300 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/api/table_comparisons/create_table_comparison_recurring_monthly.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6015 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/api/table_comparisons/delete_table_comparison_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6274 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/api/table_comparisons/get_table_comparison_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8660 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/api/table_comparisons/get_table_comparison_configurations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6264 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/api/table_comparisons/get_table_comparison_partitioned_daily.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6298 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/api/table_comparisons/get_table_comparison_partitioned_monthly.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6248 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/api/table_comparisons/get_table_comparison_profiling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6258 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/api/table_comparisons/get_table_comparison_recurring_daily.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6284 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/api/table_comparisons/get_table_comparison_recurring_monthly.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7578 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/api/table_comparisons/update_table_comparison_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7186 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/api/table_comparisons/update_table_comparison_partitioned_daily.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7220 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/api/table_comparisons/update_table_comparison_partitioned_monthly.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7026 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/api/table_comparisons/update_table_comparison_profiling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7076 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/api/table_comparisons/update_table_comparison_recurring_daily.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7094 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/api/table_comparisons/update_table_comparison_recurring_monthly.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 14:34:52.167099 dqops-0.2.0.3/dqops/client/api/tables/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/api/tables/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5431 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/api/tables/create_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4871 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/api/tables/delete_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4875 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/api/tables/get_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4983 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/api/tables/get_table_basic.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10986 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/api/tables/get_table_columns_partitioned_checks_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10070 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/api/tables/get_table_columns_profiling_checks_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10946 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/api/tables/get_table_columns_recurring_checks_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5258 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/api/tables/get_table_comments.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5638 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/api/tables/get_table_daily_partitioned_checks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5544 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/api/tables/get_table_daily_recurring_checks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5381 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/api/tables/get_table_default_grouping_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5257 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/api/tables/get_table_incident_grouping.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4906 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/api/tables/get_table_labels.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6435 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/api/tables/get_table_partitioned_checks_basic_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6319 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/api/tables/get_table_partitioned_checks_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7407 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/api/tables/get_table_partitioned_checks_model_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5682 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/api/tables/get_table_partitioned_checks_monthly.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7719 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/api/tables/get_table_partitioned_checks_templates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5137 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/api/tables/get_table_partitioning.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5416 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/api/tables/get_table_profiling_checks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5449 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/api/tables/get_table_profiling_checks_basic_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5405 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/api/tables/get_table_profiling_checks_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6342 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/api/tables/get_table_profiling_checks_model_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6845 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/api/tables/get_table_profiling_checks_templates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6367 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/api/tables/get_table_recurring_checks_basic_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6251 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/api/tables/get_table_recurring_checks_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7339 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/api/tables/get_table_recurring_checks_model_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5610 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/api/tables/get_table_recurring_checks_monthly.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7687 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/api/tables/get_table_recurring_checks_templates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6242 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/api/tables/get_table_scheduling_group_override.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5449 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/api/tables/get_table_statistics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4906 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/api/tables/get_tables.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5514 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/api/tables/update_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6051 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/api/tables/update_table_basic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5726 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/api/tables/update_table_comments.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6014 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/api/tables/update_table_daily_recurring_checks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5881 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/api/tables/update_table_default_grouping_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5749 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/api/tables/update_table_incident_grouping.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5470 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/api/tables/update_table_labels.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6082 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/api/tables/update_table_partitioned_checks_daily.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7192 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/api/tables/update_table_partitioned_checks_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6122 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/api/tables/update_table_partitioned_checks_monthly.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6027 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/api/tables/update_table_partitioning.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5936 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/api/tables/update_table_profiling_checks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6321 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/api/tables/update_table_profiling_checks_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7124 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/api/tables/update_table_recurring_checks_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6054 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/api/tables/update_table_recurring_checks_monthly.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7159 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/api/tables/update_table_scheduling_group_override.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 14:34:52.167099 dqops-0.2.0.3/dqops/client/api/timezones/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/api/timezones/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3570 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/api/timezones/get_available_zone_ids.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2817 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      470 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/errors.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 14:34:52.623105 dqops-0.2.0.3/dqops/client/models/
+-rw-r--r--   0 runner    (1001) docker     (123)   118111 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5613 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/all_checks_patch_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1841 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/all_checks_patch_parameters_selected_tables_to_columns.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2434 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/anomaly_differencing_percentile_moving_average_30_days_rule_01_parameters_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2434 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/anomaly_differencing_percentile_moving_average_30_days_rule_05_parameters_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2429 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/anomaly_differencing_percentile_moving_average_30_days_rule_1_parameters_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2506 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/anomaly_differencing_percentile_moving_average_rule_01_parameters_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2506 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/anomaly_differencing_percentile_moving_average_rule_05_parameters_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2501 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/anomaly_differencing_percentile_moving_average_rule_1_parameters_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2482 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/anomaly_stationary_percentile_moving_average_30_days_rule_01_parameters_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2482 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/anomaly_stationary_percentile_moving_average_30_days_rule_05_parameters_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2477 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/anomaly_stationary_percentile_moving_average_30_days_rule_1_parameters_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2496 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/anomaly_stationary_percentile_moving_average_rule_01_parameters_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2496 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/anomaly_stationary_percentile_moving_average_rule_05_parameters_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2491 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/anomaly_stationary_percentile_moving_average_rule_1_parameters_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2957 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/authenticated_dashboard_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1928 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/between_floats_rule_parameters_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4740 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/big_query_parameters_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)      293 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/big_query_parameters_spec_authentication_mode.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4142 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/bulk_check_disable_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1851 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/bulk_check_disable_parameters_selected_tables_to_columns.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2425 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/change_percent_1_day_rule_10_parameters_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2425 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/change_percent_1_day_rule_20_parameters_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2425 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/change_percent_1_day_rule_50_parameters_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2437 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/change_percent_30_days_rule_10_parameters_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2437 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/change_percent_30_days_rule_20_parameters_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2437 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/change_percent_30_days_rule_50_parameters_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2430 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/change_percent_7_days_rule_10_parameters_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2430 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/change_percent_7_days_rule_20_parameters_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2430 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/change_percent_7_days_rule_50_parameters_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1736 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/change_percent_rule_10_parameters_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1736 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/change_percent_rule_20_parameters_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1736 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/change_percent_rule_50_parameters_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2797 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/check_basic_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11085 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/check_configuration_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)      181 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/check_configuration_model_check_target.py
+-rw-r--r--   0 runner    (1001) docker     (123)      186 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/check_configuration_model_check_time_scale.py
+-rw-r--r--   0 runner    (1001) docker     (123)      225 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/check_configuration_model_check_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2315 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/check_container_basic_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8150 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/check_container_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)      292 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/check_container_model_effective_schedule_enabled_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3100 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/check_container_type_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)      186 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/check_container_type_model_check_time_scale.py
+-rw-r--r--   0 runner    (1001) docker     (123)      225 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/check_container_type_model_check_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20187 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/check_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)      168 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/check_model_check_target.py
+-rw-r--r--   0 runner    (1001) docker     (123)      466 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/check_model_configuration_requirements_errors_item.py
+-rw-r--r--   0 runner    (1001) docker     (123)      274 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/check_model_schedule_enabled_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10430 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/check_result_detailed_single_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5148 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/check_results_detailed_data_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7419 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/check_results_overview_data_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)      270 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/check_results_overview_data_model_statuses_item.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9437 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/check_search_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)      176 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/check_search_filters_check_target.py
+-rw-r--r--   0 runner    (1001) docker     (123)      220 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/check_search_filters_check_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)      176 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/check_search_filters_time_scale.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2580 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/check_spec_basic_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4044 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/check_spec_folder_basic_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1944 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/check_spec_folder_basic_model_folders.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3170 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/check_spec_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7835 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/check_template.py
+-rw-r--r--   0 runner    (1001) docker     (123)      171 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/check_template_check_target.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10474 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/cloud_synchronization_folders_status_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)      237 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/cloud_synchronization_folders_status_model_checks.py
+-rw-r--r--   0 runner    (1001) docker     (123)      247 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/cloud_synchronization_folders_status_model_data_check_results.py
+-rw-r--r--   0 runner    (1001) docker     (123)      241 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/cloud_synchronization_folders_status_model_data_errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)      244 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/cloud_synchronization_folders_status_model_data_incidents.py
+-rw-r--r--   0 runner    (1001) docker     (123)      249 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/cloud_synchronization_folders_status_model_data_sensor_readouts.py
+-rw-r--r--   0 runner    (1001) docker     (123)      245 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/cloud_synchronization_folders_status_model_data_statistics.py
+-rw-r--r--   0 runner    (1001) docker     (123)      236 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/cloud_synchronization_folders_status_model_rules.py
+-rw-r--r--   0 runner    (1001) docker     (123)      238 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/cloud_synchronization_folders_status_model_sensors.py
+-rw-r--r--   0 runner    (1001) docker     (123)      238 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/cloud_synchronization_folders_status_model_sources.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7555 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/collect_statistics_on_table_queue_job_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)      214 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/collect_statistics_on_table_queue_job_parameters_data_scope.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5839 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/collect_statistics_queue_job_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)      207 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/collect_statistics_queue_job_parameters_data_scope.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4437 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/collect_statistics_queue_job_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1304 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/column_accuracy_daily_partitioned_checks_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9381 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/column_accuracy_daily_recurring_checks_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1314 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/column_accuracy_monthly_partitioned_checks_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9823 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/column_accuracy_monthly_recurring_checks_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9785 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/column_accuracy_profiling_checks_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10708 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/column_accuracy_total_average_match_percent_check_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2970 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/column_accuracy_total_average_match_percent_sensor_parameters_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10634 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/column_accuracy_total_max_match_percent_check_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2950 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/column_accuracy_total_max_match_percent_sensor_parameters_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10634 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/column_accuracy_total_min_match_percent_check_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2950 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/column_accuracy_total_min_match_percent_sensor_parameters_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10767 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/column_accuracy_total_not_null_count_match_percent_check_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3007 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/column_accuracy_total_not_null_count_match_percent_sensor_parameters_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10634 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/column_accuracy_total_sum_match_percent_check_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2950 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/column_accuracy_total_sum_match_percent_sensor_parameters_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30795 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/column_anomaly_daily_partitioned_checks_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26173 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/column_anomaly_daily_recurring_checks_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11454 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/column_anomaly_differencing_sum_30_days_check_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11302 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/column_anomaly_differencing_sum_check_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5182 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/column_anomaly_monthly_partitioned_checks_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4518 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/column_anomaly_monthly_recurring_checks_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27111 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/column_anomaly_profiling_checks_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11409 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/column_anomaly_stationary_mean_30_days_check_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11337 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/column_anomaly_stationary_mean_check_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11435 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/column_anomaly_stationary_median_30_days_check_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11363 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/column_anomaly_stationary_median_check_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11551 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/column_anomaly_stationary_null_percent_30_days_check_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11455 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/column_anomaly_stationary_null_percent_check_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11468 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/column_anomaly_stationary_partition_sum_30_days_check_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11372 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/column_anomaly_stationary_partition_sum_check_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15200 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/column_basic_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3834 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/column_bool_daily_partitioned_checks_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3464 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/column_bool_daily_recurring_checks_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1793 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/column_bool_false_percent_sensor_parameters_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4062 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/column_bool_monthly_partitioned_checks_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3546 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/column_bool_monthly_recurring_checks_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3508 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/column_bool_profiling_checks_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1788 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/column_bool_true_percent_sensor_parameters_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10303 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/column_change_mean_check_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10523 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/column_change_mean_since_30_days_check_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10494 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/column_change_mean_since_7_days_check_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10487 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/column_change_mean_since_yesterday_check_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10329 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/column_change_median_check_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10549 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/column_change_median_since_30_days_check_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10520 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/column_change_median_since_7_days_check_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10513 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/column_change_median_since_yesterday_check_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10421 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/column_change_null_percent_check_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10641 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/column_change_null_percent_since_30_days_check_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10612 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/column_change_null_percent_since_7_days_check_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10605 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/column_change_null_percent_since_yesterday_check_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10290 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/column_change_sum_check_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10510 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/column_change_sum_since_30_days_check_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10481 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/column_change_sum_since_7_days_check_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10474 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/column_change_sum_since_yesterday_check_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1770 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/column_column_exists_sensor_parameters_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1783 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/column_column_type_hash_sensor_parameters_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10250 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/column_comparison_daily_partitioned_checks_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8916 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/column_comparison_daily_recurring_checks_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10344 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/column_comparison_max_match_check_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10357 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/column_comparison_mean_match_check_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10344 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/column_comparison_min_match_check_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9672 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/column_comparison_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10518 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/column_comparison_monthly_partitioned_checks_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9182 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/column_comparison_monthly_recurring_checks_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10493 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/column_comparison_not_null_count_match_check_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10449 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/column_comparison_null_count_match_check_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9144 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/column_comparison_profiling_checks_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10344 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/column_comparison_sum_match_check_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15234 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/column_daily_partitioned_check_categories_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2442 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/column_daily_partitioned_check_categories_spec_comparisons.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1954 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/column_daily_partitioned_check_categories_spec_custom.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15837 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/column_daily_recurring_check_categories_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2416 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/column_daily_recurring_check_categories_spec_comparisons.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1944 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/column_daily_recurring_check_categories_spec_custom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4970 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/column_datatype_daily_partitioned_checks_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4516 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/column_datatype_daily_recurring_checks_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10612 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/column_datatype_date_match_format_percent_check_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3146 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/column_datatype_date_match_format_percent_sensor_parameters_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)      260 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/column_datatype_date_match_format_percent_sensor_parameters_spec_date_formats.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5074 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/column_datatype_monthly_partitioned_checks_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4682 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/column_datatype_monthly_recurring_checks_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4644 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/column_datatype_profiling_checks_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9978 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/column_datatype_string_datatype_changed_check_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10581 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/column_date_values_in_future_percent_check_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5334 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/column_datetime_daily_partitioned_checks_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4886 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/column_datetime_daily_recurring_checks_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1911 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/column_datetime_date_values_in_future_percent_sensor_parameters_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5416 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/column_datetime_monthly_partitioned_checks_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4990 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/column_datetime_monthly_recurring_checks_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4952 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/column_datetime_profiling_checks_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10598 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/column_datetime_value_in_range_date_percent_check_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3201 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/column_datetime_value_in_range_date_percent_sensor_parameters_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10379 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/column_distinct_count_check_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10422 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/column_distinct_percent_check_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10294 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/column_duplicate_count_check_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10403 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/column_duplicate_percent_check_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10573 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/column_expected_numbers_in_use_count_check_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10616 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/column_expected_strings_in_top_values_count_check_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10573 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/column_expected_strings_in_use_count_check_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10321 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/column_false_percent_check_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5105 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/column_integrity_daily_partitioned_checks_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4713 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/column_integrity_daily_recurring_checks_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10625 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/column_integrity_foreign_key_match_percent_check_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2899 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/column_integrity_foreign_key_match_percent_sensor_parameters_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10552 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/column_integrity_foreign_key_not_match_count_check_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2907 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/column_integrity_foreign_key_not_match_count_sensor_parameters_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5209 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/column_integrity_monthly_partitioned_checks_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4795 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/column_integrity_monthly_recurring_checks_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4757 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/column_integrity_profiling_checks_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10393 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/column_invalid_latitude_count_check_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10406 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/column_invalid_longitude_count_check_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9780 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/column_max_in_range_check_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9793 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/column_mean_in_range_check_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9819 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/column_median_in_range_check_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9780 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/column_min_in_range_check_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3612 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/column_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15550 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/column_monthly_partitioned_check_categories_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2470 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/column_monthly_partitioned_check_categories_spec_comparisons.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1964 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/column_monthly_partitioned_check_categories_spec_custom.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16157 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/column_monthly_recurring_check_categories_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2442 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/column_monthly_recurring_check_categories_spec_comparisons.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1954 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/column_monthly_recurring_check_categories_spec_custom.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10243 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/column_negative_count_check_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10352 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/column_negative_percent_check_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10301 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/column_non_negative_count_check_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10442 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/column_non_negative_percent_check_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10330 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/column_not_nulls_count_check_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10373 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/column_not_nulls_percent_check_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10188 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/column_nulls_count_check_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18058 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/column_nulls_daily_partitioned_checks_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15712 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/column_nulls_daily_recurring_checks_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6990 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/column_nulls_monthly_partitioned_checks_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5918 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/column_nulls_monthly_recurring_checks_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1806 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/column_nulls_not_nulls_count_sensor_parameters_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2897 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/column_nulls_not_nulls_count_statistics_collector_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1816 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/column_nulls_not_nulls_percent_sensor_parameters_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2947 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/column_nulls_not_nulls_percent_statistics_collector_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1788 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/column_nulls_nulls_count_sensor_parameters_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2853 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/column_nulls_nulls_count_statistics_collector_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1798 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/column_nulls_nulls_percent_sensor_parameters_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2879 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/column_nulls_nulls_percent_statistics_collector_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10297 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/column_nulls_percent_check_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17481 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/column_nulls_profiling_checks_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6158 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/column_nulls_statistics_collectors_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10579 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/column_number_value_in_set_percent_check_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)    50357 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/column_numeric_daily_partitioned_checks_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42893 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/column_numeric_daily_recurring_checks_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2489 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/column_numeric_expected_numbers_in_use_count_sensor_parameters_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1875 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/column_numeric_invalid_latitude_count_sensor_parameters_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1880 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/column_numeric_invalid_longitude_count_sensor_parameters_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1760 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/column_numeric_max_sensor_parameters_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1765 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/column_numeric_mean_sensor_parameters_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2175 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/column_numeric_median_sensor_parameters_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1760 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/column_numeric_min_sensor_parameters_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)    51859 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/column_numeric_monthly_partitioned_checks_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)    44865 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/column_numeric_monthly_recurring_checks_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1813 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/column_numeric_negative_count_sensor_parameters_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1823 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/column_numeric_negative_percent_sensor_parameters_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1855 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/column_numeric_non_negative_count_sensor_parameters_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1865 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/column_numeric_non_negative_percent_sensor_parameters_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2601 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/column_numeric_number_value_in_set_percent_sensor_parameters_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2199 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/column_numeric_percentile_10_sensor_parameters_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2200 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/column_numeric_percentile_25_sensor_parameters_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2200 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/column_numeric_percentile_75_sensor_parameters_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2199 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/column_numeric_percentile_90_sensor_parameters_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2193 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/column_numeric_percentile_sensor_parameters_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1852 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/column_numeric_population_stddev_sensor_parameters_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1862 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/column_numeric_population_variance_sensor_parameters_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)    44827 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/column_numeric_profiling_checks_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1808 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/column_numeric_sample_stddev_sensor_parameters_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1818 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/column_numeric_sample_variance_sensor_parameters_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1760 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/column_numeric_sum_sensor_parameters_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1875 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/column_numeric_valid_latitude_percent_sensor_parameters_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1880 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/column_numeric_valid_longitude_percent_sensor_parameters_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2369 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/column_numeric_value_above_max_value_count_sensor_parameters_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2379 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/column_numeric_value_above_max_value_percent_sensor_parameters_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2369 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/column_numeric_value_below_min_value_count_sensor_parameters_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2379 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/column_numeric_value_below_min_value_percent_sensor_parameters_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2537 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/column_numeric_values_in_range_integers_percent_sensor_parameters_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2540 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/column_numeric_values_in_range_numeric_percent_sensor_parameters_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3272 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/column_partitioned_checks_root_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9932 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/column_percentile_10_in_range_check_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9932 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/column_percentile_25_in_range_check_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9932 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/column_percentile_75_in_range_check_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9932 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/column_percentile_90_in_range_check_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9901 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/column_percentile_in_range_check_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10454 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/column_pii_contains_email_percent_check_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1855 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/column_pii_contains_email_percent_sensor_parameters_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10419 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/column_pii_contains_ip_4_percent_check_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1848 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/column_pii_contains_ip_4_percent_sensor_parameters_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10419 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/column_pii_contains_ip_6_percent_check_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1848 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/column_pii_contains_ip_6_percent_sensor_parameters_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10466 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/column_pii_contains_usa_phone_percent_check_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1873 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/column_pii_contains_usa_phone_percent_sensor_parameters_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10532 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/column_pii_contains_usa_zipcode_percent_check_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1883 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/column_pii_contains_usa_zipcode_percent_sensor_parameters_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18627 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/column_pii_daily_partitioned_checks_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16189 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/column_pii_daily_recurring_checks_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19085 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/column_pii_monthly_partitioned_checks_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16785 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/column_pii_monthly_recurring_checks_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16747 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/column_pii_profiling_checks_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10401 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/column_pii_valid_email_percent_check_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1816 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/column_pii_valid_email_percent_sensor_parameters_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10490 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/column_pii_valid_ip_4_address_percent_check_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1871 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/column_pii_valid_ip_4_address_percent_sensor_parameters_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10490 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/column_pii_valid_ip_6_address_percent_check_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1871 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/column_pii_valid_ip_6_address_percent_sensor_parameters_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10459 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/column_pii_valid_usa_phone_percent_check_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1858 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/column_pii_valid_usa_phone_percent_sensor_parameters_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10485 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/column_pii_valid_usa_zipcode_percent_check_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1868 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/column_pii_valid_usa_zipcode_percent_sensor_parameters_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9998 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/column_population_stddev_in_range_check_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10024 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/column_population_variance_in_range_check_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15114 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/column_profiling_check_categories_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2346 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/column_profiling_check_categories_spec_comparisons.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1916 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/column_profiling_check_categories_spec_custom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1778 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/column_range_max_value_sensor_parameters_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2797 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/column_range_max_value_statistics_collector_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2810 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/column_range_median_value_statistics_collector_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1778 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/column_range_min_value_sensor_parameters_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2797 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/column_range_min_value_statistics_collector_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5534 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/column_range_statistics_collectors_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2771 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/column_range_sum_value_statistics_collector_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3230 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/column_recurring_checks_root_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9932 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/column_sample_stddev_in_range_check_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9958 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/column_sample_variance_in_range_check_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2185 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/column_sampling_column_samples_sensor_parameters_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2955 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/column_sampling_column_samples_statistics_collector_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2646 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/column_sampling_statistics_collectors_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9854 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/column_schema_column_exists_check_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3784 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/column_schema_daily_recurring_checks_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3880 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/column_schema_monthly_recurring_checks_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3842 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/column_schema_profiling_checks_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9725 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/column_schema_type_changed_check_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9484 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/column_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9960 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/column_sql_aggregate_expr_check_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2539 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/column_sql_aggregated_expression_sensor_parameters_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10339 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/column_sql_condition_failed_count_check_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2424 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/column_sql_condition_failed_count_sensor_parameters_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10480 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/column_sql_condition_passed_percent_check_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2434 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/column_sql_condition_passed_percent_sensor_parameters_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7098 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/column_sql_daily_partitioned_checks_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6420 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/column_sql_daily_recurring_checks_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7250 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/column_sql_monthly_partitioned_checks_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6600 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/column_sql_monthly_recurring_checks_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6562 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/column_sql_profiling_checks_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6101 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/column_statistics_collectors_root_categories_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7545 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/column_statistics_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10638 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/column_string_boolean_placeholder_percent_check_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10080 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/column_string_datatype_detected_check_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10301 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/column_string_empty_count_check_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10410 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/column_string_empty_percent_check_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10459 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/column_string_invalid_email_count_check_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10534 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/column_string_invalid_ip_4_address_count_check_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10534 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/column_string_invalid_ip_6_address_count_check_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10446 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/column_string_invalid_uuid_count_check_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10533 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/column_string_length_above_max_length_count_check_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10698 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/column_string_length_above_max_length_percent_check_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10533 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/column_string_length_below_min_length_count_check_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10698 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/column_string_length_below_min_length_percent_check_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10618 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/column_string_length_in_range_percent_check_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10631 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/column_string_match_date_regex_percent_check_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10631 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/column_string_match_name_regex_percent_check_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10574 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/column_string_match_regex_percent_check_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9813 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/column_string_max_length_check_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9962 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/column_string_mean_length_check_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9813 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/column_string_min_length_check_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10534 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/column_string_not_match_date_regex_count_check_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10477 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/column_string_not_match_regex_count_check_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10498 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/column_string_null_placeholder_count_check_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10607 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/column_string_null_placeholder_percent_check_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10644 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/column_string_parsable_to_float_percent_check_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10630 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/column_string_parsable_to_integer_percent_check_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10578 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/column_string_surrounded_by_whitespace_count_check_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10687 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/column_string_surrounded_by_whitespace_percent_check_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10617 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/column_string_valid_country_code_percent_check_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10630 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/column_string_valid_currency_code_percent_check_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10566 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/column_string_valid_dates_percent_check_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10561 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/column_string_valid_uuid_percent_check_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10579 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/column_string_value_in_set_percent_check_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10406 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/column_string_whitespace_count_check_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10537 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/column_string_whitespace_percent_check_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)    68453 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/column_strings_daily_partitioned_checks_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)    60451 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/column_strings_daily_recurring_checks_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3001 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/column_strings_expected_strings_in_top_values_count_sensor_parameters_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2488 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/column_strings_expected_strings_in_use_count_sensor_parameters_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)    70079 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/column_strings_monthly_partitioned_checks_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)    61929 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/column_strings_monthly_recurring_checks_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)    61891 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/column_strings_profiling_checks_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6888 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/column_strings_statistics_collectors_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1939 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/column_strings_string_boolean_placeholder_percent_sensor_parameters_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1875 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/column_strings_string_datatype_detect_sensor_parameters_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3092 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/column_strings_string_datatype_detect_statistics_collector_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1855 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/column_strings_string_empty_count_sensor_parameters_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1865 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/column_strings_string_empty_percent_sensor_parameters_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1893 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/column_strings_string_invalid_email_count_sensor_parameters_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1924 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/column_strings_string_invalid_ip_4_address_count_sensor_parameters_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1924 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/column_strings_string_invalid_ip_6_address_count_sensor_parameters_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1888 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/column_strings_string_invalid_uuid_count_sensor_parameters_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2493 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/column_strings_string_length_above_max_length_count_sensor_parameters_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2503 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/column_strings_string_length_above_max_length_percent_sensor_parameters_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2493 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/column_strings_string_length_below_min_length_count_sensor_parameters_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2503 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/column_strings_string_length_below_min_length_percent_sensor_parameters_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2548 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/column_strings_string_length_in_range_percent_sensor_parameters_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3207 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/column_strings_string_match_date_regex_percent_sensor_parameters_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)      331 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/column_strings_string_match_date_regex_percent_sensor_parameters_spec_date_formats.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1916 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/column_strings_string_match_name_regex_percent_sensor_parameters_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2323 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/column_strings_string_match_regex_percent_sensor_parameters_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1850 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/column_strings_string_max_length_sensor_parameters_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2973 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/column_strings_string_max_length_statistics_collector_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1855 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/column_strings_string_mean_length_sensor_parameters_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3000 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/column_strings_string_mean_length_statistics_collector_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1850 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/column_strings_string_min_length_sensor_parameters_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2973 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/column_strings_string_min_length_statistics_collector_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3182 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/column_strings_string_not_match_date_regex_count_sensor_parameters_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)      332 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/column_strings_string_not_match_date_regex_count_sensor_parameters_spec_date_formats.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2331 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/column_strings_string_not_match_regex_count_sensor_parameters_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1908 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/column_strings_string_null_placeholder_count_sensor_parameters_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1918 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/column_strings_string_null_placeholder_percent_sensor_parameters_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1921 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/column_strings_string_parsable_to_float_percent_sensor_parameters_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1937 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/column_strings_string_parsable_to_integer_percent_sensor_parameters_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2008 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/column_strings_string_surrounded_by_whitespace_count_sensor_parameters_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1962 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/column_strings_string_surrounded_by_whitespace_percent_sensor_parameters_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1926 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/column_strings_string_valid_country_code_percent_sensor_parameters_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1937 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/column_strings_string_valid_currency_code_percent_sensor_parameters_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1888 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/column_strings_string_valid_date_percent_sensor_parameters_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1888 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/column_strings_string_valid_uuid_percent_sensor_parameters_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2600 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/column_strings_string_value_in_set_percent_sensor_parameters_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1880 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/column_strings_string_whitespace_count_sensor_parameters_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1890 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/column_strings_string_whitespace_percent_sensor_parameters_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9780 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/column_sum_in_range_check_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10308 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/column_true_percent_check_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2810 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/column_type_snapshot_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7150 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/column_uniqueness_daily_partitioned_checks_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6024 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/column_uniqueness_daily_recurring_checks_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1852 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/column_uniqueness_distinct_count_sensor_parameters_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2995 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/column_uniqueness_distinct_count_statistics_collector_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1862 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/column_uniqueness_distinct_percent_sensor_parameters_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3021 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/column_uniqueness_distinct_percent_statistics_collector_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1857 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/column_uniqueness_duplicate_count_sensor_parameters_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3008 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/column_uniqueness_duplicate_count_statistics_collector_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1867 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/column_uniqueness_duplicate_percent_sensor_parameters_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3034 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/column_uniqueness_duplicate_percent_statistics_collector_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7402 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/column_uniqueness_monthly_partitioned_checks_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6178 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/column_uniqueness_monthly_recurring_checks_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6140 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/column_uniqueness_profiling_checks_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6711 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/column_uniqueness_statistics_collectors_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10508 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/column_valid_latitude_percent_check_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10521 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/column_valid_longitude_percent_check_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10464 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/column_value_above_max_value_count_check_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10605 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/column_value_above_max_value_percent_check_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10464 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/column_value_below_min_value_count_check_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10605 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/column_value_below_min_value_percent_check_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10644 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/column_values_in_range_integers_percent_check_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10599 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/column_values_in_range_numeric_percent_check_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2375 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/comment_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2033 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/common_column_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3624 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/compare_thresholds_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4973 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/comparison_check_result_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16817 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/connection_basic_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)      317 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/connection_basic_model_provider_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7057 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/connection_incident_grouping_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)      402 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/connection_incident_grouping_spec_grouping_level.py
+-rw-r--r--   0 runner    (1001) docker     (123)      214 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/connection_incident_grouping_spec_minimum_severity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2718 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/connection_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2625 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/connection_remote_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)      190 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/connection_remote_model_connection_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12935 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/connection_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)      311 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/connection_spec_provider_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10698 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/custom_check_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1218 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/custom_rule_parameters_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1704 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/custom_sensor_parameters_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3274 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/dashboard_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1284 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/dashboard_spec_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3389 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/dashboards_folder_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3794 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/data_grouping_configuration_basic_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3846 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/data_grouping_configuration_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7156 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/data_grouping_configuration_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2855 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/data_grouping_configuration_trimmed_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3784 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/data_grouping_dimension_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)      186 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/data_grouping_dimension_spec_source.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1862 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/datatype_equals_rule_parameters_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8931 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/delete_stored_data_queue_job_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4257 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/dqo_job_change_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)      318 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/dqo_job_change_model_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16878 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/dqo_job_entry_parameters_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5002 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/dqo_job_history_entry_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)      735 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/dqo_job_history_entry_model_job_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)      324 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/dqo_job_history_entry_model_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4194 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/dqo_job_queue_incremental_snapshot_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4045 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/dqo_job_queue_initial_snapshot_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2611 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/dqo_queue_job_id.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2354 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/dqo_settings_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2273 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/dqo_settings_model_properties.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1324 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/dqo_settings_model_properties_additional_property.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5428 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/dqo_user_profile_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2997 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/duration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5970 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/effective_schedule_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)      344 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/effective_schedule_model_schedule_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)      246 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/effective_schedule_model_schedule_level.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1769 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/equals_integer_1_rule_parameters_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1761 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/equals_integer_rule_parameters_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6895 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/error_detailed_single_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4933 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/errors_detailed_data_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1967 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/external_log_entry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7468 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/field_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)      179 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/find_recent_incidents_on_connection_direction.py
+-rw-r--r--   0 runner    (1001) docker     (123)      433 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/find_recent_incidents_on_connection_order.py
+-rw-r--r--   0 runner    (1001) docker     (123)      194 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/get_column_partitioned_checks_basic_model_time_scale.py
+-rw-r--r--   0 runner    (1001) docker     (123)      195 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/get_column_partitioned_checks_model_filter_time_scale.py
+-rw-r--r--   0 runner    (1001) docker     (123)      189 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/get_column_partitioned_checks_model_time_scale.py
+-rw-r--r--   0 runner    (1001) docker     (123)      192 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/get_column_partitioned_checks_overview_time_scale.py
+-rw-r--r--   0 runner    (1001) docker     (123)      191 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/get_column_partitioned_checks_results_time_scale.py
+-rw-r--r--   0 runner    (1001) docker     (123)      184 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/get_column_partitioned_errors_time_scale.py
+-rw-r--r--   0 runner    (1001) docker     (123)      192 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/get_column_partitioned_sensor_readouts_time_scale.py
+-rw-r--r--   0 runner    (1001) docker     (123)      192 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/get_column_recurring_checks_basic_model_time_scale.py
+-rw-r--r--   0 runner    (1001) docker     (123)      193 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/get_column_recurring_checks_model_filter_time_scale.py
+-rw-r--r--   0 runner    (1001) docker     (123)      187 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/get_column_recurring_checks_model_time_scale.py
+-rw-r--r--   0 runner    (1001) docker     (123)      190 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/get_column_recurring_checks_overview_time_scale.py
+-rw-r--r--   0 runner    (1001) docker     (123)      189 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/get_column_recurring_checks_results_time_scale.py
+-rw-r--r--   0 runner    (1001) docker     (123)      182 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/get_column_recurring_errors_time_scale.py
+-rw-r--r--   0 runner    (1001) docker     (123)      190 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/get_column_recurring_sensor_readouts_time_scale.py
+-rw-r--r--   0 runner    (1001) docker     (123)      352 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/get_connection_scheduling_group_scheduling_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)      165 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/get_incident_issues_direction.py
+-rw-r--r--   0 runner    (1001) docker     (123)      607 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/get_incident_issues_order.py
+-rw-r--r--   0 runner    (1001) docker     (123)      189 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/get_schema_partitioned_checks_model_check_target.py
+-rw-r--r--   0 runner    (1001) docker     (123)      189 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/get_schema_partitioned_checks_model_time_scale.py
+-rw-r--r--   0 runner    (1001) docker     (123)      193 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/get_schema_partitioned_checks_templates_check_target.py
+-rw-r--r--   0 runner    (1001) docker     (123)      193 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/get_schema_partitioned_checks_templates_time_scale.py
+-rw-r--r--   0 runner    (1001) docker     (123)      187 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/get_schema_profiling_checks_model_check_target.py
+-rw-r--r--   0 runner    (1001) docker     (123)      191 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/get_schema_profiling_checks_templates_check_target.py
+-rw-r--r--   0 runner    (1001) docker     (123)      187 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/get_schema_recurring_checks_model_check_target.py
+-rw-r--r--   0 runner    (1001) docker     (123)      187 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/get_schema_recurring_checks_model_time_scale.py
+-rw-r--r--   0 runner    (1001) docker     (123)      191 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/get_schema_recurring_checks_templates_check_target.py
+-rw-r--r--   0 runner    (1001) docker     (123)      191 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/get_schema_recurring_checks_templates_time_scale.py
+-rw-r--r--   0 runner    (1001) docker     (123)      195 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/get_table_columns_partitioned_checks_model_time_scale.py
+-rw-r--r--   0 runner    (1001) docker     (123)      193 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/get_table_columns_recurring_checks_model_time_scale.py
+-rw-r--r--   0 runner    (1001) docker     (123)      195 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/get_table_comparison_configurations_check_time_scale.py
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/get_table_comparison_configurations_check_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)      194 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/get_table_comparison_partitioned_results_time_scale.py
+-rw-r--r--   0 runner    (1001) docker     (123)      192 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/get_table_comparison_recurring_results_time_scale.py
+-rw-r--r--   0 runner    (1001) docker     (123)      188 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/get_table_data_quality_status_check_time_scale.py
+-rw-r--r--   0 runner    (1001) docker     (123)      227 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/get_table_data_quality_status_check_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)      193 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/get_table_partitioned_checks_basic_model_time_scale.py
+-rw-r--r--   0 runner    (1001) docker     (123)      194 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/get_table_partitioned_checks_model_filter_time_scale.py
+-rw-r--r--   0 runner    (1001) docker     (123)      188 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/get_table_partitioned_checks_model_time_scale.py
+-rw-r--r--   0 runner    (1001) docker     (123)      191 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/get_table_partitioned_checks_overview_time_scale.py
+-rw-r--r--   0 runner    (1001) docker     (123)      190 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/get_table_partitioned_checks_results_time_scale.py
+-rw-r--r--   0 runner    (1001) docker     (123)      192 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/get_table_partitioned_checks_templates_time_scale.py
+-rw-r--r--   0 runner    (1001) docker     (123)      183 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/get_table_partitioned_errors_time_scale.py
+-rw-r--r--   0 runner    (1001) docker     (123)      191 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/get_table_partitioned_sensor_readouts_time_scale.py
+-rw-r--r--   0 runner    (1001) docker     (123)      191 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/get_table_recurring_checks_basic_model_time_scale.py
+-rw-r--r--   0 runner    (1001) docker     (123)      192 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/get_table_recurring_checks_model_filter_time_scale.py
+-rw-r--r--   0 runner    (1001) docker     (123)      186 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/get_table_recurring_checks_model_time_scale.py
+-rw-r--r--   0 runner    (1001) docker     (123)      189 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/get_table_recurring_checks_overview_time_scale.py
+-rw-r--r--   0 runner    (1001) docker     (123)      188 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/get_table_recurring_checks_results_time_scale.py
+-rw-r--r--   0 runner    (1001) docker     (123)      190 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/get_table_recurring_checks_templates_time_scale.py
+-rw-r--r--   0 runner    (1001) docker     (123)      181 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/get_table_recurring_errors_time_scale.py
+-rw-r--r--   0 runner    (1001) docker     (123)      189 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/get_table_recurring_sensor_readouts_time_scale.py
+-rw-r--r--   0 runner    (1001) docker     (123)      355 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/get_table_scheduling_group_override_scheduling_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2135 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/hierarchy_id_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1221 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/hierarchy_id_model_path_item.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2335 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/import_schema_queue_job_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2404 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/import_tables_queue_job_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2721 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/incident_daily_issues_count.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4357 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/incident_issue_histogram_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1417 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/incident_issue_histogram_model_checks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1410 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/incident_issue_histogram_model_columns.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1978 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/incident_issue_histogram_model_days.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9875 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/incident_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)      222 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/incident_model_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4251 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/incident_webhook_notifications_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1999 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/incidents_per_connection_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1668 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/max_count_rule_0_parameters_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1673 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/max_count_rule_10_parameters_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1673 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/max_count_rule_15_parameters_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1656 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/max_days_rule_1_parameters_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1656 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/max_days_rule_2_parameters_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1656 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/max_days_rule_7_parameters_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1846 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/max_diff_percent_rule_0_parameters_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1846 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/max_diff_percent_rule_1_parameters_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1846 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/max_diff_percent_rule_5_parameters_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1817 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/max_failures_rule_0_parameters_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1822 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/max_failures_rule_10_parameters_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1817 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/max_failures_rule_5_parameters_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1738 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/max_missing_rule_0_parameters_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1738 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/max_missing_rule_1_parameters_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1738 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/max_missing_rule_2_parameters_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1716 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/max_percent_rule_0_parameters_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1726 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/max_percent_rule_100_parameters_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1716 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/max_percent_rule_1_parameters_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1716 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/max_percent_rule_2_parameters_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1716 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/max_percent_rule_5_parameters_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1721 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/max_percent_rule_95_parameters_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1721 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/max_percent_rule_99_parameters_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1664 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/max_value_rule_parameters_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1668 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/min_count_rule_0_parameters_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1688 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/min_count_rule_fatal_parameters_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1698 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/min_count_rule_warning_parameters_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1716 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/min_percent_rule_0_parameters_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1726 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/min_percent_rule_100_parameters_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1716 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/min_percent_rule_2_parameters_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1716 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/min_percent_rule_5_parameters_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1721 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/min_percent_rule_95_parameters_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1721 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/min_percent_rule_99_parameters_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1664 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/min_value_rule_parameters_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1109 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/mono.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1186 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/mono_dqo_queue_job_id.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1142 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/mono_object.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4824 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/mysql_parameters_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1243 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/mysql_parameters_spec_properties.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1704 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/optional.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1798 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/optional_check_container_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1941 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/optional_column_daily_partitioned_check_categories_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1907 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/optional_column_daily_recurring_check_categories_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1951 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/optional_column_monthly_partitioned_check_categories_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1941 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/optional_column_monthly_recurring_check_categories_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1879 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/optional_column_profiling_check_categories_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1783 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/optional_comments_list_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1856 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/optional_connection_incident_grouping_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1851 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/optional_data_grouping_configuration_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1763 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/optional_label_set_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1808 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/optional_recurring_schedule_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1912 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/optional_table_daily_partitioned_check_categories_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1902 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/optional_table_daily_recurring_check_categories_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1831 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/optional_table_incident_grouping_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1946 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/optional_table_monthly_partitioned_check_categories_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1912 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/optional_table_monthly_recurring_check_categories_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1874 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/optional_table_profiling_check_categories_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4864 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/oracle_parameters_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1248 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/oracle_parameters_spec_properties.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5578 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/parameter_definition_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)      426 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/parameter_definition_spec_data_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)      165 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/parameter_definition_spec_display_hint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5131 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/partition_incremental_time_window_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1863 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/physical_table_name.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4956 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/postgresql_parameters_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1268 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/postgresql_parameters_spec_properties.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2891 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/provider_sensor_basic_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)      321 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/provider_sensor_basic_model_provider_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5649 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/provider_sensor_definition_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1336 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/provider_sensor_definition_spec_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)      201 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/provider_sensor_definition_spec_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4475 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/provider_sensor_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)      316 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/provider_sensor_model_provider_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6176 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/quality_category_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2234 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/recurring_schedule_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5268 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/recurring_schedules_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4910 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/redshift_parameters_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1258 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/redshift_parameters_spec_properties.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3553 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/repair_stored_data_queue_job_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3789 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/rule_basic_folder_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1849 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/rule_basic_folder_model_folders.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2518 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/rule_basic_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7243 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/rule_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)      198 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/rule_model_mode.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1215 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/rule_model_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)      170 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/rule_model_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3847 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/rule_parameters_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3815 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/rule_thresholds_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4825 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/rule_time_window_settings_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)      310 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/rule_time_window_settings_spec_historic_data_point_grouping.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4715 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/run_checks_job_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)      222 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/run_checks_job_result_highest_severity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7059 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/run_checks_on_table_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5301 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/run_checks_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3916 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/run_checks_queue_job_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)      324 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/run_checks_queue_job_result_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10991 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/schema_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3620 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/schema_remote_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3984 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/sensor_basic_folder_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1877 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/sensor_basic_folder_model_folders.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4232 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/sensor_basic_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4969 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/sensor_definition_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1286 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/sensor_definition_spec_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4636 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/sensor_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6151 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/sensor_readout_detailed_single_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5612 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/sensor_readouts_detailed_data_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)      226 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/set_incident_status_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4405 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/similar_check_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)      175 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/similar_check_model_check_target.py
+-rw-r--r--   0 runner    (1001) docker     (123)      219 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/similar_check_model_check_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)      175 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/similar_check_model_time_scale.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4627 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/snowflake_parameters_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1263 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/snowflake_parameters_spec_properties.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3081 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/spring_error_payload.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4956 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/sql_server_parameters_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1266 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/sql_server_parameters_spec_properties.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6729 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/statistics_collector_search_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)      185 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/statistics_collector_search_filters_target.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5289 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/statistics_metric_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1264 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/statistics_metric_model_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)      334 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/statistics_metric_model_result_data_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7774 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/synchronize_multiple_folders_dqo_queue_job_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)      227 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/synchronize_multiple_folders_dqo_queue_job_parameters_direction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2656 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/synchronize_root_folder_dqo_queue_job_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3337 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/synchronize_root_folder_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)      211 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/synchronize_root_folder_parameters_direction.py
+-rw-r--r--   0 runner    (1001) docker     (123)      490 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/synchronize_root_folder_parameters_folder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3108 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/table_accuracy_daily_recurring_checks_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3154 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/table_accuracy_monthly_recurring_checks_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3116 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/table_accuracy_profiling_checks_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10737 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/table_accuracy_total_row_count_match_percent_check_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2433 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/table_accuracy_total_row_count_match_percent_sensor_parameters_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11527 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/table_anomaly_differencing_row_count_30_days_check_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11351 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/table_anomaly_differencing_row_count_check_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11517 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/table_anomaly_stationary_partition_row_count_30_days_check_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11445 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/table_anomaly_stationary_partition_row_count_check_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10239 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/table_availability_check_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2550 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/table_availability_daily_recurring_checks_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2596 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/table_availability_monthly_recurring_checks_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2558 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/table_availability_profiling_checks_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1762 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/table_availability_sensor_parameters_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16147 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/table_basic_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10339 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/table_change_row_count_check_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10559 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/table_change_row_count_since_30_days_check_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10530 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/table_change_row_count_since_7_days_check_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10523 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/table_change_row_count_since_yesterday_check_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1760 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/table_column_count_sensor_parameters_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1816 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/table_column_list_ordered_hash_sensor_parameters_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1850 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/table_column_list_unordered_hash_sensor_parameters_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1783 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/table_column_types_hash_sensor_parameters_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5449 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/table_columns_statistics_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8842 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/table_comparison_configuration_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)      235 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/table_comparison_configuration_model_check_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)      191 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/table_comparison_configuration_model_time_scale.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8513 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/table_comparison_configuration_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/table_comparison_configuration_spec_check_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)      190 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/table_comparison_configuration_spec_time_scale.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2972 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/table_comparison_daily_partitioned_checks_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2622 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/table_comparison_daily_recurring_checks_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3098 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/table_comparison_grouping_column_pair_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2867 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/table_comparison_grouping_columns_pair_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13371 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/table_comparison_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3018 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/table_comparison_monthly_partitioned_checks_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2682 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/table_comparison_monthly_recurring_checks_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2644 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/table_comparison_profiling_checks_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4901 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/table_comparison_results_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2688 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/table_comparison_results_model_column_comparison_results.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2156 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/table_comparison_results_model_column_comparison_results_additional_property.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2250 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/table_comparison_results_model_table_comparison_results.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10393 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/table_comparison_row_count_match_check_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6636 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/table_daily_partitioned_check_categories_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2411 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/table_daily_partitioned_check_categories_spec_comparisons.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1949 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/table_daily_partitioned_check_categories_spec_custom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9451 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/table_daily_recurring_check_categories_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2385 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/table_daily_recurring_check_categories_spec_comparisons.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1939 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/table_daily_recurring_check_categories_spec_custom.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10139 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/table_data_freshness_check_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10263 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/table_data_ingestion_delay_check_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8383 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/table_data_quality_status_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2446 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/table_data_quality_status_model_failed_checks_statuses.py
+-rw-r--r--   0 runner    (1001) docker     (123)      294 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/table_data_quality_status_model_failed_checks_statuses_additional_property.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10139 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/table_data_staleness_check_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4684 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/table_incident_grouping_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)      397 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/table_incident_grouping_spec_grouping_level.py
+-rw-r--r--   0 runner    (1001) docker     (123)      209 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/table_incident_grouping_spec_minimum_severity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2637 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/table_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6766 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/table_monthly_partitioned_check_categories_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2437 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/table_monthly_partitioned_check_categories_spec_comparisons.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1959 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/table_monthly_partitioned_check_categories_spec_custom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9619 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/table_monthly_recurring_check_categories_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2411 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/table_monthly_recurring_check_categories_spec_comparisons.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1949 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/table_monthly_recurring_check_categories_spec_custom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1891 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/table_owner_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10263 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/table_partition_reload_lag_check_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3251 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/table_partitioned_checks_root_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4596 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/table_partitioning_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10448 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/table_profiling_check_categories_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2315 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/table_profiling_check_categories_spec_comparisons.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1911 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/table_profiling_check_categories_spec_custom.py
+-rw-r--r--   0 runner    (1001) docker     (123)      322 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/table_profiling_check_categories_spec_result_truncation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3186 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/table_recurring_checks_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2652 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/table_remote_basic_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10225 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/table_row_count_check_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9724 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/table_schema_column_count_changed_check_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9810 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/table_schema_column_count_check_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9849 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/table_schema_column_list_changed_check_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9874 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/table_schema_column_list_or_order_changed_check_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9758 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/table_schema_column_types_changed_check_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8210 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/table_schema_daily_recurring_checks_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8484 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/table_schema_monthly_recurring_checks_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8446 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/table_schema_profiling_checks_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18583 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/table_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1858 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/table_spec_columns.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2414 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/table_spec_groupings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2816 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/table_spec_table_comparisons.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9811 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/table_sql_aggregate_expr_check_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2455 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/table_sql_aggregated_expression_sensor_parameters_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10312 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/table_sql_condition_failed_count_check_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2364 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/table_sql_condition_failed_count_sensor_parameters_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10467 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/table_sql_condition_passed_percent_check_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2374 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/table_sql_condition_passed_percent_sensor_parameters_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8500 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/table_sql_daily_partitioned_checks_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7800 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/table_sql_daily_recurring_checks_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8618 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/table_sql_monthly_partitioned_checks_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7962 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/table_sql_monthly_recurring_checks_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6439 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/table_sql_profiling_checks_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2322 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/table_statistics_collectors_root_categories_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6686 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/table_statistics_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6915 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/table_timeliness_daily_partitioned_checks_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4816 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/table_timeliness_daily_recurring_checks_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1823 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/table_timeliness_data_freshness_sensor_parameters_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1875 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/table_timeliness_data_ingestion_delay_sensor_parameters_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1823 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/table_timeliness_data_staleness_sensor_parameters_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7155 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/table_timeliness_monthly_partitioned_checks_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4948 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/table_timeliness_monthly_recurring_checks_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1875 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/table_timeliness_partition_reload_lag_sensor_parameters_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4910 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/table_timeliness_profiling_checks_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13225 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/table_volume_daily_partitioned_checks_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11621 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/table_volume_daily_recurring_checks_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4178 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/table_volume_monthly_partitioned_checks_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3524 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/table_volume_monthly_recurring_checks_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11951 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/table_volume_profiling_checks_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1778 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/table_volume_row_count_sensor_parameters_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2797 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/table_volume_row_count_statistics_collector_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2393 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/table_volume_statistics_collectors_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2881 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/temporal_unit.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11510 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/time_window_filter_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3347 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/timestamp_columns_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)      192 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/update_column_partitioned_checks_model_time_scale.py
+-rw-r--r--   0 runner    (1001) docker     (123)      190 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/update_column_recurring_checks_model_time_scale.py
+-rw-r--r--   0 runner    (1001) docker     (123)      355 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/update_connection_scheduling_group_scheduling_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)      191 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/update_table_partitioned_checks_model_time_scale.py
+-rw-r--r--   0 runner    (1001) docker     (123)      189 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/update_table_recurring_checks_model_time_scale.py
+-rw-r--r--   0 runner    (1001) docker     (123)      358 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/update_table_scheduling_group_override_scheduling_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1228 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/models/value_changed_parameters_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)      993 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/client/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3480 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/install.py
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     2959 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/startdqo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1117 2023-08-08 14:28:25.000000 dqops-0.2.0.3/dqops/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 14:34:52.039098 dqops-0.2.0.3/dqops.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7721 2023-08-08 14:34:51.000000 dqops-0.2.0.3/dqops.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    68273 2023-08-08 14:34:52.000000 dqops-0.2.0.3/dqops.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 14:34:51.000000 dqops-0.2.0.3/dqops.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-08-08 14:34:51.000000 dqops-0.2.0.3/dqops.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      164 2023-08-08 14:34:51.000000 dqops-0.2.0.3/dqops.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-08-08 14:34:51.000000 dqops-0.2.0.3/dqops.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      161 2023-08-08 14:28:25.000000 dqops-0.2.0.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-08-08 14:34:52.627105 dqops-0.2.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     6437 2023-08-08 14:28:25.000000 dqops-0.2.0.3/setup.py
```

### Comparing `dqops-0.2.0.2/LICENSE` & `dqops-0.2.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `dqops-0.2.0.2/PKG-INFO` & `dqops-0.2.0.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dqops
-Version: 0.2.0.2
+Version: 0.2.0.3
 Summary: DQO Data Quality Operations Center
 Home-page: https://github.com/dqops/dqo/tree/master/distribution/python
 Author: DQO Developers
 Author-email: support@dqops.com
 License: http://www.apache.org/licenses/LICENSE-2.0
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: Apache Software License
@@ -61,24 +61,24 @@
 
 
 DQO is available on [PyPi repository](https://pypi.org/project/dqops/).
 
 1. To install DQO via pip manager just run
 
     ```
-    python3 -m pip install --user dqops
+    python -m pip install --user dqops
     ```
 
    If you prefer to work with the source code, just clone our GitHub repository [https://github.com/dqops/dqo](https://github.com/dqops/dqo)
    and run
 
 2. Run dqo app to finalize the installation.
 
     ```
-    python3 -m dqops
+    python -m dqops
     ```
 
 3. Create DQO userhome folder.
 
    After installation, you will be asked whether to initialize the DQO user's home folder in the default location. Type Y to create the folder.  
    The user's home folder locally stores data such as sensor readouts and the data quality check results, as well as data source configurations. [You can learn more about data storage here](https://dqops.com/docs/dqo-concepts/data-storage/data-storage/).
 
@@ -106,23 +106,23 @@
 The DQO client could be used inside data pipelines or data preparation code to verify the quality of tables.
 
 Usage of the DQO client.
 
 ```python
 from dqops.client import Client
 
-client = Client(base_url="http://localhost:8888/")
+client = Client(base_url="http://localhost:8888")
 ```
 
 If the endpoints you're going to hit require authentication, use `AuthenticatedClient` instead:
 
 ```python
 from dqops.client import AuthenticatedClient
 
-client = AuthenticatedClient(base_url="http://localhost:8888/", token="Your DQO Cloud API Key")
+client = AuthenticatedClient(base_url="http://localhost:8888", token="Your DQO Cloud API Key")
 ```
 
 Now call your endpoint and use your models:
 
 ```python
 from dqops.client.models import MyDataModel
 from dqops.client.api.my_tag import get_my_data_model
```

### Comparing `dqops-0.2.0.2/README.md` & `dqops-0.2.0.3/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -26,24 +26,24 @@
 
 
 DQO is available on [PyPi repository](https://pypi.org/project/dqops/).
 
 1. To install DQO via pip manager just run
 
     ```
-    python3 -m pip install --user dqops
+    python -m pip install --user dqops
     ```
 
    If you prefer to work with the source code, just clone our GitHub repository [https://github.com/dqops/dqo](https://github.com/dqops/dqo)
    and run
 
 2. Run dqo app to finalize the installation.
 
     ```
-    python3 -m dqops
+    python -m dqops
     ```
 
 3. Create DQO userhome folder.
 
    After installation, you will be asked whether to initialize the DQO user's home folder in the default location. Type Y to create the folder.  
    The user's home folder locally stores data such as sensor readouts and the data quality check results, as well as data source configurations. [You can learn more about data storage here](https://dqops.com/docs/dqo-concepts/data-storage/data-storage/).
 
@@ -71,23 +71,23 @@
 The DQO client could be used inside data pipelines or data preparation code to verify the quality of tables.
 
 Usage of the DQO client.
 
 ```python
 from dqops.client import Client
 
-client = Client(base_url="http://localhost:8888/")
+client = Client(base_url="http://localhost:8888")
 ```
 
 If the endpoints you're going to hit require authentication, use `AuthenticatedClient` instead:
 
 ```python
 from dqops.client import AuthenticatedClient
 
-client = AuthenticatedClient(base_url="http://localhost:8888/", token="Your DQO Cloud API Key")
+client = AuthenticatedClient(base_url="http://localhost:8888", token="Your DQO Cloud API Key")
 ```
 
 Now call your endpoint and use your models:
 
 ```python
 from dqops.client.models import MyDataModel
 from dqops.client.api.my_tag import get_my_data_model
```

### Comparing `dqops-0.2.0.2/dqops/__init__.py` & `dqops-0.2.0.3/dqops/__init__.py`

 * *Files identical despite different names*

### Comparing `dqops-0.2.0.2/dqops/__main__.py` & `dqops-0.2.0.3/dqops/__main__.py`

 * *Files identical despite different names*

### Comparing `dqops-0.2.0.2/dqops/install.py` & `dqops-0.2.0.3/dqops/install.py`

 * *Files identical despite different names*

### Comparing `dqops-0.2.0.2/dqops/startdqo.py` & `dqops-0.2.0.3/dqops/startdqo.py`

 * *Files identical despite different names*

### Comparing `dqops-0.2.0.2/dqops/version.py` & `dqops-0.2.0.3/dqops/version.py`

 * *Files 8% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limit
 
 # WARNING: the next two lines with the version numbers (VERSION =, PIP_VERSION =) should not be modified manually. They are changed by a maven profile at compile time.
-VERSION = "0.2.0-beta2"
-PIP_VERSION = "0.2.0.2"
+VERSION = "0.2.0-beta3"
+PIP_VERSION = "0.2.0.3"
 GITHUB_RELEASE = "v" + VERSION + ""
 JAVA_VERSION = "17"
 
 
 def get_dqo_version():
     return VERSION, PIP_VERSION, GITHUB_RELEASE, JAVA_VERSION
```

### Comparing `dqops-0.2.0.2/dqops.egg-info/PKG-INFO` & `dqops-0.2.0.3/dqops.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dqops
-Version: 0.2.0.2
+Version: 0.2.0.3
 Summary: DQO Data Quality Operations Center
 Home-page: https://github.com/dqops/dqo/tree/master/distribution/python
 Author: DQO Developers
 Author-email: support@dqops.com
 License: http://www.apache.org/licenses/LICENSE-2.0
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: Apache Software License
@@ -61,24 +61,24 @@
 
 
 DQO is available on [PyPi repository](https://pypi.org/project/dqops/).
 
 1. To install DQO via pip manager just run
 
     ```
-    python3 -m pip install --user dqops
+    python -m pip install --user dqops
     ```
 
    If you prefer to work with the source code, just clone our GitHub repository [https://github.com/dqops/dqo](https://github.com/dqops/dqo)
    and run
 
 2. Run dqo app to finalize the installation.
 
     ```
-    python3 -m dqops
+    python -m dqops
     ```
 
 3. Create DQO userhome folder.
 
    After installation, you will be asked whether to initialize the DQO user's home folder in the default location. Type Y to create the folder.  
    The user's home folder locally stores data such as sensor readouts and the data quality check results, as well as data source configurations. [You can learn more about data storage here](https://dqops.com/docs/dqo-concepts/data-storage/data-storage/).
 
@@ -106,23 +106,23 @@
 The DQO client could be used inside data pipelines or data preparation code to verify the quality of tables.
 
 Usage of the DQO client.
 
 ```python
 from dqops.client import Client
 
-client = Client(base_url="http://localhost:8888/")
+client = Client(base_url="http://localhost:8888")
 ```
 
 If the endpoints you're going to hit require authentication, use `AuthenticatedClient` instead:
 
 ```python
 from dqops.client import AuthenticatedClient
 
-client = AuthenticatedClient(base_url="http://localhost:8888/", token="Your DQO Cloud API Key")
+client = AuthenticatedClient(base_url="http://localhost:8888", token="Your DQO Cloud API Key")
 ```
 
 Now call your endpoint and use your models:
 
 ```python
 from dqops.client.models import MyDataModel
 from dqops.client.api.my_tag import get_my_data_model
```

### Comparing `dqops-0.2.0.2/setup.py` & `dqops-0.2.0.3/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -18,14 +18,15 @@
 
 from glob import glob
 import os
 import sys
 import zipfile
 import jdk
 from setuptools import setup
+from setuptools import find_packages
 import importlib.util
 from setuptools.command.install import install
 from shutil import rmtree
 
 # ignore those, they are filled by importing dqops/version.py
 VERSION = "filled by dqops/version.py"
 PIP_VERSION = "filled by dqops/version.py"
@@ -107,19 +108,16 @@
         version=PIP_VERSION,
         description='DQO Data Quality Operations Center',
         long_description=long_description,
         long_description_content_type="text/markdown",
         author='DQO Developers',
         author_email='support@dqops.com',
         url='https://github.com/dqops/dqo/tree/master/distribution/python',
-        packages=['dqops'],
+        packages=find_packages(),
         include_package_data=True,
-        package_dir={
-            'dqops': 'dqops'
-        },
         package_data={
             'dqops': ['py.typed']
         },
         license='http://www.apache.org/licenses/LICENSE-2.0',
         install_requires=['install-jdk>=1.0.4',
                           'httpx>=0.15.4,<0.25.0',
                           'attrs>=21.3.0',
```


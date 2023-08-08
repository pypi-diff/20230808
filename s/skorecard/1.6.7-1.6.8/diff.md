# Comparing `tmp/skorecard-1.6.7.tar.gz` & `tmp/skorecard-1.6.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "skorecard-1.6.7.tar", last modified: Mon Jun 19 07:44:08 2023, max compression
+gzip compressed data, was "skorecard-1.6.8.tar", last modified: Tue Aug  8 12:26:43 2023, max compression
```

## Comparing `skorecard-1.6.7.tar` & `skorecard-1.6.8.tar`

### file list

```diff
@@ -1,87 +1,87 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 07:44:08.873167 skorecard-1.6.7/
--rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-06-19 07:39:06.000000 skorecard-1.6.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-06-19 07:39:06.000000 skorecard-1.6.7/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     5995 2023-06-19 07:44:08.873167 skorecard-1.6.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3787 2023-06-19 07:39:06.000000 skorecard-1.6.7/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     3642 2023-06-19 07:39:06.000000 skorecard-1.6.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-19 07:44:08.873167 skorecard-1.6.7/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 07:44:08.853166 skorecard-1.6.7/skorecard/
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-06-19 07:39:06.000000 skorecard-1.6.7/skorecard/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 07:44:08.857166 skorecard-1.6.7/skorecard/apps/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-19 07:39:06.000000 skorecard-1.6.7/skorecard/apps/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14499 2023-06-19 07:39:06.000000 skorecard-1.6.7/skorecard/apps/app_callbacks.py
--rw-r--r--   0 runner    (1001) docker     (123)    16449 2023-06-19 07:39:06.000000 skorecard-1.6.7/skorecard/apps/app_layout.py
--rw-r--r--   0 runner    (1001) docker     (123)     5316 2023-06-19 07:39:06.000000 skorecard-1.6.7/skorecard/apps/app_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 07:44:08.857166 skorecard-1.6.7/skorecard/apps/assets/
--rw-r--r--   0 runner    (1001) docker     (123)   181482 2023-06-19 07:39:06.000000 skorecard-1.6.7/skorecard/apps/assets/united-bootstrap.min.css
--rw-r--r--   0 runner    (1001) docker     (123)    17053 2023-06-19 07:39:06.000000 skorecard-1.6.7/skorecard/bucket_mapping.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 07:44:08.861166 skorecard-1.6.7/skorecard/bucketers/
--rw-r--r--   0 runner    (1001) docker     (123)      592 2023-06-19 07:39:06.000000 skorecard-1.6.7/skorecard/bucketers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17027 2023-06-19 07:39:06.000000 skorecard-1.6.7/skorecard/bucketers/base_bucketer.py
--rw-r--r--   0 runner    (1001) docker     (123)    55337 2023-06-19 07:39:06.000000 skorecard-1.6.7/skorecard/bucketers/bucketers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 07:44:08.861166 skorecard-1.6.7/skorecard/data/
--rw-r--r--   0 runner    (1001) docker     (123)    31668 2023-06-19 07:39:06.000000 skorecard-1.6.7/skorecard/data/UCI_Credit_Card.zip
--rw-r--r--   0 runner    (1001) docker     (123)     3184 2023-06-19 07:39:06.000000 skorecard-1.6.7/skorecard/datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)     5251 2023-06-19 07:39:06.000000 skorecard-1.6.7/skorecard/features_bucket_mapping.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 07:44:08.861166 skorecard-1.6.7/skorecard/linear_model/
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-06-19 07:39:06.000000 skorecard-1.6.7/skorecard/linear_model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8415 2023-06-19 07:39:06.000000 skorecard-1.6.7/skorecard/linear_model/linear_model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 07:44:08.861166 skorecard-1.6.7/skorecard/metrics/
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-06-19 07:39:06.000000 skorecard-1.6.7/skorecard/metrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3413 2023-06-19 07:39:06.000000 skorecard-1.6.7/skorecard/metrics/metrics.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 07:44:08.865167 skorecard-1.6.7/skorecard/pipeline/
--rw-r--r--   0 runner    (1001) docker     (123)      372 2023-06-19 07:39:06.000000 skorecard-1.6.7/skorecard/pipeline/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18468 2023-06-19 07:39:06.000000 skorecard-1.6.7/skorecard/pipeline/bucketing_process.py
--rw-r--r--   0 runner    (1001) docker     (123)    16658 2023-06-19 07:39:06.000000 skorecard-1.6.7/skorecard/pipeline/pipeline.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 07:44:08.865167 skorecard-1.6.7/skorecard/preprocessing/
--rw-r--r--   0 runner    (1001) docker     (123)     5927 2023-06-19 07:39:06.000000 skorecard-1.6.7/skorecard/preprocessing/_WoEEncoder.py
--rw-r--r--   0 runner    (1001) docker     (123)      122 2023-06-19 07:39:06.000000 skorecard-1.6.7/skorecard/preprocessing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2217 2023-06-19 07:39:06.000000 skorecard-1.6.7/skorecard/preprocessing/preprocessing.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 07:44:08.865167 skorecard-1.6.7/skorecard/reporting/
--rw-r--r--   0 runner    (1001) docker     (123)      221 2023-06-19 07:39:06.000000 skorecard-1.6.7/skorecard/reporting/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11196 2023-06-19 07:39:06.000000 skorecard-1.6.7/skorecard/reporting/plotting.py
--rw-r--r--   0 runner    (1001) docker     (123)    12814 2023-06-19 07:39:06.000000 skorecard-1.6.7/skorecard/reporting/report.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 07:44:08.865167 skorecard-1.6.7/skorecard/rescale/
--rw-r--r--   0 runner    (1001) docker     (123)      125 2023-06-19 07:39:06.000000 skorecard-1.6.7/skorecard/rescale/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7568 2023-06-19 07:39:06.000000 skorecard-1.6.7/skorecard/rescale/rescale.py
--rw-r--r--   0 runner    (1001) docker     (123)    15835 2023-06-19 07:39:06.000000 skorecard-1.6.7/skorecard/skorecard.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 07:44:08.865167 skorecard-1.6.7/skorecard/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      642 2023-06-19 07:39:06.000000 skorecard-1.6.7/skorecard/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1253 2023-06-19 07:39:06.000000 skorecard-1.6.7/skorecard/utils/arrayfuncs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1050 2023-06-19 07:39:06.000000 skorecard-1.6.7/skorecard/utils/dataframe.py
--rw-r--r--   0 runner    (1001) docker     (123)     4343 2023-06-19 07:39:06.000000 skorecard-1.6.7/skorecard/utils/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2445 2023-06-19 07:39:06.000000 skorecard-1.6.7/skorecard/utils/validation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 07:44:08.857166 skorecard-1.6.7/skorecard.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5995 2023-06-19 07:44:08.000000 skorecard-1.6.7/skorecard.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2131 2023-06-19 07:44:08.000000 skorecard-1.6.7/skorecard.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-19 07:44:08.000000 skorecard-1.6.7/skorecard.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      559 2023-06-19 07:44:08.000000 skorecard-1.6.7/skorecard.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-06-19 07:44:08.000000 skorecard-1.6.7/skorecard.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 07:44:08.873167 skorecard-1.6.7/tests/
--rw-r--r--   0 runner    (1001) docker     (123)    10724 2023-06-19 07:39:06.000000 skorecard-1.6.7/tests/test_Skorecard_class.py
--rw-r--r--   0 runner    (1001) docker     (123)    22184 2023-06-19 07:39:06.000000 skorecard-1.6.7/tests/test_bucket_mapping.py
--rw-r--r--   0 runner    (1001) docker     (123)      723 2023-06-19 07:39:06.000000 skorecard-1.6.7/tests/test_bucket_table_woe_values.py
--rw-r--r--   0 runner    (1001) docker     (123)     1229 2023-06-19 07:39:06.000000 skorecard-1.6.7/tests/test_bucketer_AsIsCategoricalBucketer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1146 2023-06-19 07:39:06.000000 skorecard-1.6.7/tests/test_bucketer_AsIsNumericalBucketer.py
--rw-r--r--   0 runner    (1001) docker     (123)     4148 2023-06-19 07:39:06.000000 skorecard-1.6.7/tests/test_bucketer_DecisionTreeBucketer.py
--rw-r--r--   0 runner    (1001) docker     (123)     8492 2023-06-19 07:39:06.000000 skorecard-1.6.7/tests/test_bucketer_OptimalBucketer.py
--rw-r--r--   0 runner    (1001) docker     (123)     4907 2023-06-19 07:39:06.000000 skorecard-1.6.7/tests/test_bucketer_OrdinalCategoricalBucketer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2258 2023-06-19 07:39:06.000000 skorecard-1.6.7/tests/test_bucketer_UserInputBucketer.py
--rw-r--r--   0 runner    (1001) docker     (123)     4798 2023-06-19 07:39:06.000000 skorecard-1.6.7/tests/test_bucketer_WoEBucketer.py
--rw-r--r--   0 runner    (1001) docker     (123)    14941 2023-06-19 07:39:06.000000 skorecard-1.6.7/tests/test_bucketers.py
--rw-r--r--   0 runner    (1001) docker     (123)    14751 2023-06-19 07:39:06.000000 skorecard-1.6.7/tests/test_bucketing_process.py
--rw-r--r--   0 runner    (1001) docker     (123)     1660 2023-06-19 07:39:06.000000 skorecard-1.6.7/tests/test_column_selector.py
--rw-r--r--   0 runner    (1001) docker     (123)     1020 2023-06-19 07:39:06.000000 skorecard-1.6.7/tests/test_datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)     2394 2023-06-19 07:39:06.000000 skorecard-1.6.7/tests/test_docstring.py
--rw-r--r--   0 runner    (1001) docker     (123)     7260 2023-06-19 07:39:06.000000 skorecard-1.6.7/tests/test_io.py
--rw-r--r--   0 runner    (1001) docker     (123)     2802 2023-06-19 07:39:06.000000 skorecard-1.6.7/tests/test_linear_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1577 2023-06-19 07:39:06.000000 skorecard-1.6.7/tests/test_manual_bucketer_app.py
--rw-r--r--   0 runner    (1001) docker     (123)     2190 2023-06-19 07:39:06.000000 skorecard-1.6.7/tests/test_metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)    10081 2023-06-19 07:39:06.000000 skorecard-1.6.7/tests/test_pipelines.py
--rw-r--r--   0 runner    (1001) docker     (123)     2286 2023-06-19 07:39:06.000000 skorecard-1.6.7/tests/test_reports.py
--rw-r--r--   0 runner    (1001) docker     (123)     2535 2023-06-19 07:39:06.000000 skorecard-1.6.7/tests/test_rescale.py
--rw-r--r--   0 runner    (1001) docker     (123)     7504 2023-06-19 07:39:06.000000 skorecard-1.6.7/tests/test_sklearn_compat.py
--rw-r--r--   0 runner    (1001) docker     (123)     8171 2023-06-19 07:39:06.000000 skorecard-1.6.7/tests/test_specials_bucketers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1915 2023-06-19 07:39:06.000000 skorecard-1.6.7/tests/test_suppressor_warning.py
--rw-r--r--   0 runner    (1001) docker     (123)      782 2023-06-19 07:39:06.000000 skorecard-1.6.7/tests/test_usage_flows.py
--rw-r--r--   0 runner    (1001) docker     (123)      492 2023-06-19 07:39:06.000000 skorecard-1.6.7/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 12:26:43.447941 skorecard-1.6.8/
+-rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-08-08 12:22:59.000000 skorecard-1.6.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-08-08 12:22:59.000000 skorecard-1.6.8/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     6088 2023-08-08 12:26:43.447941 skorecard-1.6.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3787 2023-08-08 12:22:59.000000 skorecard-1.6.8/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3705 2023-08-08 12:22:59.000000 skorecard-1.6.8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-08 12:26:43.447941 skorecard-1.6.8/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 12:26:43.439941 skorecard-1.6.8/skorecard/
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-08-08 12:22:59.000000 skorecard-1.6.8/skorecard/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 12:26:43.443940 skorecard-1.6.8/skorecard/apps/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 12:22:59.000000 skorecard-1.6.8/skorecard/apps/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14499 2023-08-08 12:22:59.000000 skorecard-1.6.8/skorecard/apps/app_callbacks.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16449 2023-08-08 12:22:59.000000 skorecard-1.6.8/skorecard/apps/app_layout.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5316 2023-08-08 12:22:59.000000 skorecard-1.6.8/skorecard/apps/app_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 12:26:43.443940 skorecard-1.6.8/skorecard/apps/assets/
+-rw-r--r--   0 runner    (1001) docker     (123)   181482 2023-08-08 12:22:59.000000 skorecard-1.6.8/skorecard/apps/assets/united-bootstrap.min.css
+-rw-r--r--   0 runner    (1001) docker     (123)    17053 2023-08-08 12:22:59.000000 skorecard-1.6.8/skorecard/bucket_mapping.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 12:26:43.443940 skorecard-1.6.8/skorecard/bucketers/
+-rw-r--r--   0 runner    (1001) docker     (123)      592 2023-08-08 12:22:59.000000 skorecard-1.6.8/skorecard/bucketers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17027 2023-08-08 12:22:59.000000 skorecard-1.6.8/skorecard/bucketers/base_bucketer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    55337 2023-08-08 12:22:59.000000 skorecard-1.6.8/skorecard/bucketers/bucketers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 12:26:43.443940 skorecard-1.6.8/skorecard/data/
+-rw-r--r--   0 runner    (1001) docker     (123)    31668 2023-08-08 12:22:59.000000 skorecard-1.6.8/skorecard/data/UCI_Credit_Card.zip
+-rw-r--r--   0 runner    (1001) docker     (123)     3184 2023-08-08 12:22:59.000000 skorecard-1.6.8/skorecard/datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5251 2023-08-08 12:22:59.000000 skorecard-1.6.8/skorecard/features_bucket_mapping.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 12:26:43.443940 skorecard-1.6.8/skorecard/linear_model/
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-08-08 12:22:59.000000 skorecard-1.6.8/skorecard/linear_model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8415 2023-08-08 12:22:59.000000 skorecard-1.6.8/skorecard/linear_model/linear_model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 12:26:43.443940 skorecard-1.6.8/skorecard/metrics/
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-08-08 12:22:59.000000 skorecard-1.6.8/skorecard/metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3501 2023-08-08 12:22:59.000000 skorecard-1.6.8/skorecard/metrics/metrics.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 12:26:43.443940 skorecard-1.6.8/skorecard/pipeline/
+-rw-r--r--   0 runner    (1001) docker     (123)      372 2023-08-08 12:22:59.000000 skorecard-1.6.8/skorecard/pipeline/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18468 2023-08-08 12:22:59.000000 skorecard-1.6.8/skorecard/pipeline/bucketing_process.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16658 2023-08-08 12:22:59.000000 skorecard-1.6.8/skorecard/pipeline/pipeline.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 12:26:43.443940 skorecard-1.6.8/skorecard/preprocessing/
+-rw-r--r--   0 runner    (1001) docker     (123)     5927 2023-08-08 12:22:59.000000 skorecard-1.6.8/skorecard/preprocessing/_WoEEncoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2023-08-08 12:22:59.000000 skorecard-1.6.8/skorecard/preprocessing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2217 2023-08-08 12:22:59.000000 skorecard-1.6.8/skorecard/preprocessing/preprocessing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 12:26:43.443940 skorecard-1.6.8/skorecard/reporting/
+-rw-r--r--   0 runner    (1001) docker     (123)      221 2023-08-08 12:22:59.000000 skorecard-1.6.8/skorecard/reporting/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11196 2023-08-08 12:22:59.000000 skorecard-1.6.8/skorecard/reporting/plotting.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12819 2023-08-08 12:22:59.000000 skorecard-1.6.8/skorecard/reporting/report.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 12:26:43.443940 skorecard-1.6.8/skorecard/rescale/
+-rw-r--r--   0 runner    (1001) docker     (123)      125 2023-08-08 12:22:59.000000 skorecard-1.6.8/skorecard/rescale/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7582 2023-08-08 12:22:59.000000 skorecard-1.6.8/skorecard/rescale/rescale.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15835 2023-08-08 12:22:59.000000 skorecard-1.6.8/skorecard/skorecard.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 12:26:43.447941 skorecard-1.6.8/skorecard/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      642 2023-08-08 12:22:59.000000 skorecard-1.6.8/skorecard/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1253 2023-08-08 12:22:59.000000 skorecard-1.6.8/skorecard/utils/arrayfuncs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1050 2023-08-08 12:22:59.000000 skorecard-1.6.8/skorecard/utils/dataframe.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4343 2023-08-08 12:22:59.000000 skorecard-1.6.8/skorecard/utils/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2445 2023-08-08 12:22:59.000000 skorecard-1.6.8/skorecard/utils/validation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 12:26:43.443940 skorecard-1.6.8/skorecard.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6088 2023-08-08 12:26:43.000000 skorecard-1.6.8/skorecard.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2131 2023-08-08 12:26:43.000000 skorecard-1.6.8/skorecard.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 12:26:43.000000 skorecard-1.6.8/skorecard.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      640 2023-08-08 12:26:43.000000 skorecard-1.6.8/skorecard.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-08-08 12:26:43.000000 skorecard-1.6.8/skorecard.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 12:26:43.447941 skorecard-1.6.8/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    10724 2023-08-08 12:22:59.000000 skorecard-1.6.8/tests/test_Skorecard_class.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22184 2023-08-08 12:22:59.000000 skorecard-1.6.8/tests/test_bucket_mapping.py
+-rw-r--r--   0 runner    (1001) docker     (123)      818 2023-08-08 12:22:59.000000 skorecard-1.6.8/tests/test_bucket_table_woe_values.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1229 2023-08-08 12:22:59.000000 skorecard-1.6.8/tests/test_bucketer_AsIsCategoricalBucketer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1146 2023-08-08 12:22:59.000000 skorecard-1.6.8/tests/test_bucketer_AsIsNumericalBucketer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4148 2023-08-08 12:22:59.000000 skorecard-1.6.8/tests/test_bucketer_DecisionTreeBucketer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8492 2023-08-08 12:22:59.000000 skorecard-1.6.8/tests/test_bucketer_OptimalBucketer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4907 2023-08-08 12:22:59.000000 skorecard-1.6.8/tests/test_bucketer_OrdinalCategoricalBucketer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2258 2023-08-08 12:22:59.000000 skorecard-1.6.8/tests/test_bucketer_UserInputBucketer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4798 2023-08-08 12:22:59.000000 skorecard-1.6.8/tests/test_bucketer_WoEBucketer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14941 2023-08-08 12:22:59.000000 skorecard-1.6.8/tests/test_bucketers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14751 2023-08-08 12:22:59.000000 skorecard-1.6.8/tests/test_bucketing_process.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1660 2023-08-08 12:22:59.000000 skorecard-1.6.8/tests/test_column_selector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1020 2023-08-08 12:22:59.000000 skorecard-1.6.8/tests/test_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2394 2023-08-08 12:22:59.000000 skorecard-1.6.8/tests/test_docstring.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7260 2023-08-08 12:22:59.000000 skorecard-1.6.8/tests/test_io.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2802 2023-08-08 12:22:59.000000 skorecard-1.6.8/tests/test_linear_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1577 2023-08-08 12:22:59.000000 skorecard-1.6.8/tests/test_manual_bucketer_app.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2574 2023-08-08 12:22:59.000000 skorecard-1.6.8/tests/test_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10081 2023-08-08 12:22:59.000000 skorecard-1.6.8/tests/test_pipelines.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2286 2023-08-08 12:22:59.000000 skorecard-1.6.8/tests/test_reports.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2535 2023-08-08 12:22:59.000000 skorecard-1.6.8/tests/test_rescale.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7504 2023-08-08 12:22:59.000000 skorecard-1.6.8/tests/test_sklearn_compat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8171 2023-08-08 12:22:59.000000 skorecard-1.6.8/tests/test_specials_bucketers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1915 2023-08-08 12:22:59.000000 skorecard-1.6.8/tests/test_suppressor_warning.py
+-rw-r--r--   0 runner    (1001) docker     (123)      782 2023-08-08 12:22:59.000000 skorecard-1.6.8/tests/test_usage_flows.py
+-rw-r--r--   0 runner    (1001) docker     (123)      492 2023-08-08 12:22:59.000000 skorecard-1.6.8/tests/test_utils.py
```

### Comparing `skorecard-1.6.7/LICENSE` & `skorecard-1.6.8/LICENSE`

 * *Files identical despite different names*

### Comparing `skorecard-1.6.7/PKG-INFO` & `skorecard-1.6.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: skorecard
-Version: 1.6.7
+Version: 1.6.8
 Summary: Tools for building scorecard models in python, with a sklearn-compatible API
 Author-email: "ING Bank N.V." <anilkumar.panda@ing.com>
 License: The MIT License (MIT)
         
         Copyright (c) 2020 ING Bank NV
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
@@ -23,14 +23,18 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3 :: Only
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
+Provides-Extra: dashboard
+Provides-Extra: reporting
+Provides-Extra: dev
+Provides-Extra: docs
 Provides-Extra: all
 License-File: LICENSE
 
 <img src="https://github.com/ing-bank/skorecard/raw/main/docs/assets/img/skorecard_logo.svg" width="150" align="right">
 
 # skorecard
```

### Comparing `skorecard-1.6.7/README.md` & `skorecard-1.6.8/README.md`

 * *Files identical despite different names*

### Comparing `skorecard-1.6.7/pyproject.toml` & `skorecard-1.6.8/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "skorecard"
-version = "1.6.7"
+dynamic = ["version"]
 requires-python= ">=3.8"
 description = "Tools for building scorecard models in python, with a sklearn-compatible API"
 readme = { file = "README.md", content-type = "text/markdown" }
 authors = [
     { name = "ING Bank N.V.", email = "anilkumar.panda@ing.com" }
 ]
 license = { file = "LICENSE" }
@@ -36,47 +36,53 @@
 [project.urls]
 Homepage = "https://ing-bank.github.io/skorecard/"
 Documentation = "https://ing-bank.github.io/skorecard/api/bucketers/OptimalBucketer/"
 Repository = "https://github.com/ing-bank/skorecard.git"
 Changelog = "https://github.com/ing-bank/skorecard/blob/main/CHANGELOG.md"
 
 [project.optional-dependencies]
-all = [
-    # Dashboard dependencies
+dashboard = [
     "dash>=1.21.0",
     "jupyter-dash>=0.4.0",
     "dash_bootstrap_components>=0.13",
-    # Reporting dependencies
+]
+reporting = [
     "plotly>=4.14.3",
-    # Dev dependencies
+]
+dev = [
     "black>=19.10b0",
     "pre-commit>=2.5.0",
     "pytest>=6.0.0",
     "pytest-cov>=2.10.0",
     "pyflakes>=3.0.1",
     "isort>=5.12.0",
     "codespell>=2.2.4",
     "ruff>=0.0.272",
     "mypy>=0.770",
     # Mypy type stubs
     "types-PyYAML>=6.0.12.10",
     "types-six>=1.16.21.8",
     "types-decorator>=5.1.8.3",
-    # Doc dependencies
+]
+docs = [
     "mkdocs>=1.1.2",
     "mkdocs-material>=7.1",
     "mkdocstrings>=0.13.2",
     "mknotebooks>=0.7.0",
     "mkdocs-git-revision-date-localized-plugin>=0.7.2",
     "mkdocstrings-python>=1.1.2",
 ]
+all = ["skorecard[dashboard,reporting,dev,docs]"]
 
 [tool.setuptools.packages.find]
 exclude = ["tests", "notebooks", "docs"]
 
+[tool.setuptools.dynamic]
+version = {attr = "skorecard.__version__"}
+
 [tool.nbqa.addopts]
 # E402: Ignores imports not at the top of file for IPYNB since this makes copy-pasting easier.
 ruff = ["--fix", "--ignore=E402"]
 mypy = ["--install-types", "--non-interactive", "--ignore-missing-imports"]
 isort = ["--profile=black"]
 black = ["--line-length=120"]
```

### Comparing `skorecard-1.6.7/skorecard/apps/app_callbacks.py` & `skorecard-1.6.8/skorecard/apps/app_callbacks.py`

 * *Files identical despite different names*

### Comparing `skorecard-1.6.7/skorecard/apps/app_layout.py` & `skorecard-1.6.8/skorecard/apps/app_layout.py`

 * *Files identical despite different names*

### Comparing `skorecard-1.6.7/skorecard/apps/app_utils.py` & `skorecard-1.6.8/skorecard/apps/app_utils.py`

 * *Files identical despite different names*

### Comparing `skorecard-1.6.7/skorecard/apps/assets/united-bootstrap.min.css` & `skorecard-1.6.8/skorecard/apps/assets/united-bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `skorecard-1.6.7/skorecard/bucket_mapping.py` & `skorecard-1.6.8/skorecard/bucket_mapping.py`

 * *Files identical despite different names*

### Comparing `skorecard-1.6.7/skorecard/bucketers/__init__.py` & `skorecard-1.6.8/skorecard/bucketers/__init__.py`

 * *Files identical despite different names*

### Comparing `skorecard-1.6.7/skorecard/bucketers/base_bucketer.py` & `skorecard-1.6.8/skorecard/bucketers/base_bucketer.py`

 * *Files identical despite different names*

### Comparing `skorecard-1.6.7/skorecard/bucketers/bucketers.py` & `skorecard-1.6.8/skorecard/bucketers/bucketers.py`

 * *Files identical despite different names*

### Comparing `skorecard-1.6.7/skorecard/data/UCI_Credit_Card.zip` & `skorecard-1.6.8/skorecard/data/UCI_Credit_Card.zip`

 * *Files identical despite different names*

### Comparing `skorecard-1.6.7/skorecard/datasets.py` & `skorecard-1.6.8/skorecard/datasets.py`

 * *Files identical despite different names*

### Comparing `skorecard-1.6.7/skorecard/features_bucket_mapping.py` & `skorecard-1.6.8/skorecard/features_bucket_mapping.py`

 * *Files identical despite different names*

### Comparing `skorecard-1.6.7/skorecard/linear_model/linear_model.py` & `skorecard-1.6.8/skorecard/linear_model/linear_model.py`

 * *Files identical despite different names*

### Comparing `skorecard-1.6.7/skorecard/metrics/metrics.py` & `skorecard-1.6.8/skorecard/metrics/metrics.py`

 * *Files 7% similar despite different names*

```diff
@@ -14,22 +14,26 @@
 
     Returns: (dictionary)
         - bins: indices of unique values of X
         - woe_values: calculated weight of evidence for every unique bin
         - counts_0: count of entries per bin where y==0
         - counts_1: count of entries per bin where y==1
     """
-    X = X.copy().reset_index(drop=True)
+    # Make sure y has the right number of rows.
+    if y.shape[0] != X.shape[0]:
+        raise ValueError(f"y has {y.shape[0]}, but expected {X.shape[0]}")
+
+    # Make sure y is a pd.Series so we can reset its index.
     if not isinstance(y, pd.Series):
-        if y.shape[0] == X.shape[0]:
-            y = pd.Series(y).reset_index(drop=True)
-        else:
-            raise ValueError(f"y has {y.shape[0]}, but expected {X.shape[0]}")
+        y = pd.Series(y)
+
+    X = X.reset_index(drop=True)
+    y = y.reset_index(drop=True)
 
-    # Ensure classes in y start at zero
+    # Ensure classes in y start at zero.
     y = y - min(y)
 
     df = pd.concat([X, y], axis=1, ignore_index=True)
     df.columns = ["feat", "target"]
 
     total_pos = df["target"].sum()
     total_neg = df.shape[0] - total_pos
```

### Comparing `skorecard-1.6.7/skorecard/pipeline/bucketing_process.py` & `skorecard-1.6.8/skorecard/pipeline/bucketing_process.py`

 * *Files identical despite different names*

### Comparing `skorecard-1.6.7/skorecard/pipeline/pipeline.py` & `skorecard-1.6.8/skorecard/pipeline/pipeline.py`

 * *Files identical despite different names*

### Comparing `skorecard-1.6.7/skorecard/preprocessing/_WoEEncoder.py` & `skorecard-1.6.8/skorecard/preprocessing/_WoEEncoder.py`

 * *Files identical despite different names*

### Comparing `skorecard-1.6.7/skorecard/preprocessing/preprocessing.py` & `skorecard-1.6.8/skorecard/preprocessing/preprocessing.py`

 * *Files identical despite different names*

### Comparing `skorecard-1.6.7/skorecard/reporting/plotting.py` & `skorecard-1.6.8/skorecard/reporting/plotting.py`

 * *Files identical despite different names*

### Comparing `skorecard-1.6.7/skorecard/reporting/report.py` & `skorecard-1.6.8/skorecard/reporting/report.py`

 * *Files 1% similar despite different names*

```diff
@@ -123,15 +123,15 @@
     stats["% Non-event"] = stats["Non-event"] / stats["Non-event"].sum()
 
     event_percentage = (stats["Event"] + epsilon) / (stats["Event"].sum() + 2 * epsilon)
     non_event_percentage = (stats["Non-event"] + epsilon) / (stats["Non-event"].sum() + 2 * epsilon)
     stats["WoE"] = (event_percentage / non_event_percentage).apply(lambda x: np.log(x))
     stats.loc[stats["Count"] == 0, "WoE"] = np.nan
 
-    stats["IV"] = (stats["% Non-event"] - stats["% Event"]) * stats["WoE"]
+    stats["IV"] = abs((stats["% Non-event"] - stats["% Event"]) * stats["WoE"])
 
     stats["% Event"] = np.round(100 * stats["% Event"], 2)
     stats["% Non-event"] = np.round(100 * stats["% Non-event"], 2)
     stats["Event Rate"] = np.round(stats["Event Rate"], 3)
 
     stats["WoE"] = np.round(stats["WoE"], 3)
     stats["IV"] = np.round(stats["IV"], 3)
```

### Comparing `skorecard-1.6.7/skorecard/rescale/rescale.py` & `skorecard-1.6.8/skorecard/rescale/rescale.py`

 * *Files 0% similar despite different names*

```diff
@@ -140,20 +140,21 @@
             list_dfs.append(df_)
 
         # Reduce the list of tables, to build the final scorecard feature points
         scorecard = reduce(lambda x, y: pd.concat([x, y]), list_dfs)
         scorecard = pd.concat(
             [
                 scorecard,
-                pd.DataFrame(
+                pd.DataFrame.from_records(
                     [{"feature": "Intercept", "coef": self.model.intercept_[0], "bin_index": 0, "map": 0, "woe": 0}]
                 ),
             ],
             ignore_index=True,
         )
+
         #     return buckets, woes
         scorecard["contribution"] = scorecard["woe"] * scorecard["coef"]
 
         self.scorecard = _scale_scorecard(
             scorecard, pdo=self.pdo, ref_score=self.ref_score, ref_odds=self.ref_odds, features=self.features
         )
```

### Comparing `skorecard-1.6.7/skorecard/skorecard.py` & `skorecard-1.6.8/skorecard/skorecard.py`

 * *Files identical despite different names*

### Comparing `skorecard-1.6.7/skorecard/utils/__init__.py` & `skorecard-1.6.8/skorecard/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `skorecard-1.6.7/skorecard/utils/arrayfuncs.py` & `skorecard-1.6.8/skorecard/utils/arrayfuncs.py`

 * *Files identical despite different names*

### Comparing `skorecard-1.6.7/skorecard/utils/dataframe.py` & `skorecard-1.6.8/skorecard/utils/dataframe.py`

 * *Files identical despite different names*

### Comparing `skorecard-1.6.7/skorecard/utils/exceptions.py` & `skorecard-1.6.8/skorecard/utils/exceptions.py`

 * *Files identical despite different names*

### Comparing `skorecard-1.6.7/skorecard/utils/validation.py` & `skorecard-1.6.8/skorecard/utils/validation.py`

 * *Files identical despite different names*

### Comparing `skorecard-1.6.7/skorecard.egg-info/PKG-INFO` & `skorecard-1.6.8/skorecard.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: skorecard
-Version: 1.6.7
+Version: 1.6.8
 Summary: Tools for building scorecard models in python, with a sklearn-compatible API
 Author-email: "ING Bank N.V." <anilkumar.panda@ing.com>
 License: The MIT License (MIT)
         
         Copyright (c) 2020 ING Bank NV
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
@@ -23,14 +23,18 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3 :: Only
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
+Provides-Extra: dashboard
+Provides-Extra: reporting
+Provides-Extra: dev
+Provides-Extra: docs
 Provides-Extra: all
 License-File: LICENSE
 
 <img src="https://github.com/ing-bank/skorecard/raw/main/docs/assets/img/skorecard_logo.svg" width="150" align="right">
 
 # skorecard
```

### Comparing `skorecard-1.6.7/skorecard.egg-info/SOURCES.txt` & `skorecard-1.6.8/skorecard.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `skorecard-1.6.7/skorecard.egg-info/requires.txt` & `skorecard-1.6.8/skorecard.egg-info/requires.txt`

 * *Files 13% similar despite different names*

```diff
@@ -3,29 +3,38 @@
 pandas>=1.5.3
 scikit-learn>=0.23.2
 pyyaml
 category_encoders>=2.2.2
 optbinning>=0.8.0
 
 [all]
+skorecard[dashboard,dev,docs,reporting]
+
+[dashboard]
 dash>=1.21.0
 jupyter-dash>=0.4.0
 dash_bootstrap_components>=0.13
-plotly>=4.14.3
+
+[dev]
 black>=19.10b0
 pre-commit>=2.5.0
 pytest>=6.0.0
 pytest-cov>=2.10.0
 pyflakes>=3.0.1
 isort>=5.12.0
 codespell>=2.2.4
 ruff>=0.0.272
 mypy>=0.770
 types-PyYAML>=6.0.12.10
 types-six>=1.16.21.8
 types-decorator>=5.1.8.3
+
+[docs]
 mkdocs>=1.1.2
 mkdocs-material>=7.1
 mkdocstrings>=0.13.2
 mknotebooks>=0.7.0
 mkdocs-git-revision-date-localized-plugin>=0.7.2
 mkdocstrings-python>=1.1.2
+
+[reporting]
+plotly>=4.14.3
```

### Comparing `skorecard-1.6.7/tests/test_Skorecard_class.py` & `skorecard-1.6.8/tests/test_Skorecard_class.py`

 * *Files identical despite different names*

### Comparing `skorecard-1.6.7/tests/test_bucket_mapping.py` & `skorecard-1.6.8/tests/test_bucket_mapping.py`

 * *Files identical despite different names*

### Comparing `skorecard-1.6.7/tests/test_bucket_table_woe_values.py` & `skorecard-1.6.8/tests/test_bucket_table_woe_values.py`

 * *Files 16% similar despite different names*

```diff
@@ -16,7 +16,9 @@
     X_woe = model.woe_transform(X)
     for c in X.columns:
         bucket_table = model.bucket_table(c)
         b_tab_woes = set(bucket_table["WoE"])
         b_tab_woes = {x for x in b_tab_woes if pd.notna(x)}
         data_woes = set(np.round(X_woe[c].value_counts().index, 3))
         assert b_tab_woes == data_woes
+        iv_lt_zero = [x < 0 for x in bucket_table["IV"]]
+        assert True not in iv_lt_zero
```

### Comparing `skorecard-1.6.7/tests/test_bucketer_AsIsCategoricalBucketer.py` & `skorecard-1.6.8/tests/test_bucketer_AsIsCategoricalBucketer.py`

 * *Files identical despite different names*

### Comparing `skorecard-1.6.7/tests/test_bucketer_AsIsNumericalBucketer.py` & `skorecard-1.6.8/tests/test_bucketer_AsIsNumericalBucketer.py`

 * *Files identical despite different names*

### Comparing `skorecard-1.6.7/tests/test_bucketer_DecisionTreeBucketer.py` & `skorecard-1.6.8/tests/test_bucketer_DecisionTreeBucketer.py`

 * *Files identical despite different names*

### Comparing `skorecard-1.6.7/tests/test_bucketer_OptimalBucketer.py` & `skorecard-1.6.8/tests/test_bucketer_OptimalBucketer.py`

 * *Files identical despite different names*

### Comparing `skorecard-1.6.7/tests/test_bucketer_OrdinalCategoricalBucketer.py` & `skorecard-1.6.8/tests/test_bucketer_OrdinalCategoricalBucketer.py`

 * *Files identical despite different names*

### Comparing `skorecard-1.6.7/tests/test_bucketer_UserInputBucketer.py` & `skorecard-1.6.8/tests/test_bucketer_UserInputBucketer.py`

 * *Files identical despite different names*

### Comparing `skorecard-1.6.7/tests/test_bucketer_WoEBucketer.py` & `skorecard-1.6.8/tests/test_bucketer_WoEBucketer.py`

 * *Files identical despite different names*

### Comparing `skorecard-1.6.7/tests/test_bucketers.py` & `skorecard-1.6.8/tests/test_bucketers.py`

 * *Files identical despite different names*

### Comparing `skorecard-1.6.7/tests/test_bucketing_process.py` & `skorecard-1.6.8/tests/test_bucketing_process.py`

 * *Files identical despite different names*

### Comparing `skorecard-1.6.7/tests/test_column_selector.py` & `skorecard-1.6.8/tests/test_column_selector.py`

 * *Files identical despite different names*

### Comparing `skorecard-1.6.7/tests/test_datasets.py` & `skorecard-1.6.8/tests/test_datasets.py`

 * *Files identical despite different names*

### Comparing `skorecard-1.6.7/tests/test_docstring.py` & `skorecard-1.6.8/tests/test_docstring.py`

 * *Files identical despite different names*

### Comparing `skorecard-1.6.7/tests/test_io.py` & `skorecard-1.6.8/tests/test_io.py`

 * *Files identical despite different names*

### Comparing `skorecard-1.6.7/tests/test_linear_model.py` & `skorecard-1.6.8/tests/test_linear_model.py`

 * *Files identical despite different names*

### Comparing `skorecard-1.6.7/tests/test_manual_bucketer_app.py` & `skorecard-1.6.8/tests/test_manual_bucketer_app.py`

 * *Files identical despite different names*

### Comparing `skorecard-1.6.7/tests/test_metrics.py` & `skorecard-1.6.8/tests/test_metrics.py`

 * *Files 8% similar despite different names*

```diff
@@ -64,12 +64,18 @@
 
     np.testing.assert_array_almost_equal(pd.Series(expected_psi).values, pd.Series(psi_vals).values, decimal=2)
 
 
 def test_IV_values(X_y):
     """Assert IV values match expectations."""
     X, y = X_y
-    X = pd.DataFrame(X, columns=["col1", "col2"])
+    random_index = [2 * x for x in range(0, len(y))]
+    X = pd.DataFrame(X, columns=["col1", "col2"], index=random_index)
     expected_iv = {"col1": 5.307, "col2": 4.635}
     iv_vals = skorecard.reporting.report.iv(X, y)
+    np.testing.assert_array_almost_equal(pd.Series(expected_iv).values, pd.Series(iv_vals).values, decimal=2)
 
+    # Make sure these are still accurate if y is a pd.Series with the same
+    # non-continuous indices as X.
+    y = pd.Series(y, index=random_index)
+    iv_vals = skorecard.reporting.report.iv(X, y)
     np.testing.assert_array_almost_equal(pd.Series(expected_iv).values, pd.Series(iv_vals).values, decimal=2)
```

### Comparing `skorecard-1.6.7/tests/test_pipelines.py` & `skorecard-1.6.8/tests/test_pipelines.py`

 * *Files identical despite different names*

### Comparing `skorecard-1.6.7/tests/test_reports.py` & `skorecard-1.6.8/tests/test_reports.py`

 * *Files identical despite different names*

### Comparing `skorecard-1.6.7/tests/test_rescale.py` & `skorecard-1.6.8/tests/test_rescale.py`

 * *Files identical despite different names*

### Comparing `skorecard-1.6.7/tests/test_sklearn_compat.py` & `skorecard-1.6.8/tests/test_sklearn_compat.py`

 * *Files identical despite different names*

### Comparing `skorecard-1.6.7/tests/test_specials_bucketers.py` & `skorecard-1.6.8/tests/test_specials_bucketers.py`

 * *Files identical despite different names*

### Comparing `skorecard-1.6.7/tests/test_suppressor_warning.py` & `skorecard-1.6.8/tests/test_suppressor_warning.py`

 * *Files identical despite different names*

### Comparing `skorecard-1.6.7/tests/test_usage_flows.py` & `skorecard-1.6.8/tests/test_usage_flows.py`

 * *Files identical despite different names*


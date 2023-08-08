# Comparing `tmp/trubrics-1.4.3.tar.gz` & `tmp/trubrics-1.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trubrics-1.4.3.tar", last modified: Mon Jul 17 11:10:39 2023, max compression
+gzip compressed data, was "trubrics-1.4.4.tar", last modified: Tue Aug  8 07:04:32 2023, max compression
```

## Comparing `trubrics-1.4.3.tar` & `trubrics-1.4.4.tar`

### file list

```diff
@@ -1,77 +1,78 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 11:10:39.143630 trubrics-1.4.3/
--rw-r--r--   0 runner    (1001) docker     (123)    11409 2023-07-17 11:10:24.000000 trubrics-1.4.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      327 2023-07-17 11:10:39.143630 trubrics-1.4.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3324 2023-07-17 11:10:24.000000 trubrics-1.4.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 11:10:39.139630 trubrics-1.4.3/examples/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 11:10:24.000000 trubrics-1.4.3/examples/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 11:10:39.139630 trubrics-1.4.3/examples/feedback/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 11:10:24.000000 trubrics-1.4.3/examples/feedback/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 11:10:39.139630 trubrics-1.4.3/examples/feedback/streamlit/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 11:10:24.000000 trubrics-1.4.3/examples/feedback/streamlit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1791 2023-07-17 11:10:24.000000 trubrics-1.4.3/examples/feedback/streamlit/llm_app.py
--rw-r--r--   0 runner    (1001) docker     (123)     2317 2023-07-17 11:10:24.000000 trubrics-1.4.3/examples/feedback/streamlit/titanic_app.py
--rw-r--r--   0 runner    (1001) docker     (123)     1267 2023-07-17 11:10:24.000000 trubrics-1.4.3/examples/feedback/streamlit/trubrics_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      248 2023-07-17 11:10:24.000000 trubrics-1.4.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-07-17 11:10:24.000000 trubrics-1.4.3/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      885 2023-07-17 11:10:39.143630 trubrics-1.4.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 11:10:39.139630 trubrics-1.4.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2035 2023-07-17 11:10:24.000000 trubrics-1.4.3/tests/test_context.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 11:10:39.139630 trubrics-1.4.3/trubrics/
--rw-r--r--   0 runner    (1001) docker     (123)      388 2023-07-17 11:10:24.000000 trubrics-1.4.3/trubrics/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 11:10:39.139630 trubrics-1.4.3/trubrics/cli/
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-07-17 11:10:24.000000 trubrics-1.4.3/trubrics/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2551 2023-07-17 11:10:24.000000 trubrics-1.4.3/trubrics/cli/main.py
--rw-r--r--   0 runner    (1001) docker     (123)      930 2023-07-17 11:10:24.000000 trubrics-1.4.3/trubrics/cli/run.py
--rw-r--r--   0 runner    (1001) docker     (123)     8454 2023-07-17 11:10:24.000000 trubrics-1.4.3/trubrics/context.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 11:10:39.139630 trubrics-1.4.3/trubrics/example/
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-07-17 11:10:24.000000 trubrics-1.4.3/trubrics/example/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3926 2023-07-17 11:10:24.000000 trubrics-1.4.3/trubrics/example/my_first_trubric.json
--rw-r--r--   0 runner    (1001) docker     (123)     2226 2023-07-17 11:10:24.000000 trubrics-1.4.3/trubrics/example/titanic.py
--rw-r--r--   0 runner    (1001) docker     (123)      354 2023-07-17 11:10:24.000000 trubrics-1.4.3/trubrics/example/titanic_config.py
--rw-r--r--   0 runner    (1001) docker     (123)    61194 2023-07-17 11:10:24.000000 trubrics-1.4.3/trubrics/example/titanic_data.csv
--rw-r--r--   0 runner    (1001) docker     (123)     1004 2023-07-17 11:10:24.000000 trubrics-1.4.3/trubrics/example/trubric_run.py
--rw-r--r--   0 runner    (1001) docker     (123)     1272 2023-07-17 11:10:24.000000 trubrics-1.4.3/trubrics/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 11:10:39.139630 trubrics-1.4.3/trubrics/feedback/
--rw-r--r--   0 runner    (1001) docker     (123)      157 2023-07-17 11:10:24.000000 trubrics-1.4.3/trubrics/feedback/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      644 2023-07-17 11:10:24.000000 trubrics-1.4.3/trubrics/feedback/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1450 2023-07-17 11:10:24.000000 trubrics-1.4.3/trubrics/feedback/dataclass.py
--rw-r--r--   0 runner    (1001) docker     (123)     1339 2023-07-17 11:10:24.000000 trubrics-1.4.3/trubrics/feedback/save_to_trubrics.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 11:10:39.139630 trubrics-1.4.3/trubrics/integrations/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 11:10:24.000000 trubrics-1.4.3/trubrics/integrations/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 11:10:39.139630 trubrics-1.4.3/trubrics/integrations/dash/
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-07-17 11:10:24.000000 trubrics-1.4.3/trubrics/integrations/dash/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3141 2023-07-17 11:10:24.000000 trubrics-1.4.3/trubrics/integrations/dash/collect.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 11:10:39.139630 trubrics-1.4.3/trubrics/integrations/gradio/
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-07-17 11:10:24.000000 trubrics-1.4.3/trubrics/integrations/gradio/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2523 2023-07-17 11:10:24.000000 trubrics-1.4.3/trubrics/integrations/gradio/collect.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 11:10:39.143630 trubrics-1.4.3/trubrics/integrations/mlflow/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 11:10:24.000000 trubrics-1.4.3/trubrics/integrations/mlflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2902 2023-07-17 11:10:24.000000 trubrics-1.4.3/trubrics/integrations/mlflow/trubrics_validator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 11:10:39.143630 trubrics-1.4.3/trubrics/integrations/streamlit/
--rw-r--r--   0 runner    (1001) docker     (123)      289 2023-07-17 11:10:24.000000 trubrics-1.4.3/trubrics/integrations/streamlit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14110 2023-07-17 11:10:24.000000 trubrics-1.4.3/trubrics/integrations/streamlit/collect.py
--rw-r--r--   0 runner    (1001) docker     (123)     2638 2023-07-17 11:10:24.000000 trubrics-1.4.3/trubrics/integrations/streamlit/experiment.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 11:10:24.000000 trubrics-1.4.3/trubrics/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 11:10:39.143630 trubrics-1.4.3/trubrics/trubrics_platform/
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-07-17 11:10:24.000000 trubrics-1.4.3/trubrics/trubrics_platform/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4295 2023-07-17 11:10:24.000000 trubrics-1.4.3/trubrics/trubrics_platform/auth.py
--rw-r--r--   0 runner    (1001) docker     (123)     5145 2023-07-17 11:10:24.000000 trubrics-1.4.3/trubrics/trubrics_platform/firestore.py
--rw-r--r--   0 runner    (1001) docker     (123)     1157 2023-07-17 11:10:24.000000 trubrics-1.4.3/trubrics/trubrics_platform/trubrics_config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 11:10:39.143630 trubrics-1.4.3/trubrics/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 11:10:24.000000 trubrics-1.4.3/trubrics/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      130 2023-07-17 11:10:24.000000 trubrics-1.4.3/trubrics/utils/pandas.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 11:10:39.143630 trubrics-1.4.3/trubrics/validations/
--rw-r--r--   0 runner    (1001) docker     (123)      172 2023-07-17 11:10:24.000000 trubrics-1.4.3/trubrics/validations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7281 2023-07-17 11:10:24.000000 trubrics-1.4.3/trubrics/validations/dataclass.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 11:10:39.143630 trubrics-1.4.3/trubrics/validations/model/
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-07-17 11:10:24.000000 trubrics-1.4.3/trubrics/validations/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    30069 2023-07-17 11:10:24.000000 trubrics-1.4.3/trubrics/validations/model/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     4765 2023-07-17 11:10:24.000000 trubrics-1.4.3/trubrics/validations/run.py
--rw-r--r--   0 runner    (1001) docker     (123)     2900 2023-07-17 11:10:24.000000 trubrics-1.4.3/trubrics/validations/validation_output.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 11:10:39.139630 trubrics-1.4.3/trubrics.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      327 2023-07-17 11:10:39.000000 trubrics-1.4.3/trubrics.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1806 2023-07-17 11:10:39.000000 trubrics-1.4.3/trubrics.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-17 11:10:39.000000 trubrics-1.4.3/trubrics.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      154 2023-07-17 11:10:39.000000 trubrics-1.4.3/trubrics.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      323 2023-07-17 11:10:39.000000 trubrics-1.4.3/trubrics.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-17 11:10:39.000000 trubrics-1.4.3/trubrics.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 07:04:32.903565 trubrics-1.4.4/
+-rw-r--r--   0 runner    (1001) docker     (123)    11409 2023-08-08 07:04:21.000000 trubrics-1.4.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      327 2023-08-08 07:04:32.903565 trubrics-1.4.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3671 2023-08-08 07:04:21.000000 trubrics-1.4.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 07:04:32.899565 trubrics-1.4.4/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 07:04:21.000000 trubrics-1.4.4/examples/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 07:04:32.899565 trubrics-1.4.4/examples/feedback/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 07:04:21.000000 trubrics-1.4.4/examples/feedback/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 07:04:32.899565 trubrics-1.4.4/examples/feedback/streamlit/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 07:04:21.000000 trubrics-1.4.4/examples/feedback/streamlit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1856 2023-08-08 07:04:21.000000 trubrics-1.4.4/examples/feedback/streamlit/llm_app.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1999 2023-08-08 07:04:21.000000 trubrics-1.4.4/examples/feedback/streamlit/llm_chatbot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2382 2023-08-08 07:04:21.000000 trubrics-1.4.4/examples/feedback/streamlit/titanic_app.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1267 2023-08-08 07:04:21.000000 trubrics-1.4.4/examples/feedback/streamlit/trubrics_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      248 2023-08-08 07:04:21.000000 trubrics-1.4.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-08-08 07:04:21.000000 trubrics-1.4.4/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      912 2023-08-08 07:04:32.903565 trubrics-1.4.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 07:04:32.899565 trubrics-1.4.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2035 2023-08-08 07:04:21.000000 trubrics-1.4.4/tests/test_context.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 07:04:32.899565 trubrics-1.4.4/trubrics/
+-rw-r--r--   0 runner    (1001) docker     (123)      388 2023-08-08 07:04:21.000000 trubrics-1.4.4/trubrics/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 07:04:32.899565 trubrics-1.4.4/trubrics/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-08-08 07:04:21.000000 trubrics-1.4.4/trubrics/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2551 2023-08-08 07:04:21.000000 trubrics-1.4.4/trubrics/cli/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)      930 2023-08-08 07:04:21.000000 trubrics-1.4.4/trubrics/cli/run.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8454 2023-08-08 07:04:21.000000 trubrics-1.4.4/trubrics/context.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 07:04:32.903565 trubrics-1.4.4/trubrics/example/
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-08-08 07:04:21.000000 trubrics-1.4.4/trubrics/example/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3926 2023-08-08 07:04:21.000000 trubrics-1.4.4/trubrics/example/my_first_trubric.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2226 2023-08-08 07:04:21.000000 trubrics-1.4.4/trubrics/example/titanic.py
+-rw-r--r--   0 runner    (1001) docker     (123)      354 2023-08-08 07:04:21.000000 trubrics-1.4.4/trubrics/example/titanic_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    61194 2023-08-08 07:04:21.000000 trubrics-1.4.4/trubrics/example/titanic_data.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     1004 2023-08-08 07:04:21.000000 trubrics-1.4.4/trubrics/example/trubric_run.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1272 2023-08-08 07:04:21.000000 trubrics-1.4.4/trubrics/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 07:04:32.903565 trubrics-1.4.4/trubrics/feedback/
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-08-08 07:04:21.000000 trubrics-1.4.4/trubrics/feedback/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      644 2023-08-08 07:04:21.000000 trubrics-1.4.4/trubrics/feedback/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1450 2023-08-08 07:04:21.000000 trubrics-1.4.4/trubrics/feedback/dataclass.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1339 2023-08-08 07:04:21.000000 trubrics-1.4.4/trubrics/feedback/save_to_trubrics.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 07:04:32.903565 trubrics-1.4.4/trubrics/integrations/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 07:04:21.000000 trubrics-1.4.4/trubrics/integrations/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 07:04:32.903565 trubrics-1.4.4/trubrics/integrations/dash/
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-08-08 07:04:21.000000 trubrics-1.4.4/trubrics/integrations/dash/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3141 2023-08-08 07:04:21.000000 trubrics-1.4.4/trubrics/integrations/dash/collect.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 07:04:32.903565 trubrics-1.4.4/trubrics/integrations/gradio/
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-08-08 07:04:21.000000 trubrics-1.4.4/trubrics/integrations/gradio/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2523 2023-08-08 07:04:21.000000 trubrics-1.4.4/trubrics/integrations/gradio/collect.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 07:04:32.903565 trubrics-1.4.4/trubrics/integrations/mlflow/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 07:04:21.000000 trubrics-1.4.4/trubrics/integrations/mlflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2902 2023-08-08 07:04:21.000000 trubrics-1.4.4/trubrics/integrations/mlflow/trubrics_validator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 07:04:32.903565 trubrics-1.4.4/trubrics/integrations/streamlit/
+-rw-r--r--   0 runner    (1001) docker     (123)      289 2023-08-08 07:04:21.000000 trubrics-1.4.4/trubrics/integrations/streamlit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7322 2023-08-08 07:04:21.000000 trubrics-1.4.4/trubrics/integrations/streamlit/collect.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2638 2023-08-08 07:04:21.000000 trubrics-1.4.4/trubrics/integrations/streamlit/experiment.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 07:04:21.000000 trubrics-1.4.4/trubrics/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 07:04:32.903565 trubrics-1.4.4/trubrics/trubrics_platform/
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-08-08 07:04:21.000000 trubrics-1.4.4/trubrics/trubrics_platform/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4295 2023-08-08 07:04:21.000000 trubrics-1.4.4/trubrics/trubrics_platform/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5145 2023-08-08 07:04:21.000000 trubrics-1.4.4/trubrics/trubrics_platform/firestore.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1157 2023-08-08 07:04:21.000000 trubrics-1.4.4/trubrics/trubrics_platform/trubrics_config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 07:04:32.903565 trubrics-1.4.4/trubrics/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 07:04:21.000000 trubrics-1.4.4/trubrics/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-08-08 07:04:21.000000 trubrics-1.4.4/trubrics/utils/pandas.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 07:04:32.903565 trubrics-1.4.4/trubrics/validations/
+-rw-r--r--   0 runner    (1001) docker     (123)      172 2023-08-08 07:04:21.000000 trubrics-1.4.4/trubrics/validations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7281 2023-08-08 07:04:21.000000 trubrics-1.4.4/trubrics/validations/dataclass.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 07:04:32.903565 trubrics-1.4.4/trubrics/validations/model/
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-08-08 07:04:21.000000 trubrics-1.4.4/trubrics/validations/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30069 2023-08-08 07:04:21.000000 trubrics-1.4.4/trubrics/validations/model/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4765 2023-08-08 07:04:21.000000 trubrics-1.4.4/trubrics/validations/run.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2900 2023-08-08 07:04:21.000000 trubrics-1.4.4/trubrics/validations/validation_output.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 07:04:32.899565 trubrics-1.4.4/trubrics.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      327 2023-08-08 07:04:32.000000 trubrics-1.4.4/trubrics.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1849 2023-08-08 07:04:32.000000 trubrics-1.4.4/trubrics.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 07:04:32.000000 trubrics-1.4.4/trubrics.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-08-08 07:04:32.000000 trubrics-1.4.4/trubrics.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      349 2023-08-08 07:04:32.000000 trubrics-1.4.4/trubrics.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-08-08 07:04:32.000000 trubrics-1.4.4/trubrics.egg-info/top_level.txt
```

### Comparing `trubrics-1.4.3/LICENSE` & `trubrics-1.4.4/LICENSE`

 * *Files identical despite different names*

### Comparing `trubrics-1.4.3/README.md` & `trubrics-1.4.4/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -10,14 +10,16 @@
 
     [<img src="./assets/sign_up.png"  width="200">](https://trubrics.streamlit.app/)
 
 2. Save feedback to Trubrics from our **demo LLM app**:
 
     [<img src="https://static.streamlit.io/badges/streamlit_badge_black_white.svg"  width="200">](https://trubrics-llm-example.streamlit.app/)
 
+Or watch a step by step video of integrating Trubrics into the LLM Streamlit app [here](https://www.youtube.com/watch?v=2Qt54qGwIdQ).
+
 ## Collect user feedback with the Python SDK
 
 The python SDK allows you to collect user feedback from your ML apps from any python backend or web framework. Install it with:
 
 ```console
 pip install trubrics
 ```
@@ -76,14 +78,18 @@
 collector.st_feedback(
     feedback_type="thumbs",
     model="your_model_name",
     open_feedback_label="[Optional] Provide additional feedback",
 )
 ```
 
+## Collect user feedback from a React.js app
+
+We have developed an [example](https://github.com/trubrics/trubrics-sdk/blob/main/examples/feedback/react_js) showing how you can collect feedback from a React app.
+
 ## Why should you monitor usage of your models?
 
 - **🚨 Identify bugs** - users are constantly running inference on your models, and may be more likely to find bugs than your ML monitoring system
 - **🧑‍💻️ Fine tune** - users often hold domain knowledge that can be useful to fine tune models
 - **👥 Align** - identifying user preferences will help you to align models to your users
 
 ## What's next?
```

### Comparing `trubrics-1.4.3/examples/feedback/streamlit/llm_app.py` & `trubrics-1.4.4/examples/feedback/streamlit/llm_app.py`

 * *Files 5% similar despite different names*

```diff
@@ -42,14 +42,16 @@
         )
 
         feedback = collector.st_feedback(
             feedback_type="thumbs",
             model=model,
             open_feedback_label="[Optional] Provide additional feedback",
             metadata={"response": st.session_state["response"], "prompt": prompt},
+            align="flex-start",
+            single_submit=False,
         )
 
         if feedback:
             trubrics_successful_feedback(feedback)
 
     else:
         st.warning("To save some feedback to Trubrics, add your account details in the sidebar.")
```

### Comparing `trubrics-1.4.3/examples/feedback/streamlit/titanic_app.py` & `trubrics-1.4.4/examples/feedback/streamlit/titanic_app.py`

 * *Files 2% similar despite different names*

```diff
@@ -62,12 +62,14 @@
         )
 
         feedback = collector.st_feedback(
             feedback_type=feedback_type,
             model="your_model_name",
             open_feedback_label="[Optional] Provide additional feedback",
             metadata=metadata,
+            align="flex-start",
+            single_submit=False,
         )
         if feedback:
             trubrics_successful_feedback(feedback)
 else:
     st.warning("Click 'Predict' in the sidebar to generate predictions.")
```

### Comparing `trubrics-1.4.3/examples/feedback/streamlit/trubrics_utils.py` & `trubrics-1.4.4/examples/feedback/streamlit/trubrics_utils.py`

 * *Files identical despite different names*

### Comparing `trubrics-1.4.3/setup.cfg` & `trubrics-1.4.4/setup.cfg`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = trubrics
-version = 1.4.3
+version = 1.4.4
 description = The first user insights platform for AI models.
 long_description = Full documentation available at https://trubrics.github.io/trubrics-sdk/.
 
 [options]
 packages = find:
 install_requires = file: requirements.txt
 
@@ -24,15 +24,15 @@
 [flake8]
 max-line-length = 120
 
 [isort]
 profile = black
 
 [options.extras_require]
-streamlit = streamlit>=1.20.0
+streamlit = streamlit>=1.20.0; streamlit-feedback>=0.0.8
 dash = dash>=2.6.2; dash-bootstrap-components>=1.2.1
 gradio = gradio>=3.8.1
 mlflow = mlflow>=2.0.0
 validations = GitPython>=3.1.31; numpy>=1.21.6; pandas>=1.3.5; scikit-learn>=1.0.0,<1.1.0
 
 [egg_info]
 tag_build =
```

### Comparing `trubrics-1.4.3/tests/test_context.py` & `trubrics-1.4.4/tests/test_context.py`

 * *Files identical despite different names*

### Comparing `trubrics-1.4.3/trubrics/cli/main.py` & `trubrics-1.4.4/trubrics/cli/main.py`

 * *Files identical despite different names*

### Comparing `trubrics-1.4.3/trubrics/cli/run.py` & `trubrics-1.4.4/trubrics/cli/run.py`

 * *Files identical despite different names*

### Comparing `trubrics-1.4.3/trubrics/context.py` & `trubrics-1.4.4/trubrics/context.py`

 * *Files identical despite different names*

### Comparing `trubrics-1.4.3/trubrics/example/my_first_trubric.json` & `trubrics-1.4.4/trubrics/example/my_first_trubric.json`

 * *Files identical despite different names*

### Comparing `trubrics-1.4.3/trubrics/example/titanic.py` & `trubrics-1.4.4/trubrics/example/titanic.py`

 * *Files identical despite different names*

### Comparing `trubrics-1.4.3/trubrics/example/titanic_data.csv` & `trubrics-1.4.4/trubrics/example/titanic_data.csv`

 * *Files identical despite different names*

### Comparing `trubrics-1.4.3/trubrics/example/trubric_run.py` & `trubrics-1.4.4/trubrics/example/trubric_run.py`

 * *Files identical despite different names*

### Comparing `trubrics-1.4.3/trubrics/exceptions.py` & `trubrics-1.4.4/trubrics/exceptions.py`

 * *Files identical despite different names*

### Comparing `trubrics-1.4.3/trubrics/feedback/config.py` & `trubrics-1.4.4/trubrics/feedback/config.py`

 * *Files identical despite different names*

### Comparing `trubrics-1.4.3/trubrics/feedback/dataclass.py` & `trubrics-1.4.4/trubrics/feedback/dataclass.py`

 * *Files identical despite different names*

### Comparing `trubrics-1.4.3/trubrics/feedback/save_to_trubrics.py` & `trubrics-1.4.4/trubrics/feedback/save_to_trubrics.py`

 * *Files identical despite different names*

### Comparing `trubrics-1.4.3/trubrics/integrations/dash/collect.py` & `trubrics-1.4.4/trubrics/integrations/dash/collect.py`

 * *Files identical despite different names*

### Comparing `trubrics-1.4.3/trubrics/integrations/gradio/collect.py` & `trubrics-1.4.4/trubrics/integrations/gradio/collect.py`

 * *Files identical despite different names*

### Comparing `trubrics-1.4.3/trubrics/integrations/mlflow/trubrics_validator.py` & `trubrics-1.4.4/trubrics/integrations/mlflow/trubrics_validator.py`

 * *Files identical despite different names*

### Comparing `trubrics-1.4.3/trubrics/integrations/streamlit/experiment.py` & `trubrics-1.4.4/trubrics/integrations/streamlit/experiment.py`

 * *Files identical despite different names*

### Comparing `trubrics-1.4.3/trubrics/trubrics_platform/auth.py` & `trubrics-1.4.4/trubrics/trubrics_platform/auth.py`

 * *Files identical despite different names*

### Comparing `trubrics-1.4.3/trubrics/trubrics_platform/firestore.py` & `trubrics-1.4.4/trubrics/trubrics_platform/firestore.py`

 * *Files identical despite different names*

### Comparing `trubrics-1.4.3/trubrics/trubrics_platform/trubrics_config.py` & `trubrics-1.4.4/trubrics/trubrics_platform/trubrics_config.py`

 * *Files identical despite different names*

### Comparing `trubrics-1.4.3/trubrics/validations/dataclass.py` & `trubrics-1.4.4/trubrics/validations/dataclass.py`

 * *Files identical despite different names*

### Comparing `trubrics-1.4.3/trubrics/validations/model/base.py` & `trubrics-1.4.4/trubrics/validations/model/base.py`

 * *Files identical despite different names*

### Comparing `trubrics-1.4.3/trubrics/validations/run.py` & `trubrics-1.4.4/trubrics/validations/run.py`

 * *Files identical despite different names*

### Comparing `trubrics-1.4.3/trubrics/validations/validation_output.py` & `trubrics-1.4.4/trubrics/validations/validation_output.py`

 * *Files identical despite different names*

### Comparing `trubrics-1.4.3/trubrics.egg-info/SOURCES.txt` & `trubrics-1.4.4/trubrics.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 pyproject.toml
 requirements.txt
 setup.cfg
 examples/__init__.py
 examples/feedback/__init__.py
 examples/feedback/streamlit/__init__.py
 examples/feedback/streamlit/llm_app.py
+examples/feedback/streamlit/llm_chatbot.py
 examples/feedback/streamlit/titanic_app.py
 examples/feedback/streamlit/trubrics_utils.py
 tests/test_context.py
 trubrics/__init__.py
 trubrics/context.py
 trubrics/exceptions.py
 trubrics/py.typed
```


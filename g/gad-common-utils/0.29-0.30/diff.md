# Comparing `tmp/gad_common_utils-0.29.tar.gz` & `tmp/gad_common_utils-0.30.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gad_common_utils-0.29.tar", last modified: Sun Jul 16 12:02:44 2023, max compression
+gzip compressed data, was "gad_common_utils-0.30.tar", last modified: Tue Aug  8 07:14:24 2023, max compression
```

## Comparing `gad_common_utils-0.29.tar` & `gad_common_utils-0.30.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 12:02:44.948770 gad_common_utils-0.29/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 12:02:44.944769 gad_common_utils-0.29/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 12:02:44.944769 gad_common_utils-0.29/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      859 2023-07-16 12:02:35.000000 gad_common_utils-0.29/.github/workflows/black-format-checker.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1196 2023-07-16 12:02:35.000000 gad_common_utils-0.29/.github/workflows/publish-to-pypi.yml
--rw-r--r--   0 runner    (1001) docker     (123)      957 2023-07-16 12:02:35.000000 gad_common_utils-0.29/.github/workflows/pytest.yml
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-07-16 12:02:35.000000 gad_common_utils-0.29/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      426 2023-07-16 12:02:35.000000 gad_common_utils-0.29/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      545 2023-07-16 12:02:44.948770 gad_common_utils-0.29/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      215 2023-07-16 12:02:35.000000 gad_common_utils-0.29/Readme.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 12:02:44.944769 gad_common_utils-0.29/common_utils/
--rw-r--r--   0 runner    (1001) docker     (123)      130 2023-07-16 12:02:35.000000 gad_common_utils-0.29/common_utils/Readme.md
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-16 12:02:35.000000 gad_common_utils-0.29/common_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      157 2023-07-16 12:02:44.000000 gad_common_utils-0.29/common_utils/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     8304 2023-07-16 12:02:35.000000 gad_common_utils-0.29/common_utils/data_loading_management.py
--rw-r--r--   0 runner    (1001) docker     (123)     4853 2023-07-16 12:02:35.000000 gad_common_utils-0.29/common_utils/data_type_conversion.py
--rw-r--r--   0 runner    (1001) docker     (123)     3882 2023-07-16 12:02:35.000000 gad_common_utils-0.29/common_utils/date_time_methods.py
--rw-r--r--   0 runner    (1001) docker     (123)     7941 2023-07-16 12:02:35.000000 gad_common_utils-0.29/common_utils/dynamodb_methods.py
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-07-16 12:02:35.000000 gad_common_utils-0.29/common_utils/dynamodb_ray.py
--rw-r--r--   0 runner    (1001) docker     (123)     1438 2023-07-16 12:02:35.000000 gad_common_utils-0.29/common_utils/files_methods.py
--rw-r--r--   0 runner    (1001) docker     (123)    29472 2023-07-16 12:02:35.000000 gad_common_utils-0.29/common_utils/gad_utils.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      895 2023-07-16 12:02:35.000000 gad_common_utils-0.29/common_utils/gad_utils_additionals.py
--rw-r--r--   0 runner    (1001) docker     (123)     6169 2023-07-16 12:02:35.000000 gad_common_utils-0.29/common_utils/json_schema_methods.py
--rw-r--r--   0 runner    (1001) docker     (123)     2165 2023-07-16 12:02:35.000000 gad_common_utils-0.29/common_utils/run_athena_query.py
--rw-r--r--   0 runner    (1001) docker     (123)     4421 2023-07-16 12:02:35.000000 gad_common_utils-0.29/common_utils/s3_methods.py
--rw-r--r--   0 runner    (1001) docker     (123)     1443 2023-07-16 12:02:35.000000 gad_common_utils-0.29/common_utils/sql_methods.py
--rw-r--r--   0 runner    (1001) docker     (123)      632 2023-07-16 12:02:35.000000 gad_common_utils-0.29/common_utils/string_transformations.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 12:02:44.948770 gad_common_utils-0.29/gad_common_utils.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      545 2023-07-16 12:02:44.000000 gad_common_utils-0.29/gad_common_utils.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      923 2023-07-16 12:02:44.000000 gad_common_utils-0.29/gad_common_utils.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-16 12:02:44.000000 gad_common_utils-0.29/gad_common_utils.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-16 12:02:44.000000 gad_common_utils-0.29/gad_common_utils.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-16 12:02:44.000000 gad_common_utils-0.29/gad_common_utils.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      598 2023-07-16 12:02:35.000000 gad_common_utils-0.29/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-16 12:02:44.948770 gad_common_utils-0.29/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 12:02:44.948770 gad_common_utils-0.29/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-16 12:02:35.000000 gad_common_utils-0.29/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      792 2023-07-16 12:02:35.000000 gad_common_utils-0.29/tests/test_json_schema_methods.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 07:14:24.370375 gad_common_utils-0.30/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 07:14:24.366375 gad_common_utils-0.30/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 07:14:24.366375 gad_common_utils-0.30/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      859 2023-08-08 07:14:10.000000 gad_common_utils-0.30/.github/workflows/black-format-checker.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1196 2023-08-08 07:14:10.000000 gad_common_utils-0.30/.github/workflows/publish-to-pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      957 2023-08-08 07:14:10.000000 gad_common_utils-0.30/.github/workflows/pytest.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-08-08 07:14:10.000000 gad_common_utils-0.30/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      426 2023-08-08 07:14:10.000000 gad_common_utils-0.30/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      545 2023-08-08 07:14:24.370375 gad_common_utils-0.30/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      215 2023-08-08 07:14:10.000000 gad_common_utils-0.30/Readme.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 07:14:24.370375 gad_common_utils-0.30/common_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-08-08 07:14:10.000000 gad_common_utils-0.30/common_utils/Readme.md
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 07:14:10.000000 gad_common_utils-0.30/common_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-08-08 07:14:24.000000 gad_common_utils-0.30/common_utils/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8304 2023-08-08 07:14:10.000000 gad_common_utils-0.30/common_utils/data_loading_management.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4853 2023-08-08 07:14:10.000000 gad_common_utils-0.30/common_utils/data_type_conversion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3882 2023-08-08 07:14:10.000000 gad_common_utils-0.30/common_utils/date_time_methods.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7941 2023-08-08 07:14:10.000000 gad_common_utils-0.30/common_utils/dynamodb_methods.py
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-08-08 07:14:10.000000 gad_common_utils-0.30/common_utils/dynamodb_ray.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1438 2023-08-08 07:14:10.000000 gad_common_utils-0.30/common_utils/files_methods.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29519 2023-08-08 07:14:10.000000 gad_common_utils-0.30/common_utils/gad_utils.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      895 2023-08-08 07:14:10.000000 gad_common_utils-0.30/common_utils/gad_utils_additionals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6169 2023-08-08 07:14:10.000000 gad_common_utils-0.30/common_utils/json_schema_methods.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2165 2023-08-08 07:14:10.000000 gad_common_utils-0.30/common_utils/run_athena_query.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4421 2023-08-08 07:14:10.000000 gad_common_utils-0.30/common_utils/s3_methods.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1443 2023-08-08 07:14:10.000000 gad_common_utils-0.30/common_utils/sql_methods.py
+-rw-r--r--   0 runner    (1001) docker     (123)      632 2023-08-08 07:14:10.000000 gad_common_utils-0.30/common_utils/string_transformations.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 07:14:24.370375 gad_common_utils-0.30/gad_common_utils.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      545 2023-08-08 07:14:24.000000 gad_common_utils-0.30/gad_common_utils.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      923 2023-08-08 07:14:24.000000 gad_common_utils-0.30/gad_common_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 07:14:24.000000 gad_common_utils-0.30/gad_common_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-08-08 07:14:24.000000 gad_common_utils-0.30/gad_common_utils.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-08-08 07:14:24.000000 gad_common_utils-0.30/gad_common_utils.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      598 2023-08-08 07:14:10.000000 gad_common_utils-0.30/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-08 07:14:24.370375 gad_common_utils-0.30/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 07:14:24.370375 gad_common_utils-0.30/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 07:14:10.000000 gad_common_utils-0.30/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      792 2023-08-08 07:14:10.000000 gad_common_utils-0.30/tests/test_json_schema_methods.py
```

### Comparing `gad_common_utils-0.29/.github/workflows/black-format-checker.yml` & `gad_common_utils-0.30/.github/workflows/black-format-checker.yml`

 * *Files identical despite different names*

### Comparing `gad_common_utils-0.29/.github/workflows/publish-to-pypi.yml` & `gad_common_utils-0.30/.github/workflows/publish-to-pypi.yml`

 * *Files identical despite different names*

### Comparing `gad_common_utils-0.29/.github/workflows/pytest.yml` & `gad_common_utils-0.30/.github/workflows/pytest.yml`

 * *Files identical despite different names*

### Comparing `gad_common_utils-0.29/PKG-INFO` & `gad_common_utils-0.30/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gad_common_utils
-Version: 0.29
+Version: 0.30
 Summary: gad utility
 Project-URL: Homepage, http://gad-co.ml
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

### Comparing `gad_common_utils-0.29/common_utils/data_loading_management.py` & `gad_common_utils-0.30/common_utils/data_loading_management.py`

 * *Files identical despite different names*

### Comparing `gad_common_utils-0.29/common_utils/data_type_conversion.py` & `gad_common_utils-0.30/common_utils/data_type_conversion.py`

 * *Files identical despite different names*

### Comparing `gad_common_utils-0.29/common_utils/date_time_methods.py` & `gad_common_utils-0.30/common_utils/date_time_methods.py`

 * *Files identical despite different names*

### Comparing `gad_common_utils-0.29/common_utils/dynamodb_methods.py` & `gad_common_utils-0.30/common_utils/dynamodb_methods.py`

 * *Files identical despite different names*

### Comparing `gad_common_utils-0.29/common_utils/files_methods.py` & `gad_common_utils-0.30/common_utils/files_methods.py`

 * *Files identical despite different names*

### Comparing `gad_common_utils-0.29/common_utils/gad_utils.py` & `gad_common_utils-0.30/common_utils/gad_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -84,14 +84,15 @@
 
 
 def generate_airflow_dag(
     project: str,
     dag_id: str,
     schedule_interval,
     tasks: list,
+    doc_md: str = None,
     content_path: str = "gad-deliveries",
     dag_params: dict = {},
 ):
     """
     Creates a DAG using the specified parameters.
 
     Args:
@@ -638,14 +639,15 @@
     # dag creation
     dag = DAG(
         dag_id=dag_id,
         default_args=default_args,
         schedule_interval=schedule_interval,
         max_active_runs=1,
         concurrency=10,
+        doc_md=doc_md,
         params=dag_params,
     )
 
     # use only the params that are not empty
     dag_params_not_empty = {key: val for key, val in dag_params.items() if val != ""}
 
     """
```

### Comparing `gad_common_utils-0.29/common_utils/gad_utils_additionals.py` & `gad_common_utils-0.30/common_utils/gad_utils_additionals.py`

 * *Files identical despite different names*

### Comparing `gad_common_utils-0.29/common_utils/json_schema_methods.py` & `gad_common_utils-0.30/common_utils/json_schema_methods.py`

 * *Files identical despite different names*

### Comparing `gad_common_utils-0.29/common_utils/run_athena_query.py` & `gad_common_utils-0.30/common_utils/run_athena_query.py`

 * *Files identical despite different names*

### Comparing `gad_common_utils-0.29/common_utils/s3_methods.py` & `gad_common_utils-0.30/common_utils/s3_methods.py`

 * *Files identical despite different names*

### Comparing `gad_common_utils-0.29/common_utils/sql_methods.py` & `gad_common_utils-0.30/common_utils/sql_methods.py`

 * *Files identical despite different names*

### Comparing `gad_common_utils-0.29/common_utils/string_transformations.py` & `gad_common_utils-0.30/common_utils/string_transformations.py`

 * *Files identical despite different names*

### Comparing `gad_common_utils-0.29/gad_common_utils.egg-info/PKG-INFO` & `gad_common_utils-0.30/gad_common_utils.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gad-common-utils
-Version: 0.29
+Version: 0.30
 Summary: gad utility
 Project-URL: Homepage, http://gad-co.ml
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

### Comparing `gad_common_utils-0.29/gad_common_utils.egg-info/SOURCES.txt` & `gad_common_utils-0.30/gad_common_utils.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gad_common_utils-0.29/pyproject.toml` & `gad_common_utils-0.30/pyproject.toml`

 * *Files identical despite different names*

### Comparing `gad_common_utils-0.29/tests/test_json_schema_methods.py` & `gad_common_utils-0.30/tests/test_json_schema_methods.py`

 * *Files identical despite different names*


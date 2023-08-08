# Comparing `tmp/baram-0.3.2.tar.gz` & `tmp/baram-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "baram-0.3.2.tar", max compression
+gzip compressed data, was "baram-0.3.3.tar", max compression
```

## Comparing `baram-0.3.2.tar` & `baram-0.3.3.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0      660 2022-05-04 05:03:24.350145 baram-0.3.2/baram/airflow_manager.py
--rw-r--r--   0        0        0     1161 2022-05-31 00:21:03.987264 baram-0.3.2/baram/async_crawler.py
--rw-r--r--   0        0        0      644 2023-02-13 00:11:32.025035 baram-0.3.2/baram/conf_manager.py
--rw-r--r--   0        0        0    14117 2023-08-07 01:33:48.528999 baram-0.3.2/baram/ec2_manager.py
--rw-r--r--   0        0        0      773 2022-05-24 00:56:46.354660 baram-0.3.2/baram/ecr_manager.py
--rw-r--r--   0        0        0     2385 2023-03-15 07:55:06.640970 baram-0.3.2/baram/efs_manager.py
--rw-r--r--   0        0        0    15031 2023-08-05 15:07:15.520000 baram-0.3.2/baram/ge_manager.py
--rw-r--r--   0        0        0     7405 2022-05-24 00:56:46.354824 baram-0.3.2/baram/glue_manager.py
--rw-r--r--   0        0        0     3101 2023-03-25 00:11:36.843156 baram-0.3.2/baram/iam_manager.py
--rw-r--r--   0        0        0     1098 2022-05-04 05:35:56.208476 baram-0.3.2/baram/kms_manager.py
--rw-r--r--   0        0        0     2064 2022-05-06 01:06:54.382347 baram-0.3.2/baram/lambda_manager.py
--rw-r--r--   0        0        0      477 2022-05-06 01:06:54.382534 baram-0.3.2/baram/log_manager.py
--rw-r--r--   0        0        0      605 2022-05-04 05:35:56.213543 baram-0.3.2/baram/poetry_manager.py
--rw-r--r--   0        0        0      560 2022-05-04 05:23:44.845922 baram-0.3.2/baram/process_manager.py
--rw-r--r--   0        0        0      679 2023-02-13 00:11:32.025599 baram-0.3.2/baram/requests_manager.py
--rw-r--r--   0        0        0     9281 2022-06-28 04:05:40.812460 baram-0.3.2/baram/s3_manager.py
--rw-r--r--   0        0        0     7231 2023-03-15 07:55:06.641394 baram-0.3.2/baram/sagemaker_manager.py
--rw-r--r--   0        0        0      566 2023-08-07 01:40:55.932601 baram-0.3.2/pyproject.toml
--rw-r--r--   0        0        0      224 2022-05-03 23:39:58.553478 baram-0.3.2/readme.md
--rw-r--r--   0        0        0      961 1970-01-01 00:00:00.000000 baram-0.3.2/PKG-INFO
+-rw-r--r--   0        0        0      660 2022-05-04 05:03:24.350145 baram-0.3.3/baram/airflow_manager.py
+-rw-r--r--   0        0        0     1161 2022-05-31 00:21:03.987264 baram-0.3.3/baram/async_crawler.py
+-rw-r--r--   0        0        0      644 2023-02-13 00:11:32.025035 baram-0.3.3/baram/conf_manager.py
+-rw-r--r--   0        0        0    14117 2023-08-07 01:33:48.528999 baram-0.3.3/baram/ec2_manager.py
+-rw-r--r--   0        0        0      773 2022-05-24 00:56:46.354660 baram-0.3.3/baram/ecr_manager.py
+-rw-r--r--   0        0        0     2385 2023-03-15 07:55:06.640970 baram-0.3.3/baram/efs_manager.py
+-rw-r--r--   0        0        0    15031 2023-08-07 01:42:39.711053 baram-0.3.3/baram/ge_manager.py
+-rw-r--r--   0        0        0     7405 2022-05-24 00:56:46.354824 baram-0.3.3/baram/glue_manager.py
+-rw-r--r--   0        0        0     3101 2023-03-25 00:11:36.843156 baram-0.3.3/baram/iam_manager.py
+-rw-r--r--   0        0        0     1098 2022-05-04 05:35:56.208476 baram-0.3.3/baram/kms_manager.py
+-rw-r--r--   0        0        0     2064 2022-05-06 01:06:54.382347 baram-0.3.3/baram/lambda_manager.py
+-rw-r--r--   0        0        0      477 2022-05-06 01:06:54.382534 baram-0.3.3/baram/log_manager.py
+-rw-r--r--   0        0        0      605 2022-05-04 05:35:56.213543 baram-0.3.3/baram/poetry_manager.py
+-rw-r--r--   0        0        0      560 2022-05-04 05:23:44.845922 baram-0.3.3/baram/process_manager.py
+-rw-r--r--   0        0        0      679 2023-02-13 00:11:32.025599 baram-0.3.3/baram/requests_manager.py
+-rw-r--r--   0        0        0     9281 2022-06-28 04:05:40.812460 baram-0.3.3/baram/s3_manager.py
+-rw-r--r--   0        0        0     7231 2023-03-15 07:55:06.641394 baram-0.3.3/baram/sagemaker_manager.py
+-rw-r--r--   0        0        0      567 2023-08-07 04:00:46.335203 baram-0.3.3/pyproject.toml
+-rw-r--r--   0        0        0      224 2022-05-03 23:39:58.553478 baram-0.3.3/readme.md
+-rw-r--r--   0        0        0      963 1970-01-01 00:00:00.000000 baram-0.3.3/PKG-INFO
```

### Comparing `baram-0.3.2/baram/airflow_manager.py` & `baram-0.3.3/baram/airflow_manager.py`

 * *Files identical despite different names*

### Comparing `baram-0.3.2/baram/async_crawler.py` & `baram-0.3.3/baram/async_crawler.py`

 * *Files identical despite different names*

### Comparing `baram-0.3.2/baram/conf_manager.py` & `baram-0.3.3/baram/conf_manager.py`

 * *Files identical despite different names*

### Comparing `baram-0.3.2/baram/ec2_manager.py` & `baram-0.3.3/baram/ec2_manager.py`

 * *Files identical despite different names*

### Comparing `baram-0.3.2/baram/ecr_manager.py` & `baram-0.3.3/baram/ecr_manager.py`

 * *Files identical despite different names*

### Comparing `baram-0.3.2/baram/efs_manager.py` & `baram-0.3.3/baram/efs_manager.py`

 * *Files identical despite different names*

### Comparing `baram-0.3.2/baram/ge_manager.py` & `baram-0.3.3/baram/ge_manager.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 from typing import Union, List, Optional
 
-from great_expectations.dataset import Dataset
-from great_expectations.core.batch import Batch
+from great_expectations.checkpoint.types.checkpoint_result import CheckpointResult
 from great_expectations.core import ExpectationSuite, ExpectationConfiguration
-from great_expectations.datasource.fluent.sql_datasource import TableAsset
-from great_expectations.exceptions import DataContextError
-from great_expectations.validator.validator import Validator
+from great_expectations.core import ExpectationSuiteValidationResult
 from great_expectations.core import ExpectationValidationResult
+from great_expectations.core.batch import Batch
 from great_expectations.data_context import EphemeralDataContext
-from great_expectations.core import ExpectationSuiteValidationResult
 from great_expectations.data_context.types.base import DataContextConfig
-from great_expectations.datasource.fluent.pandas_datasource import CSVAsset
-from great_expectations.checkpoint.types.checkpoint_result import CheckpointResult
 from great_expectations.data_context.types.resource_identifiers import GXCloudIdentifier
+from great_expectations.dataset import Dataset
+from great_expectations.datasource.fluent.pandas_datasource import CSVAsset
+from great_expectations.datasource.fluent.sql_datasource import TableAsset
+from great_expectations.exceptions import DataContextError
 from great_expectations.profile.user_configurable_profiler import UserConfigurableProfiler
+from great_expectations.validator.validator import Validator
 
 
 class GEManager(object):
     def __init__(self, gx_s3_bucket_name: str, data_s3_bucket_name: str):
         '''
 
         :param data_s3_bucket_name:
```

### Comparing `baram-0.3.2/baram/glue_manager.py` & `baram-0.3.3/baram/glue_manager.py`

 * *Files identical despite different names*

### Comparing `baram-0.3.2/baram/iam_manager.py` & `baram-0.3.3/baram/iam_manager.py`

 * *Files identical despite different names*

### Comparing `baram-0.3.2/baram/kms_manager.py` & `baram-0.3.3/baram/kms_manager.py`

 * *Files identical despite different names*

### Comparing `baram-0.3.2/baram/lambda_manager.py` & `baram-0.3.3/baram/lambda_manager.py`

 * *Files identical despite different names*

### Comparing `baram-0.3.2/baram/poetry_manager.py` & `baram-0.3.3/baram/poetry_manager.py`

 * *Files identical despite different names*

### Comparing `baram-0.3.2/baram/process_manager.py` & `baram-0.3.3/baram/process_manager.py`

 * *Files identical despite different names*

### Comparing `baram-0.3.2/baram/requests_manager.py` & `baram-0.3.3/baram/requests_manager.py`

 * *Files identical despite different names*

### Comparing `baram-0.3.2/baram/s3_manager.py` & `baram-0.3.3/baram/s3_manager.py`

 * *Files identical despite different names*

### Comparing `baram-0.3.2/baram/sagemaker_manager.py` & `baram-0.3.3/baram/sagemaker_manager.py`

 * *Files identical despite different names*

### Comparing `baram-0.3.2/pyproject.toml` & `baram-0.3.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 [tool.poetry]
 name = "baram"
-version = "0.3.2"
+version = "0.3.3"
 description = "AWS Framework for python"
 authors = ["Kwangsik Lee <lks21c@gmail.com>"]
 readme = "readme.md"
 
 [tool.poetry.dependencies]
-python = "~3.9"
+python = "~3.11"
 fire = "^0.4.0"
 pytest-cov = "^3.0.0"
 boto3 = "1.26.74"
 aiohttp = "^3.8.1"
 nest-asyncio = "^1.5.5"
 toml = "^0.10.2"
 ujson = "^5.5.0"
```

### Comparing `baram-0.3.2/PKG-INFO` & `baram-0.3.3/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: baram
-Version: 0.3.2
+Version: 0.3.3
 Summary: AWS Framework for python
 Author: Kwangsik Lee
 Author-email: lks21c@gmail.com
-Requires-Python: >=3.9,<3.10
+Requires-Python: >=3.11,<3.12
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: aiohttp (>=3.8.1,<4.0.0)
 Requires-Dist: boto3 (==1.26.74)
 Requires-Dist: fire (>=0.4.0,<0.5.0)
 Requires-Dist: great-expectations (==0.17.8)
 Requires-Dist: nest-asyncio (>=1.5.5,<2.0.0)
 Requires-Dist: pyathena (==3.0.6)
 Requires-Dist: pytest-cov (>=3.0.0,<4.0.0)
```


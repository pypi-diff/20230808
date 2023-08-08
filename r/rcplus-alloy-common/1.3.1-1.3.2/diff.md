# Comparing `tmp/rcplus_alloy_common-1.3.1.tar.gz` & `tmp/rcplus_alloy_common-1.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rcplus_alloy_common-1.3.1.tar", max compression
+gzip compressed data, was "rcplus_alloy_common-1.3.2.tar", max compression
```

## Comparing `rcplus_alloy_common-1.3.1.tar` & `rcplus_alloy_common-1.3.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0       77 2023-08-07 14:20:40.868916 rcplus_alloy_common-1.3.1/LICENSE
--rw-r--r--   0        0        0      571 2023-08-07 14:20:40.868916 rcplus_alloy_common-1.3.1/README.md
--rw-r--r--   0        0        0     1951 2023-08-07 14:20:40.872916 rcplus_alloy_common-1.3.1/pyproject.toml
--rw-r--r--   0        0        0     2839 2023-08-07 14:20:40.872916 rcplus_alloy_common-1.3.1/src/rcplus_alloy_common/__init__.py
--rw-r--r--   0        0        0      567 2023-08-07 14:20:40.872916 rcplus_alloy_common-1.3.1/src/rcplus_alloy_common/airflow/__init__.py
--rw-r--r--   0        0        0     1179 2023-08-07 14:20:40.872916 rcplus_alloy_common-1.3.1/src/rcplus_alloy_common/airflow/dag.py
--rw-r--r--   0        0        0     1681 2023-08-07 14:20:40.872916 rcplus_alloy_common-1.3.1/src/rcplus_alloy_common/airflow/decorators.py
--rw-r--r--   0        0        0      703 2023-08-07 14:20:40.872916 rcplus_alloy_common-1.3.1/src/rcplus_alloy_common/airflow/hooks.py
--rw-r--r--   0        0        0     7448 2023-08-07 14:20:40.872916 rcplus_alloy_common-1.3.1/src/rcplus_alloy_common/airflow/observability.py
--rw-r--r--   0        0        0    20030 2023-08-07 14:20:40.872916 rcplus_alloy_common-1.3.1/src/rcplus_alloy_common/airflow/operators.py
--rw-r--r--   0        0        0     2611 2023-08-07 14:20:40.872916 rcplus_alloy_common-1.3.1/src/rcplus_alloy_common/airflow/sensors.py
--rw-r--r--   0        0        0     2799 2023-08-07 14:20:40.872916 rcplus_alloy_common-1.3.1/src/rcplus_alloy_common/airflow/utils.py
--rw-r--r--   0        0        0     2279 2023-08-07 14:20:40.872916 rcplus_alloy_common-1.3.1/src/rcplus_alloy_common/constants.py
--rw-r--r--   0        0        0     4391 2023-08-07 14:20:40.872916 rcplus_alloy_common-1.3.1/src/rcplus_alloy_common/logging.py
--rw-r--r--   0        0        0     6326 2023-08-07 14:20:40.872916 rcplus_alloy_common-1.3.1/src/rcplus_alloy_common/metrics.py
--rw-r--r--   0        0        0     3926 2023-08-07 14:20:40.872916 rcplus_alloy_common-1.3.1/src/rcplus_alloy_common/retry.py
--rw-r--r--   0        0        0       19 2023-08-07 14:20:40.872916 rcplus_alloy_common-1.3.1/src/rcplus_alloy_common/version.py
--rw-r--r--   0        0        0     1781 1970-01-01 00:00:00.000000 rcplus_alloy_common-1.3.1/PKG-INFO
+-rw-r--r--   0        0        0       77 2023-08-08 12:37:02.228426 rcplus_alloy_common-1.3.2/LICENSE
+-rw-r--r--   0        0        0      571 2023-08-08 12:37:02.228426 rcplus_alloy_common-1.3.2/README.md
+-rw-r--r--   0        0        0     1951 2023-08-08 12:37:02.228426 rcplus_alloy_common-1.3.2/pyproject.toml
+-rw-r--r--   0        0        0     2839 2023-08-08 12:37:02.228426 rcplus_alloy_common-1.3.2/src/rcplus_alloy_common/__init__.py
+-rw-r--r--   0        0        0      567 2023-08-08 12:37:02.228426 rcplus_alloy_common-1.3.2/src/rcplus_alloy_common/airflow/__init__.py
+-rw-r--r--   0        0        0     1179 2023-08-08 12:37:02.228426 rcplus_alloy_common-1.3.2/src/rcplus_alloy_common/airflow/dag.py
+-rw-r--r--   0        0        0     1681 2023-08-08 12:37:02.228426 rcplus_alloy_common-1.3.2/src/rcplus_alloy_common/airflow/decorators.py
+-rw-r--r--   0        0        0      703 2023-08-08 12:37:02.228426 rcplus_alloy_common-1.3.2/src/rcplus_alloy_common/airflow/hooks.py
+-rw-r--r--   0        0        0     7448 2023-08-08 12:37:02.228426 rcplus_alloy_common-1.3.2/src/rcplus_alloy_common/airflow/observability.py
+-rw-r--r--   0        0        0    20030 2023-08-08 12:37:02.228426 rcplus_alloy_common-1.3.2/src/rcplus_alloy_common/airflow/operators.py
+-rw-r--r--   0        0        0     2611 2023-08-08 12:37:02.228426 rcplus_alloy_common-1.3.2/src/rcplus_alloy_common/airflow/sensors.py
+-rw-r--r--   0        0        0     2799 2023-08-08 12:37:02.228426 rcplus_alloy_common-1.3.2/src/rcplus_alloy_common/airflow/utils.py
+-rw-r--r--   0        0        0     2279 2023-08-08 12:37:02.228426 rcplus_alloy_common-1.3.2/src/rcplus_alloy_common/constants.py
+-rw-r--r--   0        0        0     6148 2023-08-08 12:37:02.228426 rcplus_alloy_common-1.3.2/src/rcplus_alloy_common/logging.py
+-rw-r--r--   0        0        0     6326 2023-08-08 12:37:02.228426 rcplus_alloy_common-1.3.2/src/rcplus_alloy_common/metrics.py
+-rw-r--r--   0        0        0     3926 2023-08-08 12:37:02.228426 rcplus_alloy_common-1.3.2/src/rcplus_alloy_common/retry.py
+-rw-r--r--   0        0        0       19 2023-08-08 12:37:02.228426 rcplus_alloy_common-1.3.2/src/rcplus_alloy_common/version.py
+-rw-r--r--   0        0        0     1781 1970-01-01 00:00:00.000000 rcplus_alloy_common-1.3.2/PKG-INFO
```

### Comparing `rcplus_alloy_common-1.3.1/README.md` & `rcplus_alloy_common-1.3.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # rcplus-alloy-lib-py-common
 
 ![PyPI](https://img.shields.io/pypi/v/rcplus-alloy-common)
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/rcplus-alloy-common)
 ![Coverage badge](./coverage.svg)
 
-Current version: **v1.3.1**
+Current version: **v1.3.2**
 
 ---
 
 Python utilities for RC+/Alloy.
 
 _**NOTE**_: This Python package is published to PyPI.org as publicly available package.
```

### Comparing `rcplus_alloy_common-1.3.1/pyproject.toml` & `rcplus_alloy_common-1.3.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 build-backend = "poetry.core.masonry.api"
 
 [tool.black]
 line-length = 120
 
 [tool.poetry]
 name = "rcplus_alloy_common"
-version = "1.3.1"
+version = "1.3.2"
 description = "RC+/Alloy helpers functions for Python"
 readme = "README.md"
 authors = [
     "Ringier AG <info@rcplus.io>",
 ]
 license = "Proprietary"
 repository = "https://github.com/ringier-data/rcplus-alloy-lib-py-common"
```

### Comparing `rcplus_alloy_common-1.3.1/src/rcplus_alloy_common/__init__.py` & `rcplus_alloy_common-1.3.2/src/rcplus_alloy_common/__init__.py`

 * *Files identical despite different names*

### Comparing `rcplus_alloy_common-1.3.1/src/rcplus_alloy_common/airflow/__init__.py` & `rcplus_alloy_common-1.3.2/src/rcplus_alloy_common/airflow/__init__.py`

 * *Files identical despite different names*

### Comparing `rcplus_alloy_common-1.3.1/src/rcplus_alloy_common/airflow/dag.py` & `rcplus_alloy_common-1.3.2/src/rcplus_alloy_common/airflow/dag.py`

 * *Files identical despite different names*

### Comparing `rcplus_alloy_common-1.3.1/src/rcplus_alloy_common/airflow/decorators.py` & `rcplus_alloy_common-1.3.2/src/rcplus_alloy_common/airflow/decorators.py`

 * *Files identical despite different names*

### Comparing `rcplus_alloy_common-1.3.1/src/rcplus_alloy_common/airflow/hooks.py` & `rcplus_alloy_common-1.3.2/src/rcplus_alloy_common/airflow/hooks.py`

 * *Files identical despite different names*

### Comparing `rcplus_alloy_common-1.3.1/src/rcplus_alloy_common/airflow/observability.py` & `rcplus_alloy_common-1.3.2/src/rcplus_alloy_common/airflow/observability.py`

 * *Files identical despite different names*

### Comparing `rcplus_alloy_common-1.3.1/src/rcplus_alloy_common/airflow/operators.py` & `rcplus_alloy_common-1.3.2/src/rcplus_alloy_common/airflow/operators.py`

 * *Files identical despite different names*

### Comparing `rcplus_alloy_common-1.3.1/src/rcplus_alloy_common/airflow/sensors.py` & `rcplus_alloy_common-1.3.2/src/rcplus_alloy_common/airflow/sensors.py`

 * *Files identical despite different names*

### Comparing `rcplus_alloy_common-1.3.1/src/rcplus_alloy_common/airflow/utils.py` & `rcplus_alloy_common-1.3.2/src/rcplus_alloy_common/airflow/utils.py`

 * *Files identical despite different names*

### Comparing `rcplus_alloy_common-1.3.1/src/rcplus_alloy_common/constants.py` & `rcplus_alloy_common-1.3.2/src/rcplus_alloy_common/constants.py`

 * *Files identical despite different names*

### Comparing `rcplus_alloy_common-1.3.1/src/rcplus_alloy_common/metrics.py` & `rcplus_alloy_common-1.3.2/src/rcplus_alloy_common/metrics.py`

 * *Files identical despite different names*

### Comparing `rcplus_alloy_common-1.3.1/src/rcplus_alloy_common/retry.py` & `rcplus_alloy_common-1.3.2/src/rcplus_alloy_common/retry.py`

 * *Files identical despite different names*

### Comparing `rcplus_alloy_common-1.3.1/PKG-INFO` & `rcplus_alloy_common-1.3.2/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rcplus-alloy-common
-Version: 1.3.1
+Version: 1.3.2
 Summary: RC+/Alloy helpers functions for Python
 Home-page: https://github.com/ringier-data/rcplus-alloy-lib-py-common
 License: Proprietary
 Keywords: rcplus,alloy,logging,metrics,utilities
 Author: Ringier AG
 Author-email: info@rcplus.io
 Requires-Python: >=3.10,<4
@@ -29,15 +29,15 @@
 
 # rcplus-alloy-lib-py-common
 
 ![PyPI](https://img.shields.io/pypi/v/rcplus-alloy-common)
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/rcplus-alloy-common)
 ![Coverage badge](./coverage.svg)
 
-Current version: **v1.3.1**
+Current version: **v1.3.2**
 
 ---
 
 Python utilities for RC+/Alloy.
 
 _**NOTE**_: This Python package is published to PyPI.org as publicly available package.
```


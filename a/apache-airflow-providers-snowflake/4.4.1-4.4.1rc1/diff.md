# Comparing `tmp/apache-airflow-providers-snowflake-4.4.1.tar.gz` & `tmp/apache-airflow-providers-snowflake-4.4.1rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apache-airflow-providers-snowflake-4.4.1.tar", last modified: Fri Aug  4 21:35:58 2023, max compression
+gzip compressed data, was "apache-airflow-providers-snowflake-4.4.1rc1.tar", last modified: Fri Aug  4 21:41:41 2023, max compression
```

## Comparing `apache-airflow-providers-snowflake-4.4.1.tar` & `apache-airflow-providers-snowflake-4.4.1rc1.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 21:35:58.651176 apache-airflow-providers-snowflake-4.4.1/
--rw-r--r--   0 root         (0) root         (0)    10850 2023-06-01 06:14:29.000000 apache-airflow-providers-snowflake-4.4.1/LICENSE
--rw-r--r--   0 root         (0) root         (0)     1104 2023-08-04 21:35:57.000000 apache-airflow-providers-snowflake-4.4.1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      240 2023-06-01 06:14:29.000000 apache-airflow-providers-snowflake-4.4.1/NOTICE
--rw-r--r--   0 root         (0) root         (0)     6038 2023-08-04 21:35:58.651767 apache-airflow-providers-snowflake-4.4.1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     4314 2023-08-04 21:35:57.000000 apache-airflow-providers-snowflake-4.4.1/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 21:35:58.537130 apache-airflow-providers-snowflake-4.4.1/airflow/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 21:35:58.538284 apache-airflow-providers-snowflake-4.4.1/airflow/providers/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 21:35:58.577444 apache-airflow-providers-snowflake-4.4.1/airflow/providers/snowflake/
--rw-r--r--   0 root         (0) root         (0)     1578 2023-08-04 21:33:34.000000 apache-airflow-providers-snowflake-4.4.1/airflow/providers/snowflake/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5012 2023-08-04 21:35:57.000000 apache-airflow-providers-snowflake-4.4.1/airflow/providers/snowflake/get_provider_info.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 21:35:58.586571 apache-airflow-providers-snowflake-4.4.1/airflow/providers/snowflake/hooks/
--rw-r--r--   0 root         (0) root         (0)      785 2023-06-01 06:14:29.000000 apache-airflow-providers-snowflake-4.4.1/airflow/providers/snowflake/hooks/__init__.py
--rw-r--r--   0 root         (0) root         (0)    21801 2023-07-26 06:59:50.000000 apache-airflow-providers-snowflake-4.4.1/airflow/providers/snowflake/hooks/snowflake.py
--rw-r--r--   0 root         (0) root         (0)    12677 2023-07-09 14:40:47.000000 apache-airflow-providers-snowflake-4.4.1/airflow/providers/snowflake/hooks/snowflake_sql_api.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 21:35:58.592798 apache-airflow-providers-snowflake-4.4.1/airflow/providers/snowflake/operators/
--rw-r--r--   0 root         (0) root         (0)      785 2023-06-01 06:14:29.000000 apache-airflow-providers-snowflake-4.4.1/airflow/providers/snowflake/operators/__init__.py
--rw-r--r--   0 root         (0) root         (0)    25105 2023-08-04 10:24:22.000000 apache-airflow-providers-snowflake-4.4.1/airflow/providers/snowflake/operators/snowflake.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 21:35:58.605546 apache-airflow-providers-snowflake-4.4.1/airflow/providers/snowflake/transfers/
--rw-r--r--   0 root         (0) root         (0)      785 2023-06-01 06:14:29.000000 apache-airflow-providers-snowflake-4.4.1/airflow/providers/snowflake/transfers/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5765 2023-07-09 14:40:47.000000 apache-airflow-providers-snowflake-4.4.1/airflow/providers/snowflake/transfers/copy_into_snowflake.py
--rw-r--r--   0 root         (0) root         (0)     6054 2023-06-02 11:31:21.000000 apache-airflow-providers-snowflake-4.4.1/airflow/providers/snowflake/transfers/s3_to_snowflake.py
--rw-r--r--   0 root         (0) root         (0)     5098 2023-07-26 06:59:50.000000 apache-airflow-providers-snowflake-4.4.1/airflow/providers/snowflake/transfers/snowflake_to_slack.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 21:35:58.612394 apache-airflow-providers-snowflake-4.4.1/airflow/providers/snowflake/triggers/
--rw-r--r--   0 root         (0) root         (0)      785 2023-07-05 07:19:39.000000 apache-airflow-providers-snowflake-4.4.1/airflow/providers/snowflake/triggers/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4186 2023-07-09 14:40:47.000000 apache-airflow-providers-snowflake-4.4.1/airflow/providers/snowflake/triggers/snowflake_trigger.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 21:35:58.621799 apache-airflow-providers-snowflake-4.4.1/airflow/providers/snowflake/utils/
--rw-r--r--   0 root         (0) root         (0)      785 2023-06-01 06:14:29.000000 apache-airflow-providers-snowflake-4.4.1/airflow/providers/snowflake/utils/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1644 2023-06-01 06:14:29.000000 apache-airflow-providers-snowflake-4.4.1/airflow/providers/snowflake/utils/common.py
--rw-r--r--   0 root         (0) root         (0)     6889 2023-07-09 14:40:47.000000 apache-airflow-providers-snowflake-4.4.1/airflow/providers/snowflake/utils/sql_api_generate_jwt.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 21:35:58.648210 apache-airflow-providers-snowflake-4.4.1/apache_airflow_providers_snowflake.egg-info/
--rw-r--r--   0 root         (0) root         (0)     6038 2023-08-04 21:35:58.000000 apache-airflow-providers-snowflake-4.4.1/apache_airflow_providers_snowflake.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1299 2023-08-04 21:35:58.000000 apache-airflow-providers-snowflake-4.4.1/apache_airflow_providers_snowflake.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-08-04 21:35:58.000000 apache-airflow-providers-snowflake-4.4.1/apache_airflow_providers_snowflake.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      106 2023-08-04 21:35:58.000000 apache-airflow-providers-snowflake-4.4.1/apache_airflow_providers_snowflake.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-08-04 21:35:58.000000 apache-airflow-providers-snowflake-4.4.1/apache_airflow_providers_snowflake.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      269 2023-08-04 21:35:58.000000 apache-airflow-providers-snowflake-4.4.1/apache_airflow_providers_snowflake.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-08-04 21:35:58.000000 apache-airflow-providers-snowflake-4.4.1/apache_airflow_providers_snowflake.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     5031 2023-08-04 10:24:23.000000 apache-airflow-providers-snowflake-4.4.1/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)     2046 2023-08-04 21:35:58.653635 apache-airflow-providers-snowflake-4.4.1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1858 2023-08-04 21:35:57.000000 apache-airflow-providers-snowflake-4.4.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 21:41:41.746368 apache-airflow-providers-snowflake-4.4.1rc1/
+-rw-r--r--   0 root         (0) root         (0)    10850 2023-06-01 06:14:29.000000 apache-airflow-providers-snowflake-4.4.1rc1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     1104 2023-08-04 21:41:40.000000 apache-airflow-providers-snowflake-4.4.1rc1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      240 2023-06-01 06:14:29.000000 apache-airflow-providers-snowflake-4.4.1rc1/NOTICE
+-rw-r--r--   0 root         (0) root         (0)     6044 2023-08-04 21:41:41.746964 apache-airflow-providers-snowflake-4.4.1rc1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     4317 2023-08-04 21:41:40.000000 apache-airflow-providers-snowflake-4.4.1rc1/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 21:41:41.641469 apache-airflow-providers-snowflake-4.4.1rc1/airflow/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 21:41:41.642672 apache-airflow-providers-snowflake-4.4.1rc1/airflow/providers/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 21:41:41.678819 apache-airflow-providers-snowflake-4.4.1rc1/airflow/providers/snowflake/
+-rw-r--r--   0 root         (0) root         (0)     1578 2023-08-04 21:33:34.000000 apache-airflow-providers-snowflake-4.4.1rc1/airflow/providers/snowflake/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5012 2023-08-04 21:41:40.000000 apache-airflow-providers-snowflake-4.4.1rc1/airflow/providers/snowflake/get_provider_info.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 21:41:41.687801 apache-airflow-providers-snowflake-4.4.1rc1/airflow/providers/snowflake/hooks/
+-rw-r--r--   0 root         (0) root         (0)      785 2023-06-01 06:14:29.000000 apache-airflow-providers-snowflake-4.4.1rc1/airflow/providers/snowflake/hooks/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    21801 2023-07-26 06:59:50.000000 apache-airflow-providers-snowflake-4.4.1rc1/airflow/providers/snowflake/hooks/snowflake.py
+-rw-r--r--   0 root         (0) root         (0)    12677 2023-07-09 14:40:47.000000 apache-airflow-providers-snowflake-4.4.1rc1/airflow/providers/snowflake/hooks/snowflake_sql_api.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 21:41:41.693593 apache-airflow-providers-snowflake-4.4.1rc1/airflow/providers/snowflake/operators/
+-rw-r--r--   0 root         (0) root         (0)      785 2023-06-01 06:14:29.000000 apache-airflow-providers-snowflake-4.4.1rc1/airflow/providers/snowflake/operators/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    25105 2023-08-04 10:24:22.000000 apache-airflow-providers-snowflake-4.4.1rc1/airflow/providers/snowflake/operators/snowflake.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 21:41:41.705462 apache-airflow-providers-snowflake-4.4.1rc1/airflow/providers/snowflake/transfers/
+-rw-r--r--   0 root         (0) root         (0)      785 2023-06-01 06:14:29.000000 apache-airflow-providers-snowflake-4.4.1rc1/airflow/providers/snowflake/transfers/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5765 2023-07-09 14:40:47.000000 apache-airflow-providers-snowflake-4.4.1rc1/airflow/providers/snowflake/transfers/copy_into_snowflake.py
+-rw-r--r--   0 root         (0) root         (0)     6054 2023-06-02 11:31:21.000000 apache-airflow-providers-snowflake-4.4.1rc1/airflow/providers/snowflake/transfers/s3_to_snowflake.py
+-rw-r--r--   0 root         (0) root         (0)     5098 2023-07-26 06:59:50.000000 apache-airflow-providers-snowflake-4.4.1rc1/airflow/providers/snowflake/transfers/snowflake_to_slack.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 21:41:41.711216 apache-airflow-providers-snowflake-4.4.1rc1/airflow/providers/snowflake/triggers/
+-rw-r--r--   0 root         (0) root         (0)      785 2023-07-05 07:19:39.000000 apache-airflow-providers-snowflake-4.4.1rc1/airflow/providers/snowflake/triggers/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4186 2023-07-09 14:40:47.000000 apache-airflow-providers-snowflake-4.4.1rc1/airflow/providers/snowflake/triggers/snowflake_trigger.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 21:41:41.719766 apache-airflow-providers-snowflake-4.4.1rc1/airflow/providers/snowflake/utils/
+-rw-r--r--   0 root         (0) root         (0)      785 2023-06-01 06:14:29.000000 apache-airflow-providers-snowflake-4.4.1rc1/airflow/providers/snowflake/utils/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1644 2023-06-01 06:14:29.000000 apache-airflow-providers-snowflake-4.4.1rc1/airflow/providers/snowflake/utils/common.py
+-rw-r--r--   0 root         (0) root         (0)     6889 2023-07-09 14:40:47.000000 apache-airflow-providers-snowflake-4.4.1rc1/airflow/providers/snowflake/utils/sql_api_generate_jwt.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 21:41:41.744024 apache-airflow-providers-snowflake-4.4.1rc1/apache_airflow_providers_snowflake.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     6044 2023-08-04 21:41:41.000000 apache-airflow-providers-snowflake-4.4.1rc1/apache_airflow_providers_snowflake.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1299 2023-08-04 21:41:41.000000 apache-airflow-providers-snowflake-4.4.1rc1/apache_airflow_providers_snowflake.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-08-04 21:41:41.000000 apache-airflow-providers-snowflake-4.4.1rc1/apache_airflow_providers_snowflake.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      106 2023-08-04 21:41:41.000000 apache-airflow-providers-snowflake-4.4.1rc1/apache_airflow_providers_snowflake.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-08-04 21:41:41.000000 apache-airflow-providers-snowflake-4.4.1rc1/apache_airflow_providers_snowflake.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      279 2023-08-04 21:41:41.000000 apache-airflow-providers-snowflake-4.4.1rc1/apache_airflow_providers_snowflake.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-08-04 21:41:41.000000 apache-airflow-providers-snowflake-4.4.1rc1/apache_airflow_providers_snowflake.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     5031 2023-08-04 10:24:23.000000 apache-airflow-providers-snowflake-4.4.1rc1/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)     2059 2023-08-04 21:41:41.748769 apache-airflow-providers-snowflake-4.4.1rc1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1858 2023-08-04 21:41:40.000000 apache-airflow-providers-snowflake-4.4.1rc1/setup.py
```

### Comparing `apache-airflow-providers-snowflake-4.4.1/LICENSE` & `apache-airflow-providers-snowflake-4.4.1rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-snowflake-4.4.1/MANIFEST.in` & `apache-airflow-providers-snowflake-4.4.1rc1/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-snowflake-4.4.1/PKG-INFO` & `apache-airflow-providers-snowflake-4.4.1rc1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-snowflake
-Version: 4.4.1
+Version: 4.4.1rc1
 Summary: Provider for Apache Airflow. Implements apache-airflow-providers-snowflake package
 Home-page: https://airflow.apache.org/
 Download-URL: https://archive.apache.org/dist/airflow/providers
 Author: Apache Software Foundation
 Author-email: dev@airflow.apache.org
 License: Apache License 2.0
 Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-snowflake/4.4.1/
@@ -69,15 +69,15 @@
     KIND, either express or implied.  See the License for the
     specific language governing permissions and limitations
     under the License.
 
 
 Package ``apache-airflow-providers-snowflake``
 
-Release: ``4.4.1``
+Release: ``4.4.1rc1``
 
 
 `Snowflake <https://www.snowflake.com/>`__
 
 
 Provider package
 ----------------
```

### Comparing `apache-airflow-providers-snowflake-4.4.1/README.rst` & `apache-airflow-providers-snowflake-4.4.1rc1/README.rst`

 * *Files 0% similar despite different names*

```diff
@@ -32,15 +32,15 @@
     KIND, either express or implied.  See the License for the
     specific language governing permissions and limitations
     under the License.
 
 
 Package ``apache-airflow-providers-snowflake``
 
-Release: ``4.4.1``
+Release: ``4.4.1rc1``
 
 
 `Snowflake <https://www.snowflake.com/>`__
 
 
 Provider package
 ----------------
```

### Comparing `apache-airflow-providers-snowflake-4.4.1/airflow/providers/snowflake/__init__.py` & `apache-airflow-providers-snowflake-4.4.1rc1/airflow/providers/snowflake/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-snowflake-4.4.1/airflow/providers/snowflake/get_provider_info.py` & `apache-airflow-providers-snowflake-4.4.1rc1/airflow/providers/snowflake/get_provider_info.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-snowflake-4.4.1/airflow/providers/snowflake/hooks/__init__.py` & `apache-airflow-providers-snowflake-4.4.1rc1/airflow/providers/snowflake/hooks/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-snowflake-4.4.1/airflow/providers/snowflake/hooks/snowflake.py` & `apache-airflow-providers-snowflake-4.4.1rc1/airflow/providers/snowflake/hooks/snowflake.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-snowflake-4.4.1/airflow/providers/snowflake/hooks/snowflake_sql_api.py` & `apache-airflow-providers-snowflake-4.4.1rc1/airflow/providers/snowflake/hooks/snowflake_sql_api.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-snowflake-4.4.1/airflow/providers/snowflake/operators/__init__.py` & `apache-airflow-providers-snowflake-4.4.1rc1/airflow/providers/snowflake/operators/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-snowflake-4.4.1/airflow/providers/snowflake/operators/snowflake.py` & `apache-airflow-providers-snowflake-4.4.1rc1/airflow/providers/snowflake/operators/snowflake.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-snowflake-4.4.1/airflow/providers/snowflake/transfers/__init__.py` & `apache-airflow-providers-snowflake-4.4.1rc1/airflow/providers/snowflake/transfers/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-snowflake-4.4.1/airflow/providers/snowflake/transfers/copy_into_snowflake.py` & `apache-airflow-providers-snowflake-4.4.1rc1/airflow/providers/snowflake/transfers/copy_into_snowflake.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-snowflake-4.4.1/airflow/providers/snowflake/transfers/s3_to_snowflake.py` & `apache-airflow-providers-snowflake-4.4.1rc1/airflow/providers/snowflake/transfers/s3_to_snowflake.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-snowflake-4.4.1/airflow/providers/snowflake/transfers/snowflake_to_slack.py` & `apache-airflow-providers-snowflake-4.4.1rc1/airflow/providers/snowflake/transfers/snowflake_to_slack.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-snowflake-4.4.1/airflow/providers/snowflake/triggers/__init__.py` & `apache-airflow-providers-snowflake-4.4.1rc1/airflow/providers/snowflake/triggers/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-snowflake-4.4.1/airflow/providers/snowflake/triggers/snowflake_trigger.py` & `apache-airflow-providers-snowflake-4.4.1rc1/airflow/providers/snowflake/triggers/snowflake_trigger.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-snowflake-4.4.1/airflow/providers/snowflake/utils/__init__.py` & `apache-airflow-providers-snowflake-4.4.1rc1/airflow/providers/snowflake/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-snowflake-4.4.1/airflow/providers/snowflake/utils/common.py` & `apache-airflow-providers-snowflake-4.4.1rc1/airflow/providers/snowflake/utils/common.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-snowflake-4.4.1/airflow/providers/snowflake/utils/sql_api_generate_jwt.py` & `apache-airflow-providers-snowflake-4.4.1rc1/airflow/providers/snowflake/utils/sql_api_generate_jwt.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-snowflake-4.4.1/apache_airflow_providers_snowflake.egg-info/PKG-INFO` & `apache-airflow-providers-snowflake-4.4.1rc1/apache_airflow_providers_snowflake.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-snowflake
-Version: 4.4.1
+Version: 4.4.1rc1
 Summary: Provider for Apache Airflow. Implements apache-airflow-providers-snowflake package
 Home-page: https://airflow.apache.org/
 Download-URL: https://archive.apache.org/dist/airflow/providers
 Author: Apache Software Foundation
 Author-email: dev@airflow.apache.org
 License: Apache License 2.0
 Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-snowflake/4.4.1/
@@ -69,15 +69,15 @@
     KIND, either express or implied.  See the License for the
     specific language governing permissions and limitations
     under the License.
 
 
 Package ``apache-airflow-providers-snowflake``
 
-Release: ``4.4.1``
+Release: ``4.4.1rc1``
 
 
 `Snowflake <https://www.snowflake.com/>`__
 
 
 Provider package
 ----------------
```

### Comparing `apache-airflow-providers-snowflake-4.4.1/apache_airflow_providers_snowflake.egg-info/SOURCES.txt` & `apache-airflow-providers-snowflake-4.4.1rc1/apache_airflow_providers_snowflake.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-snowflake-4.4.1/pyproject.toml` & `apache-airflow-providers-snowflake-4.4.1rc1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-snowflake-4.4.1/setup.cfg` & `apache-airflow-providers-snowflake-4.4.1rc1/setup.cfg`

 * *Files 9% similar despite different names*

```diff
@@ -43,23 +43,23 @@
 include_package_data = True
 python_requires = ~=3.8
 packages = find:
 setup_requires = 
 	setuptools
 	wheel
 install_requires = 
-	apache-airflow-providers-common-sql>=1.3.1
-	apache-airflow>=2.4.0
+	apache-airflow-providers-common-sql>=1.3.1.dev0
+	apache-airflow>=2.4.0.dev0
 	snowflake-connector-python>=2.4.1
 	snowflake-sqlalchemy>=1.1.0
 
 [options.entry_points]
 apache_airflow_provider = 
 	provider_info=airflow.providers.snowflake.get_provider_info:get_provider_info
 
 [files]
 packages = airflow.providers.snowflake
 
 [egg_info]
-tag_build = 
+tag_build = rc1
 tag_date = 0
```

### Comparing `apache-airflow-providers-snowflake-4.4.1/setup.py` & `apache-airflow-providers-snowflake-4.4.1rc1/setup.py`

 * *Files identical despite different names*


# Comparing `tmp/apache-airflow-providers-apache-spark-4.1.3.tar.gz` & `tmp/apache-airflow-providers-apache-spark-4.1.3rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apache-airflow-providers-apache-spark-4.1.3.tar", last modified: Fri Aug  4 21:35:06 2023, max compression
+gzip compressed data, was "apache-airflow-providers-apache-spark-4.1.3rc1.tar", last modified: Fri Aug  4 21:40:46 2023, max compression
```

## Comparing `apache-airflow-providers-apache-spark-4.1.3.tar` & `apache-airflow-providers-apache-spark-4.1.3rc1.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 21:35:06.072331 apache-airflow-providers-apache-spark-4.1.3/
--rw-r--r--   0 root         (0) root         (0)    10850 2023-06-01 06:14:29.000000 apache-airflow-providers-apache-spark-4.1.3/LICENSE
--rw-r--r--   0 root         (0) root         (0)     1104 2023-08-04 21:35:04.000000 apache-airflow-providers-apache-spark-4.1.3/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      240 2023-06-01 06:14:29.000000 apache-airflow-providers-apache-spark-4.1.3/NOTICE
--rw-r--r--   0 root         (0) root         (0)     5588 2023-08-04 21:35:06.072861 apache-airflow-providers-apache-spark-4.1.3/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     3897 2023-08-04 21:35:04.000000 apache-airflow-providers-apache-spark-4.1.3/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 21:35:05.988548 apache-airflow-providers-apache-spark-4.1.3/airflow/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 21:35:05.989625 apache-airflow-providers-apache-spark-4.1.3/airflow/providers/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 21:35:05.990644 apache-airflow-providers-apache-spark-4.1.3/airflow/providers/apache/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 21:35:06.021792 apache-airflow-providers-apache-spark-4.1.3/airflow/providers/apache/spark/
--rw-r--r--   0 root         (0) root         (0)     1581 2023-08-04 21:33:34.000000 apache-airflow-providers-apache-spark-4.1.3/airflow/providers/apache/spark/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3709 2023-08-04 21:35:04.000000 apache-airflow-providers-apache-spark-4.1.3/airflow/providers/apache/spark/get_provider_info.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 21:35:06.035702 apache-airflow-providers-apache-spark-4.1.3/airflow/providers/apache/spark/hooks/
--rw-r--r--   0 root         (0) root         (0)      787 2023-06-01 06:14:28.000000 apache-airflow-providers-apache-spark-4.1.3/airflow/providers/apache/spark/hooks/__init__.py
--rw-r--r--   0 root         (0) root         (0)    11492 2023-08-04 10:24:22.000000 apache-airflow-providers-apache-spark-4.1.3/airflow/providers/apache/spark/hooks/spark_jdbc.py
--rw-r--r--   0 root         (0) root         (0)     6753 2023-06-01 07:44:14.000000 apache-airflow-providers-apache-spark-4.1.3/airflow/providers/apache/spark/hooks/spark_jdbc_script.py
--rw-r--r--   0 root         (0) root         (0)     7037 2023-06-29 05:49:30.000000 apache-airflow-providers-apache-spark-4.1.3/airflow/providers/apache/spark/hooks/spark_sql.py
--rw-r--r--   0 root         (0) root         (0)    28687 2023-07-26 06:59:50.000000 apache-airflow-providers-apache-spark-4.1.3/airflow/providers/apache/spark/hooks/spark_submit.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 21:35:06.047187 apache-airflow-providers-apache-spark-4.1.3/airflow/providers/apache/spark/operators/
--rw-r--r--   0 root         (0) root         (0)      787 2023-06-01 06:14:28.000000 apache-airflow-providers-apache-spark-4.1.3/airflow/providers/apache/spark/operators/__init__.py
--rw-r--r--   0 root         (0) root         (0)     9935 2023-06-29 05:49:30.000000 apache-airflow-providers-apache-spark-4.1.3/airflow/providers/apache/spark/operators/spark_jdbc.py
--rw-r--r--   0 root         (0) root         (0)     4508 2023-06-01 07:44:14.000000 apache-airflow-providers-apache-spark-4.1.3/airflow/providers/apache/spark/operators/spark_sql.py
--rw-r--r--   0 root         (0) root         (0)     8370 2023-06-29 05:49:30.000000 apache-airflow-providers-apache-spark-4.1.3/airflow/providers/apache/spark/operators/spark_submit.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 21:35:06.069815 apache-airflow-providers-apache-spark-4.1.3/apache_airflow_providers_apache_spark.egg-info/
--rw-r--r--   0 root         (0) root         (0)     5588 2023-08-04 21:35:05.000000 apache-airflow-providers-apache-spark-4.1.3/apache_airflow_providers_apache_spark.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1074 2023-08-04 21:35:05.000000 apache-airflow-providers-apache-spark-4.1.3/apache_airflow_providers_apache_spark.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-08-04 21:35:05.000000 apache-airflow-providers-apache-spark-4.1.3/apache_airflow_providers_apache_spark.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      109 2023-08-04 21:35:05.000000 apache-airflow-providers-apache-spark-4.1.3/apache_airflow_providers_apache_spark.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-08-04 21:35:05.000000 apache-airflow-providers-apache-spark-4.1.3/apache_airflow_providers_apache_spark.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       97 2023-08-04 21:35:05.000000 apache-airflow-providers-apache-spark-4.1.3/apache_airflow_providers_apache_spark.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-08-04 21:35:05.000000 apache-airflow-providers-apache-spark-4.1.3/apache_airflow_providers_apache_spark.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     5031 2023-08-04 10:24:23.000000 apache-airflow-providers-apache-spark-4.1.3/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)     1968 2023-08-04 21:35:06.074742 apache-airflow-providers-apache-spark-4.1.3/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1744 2023-08-04 21:35:04.000000 apache-airflow-providers-apache-spark-4.1.3/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 21:40:46.135375 apache-airflow-providers-apache-spark-4.1.3rc1/
+-rw-r--r--   0 root         (0) root         (0)    10850 2023-06-01 06:14:29.000000 apache-airflow-providers-apache-spark-4.1.3rc1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     1104 2023-08-04 21:40:45.000000 apache-airflow-providers-apache-spark-4.1.3rc1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      240 2023-06-01 06:14:29.000000 apache-airflow-providers-apache-spark-4.1.3rc1/NOTICE
+-rw-r--r--   0 root         (0) root         (0)     5594 2023-08-04 21:40:46.135906 apache-airflow-providers-apache-spark-4.1.3rc1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     3900 2023-08-04 21:40:45.000000 apache-airflow-providers-apache-spark-4.1.3rc1/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 21:40:46.048141 apache-airflow-providers-apache-spark-4.1.3rc1/airflow/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 21:40:46.049292 apache-airflow-providers-apache-spark-4.1.3rc1/airflow/providers/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 21:40:46.050266 apache-airflow-providers-apache-spark-4.1.3rc1/airflow/providers/apache/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 21:40:46.081304 apache-airflow-providers-apache-spark-4.1.3rc1/airflow/providers/apache/spark/
+-rw-r--r--   0 root         (0) root         (0)     1581 2023-08-04 21:33:34.000000 apache-airflow-providers-apache-spark-4.1.3rc1/airflow/providers/apache/spark/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3709 2023-08-04 21:40:45.000000 apache-airflow-providers-apache-spark-4.1.3rc1/airflow/providers/apache/spark/get_provider_info.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 21:40:46.095656 apache-airflow-providers-apache-spark-4.1.3rc1/airflow/providers/apache/spark/hooks/
+-rw-r--r--   0 root         (0) root         (0)      787 2023-06-01 06:14:28.000000 apache-airflow-providers-apache-spark-4.1.3rc1/airflow/providers/apache/spark/hooks/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    11492 2023-08-04 10:24:22.000000 apache-airflow-providers-apache-spark-4.1.3rc1/airflow/providers/apache/spark/hooks/spark_jdbc.py
+-rw-r--r--   0 root         (0) root         (0)     6753 2023-06-01 07:44:14.000000 apache-airflow-providers-apache-spark-4.1.3rc1/airflow/providers/apache/spark/hooks/spark_jdbc_script.py
+-rw-r--r--   0 root         (0) root         (0)     7037 2023-06-29 05:49:30.000000 apache-airflow-providers-apache-spark-4.1.3rc1/airflow/providers/apache/spark/hooks/spark_sql.py
+-rw-r--r--   0 root         (0) root         (0)    28687 2023-07-26 06:59:50.000000 apache-airflow-providers-apache-spark-4.1.3rc1/airflow/providers/apache/spark/hooks/spark_submit.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 21:40:46.107202 apache-airflow-providers-apache-spark-4.1.3rc1/airflow/providers/apache/spark/operators/
+-rw-r--r--   0 root         (0) root         (0)      787 2023-06-01 06:14:28.000000 apache-airflow-providers-apache-spark-4.1.3rc1/airflow/providers/apache/spark/operators/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     9935 2023-06-29 05:49:30.000000 apache-airflow-providers-apache-spark-4.1.3rc1/airflow/providers/apache/spark/operators/spark_jdbc.py
+-rw-r--r--   0 root         (0) root         (0)     4508 2023-06-01 07:44:14.000000 apache-airflow-providers-apache-spark-4.1.3rc1/airflow/providers/apache/spark/operators/spark_sql.py
+-rw-r--r--   0 root         (0) root         (0)     8370 2023-06-29 05:49:30.000000 apache-airflow-providers-apache-spark-4.1.3rc1/airflow/providers/apache/spark/operators/spark_submit.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 21:40:46.133107 apache-airflow-providers-apache-spark-4.1.3rc1/apache_airflow_providers_apache_spark.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     5594 2023-08-04 21:40:45.000000 apache-airflow-providers-apache-spark-4.1.3rc1/apache_airflow_providers_apache_spark.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1074 2023-08-04 21:40:46.000000 apache-airflow-providers-apache-spark-4.1.3rc1/apache_airflow_providers_apache_spark.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-08-04 21:40:45.000000 apache-airflow-providers-apache-spark-4.1.3rc1/apache_airflow_providers_apache_spark.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      109 2023-08-04 21:40:45.000000 apache-airflow-providers-apache-spark-4.1.3rc1/apache_airflow_providers_apache_spark.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-08-04 21:40:45.000000 apache-airflow-providers-apache-spark-4.1.3rc1/apache_airflow_providers_apache_spark.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      102 2023-08-04 21:40:45.000000 apache-airflow-providers-apache-spark-4.1.3rc1/apache_airflow_providers_apache_spark.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-08-04 21:40:45.000000 apache-airflow-providers-apache-spark-4.1.3rc1/apache_airflow_providers_apache_spark.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     5031 2023-08-04 10:24:23.000000 apache-airflow-providers-apache-spark-4.1.3rc1/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)     1976 2023-08-04 21:40:46.137691 apache-airflow-providers-apache-spark-4.1.3rc1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1744 2023-08-04 21:40:45.000000 apache-airflow-providers-apache-spark-4.1.3rc1/setup.py
```

### Comparing `apache-airflow-providers-apache-spark-4.1.3/LICENSE` & `apache-airflow-providers-apache-spark-4.1.3rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-spark-4.1.3/MANIFEST.in` & `apache-airflow-providers-apache-spark-4.1.3rc1/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-spark-4.1.3/PKG-INFO` & `apache-airflow-providers-apache-spark-4.1.3rc1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-apache-spark
-Version: 4.1.3
+Version: 4.1.3rc1
 Summary: Provider for Apache Airflow. Implements apache-airflow-providers-apache-spark package
 Home-page: https://airflow.apache.org/
 Download-URL: https://archive.apache.org/dist/airflow/providers
 Author: Apache Software Foundation
 Author-email: dev@airflow.apache.org
 License: Apache License 2.0
 Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-apache-spark/4.1.3/
@@ -67,15 +67,15 @@
     KIND, either express or implied.  See the License for the
     specific language governing permissions and limitations
     under the License.
 
 
 Package ``apache-airflow-providers-apache-spark``
 
-Release: ``4.1.3``
+Release: ``4.1.3rc1``
 
 
 `Apache Spark <https://spark.apache.org/>`__
 
 
 Provider package
 ----------------
```

### Comparing `apache-airflow-providers-apache-spark-4.1.3/README.rst` & `apache-airflow-providers-apache-spark-4.1.3rc1/README.rst`

 * *Files 0% similar despite different names*

```diff
@@ -32,15 +32,15 @@
     KIND, either express or implied.  See the License for the
     specific language governing permissions and limitations
     under the License.
 
 
 Package ``apache-airflow-providers-apache-spark``
 
-Release: ``4.1.3``
+Release: ``4.1.3rc1``
 
 
 `Apache Spark <https://spark.apache.org/>`__
 
 
 Provider package
 ----------------
```

### Comparing `apache-airflow-providers-apache-spark-4.1.3/airflow/providers/apache/spark/__init__.py` & `apache-airflow-providers-apache-spark-4.1.3rc1/airflow/providers/apache/spark/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-spark-4.1.3/airflow/providers/apache/spark/get_provider_info.py` & `apache-airflow-providers-apache-spark-4.1.3rc1/airflow/providers/apache/spark/get_provider_info.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-spark-4.1.3/airflow/providers/apache/spark/hooks/__init__.py` & `apache-airflow-providers-apache-spark-4.1.3rc1/airflow/providers/apache/spark/hooks/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-spark-4.1.3/airflow/providers/apache/spark/hooks/spark_jdbc.py` & `apache-airflow-providers-apache-spark-4.1.3rc1/airflow/providers/apache/spark/hooks/spark_jdbc.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-spark-4.1.3/airflow/providers/apache/spark/hooks/spark_jdbc_script.py` & `apache-airflow-providers-apache-spark-4.1.3rc1/airflow/providers/apache/spark/hooks/spark_jdbc_script.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-spark-4.1.3/airflow/providers/apache/spark/hooks/spark_sql.py` & `apache-airflow-providers-apache-spark-4.1.3rc1/airflow/providers/apache/spark/hooks/spark_sql.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-spark-4.1.3/airflow/providers/apache/spark/hooks/spark_submit.py` & `apache-airflow-providers-apache-spark-4.1.3rc1/airflow/providers/apache/spark/hooks/spark_submit.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-spark-4.1.3/airflow/providers/apache/spark/operators/__init__.py` & `apache-airflow-providers-apache-spark-4.1.3rc1/airflow/providers/apache/spark/operators/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-spark-4.1.3/airflow/providers/apache/spark/operators/spark_jdbc.py` & `apache-airflow-providers-apache-spark-4.1.3rc1/airflow/providers/apache/spark/operators/spark_jdbc.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-spark-4.1.3/airflow/providers/apache/spark/operators/spark_sql.py` & `apache-airflow-providers-apache-spark-4.1.3rc1/airflow/providers/apache/spark/operators/spark_sql.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-spark-4.1.3/airflow/providers/apache/spark/operators/spark_submit.py` & `apache-airflow-providers-apache-spark-4.1.3rc1/airflow/providers/apache/spark/operators/spark_submit.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-spark-4.1.3/apache_airflow_providers_apache_spark.egg-info/PKG-INFO` & `apache-airflow-providers-apache-spark-4.1.3rc1/apache_airflow_providers_apache_spark.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-apache-spark
-Version: 4.1.3
+Version: 4.1.3rc1
 Summary: Provider for Apache Airflow. Implements apache-airflow-providers-apache-spark package
 Home-page: https://airflow.apache.org/
 Download-URL: https://archive.apache.org/dist/airflow/providers
 Author: Apache Software Foundation
 Author-email: dev@airflow.apache.org
 License: Apache License 2.0
 Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-apache-spark/4.1.3/
@@ -67,15 +67,15 @@
     KIND, either express or implied.  See the License for the
     specific language governing permissions and limitations
     under the License.
 
 
 Package ``apache-airflow-providers-apache-spark``
 
-Release: ``4.1.3``
+Release: ``4.1.3rc1``
 
 
 `Apache Spark <https://spark.apache.org/>`__
 
 
 Provider package
 ----------------
```

### Comparing `apache-airflow-providers-apache-spark-4.1.3/apache_airflow_providers_apache_spark.egg-info/SOURCES.txt` & `apache-airflow-providers-apache-spark-4.1.3rc1/apache_airflow_providers_apache_spark.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-spark-4.1.3/pyproject.toml` & `apache-airflow-providers-apache-spark-4.1.3rc1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-spark-4.1.3/setup.cfg` & `apache-airflow-providers-apache-spark-4.1.3rc1/setup.cfg`

 * *Files 4% similar despite different names*

```diff
@@ -43,21 +43,21 @@
 include_package_data = True
 python_requires = ~=3.8
 packages = find:
 setup_requires = 
 	setuptools
 	wheel
 install_requires = 
-	apache-airflow>=2.4.0
+	apache-airflow>=2.4.0.dev0
 	pyspark
 
 [options.entry_points]
 apache_airflow_provider = 
 	provider_info=airflow.providers.apache.spark.get_provider_info:get_provider_info
 
 [files]
 packages = airflow.providers.apache.spark
 
 [egg_info]
-tag_build = 
+tag_build = rc1
 tag_date = 0
```

### Comparing `apache-airflow-providers-apache-spark-4.1.3/setup.py` & `apache-airflow-providers-apache-spark-4.1.3rc1/setup.py`

 * *Files identical despite different names*


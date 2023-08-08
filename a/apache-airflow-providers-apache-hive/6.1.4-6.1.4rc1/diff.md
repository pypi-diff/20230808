# Comparing `tmp/apache-airflow-providers-apache-hive-6.1.4.tar.gz` & `tmp/apache-airflow-providers-apache-hive-6.1.4rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apache-airflow-providers-apache-hive-6.1.4.tar", last modified: Fri Aug  4 21:35:01 2023, max compression
+gzip compressed data, was "apache-airflow-providers-apache-hive-6.1.4rc1.tar", last modified: Fri Aug  4 21:40:40 2023, max compression
```

## Comparing `apache-airflow-providers-apache-hive-6.1.4.tar` & `apache-airflow-providers-apache-hive-6.1.4rc1.tar`

### file list

```diff
@@ -1,49 +1,49 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 21:35:01.409795 apache-airflow-providers-apache-hive-6.1.4/
--rw-r--r--   0 root         (0) root         (0)    10850 2023-06-01 06:14:29.000000 apache-airflow-providers-apache-hive-6.1.4/LICENSE
--rw-r--r--   0 root         (0) root         (0)     1104 2023-08-04 21:35:00.000000 apache-airflow-providers-apache-hive-6.1.4/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      240 2023-06-01 06:14:29.000000 apache-airflow-providers-apache-hive-6.1.4/NOTICE
--rw-r--r--   0 root         (0) root         (0)     6923 2023-08-04 21:35:01.410307 apache-airflow-providers-apache-hive-6.1.4/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     5146 2023-08-04 21:35:00.000000 apache-airflow-providers-apache-hive-6.1.4/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 21:35:01.285075 apache-airflow-providers-apache-hive-6.1.4/airflow/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 21:35:01.286190 apache-airflow-providers-apache-hive-6.1.4/airflow/providers/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 21:35:01.287164 apache-airflow-providers-apache-hive-6.1.4/airflow/providers/apache/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 21:35:01.324664 apache-airflow-providers-apache-hive-6.1.4/airflow/providers/apache/hive/
--rw-r--r--   0 root         (0) root         (0)     1580 2023-08-04 21:33:34.000000 apache-airflow-providers-apache-hive-6.1.4/airflow/providers/apache/hive/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6634 2023-08-04 21:35:00.000000 apache-airflow-providers-apache-hive-6.1.4/airflow/providers/apache/hive/get_provider_info.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 21:35:01.330296 apache-airflow-providers-apache-hive-6.1.4/airflow/providers/apache/hive/hooks/
--rw-r--r--   0 root         (0) root         (0)      787 2023-06-01 06:14:28.000000 apache-airflow-providers-apache-hive-6.1.4/airflow/providers/apache/hive/hooks/__init__.py
--rw-r--r--   0 root         (0) root         (0)    42466 2023-07-26 06:59:50.000000 apache-airflow-providers-apache-hive-6.1.4/airflow/providers/apache/hive/hooks/hive.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 21:35:01.336751 apache-airflow-providers-apache-hive-6.1.4/airflow/providers/apache/hive/macros/
--rw-r--r--   0 root         (0) root         (0)      787 2023-06-01 06:14:28.000000 apache-airflow-providers-apache-hive-6.1.4/airflow/providers/apache/hive/macros/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4583 2023-06-29 05:49:30.000000 apache-airflow-providers-apache-hive-6.1.4/airflow/providers/apache/hive/macros/hive.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 21:35:01.345280 apache-airflow-providers-apache-hive-6.1.4/airflow/providers/apache/hive/operators/
--rw-r--r--   0 root         (0) root         (0)      787 2023-06-01 06:14:28.000000 apache-airflow-providers-apache-hive-6.1.4/airflow/providers/apache/hive/operators/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7384 2023-06-01 07:44:14.000000 apache-airflow-providers-apache-hive-6.1.4/airflow/providers/apache/hive/operators/hive.py
--rw-r--r--   0 root         (0) root         (0)     7502 2023-06-08 05:42:54.000000 apache-airflow-providers-apache-hive-6.1.4/airflow/providers/apache/hive/operators/hive_stats.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 21:35:01.350941 apache-airflow-providers-apache-hive-6.1.4/airflow/providers/apache/hive/plugins/
--rw-r--r--   0 root         (0) root         (0)      787 2023-06-01 06:14:28.000000 apache-airflow-providers-apache-hive-6.1.4/airflow/providers/apache/hive/plugins/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1146 2023-06-01 06:14:28.000000 apache-airflow-providers-apache-hive-6.1.4/airflow/providers/apache/hive/plugins/hive.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 21:35:01.362318 apache-airflow-providers-apache-hive-6.1.4/airflow/providers/apache/hive/sensors/
--rw-r--r--   0 root         (0) root         (0)      787 2023-06-01 06:14:28.000000 apache-airflow-providers-apache-hive-6.1.4/airflow/providers/apache/hive/sensors/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3039 2023-06-01 06:14:28.000000 apache-airflow-providers-apache-hive-6.1.4/airflow/providers/apache/hive/sensors/hive_partition.py
--rw-r--r--   0 root         (0) root         (0)     3386 2023-06-29 05:49:30.000000 apache-airflow-providers-apache-hive-6.1.4/airflow/providers/apache/hive/sensors/metastore_partition.py
--rw-r--r--   0 root         (0) root         (0)     4159 2023-06-01 06:14:28.000000 apache-airflow-providers-apache-hive-6.1.4/airflow/providers/apache/hive/sensors/named_hive_partition.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 21:35:01.382160 apache-airflow-providers-apache-hive-6.1.4/airflow/providers/apache/hive/transfers/
--rw-r--r--   0 root         (0) root         (0)      785 2023-06-01 06:14:28.000000 apache-airflow-providers-apache-hive-6.1.4/airflow/providers/apache/hive/transfers/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5280 2023-06-29 05:49:30.000000 apache-airflow-providers-apache-hive-6.1.4/airflow/providers/apache/hive/transfers/hive_to_mysql.py
--rw-r--r--   0 root         (0) root         (0)     2954 2023-06-29 05:49:30.000000 apache-airflow-providers-apache-hive-6.1.4/airflow/providers/apache/hive/transfers/hive_to_samba.py
--rw-r--r--   0 root         (0) root         (0)     5664 2023-06-29 05:49:30.000000 apache-airflow-providers-apache-hive-6.1.4/airflow/providers/apache/hive/transfers/mssql_to_hive.py
--rw-r--r--   0 root         (0) root         (0)     6745 2023-08-04 19:44:14.000000 apache-airflow-providers-apache-hive-6.1.4/airflow/providers/apache/hive/transfers/mysql_to_hive.py
--rw-r--r--   0 root         (0) root         (0)    11748 2023-06-29 05:49:30.000000 apache-airflow-providers-apache-hive-6.1.4/airflow/providers/apache/hive/transfers/s3_to_hive.py
--rw-r--r--   0 root         (0) root         (0)     5565 2023-06-29 05:49:30.000000 apache-airflow-providers-apache-hive-6.1.4/airflow/providers/apache/hive/transfers/vertica_to_hive.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 21:35:01.407565 apache-airflow-providers-apache-hive-6.1.4/apache_airflow_providers_apache_hive.egg-info/
--rw-r--r--   0 root         (0) root         (0)     6923 2023-08-04 21:35:01.000000 apache-airflow-providers-apache-hive-6.1.4/apache_airflow_providers_apache_hive.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1643 2023-08-04 21:35:01.000000 apache-airflow-providers-apache-hive-6.1.4/apache_airflow_providers_apache_hive.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-08-04 21:35:01.000000 apache-airflow-providers-apache-hive-6.1.4/apache_airflow_providers_apache_hive.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      188 2023-08-04 21:35:01.000000 apache-airflow-providers-apache-hive-6.1.4/apache_airflow_providers_apache_hive.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-08-04 21:35:01.000000 apache-airflow-providers-apache-hive-6.1.4/apache_airflow_providers_apache_hive.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      489 2023-08-04 21:35:01.000000 apache-airflow-providers-apache-hive-6.1.4/apache_airflow_providers_apache_hive.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-08-04 21:35:01.000000 apache-airflow-providers-apache-hive-6.1.4/apache_airflow_providers_apache_hive.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     5031 2023-08-04 10:24:23.000000 apache-airflow-providers-apache-hive-6.1.4/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)     2141 2023-08-04 21:35:01.412140 apache-airflow-providers-apache-hive-6.1.4/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2114 2023-08-04 21:35:00.000000 apache-airflow-providers-apache-hive-6.1.4/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 21:40:40.974183 apache-airflow-providers-apache-hive-6.1.4rc1/
+-rw-r--r--   0 root         (0) root         (0)    10850 2023-06-01 06:14:29.000000 apache-airflow-providers-apache-hive-6.1.4rc1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     1104 2023-08-04 21:40:39.000000 apache-airflow-providers-apache-hive-6.1.4rc1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      240 2023-06-01 06:14:29.000000 apache-airflow-providers-apache-hive-6.1.4rc1/NOTICE
+-rw-r--r--   0 root         (0) root         (0)     6929 2023-08-04 21:40:40.974795 apache-airflow-providers-apache-hive-6.1.4rc1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     5149 2023-08-04 21:40:39.000000 apache-airflow-providers-apache-hive-6.1.4rc1/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 21:40:40.839728 apache-airflow-providers-apache-hive-6.1.4rc1/airflow/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 21:40:40.840782 apache-airflow-providers-apache-hive-6.1.4rc1/airflow/providers/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 21:40:40.841891 apache-airflow-providers-apache-hive-6.1.4rc1/airflow/providers/apache/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 21:40:40.883142 apache-airflow-providers-apache-hive-6.1.4rc1/airflow/providers/apache/hive/
+-rw-r--r--   0 root         (0) root         (0)     1580 2023-08-04 21:33:34.000000 apache-airflow-providers-apache-hive-6.1.4rc1/airflow/providers/apache/hive/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6634 2023-08-04 21:40:39.000000 apache-airflow-providers-apache-hive-6.1.4rc1/airflow/providers/apache/hive/get_provider_info.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 21:40:40.890655 apache-airflow-providers-apache-hive-6.1.4rc1/airflow/providers/apache/hive/hooks/
+-rw-r--r--   0 root         (0) root         (0)      787 2023-06-01 06:14:28.000000 apache-airflow-providers-apache-hive-6.1.4rc1/airflow/providers/apache/hive/hooks/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    42466 2023-07-26 06:59:50.000000 apache-airflow-providers-apache-hive-6.1.4rc1/airflow/providers/apache/hive/hooks/hive.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 21:40:40.897712 apache-airflow-providers-apache-hive-6.1.4rc1/airflow/providers/apache/hive/macros/
+-rw-r--r--   0 root         (0) root         (0)      787 2023-06-01 06:14:28.000000 apache-airflow-providers-apache-hive-6.1.4rc1/airflow/providers/apache/hive/macros/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4583 2023-06-29 05:49:30.000000 apache-airflow-providers-apache-hive-6.1.4rc1/airflow/providers/apache/hive/macros/hive.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 21:40:40.907736 apache-airflow-providers-apache-hive-6.1.4rc1/airflow/providers/apache/hive/operators/
+-rw-r--r--   0 root         (0) root         (0)      787 2023-06-01 06:14:28.000000 apache-airflow-providers-apache-hive-6.1.4rc1/airflow/providers/apache/hive/operators/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7384 2023-06-01 07:44:14.000000 apache-airflow-providers-apache-hive-6.1.4rc1/airflow/providers/apache/hive/operators/hive.py
+-rw-r--r--   0 root         (0) root         (0)     7502 2023-06-08 05:42:54.000000 apache-airflow-providers-apache-hive-6.1.4rc1/airflow/providers/apache/hive/operators/hive_stats.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 21:40:40.913688 apache-airflow-providers-apache-hive-6.1.4rc1/airflow/providers/apache/hive/plugins/
+-rw-r--r--   0 root         (0) root         (0)      787 2023-06-01 06:14:28.000000 apache-airflow-providers-apache-hive-6.1.4rc1/airflow/providers/apache/hive/plugins/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1146 2023-06-01 06:14:28.000000 apache-airflow-providers-apache-hive-6.1.4rc1/airflow/providers/apache/hive/plugins/hive.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 21:40:40.926473 apache-airflow-providers-apache-hive-6.1.4rc1/airflow/providers/apache/hive/sensors/
+-rw-r--r--   0 root         (0) root         (0)      787 2023-06-01 06:14:28.000000 apache-airflow-providers-apache-hive-6.1.4rc1/airflow/providers/apache/hive/sensors/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3039 2023-06-01 06:14:28.000000 apache-airflow-providers-apache-hive-6.1.4rc1/airflow/providers/apache/hive/sensors/hive_partition.py
+-rw-r--r--   0 root         (0) root         (0)     3386 2023-06-29 05:49:30.000000 apache-airflow-providers-apache-hive-6.1.4rc1/airflow/providers/apache/hive/sensors/metastore_partition.py
+-rw-r--r--   0 root         (0) root         (0)     4159 2023-06-01 06:14:28.000000 apache-airflow-providers-apache-hive-6.1.4rc1/airflow/providers/apache/hive/sensors/named_hive_partition.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 21:40:40.947061 apache-airflow-providers-apache-hive-6.1.4rc1/airflow/providers/apache/hive/transfers/
+-rw-r--r--   0 root         (0) root         (0)      785 2023-06-01 06:14:28.000000 apache-airflow-providers-apache-hive-6.1.4rc1/airflow/providers/apache/hive/transfers/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5280 2023-06-29 05:49:30.000000 apache-airflow-providers-apache-hive-6.1.4rc1/airflow/providers/apache/hive/transfers/hive_to_mysql.py
+-rw-r--r--   0 root         (0) root         (0)     2954 2023-06-29 05:49:30.000000 apache-airflow-providers-apache-hive-6.1.4rc1/airflow/providers/apache/hive/transfers/hive_to_samba.py
+-rw-r--r--   0 root         (0) root         (0)     5664 2023-06-29 05:49:30.000000 apache-airflow-providers-apache-hive-6.1.4rc1/airflow/providers/apache/hive/transfers/mssql_to_hive.py
+-rw-r--r--   0 root         (0) root         (0)     6745 2023-08-04 19:44:14.000000 apache-airflow-providers-apache-hive-6.1.4rc1/airflow/providers/apache/hive/transfers/mysql_to_hive.py
+-rw-r--r--   0 root         (0) root         (0)    11748 2023-06-29 05:49:30.000000 apache-airflow-providers-apache-hive-6.1.4rc1/airflow/providers/apache/hive/transfers/s3_to_hive.py
+-rw-r--r--   0 root         (0) root         (0)     5565 2023-06-29 05:49:30.000000 apache-airflow-providers-apache-hive-6.1.4rc1/airflow/providers/apache/hive/transfers/vertica_to_hive.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 21:40:40.971361 apache-airflow-providers-apache-hive-6.1.4rc1/apache_airflow_providers_apache_hive.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     6929 2023-08-04 21:40:40.000000 apache-airflow-providers-apache-hive-6.1.4rc1/apache_airflow_providers_apache_hive.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1643 2023-08-04 21:40:40.000000 apache-airflow-providers-apache-hive-6.1.4rc1/apache_airflow_providers_apache_hive.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-08-04 21:40:40.000000 apache-airflow-providers-apache-hive-6.1.4rc1/apache_airflow_providers_apache_hive.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      188 2023-08-04 21:40:40.000000 apache-airflow-providers-apache-hive-6.1.4rc1/apache_airflow_providers_apache_hive.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-08-04 21:40:40.000000 apache-airflow-providers-apache-hive-6.1.4rc1/apache_airflow_providers_apache_hive.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      499 2023-08-04 21:40:40.000000 apache-airflow-providers-apache-hive-6.1.4rc1/apache_airflow_providers_apache_hive.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-08-04 21:40:40.000000 apache-airflow-providers-apache-hive-6.1.4rc1/apache_airflow_providers_apache_hive.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     5031 2023-08-04 10:24:23.000000 apache-airflow-providers-apache-hive-6.1.4rc1/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)     2154 2023-08-04 21:40:40.976727 apache-airflow-providers-apache-hive-6.1.4rc1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2114 2023-08-04 21:40:39.000000 apache-airflow-providers-apache-hive-6.1.4rc1/setup.py
```

### Comparing `apache-airflow-providers-apache-hive-6.1.4/LICENSE` & `apache-airflow-providers-apache-hive-6.1.4rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-hive-6.1.4/MANIFEST.in` & `apache-airflow-providers-apache-hive-6.1.4rc1/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-hive-6.1.4/PKG-INFO` & `apache-airflow-providers-apache-hive-6.1.4rc1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-apache-hive
-Version: 6.1.4
+Version: 6.1.4rc1
 Summary: Provider for Apache Airflow. Implements apache-airflow-providers-apache-hive package
 Home-page: https://airflow.apache.org/
 Download-URL: https://archive.apache.org/dist/airflow/providers
 Author: Apache Software Foundation
 Author-email: dev@airflow.apache.org
 License: Apache License 2.0
 Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-apache-hive/6.1.4/
@@ -72,15 +72,15 @@
     KIND, either express or implied.  See the License for the
     specific language governing permissions and limitations
     under the License.
 
 
 Package ``apache-airflow-providers-apache-hive``
 
-Release: ``6.1.4``
+Release: ``6.1.4rc1``
 
 
 `Apache Hive <https://hive.apache.org/>`__
 
 
 Provider package
 ----------------
```

### Comparing `apache-airflow-providers-apache-hive-6.1.4/README.rst` & `apache-airflow-providers-apache-hive-6.1.4rc1/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -32,15 +32,15 @@
     KIND, either express or implied.  See the License for the
     specific language governing permissions and limitations
     under the License.
 
 
 Package ``apache-airflow-providers-apache-hive``
 
-Release: ``6.1.4``
+Release: ``6.1.4rc1``
 
 
 `Apache Hive <https://hive.apache.org/>`__
 
 
 Provider package
 ----------------
```

### Comparing `apache-airflow-providers-apache-hive-6.1.4/airflow/providers/apache/hive/__init__.py` & `apache-airflow-providers-apache-hive-6.1.4rc1/airflow/providers/apache/hive/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-hive-6.1.4/airflow/providers/apache/hive/get_provider_info.py` & `apache-airflow-providers-apache-hive-6.1.4rc1/airflow/providers/apache/hive/get_provider_info.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-hive-6.1.4/airflow/providers/apache/hive/hooks/__init__.py` & `apache-airflow-providers-apache-hive-6.1.4rc1/airflow/providers/apache/hive/hooks/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-hive-6.1.4/airflow/providers/apache/hive/hooks/hive.py` & `apache-airflow-providers-apache-hive-6.1.4rc1/airflow/providers/apache/hive/hooks/hive.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-hive-6.1.4/airflow/providers/apache/hive/macros/__init__.py` & `apache-airflow-providers-apache-hive-6.1.4rc1/airflow/providers/apache/hive/macros/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-hive-6.1.4/airflow/providers/apache/hive/macros/hive.py` & `apache-airflow-providers-apache-hive-6.1.4rc1/airflow/providers/apache/hive/macros/hive.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-hive-6.1.4/airflow/providers/apache/hive/operators/__init__.py` & `apache-airflow-providers-apache-hive-6.1.4rc1/airflow/providers/apache/hive/operators/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-hive-6.1.4/airflow/providers/apache/hive/operators/hive.py` & `apache-airflow-providers-apache-hive-6.1.4rc1/airflow/providers/apache/hive/operators/hive.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-hive-6.1.4/airflow/providers/apache/hive/operators/hive_stats.py` & `apache-airflow-providers-apache-hive-6.1.4rc1/airflow/providers/apache/hive/operators/hive_stats.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-hive-6.1.4/airflow/providers/apache/hive/plugins/__init__.py` & `apache-airflow-providers-apache-hive-6.1.4rc1/airflow/providers/apache/hive/plugins/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-hive-6.1.4/airflow/providers/apache/hive/plugins/hive.py` & `apache-airflow-providers-apache-hive-6.1.4rc1/airflow/providers/apache/hive/plugins/hive.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-hive-6.1.4/airflow/providers/apache/hive/sensors/__init__.py` & `apache-airflow-providers-apache-hive-6.1.4rc1/airflow/providers/apache/hive/sensors/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-hive-6.1.4/airflow/providers/apache/hive/sensors/hive_partition.py` & `apache-airflow-providers-apache-hive-6.1.4rc1/airflow/providers/apache/hive/sensors/hive_partition.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-hive-6.1.4/airflow/providers/apache/hive/sensors/metastore_partition.py` & `apache-airflow-providers-apache-hive-6.1.4rc1/airflow/providers/apache/hive/sensors/metastore_partition.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-hive-6.1.4/airflow/providers/apache/hive/sensors/named_hive_partition.py` & `apache-airflow-providers-apache-hive-6.1.4rc1/airflow/providers/apache/hive/sensors/named_hive_partition.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-hive-6.1.4/airflow/providers/apache/hive/transfers/__init__.py` & `apache-airflow-providers-apache-hive-6.1.4rc1/airflow/providers/apache/hive/transfers/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-hive-6.1.4/airflow/providers/apache/hive/transfers/hive_to_mysql.py` & `apache-airflow-providers-apache-hive-6.1.4rc1/airflow/providers/apache/hive/transfers/hive_to_mysql.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-hive-6.1.4/airflow/providers/apache/hive/transfers/hive_to_samba.py` & `apache-airflow-providers-apache-hive-6.1.4rc1/airflow/providers/apache/hive/transfers/hive_to_samba.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-hive-6.1.4/airflow/providers/apache/hive/transfers/mssql_to_hive.py` & `apache-airflow-providers-apache-hive-6.1.4rc1/airflow/providers/apache/hive/transfers/mssql_to_hive.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-hive-6.1.4/airflow/providers/apache/hive/transfers/mysql_to_hive.py` & `apache-airflow-providers-apache-hive-6.1.4rc1/airflow/providers/apache/hive/transfers/mysql_to_hive.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-hive-6.1.4/airflow/providers/apache/hive/transfers/s3_to_hive.py` & `apache-airflow-providers-apache-hive-6.1.4rc1/airflow/providers/apache/hive/transfers/s3_to_hive.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-hive-6.1.4/airflow/providers/apache/hive/transfers/vertica_to_hive.py` & `apache-airflow-providers-apache-hive-6.1.4rc1/airflow/providers/apache/hive/transfers/vertica_to_hive.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-hive-6.1.4/apache_airflow_providers_apache_hive.egg-info/PKG-INFO` & `apache-airflow-providers-apache-hive-6.1.4rc1/apache_airflow_providers_apache_hive.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-apache-hive
-Version: 6.1.4
+Version: 6.1.4rc1
 Summary: Provider for Apache Airflow. Implements apache-airflow-providers-apache-hive package
 Home-page: https://airflow.apache.org/
 Download-URL: https://archive.apache.org/dist/airflow/providers
 Author: Apache Software Foundation
 Author-email: dev@airflow.apache.org
 License: Apache License 2.0
 Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-apache-hive/6.1.4/
@@ -72,15 +72,15 @@
     KIND, either express or implied.  See the License for the
     specific language governing permissions and limitations
     under the License.
 
 
 Package ``apache-airflow-providers-apache-hive``
 
-Release: ``6.1.4``
+Release: ``6.1.4rc1``
 
 
 `Apache Hive <https://hive.apache.org/>`__
 
 
 Provider package
 ----------------
```

### Comparing `apache-airflow-providers-apache-hive-6.1.4/apache_airflow_providers_apache_hive.egg-info/SOURCES.txt` & `apache-airflow-providers-apache-hive-6.1.4rc1/apache_airflow_providers_apache_hive.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-hive-6.1.4/pyproject.toml` & `apache-airflow-providers-apache-hive-6.1.4rc1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-hive-6.1.4/setup.cfg` & `apache-airflow-providers-apache-hive-6.1.4rc1/setup.cfg`

 * *Files 5% similar despite different names*

```diff
@@ -42,16 +42,16 @@
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
 	hmsclient>=0.1.0
 	pandas>=0.17.1
 	pyhive[hive]>=0.6.0
 	sasl>=0.3.1; python_version>="3.9"
 	thrift>=0.9.2
 
 [options.entry_points]
@@ -60,10 +60,10 @@
 airflow.plugins = 
 	hive=airflow.providers.apache.hive.plugins.hive:HivePlugin
 
 [files]
 packages = airflow.providers.apache.hive
 
 [egg_info]
-tag_build = 
+tag_build = rc1
 tag_date = 0
```

### Comparing `apache-airflow-providers-apache-hive-6.1.4/setup.py` & `apache-airflow-providers-apache-hive-6.1.4rc1/setup.py`

 * *Files identical despite different names*


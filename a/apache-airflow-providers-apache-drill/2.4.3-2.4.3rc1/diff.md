# Comparing `tmp/apache-airflow-providers-apache-drill-2.4.3.tar.gz` & `tmp/apache-airflow-providers-apache-drill-2.4.3rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apache-airflow-providers-apache-drill-2.4.3.tar", last modified: Fri Aug  4 21:34:58 2023, max compression
+gzip compressed data, was "apache-airflow-providers-apache-drill-2.4.3rc1.tar", last modified: Fri Aug  4 21:40:37 2023, max compression
```

## Comparing `apache-airflow-providers-apache-drill-2.4.3.tar` & `apache-airflow-providers-apache-drill-2.4.3rc1.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 21:34:58.152150 apache-airflow-providers-apache-drill-2.4.3/
--rw-r--r--   0 root         (0) root         (0)    10850 2023-06-01 06:14:29.000000 apache-airflow-providers-apache-drill-2.4.3/LICENSE
--rw-r--r--   0 root         (0) root         (0)     1104 2023-08-04 21:34:57.000000 apache-airflow-providers-apache-drill-2.4.3/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      240 2023-06-01 06:14:29.000000 apache-airflow-providers-apache-drill-2.4.3/NOTICE
--rw-r--r--   0 root         (0) root         (0)     5708 2023-08-04 21:34:58.152748 apache-airflow-providers-apache-drill-2.4.3/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     4022 2023-08-04 21:34:57.000000 apache-airflow-providers-apache-drill-2.4.3/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 21:34:58.082029 apache-airflow-providers-apache-drill-2.4.3/airflow/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 21:34:58.083162 apache-airflow-providers-apache-drill-2.4.3/airflow/providers/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 21:34:58.084213 apache-airflow-providers-apache-drill-2.4.3/airflow/providers/apache/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 21:34:58.115605 apache-airflow-providers-apache-drill-2.4.3/airflow/providers/apache/drill/
--rw-r--r--   0 root         (0) root         (0)     1581 2023-08-04 21:33:34.000000 apache-airflow-providers-apache-drill-2.4.3/airflow/providers/apache/drill/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2778 2023-08-04 21:34:56.000000 apache-airflow-providers-apache-drill-2.4.3/airflow/providers/apache/drill/get_provider_info.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 21:34:58.121339 apache-airflow-providers-apache-drill-2.4.3/airflow/providers/apache/drill/hooks/
--rw-r--r--   0 root         (0) root         (0)      787 2023-06-01 06:14:28.000000 apache-airflow-providers-apache-drill-2.4.3/airflow/providers/apache/drill/hooks/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4149 2023-08-04 10:24:22.000000 apache-airflow-providers-apache-drill-2.4.3/airflow/providers/apache/drill/hooks/drill.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 21:34:58.126956 apache-airflow-providers-apache-drill-2.4.3/airflow/providers/apache/drill/operators/
--rw-r--r--   0 root         (0) root         (0)      787 2023-06-01 06:14:28.000000 apache-airflow-providers-apache-drill-2.4.3/airflow/providers/apache/drill/operators/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2346 2023-07-16 17:25:26.000000 apache-airflow-providers-apache-drill-2.4.3/airflow/providers/apache/drill/operators/drill.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 21:34:58.149487 apache-airflow-providers-apache-drill-2.4.3/apache_airflow_providers_apache_drill.egg-info/
--rw-r--r--   0 root         (0) root         (0)     5708 2023-08-04 21:34:58.000000 apache-airflow-providers-apache-drill-2.4.3/apache_airflow_providers_apache_drill.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      792 2023-08-04 21:34:58.000000 apache-airflow-providers-apache-drill-2.4.3/apache_airflow_providers_apache_drill.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-08-04 21:34:58.000000 apache-airflow-providers-apache-drill-2.4.3/apache_airflow_providers_apache_drill.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      109 2023-08-04 21:34:58.000000 apache-airflow-providers-apache-drill-2.4.3/apache_airflow_providers_apache_drill.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-08-04 21:34:58.000000 apache-airflow-providers-apache-drill-2.4.3/apache_airflow_providers_apache_drill.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      139 2023-08-04 21:34:58.000000 apache-airflow-providers-apache-drill-2.4.3/apache_airflow_providers_apache_drill.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-08-04 21:34:58.000000 apache-airflow-providers-apache-drill-2.4.3/apache_airflow_providers_apache_drill.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     5031 2023-08-04 10:24:23.000000 apache-airflow-providers-apache-drill-2.4.3/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)     2028 2023-08-04 21:34:58.154638 apache-airflow-providers-apache-drill-2.4.3/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1727 2023-08-04 21:34:56.000000 apache-airflow-providers-apache-drill-2.4.3/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 21:40:37.478341 apache-airflow-providers-apache-drill-2.4.3rc1/
+-rw-r--r--   0 root         (0) root         (0)    10850 2023-06-01 06:14:29.000000 apache-airflow-providers-apache-drill-2.4.3rc1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     1104 2023-08-04 21:40:36.000000 apache-airflow-providers-apache-drill-2.4.3rc1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      240 2023-06-01 06:14:29.000000 apache-airflow-providers-apache-drill-2.4.3rc1/NOTICE
+-rw-r--r--   0 root         (0) root         (0)     5714 2023-08-04 21:40:37.478901 apache-airflow-providers-apache-drill-2.4.3rc1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     4025 2023-08-04 21:40:36.000000 apache-airflow-providers-apache-drill-2.4.3rc1/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 21:40:37.380637 apache-airflow-providers-apache-drill-2.4.3rc1/airflow/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 21:40:37.381959 apache-airflow-providers-apache-drill-2.4.3rc1/airflow/providers/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 21:40:37.383293 apache-airflow-providers-apache-drill-2.4.3rc1/airflow/providers/apache/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 21:40:37.430619 apache-airflow-providers-apache-drill-2.4.3rc1/airflow/providers/apache/drill/
+-rw-r--r--   0 root         (0) root         (0)     1581 2023-08-04 21:33:34.000000 apache-airflow-providers-apache-drill-2.4.3rc1/airflow/providers/apache/drill/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2778 2023-08-04 21:40:36.000000 apache-airflow-providers-apache-drill-2.4.3rc1/airflow/providers/apache/drill/get_provider_info.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 21:40:37.438827 apache-airflow-providers-apache-drill-2.4.3rc1/airflow/providers/apache/drill/hooks/
+-rw-r--r--   0 root         (0) root         (0)      787 2023-06-01 06:14:28.000000 apache-airflow-providers-apache-drill-2.4.3rc1/airflow/providers/apache/drill/hooks/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4149 2023-08-04 10:24:22.000000 apache-airflow-providers-apache-drill-2.4.3rc1/airflow/providers/apache/drill/hooks/drill.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 21:40:37.445840 apache-airflow-providers-apache-drill-2.4.3rc1/airflow/providers/apache/drill/operators/
+-rw-r--r--   0 root         (0) root         (0)      787 2023-06-01 06:14:28.000000 apache-airflow-providers-apache-drill-2.4.3rc1/airflow/providers/apache/drill/operators/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2346 2023-07-16 17:25:26.000000 apache-airflow-providers-apache-drill-2.4.3rc1/airflow/providers/apache/drill/operators/drill.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 21:40:37.475566 apache-airflow-providers-apache-drill-2.4.3rc1/apache_airflow_providers_apache_drill.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     5714 2023-08-04 21:40:37.000000 apache-airflow-providers-apache-drill-2.4.3rc1/apache_airflow_providers_apache_drill.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      792 2023-08-04 21:40:37.000000 apache-airflow-providers-apache-drill-2.4.3rc1/apache_airflow_providers_apache_drill.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-08-04 21:40:37.000000 apache-airflow-providers-apache-drill-2.4.3rc1/apache_airflow_providers_apache_drill.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      109 2023-08-04 21:40:37.000000 apache-airflow-providers-apache-drill-2.4.3rc1/apache_airflow_providers_apache_drill.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-08-04 21:40:37.000000 apache-airflow-providers-apache-drill-2.4.3rc1/apache_airflow_providers_apache_drill.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      149 2023-08-04 21:40:37.000000 apache-airflow-providers-apache-drill-2.4.3rc1/apache_airflow_providers_apache_drill.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-08-04 21:40:37.000000 apache-airflow-providers-apache-drill-2.4.3rc1/apache_airflow_providers_apache_drill.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     5031 2023-08-04 10:24:23.000000 apache-airflow-providers-apache-drill-2.4.3rc1/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)     2041 2023-08-04 21:40:37.480942 apache-airflow-providers-apache-drill-2.4.3rc1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1727 2023-08-04 21:40:36.000000 apache-airflow-providers-apache-drill-2.4.3rc1/setup.py
```

### Comparing `apache-airflow-providers-apache-drill-2.4.3/LICENSE` & `apache-airflow-providers-apache-drill-2.4.3rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-drill-2.4.3/MANIFEST.in` & `apache-airflow-providers-apache-drill-2.4.3rc1/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-drill-2.4.3/PKG-INFO` & `apache-airflow-providers-apache-drill-2.4.3rc1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-apache-drill
-Version: 2.4.3
+Version: 2.4.3rc1
 Summary: Provider for Apache Airflow. Implements apache-airflow-providers-apache-drill package
 Home-page: https://airflow.apache.org/
 Download-URL: https://archive.apache.org/dist/airflow/providers
 Author: Apache Software Foundation
 Author-email: dev@airflow.apache.org
 License: Apache License 2.0
 Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-apache-drill/2.4.3/
@@ -67,15 +67,15 @@
     KIND, either express or implied.  See the License for the
     specific language governing permissions and limitations
     under the License.
 
 
 Package ``apache-airflow-providers-apache-drill``
 
-Release: ``2.4.3``
+Release: ``2.4.3rc1``
 
 
 `Apache Drill <https://drill.apache.org/>`__.
 
 
 Provider package
 ----------------
```

### Comparing `apache-airflow-providers-apache-drill-2.4.3/README.rst` & `apache-airflow-providers-apache-drill-2.4.3rc1/README.rst`

 * *Files 0% similar despite different names*

```diff
@@ -32,15 +32,15 @@
     KIND, either express or implied.  See the License for the
     specific language governing permissions and limitations
     under the License.
 
 
 Package ``apache-airflow-providers-apache-drill``
 
-Release: ``2.4.3``
+Release: ``2.4.3rc1``
 
 
 `Apache Drill <https://drill.apache.org/>`__.
 
 
 Provider package
 ----------------
```

### Comparing `apache-airflow-providers-apache-drill-2.4.3/airflow/providers/apache/drill/__init__.py` & `apache-airflow-providers-apache-drill-2.4.3rc1/airflow/providers/apache/drill/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-drill-2.4.3/airflow/providers/apache/drill/get_provider_info.py` & `apache-airflow-providers-apache-drill-2.4.3rc1/airflow/providers/apache/drill/get_provider_info.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-drill-2.4.3/airflow/providers/apache/drill/hooks/__init__.py` & `apache-airflow-providers-apache-drill-2.4.3rc1/airflow/providers/apache/drill/hooks/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-drill-2.4.3/airflow/providers/apache/drill/hooks/drill.py` & `apache-airflow-providers-apache-drill-2.4.3rc1/airflow/providers/apache/drill/hooks/drill.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-drill-2.4.3/airflow/providers/apache/drill/operators/__init__.py` & `apache-airflow-providers-apache-drill-2.4.3rc1/airflow/providers/apache/drill/operators/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-drill-2.4.3/airflow/providers/apache/drill/operators/drill.py` & `apache-airflow-providers-apache-drill-2.4.3rc1/airflow/providers/apache/drill/operators/drill.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-drill-2.4.3/apache_airflow_providers_apache_drill.egg-info/PKG-INFO` & `apache-airflow-providers-apache-drill-2.4.3rc1/apache_airflow_providers_apache_drill.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-apache-drill
-Version: 2.4.3
+Version: 2.4.3rc1
 Summary: Provider for Apache Airflow. Implements apache-airflow-providers-apache-drill package
 Home-page: https://airflow.apache.org/
 Download-URL: https://archive.apache.org/dist/airflow/providers
 Author: Apache Software Foundation
 Author-email: dev@airflow.apache.org
 License: Apache License 2.0
 Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-apache-drill/2.4.3/
@@ -67,15 +67,15 @@
     KIND, either express or implied.  See the License for the
     specific language governing permissions and limitations
     under the License.
 
 
 Package ``apache-airflow-providers-apache-drill``
 
-Release: ``2.4.3``
+Release: ``2.4.3rc1``
 
 
 `Apache Drill <https://drill.apache.org/>`__.
 
 
 Provider package
 ----------------
```

### Comparing `apache-airflow-providers-apache-drill-2.4.3/apache_airflow_providers_apache_drill.egg-info/SOURCES.txt` & `apache-airflow-providers-apache-drill-2.4.3rc1/apache_airflow_providers_apache_drill.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-drill-2.4.3/pyproject.toml` & `apache-airflow-providers-apache-drill-2.4.3rc1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-drill-2.4.3/setup.cfg` & `apache-airflow-providers-apache-drill-2.4.3rc1/setup.cfg`

 * *Files 8% similar despite different names*

```diff
@@ -43,22 +43,22 @@
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
 	sqlalchemy-drill>=1.1.0
 
 [options.entry_points]
 apache_airflow_provider = 
 	provider_info=airflow.providers.apache.drill.get_provider_info:get_provider_info
 
 [files]
 packages = airflow.providers.apache.drill
 
 [egg_info]
-tag_build = 
+tag_build = rc1
 tag_date = 0
```

### Comparing `apache-airflow-providers-apache-drill-2.4.3/setup.py` & `apache-airflow-providers-apache-drill-2.4.3rc1/setup.py`

 * *Files identical despite different names*


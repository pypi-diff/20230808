# Comparing `tmp/apache-airflow-providers-apache-sqoop-4.0.0.tar.gz` & `tmp/apache-airflow-providers-apache-sqoop-4.0.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apache-airflow-providers-apache-sqoop-4.0.0.tar", last modified: Fri Aug  4 21:35:07 2023, max compression
+gzip compressed data, was "apache-airflow-providers-apache-sqoop-4.0.0rc1.tar", last modified: Fri Aug  4 21:40:47 2023, max compression
```

## Comparing `apache-airflow-providers-apache-sqoop-4.0.0.tar` & `apache-airflow-providers-apache-sqoop-4.0.0rc1.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 21:35:07.846392 apache-airflow-providers-apache-sqoop-4.0.0/
--rw-r--r--   0 root         (0) root         (0)    10850 2023-06-01 06:14:29.000000 apache-airflow-providers-apache-sqoop-4.0.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)     1104 2023-08-04 21:35:06.000000 apache-airflow-providers-apache-sqoop-4.0.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      240 2023-06-01 06:14:29.000000 apache-airflow-providers-apache-sqoop-4.0.0/NOTICE
--rw-r--r--   0 root         (0) root         (0)     4431 2023-08-04 21:35:07.846963 apache-airflow-providers-apache-sqoop-4.0.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2772 2023-08-04 21:35:06.000000 apache-airflow-providers-apache-sqoop-4.0.0/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 21:35:07.775058 apache-airflow-providers-apache-sqoop-4.0.0/airflow/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 21:35:07.776128 apache-airflow-providers-apache-sqoop-4.0.0/airflow/providers/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 21:35:07.777168 apache-airflow-providers-apache-sqoop-4.0.0/airflow/providers/apache/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 21:35:07.808902 apache-airflow-providers-apache-sqoop-4.0.0/airflow/providers/apache/sqoop/
--rw-r--r--   0 root         (0) root         (0)     1581 2023-08-04 21:33:34.000000 apache-airflow-providers-apache-sqoop-4.0.0/airflow/providers/apache/sqoop/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2636 2023-08-04 21:35:06.000000 apache-airflow-providers-apache-sqoop-4.0.0/airflow/providers/apache/sqoop/get_provider_info.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 21:35:07.814373 apache-airflow-providers-apache-sqoop-4.0.0/airflow/providers/apache/sqoop/hooks/
--rw-r--r--   0 root         (0) root         (0)      787 2023-06-01 06:14:28.000000 apache-airflow-providers-apache-sqoop-4.0.0/airflow/providers/apache/sqoop/hooks/__init__.py
--rw-r--r--   0 root         (0) root         (0)    15200 2023-08-04 10:24:22.000000 apache-airflow-providers-apache-sqoop-4.0.0/airflow/providers/apache/sqoop/hooks/sqoop.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 21:35:07.819959 apache-airflow-providers-apache-sqoop-4.0.0/airflow/providers/apache/sqoop/operators/
--rw-r--r--   0 root         (0) root         (0)      787 2023-06-01 06:14:28.000000 apache-airflow-providers-apache-sqoop-4.0.0/airflow/providers/apache/sqoop/operators/__init__.py
--rw-r--r--   0 root         (0) root         (0)    11028 2023-08-04 10:24:22.000000 apache-airflow-providers-apache-sqoop-4.0.0/airflow/providers/apache/sqoop/operators/sqoop.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 21:35:07.844094 apache-airflow-providers-apache-sqoop-4.0.0/apache_airflow_providers_apache_sqoop.egg-info/
--rw-r--r--   0 root         (0) root         (0)     4431 2023-08-04 21:35:07.000000 apache-airflow-providers-apache-sqoop-4.0.0/apache_airflow_providers_apache_sqoop.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      792 2023-08-04 21:35:07.000000 apache-airflow-providers-apache-sqoop-4.0.0/apache_airflow_providers_apache_sqoop.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-08-04 21:35:07.000000 apache-airflow-providers-apache-sqoop-4.0.0/apache_airflow_providers_apache_sqoop.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      109 2023-08-04 21:35:07.000000 apache-airflow-providers-apache-sqoop-4.0.0/apache_airflow_providers_apache_sqoop.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-08-04 21:35:07.000000 apache-airflow-providers-apache-sqoop-4.0.0/apache_airflow_providers_apache_sqoop.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       22 2023-08-04 21:35:07.000000 apache-airflow-providers-apache-sqoop-4.0.0/apache_airflow_providers_apache_sqoop.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-08-04 21:35:07.000000 apache-airflow-providers-apache-sqoop-4.0.0/apache_airflow_providers_apache_sqoop.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     5031 2023-08-04 10:24:23.000000 apache-airflow-providers-apache-sqoop-4.0.0/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)     1959 2023-08-04 21:35:07.848848 apache-airflow-providers-apache-sqoop-4.0.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1674 2023-08-04 21:35:06.000000 apache-airflow-providers-apache-sqoop-4.0.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 21:40:47.959609 apache-airflow-providers-apache-sqoop-4.0.0rc1/
+-rw-r--r--   0 root         (0) root         (0)    10850 2023-06-01 06:14:29.000000 apache-airflow-providers-apache-sqoop-4.0.0rc1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     1104 2023-08-04 21:40:46.000000 apache-airflow-providers-apache-sqoop-4.0.0rc1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      240 2023-06-01 06:14:29.000000 apache-airflow-providers-apache-sqoop-4.0.0rc1/NOTICE
+-rw-r--r--   0 root         (0) root         (0)     4437 2023-08-04 21:40:47.960189 apache-airflow-providers-apache-sqoop-4.0.0rc1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2775 2023-08-04 21:40:46.000000 apache-airflow-providers-apache-sqoop-4.0.0rc1/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 21:40:47.880204 apache-airflow-providers-apache-sqoop-4.0.0rc1/airflow/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 21:40:47.881287 apache-airflow-providers-apache-sqoop-4.0.0rc1/airflow/providers/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 21:40:47.882306 apache-airflow-providers-apache-sqoop-4.0.0rc1/airflow/providers/apache/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 21:40:47.914752 apache-airflow-providers-apache-sqoop-4.0.0rc1/airflow/providers/apache/sqoop/
+-rw-r--r--   0 root         (0) root         (0)     1581 2023-08-04 21:33:34.000000 apache-airflow-providers-apache-sqoop-4.0.0rc1/airflow/providers/apache/sqoop/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2636 2023-08-04 21:40:46.000000 apache-airflow-providers-apache-sqoop-4.0.0rc1/airflow/providers/apache/sqoop/get_provider_info.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 21:40:47.922210 apache-airflow-providers-apache-sqoop-4.0.0rc1/airflow/providers/apache/sqoop/hooks/
+-rw-r--r--   0 root         (0) root         (0)      787 2023-06-01 06:14:28.000000 apache-airflow-providers-apache-sqoop-4.0.0rc1/airflow/providers/apache/sqoop/hooks/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    15200 2023-08-04 10:24:22.000000 apache-airflow-providers-apache-sqoop-4.0.0rc1/airflow/providers/apache/sqoop/hooks/sqoop.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 21:40:47.931244 apache-airflow-providers-apache-sqoop-4.0.0rc1/airflow/providers/apache/sqoop/operators/
+-rw-r--r--   0 root         (0) root         (0)      787 2023-06-01 06:14:28.000000 apache-airflow-providers-apache-sqoop-4.0.0rc1/airflow/providers/apache/sqoop/operators/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    11028 2023-08-04 10:24:22.000000 apache-airflow-providers-apache-sqoop-4.0.0rc1/airflow/providers/apache/sqoop/operators/sqoop.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 21:40:47.956863 apache-airflow-providers-apache-sqoop-4.0.0rc1/apache_airflow_providers_apache_sqoop.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     4437 2023-08-04 21:40:47.000000 apache-airflow-providers-apache-sqoop-4.0.0rc1/apache_airflow_providers_apache_sqoop.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      792 2023-08-04 21:40:47.000000 apache-airflow-providers-apache-sqoop-4.0.0rc1/apache_airflow_providers_apache_sqoop.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-08-04 21:40:47.000000 apache-airflow-providers-apache-sqoop-4.0.0rc1/apache_airflow_providers_apache_sqoop.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      109 2023-08-04 21:40:47.000000 apache-airflow-providers-apache-sqoop-4.0.0rc1/apache_airflow_providers_apache_sqoop.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-08-04 21:40:47.000000 apache-airflow-providers-apache-sqoop-4.0.0rc1/apache_airflow_providers_apache_sqoop.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       27 2023-08-04 21:40:47.000000 apache-airflow-providers-apache-sqoop-4.0.0rc1/apache_airflow_providers_apache_sqoop.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-08-04 21:40:47.000000 apache-airflow-providers-apache-sqoop-4.0.0rc1/apache_airflow_providers_apache_sqoop.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     5031 2023-08-04 10:24:23.000000 apache-airflow-providers-apache-sqoop-4.0.0rc1/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)     1967 2023-08-04 21:40:47.962062 apache-airflow-providers-apache-sqoop-4.0.0rc1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1674 2023-08-04 21:40:46.000000 apache-airflow-providers-apache-sqoop-4.0.0rc1/setup.py
```

### Comparing `apache-airflow-providers-apache-sqoop-4.0.0/LICENSE` & `apache-airflow-providers-apache-sqoop-4.0.0rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-sqoop-4.0.0/MANIFEST.in` & `apache-airflow-providers-apache-sqoop-4.0.0rc1/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-sqoop-4.0.0/PKG-INFO` & `apache-airflow-providers-apache-sqoop-4.0.0rc1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-apache-sqoop
-Version: 4.0.0
+Version: 4.0.0rc1
 Summary: Provider for Apache Airflow. Implements apache-airflow-providers-apache-sqoop package
 Home-page: https://airflow.apache.org/
 Download-URL: https://archive.apache.org/dist/airflow/providers
 Author: Apache Software Foundation
 Author-email: dev@airflow.apache.org
 License: Apache License 2.0
 Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-apache-sqoop/4.0.0/
@@ -66,15 +66,15 @@
     KIND, either express or implied.  See the License for the
     specific language governing permissions and limitations
     under the License.
 
 
 Package ``apache-airflow-providers-apache-sqoop``
 
-Release: ``4.0.0``
+Release: ``4.0.0rc1``
 
 
 `Apache Sqoop <https://sqoop.apache.org/>`__
 
 
 Provider package
 ----------------
```

### Comparing `apache-airflow-providers-apache-sqoop-4.0.0/README.rst` & `apache-airflow-providers-apache-sqoop-4.0.0rc1/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -32,15 +32,15 @@
     KIND, either express or implied.  See the License for the
     specific language governing permissions and limitations
     under the License.
 
 
 Package ``apache-airflow-providers-apache-sqoop``
 
-Release: ``4.0.0``
+Release: ``4.0.0rc1``
 
 
 `Apache Sqoop <https://sqoop.apache.org/>`__
 
 
 Provider package
 ----------------
```

### Comparing `apache-airflow-providers-apache-sqoop-4.0.0/airflow/providers/apache/sqoop/__init__.py` & `apache-airflow-providers-apache-sqoop-4.0.0rc1/airflow/providers/apache/sqoop/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-sqoop-4.0.0/airflow/providers/apache/sqoop/get_provider_info.py` & `apache-airflow-providers-apache-sqoop-4.0.0rc1/airflow/providers/apache/sqoop/get_provider_info.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-sqoop-4.0.0/airflow/providers/apache/sqoop/hooks/__init__.py` & `apache-airflow-providers-apache-sqoop-4.0.0rc1/airflow/providers/apache/sqoop/hooks/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-sqoop-4.0.0/airflow/providers/apache/sqoop/hooks/sqoop.py` & `apache-airflow-providers-apache-sqoop-4.0.0rc1/airflow/providers/apache/sqoop/hooks/sqoop.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-sqoop-4.0.0/airflow/providers/apache/sqoop/operators/__init__.py` & `apache-airflow-providers-apache-sqoop-4.0.0rc1/airflow/providers/apache/sqoop/operators/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-sqoop-4.0.0/airflow/providers/apache/sqoop/operators/sqoop.py` & `apache-airflow-providers-apache-sqoop-4.0.0rc1/airflow/providers/apache/sqoop/operators/sqoop.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-sqoop-4.0.0/apache_airflow_providers_apache_sqoop.egg-info/PKG-INFO` & `apache-airflow-providers-apache-sqoop-4.0.0rc1/apache_airflow_providers_apache_sqoop.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-apache-sqoop
-Version: 4.0.0
+Version: 4.0.0rc1
 Summary: Provider for Apache Airflow. Implements apache-airflow-providers-apache-sqoop package
 Home-page: https://airflow.apache.org/
 Download-URL: https://archive.apache.org/dist/airflow/providers
 Author: Apache Software Foundation
 Author-email: dev@airflow.apache.org
 License: Apache License 2.0
 Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-apache-sqoop/4.0.0/
@@ -66,15 +66,15 @@
     KIND, either express or implied.  See the License for the
     specific language governing permissions and limitations
     under the License.
 
 
 Package ``apache-airflow-providers-apache-sqoop``
 
-Release: ``4.0.0``
+Release: ``4.0.0rc1``
 
 
 `Apache Sqoop <https://sqoop.apache.org/>`__
 
 
 Provider package
 ----------------
```

### Comparing `apache-airflow-providers-apache-sqoop-4.0.0/apache_airflow_providers_apache_sqoop.egg-info/SOURCES.txt` & `apache-airflow-providers-apache-sqoop-4.0.0rc1/apache_airflow_providers_apache_sqoop.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-sqoop-4.0.0/pyproject.toml` & `apache-airflow-providers-apache-sqoop-4.0.0rc1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-sqoop-4.0.0/setup.cfg` & `apache-airflow-providers-apache-sqoop-4.0.0rc1/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -43,20 +43,20 @@
 include_package_data = True
 python_requires = ~=3.8
 packages = find:
 setup_requires = 
 	setuptools
 	wheel
 install_requires = 
-	apache-airflow>=2.4.0
+	apache-airflow>=2.4.0.dev0
 
 [options.entry_points]
 apache_airflow_provider = 
 	provider_info=airflow.providers.apache.sqoop.get_provider_info:get_provider_info
 
 [files]
 packages = airflow.providers.apache.sqoop
 
 [egg_info]
-tag_build = 
+tag_build = rc1
 tag_date = 0
```

### Comparing `apache-airflow-providers-apache-sqoop-4.0.0/setup.py` & `apache-airflow-providers-apache-sqoop-4.0.0rc1/setup.py`

 * *Files identical despite different names*


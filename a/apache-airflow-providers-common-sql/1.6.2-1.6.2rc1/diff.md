# Comparing `tmp/apache-airflow-providers-common-sql-1.6.2.tar.gz` & `tmp/apache-airflow-providers-common-sql-1.6.2rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apache-airflow-providers-common-sql-1.6.2.tar", last modified: Fri Aug  4 21:35:17 2023, max compression
+gzip compressed data, was "apache-airflow-providers-common-sql-1.6.2rc1.tar", last modified: Fri Aug  4 21:40:58 2023, max compression
```

## Comparing `apache-airflow-providers-common-sql-1.6.2.tar` & `apache-airflow-providers-common-sql-1.6.2rc1.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 21:35:17.623457 apache-airflow-providers-common-sql-1.6.2/
--rw-r--r--   0 root         (0) root         (0)    10850 2023-06-01 06:14:29.000000 apache-airflow-providers-common-sql-1.6.2/LICENSE
--rw-r--r--   0 root         (0) root         (0)     1104 2023-08-04 21:35:16.000000 apache-airflow-providers-common-sql-1.6.2/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      240 2023-06-01 06:14:29.000000 apache-airflow-providers-common-sql-1.6.2/NOTICE
--rw-r--r--   0 root         (0) root         (0)     5560 2023-08-04 21:35:17.624001 apache-airflow-providers-common-sql-1.6.2/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     3858 2023-08-04 21:35:16.000000 apache-airflow-providers-common-sql-1.6.2/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 21:35:17.544874 apache-airflow-providers-common-sql-1.6.2/airflow/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 21:35:17.545893 apache-airflow-providers-common-sql-1.6.2/airflow/providers/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 21:35:17.547036 apache-airflow-providers-common-sql-1.6.2/airflow/providers/common/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 21:35:17.579300 apache-airflow-providers-common-sql-1.6.2/airflow/providers/common/sql/
--rw-r--r--   0 root         (0) root         (0)     1579 2023-08-04 21:33:34.000000 apache-airflow-providers-common-sql-1.6.2/airflow/providers/common/sql/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2641 2023-08-04 21:35:16.000000 apache-airflow-providers-common-sql-1.6.2/airflow/providers/common/sql/get_provider_info.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 21:35:17.584979 apache-airflow-providers-common-sql-1.6.2/airflow/providers/common/sql/hooks/
--rw-r--r--   0 root         (0) root         (0)      785 2023-06-01 06:14:28.000000 apache-airflow-providers-common-sql-1.6.2/airflow/providers/common/sql/hooks/__init__.py
--rw-r--r--   0 root         (0) root         (0)    24869 2023-07-26 06:59:50.000000 apache-airflow-providers-common-sql-1.6.2/airflow/providers/common/sql/hooks/sql.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 21:35:17.590964 apache-airflow-providers-common-sql-1.6.2/airflow/providers/common/sql/operators/
--rw-r--r--   0 root         (0) root         (0)      785 2023-06-01 06:14:28.000000 apache-airflow-providers-common-sql-1.6.2/airflow/providers/common/sql/operators/__init__.py
--rw-r--r--   0 root         (0) root         (0)    47157 2023-08-04 19:44:14.000000 apache-airflow-providers-common-sql-1.6.2/airflow/providers/common/sql/operators/sql.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 21:35:17.596975 apache-airflow-providers-common-sql-1.6.2/airflow/providers/common/sql/sensors/
--rw-r--r--   0 root         (0) root         (0)      785 2023-06-01 06:14:28.000000 apache-airflow-providers-common-sql-1.6.2/airflow/providers/common/sql/sensors/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4726 2023-06-05 12:50:36.000000 apache-airflow-providers-common-sql-1.6.2/airflow/providers/common/sql/sensors/sql.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 21:35:17.620871 apache-airflow-providers-common-sql-1.6.2/apache_airflow_providers_common_sql.egg-info/
--rw-r--r--   0 root         (0) root         (0)     5560 2023-08-04 21:35:17.000000 apache-airflow-providers-common-sql-1.6.2/apache_airflow_providers_common_sql.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      855 2023-08-04 21:35:17.000000 apache-airflow-providers-common-sql-1.6.2/apache_airflow_providers_common_sql.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-08-04 21:35:17.000000 apache-airflow-providers-common-sql-1.6.2/apache_airflow_providers_common_sql.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      107 2023-08-04 21:35:17.000000 apache-airflow-providers-common-sql-1.6.2/apache_airflow_providers_common_sql.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-08-04 21:35:17.000000 apache-airflow-providers-common-sql-1.6.2/apache_airflow_providers_common_sql.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      115 2023-08-04 21:35:17.000000 apache-airflow-providers-common-sql-1.6.2/apache_airflow_providers_common_sql.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-08-04 21:35:17.000000 apache-airflow-providers-common-sql-1.6.2/apache_airflow_providers_common_sql.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     5031 2023-08-04 10:24:23.000000 apache-airflow-providers-common-sql-1.6.2/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)     1962 2023-08-04 21:35:17.625960 apache-airflow-providers-common-sql-1.6.2/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1782 2023-08-04 21:35:16.000000 apache-airflow-providers-common-sql-1.6.2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 21:40:58.024927 apache-airflow-providers-common-sql-1.6.2rc1/
+-rw-r--r--   0 root         (0) root         (0)    10850 2023-06-01 06:14:29.000000 apache-airflow-providers-common-sql-1.6.2rc1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     1104 2023-08-04 21:40:56.000000 apache-airflow-providers-common-sql-1.6.2rc1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      240 2023-06-01 06:14:29.000000 apache-airflow-providers-common-sql-1.6.2rc1/NOTICE
+-rw-r--r--   0 root         (0) root         (0)     5566 2023-08-04 21:40:58.025505 apache-airflow-providers-common-sql-1.6.2rc1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     3861 2023-08-04 21:40:56.000000 apache-airflow-providers-common-sql-1.6.2rc1/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 21:40:57.943530 apache-airflow-providers-common-sql-1.6.2rc1/airflow/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 21:40:57.944697 apache-airflow-providers-common-sql-1.6.2rc1/airflow/providers/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 21:40:57.945738 apache-airflow-providers-common-sql-1.6.2rc1/airflow/providers/common/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 21:40:57.978421 apache-airflow-providers-common-sql-1.6.2rc1/airflow/providers/common/sql/
+-rw-r--r--   0 root         (0) root         (0)     1579 2023-08-04 21:33:34.000000 apache-airflow-providers-common-sql-1.6.2rc1/airflow/providers/common/sql/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2641 2023-08-04 21:40:56.000000 apache-airflow-providers-common-sql-1.6.2rc1/airflow/providers/common/sql/get_provider_info.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 21:40:57.984055 apache-airflow-providers-common-sql-1.6.2rc1/airflow/providers/common/sql/hooks/
+-rw-r--r--   0 root         (0) root         (0)      785 2023-06-01 06:14:28.000000 apache-airflow-providers-common-sql-1.6.2rc1/airflow/providers/common/sql/hooks/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    24869 2023-07-26 06:59:50.000000 apache-airflow-providers-common-sql-1.6.2rc1/airflow/providers/common/sql/hooks/sql.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 21:40:57.989944 apache-airflow-providers-common-sql-1.6.2rc1/airflow/providers/common/sql/operators/
+-rw-r--r--   0 root         (0) root         (0)      785 2023-06-01 06:14:28.000000 apache-airflow-providers-common-sql-1.6.2rc1/airflow/providers/common/sql/operators/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    47157 2023-08-04 19:44:14.000000 apache-airflow-providers-common-sql-1.6.2rc1/airflow/providers/common/sql/operators/sql.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 21:40:57.996311 apache-airflow-providers-common-sql-1.6.2rc1/airflow/providers/common/sql/sensors/
+-rw-r--r--   0 root         (0) root         (0)      785 2023-06-01 06:14:28.000000 apache-airflow-providers-common-sql-1.6.2rc1/airflow/providers/common/sql/sensors/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4726 2023-06-05 12:50:36.000000 apache-airflow-providers-common-sql-1.6.2rc1/airflow/providers/common/sql/sensors/sql.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 21:40:58.022182 apache-airflow-providers-common-sql-1.6.2rc1/apache_airflow_providers_common_sql.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     5566 2023-08-04 21:40:57.000000 apache-airflow-providers-common-sql-1.6.2rc1/apache_airflow_providers_common_sql.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      855 2023-08-04 21:40:57.000000 apache-airflow-providers-common-sql-1.6.2rc1/apache_airflow_providers_common_sql.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-08-04 21:40:57.000000 apache-airflow-providers-common-sql-1.6.2rc1/apache_airflow_providers_common_sql.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      107 2023-08-04 21:40:57.000000 apache-airflow-providers-common-sql-1.6.2rc1/apache_airflow_providers_common_sql.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-08-04 21:40:57.000000 apache-airflow-providers-common-sql-1.6.2rc1/apache_airflow_providers_common_sql.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      120 2023-08-04 21:40:57.000000 apache-airflow-providers-common-sql-1.6.2rc1/apache_airflow_providers_common_sql.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-08-04 21:40:57.000000 apache-airflow-providers-common-sql-1.6.2rc1/apache_airflow_providers_common_sql.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     5031 2023-08-04 10:24:23.000000 apache-airflow-providers-common-sql-1.6.2rc1/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)     1970 2023-08-04 21:40:58.027302 apache-airflow-providers-common-sql-1.6.2rc1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1782 2023-08-04 21:40:56.000000 apache-airflow-providers-common-sql-1.6.2rc1/setup.py
```

### Comparing `apache-airflow-providers-common-sql-1.6.2/LICENSE` & `apache-airflow-providers-common-sql-1.6.2rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-common-sql-1.6.2/MANIFEST.in` & `apache-airflow-providers-common-sql-1.6.2rc1/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-common-sql-1.6.2/PKG-INFO` & `apache-airflow-providers-common-sql-1.6.2rc1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-common-sql
-Version: 1.6.2
+Version: 1.6.2rc1
 Summary: Provider for Apache Airflow. Implements apache-airflow-providers-common-sql package
 Home-page: https://airflow.apache.org/
 Download-URL: https://archive.apache.org/dist/airflow/providers
 Author: Apache Software Foundation
 Author-email: dev@airflow.apache.org
 License: Apache License 2.0
 Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-common-sql/1.6.2/
@@ -68,15 +68,15 @@
     KIND, either express or implied.  See the License for the
     specific language governing permissions and limitations
     under the License.
 
 
 Package ``apache-airflow-providers-common-sql``
 
-Release: ``1.6.2``
+Release: ``1.6.2rc1``
 
 
 `Common SQL Provider <https://en.wikipedia.org/wiki/SQL>`__
 
 
 Provider package
 ----------------
```

### Comparing `apache-airflow-providers-common-sql-1.6.2/README.rst` & `apache-airflow-providers-common-sql-1.6.2rc1/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -32,15 +32,15 @@
     KIND, either express or implied.  See the License for the
     specific language governing permissions and limitations
     under the License.
 
 
 Package ``apache-airflow-providers-common-sql``
 
-Release: ``1.6.2``
+Release: ``1.6.2rc1``
 
 
 `Common SQL Provider <https://en.wikipedia.org/wiki/SQL>`__
 
 
 Provider package
 ----------------
```

### Comparing `apache-airflow-providers-common-sql-1.6.2/airflow/providers/common/sql/__init__.py` & `apache-airflow-providers-common-sql-1.6.2rc1/airflow/providers/common/sql/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-common-sql-1.6.2/airflow/providers/common/sql/get_provider_info.py` & `apache-airflow-providers-common-sql-1.6.2rc1/airflow/providers/common/sql/get_provider_info.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-common-sql-1.6.2/airflow/providers/common/sql/hooks/__init__.py` & `apache-airflow-providers-common-sql-1.6.2rc1/airflow/providers/common/sql/hooks/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-common-sql-1.6.2/airflow/providers/common/sql/hooks/sql.py` & `apache-airflow-providers-common-sql-1.6.2rc1/airflow/providers/common/sql/hooks/sql.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-common-sql-1.6.2/airflow/providers/common/sql/operators/__init__.py` & `apache-airflow-providers-common-sql-1.6.2rc1/airflow/providers/common/sql/operators/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-common-sql-1.6.2/airflow/providers/common/sql/operators/sql.py` & `apache-airflow-providers-common-sql-1.6.2rc1/airflow/providers/common/sql/operators/sql.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-common-sql-1.6.2/airflow/providers/common/sql/sensors/__init__.py` & `apache-airflow-providers-common-sql-1.6.2rc1/airflow/providers/common/sql/sensors/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-common-sql-1.6.2/airflow/providers/common/sql/sensors/sql.py` & `apache-airflow-providers-common-sql-1.6.2rc1/airflow/providers/common/sql/sensors/sql.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-common-sql-1.6.2/apache_airflow_providers_common_sql.egg-info/PKG-INFO` & `apache-airflow-providers-common-sql-1.6.2rc1/apache_airflow_providers_common_sql.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-common-sql
-Version: 1.6.2
+Version: 1.6.2rc1
 Summary: Provider for Apache Airflow. Implements apache-airflow-providers-common-sql package
 Home-page: https://airflow.apache.org/
 Download-URL: https://archive.apache.org/dist/airflow/providers
 Author: Apache Software Foundation
 Author-email: dev@airflow.apache.org
 License: Apache License 2.0
 Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-common-sql/1.6.2/
@@ -68,15 +68,15 @@
     KIND, either express or implied.  See the License for the
     specific language governing permissions and limitations
     under the License.
 
 
 Package ``apache-airflow-providers-common-sql``
 
-Release: ``1.6.2``
+Release: ``1.6.2rc1``
 
 
 `Common SQL Provider <https://en.wikipedia.org/wiki/SQL>`__
 
 
 Provider package
 ----------------
```

### Comparing `apache-airflow-providers-common-sql-1.6.2/apache_airflow_providers_common_sql.egg-info/SOURCES.txt` & `apache-airflow-providers-common-sql-1.6.2rc1/apache_airflow_providers_common_sql.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-common-sql-1.6.2/pyproject.toml` & `apache-airflow-providers-common-sql-1.6.2rc1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-common-sql-1.6.2/setup.cfg` & `apache-airflow-providers-common-sql-1.6.2rc1/setup.cfg`

 * *Files 5% similar despite different names*

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
 	sqlparse>=0.4.2
 
 [options.entry_points]
 apache_airflow_provider = 
 	provider_info=airflow.providers.common.sql.get_provider_info:get_provider_info
 
 [files]
 packages = airflow.providers.common.sql
 
 [egg_info]
-tag_build = 
+tag_build = rc1
 tag_date = 0
```

### Comparing `apache-airflow-providers-common-sql-1.6.2/setup.py` & `apache-airflow-providers-common-sql-1.6.2rc1/setup.py`

 * *Files identical despite different names*


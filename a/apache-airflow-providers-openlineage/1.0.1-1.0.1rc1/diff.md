# Comparing `tmp/apache-airflow-providers-openlineage-1.0.1.tar.gz` & `tmp/apache-airflow-providers-openlineage-1.0.1rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apache-airflow-providers-openlineage-1.0.1.tar", last modified: Fri Aug  4 21:35:46 2023, max compression
+gzip compressed data, was "apache-airflow-providers-openlineage-1.0.1rc1.tar", last modified: Fri Aug  4 21:41:28 2023, max compression
```

## Comparing `apache-airflow-providers-openlineage-1.0.1.tar` & `apache-airflow-providers-openlineage-1.0.1rc1.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 21:35:46.294538 apache-airflow-providers-openlineage-1.0.1/
--rw-r--r--   0 root         (0) root         (0)    10850 2023-06-01 06:14:29.000000 apache-airflow-providers-openlineage-1.0.1/LICENSE
--rw-r--r--   0 root         (0) root         (0)     1104 2023-08-04 21:35:45.000000 apache-airflow-providers-openlineage-1.0.1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      240 2023-06-01 06:14:29.000000 apache-airflow-providers-openlineage-1.0.1/NOTICE
--rw-r--r--   0 root         (0) root         (0)     5800 2023-08-04 21:35:46.295088 apache-airflow-providers-openlineage-1.0.1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     4118 2023-08-04 21:35:45.000000 apache-airflow-providers-openlineage-1.0.1/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 21:35:46.187949 apache-airflow-providers-openlineage-1.0.1/airflow/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 21:35:46.189061 apache-airflow-providers-openlineage-1.0.1/airflow/providers/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 21:35:46.224512 apache-airflow-providers-openlineage-1.0.1/airflow/providers/openlineage/
--rw-r--r--   0 root         (0) root         (0)     1580 2023-08-04 21:33:34.000000 apache-airflow-providers-openlineage-1.0.1/airflow/providers/openlineage/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 21:35:46.238636 apache-airflow-providers-openlineage-1.0.1/airflow/providers/openlineage/extractors/
--rw-r--r--   0 root         (0) root         (0)     1081 2023-06-01 06:14:28.000000 apache-airflow-providers-openlineage-1.0.1/airflow/providers/openlineage/extractors/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4831 2023-08-04 19:44:14.000000 apache-airflow-providers-openlineage-1.0.1/airflow/providers/openlineage/extractors/base.py
--rw-r--r--   0 root         (0) root         (0)     2735 2023-07-27 05:54:58.000000 apache-airflow-providers-openlineage-1.0.1/airflow/providers/openlineage/extractors/bash.py
--rw-r--r--   0 root         (0) root         (0)     7806 2023-07-27 05:54:58.000000 apache-airflow-providers-openlineage-1.0.1/airflow/providers/openlineage/extractors/manager.py
--rw-r--r--   0 root         (0) root         (0)     3270 2023-07-27 05:54:58.000000 apache-airflow-providers-openlineage-1.0.1/airflow/providers/openlineage/extractors/python.py
--rw-r--r--   0 root         (0) root         (0)     4850 2023-08-04 21:35:45.000000 apache-airflow-providers-openlineage-1.0.1/airflow/providers/openlineage/get_provider_info.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 21:35:46.259026 apache-airflow-providers-openlineage-1.0.1/airflow/providers/openlineage/plugins/
--rw-r--r--   0 root         (0) root         (0)      785 2023-06-01 06:14:28.000000 apache-airflow-providers-openlineage-1.0.1/airflow/providers/openlineage/plugins/__init__.py
--rw-r--r--   0 root         (0) root         (0)    12484 2023-07-27 05:54:58.000000 apache-airflow-providers-openlineage-1.0.1/airflow/providers/openlineage/plugins/adapter.py
--rw-r--r--   0 root         (0) root         (0)     2218 2023-07-27 05:54:58.000000 apache-airflow-providers-openlineage-1.0.1/airflow/providers/openlineage/plugins/facets.py
--rw-r--r--   0 root         (0) root         (0)     7256 2023-07-05 07:19:39.000000 apache-airflow-providers-openlineage-1.0.1/airflow/providers/openlineage/plugins/listener.py
--rw-r--r--   0 root         (0) root         (0)     2356 2023-07-05 07:19:39.000000 apache-airflow-providers-openlineage-1.0.1/airflow/providers/openlineage/plugins/macros.py
--rw-r--r--   0 root         (0) root         (0)     1986 2023-08-04 20:15:26.000000 apache-airflow-providers-openlineage-1.0.1/airflow/providers/openlineage/plugins/openlineage.py
--rw-r--r--   0 root         (0) root         (0)    11220 2023-08-04 10:24:22.000000 apache-airflow-providers-openlineage-1.0.1/airflow/providers/openlineage/sqlparser.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 21:35:46.267869 apache-airflow-providers-openlineage-1.0.1/airflow/providers/openlineage/utils/
--rw-r--r--   0 root         (0) root         (0)      785 2023-06-01 06:14:28.000000 apache-airflow-providers-openlineage-1.0.1/airflow/providers/openlineage/utils/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7038 2023-07-27 05:54:58.000000 apache-airflow-providers-openlineage-1.0.1/airflow/providers/openlineage/utils/sql.py
--rw-r--r--   0 root         (0) root         (0)    13516 2023-08-04 19:44:14.000000 apache-airflow-providers-openlineage-1.0.1/airflow/providers/openlineage/utils/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 21:35:46.292325 apache-airflow-providers-openlineage-1.0.1/apache_airflow_providers_openlineage.egg-info/
--rw-r--r--   0 root         (0) root         (0)     5800 2023-08-04 21:35:46.000000 apache-airflow-providers-openlineage-1.0.1/apache_airflow_providers_openlineage.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1316 2023-08-04 21:35:46.000000 apache-airflow-providers-openlineage-1.0.1/apache_airflow_providers_openlineage.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-08-04 21:35:46.000000 apache-airflow-providers-openlineage-1.0.1/apache_airflow_providers_openlineage.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      217 2023-08-04 21:35:46.000000 apache-airflow-providers-openlineage-1.0.1/apache_airflow_providers_openlineage.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-08-04 21:35:46.000000 apache-airflow-providers-openlineage-1.0.1/apache_airflow_providers_openlineage.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      193 2023-08-04 21:35:46.000000 apache-airflow-providers-openlineage-1.0.1/apache_airflow_providers_openlineage.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-08-04 21:35:46.000000 apache-airflow-providers-openlineage-1.0.1/apache_airflow_providers_openlineage.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     5031 2023-08-04 10:24:23.000000 apache-airflow-providers-openlineage-1.0.1/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)     2185 2023-08-04 21:35:46.296965 apache-airflow-providers-openlineage-1.0.1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1721 2023-08-04 21:35:45.000000 apache-airflow-providers-openlineage-1.0.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 21:41:28.918074 apache-airflow-providers-openlineage-1.0.1rc1/
+-rw-r--r--   0 root         (0) root         (0)    10850 2023-06-01 06:14:29.000000 apache-airflow-providers-openlineage-1.0.1rc1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     1104 2023-08-04 21:41:27.000000 apache-airflow-providers-openlineage-1.0.1rc1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      240 2023-06-01 06:14:29.000000 apache-airflow-providers-openlineage-1.0.1rc1/NOTICE
+-rw-r--r--   0 root         (0) root         (0)     5806 2023-08-04 21:41:28.918956 apache-airflow-providers-openlineage-1.0.1rc1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     4121 2023-08-04 21:41:27.000000 apache-airflow-providers-openlineage-1.0.1rc1/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 21:41:28.802473 apache-airflow-providers-openlineage-1.0.1rc1/airflow/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 21:41:28.803773 apache-airflow-providers-openlineage-1.0.1rc1/airflow/providers/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 21:41:28.841940 apache-airflow-providers-openlineage-1.0.1rc1/airflow/providers/openlineage/
+-rw-r--r--   0 root         (0) root         (0)     1580 2023-08-04 21:33:34.000000 apache-airflow-providers-openlineage-1.0.1rc1/airflow/providers/openlineage/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 21:41:28.855989 apache-airflow-providers-openlineage-1.0.1rc1/airflow/providers/openlineage/extractors/
+-rw-r--r--   0 root         (0) root         (0)     1081 2023-06-01 06:14:28.000000 apache-airflow-providers-openlineage-1.0.1rc1/airflow/providers/openlineage/extractors/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4831 2023-08-04 19:44:14.000000 apache-airflow-providers-openlineage-1.0.1rc1/airflow/providers/openlineage/extractors/base.py
+-rw-r--r--   0 root         (0) root         (0)     2735 2023-07-27 05:54:58.000000 apache-airflow-providers-openlineage-1.0.1rc1/airflow/providers/openlineage/extractors/bash.py
+-rw-r--r--   0 root         (0) root         (0)     7806 2023-07-27 05:54:58.000000 apache-airflow-providers-openlineage-1.0.1rc1/airflow/providers/openlineage/extractors/manager.py
+-rw-r--r--   0 root         (0) root         (0)     3270 2023-07-27 05:54:58.000000 apache-airflow-providers-openlineage-1.0.1rc1/airflow/providers/openlineage/extractors/python.py
+-rw-r--r--   0 root         (0) root         (0)     4850 2023-08-04 21:41:27.000000 apache-airflow-providers-openlineage-1.0.1rc1/airflow/providers/openlineage/get_provider_info.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 21:41:28.873537 apache-airflow-providers-openlineage-1.0.1rc1/airflow/providers/openlineage/plugins/
+-rw-r--r--   0 root         (0) root         (0)      785 2023-06-01 06:14:28.000000 apache-airflow-providers-openlineage-1.0.1rc1/airflow/providers/openlineage/plugins/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    12484 2023-07-27 05:54:58.000000 apache-airflow-providers-openlineage-1.0.1rc1/airflow/providers/openlineage/plugins/adapter.py
+-rw-r--r--   0 root         (0) root         (0)     2218 2023-07-27 05:54:58.000000 apache-airflow-providers-openlineage-1.0.1rc1/airflow/providers/openlineage/plugins/facets.py
+-rw-r--r--   0 root         (0) root         (0)     7256 2023-07-05 07:19:39.000000 apache-airflow-providers-openlineage-1.0.1rc1/airflow/providers/openlineage/plugins/listener.py
+-rw-r--r--   0 root         (0) root         (0)     2356 2023-07-05 07:19:39.000000 apache-airflow-providers-openlineage-1.0.1rc1/airflow/providers/openlineage/plugins/macros.py
+-rw-r--r--   0 root         (0) root         (0)     1986 2023-08-04 20:15:26.000000 apache-airflow-providers-openlineage-1.0.1rc1/airflow/providers/openlineage/plugins/openlineage.py
+-rw-r--r--   0 root         (0) root         (0)    11220 2023-08-04 10:24:22.000000 apache-airflow-providers-openlineage-1.0.1rc1/airflow/providers/openlineage/sqlparser.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 21:41:28.882160 apache-airflow-providers-openlineage-1.0.1rc1/airflow/providers/openlineage/utils/
+-rw-r--r--   0 root         (0) root         (0)      785 2023-06-01 06:14:28.000000 apache-airflow-providers-openlineage-1.0.1rc1/airflow/providers/openlineage/utils/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7038 2023-07-27 05:54:58.000000 apache-airflow-providers-openlineage-1.0.1rc1/airflow/providers/openlineage/utils/sql.py
+-rw-r--r--   0 root         (0) root         (0)    13516 2023-08-04 19:44:14.000000 apache-airflow-providers-openlineage-1.0.1rc1/airflow/providers/openlineage/utils/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 21:41:28.913214 apache-airflow-providers-openlineage-1.0.1rc1/apache_airflow_providers_openlineage.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     5806 2023-08-04 21:41:28.000000 apache-airflow-providers-openlineage-1.0.1rc1/apache_airflow_providers_openlineage.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1316 2023-08-04 21:41:28.000000 apache-airflow-providers-openlineage-1.0.1rc1/apache_airflow_providers_openlineage.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-08-04 21:41:28.000000 apache-airflow-providers-openlineage-1.0.1rc1/apache_airflow_providers_openlineage.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      217 2023-08-04 21:41:28.000000 apache-airflow-providers-openlineage-1.0.1rc1/apache_airflow_providers_openlineage.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-08-04 21:41:28.000000 apache-airflow-providers-openlineage-1.0.1rc1/apache_airflow_providers_openlineage.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      203 2023-08-04 21:41:28.000000 apache-airflow-providers-openlineage-1.0.1rc1/apache_airflow_providers_openlineage.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-08-04 21:41:28.000000 apache-airflow-providers-openlineage-1.0.1rc1/apache_airflow_providers_openlineage.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     5031 2023-08-04 10:24:23.000000 apache-airflow-providers-openlineage-1.0.1rc1/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)     2198 2023-08-04 21:41:28.921712 apache-airflow-providers-openlineage-1.0.1rc1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1721 2023-08-04 21:41:27.000000 apache-airflow-providers-openlineage-1.0.1rc1/setup.py
```

### Comparing `apache-airflow-providers-openlineage-1.0.1/LICENSE` & `apache-airflow-providers-openlineage-1.0.1rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-openlineage-1.0.1/MANIFEST.in` & `apache-airflow-providers-openlineage-1.0.1rc1/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-openlineage-1.0.1/PKG-INFO` & `apache-airflow-providers-openlineage-1.0.1rc1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-openlineage
-Version: 1.0.1
+Version: 1.0.1rc1
 Summary: Provider for Apache Airflow. Implements apache-airflow-providers-openlineage package
 Home-page: https://airflow.apache.org/
 Download-URL: https://archive.apache.org/dist/airflow/providers
 Author: Apache Software Foundation
 Author-email: dev@airflow.apache.org
 License: Apache License 2.0
 Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-openlineage/1.0.1/
@@ -67,15 +67,15 @@
     KIND, either express or implied.  See the License for the
     specific language governing permissions and limitations
     under the License.
 
 
 Package ``apache-airflow-providers-openlineage``
 
-Release: ``1.0.1``
+Release: ``1.0.1rc1``
 
 
 `OpenLineage <https://openlineage.io/>`__
 
 
 Provider package
 ----------------
```

### Comparing `apache-airflow-providers-openlineage-1.0.1/README.rst` & `apache-airflow-providers-openlineage-1.0.1rc1/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -32,15 +32,15 @@
     KIND, either express or implied.  See the License for the
     specific language governing permissions and limitations
     under the License.
 
 
 Package ``apache-airflow-providers-openlineage``
 
-Release: ``1.0.1``
+Release: ``1.0.1rc1``
 
 
 `OpenLineage <https://openlineage.io/>`__
 
 
 Provider package
 ----------------
```

### Comparing `apache-airflow-providers-openlineage-1.0.1/airflow/providers/openlineage/__init__.py` & `apache-airflow-providers-openlineage-1.0.1rc1/airflow/providers/openlineage/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-openlineage-1.0.1/airflow/providers/openlineage/extractors/__init__.py` & `apache-airflow-providers-openlineage-1.0.1rc1/airflow/providers/openlineage/extractors/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-openlineage-1.0.1/airflow/providers/openlineage/extractors/base.py` & `apache-airflow-providers-openlineage-1.0.1rc1/airflow/providers/openlineage/extractors/base.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-openlineage-1.0.1/airflow/providers/openlineage/extractors/bash.py` & `apache-airflow-providers-openlineage-1.0.1rc1/airflow/providers/openlineage/extractors/bash.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-openlineage-1.0.1/airflow/providers/openlineage/extractors/manager.py` & `apache-airflow-providers-openlineage-1.0.1rc1/airflow/providers/openlineage/extractors/manager.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-openlineage-1.0.1/airflow/providers/openlineage/extractors/python.py` & `apache-airflow-providers-openlineage-1.0.1rc1/airflow/providers/openlineage/extractors/python.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-openlineage-1.0.1/airflow/providers/openlineage/get_provider_info.py` & `apache-airflow-providers-openlineage-1.0.1rc1/airflow/providers/openlineage/get_provider_info.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-openlineage-1.0.1/airflow/providers/openlineage/plugins/__init__.py` & `apache-airflow-providers-openlineage-1.0.1rc1/airflow/providers/openlineage/plugins/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-openlineage-1.0.1/airflow/providers/openlineage/plugins/adapter.py` & `apache-airflow-providers-openlineage-1.0.1rc1/airflow/providers/openlineage/plugins/adapter.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-openlineage-1.0.1/airflow/providers/openlineage/plugins/facets.py` & `apache-airflow-providers-openlineage-1.0.1rc1/airflow/providers/openlineage/plugins/facets.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-openlineage-1.0.1/airflow/providers/openlineage/plugins/listener.py` & `apache-airflow-providers-openlineage-1.0.1rc1/airflow/providers/openlineage/plugins/listener.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-openlineage-1.0.1/airflow/providers/openlineage/plugins/macros.py` & `apache-airflow-providers-openlineage-1.0.1rc1/airflow/providers/openlineage/plugins/macros.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-openlineage-1.0.1/airflow/providers/openlineage/plugins/openlineage.py` & `apache-airflow-providers-openlineage-1.0.1rc1/airflow/providers/openlineage/plugins/openlineage.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-openlineage-1.0.1/airflow/providers/openlineage/sqlparser.py` & `apache-airflow-providers-openlineage-1.0.1rc1/airflow/providers/openlineage/sqlparser.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-openlineage-1.0.1/airflow/providers/openlineage/utils/__init__.py` & `apache-airflow-providers-openlineage-1.0.1rc1/airflow/providers/openlineage/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-openlineage-1.0.1/airflow/providers/openlineage/utils/sql.py` & `apache-airflow-providers-openlineage-1.0.1rc1/airflow/providers/openlineage/utils/sql.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-openlineage-1.0.1/airflow/providers/openlineage/utils/utils.py` & `apache-airflow-providers-openlineage-1.0.1rc1/airflow/providers/openlineage/utils/utils.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-openlineage-1.0.1/apache_airflow_providers_openlineage.egg-info/PKG-INFO` & `apache-airflow-providers-openlineage-1.0.1rc1/apache_airflow_providers_openlineage.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-openlineage
-Version: 1.0.1
+Version: 1.0.1rc1
 Summary: Provider for Apache Airflow. Implements apache-airflow-providers-openlineage package
 Home-page: https://airflow.apache.org/
 Download-URL: https://archive.apache.org/dist/airflow/providers
 Author: Apache Software Foundation
 Author-email: dev@airflow.apache.org
 License: Apache License 2.0
 Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-openlineage/1.0.1/
@@ -67,15 +67,15 @@
     KIND, either express or implied.  See the License for the
     specific language governing permissions and limitations
     under the License.
 
 
 Package ``apache-airflow-providers-openlineage``
 
-Release: ``1.0.1``
+Release: ``1.0.1rc1``
 
 
 `OpenLineage <https://openlineage.io/>`__
 
 
 Provider package
 ----------------
```

### Comparing `apache-airflow-providers-openlineage-1.0.1/apache_airflow_providers_openlineage.egg-info/SOURCES.txt` & `apache-airflow-providers-openlineage-1.0.1rc1/apache_airflow_providers_openlineage.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-openlineage-1.0.1/pyproject.toml` & `apache-airflow-providers-openlineage-1.0.1rc1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-openlineage-1.0.1/setup.cfg` & `apache-airflow-providers-openlineage-1.0.1rc1/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -43,26 +43,26 @@
 include_package_data = True
 python_requires = ~=3.8
 packages = find:
 setup_requires = 
 	setuptools
 	wheel
 install_requires = 
-	apache-airflow-providers-common-sql>=1.6.0
-	apache-airflow>=2.7.0
+	apache-airflow-providers-common-sql>=1.6.0.dev0
+	apache-airflow>=2.7.0.dev0
 	attrs>=22.2
 	openlineage-integration-common>=0.28.0
 	openlineage-python>=0.28.0
 
 [options.entry_points]
 apache_airflow_provider = 
 	provider_info=airflow.providers.openlineage.get_provider_info:get_provider_info
 airflow.plugins = 
 	openlineage=airflow.providers.openlineage.plugins.openlineage:OpenLineageProviderPlugin
 
 [files]
 packages = airflow.providers.openlineage
 
 [egg_info]
-tag_build = 
+tag_build = rc1
 tag_date = 0
```

### Comparing `apache-airflow-providers-openlineage-1.0.1/setup.py` & `apache-airflow-providers-openlineage-1.0.1rc1/setup.py`

 * *Files identical despite different names*


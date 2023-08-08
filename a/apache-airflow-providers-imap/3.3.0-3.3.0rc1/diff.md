# Comparing `tmp/apache-airflow-providers-imap-3.3.0.tar.gz` & `tmp/apache-airflow-providers-imap-3.3.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apache-airflow-providers-imap-3.3.0.tar", last modified: Fri Aug  4 21:35:35 2023, max compression
+gzip compressed data, was "apache-airflow-providers-imap-3.3.0rc1.tar", last modified: Fri Aug  4 21:41:17 2023, max compression
```

## Comparing `apache-airflow-providers-imap-3.3.0.tar` & `apache-airflow-providers-imap-3.3.0rc1.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 21:35:35.642648 apache-airflow-providers-imap-3.3.0/
--rw-r--r--   0 root         (0) root         (0)    10850 2023-06-01 06:14:29.000000 apache-airflow-providers-imap-3.3.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)     1104 2023-08-04 21:35:34.000000 apache-airflow-providers-imap-3.3.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      240 2023-06-01 06:14:29.000000 apache-airflow-providers-imap-3.3.0/NOTICE
--rw-r--r--   0 root         (0) root         (0)     4388 2023-08-04 21:35:35.643242 apache-airflow-providers-imap-3.3.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2761 2023-08-04 21:35:34.000000 apache-airflow-providers-imap-3.3.0/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 21:35:35.569150 apache-airflow-providers-imap-3.3.0/airflow/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 21:35:35.570268 apache-airflow-providers-imap-3.3.0/airflow/providers/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 21:35:35.604526 apache-airflow-providers-imap-3.3.0/airflow/providers/imap/
--rw-r--r--   0 root         (0) root         (0)     1573 2023-08-04 21:33:34.000000 apache-airflow-providers-imap-3.3.0/airflow/providers/imap/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4200 2023-08-04 21:35:34.000000 apache-airflow-providers-imap-3.3.0/airflow/providers/imap/get_provider_info.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 21:35:35.610701 apache-airflow-providers-imap-3.3.0/airflow/providers/imap/hooks/
--rw-r--r--   0 root         (0) root         (0)      787 2023-06-01 06:14:28.000000 apache-airflow-providers-imap-3.3.0/airflow/providers/imap/hooks/__init__.py
--rw-r--r--   0 root         (0) root         (0)    15241 2023-08-04 19:44:14.000000 apache-airflow-providers-imap-3.3.0/airflow/providers/imap/hooks/imap.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 21:35:35.616505 apache-airflow-providers-imap-3.3.0/airflow/providers/imap/sensors/
--rw-r--r--   0 root         (0) root         (0)      787 2023-06-01 06:14:28.000000 apache-airflow-providers-imap-3.3.0/airflow/providers/imap/sensors/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3054 2023-06-01 06:14:28.000000 apache-airflow-providers-imap-3.3.0/airflow/providers/imap/sensors/imap_attachment.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 21:35:35.640047 apache-airflow-providers-imap-3.3.0/apache_airflow_providers_imap.egg-info/
--rw-r--r--   0 root         (0) root         (0)     4388 2023-08-04 21:35:35.000000 apache-airflow-providers-imap-3.3.0/apache_airflow_providers_imap.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      693 2023-08-04 21:35:35.000000 apache-airflow-providers-imap-3.3.0/apache_airflow_providers_imap.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-08-04 21:35:35.000000 apache-airflow-providers-imap-3.3.0/apache_airflow_providers_imap.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      101 2023-08-04 21:35:35.000000 apache-airflow-providers-imap-3.3.0/apache_airflow_providers_imap.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-08-04 21:35:35.000000 apache-airflow-providers-imap-3.3.0/apache_airflow_providers_imap.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       22 2023-08-04 21:35:35.000000 apache-airflow-providers-imap-3.3.0/apache_airflow_providers_imap.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-08-04 21:35:35.000000 apache-airflow-providers-imap-3.3.0/apache_airflow_providers_imap.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     5031 2023-08-04 10:24:23.000000 apache-airflow-providers-imap-3.3.0/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)     1903 2023-08-04 21:35:35.645070 apache-airflow-providers-imap-3.3.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1626 2023-08-04 21:35:34.000000 apache-airflow-providers-imap-3.3.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 21:41:17.873464 apache-airflow-providers-imap-3.3.0rc1/
+-rw-r--r--   0 root         (0) root         (0)    10850 2023-06-01 06:14:29.000000 apache-airflow-providers-imap-3.3.0rc1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     1104 2023-08-04 21:41:16.000000 apache-airflow-providers-imap-3.3.0rc1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      240 2023-06-01 06:14:29.000000 apache-airflow-providers-imap-3.3.0rc1/NOTICE
+-rw-r--r--   0 root         (0) root         (0)     4394 2023-08-04 21:41:17.874018 apache-airflow-providers-imap-3.3.0rc1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2764 2023-08-04 21:41:16.000000 apache-airflow-providers-imap-3.3.0rc1/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 21:41:17.802392 apache-airflow-providers-imap-3.3.0rc1/airflow/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 21:41:17.803547 apache-airflow-providers-imap-3.3.0rc1/airflow/providers/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 21:41:17.835532 apache-airflow-providers-imap-3.3.0rc1/airflow/providers/imap/
+-rw-r--r--   0 root         (0) root         (0)     1573 2023-08-04 21:33:34.000000 apache-airflow-providers-imap-3.3.0rc1/airflow/providers/imap/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4200 2023-08-04 21:41:16.000000 apache-airflow-providers-imap-3.3.0rc1/airflow/providers/imap/get_provider_info.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 21:41:17.841344 apache-airflow-providers-imap-3.3.0rc1/airflow/providers/imap/hooks/
+-rw-r--r--   0 root         (0) root         (0)      787 2023-06-01 06:14:28.000000 apache-airflow-providers-imap-3.3.0rc1/airflow/providers/imap/hooks/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    15241 2023-08-04 19:44:14.000000 apache-airflow-providers-imap-3.3.0rc1/airflow/providers/imap/hooks/imap.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 21:41:17.847041 apache-airflow-providers-imap-3.3.0rc1/airflow/providers/imap/sensors/
+-rw-r--r--   0 root         (0) root         (0)      787 2023-06-01 06:14:28.000000 apache-airflow-providers-imap-3.3.0rc1/airflow/providers/imap/sensors/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3054 2023-06-01 06:14:28.000000 apache-airflow-providers-imap-3.3.0rc1/airflow/providers/imap/sensors/imap_attachment.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 21:41:17.871279 apache-airflow-providers-imap-3.3.0rc1/apache_airflow_providers_imap.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     4394 2023-08-04 21:41:17.000000 apache-airflow-providers-imap-3.3.0rc1/apache_airflow_providers_imap.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      693 2023-08-04 21:41:17.000000 apache-airflow-providers-imap-3.3.0rc1/apache_airflow_providers_imap.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-08-04 21:41:17.000000 apache-airflow-providers-imap-3.3.0rc1/apache_airflow_providers_imap.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      101 2023-08-04 21:41:17.000000 apache-airflow-providers-imap-3.3.0rc1/apache_airflow_providers_imap.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-08-04 21:41:17.000000 apache-airflow-providers-imap-3.3.0rc1/apache_airflow_providers_imap.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       27 2023-08-04 21:41:17.000000 apache-airflow-providers-imap-3.3.0rc1/apache_airflow_providers_imap.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-08-04 21:41:17.000000 apache-airflow-providers-imap-3.3.0rc1/apache_airflow_providers_imap.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     5031 2023-08-04 10:24:23.000000 apache-airflow-providers-imap-3.3.0rc1/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)     1911 2023-08-04 21:41:17.875895 apache-airflow-providers-imap-3.3.0rc1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1626 2023-08-04 21:41:16.000000 apache-airflow-providers-imap-3.3.0rc1/setup.py
```

### Comparing `apache-airflow-providers-imap-3.3.0/LICENSE` & `apache-airflow-providers-imap-3.3.0rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-imap-3.3.0/MANIFEST.in` & `apache-airflow-providers-imap-3.3.0rc1/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-imap-3.3.0/PKG-INFO` & `apache-airflow-providers-imap-3.3.0rc1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-imap
-Version: 3.3.0
+Version: 3.3.0rc1
 Summary: Provider for Apache Airflow. Implements apache-airflow-providers-imap package
 Home-page: https://airflow.apache.org/
 Download-URL: https://archive.apache.org/dist/airflow/providers
 Author: Apache Software Foundation
 Author-email: dev@airflow.apache.org
 License: Apache License 2.0
 Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-imap/3.3.0/
@@ -66,15 +66,15 @@
     KIND, either express or implied.  See the License for the
     specific language governing permissions and limitations
     under the License.
 
 
 Package ``apache-airflow-providers-imap``
 
-Release: ``3.3.0``
+Release: ``3.3.0rc1``
 
 
 `Internet Message Access Protocol (IMAP) <https://tools.ietf.org/html/rfc3501>`__
 
 
 Provider package
 ----------------
```

### Comparing `apache-airflow-providers-imap-3.3.0/README.rst` & `apache-airflow-providers-imap-3.3.0rc1/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -32,15 +32,15 @@
     KIND, either express or implied.  See the License for the
     specific language governing permissions and limitations
     under the License.
 
 
 Package ``apache-airflow-providers-imap``
 
-Release: ``3.3.0``
+Release: ``3.3.0rc1``
 
 
 `Internet Message Access Protocol (IMAP) <https://tools.ietf.org/html/rfc3501>`__
 
 
 Provider package
 ----------------
```

### Comparing `apache-airflow-providers-imap-3.3.0/airflow/providers/imap/__init__.py` & `apache-airflow-providers-imap-3.3.0rc1/airflow/providers/imap/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-imap-3.3.0/airflow/providers/imap/get_provider_info.py` & `apache-airflow-providers-imap-3.3.0rc1/airflow/providers/imap/get_provider_info.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-imap-3.3.0/airflow/providers/imap/hooks/__init__.py` & `apache-airflow-providers-imap-3.3.0rc1/airflow/providers/imap/hooks/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-imap-3.3.0/airflow/providers/imap/hooks/imap.py` & `apache-airflow-providers-imap-3.3.0rc1/airflow/providers/imap/hooks/imap.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-imap-3.3.0/airflow/providers/imap/sensors/__init__.py` & `apache-airflow-providers-imap-3.3.0rc1/airflow/providers/imap/sensors/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-imap-3.3.0/airflow/providers/imap/sensors/imap_attachment.py` & `apache-airflow-providers-imap-3.3.0rc1/airflow/providers/imap/sensors/imap_attachment.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-imap-3.3.0/apache_airflow_providers_imap.egg-info/PKG-INFO` & `apache-airflow-providers-imap-3.3.0rc1/apache_airflow_providers_imap.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-imap
-Version: 3.3.0
+Version: 3.3.0rc1
 Summary: Provider for Apache Airflow. Implements apache-airflow-providers-imap package
 Home-page: https://airflow.apache.org/
 Download-URL: https://archive.apache.org/dist/airflow/providers
 Author: Apache Software Foundation
 Author-email: dev@airflow.apache.org
 License: Apache License 2.0
 Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-imap/3.3.0/
@@ -66,15 +66,15 @@
     KIND, either express or implied.  See the License for the
     specific language governing permissions and limitations
     under the License.
 
 
 Package ``apache-airflow-providers-imap``
 
-Release: ``3.3.0``
+Release: ``3.3.0rc1``
 
 
 `Internet Message Access Protocol (IMAP) <https://tools.ietf.org/html/rfc3501>`__
 
 
 Provider package
 ----------------
```

### Comparing `apache-airflow-providers-imap-3.3.0/apache_airflow_providers_imap.egg-info/SOURCES.txt` & `apache-airflow-providers-imap-3.3.0rc1/apache_airflow_providers_imap.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-imap-3.3.0/pyproject.toml` & `apache-airflow-providers-imap-3.3.0rc1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-imap-3.3.0/setup.cfg` & `apache-airflow-providers-imap-3.3.0rc1/setup.cfg`

 * *Files 8% similar despite different names*

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
 	provider_info=airflow.providers.imap.get_provider_info:get_provider_info
 
 [files]
 packages = airflow.providers.imap
 
 [egg_info]
-tag_build = 
+tag_build = rc1
 tag_date = 0
```

### Comparing `apache-airflow-providers-imap-3.3.0/setup.py` & `apache-airflow-providers-imap-3.3.0rc1/setup.py`

 * *Files identical despite different names*


# Comparing `tmp/apache-airflow-providers-ftp-3.5.0.tar.gz` & `tmp/apache-airflow-providers-ftp-3.5.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apache-airflow-providers-ftp-3.5.0.tar", last modified: Fri Aug  4 21:35:25 2023, max compression
+gzip compressed data, was "apache-airflow-providers-ftp-3.5.0rc1.tar", last modified: Fri Aug  4 21:41:06 2023, max compression
```

## Comparing `apache-airflow-providers-ftp-3.5.0.tar` & `apache-airflow-providers-ftp-3.5.0rc1.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 21:35:25.173849 apache-airflow-providers-ftp-3.5.0/
--rw-r--r--   0 root         (0) root         (0)    10850 2023-06-01 06:14:29.000000 apache-airflow-providers-ftp-3.5.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)     1104 2023-08-04 21:35:24.000000 apache-airflow-providers-ftp-3.5.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      240 2023-06-01 06:14:29.000000 apache-airflow-providers-ftp-3.5.0/NOTICE
--rw-r--r--   0 root         (0) root         (0)     5438 2023-08-04 21:35:25.174409 apache-airflow-providers-ftp-3.5.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     3787 2023-08-04 21:35:24.000000 apache-airflow-providers-ftp-3.5.0/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 21:35:25.085399 apache-airflow-providers-ftp-3.5.0/airflow/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 21:35:25.086371 apache-airflow-providers-ftp-3.5.0/airflow/providers/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 21:35:25.124728 apache-airflow-providers-ftp-3.5.0/airflow/providers/ftp/
--rw-r--r--   0 root         (0) root         (0)     1572 2023-08-04 21:33:34.000000 apache-airflow-providers-ftp-3.5.0/airflow/providers/ftp/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2786 2023-08-04 21:35:24.000000 apache-airflow-providers-ftp-3.5.0/airflow/providers/ftp/get_provider_info.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 21:35:25.130977 apache-airflow-providers-ftp-3.5.0/airflow/providers/ftp/hooks/
--rw-r--r--   0 root         (0) root         (0)      787 2023-06-01 06:14:28.000000 apache-airflow-providers-ftp-3.5.0/airflow/providers/ftp/hooks/__init__.py
--rw-r--r--   0 root         (0) root         (0)     9788 2023-06-29 05:49:30.000000 apache-airflow-providers-ftp-3.5.0/airflow/providers/ftp/hooks/ftp.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 21:35:25.139459 apache-airflow-providers-ftp-3.5.0/airflow/providers/ftp/operators/
--rw-r--r--   0 root         (0) root         (0)      785 2023-06-01 06:14:28.000000 apache-airflow-providers-ftp-3.5.0/airflow/providers/ftp/operators/__init__.py
--rw-r--r--   0 root         (0) root         (0)     8151 2023-08-04 10:24:22.000000 apache-airflow-providers-ftp-3.5.0/airflow/providers/ftp/operators/ftp.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 21:35:25.145798 apache-airflow-providers-ftp-3.5.0/airflow/providers/ftp/sensors/
--rw-r--r--   0 root         (0) root         (0)      787 2023-06-01 06:14:28.000000 apache-airflow-providers-ftp-3.5.0/airflow/providers/ftp/sensors/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3364 2023-06-02 11:31:21.000000 apache-airflow-providers-ftp-3.5.0/airflow/providers/ftp/sensors/ftp.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 21:35:25.171139 apache-airflow-providers-ftp-3.5.0/apache_airflow_providers_ftp.egg-info/
--rw-r--r--   0 root         (0) root         (0)     5438 2023-08-04 21:35:25.000000 apache-airflow-providers-ftp-3.5.0/apache_airflow_providers_ftp.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      750 2023-08-04 21:35:25.000000 apache-airflow-providers-ftp-3.5.0/apache_airflow_providers_ftp.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-08-04 21:35:25.000000 apache-airflow-providers-ftp-3.5.0/apache_airflow_providers_ftp.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      100 2023-08-04 21:35:25.000000 apache-airflow-providers-ftp-3.5.0/apache_airflow_providers_ftp.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-08-04 21:35:25.000000 apache-airflow-providers-ftp-3.5.0/apache_airflow_providers_ftp.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       74 2023-08-04 21:35:25.000000 apache-airflow-providers-ftp-3.5.0/apache_airflow_providers_ftp.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-08-04 21:35:25.000000 apache-airflow-providers-ftp-3.5.0/apache_airflow_providers_ftp.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     5031 2023-08-04 10:24:23.000000 apache-airflow-providers-ftp-3.5.0/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)     1896 2023-08-04 21:35:25.176267 apache-airflow-providers-ftp-3.5.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1675 2023-08-04 21:35:24.000000 apache-airflow-providers-ftp-3.5.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 21:41:06.801802 apache-airflow-providers-ftp-3.5.0rc1/
+-rw-r--r--   0 root         (0) root         (0)    10850 2023-06-01 06:14:29.000000 apache-airflow-providers-ftp-3.5.0rc1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     1104 2023-08-04 21:41:05.000000 apache-airflow-providers-ftp-3.5.0rc1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      240 2023-06-01 06:14:29.000000 apache-airflow-providers-ftp-3.5.0rc1/NOTICE
+-rw-r--r--   0 root         (0) root         (0)     5444 2023-08-04 21:41:06.802375 apache-airflow-providers-ftp-3.5.0rc1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     3790 2023-08-04 21:41:05.000000 apache-airflow-providers-ftp-3.5.0rc1/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 21:41:06.724097 apache-airflow-providers-ftp-3.5.0rc1/airflow/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 21:41:06.725152 apache-airflow-providers-ftp-3.5.0rc1/airflow/providers/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 21:41:06.759046 apache-airflow-providers-ftp-3.5.0rc1/airflow/providers/ftp/
+-rw-r--r--   0 root         (0) root         (0)     1572 2023-08-04 21:33:34.000000 apache-airflow-providers-ftp-3.5.0rc1/airflow/providers/ftp/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2786 2023-08-04 21:41:05.000000 apache-airflow-providers-ftp-3.5.0rc1/airflow/providers/ftp/get_provider_info.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 21:41:06.764593 apache-airflow-providers-ftp-3.5.0rc1/airflow/providers/ftp/hooks/
+-rw-r--r--   0 root         (0) root         (0)      787 2023-06-01 06:14:28.000000 apache-airflow-providers-ftp-3.5.0rc1/airflow/providers/ftp/hooks/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     9788 2023-06-29 05:49:30.000000 apache-airflow-providers-ftp-3.5.0rc1/airflow/providers/ftp/hooks/ftp.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 21:41:06.770158 apache-airflow-providers-ftp-3.5.0rc1/airflow/providers/ftp/operators/
+-rw-r--r--   0 root         (0) root         (0)      785 2023-06-01 06:14:28.000000 apache-airflow-providers-ftp-3.5.0rc1/airflow/providers/ftp/operators/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8151 2023-08-04 10:24:22.000000 apache-airflow-providers-ftp-3.5.0rc1/airflow/providers/ftp/operators/ftp.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 21:41:06.775764 apache-airflow-providers-ftp-3.5.0rc1/airflow/providers/ftp/sensors/
+-rw-r--r--   0 root         (0) root         (0)      787 2023-06-01 06:14:28.000000 apache-airflow-providers-ftp-3.5.0rc1/airflow/providers/ftp/sensors/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3364 2023-06-02 11:31:21.000000 apache-airflow-providers-ftp-3.5.0rc1/airflow/providers/ftp/sensors/ftp.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 21:41:06.799308 apache-airflow-providers-ftp-3.5.0rc1/apache_airflow_providers_ftp.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     5444 2023-08-04 21:41:06.000000 apache-airflow-providers-ftp-3.5.0rc1/apache_airflow_providers_ftp.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      750 2023-08-04 21:41:06.000000 apache-airflow-providers-ftp-3.5.0rc1/apache_airflow_providers_ftp.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-08-04 21:41:06.000000 apache-airflow-providers-ftp-3.5.0rc1/apache_airflow_providers_ftp.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      100 2023-08-04 21:41:06.000000 apache-airflow-providers-ftp-3.5.0rc1/apache_airflow_providers_ftp.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-08-04 21:41:06.000000 apache-airflow-providers-ftp-3.5.0rc1/apache_airflow_providers_ftp.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       79 2023-08-04 21:41:06.000000 apache-airflow-providers-ftp-3.5.0rc1/apache_airflow_providers_ftp.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-08-04 21:41:06.000000 apache-airflow-providers-ftp-3.5.0rc1/apache_airflow_providers_ftp.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     5031 2023-08-04 10:24:23.000000 apache-airflow-providers-ftp-3.5.0rc1/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)     1904 2023-08-04 21:41:06.804284 apache-airflow-providers-ftp-3.5.0rc1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1675 2023-08-04 21:41:05.000000 apache-airflow-providers-ftp-3.5.0rc1/setup.py
```

### Comparing `apache-airflow-providers-ftp-3.5.0/LICENSE` & `apache-airflow-providers-ftp-3.5.0rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-ftp-3.5.0/MANIFEST.in` & `apache-airflow-providers-ftp-3.5.0rc1/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-ftp-3.5.0/PKG-INFO` & `apache-airflow-providers-ftp-3.5.0rc1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-ftp
-Version: 3.5.0
+Version: 3.5.0rc1
 Summary: Provider for Apache Airflow. Implements apache-airflow-providers-ftp package
 Home-page: https://airflow.apache.org/
 Download-URL: https://archive.apache.org/dist/airflow/providers
 Author: Apache Software Foundation
 Author-email: dev@airflow.apache.org
 License: Apache License 2.0
 Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-ftp/3.5.0/
@@ -67,15 +67,15 @@
     KIND, either express or implied.  See the License for the
     specific language governing permissions and limitations
     under the License.
 
 
 Package ``apache-airflow-providers-ftp``
 
-Release: ``3.5.0``
+Release: ``3.5.0rc1``
 
 
 `File Transfer Protocol (FTP) <https://tools.ietf.org/html/rfc114>`__
 
 
 Provider package
 ----------------
```

### Comparing `apache-airflow-providers-ftp-3.5.0/README.rst` & `apache-airflow-providers-ftp-3.5.0rc1/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -32,15 +32,15 @@
     KIND, either express or implied.  See the License for the
     specific language governing permissions and limitations
     under the License.
 
 
 Package ``apache-airflow-providers-ftp``
 
-Release: ``3.5.0``
+Release: ``3.5.0rc1``
 
 
 `File Transfer Protocol (FTP) <https://tools.ietf.org/html/rfc114>`__
 
 
 Provider package
 ----------------
```

### Comparing `apache-airflow-providers-ftp-3.5.0/airflow/providers/ftp/__init__.py` & `apache-airflow-providers-ftp-3.5.0rc1/airflow/providers/ftp/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-ftp-3.5.0/airflow/providers/ftp/get_provider_info.py` & `apache-airflow-providers-ftp-3.5.0rc1/airflow/providers/ftp/get_provider_info.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-ftp-3.5.0/airflow/providers/ftp/hooks/__init__.py` & `apache-airflow-providers-ftp-3.5.0rc1/airflow/providers/ftp/hooks/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-ftp-3.5.0/airflow/providers/ftp/hooks/ftp.py` & `apache-airflow-providers-ftp-3.5.0rc1/airflow/providers/ftp/hooks/ftp.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-ftp-3.5.0/airflow/providers/ftp/operators/__init__.py` & `apache-airflow-providers-ftp-3.5.0rc1/airflow/providers/ftp/operators/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-ftp-3.5.0/airflow/providers/ftp/operators/ftp.py` & `apache-airflow-providers-ftp-3.5.0rc1/airflow/providers/ftp/operators/ftp.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-ftp-3.5.0/airflow/providers/ftp/sensors/__init__.py` & `apache-airflow-providers-ftp-3.5.0rc1/airflow/providers/ftp/sensors/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-ftp-3.5.0/airflow/providers/ftp/sensors/ftp.py` & `apache-airflow-providers-ftp-3.5.0rc1/airflow/providers/ftp/sensors/ftp.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-ftp-3.5.0/apache_airflow_providers_ftp.egg-info/PKG-INFO` & `apache-airflow-providers-ftp-3.5.0rc1/apache_airflow_providers_ftp.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-ftp
-Version: 3.5.0
+Version: 3.5.0rc1
 Summary: Provider for Apache Airflow. Implements apache-airflow-providers-ftp package
 Home-page: https://airflow.apache.org/
 Download-URL: https://archive.apache.org/dist/airflow/providers
 Author: Apache Software Foundation
 Author-email: dev@airflow.apache.org
 License: Apache License 2.0
 Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-ftp/3.5.0/
@@ -67,15 +67,15 @@
     KIND, either express or implied.  See the License for the
     specific language governing permissions and limitations
     under the License.
 
 
 Package ``apache-airflow-providers-ftp``
 
-Release: ``3.5.0``
+Release: ``3.5.0rc1``
 
 
 `File Transfer Protocol (FTP) <https://tools.ietf.org/html/rfc114>`__
 
 
 Provider package
 ----------------
```

### Comparing `apache-airflow-providers-ftp-3.5.0/apache_airflow_providers_ftp.egg-info/SOURCES.txt` & `apache-airflow-providers-ftp-3.5.0rc1/apache_airflow_providers_ftp.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-ftp-3.5.0/pyproject.toml` & `apache-airflow-providers-ftp-3.5.0rc1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-ftp-3.5.0/setup.cfg` & `apache-airflow-providers-ftp-3.5.0rc1/setup.cfg`

 * *Files 4% similar despite different names*

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
 	provider_info=airflow.providers.ftp.get_provider_info:get_provider_info
 
 [files]
 packages = airflow.providers.ftp
 
 [egg_info]
-tag_build = 
+tag_build = rc1
 tag_date = 0
```

### Comparing `apache-airflow-providers-ftp-3.5.0/setup.py` & `apache-airflow-providers-ftp-3.5.0rc1/setup.py`

 * *Files identical despite different names*


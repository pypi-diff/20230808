# Comparing `tmp/apache-airflow-providers-smtp-1.3.0.tar.gz` & `tmp/apache-airflow-providers-smtp-1.3.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apache-airflow-providers-smtp-1.3.0.tar", last modified: Fri Aug  4 21:35:56 2023, max compression
+gzip compressed data, was "apache-airflow-providers-smtp-1.3.0rc1.tar", last modified: Fri Aug  4 21:41:39 2023, max compression
```

## Comparing `apache-airflow-providers-smtp-1.3.0.tar` & `apache-airflow-providers-smtp-1.3.0rc1.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 21:35:56.681045 apache-airflow-providers-smtp-1.3.0/
--rw-r--r--   0 root         (0) root         (0)    10850 2023-06-01 06:14:29.000000 apache-airflow-providers-smtp-1.3.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)     1104 2023-08-04 21:35:55.000000 apache-airflow-providers-smtp-1.3.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      240 2023-06-01 06:14:29.000000 apache-airflow-providers-smtp-1.3.0/NOTICE
--rw-r--r--   0 root         (0) root         (0)     4385 2023-08-04 21:35:56.681608 apache-airflow-providers-smtp-1.3.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2758 2023-08-04 21:35:55.000000 apache-airflow-providers-smtp-1.3.0/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 21:35:56.594131 apache-airflow-providers-smtp-1.3.0/airflow/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 21:35:56.595245 apache-airflow-providers-smtp-1.3.0/airflow/providers/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 21:35:56.632015 apache-airflow-providers-smtp-1.3.0/airflow/providers/smtp/
--rw-r--r--   0 root         (0) root         (0)     1573 2023-08-04 21:33:34.000000 apache-airflow-providers-smtp-1.3.0/airflow/providers/smtp/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3972 2023-08-04 21:35:55.000000 apache-airflow-providers-smtp-1.3.0/airflow/providers/smtp/get_provider_info.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 21:35:56.637638 apache-airflow-providers-smtp-1.3.0/airflow/providers/smtp/hooks/
--rw-r--r--   0 root         (0) root         (0)      787 2023-06-01 06:14:29.000000 apache-airflow-providers-smtp-1.3.0/airflow/providers/smtp/hooks/__init__.py
--rw-r--r--   0 root         (0) root         (0)    14837 2023-08-04 19:44:14.000000 apache-airflow-providers-smtp-1.3.0/airflow/providers/smtp/hooks/smtp.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 21:35:56.643333 apache-airflow-providers-smtp-1.3.0/airflow/providers/smtp/notifications/
--rw-r--r--   0 root         (0) root         (0)      785 2023-06-08 05:42:54.000000 apache-airflow-providers-smtp-1.3.0/airflow/providers/smtp/notifications/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3374 2023-06-08 05:42:54.000000 apache-airflow-providers-smtp-1.3.0/airflow/providers/smtp/notifications/smtp.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 21:35:56.649020 apache-airflow-providers-smtp-1.3.0/airflow/providers/smtp/operators/
--rw-r--r--   0 root         (0) root         (0)      787 2023-06-01 06:14:29.000000 apache-airflow-providers-smtp-1.3.0/airflow/providers/smtp/operators/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3434 2023-06-01 06:14:29.000000 apache-airflow-providers-smtp-1.3.0/airflow/providers/smtp/operators/smtp.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 21:35:56.678687 apache-airflow-providers-smtp-1.3.0/apache_airflow_providers_smtp.egg-info/
--rw-r--r--   0 root         (0) root         (0)     4385 2023-08-04 21:35:56.000000 apache-airflow-providers-smtp-1.3.0/apache_airflow_providers_smtp.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      780 2023-08-04 21:35:56.000000 apache-airflow-providers-smtp-1.3.0/apache_airflow_providers_smtp.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-08-04 21:35:56.000000 apache-airflow-providers-smtp-1.3.0/apache_airflow_providers_smtp.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      101 2023-08-04 21:35:56.000000 apache-airflow-providers-smtp-1.3.0/apache_airflow_providers_smtp.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-08-04 21:35:56.000000 apache-airflow-providers-smtp-1.3.0/apache_airflow_providers_smtp.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       22 2023-08-04 21:35:56.000000 apache-airflow-providers-smtp-1.3.0/apache_airflow_providers_smtp.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-08-04 21:35:56.000000 apache-airflow-providers-smtp-1.3.0/apache_airflow_providers_smtp.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     5031 2023-08-04 10:24:23.000000 apache-airflow-providers-smtp-1.3.0/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)     1903 2023-08-04 21:35:56.683447 apache-airflow-providers-smtp-1.3.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1626 2023-08-04 21:35:55.000000 apache-airflow-providers-smtp-1.3.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 21:41:39.808899 apache-airflow-providers-smtp-1.3.0rc1/
+-rw-r--r--   0 root         (0) root         (0)    10850 2023-06-01 06:14:29.000000 apache-airflow-providers-smtp-1.3.0rc1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     1104 2023-08-04 21:41:38.000000 apache-airflow-providers-smtp-1.3.0rc1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      240 2023-06-01 06:14:29.000000 apache-airflow-providers-smtp-1.3.0rc1/NOTICE
+-rw-r--r--   0 root         (0) root         (0)     4391 2023-08-04 21:41:39.809493 apache-airflow-providers-smtp-1.3.0rc1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2761 2023-08-04 21:41:38.000000 apache-airflow-providers-smtp-1.3.0rc1/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 21:41:39.716441 apache-airflow-providers-smtp-1.3.0rc1/airflow/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 21:41:39.717645 apache-airflow-providers-smtp-1.3.0rc1/airflow/providers/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 21:41:39.759587 apache-airflow-providers-smtp-1.3.0rc1/airflow/providers/smtp/
+-rw-r--r--   0 root         (0) root         (0)     1573 2023-08-04 21:33:34.000000 apache-airflow-providers-smtp-1.3.0rc1/airflow/providers/smtp/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3972 2023-08-04 21:41:38.000000 apache-airflow-providers-smtp-1.3.0rc1/airflow/providers/smtp/get_provider_info.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 21:41:39.767041 apache-airflow-providers-smtp-1.3.0rc1/airflow/providers/smtp/hooks/
+-rw-r--r--   0 root         (0) root         (0)      787 2023-06-01 06:14:29.000000 apache-airflow-providers-smtp-1.3.0rc1/airflow/providers/smtp/hooks/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    14837 2023-08-04 19:44:14.000000 apache-airflow-providers-smtp-1.3.0rc1/airflow/providers/smtp/hooks/smtp.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 21:41:39.773894 apache-airflow-providers-smtp-1.3.0rc1/airflow/providers/smtp/notifications/
+-rw-r--r--   0 root         (0) root         (0)      785 2023-06-08 05:42:54.000000 apache-airflow-providers-smtp-1.3.0rc1/airflow/providers/smtp/notifications/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3374 2023-06-08 05:42:54.000000 apache-airflow-providers-smtp-1.3.0rc1/airflow/providers/smtp/notifications/smtp.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 21:41:39.780107 apache-airflow-providers-smtp-1.3.0rc1/airflow/providers/smtp/operators/
+-rw-r--r--   0 root         (0) root         (0)      787 2023-06-01 06:14:29.000000 apache-airflow-providers-smtp-1.3.0rc1/airflow/providers/smtp/operators/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3434 2023-06-01 06:14:29.000000 apache-airflow-providers-smtp-1.3.0rc1/airflow/providers/smtp/operators/smtp.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 21:41:39.806470 apache-airflow-providers-smtp-1.3.0rc1/apache_airflow_providers_smtp.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     4391 2023-08-04 21:41:39.000000 apache-airflow-providers-smtp-1.3.0rc1/apache_airflow_providers_smtp.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      780 2023-08-04 21:41:39.000000 apache-airflow-providers-smtp-1.3.0rc1/apache_airflow_providers_smtp.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-08-04 21:41:39.000000 apache-airflow-providers-smtp-1.3.0rc1/apache_airflow_providers_smtp.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      101 2023-08-04 21:41:39.000000 apache-airflow-providers-smtp-1.3.0rc1/apache_airflow_providers_smtp.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-08-04 21:41:39.000000 apache-airflow-providers-smtp-1.3.0rc1/apache_airflow_providers_smtp.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       27 2023-08-04 21:41:39.000000 apache-airflow-providers-smtp-1.3.0rc1/apache_airflow_providers_smtp.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-08-04 21:41:39.000000 apache-airflow-providers-smtp-1.3.0rc1/apache_airflow_providers_smtp.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     5031 2023-08-04 10:24:23.000000 apache-airflow-providers-smtp-1.3.0rc1/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)     1911 2023-08-04 21:41:39.811854 apache-airflow-providers-smtp-1.3.0rc1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1626 2023-08-04 21:41:38.000000 apache-airflow-providers-smtp-1.3.0rc1/setup.py
```

### Comparing `apache-airflow-providers-smtp-1.3.0/LICENSE` & `apache-airflow-providers-smtp-1.3.0rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-smtp-1.3.0/MANIFEST.in` & `apache-airflow-providers-smtp-1.3.0rc1/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-smtp-1.3.0/PKG-INFO` & `apache-airflow-providers-smtp-1.3.0rc1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-smtp
-Version: 1.3.0
+Version: 1.3.0rc1
 Summary: Provider for Apache Airflow. Implements apache-airflow-providers-smtp package
 Home-page: https://airflow.apache.org/
 Download-URL: https://archive.apache.org/dist/airflow/providers
 Author: Apache Software Foundation
 Author-email: dev@airflow.apache.org
 License: Apache License 2.0
 Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-smtp/1.3.0/
@@ -66,15 +66,15 @@
     KIND, either express or implied.  See the License for the
     specific language governing permissions and limitations
     under the License.
 
 
 Package ``apache-airflow-providers-smtp``
 
-Release: ``1.3.0``
+Release: ``1.3.0rc1``
 
 
 `Simple Mail Transfer Protocol (SMTP) <https://tools.ietf.org/html/rfc5321>`__
 
 
 Provider package
 ----------------
```

### Comparing `apache-airflow-providers-smtp-1.3.0/README.rst` & `apache-airflow-providers-smtp-1.3.0rc1/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -32,15 +32,15 @@
     KIND, either express or implied.  See the License for the
     specific language governing permissions and limitations
     under the License.
 
 
 Package ``apache-airflow-providers-smtp``
 
-Release: ``1.3.0``
+Release: ``1.3.0rc1``
 
 
 `Simple Mail Transfer Protocol (SMTP) <https://tools.ietf.org/html/rfc5321>`__
 
 
 Provider package
 ----------------
```

### Comparing `apache-airflow-providers-smtp-1.3.0/airflow/providers/smtp/__init__.py` & `apache-airflow-providers-smtp-1.3.0rc1/airflow/providers/smtp/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-smtp-1.3.0/airflow/providers/smtp/get_provider_info.py` & `apache-airflow-providers-smtp-1.3.0rc1/airflow/providers/smtp/get_provider_info.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-smtp-1.3.0/airflow/providers/smtp/hooks/__init__.py` & `apache-airflow-providers-smtp-1.3.0rc1/airflow/providers/smtp/hooks/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-smtp-1.3.0/airflow/providers/smtp/hooks/smtp.py` & `apache-airflow-providers-smtp-1.3.0rc1/airflow/providers/smtp/hooks/smtp.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-smtp-1.3.0/airflow/providers/smtp/notifications/__init__.py` & `apache-airflow-providers-smtp-1.3.0rc1/airflow/providers/smtp/notifications/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-smtp-1.3.0/airflow/providers/smtp/notifications/smtp.py` & `apache-airflow-providers-smtp-1.3.0rc1/airflow/providers/smtp/notifications/smtp.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-smtp-1.3.0/airflow/providers/smtp/operators/__init__.py` & `apache-airflow-providers-smtp-1.3.0rc1/airflow/providers/smtp/operators/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-smtp-1.3.0/airflow/providers/smtp/operators/smtp.py` & `apache-airflow-providers-smtp-1.3.0rc1/airflow/providers/smtp/operators/smtp.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-smtp-1.3.0/apache_airflow_providers_smtp.egg-info/PKG-INFO` & `apache-airflow-providers-smtp-1.3.0rc1/apache_airflow_providers_smtp.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-smtp
-Version: 1.3.0
+Version: 1.3.0rc1
 Summary: Provider for Apache Airflow. Implements apache-airflow-providers-smtp package
 Home-page: https://airflow.apache.org/
 Download-URL: https://archive.apache.org/dist/airflow/providers
 Author: Apache Software Foundation
 Author-email: dev@airflow.apache.org
 License: Apache License 2.0
 Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-smtp/1.3.0/
@@ -66,15 +66,15 @@
     KIND, either express or implied.  See the License for the
     specific language governing permissions and limitations
     under the License.
 
 
 Package ``apache-airflow-providers-smtp``
 
-Release: ``1.3.0``
+Release: ``1.3.0rc1``
 
 
 `Simple Mail Transfer Protocol (SMTP) <https://tools.ietf.org/html/rfc5321>`__
 
 
 Provider package
 ----------------
```

### Comparing `apache-airflow-providers-smtp-1.3.0/apache_airflow_providers_smtp.egg-info/SOURCES.txt` & `apache-airflow-providers-smtp-1.3.0rc1/apache_airflow_providers_smtp.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-smtp-1.3.0/pyproject.toml` & `apache-airflow-providers-smtp-1.3.0rc1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-smtp-1.3.0/setup.cfg` & `apache-airflow-providers-smtp-1.3.0rc1/setup.cfg`

 * *Files 1% similar despite different names*

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
 	provider_info=airflow.providers.smtp.get_provider_info:get_provider_info
 
 [files]
 packages = airflow.providers.smtp
 
 [egg_info]
-tag_build = 
+tag_build = rc1
 tag_date = 0
```

### Comparing `apache-airflow-providers-smtp-1.3.0/setup.py` & `apache-airflow-providers-smtp-1.3.0rc1/setup.py`

 * *Files identical despite different names*


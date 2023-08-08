# Comparing `tmp/apache-airflow-providers-docker-3.7.2.tar.gz` & `tmp/apache-airflow-providers-docker-3.7.2rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apache-airflow-providers-docker-3.7.2.tar", last modified: Fri Aug  4 21:35:22 2023, max compression
+gzip compressed data, was "apache-airflow-providers-docker-3.7.2rc1.tar", last modified: Fri Aug  4 21:41:03 2023, max compression
```

## Comparing `apache-airflow-providers-docker-3.7.2.tar` & `apache-airflow-providers-docker-3.7.2rc1.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 21:35:22.071254 apache-airflow-providers-docker-3.7.2/
--rw-r--r--   0 root         (0) root         (0)    10850 2023-06-01 06:14:29.000000 apache-airflow-providers-docker-3.7.2/LICENSE
--rw-r--r--   0 root         (0) root         (0)     1104 2023-08-04 21:35:20.000000 apache-airflow-providers-docker-3.7.2/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      240 2023-06-01 06:14:29.000000 apache-airflow-providers-docker-3.7.2/NOTICE
--rw-r--r--   0 root         (0) root         (0)     4437 2023-08-04 21:35:22.071836 apache-airflow-providers-docker-3.7.2/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2802 2023-08-04 21:35:20.000000 apache-airflow-providers-docker-3.7.2/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 21:35:21.988927 apache-airflow-providers-docker-3.7.2/airflow/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 21:35:21.989966 apache-airflow-providers-docker-3.7.2/airflow/providers/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 21:35:22.025727 apache-airflow-providers-docker-3.7.2/airflow/providers/docker/
--rw-r--r--   0 root         (0) root         (0)     1575 2023-08-04 21:33:34.000000 apache-airflow-providers-docker-3.7.2/airflow/providers/docker/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 21:35:22.031088 apache-airflow-providers-docker-3.7.2/airflow/providers/docker/decorators/
--rw-r--r--   0 root         (0) root         (0)      787 2023-06-01 06:14:28.000000 apache-airflow-providers-docker-3.7.2/airflow/providers/docker/decorators/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6806 2023-06-29 05:49:30.000000 apache-airflow-providers-docker-3.7.2/airflow/providers/docker/decorators/docker.py
--rw-r--r--   0 root         (0) root         (0)     3301 2023-08-04 21:35:20.000000 apache-airflow-providers-docker-3.7.2/airflow/providers/docker/get_provider_info.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 21:35:22.036527 apache-airflow-providers-docker-3.7.2/airflow/providers/docker/hooks/
--rw-r--r--   0 root         (0) root         (0)      787 2023-06-01 06:14:28.000000 apache-airflow-providers-docker-3.7.2/airflow/providers/docker/hooks/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7940 2023-06-02 11:31:21.000000 apache-airflow-providers-docker-3.7.2/airflow/providers/docker/hooks/docker.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 21:35:22.045064 apache-airflow-providers-docker-3.7.2/airflow/providers/docker/operators/
--rw-r--r--   0 root         (0) root         (0)      787 2023-06-01 06:14:28.000000 apache-airflow-providers-docker-3.7.2/airflow/providers/docker/operators/__init__.py
--rw-r--r--   0 root         (0) root         (0)    23409 2023-08-04 10:24:22.000000 apache-airflow-providers-docker-3.7.2/airflow/providers/docker/operators/docker.py
--rw-r--r--   0 root         (0) root         (0)     9637 2023-06-29 05:49:30.000000 apache-airflow-providers-docker-3.7.2/airflow/providers/docker/operators/docker_swarm.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 21:35:22.068382 apache-airflow-providers-docker-3.7.2/apache_airflow_providers_docker.egg-info/
--rw-r--r--   0 root         (0) root         (0)     4437 2023-08-04 21:35:21.000000 apache-airflow-providers-docker-3.7.2/apache_airflow_providers_docker.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      861 2023-08-04 21:35:21.000000 apache-airflow-providers-docker-3.7.2/apache_airflow_providers_docker.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-08-04 21:35:21.000000 apache-airflow-providers-docker-3.7.2/apache_airflow_providers_docker.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      103 2023-08-04 21:35:21.000000 apache-airflow-providers-docker-3.7.2/apache_airflow_providers_docker.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-08-04 21:35:21.000000 apache-airflow-providers-docker-3.7.2/apache_airflow_providers_docker.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       58 2023-08-04 21:35:21.000000 apache-airflow-providers-docker-3.7.2/apache_airflow_providers_docker.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-08-04 21:35:21.000000 apache-airflow-providers-docker-3.7.2/apache_airflow_providers_docker.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     5031 2023-08-04 10:24:23.000000 apache-airflow-providers-docker-3.7.2/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)     1955 2023-08-04 21:35:22.073758 apache-airflow-providers-docker-3.7.2/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1638 2023-08-04 21:35:20.000000 apache-airflow-providers-docker-3.7.2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 21:41:03.406999 apache-airflow-providers-docker-3.7.2rc1/
+-rw-r--r--   0 root         (0) root         (0)    10850 2023-06-01 06:14:29.000000 apache-airflow-providers-docker-3.7.2rc1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     1104 2023-08-04 21:41:02.000000 apache-airflow-providers-docker-3.7.2rc1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      240 2023-06-01 06:14:29.000000 apache-airflow-providers-docker-3.7.2rc1/NOTICE
+-rw-r--r--   0 root         (0) root         (0)     4443 2023-08-04 21:41:03.407724 apache-airflow-providers-docker-3.7.2rc1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2805 2023-08-04 21:41:02.000000 apache-airflow-providers-docker-3.7.2rc1/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 21:41:03.315339 apache-airflow-providers-docker-3.7.2rc1/airflow/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 21:41:03.316325 apache-airflow-providers-docker-3.7.2rc1/airflow/providers/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 21:41:03.351298 apache-airflow-providers-docker-3.7.2rc1/airflow/providers/docker/
+-rw-r--r--   0 root         (0) root         (0)     1575 2023-08-04 21:33:34.000000 apache-airflow-providers-docker-3.7.2rc1/airflow/providers/docker/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 21:41:03.358707 apache-airflow-providers-docker-3.7.2rc1/airflow/providers/docker/decorators/
+-rw-r--r--   0 root         (0) root         (0)      787 2023-06-01 06:14:28.000000 apache-airflow-providers-docker-3.7.2rc1/airflow/providers/docker/decorators/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6806 2023-06-29 05:49:30.000000 apache-airflow-providers-docker-3.7.2rc1/airflow/providers/docker/decorators/docker.py
+-rw-r--r--   0 root         (0) root         (0)     3301 2023-08-04 21:41:02.000000 apache-airflow-providers-docker-3.7.2rc1/airflow/providers/docker/get_provider_info.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 21:41:03.365745 apache-airflow-providers-docker-3.7.2rc1/airflow/providers/docker/hooks/
+-rw-r--r--   0 root         (0) root         (0)      787 2023-06-01 06:14:28.000000 apache-airflow-providers-docker-3.7.2rc1/airflow/providers/docker/hooks/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7940 2023-06-02 11:31:21.000000 apache-airflow-providers-docker-3.7.2rc1/airflow/providers/docker/hooks/docker.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 21:41:03.376606 apache-airflow-providers-docker-3.7.2rc1/airflow/providers/docker/operators/
+-rw-r--r--   0 root         (0) root         (0)      787 2023-06-01 06:14:28.000000 apache-airflow-providers-docker-3.7.2rc1/airflow/providers/docker/operators/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    23409 2023-08-04 10:24:22.000000 apache-airflow-providers-docker-3.7.2rc1/airflow/providers/docker/operators/docker.py
+-rw-r--r--   0 root         (0) root         (0)     9637 2023-06-29 05:49:30.000000 apache-airflow-providers-docker-3.7.2rc1/airflow/providers/docker/operators/docker_swarm.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 21:41:03.404133 apache-airflow-providers-docker-3.7.2rc1/apache_airflow_providers_docker.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     4443 2023-08-04 21:41:03.000000 apache-airflow-providers-docker-3.7.2rc1/apache_airflow_providers_docker.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      861 2023-08-04 21:41:03.000000 apache-airflow-providers-docker-3.7.2rc1/apache_airflow_providers_docker.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-08-04 21:41:03.000000 apache-airflow-providers-docker-3.7.2rc1/apache_airflow_providers_docker.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      103 2023-08-04 21:41:03.000000 apache-airflow-providers-docker-3.7.2rc1/apache_airflow_providers_docker.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-08-04 21:41:03.000000 apache-airflow-providers-docker-3.7.2rc1/apache_airflow_providers_docker.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       63 2023-08-04 21:41:03.000000 apache-airflow-providers-docker-3.7.2rc1/apache_airflow_providers_docker.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-08-04 21:41:03.000000 apache-airflow-providers-docker-3.7.2rc1/apache_airflow_providers_docker.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     5031 2023-08-04 10:24:23.000000 apache-airflow-providers-docker-3.7.2rc1/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)     1963 2023-08-04 21:41:03.410053 apache-airflow-providers-docker-3.7.2rc1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1638 2023-08-04 21:41:02.000000 apache-airflow-providers-docker-3.7.2rc1/setup.py
```

### Comparing `apache-airflow-providers-docker-3.7.2/LICENSE` & `apache-airflow-providers-docker-3.7.2rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-docker-3.7.2/MANIFEST.in` & `apache-airflow-providers-docker-3.7.2rc1/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-docker-3.7.2/PKG-INFO` & `apache-airflow-providers-docker-3.7.2rc1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-docker
-Version: 3.7.2
+Version: 3.7.2rc1
 Summary: Provider for Apache Airflow. Implements apache-airflow-providers-docker package
 Home-page: https://airflow.apache.org/
 Download-URL: https://archive.apache.org/dist/airflow/providers
 Author: Apache Software Foundation
 Author-email: dev@airflow.apache.org
 License: Apache License 2.0
 Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-docker/3.7.2/
@@ -66,15 +66,15 @@
     KIND, either express or implied.  See the License for the
     specific language governing permissions and limitations
     under the License.
 
 
 Package ``apache-airflow-providers-docker``
 
-Release: ``3.7.2``
+Release: ``3.7.2rc1``
 
 
 `Docker <https://docs.docker.com/install/>`__
 
 
 Provider package
 ----------------
```

### Comparing `apache-airflow-providers-docker-3.7.2/README.rst` & `apache-airflow-providers-docker-3.7.2rc1/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -32,15 +32,15 @@
     KIND, either express or implied.  See the License for the
     specific language governing permissions and limitations
     under the License.
 
 
 Package ``apache-airflow-providers-docker``
 
-Release: ``3.7.2``
+Release: ``3.7.2rc1``
 
 
 `Docker <https://docs.docker.com/install/>`__
 
 
 Provider package
 ----------------
```

### Comparing `apache-airflow-providers-docker-3.7.2/airflow/providers/docker/__init__.py` & `apache-airflow-providers-docker-3.7.2rc1/airflow/providers/docker/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-docker-3.7.2/airflow/providers/docker/decorators/__init__.py` & `apache-airflow-providers-docker-3.7.2rc1/airflow/providers/docker/decorators/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-docker-3.7.2/airflow/providers/docker/decorators/docker.py` & `apache-airflow-providers-docker-3.7.2rc1/airflow/providers/docker/decorators/docker.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-docker-3.7.2/airflow/providers/docker/get_provider_info.py` & `apache-airflow-providers-docker-3.7.2rc1/airflow/providers/docker/get_provider_info.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-docker-3.7.2/airflow/providers/docker/hooks/__init__.py` & `apache-airflow-providers-docker-3.7.2rc1/airflow/providers/docker/hooks/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-docker-3.7.2/airflow/providers/docker/hooks/docker.py` & `apache-airflow-providers-docker-3.7.2rc1/airflow/providers/docker/hooks/docker.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-docker-3.7.2/airflow/providers/docker/operators/__init__.py` & `apache-airflow-providers-docker-3.7.2rc1/airflow/providers/docker/operators/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-docker-3.7.2/airflow/providers/docker/operators/docker.py` & `apache-airflow-providers-docker-3.7.2rc1/airflow/providers/docker/operators/docker.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-docker-3.7.2/airflow/providers/docker/operators/docker_swarm.py` & `apache-airflow-providers-docker-3.7.2rc1/airflow/providers/docker/operators/docker_swarm.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-docker-3.7.2/apache_airflow_providers_docker.egg-info/PKG-INFO` & `apache-airflow-providers-docker-3.7.2rc1/apache_airflow_providers_docker.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-docker
-Version: 3.7.2
+Version: 3.7.2rc1
 Summary: Provider for Apache Airflow. Implements apache-airflow-providers-docker package
 Home-page: https://airflow.apache.org/
 Download-URL: https://archive.apache.org/dist/airflow/providers
 Author: Apache Software Foundation
 Author-email: dev@airflow.apache.org
 License: Apache License 2.0
 Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-docker/3.7.2/
@@ -66,15 +66,15 @@
     KIND, either express or implied.  See the License for the
     specific language governing permissions and limitations
     under the License.
 
 
 Package ``apache-airflow-providers-docker``
 
-Release: ``3.7.2``
+Release: ``3.7.2rc1``
 
 
 `Docker <https://docs.docker.com/install/>`__
 
 
 Provider package
 ----------------
```

### Comparing `apache-airflow-providers-docker-3.7.2/apache_airflow_providers_docker.egg-info/SOURCES.txt` & `apache-airflow-providers-docker-3.7.2rc1/apache_airflow_providers_docker.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-docker-3.7.2/pyproject.toml` & `apache-airflow-providers-docker-3.7.2rc1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-docker-3.7.2/setup.cfg` & `apache-airflow-providers-docker-3.7.2rc1/setup.cfg`

 * *Files 6% similar despite different names*

```diff
@@ -43,22 +43,22 @@
 include_package_data = True
 python_requires = ~=3.8
 packages = find:
 setup_requires = 
 	setuptools
 	wheel
 install_requires = 
-	apache-airflow>=2.4.0
+	apache-airflow>=2.4.0.dev0
 	docker>=5.0.3
 	python-dotenv>=0.21.0
 
 [options.entry_points]
 apache_airflow_provider = 
 	provider_info=airflow.providers.docker.get_provider_info:get_provider_info
 
 [files]
 packages = airflow.providers.docker
 
 [egg_info]
-tag_build = 
+tag_build = rc1
 tag_date = 0
```

### Comparing `apache-airflow-providers-docker-3.7.2/setup.py` & `apache-airflow-providers-docker-3.7.2rc1/setup.py`

 * *Files identical despite different names*

